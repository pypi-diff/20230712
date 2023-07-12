# Comparing `tmp/ampligraph-2.0.0-py3-none-any.whl.zip` & `tmp/ampligraph-2.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,71 +1,73 @@
-Zip file size: 178256 bytes, number of entries: 69
--rw-r--r--  2.0 unx      679 b- defN 23-Mar-07 18:31 ampligraph/__init__.py
+Zip file size: 204048 bytes, number of entries: 71
+-rw-r--r--  2.0 unx      679 b- defN 23-Jul-12 15:48 ampligraph/__init__.py
 -rw-r--r--  2.0 unx      506 b- defN 22-Nov-23 14:09 ampligraph/logger.conf
--rw-r--r--  2.0 unx      473 b- defN 23-Mar-07 18:30 ampligraph/compat/__init__.py
--rw-r--r--  2.0 unx     7534 b- defN 23-Mar-07 18:30 ampligraph/compat/evaluate.py
--rw-r--r--  2.0 unx    29377 b- defN 23-Mar-07 18:30 ampligraph/compat/models.py
--rw-r--r--  2.0 unx     1533 b- defN 23-Mar-07 18:30 ampligraph/datasets/__init__.py
--rw-r--r--  2.0 unx     4961 b- defN 23-Mar-07 18:30 ampligraph/datasets/data_adapter.py
--rw-r--r--  2.0 unx    64485 b- defN 23-Mar-07 18:30 ampligraph/datasets/data_indexer.py
--rw-r--r--  2.0 unx    74774 b- defN 23-Mar-07 18:30 ampligraph/datasets/datasets.py
--rw-r--r--  2.0 unx    35488 b- defN 23-Mar-07 18:30 ampligraph/datasets/graph_data_loader.py
--rw-r--r--  2.0 unx    32263 b- defN 23-Mar-07 18:30 ampligraph/datasets/graph_partitioner.py
--rw-r--r--  2.0 unx    38764 b- defN 23-Mar-07 18:30 ampligraph/datasets/partitioned_data_manager.py
--rw-r--r--  2.0 unx    15810 b- defN 23-Mar-07 18:30 ampligraph/datasets/partitioning_reporter.py
--rw-r--r--  2.0 unx     5677 b- defN 23-Mar-07 18:30 ampligraph/datasets/source_identifier.py
--rw-r--r--  2.0 unx    34921 b- defN 23-Mar-07 18:30 ampligraph/datasets/sqlite_adapter.py
--rw-r--r--  2.0 unx     1057 b- defN 23-Mar-07 18:30 ampligraph/discovery/__init__.py
--rw-r--r--  2.0 unx    45346 b- defN 23-Mar-07 18:30 ampligraph/discovery/discovery.py
--rw-r--r--  2.0 unx      848 b- defN 23-Mar-07 18:30 ampligraph/evaluation/__init__.py
--rw-r--r--  2.0 unx     7823 b- defN 23-Mar-07 18:30 ampligraph/evaluation/metrics.py
--rw-r--r--  2.0 unx    31224 b- defN 23-Mar-07 18:30 ampligraph/evaluation/protocol.py
--rw-r--r--  2.0 unx     1172 b- defN 23-Mar-07 18:30 ampligraph/latent_features/__init__.py
--rw-r--r--  2.0 unx    24974 b- defN 23-Mar-07 18:30 ampligraph/latent_features/loss_functions.py
--rw-r--r--  2.0 unx     7263 b- defN 23-Mar-07 18:30 ampligraph/latent_features/optimizers.py
--rw-r--r--  2.0 unx     2295 b- defN 23-Mar-07 18:30 ampligraph/latent_features/regularizers.py
--rw-r--r--  2.0 unx      315 b- defN 23-Mar-07 18:30 ampligraph/latent_features/layers/__init__.py
--rw-r--r--  2.0 unx      313 b- defN 23-Mar-07 18:30 ampligraph/latent_features/layers/calibration/__init__.py
--rw-r--r--  2.0 unx     4151 b- defN 23-Mar-07 18:30 ampligraph/latent_features/layers/calibration/calibrate.py
--rw-r--r--  2.0 unx     3474 b- defN 23-Mar-07 18:30 ampligraph/latent_features/layers/corruption_generation/CorruptionGenerationLayerTrain.py
--rw-r--r--  2.0 unx      362 b- defN 23-Mar-07 18:30 ampligraph/latent_features/layers/corruption_generation/__init__.py
--rw-r--r--  2.0 unx    12594 b- defN 23-Mar-07 18:30 ampligraph/latent_features/layers/encoding/EmbeddingLookupLayer.py
--rw-r--r--  2.0 unx      332 b- defN 23-Mar-07 18:30 ampligraph/latent_features/layers/encoding/__init__.py
--rw-r--r--  2.0 unx    16689 b- defN 23-Mar-07 18:30 ampligraph/latent_features/layers/scoring/AbstractScoringLayer.py
--rw-r--r--  2.0 unx     5339 b- defN 23-Mar-07 18:30 ampligraph/latent_features/layers/scoring/ComplEx.py
--rw-r--r--  2.0 unx     3413 b- defN 23-Mar-07 18:30 ampligraph/latent_features/layers/scoring/DistMult.py
--rw-r--r--  2.0 unx     2784 b- defN 23-Mar-07 18:30 ampligraph/latent_features/layers/scoring/HolE.py
--rw-r--r--  2.0 unx     2510 b- defN 23-Mar-07 18:30 ampligraph/latent_features/layers/scoring/Random.py
--rw-r--r--  2.0 unx     3969 b- defN 23-Mar-07 18:30 ampligraph/latent_features/layers/scoring/TransE.py
--rw-r--r--  2.0 unx      441 b- defN 23-Mar-07 18:30 ampligraph/latent_features/layers/scoring/__init__.py
--rw-r--r--  2.0 unx    93355 b- defN 23-Mar-07 18:30 ampligraph/latent_features/models/ScoringBasedEmbeddingModel.py
--rw-r--r--  2.0 unx      350 b- defN 23-Mar-07 18:30 ampligraph/latent_features/models/__init__.py
--rw-r--r--  2.0 unx      703 b- defN 23-Mar-07 18:30 ampligraph/utils/__init__.py
--rw-r--r--  2.0 unx    15606 b- defN 23-Mar-07 18:30 ampligraph/utils/model_utils.py
--rw-r--r--  2.0 unx     2841 b- defN 23-Mar-07 18:30 ampligraph/utils/profiling.py
--rw-r--r--  2.0 unx     2298 b- defN 23-Mar-07 18:30 ampligraph/utils/tags.py
--rw-r--r--  2.0 unx      241 b- defN 23-Mar-07 18:30 tests/ampligraph/__init__.py
--rw-r--r--  2.0 unx      241 b- defN 23-Mar-07 18:30 tests/ampligraph/datasets/__init__.py
--rw-r--r--  2.0 unx     2935 b- defN 23-Mar-07 17:50 tests/ampligraph/datasets/test_data_indexer.py
--rw-r--r--  2.0 unx     7161 b- defN 23-Mar-07 17:50 tests/ampligraph/datasets/test_datasets.py
--rw-r--r--  2.0 unx     4585 b- defN 23-Mar-07 17:50 tests/ampligraph/datasets/test_graph_data_loader.py
--rw-r--r--  2.0 unx     8582 b- defN 23-Mar-07 17:50 tests/ampligraph/datasets/test_graph_partitioner.py
--rw-r--r--  2.0 unx     4936 b- defN 23-Mar-07 17:50 tests/ampligraph/datasets/test_partitioning_reporter.py
--rw-r--r--  2.0 unx     2430 b- defN 23-Mar-07 17:50 tests/ampligraph/datasets/test_source_identifier.py
--rw-r--r--  2.0 unx     1368 b- defN 23-Mar-07 17:50 tests/ampligraph/datasets/test_sqlite_adapter.py
--rw-r--r--  2.0 unx      240 b- defN 23-Mar-07 17:50 tests/ampligraph/discovery/__init__.py
--rw-r--r--  2.0 unx    12382 b- defN 23-Mar-07 17:50 tests/ampligraph/discovery/test_discovery.py
--rw-r--r--  2.0 unx      240 b- defN 23-Mar-07 17:50 tests/ampligraph/evaluation/__init__.py
--rw-r--r--  2.0 unx     5343 b- defN 23-Mar-07 17:50 tests/ampligraph/evaluation/test_evaluate.py
--rw-r--r--  2.0 unx      240 b- defN 23-Mar-07 17:50 tests/ampligraph/latent_features/__init__.py
--rw-r--r--  2.0 unx     2121 b- defN 23-Mar-07 17:50 tests/ampligraph/latent_features/test_initializers.py
--rw-r--r--  2.0 unx     8632 b- defN 23-Mar-07 17:50 tests/ampligraph/latent_features/test_loss_functions.py
--rw-r--r--  2.0 unx     3198 b- defN 23-Mar-07 17:50 tests/ampligraph/latent_features/test_optimizers.py
--rw-r--r--  2.0 unx     1519 b- defN 23-Mar-07 17:50 tests/ampligraph/latent_features/test_regularizer.py
--rw-r--r--  2.0 unx      242 b- defN 23-Mar-07 17:50 tests/ampligraph/utils/__init__.py
--rw-r--r--  2.0 unx     1257 b- defN 23-Mar-07 17:50 tests/ampligraph/utils/test_profiling.py
--rwxr-xr-x  2.0 unx    11351 b- defN 23-Mar-08 12:03 ampligraph-2.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1033 b- defN 23-Mar-08 12:03 ampligraph-2.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-08 12:03 ampligraph-2.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Mar-08 12:03 ampligraph-2.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6818 b- defN 23-Mar-08 12:03 ampligraph-2.0.0.dist-info/RECORD
-69 files, 728290 bytes uncompressed, 167104 bytes compressed:  77.1%
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-12 11:04 ampligraph/compat/__init__.py
+-rw-r--r--  2.0 unx     7534 b- defN 23-Jul-12 11:04 ampligraph/compat/evaluate.py
+-rw-r--r--  2.0 unx    29377 b- defN 23-Jul-12 11:04 ampligraph/compat/models.py
+-rw-r--r--  2.0 unx     1533 b- defN 23-Jul-12 11:04 ampligraph/datasets/__init__.py
+-rw-r--r--  2.0 unx     4961 b- defN 23-Jul-12 11:04 ampligraph/datasets/data_adapter.py
+-rw-r--r--  2.0 unx    64717 b- defN 23-Jul-12 15:48 ampligraph/datasets/data_indexer.py
+-rw-r--r--  2.0 unx    74882 b- defN 23-Jul-12 15:48 ampligraph/datasets/datasets.py
+-rw-r--r--  2.0 unx    35727 b- defN 23-Jul-12 15:48 ampligraph/datasets/graph_data_loader.py
+-rw-r--r--  2.0 unx    32263 b- defN 23-Jul-12 11:04 ampligraph/datasets/graph_partitioner.py
+-rw-r--r--  2.0 unx    38764 b- defN 23-Jul-12 11:04 ampligraph/datasets/partitioned_data_manager.py
+-rw-r--r--  2.0 unx    15810 b- defN 23-Jul-12 11:04 ampligraph/datasets/partitioning_reporter.py
+-rw-r--r--  2.0 unx     5677 b- defN 23-Jul-12 11:04 ampligraph/datasets/source_identifier.py
+-rw-r--r--  2.0 unx    34921 b- defN 23-Jul-12 11:04 ampligraph/datasets/sqlite_adapter.py
+-rw-r--r--  2.0 unx     1112 b- defN 23-Jul-12 15:48 ampligraph/discovery/__init__.py
+-rw-r--r--  2.0 unx    49019 b- defN 23-Jul-12 15:48 ampligraph/discovery/discovery.py
+-rw-r--r--  2.0 unx      848 b- defN 23-Jul-12 11:04 ampligraph/evaluation/__init__.py
+-rw-r--r--  2.0 unx     7883 b- defN 23-Jul-12 15:48 ampligraph/evaluation/metrics.py
+-rw-r--r--  2.0 unx    31276 b- defN 23-Jul-12 11:04 ampligraph/evaluation/protocol.py
+-rw-r--r--  2.0 unx     1172 b- defN 23-Jul-12 11:04 ampligraph/latent_features/__init__.py
+-rw-r--r--  2.0 unx    24974 b- defN 23-Jul-12 11:04 ampligraph/latent_features/loss_functions.py
+-rw-r--r--  2.0 unx     7263 b- defN 23-Jul-12 11:04 ampligraph/latent_features/optimizers.py
+-rw-r--r--  2.0 unx     2295 b- defN 23-Jul-12 11:04 ampligraph/latent_features/regularizers.py
+-rw-r--r--  2.0 unx      315 b- defN 23-Jul-12 11:04 ampligraph/latent_features/layers/__init__.py
+-rw-r--r--  2.0 unx      313 b- defN 23-Jul-12 11:04 ampligraph/latent_features/layers/calibration/__init__.py
+-rw-r--r--  2.0 unx     4064 b- defN 23-Jul-12 15:48 ampligraph/latent_features/layers/calibration/calibrate.py
+-rw-r--r--  2.0 unx     3474 b- defN 23-Jul-12 11:04 ampligraph/latent_features/layers/corruption_generation/CorruptionGenerationLayerTrain.py
+-rw-r--r--  2.0 unx      362 b- defN 23-Jul-12 11:04 ampligraph/latent_features/layers/corruption_generation/__init__.py
+-rw-r--r--  2.0 unx    13633 b- defN 23-Jul-12 15:48 ampligraph/latent_features/layers/encoding/EmbeddingLookupLayer.py
+-rw-r--r--  2.0 unx      332 b- defN 23-Jul-12 11:04 ampligraph/latent_features/layers/encoding/__init__.py
+-rw-r--r--  2.0 unx    16689 b- defN 23-Jul-12 11:04 ampligraph/latent_features/layers/scoring/AbstractScoringLayer.py
+-rw-r--r--  2.0 unx     5339 b- defN 23-Jul-12 11:04 ampligraph/latent_features/layers/scoring/ComplEx.py
+-rw-r--r--  2.0 unx     3413 b- defN 23-Jul-12 11:04 ampligraph/latent_features/layers/scoring/DistMult.py
+-rw-r--r--  2.0 unx     2784 b- defN 23-Jul-12 11:04 ampligraph/latent_features/layers/scoring/HolE.py
+-rw-r--r--  2.0 unx     2510 b- defN 23-Jul-12 11:04 ampligraph/latent_features/layers/scoring/Random.py
+-rw-r--r--  2.0 unx     6275 b- defN 23-Apr-17 14:25 ampligraph/latent_features/layers/scoring/RotatE.py
+-rw-r--r--  2.0 unx     3969 b- defN 23-Jul-12 11:04 ampligraph/latent_features/layers/scoring/TransE.py
+-rw-r--r--  2.0 unx      441 b- defN 23-Jul-12 11:04 ampligraph/latent_features/layers/scoring/__init__.py
+-rw-r--r--  2.0 unx    99848 b- defN 23-May-04 09:11 ampligraph/latent_features/models/NodePiece.py
+-rw-r--r--  2.0 unx    93678 b- defN 23-Jul-12 15:48 ampligraph/latent_features/models/ScoringBasedEmbeddingModel.py
+-rw-r--r--  2.0 unx      350 b- defN 23-Jul-12 11:04 ampligraph/latent_features/models/__init__.py
+-rw-r--r--  2.0 unx      703 b- defN 23-Jul-12 11:04 ampligraph/utils/__init__.py
+-rw-r--r--  2.0 unx    15516 b- defN 23-Jul-12 15:48 ampligraph/utils/model_utils.py
+-rw-r--r--  2.0 unx     2841 b- defN 23-Jul-12 11:04 ampligraph/utils/profiling.py
+-rw-r--r--  2.0 unx     2298 b- defN 23-Jul-12 11:04 ampligraph/utils/tags.py
+-rw-r--r--  2.0 unx      241 b- defN 23-Jul-12 11:04 tests/ampligraph/__init__.py
+-rw-r--r--  2.0 unx      241 b- defN 23-Jul-12 11:04 tests/ampligraph/datasets/__init__.py
+-rw-r--r--  2.0 unx     2935 b- defN 23-Jul-12 11:04 tests/ampligraph/datasets/test_data_indexer.py
+-rw-r--r--  2.0 unx     7171 b- defN 23-Jul-12 11:04 tests/ampligraph/datasets/test_datasets.py
+-rw-r--r--  2.0 unx     4585 b- defN 23-Jul-12 11:04 tests/ampligraph/datasets/test_graph_data_loader.py
+-rw-r--r--  2.0 unx     8582 b- defN 23-Jul-12 11:04 tests/ampligraph/datasets/test_graph_partitioner.py
+-rw-r--r--  2.0 unx     4936 b- defN 23-Jul-12 11:04 tests/ampligraph/datasets/test_partitioning_reporter.py
+-rw-r--r--  2.0 unx     2430 b- defN 23-Jul-12 11:04 tests/ampligraph/datasets/test_source_identifier.py
+-rw-r--r--  2.0 unx     1368 b- defN 23-Jul-12 11:04 tests/ampligraph/datasets/test_sqlite_adapter.py
+-rw-r--r--  2.0 unx      240 b- defN 23-Jul-12 11:04 tests/ampligraph/discovery/__init__.py
+-rw-r--r--  2.0 unx    12382 b- defN 23-Jul-12 11:04 tests/ampligraph/discovery/test_discovery.py
+-rw-r--r--  2.0 unx      240 b- defN 23-Jul-12 11:04 tests/ampligraph/evaluation/__init__.py
+-rw-r--r--  2.0 unx     5343 b- defN 23-Jul-12 11:04 tests/ampligraph/evaluation/test_evaluate.py
+-rw-r--r--  2.0 unx      240 b- defN 23-Jul-12 11:04 tests/ampligraph/latent_features/__init__.py
+-rw-r--r--  2.0 unx     2121 b- defN 23-Jul-12 11:04 tests/ampligraph/latent_features/test_initializers.py
+-rw-r--r--  2.0 unx     8632 b- defN 23-Jul-12 11:04 tests/ampligraph/latent_features/test_loss_functions.py
+-rw-r--r--  2.0 unx     3198 b- defN 23-Jul-12 11:04 tests/ampligraph/latent_features/test_optimizers.py
+-rw-r--r--  2.0 unx     1519 b- defN 23-Jul-12 11:04 tests/ampligraph/latent_features/test_regularizer.py
+-rw-r--r--  2.0 unx      242 b- defN 23-Jul-12 11:04 tests/ampligraph/utils/__init__.py
+-rw-r--r--  2.0 unx     1257 b- defN 23-Jul-12 11:04 tests/ampligraph/utils/test_profiling.py
+-rwxr-xr-x  2.0 unx    11356 b- defN 23-Jul-12 18:03 ampligraph-2.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      972 b- defN 23-Jul-12 18:03 ampligraph-2.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 18:03 ampligraph-2.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-12 18:03 ampligraph-2.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     7029 b- defN 23-Jul-12 18:03 ampligraph-2.0.1.dist-info/RECORD
+71 files, 840182 bytes uncompressed, 192550 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -102,20 +102,26 @@
 
 Filename: ampligraph/latent_features/layers/scoring/HolE.py
 Comment: 
 
 Filename: ampligraph/latent_features/layers/scoring/Random.py
 Comment: 
 
+Filename: ampligraph/latent_features/layers/scoring/RotatE.py
+Comment: 
+
 Filename: ampligraph/latent_features/layers/scoring/TransE.py
 Comment: 
 
 Filename: ampligraph/latent_features/layers/scoring/__init__.py
 Comment: 
 
+Filename: ampligraph/latent_features/models/NodePiece.py
+Comment: 
+
 Filename: ampligraph/latent_features/models/ScoringBasedEmbeddingModel.py
 Comment: 
 
 Filename: ampligraph/latent_features/models/__init__.py
 Comment: 
 
 Filename: ampligraph/utils/__init__.py
@@ -186,23 +192,23 @@
 
 Filename: tests/ampligraph/utils/__init__.py
 Comment: 
 
 Filename: tests/ampligraph/utils/test_profiling.py
 Comment: 
 
-Filename: ampligraph-2.0.0.dist-info/LICENSE
+Filename: ampligraph-2.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: ampligraph-2.0.0.dist-info/METADATA
+Filename: ampligraph-2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: ampligraph-2.0.0.dist-info/WHEEL
+Filename: ampligraph-2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: ampligraph-2.0.0.dist-info/top_level.txt
+Filename: ampligraph-2.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ampligraph-2.0.0.dist-info/RECORD
+Filename: ampligraph-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ampligraph/__init__.py

```diff
@@ -9,14 +9,14 @@
 import logging.config
 
 import pkg_resources
 import tensorflow as tf
 
 tf.compat.v1.logging.set_verbosity(tf.compat.v1.logging.ERROR)
 
-__version__ = '2.0.0'
+__version__ = '2.0.1'
 __all__ = ['datasets', 'latent_features', 'discovery', 'evaluation', 'utils']
 
 logging.config.fileConfig(
     pkg_resources.resource_filename(__name__, "logger.conf"),
     disable_existing_loggers=False,
 )
```

## ampligraph/datasets/data_indexer.py

```diff
@@ -558,27 +558,32 @@
             raise Exception(msg)
 
         if entities is None and relations is None:
             msg = "Requested entities and relations mappings are empty."
             logger.error(msg)
             raise Exception(msg)
 
+        elements = []
         if type_of == "e":
-            elements = np.array([entities[x] for x in sample], dtype=dtype)
-            return elements
+            elements = np.array([entities[x] for x in sample if x in entities.keys()], dtype=dtype)
         elif type_of == "r":
-            elements = np.array([relations[x] for x in sample], dtype=dtype)
-            return elements
+            elements = np.array([relations[x] for x in sample if x in relations.keys()], dtype=dtype)
         else:
             if type_of not in ["r", "e"]:
                 msg = "No such option, should be r (relations) or e (entities), instead got {}".format(
                     type_of
                 )
                 logger.error(msg)
                 raise Exception(msg)
+        invalid_keys = len(sample) - len(elements)
+        if invalid_keys > 0:
+            print(
+                "\n{} entities with invalid keys skipped!".format(invalid_keys)
+            )
+        return elements
 
     def get_relations_count(self):
         """Get number of unique relations."""
         return len(self.relations_dict)
 
     def get_entities_count(self):
         """Get number of unique entities."""
```

## ampligraph/datasets/datasets.py

```diff
@@ -311,15 +311,16 @@
     cols[0], cols[2] = cols[2], cols[0]
     df_reciprocal.columns = cols
 
     # add reciprocal relations
     df_reciprocal.iloc[:, 1] = df_reciprocal.iloc[:, 1] + "_reciprocal"
 
     # append to original triples
-    triples_df = triples_df.append(df_reciprocal)
+    triples_df = pd.concat([triples_df, df_reciprocal])
+
     return triples_df
 
 
 def load_from_csv(
     directory_path, file_name, sep="\t", header=None, add_reciprocal_rels=False
 ):
     """Load a knowledge graph from a .csv file.
@@ -1295,14 +1296,17 @@
         sep=" ",
         header=None,
         names=None,
         dtype=str,
         usecols=[0, 1, 2],
     )
 
+    # Remove trailing full stop (if present)
+    df[2] = df[2].apply(lambda x: x.rsplit(".", 1)[0])
+
     if add_reciprocal_rels:
         df = _add_reciprocal_relations(df)
 
     return df.values
 
 
 # FocusE
```

## ampligraph/datasets/graph_data_loader.py

```diff
@@ -13,14 +13,15 @@
 """
 import logging
 import tempfile
 import uuid
 from datetime import datetime
 
 import numpy as np
+import pandas as pd
 import tensorflow as tf
 
 from .data_indexer import DataIndexer
 from .source_identifier import DataSourceIdentifier
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
@@ -118,14 +119,20 @@
              Kind of data to be loaded (`"train"` | `"test"` | `"validation"`).
         """
         logger.debug(
             "Simple in-memory data loading of {} dataset.".format(dataset_type)
         )
         self.data_source = data_source
         self.dataset_type = dataset_type
+
+        if isinstance(self.data_source, pd.DataFrame):
+            self.data_source = self.data_source.values
+        elif isinstance(self.data_source, list):
+            self.data_source = np.array(self.data_source)
+
         if isinstance(self.data_source, np.ndarray):
             if self.use_indexer is True:
                 self.mapper = DataIndexer(
                     self.data_source,
                     backend="in_memory" if self.in_memory else "sqlite",
                     root_directory=self.root_directory,
                 )
```

## ampligraph/discovery/__init__.py

```diff
@@ -20,10 +20,11 @@
 """
 
 from .discovery import (
     discover_facts,
     find_clusters,
     find_duplicates,
     query_topn,
+    find_nearest_neighbours
 )
 
-__all__ = ["discover_facts", "find_clusters", "find_duplicates", "query_topn"]
+__all__ = ["discover_facts", "find_clusters", "find_duplicates", "query_topn", "find_nearest_neighbours"]
```

## ampligraph/discovery/discovery.py

```diff
@@ -26,63 +26,71 @@
     max_candidates=100,
     target_rel=None,
     seed=0,
 ):
     """
     Discover new facts from an existing knowledge graph.
 
-    You should use this function when you already have a model trained on a knowledge graph and you want to
-    discover potentially true statements in that knowledge graph.
+    You should use this function when you already have a model trained on a knowledge graph
+    and you want to discover potentially true statements in that knowledge graph.
 
-    The general procedure of this function is to generate a set of candidate statements :math:`C` according to some
-    sampling strategy ``strategy``, then rank them against a set of corruptions using the
-    :meth:`ampligraph.evaluation.evaluate_performance` function.
-    Candidates that appear in the ``top_n`` ranked statements of this procedure are returned as likely true
-    statements.
+    The general procedure of this function is to generate a set of candidate statements
+    :math:`C` according to some sampling strategy ``strategy``, then rank them against a set
+    of corruptions using the :meth:`ampligraph.latent_features.ScoringBasedEmbeddingModel.evaluate`
+    method.
+    Candidates that appear in the ``top_n`` ranked statements of this procedure are returned
+    as likely true statements.
 
-    The majority of the strategies are implemented with the same underlying principle of searching for
-    candidate statements:
+    The majority of the strategies are implemented with the same underlying principle of
+    searching for candidate statements:
 
     - from among the less frequent entities (`'entity_frequency'`),
     - less connected entities (`'graph_degree'`, `'cluster_coefficient'`),
-    - | less frequent local graph structures (`'cluster_triangles'`, `'cluster_squares'`), on the assumption that
-        densely connected entities are less likely to have missing true statements.
-    - | The remaining strategies (`'random_uniform'`, `'exhaustive'`) generate candidate statements by a random
-        sampling of entities and relations or exhaustively, respectively.
+    - | less frequent local graph structures (`'cluster_triangles'`, `'cluster_squares'`),
+        on the assumption that densely connected entities are less likely to have missing
+        true statements.
+    - | The remaining strategies (`'random_uniform'`, `'exhaustive'`) generate candidate
+        statements by a random sampling of entities and relations or exhaustively, respectively.
 
     .. warning::
-        Due to the significant amount of computation required to evaluate all triples using the 'exhaustive' strategy,
-        we do not recommend its use at this time.
+        Due to the significant amount of computation required to evaluate all triples using
+        the 'exhaustive' strategy, we do not recommend its use at this time.
 
-    The function will automatically filter entities that have not been seen by the model, and operates on
-    the assumption that the model provided has been fit on the data ``X`` (determined heuristically), although ``X``
-    may be a subset of the original data, in which case a warning is shown.
+    The function will automatically filter entities that have not been seen by the model,
+    and operates on the assumption that the model provided has been fit on the data ``X``
+    (determined heuristically), although ``X`` may be a subset of the original data, in
+    which case a warning is shown.
 
-    The ``target_rel`` argument indicates what relation to generate candidate statements for. If this is set to ``None``
-    then all target relations will be considered for sampling.
+    The ``target_rel`` argument indicates what relation to generate candidate statements for.
+    If this is set to ``None`` then all target relations will be considered for sampling.
 
     Parameters
     ----------
 
     X : ndarray of shape (n, 3)
         The input knowledge graph used to train ``model``, or a subset of it.
     model : EmbeddingModel
         The trained model that will be used to score candidate facts.
     top_n : int
         The cutoff position in ranking to consider a candidate triple as true positive.
     strategy: str
         The candidates generation strategy:
 
-        - `'random_uniform'` : generates `N` candidates (:math:`N <= max_candidates`) based on a uniform sampling of
-            entities.
-        - `'entity_frequency'` : generates candidates by weighted sampling of entities using entity frequency.
-        - `'graph_degree'` : generates candidates by weighted sampling of entities with graph degree.
-        - `'cluster_coefficient'` : generates candidates by weighted sampling entities with clustering coefficient.
-        - `'cluster_triangles'` : generates candidates by weighted sampling entities with cluster triangles.
-        - `'cluster_squares'` : generates candidates by weighted sampling entities with cluster squares.
+        - `'random_uniform'` : generates `N` candidates (:math:`N <= max_candidates`) based on
+            a uniform sampling of entities.
+        - `'entity_frequency'` : generates candidates by weighted sampling of entities using
+            entity frequency.
+        - `'graph_degree'` : generates candidates by weighted sampling of entities with
+            graph degree.
+        - `'cluster_coefficient'` : generates candidates by weighted sampling entities
+            with clustering coefficient.
+        - `'cluster_triangles'` : generates candidates by weighted sampling entities
+            with cluster triangles.
+        - `'cluster_squares'` : generates candidates by weighted sampling entities
+            with cluster squares.
 
     max_candidates: int or float
         The maximum numbers of candidates generated by ``strategy``.
         Can be an absolute number or a percentage [0,1] of the size of the `X` parameter.
     target_rel : str or list(str)
         Target relations to focus on. The function will discover facts only for that specific relation types.
         If `None`, the function attempts to discover new facts for all relation types in the graph.
@@ -100,26 +108,26 @@
     >>> import requests
     >>> from ampligraph.latent_features import ScoringBasedEmbeddingModel
     >>> from ampligraph.datasets import load_from_csv
     >>> from ampligraph.discovery import discover_facts
     >>> # Game of Thrones relations dataset
     >>> url = 'https://ampligraph.s3-eu-west-1.amazonaws.com/datasets/GoT.csv'
     >>> open('GoT.csv', 'wb').write(requests.get(url).content)
-    >>> X = load_from_csv('.', 'GoT.csv', sep=',')
+    >>> dataset = load_from_csv('.', 'GoT.csv', sep=',')
     >>> model = ScoringBasedEmbeddingModel(eta=5,
-    >>>                                      k=300,
-    >>>                                      scoring_type='ComplEx')
+    >>>                                    k=300,
+    >>>                                    scoring_type='ComplEx')
     >>> model.compile(optimizer='adam', loss='multiclass_nll')
-    >>> model.fit(X,
-    >>>              batch_size=100,
-    >>>              epochs=10,
-    >>>              validation_freq=50,
-    >>>              validation_batch_size=100,
-    >>>              validation_data = dataset['valid'])
-    >>> discover_facts(X,
+    >>> model.fit(dataset,
+    >>>           batch_size=100,
+    >>>           epochs=10,
+    >>>           validation_freq=50,
+    >>>           validation_batch_size=100,
+    >>>           validation_data = dataset['valid'])
+    >>> discover_facts(dataset,
     >>>                model,
     >>>                top_n=100,
     >>>                strategy='random_uniform',
     >>>                max_candidates=100,
     >>>                target_rel='ALLIED_WITH',
     >>>                seed=0)
     Epoch 1/10
@@ -270,31 +278,34 @@
 
     Parameters
     ----------
     X: np.array, shape (n, 3)
         Triples from which to discover new facts.
     strategy: str
         The candidates generation strategy.
-        - `'random_uniform'` : generates `N` candidates (:math:`N <= max_candidates`) based on a uniform random
-            sampling of head and tail entities.
+        - `'random_uniform'` : generates `N` candidates (:math:`N <= max_candidates`) based on
+            a uniform random sampling of head and tail entities.
         - `'entity_frequency'` : generates candidates by sampling entities with low frequency.
         - `'graph_degree'` : generates candidates by sampling entities with a low graph degree.
-        - `'cluster_coefficient'` : generates candidates by sampling entities with a low clustering coefficient.
-        - `'cluster_triangles'` : generates candidates by sampling entities with a low number of cluster triangles.
-        - `'cluster_squares'` : generates candidates by sampling entities with a low number of cluster squares.
+        - `'cluster_coefficient'` : generates candidates by sampling entities with a low
+            clustering coefficient.
+        - `'cluster_triangles'` : generates candidates by sampling entities with a low number
+            of cluster triangles.
+        - `'cluster_squares'` : generates candidates by sampling entities with a low number
+            of cluster squares.
     max_candidates: int or float
         The maximum numbers of candidates generated by ``strategy``.
         Can be an absolute number or a percentage [0,1].
         This does not guarantee the number of candidates generated.
     target_rel : str
         Target relation to focus on. The function will generate candidate
          statements only with this specific relation type.
     consolidate_sides: bool
-        If `True` will generate candidate statements as a product of unique head and tail entities, otherwise will
-        consider head and tail entities separately (default: `False`).
+        If `True` will generate candidate statements as a product of unique head and tail
+        entities, otherwise will consider head and tail entities separately (default: `False`).
     seed : int
         Seed to use for reproducible results.
 
     Returns
     -------
     X_candidates : ndarray, shape (n, 3)
         A list of candidate statements.
@@ -533,21 +544,23 @@
 
 
 def find_clusters(X, model, clustering_algorithm=DBSCAN(), mode="e"):
     """
     Perform link-based cluster analysis on a knowledge graph.
 
     The clustering happens on the embedding space of the entities and relations.
-    For example, if we cluster some entities of a model that uses :math:`k=100` (i.e. embedding space of size 100),
-    we will apply the chosen clustering algorithm on the 100-dimensional space of the provided input samples.
-
-    Clustering can be used to evaluate the quality of the knowledge embeddings, by comparing to natural clusters.
-    For example, in the example below we cluster the embeddings of international football matches and end up
-    finding geographical clusters very similar to the continents.
-    This comparison can be subjective by inspecting a 2D projection of the embedding space or objective using a
+    For example, if we cluster some entities of a model that uses :math:`k=100`
+    (i.e. embedding space of size 100), we will apply the chosen clustering algorithm
+    on the 100-dimensional space of the provided input samples.
+
+    Clustering can be used to evaluate the quality of the knowledge embeddings,
+    by comparing to natural clusters. For example, in the example below we cluster
+    the embeddings of international football matches and end up finding geographical
+    clusters very similar to the continents. This comparison can be subjective by
+    inspecting a 2D projection of the embedding space or objective using a
     `clustering metric <https://scikit-learn.org/stable/modules/clustering.html#clustering-performance-evaluation>`_.
 
     | The choice of the clustering algorithm and its corresponding tuning will greatly impact the results.
       Please see `scikit-learn documentation <https://scikit-learn.org/stable/modules/clustering.html#clustering>`_
       for a list of algorithms, their parameters, and pros and cons.
 
     Clustering is exclusive (i.e., a triple is assigned to one and only one cluster).
@@ -706,16 +719,16 @@
     tolerance="auto",
     expected_fraction_duplicates=0.1,
     verbose=False,
 ):
     r"""
     Find duplicate entities, relations or triples in a graph based on their embeddings.
 
-    For example, say you have a movie dataset that was scraped off the web with possible duplicate movies.
-    The movies in this case are the entities.
+    For example, say you have a movie dataset that was scraped off the web with possible
+    duplicate movies. The movies in this case are the entities.
     Therefore, you would use the `"e"` mode to find all the movies that could de duplicates of each other.
 
     Duplicates are defined as points whose distance in the embedding space are smaller than
     some given threshold (called the tolerance).
 
     The tolerance can be defined a priori or be found via an optimisation procedure given
     an expected fraction of duplicates. The optimisation algorithm applies a root-finding routine
@@ -750,29 +763,32 @@
         - | `'t'` : the algorithm will find duplicates of the concatenation
             of the embeddings of the subject, predicate and object for each provided triple.
 
     metric: str
         A distance metric used to compare entity distance in the embedding space.
         `See options here <https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.NearestNeighbors.html>`_.
     tolerance: int or str
-        Minimum distance (depending on the chosen ``metric``) to define one entity as the duplicate of another.
-        If `'auto'`, it will be determined automatically in a way that you get the ``expected_fraction_duplicates``.
-        The `'auto'` option can be much slower than the regular one, as the finding duplicate internal procedure
-        will be repeated multiple times.
+        Minimum distance (depending on the chosen ``metric``) to define one entity as the
+        duplicate of another.
+        If `'auto'`, it will be determined automatically in a way that you get
+        the ``expected_fraction_duplicates``.
+        The `'auto'` option can be much slower than the regular one, as the finding duplicate
+        internal procedure will be repeated multiple times.
     expected_fraction_duplicates: float
         Expected fraction of duplicates to be found. It is used only when ``tolerance='auto'``.
         Should be between 0 and 1 (default: 0.1).
     verbose: bool
-        Whether to print evaluation messages during optimisation when ``tolerance='auto'`` (default: `False`).
+        Whether to print evaluation messages during optimisation when ``tolerance='auto'``
+        (default: `False`).
 
     Returns
     -------
     duplicates : set of frozensets
-        Each entry in the duplicates set is a frozenset containing all entities that were found to be duplicates
-        according to the metric and tolerance.
+        Each entry in the duplicates set is a frozenset containing all entities that were found
+        to be duplicates according to the metric and tolerance.
         Each frozenset will contain at least two entities.
 
     tolerance: float
         Tolerance used to find the duplicates (useful if the automatic tolerance option is selected).
 
     Example
     -------
@@ -932,16 +948,16 @@
             }
         else:
             dups = {frozenset(X[idx] for idx in row) for i, row in idx_dups}
         return dups
 
     def opt(tol, info):
         """
-        Auxiliary function for the optimization procedure to find the tolerance that corresponds to the expected
-        number of duplicates.
+        Auxiliary function for the optimization procedure to find the tolerance that corresponds
+        to the expected number of duplicates.
 
         Returns the difference between actual and expected fraction of duplicates.
         """
         duplicates = get_dups(tol)
         fraction_duplicates = len(set().union(*duplicates)) / len(emb)
         if verbose:
             info["Nfeval"] += 1
@@ -979,36 +995,39 @@
     all possible completions ordered by score predicted by the model.
 
     For example, given a `<subject, predicate>` pair in the arguments, the model will score
     all possible triples `<subject, predicate, ?>`, filling in the missing element with known
     entities, and return the top_n triples ordered by score. If given a `<subject, object>`
     pair it will fill in the missing element with known relations.
 
+    Therefore, if we feed the funcion with `<subject, predicate>` or `<predicate, object>`, it
+    solves the link prediction task.
+
     .. note::
         This function does not filter out true statements - triples returned can include those
         the model was trained on.
 
     Parameters
     ----------
-    model : EmbeddingModel
+    model : ScoringBasedEmbeddingModel
         The trained model that will be used to score triple completions.
     top_n : int
         The number of completed triples to returned.
     head : str
         An entity string to query.
     relation : str
         A relation string to query.
     tail : str
         An object string to query.
     ents_to_consider: array-like
-        List of entities to use for triple completions. If `None`, will generate completions using all distinct entities
-        (Default: `None`).
+        List of entities to use for triple completions. If `None`, will generate completions
+        using all distinct entities (default: `None`).
     rels_to_consider: array-like
-        List of relations to use for triple completions. If `None`, will generate completions using all distinct
-        relations (default: `None`).
+        List of relations to use for triple completions. If `None`, will generate completions
+        using all distinct relations (default: `None`).
 
     Returns
     -------
     X : ndarray of shape (n, 3)
         A list of triples ordered by score.
     S : ndarray, shape (n)
        A list of scores.
@@ -1143,7 +1162,83 @@
     # Join triples and scores, sort ascending by scores, then take top_n
     # results
     topn_idx = np.squeeze(np.argsort(scores, axis=0)[::-1][:top_n])
     scores_out = np.array(scores)[topn_idx]
     triples_out = np.copy(triples[topn_idx, :])
 
     return triples_out, scores_out
+
+
+def find_nearest_neighbours(kge_model, entities, n_neighbors=10, entities_subset=None, metric="euclidean"):
+    """ Return the nearest neighbors of entities.
+
+    The method works in the embedding space and finds a desired number of neighboring embeddings.
+    It can operate from all the entities in the graph or from a subset of interest.
+
+    Parameters
+    ----------
+    kge_model: ampligraph.latent_features.EmbeddingModel
+        Trained kge model
+    entities: list or np.array
+        List of entities whose neighbors need to be found
+    n_neighbors: int
+        number of neighbors to be computed
+    entities_subset: list or np.array
+        List of entities from which neighbors need to be computed.
+        If this list is not passed, all the entities in the graph would be used
+    metric: string or callable
+        distance metric to be used with NearestNeighbors algorithm
+        For values that can be passed, refer sklearn NearestNeighbors
+
+    Returns
+    -------
+    neighbors: np.array of size (len(entities), n_neighbors)
+        Each row contains the n_neighbors neighbours of corresponding concepts in entities
+    distance: np.array of size (len(entities), n_neighbors)
+        Each row contains distances of corresponding neighbours
+
+    Examples
+    --------
+    >>> model = DistMult(batches_count=2, seed=555, epochs=1, k=10,
+    >>>                  loss='pairwise', loss_params={'margin': 5},
+    >>>                  optimizer='adagrad', optimizer_params={'lr': 0.1})
+    >>> X = np.array([['a', 'y', 'b'],
+    >>>               ['b', 'y', 'a'],
+    >>>               ['e', 'y', 'c'],
+    >>>               ['c', 'z', 'a'],
+    >>>               ['a', 'z', 'd'],
+    >>>               ['f', 'z', 'g'],
+    >>>               ['c', 'z', 'g']])
+    >>> model.fit(X)
+    >>> neighbors, dist = find_nearest_neighbours(model,
+    >>>                                           entities=['b'],
+    >>>                                           n_neighbors=3,
+    >>>                                           entities_subset=['a', 'c', 'd', 'e', 'f'])
+    >>> print(neighbors, dist)
+    [['e' 'd' 'c']] [[0.97474706 0.979108   1.2323136 ]]
+    """
+    assert kge_model.is_fitted, "KGE model is not fit!"
+    assert isinstance(entities, (list, np.ndarray)), \
+        "Invalid type for entities! Must be a list or np.array"
+
+    if entities_subset is not None:
+        assert isinstance(entities_subset, (list, np.ndarray)), \
+            "Invalid type for entities_subset! Must be a list or np.array"
+
+        all_neighbors_emb = kge_model.get_embeddings(entities_subset)
+        all_neighbors = entities_subset
+    else:
+        all_neighbors_emb = kge_model.trained_model_params[0]
+        all_neighbors = list(kge_model.ent_to_idx.keys())
+
+    assert n_neighbors < len(all_neighbors), 'n_neighbors must be less than the number of entities being fit!'
+    knn_model = NearestNeighbors(n_neighbors=n_neighbors, metric=metric).fit(all_neighbors_emb)
+
+    test_entities_emb = kge_model.get_embeddings(entities)
+    distances, indices = knn_model.kneighbors(test_entities_emb)
+    out_neighbors = []
+    for neighbor_idx_list in indices:
+        out_neighbors.append([])
+        for neighbor_idx in neighbor_idx_list:
+            out_neighbors[-1].append(all_neighbors[neighbor_idx])
+
+    return np.array(out_neighbors), np.array(distances)
```

## ampligraph/evaluation/metrics.py

```diff
@@ -17,15 +17,15 @@
 
 def hits_at_n_score(ranks, n):
     r"""Hits@N.
 
     The function computes how many elements of a vector of rankings ``ranks`` make it to the top ``n`` positions.
 
     It can be used in conjunction with the learning to rank evaluation protocol of
-    :meth:`ampligraph.evaluation.evaluate_performance`.
+    :meth:`ampligraph.latent_features.ScoringBasedEmbeddingModel.evaluate`.
 
     It is formally defined as follows:
 
     .. math::
 
         Hits@N = \sum_{i = 1}^{|Q|} 1 \, \text{if } rank_{(s, p, o)_i} \leq N
 
@@ -86,15 +86,15 @@
 
 def mrr_score(ranks):
     r"""Mean Reciprocal Rank (MRR).
 
     The function computes the mean of the reciprocal of elements of a vector of rankings ``ranks``.
 
     It is used in conjunction with the learning to rank evaluation protocol of
-    :meth:`ampligraph.evaluation.evaluate_performance`.
+    :meth:`ampligraph.latent_features.ScoringBasedEmbeddingModel.evaluate`.
 
     It is formally defined as follows:
 
     .. math::
 
         MRR = \frac{1}{|Q|}\sum_{i = 1}^{|Q|}\frac{1}{rank_{(s, p, o)_i}}
 
@@ -195,15 +195,15 @@
 
 def mr_score(ranks):
     r"""Mean Rank (MR).
 
     The function computes the mean of a vector of rankings ``ranks``.
 
     It can be used in conjunction with the learning to rank evaluation protocol of
-    :meth:`ampligraph.evaluation.evaluate_performance`.
+    :meth:`ampligraph.latent_features.ScoringBasedEmbeddingModel.evaluate`.
 
     It is formally defined as follows:
 
     .. math::
         MR = \frac{1}{|Q|}\sum_{i = 1}^{|Q|}rank_{(s, p, o)_i}
 
     where :math:`Q` is a set of triples and :math:`(s, p, o)` is a triple :math:`\in Q`.
```

## ampligraph/evaluation/protocol.py

```diff
@@ -85,16 +85,16 @@
        ['a', 'y', 'b'],
        ['c', 'y', 'a'],
        ['b', 'y', 'c']], dtype='<U1')
     >>> X_test
     array([['f', 'y', 'e'],
        ['c', 'y', 'd']], dtype='<U1')
     >>> # if you want to split into train/valid/test datasets, call it 2 times
-    >>> X_train_valid, X_test = train_test_split_no_unseen(X, test_size=2)
-    >>> X_train, X_valid = train_test_split_no_unseen(X_train_valid, test_size=2)
+    >>> X_train_valid, X_test = train_test_split_no_unseen(X, test_size=2, backward_compatible=True)
+    >>> X_train, X_valid = train_test_split_no_unseen(X_train_valid, test_size=2, backward_compatible=True)
     >>> X_train
     array([['a', 'y', 'b'],
        ['a', 'y', 'd'],
        ['a', 'y', 'c'],
        ['c', 'y', 'a'],
        ['f', 'y', 'e']], dtype='<U1')
     >>> X_valid
```

## ampligraph/latent_features/layers/calibration/calibrate.py

```diff
@@ -2,15 +2,14 @@
 #
 # This file is Licensed under the Apache License, Version 2.0.
 # A copy of the Licence is available in LICENCE, or at:
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 import tensorflow as tf
-import numpy as np
 
 
 class CalibrationLayer(tf.keras.layers.Layer):
     """Layer to calibrate the model outputs.
 
     The class implements the heuristics described in :cite:`calibration`,
     using Platt scaling :cite:`platt1999probabilistic`.
@@ -46,17 +45,15 @@
             positive_base_rate = pos_size / (pos_size + neg_size)
 
         self.positive_base_rate = positive_base_rate
         self.w_init = tf.constant_initializer(kwargs.pop("calib_w", 0.0))
         self.b_init = tf.constant_initializer(
             kwargs.pop(
                 "calib_b",
-                np.log((self.neg_size + 1.0) / (self.pos_size + 1.0)).astype(
-                    np.float32
-                ),
+                float(tf.math.log((self.neg_size + 1.0) / (self.pos_size + 1.0)))
             )
         )
         super(CalibrationLayer, self).__init__(**kwargs)
 
     def build(self, input_shape):
         """
         Build method.
@@ -75,15 +72,15 @@
             initializer=self.b_init,
             dtype=tf.float32,
             trainable=True,
         )
         self.built = True
 
     def call(
-        self, scores_pos, scores_neg=tf.convert_to_tensor(()), training=0
+        self, scores_pos, scores_neg=[], training=0
     ):
         """
         Call method.
         """
         if training:
             scores_all = tf.concat([scores_pos, scores_neg], axis=0)
         else:
```

## ampligraph/latent_features/layers/encoding/EmbeddingLookupLayer.py

```diff
@@ -300,33 +300,50 @@
         )
         self.rel_emb.assign(
             tf.pad(
                 partition_rel_emb, paddings_rel, "CONSTANT", constant_values=0
             )
         )
 
-    def call(self, triples):
+    def call(self, sample, type_of="t"):
         """
         Looks up the embeddings of entities and relations of the triples.
 
         Parameters
         ----------
-        triples : ndarray, shape (n, 3)
-            Batch of input triples.
+        sample : ndarray, shape (n, 3) or list
+            Batch of input triples if a ndarray of shape (n,3) is given or a list
+            (of lists) of entities or relations or distances as specified in ``type_of``.
+        type_of : str
+            Specifies whether we get in input triples or entities or relations.
+            Possible values are `"t"` for triples, `"e"` for entities, `"r"`
+            for relations and "d" for distances (useful in Nodepiece) (default: `"t"`).
+
 
         Returns
         -------
         emb_triples : list
-            List of embeddings of subjects, predicates, objects.
+            List of embeddings of subjects, predicates, objects if ``type_of="t"``
+            or a list of embeddings of entities (relations/distance) if ``type_of="e"``
+            (``type_of="r"``/``type_of="d"``).
         """
-        # look up in the respective embedding matrix
-        e_s = tf.nn.embedding_lookup(self.ent_emb, triples[:, 0])
-        e_p = tf.nn.embedding_lookup(self.rel_emb, triples[:, 1])
-        e_o = tf.nn.embedding_lookup(self.ent_emb, triples[:, 2])
-        return [e_s, e_p, e_o]
+        assert type_of in ["t", "e", "r", "d"], 'Wrong selection! type_of must be in ["t", "e", "r", "d"]'
+        if type_of == "t" or type_of == "triples":
+            # look up in the respective embedding matrix
+            e_s = tf.nn.embedding_lookup(self.ent_emb, sample[:, 0])
+            e_p = tf.nn.embedding_lookup(self.rel_emb, sample[:, 1])
+            e_o = tf.nn.embedding_lookup(self.ent_emb, sample[:, 2])
+            return [e_s, e_p, e_o]
+        elif type_of == "e":
+            e = tf.nn.embedding_lookup(self.ent_emb, sample)
+        elif type_of == "r":
+            e = tf.nn.embedding_lookup(self.rel_emb, sample)
+        elif type_of == "d":
+            e = tf.nn.embedding_lookup(self.dist_emb, sample)
+        return e
 
     def compute_output_shape(self, input_shape):
         """Returns the output shape of outputs of call function.
 
         Parameters
         ----------
         input_shape: list
```

## ampligraph/latent_features/models/ScoringBasedEmbeddingModel.py

```diff
@@ -412,5424 +412,5444 @@
 000019b0: 6d73 203d 207b 7d0a 0a20 2020 2020 2020  ms = {}..       
 000019c0: 2073 656c 662e 6973 5f63 616c 6962 7261   self.is_calibra
 000019d0: 7465 6420 3d20 4661 6c73 650a 2020 2020  ted = False.    
 000019e0: 2020 2020 7365 6c66 2e69 735f 6669 7474      self.is_fitt
 000019f0: 6564 203d 2046 616c 7365 0a20 2020 2020  ed = False.     
 00001a00: 2020 2073 656c 662e 6973 5f62 6163 6b77     self.is_backw
 00001a10: 6172 6420 3d20 4661 6c73 650a 0a20 2020  ard = False..   
-00001a20: 2020 2020 2073 656c 662e 7365 6564 203d       self.seed =
-00001a30: 2073 6565 640a 2020 2020 2020 2020 7365   seed.        se
-00001a40: 6c66 2e62 6173 655f 6469 7220 3d20 7465  lf.base_dir = te
-00001a50: 6d70 6669 6c65 2e67 6574 7465 6d70 6469  mpfile.gettempdi
-00001a60: 7228 290a 2020 2020 2020 2020 7365 6c66  r().        self
-00001a70: 2e70 6172 7469 7469 6f6e 6572 5f6d 6574  .partitioner_met
-00001a80: 6164 6174 6120 3d20 7b7d 0a0a 2020 2020  adata = {}..    
-00001a90: 6465 6620 6973 5f66 6974 2873 656c 6629  def is_fit(self)
-00001aa0: 3a0a 2020 2020 2020 2020 2222 2243 6865  :.        """Che
-00001ab0: 636b 2077 6865 7468 6572 2074 6865 206d  ck whether the m
-00001ac0: 6f64 656c 2068 6173 2062 6565 6e20 6669  odel has been fi
-00001ad0: 7474 6564 2061 6c72 6561 6479 2e22 2222  tted already."""
-00001ae0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001af0: 7365 6c66 2e69 735f 6669 7474 6564 0a0a  self.is_fitted..
-00001b00: 2020 2020 6465 6620 636f 6d70 7574 655f      def compute_
-00001b10: 6f75 7470 7574 5f73 6861 7065 2873 656c  output_shape(sel
-00001b20: 662c 2069 6e70 7574 5368 6170 6529 3a0a  f, inputShape):.
-00001b30: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-00001b40: 6e73 2074 6865 206f 7574 7075 7420 7368  ns the output sh
-00001b50: 6170 6520 6f66 2074 6865 206f 7574 7075  ape of the outpu
-00001b60: 7473 206f 6620 7468 6520 6361 6c6c 2066  ts of the call f
-00001b70: 756e 6374 696f 6e2e 0a0a 2020 2020 2020  unction...      
-00001b80: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00001b90: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-00001ba0: 2020 2020 2020 2020 696e 7075 745f 7368          input_sh
-00001bb0: 6170 653a 2074 7570 6c65 0a20 2020 2020  ape: tuple.     
-00001bc0: 2020 2020 2020 2053 6861 7065 206f 6620         Shape of 
-00001bd0: 696e 7075 7473 206f 6620 6361 6c6c 2066  inputs of call f
-00001be0: 756e 6374 696f 6e2e 0a0a 2020 2020 2020  unction...      
-00001bf0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-00001c00: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00001c10: 2020 6f75 7470 7574 5f73 6861 7065 3a20    output_shape: 
-00001c20: 6c69 7374 206f 6620 7475 706c 6573 0a20  list of tuples. 
-00001c30: 2020 2020 2020 2020 2020 204c 6973 7420             List 
-00001c40: 7769 7468 2074 6865 2073 6861 7065 206f  with the shape o
-00001c50: 6620 6f75 7470 7574 7320 6f66 2063 616c  f outputs of cal
-00001c60: 6c20 6675 6e63 7469 6f6e 2066 6f72 2074  l function for t
-00001c70: 6865 2069 6e70 7574 2074 7269 706c 6573  he input triples
-00001c80: 2061 6e64 2074 6865 2063 6f72 7275 7074   and the corrupt
-00001c90: 696f 6e20 7363 6f72 6573 2e0a 2020 2020  ion scores..    
-00001ca0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00001cb0: 2320 696e 7075 7420 7472 6970 6c65 2073  # input triple s
-00001cc0: 636f 7265 2028 6261 7463 685f 7369 7a65  core (batch_size
-00001cd0: 2c20 3129 2061 6e64 2063 6f72 7275 7074  , 1) and corrupt
-00001ce0: 696f 6e20 7363 6f72 6520 2862 6174 6368  ion score (batch
-00001cf0: 5f73 697a 6520 2a0a 2020 2020 2020 2020  _size *.        
-00001d00: 2320 6574 612c 2031 290a 2020 2020 2020  # eta, 1).      
-00001d10: 2020 7265 7475 726e 205b 284e 6f6e 652c    return [(None,
-00001d20: 2031 292c 2028 4e6f 6e65 2c20 3129 5d0a   1), (None, 1)].
-00001d30: 0a20 2020 2064 6566 2070 6172 7469 7469  .    def partiti
-00001d40: 6f6e 5f63 6861 6e67 655f 7570 6461 7465  on_change_update
-00001d50: 7328 7365 6c66 2c20 6e75 6d5f 656e 7473  s(self, num_ents
-00001d60: 2c20 656e 745f 656d 622c 2072 656c 5f65  , ent_emb, rel_e
-00001d70: 6d62 293a 0a20 2020 2020 2020 2022 2222  mb):.        """
-00001d80: 5065 7266 6f72 6d20 7468 6520 6368 616e  Perform the chan
-00001d90: 6765 7320 7468 6174 2061 7265 2072 6571  ges that are req
-00001da0: 7569 7265 6420 7768 656e 2074 6865 2070  uired when the p
-00001db0: 6172 7469 7469 6f6e 2069 7320 6d6f 6469  artition is modi
-00001dc0: 6669 6564 2064 7572 696e 6720 7472 6169  fied during trai
-00001dd0: 6e69 6e67 2e0a 0a20 2020 2020 2020 2050  ning...        P
-00001de0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00001df0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00001e00: 2020 2020 206e 756d 5f65 6e74 733a 2069       num_ents: i
-00001e10: 6e74 0a20 2020 2020 2020 2020 2020 204e  nt.            N
-00001e20: 756d 6265 7220 6f66 2075 6e69 7175 6520  umber of unique 
-00001e30: 656e 7469 7469 6573 2069 6e20 7468 6520  entities in the 
-00001e40: 7061 7274 6974 696f 6e2e 0a20 2020 2020  partition..     
-00001e50: 2020 2065 6e74 5f65 6d62 3a20 6172 7261     ent_emb: arra
-00001e60: 792d 6c69 6b65 0a20 2020 2020 2020 2020  y-like.         
-00001e70: 2020 2045 6e74 6974 7920 656d 6265 6464     Entity embedd
-00001e80: 696e 6773 2074 6861 7420 6e65 6564 2074  ings that need t
-00001e90: 6f20 6265 2074 7261 696e 6564 2066 6f72  o be trained for
-00001ea0: 2074 6865 2070 6172 7469 7469 6f6e 0a20   the partition. 
-00001eb0: 2020 2020 2020 2020 2020 2028 616c 6c20             (all 
-00001ec0: 7472 6970 6c65 7320 6f66 2074 6865 2070  triples of the p
-00001ed0: 6172 7469 7469 6f6e 2077 696c 6c20 6861  artition will ha
-00001ee0: 7665 2065 6d62 6564 6469 6e67 7320 696e  ve embeddings in
-00001ef0: 2074 6869 7320 6d61 7472 6978 292e 0a20   this matrix).. 
-00001f00: 2020 2020 2020 2072 656c 5f65 6d62 3a20         rel_emb: 
-00001f10: 6172 7261 792d 6c69 6b65 0a20 2020 2020  array-like.     
-00001f20: 2020 2020 2020 2072 656c 6174 696f 6e20         relation 
-00001f30: 656d 6265 6464 696e 6773 2074 6861 7420  embeddings that 
-00001f40: 6e65 6564 2074 6f20 6265 2074 7261 696e  need to be train
-00001f50: 6564 2066 6f72 2074 6865 2070 6172 7469  ed for the parti
-00001f60: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00001f70: 2028 616c 6c20 7472 6970 6c65 7320 6f66   (all triples of
-00001f80: 2074 6865 2070 6172 7469 7469 6f6e 2077   the partition w
-00001f90: 696c 6c20 6861 7665 2065 6d62 6564 6469  ill have embeddi
-00001fa0: 6e67 7320 696e 2074 6869 7320 6d61 7472  ngs in this matr
-00001fb0: 6978 292e 0a0a 2020 2020 2020 2020 2222  ix)...        ""
-00001fc0: 220a 2020 2020 2020 2020 2320 7361 7665  ".        # save
-00001fd0: 2074 6865 2075 6e69 7175 6520 656e 7469   the unique enti
-00001fe0: 7469 6573 206f 6620 7468 6520 7061 7274  ties of the part
-00001ff0: 6974 696f 6e20 3a20 7769 6c6c 2062 6520  ition : will be 
-00002000: 7573 6564 2066 6f72 0a20 2020 2020 2020  used for.       
-00002010: 2023 2063 6f72 7275 7074 696f 6e20 6765   # corruption ge
-00002020: 6e65 7261 7469 6f6e 0a20 2020 2020 2020  neration.       
-00002030: 2073 656c 662e 6e75 6d5f 656e 7473 203d   self.num_ents =
-00002040: 206e 756d 5f65 6e74 730a 2020 2020 2020   num_ents.      
-00002050: 2020 6966 2073 656c 662e 656e 636f 6469    if self.encodi
-00002060: 6e67 5f6c 6179 6572 2e62 7569 6c74 3a0a  ng_layer.built:.
-00002070: 2020 2020 2020 2020 2020 2020 2320 7570              # up
-00002080: 6461 7465 2074 6865 2074 7261 696e 6162  date the trainab
-00002090: 6c65 2076 6172 6961 626c 6520 696e 2074  le variable in t
-000020a0: 6865 2065 6e63 6f64 696e 6720 6c61 7965  he encoding laye
-000020b0: 720a 2020 2020 2020 2020 2020 2020 7365  r.            se
-000020c0: 6c66 2e65 6e63 6f64 696e 675f 6c61 7965  lf.encoding_laye
-000020d0: 722e 7061 7274 6974 696f 6e5f 6368 616e  r.partition_chan
-000020e0: 6765 5f75 7064 6174 6573 2865 6e74 5f65  ge_updates(ent_e
-000020f0: 6d62 2c20 7265 6c5f 656d 6229 0a20 2020  mb, rel_emb).   
-00002100: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00002110: 2020 2020 2020 2023 2069 6620 7468 6520         # if the 
-00002120: 656e 636f 6469 6e67 206c 6179 6572 2068  encoding layer h
-00002130: 6173 206e 6f74 2062 6565 6e20 6275 696c  as not been buil
-00002140: 7420 7468 656e 2073 746f 7265 2069 7420  t then store it 
-00002150: 6173 2061 6e20 696e 6974 6961 6c69 7a65  as an initialize
-00002160: 720a 2020 2020 2020 2020 2020 2020 2320  r.            # 
-00002170: 7468 6973 2077 6f75 6c64 2062 6520 7468  this would be th
-00002180: 6520 6361 7365 206f 6620 6475 7269 6e67  e case of during
-00002190: 2070 6172 7469 7469 6f6e 6564 2074 7261   partitioned tra
-000021a0: 696e 696e 6720 2866 6972 7374 0a20 2020  ining (first.   
-000021b0: 2020 2020 2020 2020 2023 2062 6174 6368           # batch
-000021c0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000021d0: 6c66 2e65 6e63 6f64 696e 675f 6c61 7965  lf.encoding_laye
-000021e0: 722e 7365 745f 656e 745f 7265 6c5f 696e  r.set_ent_rel_in
-000021f0: 6974 6961 6c5f 7661 6c75 6528 656e 745f  itial_value(ent_
-00002200: 656d 622c 2072 656c 5f65 6d62 290a 0a20  emb, rel_emb).. 
-00002210: 2020 2064 6566 2063 616c 6c28 7365 6c66     def call(self
-00002220: 2c20 696e 7075 7473 2c20 7472 6169 6e69  , inputs, traini
-00002230: 6e67 3d46 616c 7365 293a 0a20 2020 2020  ng=False):.     
-00002240: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-00002250: 6f6d 7075 7465 7320 7468 6520 7363 6f72  omputes the scor
-00002260: 6573 206f 6620 7468 6520 7472 6970 6c65  es of the triple
-00002270: 7320 616e 6420 7265 7475 726e 7320 7468  s and returns th
-00002280: 6520 636f 7272 7570 7469 6f6e 2073 636f  e corruption sco
-00002290: 7265 7320 6173 2077 656c 6c2e 0a0a 2020  res as well...  
-000022a0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-000022b0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000022c0: 2d2d 2d0a 2020 2020 2020 2020 696e 7075  ---.        inpu
-000022d0: 7473 3a20 6e64 6172 7261 792c 2073 6861  ts: ndarray, sha
-000022e0: 7065 2028 6e2c 2033 290a 2020 2020 2020  pe (n, 3).      
-000022f0: 2020 2020 2020 4261 7463 6820 6f66 2069        Batch of i
-00002300: 6e70 7574 2074 7269 706c 6573 2e0a 0a20  nput triples... 
-00002310: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-00002320: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00002330: 2020 2020 2020 206f 7574 3a20 6c69 7374         out: list
-00002340: 0a20 2020 2020 2020 2020 2020 204c 6973  .            Lis
-00002350: 7420 6f66 2069 6e70 7574 2073 636f 7265  t of input score
-00002360: 7320 616c 6f6e 6720 7769 7468 2074 6865  s along with the
-00002370: 6972 2063 6f72 7275 7074 696f 6e73 2e0a  ir corruptions..
-00002380: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00002390: 2020 2020 2320 6c6f 6f6b 7570 2065 6d62      # lookup emb
-000023a0: 6564 6469 6e67 7320 6f66 2074 6865 2069  eddings of the i
-000023b0: 6e70 7574 730a 2020 2020 2020 2020 696e  nputs.        in
-000023c0: 705f 656d 6220 3d20 7365 6c66 2e65 6e63  p_emb = self.enc
-000023d0: 6f64 696e 675f 6c61 7965 7228 696e 7075  oding_layer(inpu
-000023e0: 7473 290a 2020 2020 2020 2020 2320 7363  ts).        # sc
-000023f0: 6f72 6520 7468 6520 696e 7075 7473 0a20  ore the inputs. 
-00002400: 2020 2020 2020 2069 6e70 5f73 636f 7265         inp_score
-00002410: 203d 2073 656c 662e 7363 6f72 696e 675f   = self.scoring_
-00002420: 6c61 7965 7228 696e 705f 656d 6229 0a20  layer(inp_emb). 
-00002430: 2020 2020 2020 2023 2073 636f 7265 2074         # score t
-00002440: 6865 2063 6f72 7275 7074 696f 6e73 0a0a  he corruptions..
-00002450: 2020 2020 2020 2020 6966 2074 7261 696e          if train
-00002460: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
-00002470: 2023 2067 656e 6572 6174 6520 7468 6520   # generate the 
-00002480: 636f 7272 7570 7469 6f6e 7320 666f 7220  corruptions for 
-00002490: 7468 6520 696e 7075 7420 7472 6970 6c65  the input triple
-000024a0: 730a 2020 2020 2020 2020 2020 2020 636f  s.            co
-000024b0: 7272 7570 7469 6f6e 7320 3d20 7365 6c66  rruptions = self
-000024c0: 2e63 6f72 7275 7074 696f 6e5f 6c61 7965  .corruption_laye
-000024d0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-000024e0: 2020 2069 6e70 7574 732c 2073 656c 662e     inputs, self.
-000024f0: 6e75 6d5f 656e 7473 2c20 7365 6c66 2e65  num_ents, self.e
-00002500: 7461 0a20 2020 2020 2020 2020 2020 2029  ta.            )
-00002510: 0a20 2020 2020 2020 2020 2020 2023 206c  .            # l
-00002520: 6f6f 6b75 7020 656d 6265 6464 696e 6773  ookup embeddings
-00002530: 206f 6620 7468 6520 696e 7075 7473 0a20   of the inputs. 
-00002540: 2020 2020 2020 2020 2020 2063 6f72 725f             corr_
-00002550: 656d 6220 3d20 7365 6c66 2e65 6e63 6f64  emb = self.encod
-00002560: 696e 675f 6c61 7965 7228 636f 7272 7570  ing_layer(corrup
-00002570: 7469 6f6e 7329 0a20 2020 2020 2020 2020  tions).         
-00002580: 2020 2063 6f72 725f 7363 6f72 6520 3d20     corr_score = 
-00002590: 7365 6c66 2e73 636f 7269 6e67 5f6c 6179  self.scoring_lay
-000025a0: 6572 2863 6f72 725f 656d 6229 0a0a 2020  er(corr_emb)..  
-000025b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000025c0: 2069 6e70 5f73 636f 7265 2c20 636f 7272   inp_score, corr
-000025d0: 5f73 636f 7265 0a0a 2020 2020 2020 2020  _score..        
-000025e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000025f0: 2020 7265 7475 726e 2069 6e70 5f73 636f    return inp_sco
-00002600: 7265 0a0a 2020 2020 4074 662e 6675 6e63  re..    @tf.func
-00002610: 7469 6f6e 2865 7870 6572 696d 656e 7461  tion(experimenta
-00002620: 6c5f 7265 6c61 785f 7368 6170 6573 3d54  l_relax_shapes=T
-00002630: 7275 6529 0a20 2020 2064 6566 205f 6765  rue).    def _ge
-00002640: 745f 7261 6e6b 7328 0a20 2020 2020 2020  t_ranks(.       
-00002650: 2073 656c 662c 0a20 2020 2020 2020 2069   self,.        i
-00002660: 6e70 7574 732c 0a20 2020 2020 2020 2065  nputs,.        e
-00002670: 6e74 5f65 6d62 732c 0a20 2020 2020 2020  nt_embs,.       
-00002680: 2073 7461 7274 5f69 642c 0a20 2020 2020   start_id,.     
-00002690: 2020 2065 6e64 5f69 642c 0a20 2020 2020     end_id,.     
-000026a0: 2020 2066 696c 7465 7273 2c0a 2020 2020     filters,.    
-000026b0: 2020 2020 6d61 7070 696e 675f 6469 6374      mapping_dict
-000026c0: 2c0a 2020 2020 2020 2020 636f 7272 7570  ,.        corrup
-000026d0: 745f 7369 6465 3d22 732c 6f22 2c0a 2020  t_side="s,o",.  
-000026e0: 2020 2020 2020 7261 6e6b 696e 675f 7374        ranking_st
-000026f0: 7261 7465 6779 3d22 776f 7273 7422 2c0a  rategy="worst",.
-00002700: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-00002710: 2222 0a20 2020 2020 2020 2045 7661 6c75  "".        Evalu
-00002720: 6174 6520 7468 6520 696e 7075 7473 2061  ate the inputs a
-00002730: 6761 696e 7374 2063 6f72 7275 7074 696f  gainst corruptio
-00002740: 6e73 2061 6e64 2072 6574 7572 6e20 7261  ns and return ra
-00002750: 6e6b 732e 0a0a 2020 2020 2020 2020 5061  nks...        Pa
-00002760: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00002770: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00002780: 2020 2020 696e 7075 7473 3a20 6172 7261      inputs: arra
-00002790: 792d 6c69 6b65 2c20 7368 6170 6520 286e  y-like, shape (n
-000027a0: 2c20 3329 0a20 2020 2020 2020 2020 2020  , 3).           
-000027b0: 2042 6174 6368 206f 6620 696e 7075 7420   Batch of input 
-000027c0: 7472 6970 6c65 732e 0a20 2020 2020 2020  triples..       
-000027d0: 2065 6e74 5f65 6d62 733a 2061 7272 6179   ent_embs: array
-000027e0: 2d6c 696b 652c 2073 6861 7065 2028 6d2c  -like, shape (m,
-000027f0: 206b 290a 2020 2020 2020 2020 2020 2020   k).            
-00002800: 536c 6963 6520 6f66 2065 6d62 6564 6469  Slice of embeddi
-00002810: 6e67 206d 6174 7269 7820 2863 6f72 7275  ng matrix (corru
-00002820: 7074 696f 6e73 292e 0a20 2020 2020 2020  ptions)..       
-00002830: 2073 7461 7274 5f69 643a 2069 6e74 0a20   start_id: int. 
-00002840: 2020 2020 2020 2020 2020 204f 7269 6769             Origi
-00002850: 6e61 6c20 6964 206f 6620 7468 6520 6669  nal id of the fi
-00002860: 7273 7420 726f 7720 6f66 2065 6d62 6564  rst row of embed
-00002870: 6469 6e67 206d 6174 7269 7820 2875 7365  ding matrix (use
-00002880: 6420 6475 7269 6e67 2070 6172 7469 7469  d during partiti
-00002890: 6f6e 6564 2061 7070 726f 6163 6829 2e0a  oned approach)..
-000028a0: 2020 2020 2020 2020 656e 645f 6964 3a20          end_id: 
-000028b0: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-000028c0: 4f72 6967 696e 616c 2069 6420 6f66 2074  Original id of t
-000028d0: 6865 206c 6173 7420 726f 7720 6f66 2065  he last row of e
-000028e0: 6d62 6564 6469 6e67 206d 6174 7269 7820  mbedding matrix 
-000028f0: 2875 7365 6420 6475 7269 6e67 2070 6172  (used during par
-00002900: 7469 7469 6f6e 6564 2061 7070 726f 6163  titioned approac
-00002910: 6829 2e0a 2020 2020 2020 2020 6669 6c74  h)..        filt
-00002920: 6572 733a 206c 6973 7420 6f66 206c 6973  ers: list of lis
-00002930: 7473 0a20 2020 2020 2020 2020 2020 2053  ts.            S
-00002940: 697a 6520 6f66 206c 6973 7420 6973 2065  ize of list is e
-00002950: 6974 6865 7220 3120 6f72 2032 2064 6570  ither 1 or 2 dep
-00002960: 656e 6469 6e67 206f 6e20 6060 636f 7272  ending on ``corr
-00002970: 7570 745f 7369 6465 6060 2e0a 2020 2020  upt_side``..    
-00002980: 2020 2020 2020 2020 5369 7a65 206f 6620          Size of 
-00002990: 7468 6520 696e 7465 726e 616c 206c 6973  the internal lis
-000029a0: 7420 6973 2065 7175 616c 2074 6f20 7468  t is equal to th
-000029b0: 6520 7369 7a65 206f 6620 7468 6520 696e  e size of the in
-000029c0: 7075 7420 7472 6970 6c65 732e 0a20 2020  put triples..   
-000029d0: 2020 2020 2020 2020 2045 6163 6820 6c69           Each li
-000029e0: 7374 2063 6f6e 7461 696e 7320 616e 2061  st contains an a
-000029f0: 7272 6179 206f 6620 6669 6c74 6572 7320  rray of filters 
-00002a00: 2869 2e65 2e2c 2054 7275 6520 506f 7369  (i.e., True Posi
-00002a10: 7469 7665 7329 2072 656c 6174 6564 2074  tives) related t
-00002a20: 6f20 7468 6520 7370 6563 6966 6965 6420  o the specified 
-00002a30: 7369 6465 206f 6620 7468 650a 2020 2020  side of the.    
-00002a40: 2020 2020 2020 2020 636f 7272 6573 706f          correspo
-00002a50: 6e64 696e 6720 696e 7075 7420 7472 6970  nding input trip
-00002a60: 6c65 732e 0a20 2020 2020 2020 2063 6f72  les..        cor
-00002a70: 7275 7074 5f73 6964 653a 2073 7472 0a20  rupt_side: str. 
-00002a80: 2020 2020 2020 2020 2020 2057 6869 6368             Which
-00002a90: 2073 6964 6520 746f 2063 6f72 7275 7074   side to corrupt
-00002aa0: 2064 7572 696e 6720 6576 616c 7561 7469   during evaluati
-00002ab0: 6f6e 2e0a 2020 2020 2020 2020 7261 6e6b  on..        rank
-00002ac0: 696e 675f 7374 7261 7465 6779 3a20 7374  ing_strategy: st
-00002ad0: 720a 2020 2020 2020 2020 2020 2020 496e  r.            In
-00002ae0: 6469 6361 7465 7320 686f 7720 746f 2062  dicates how to b
-00002af0: 7265 616b 2074 6965 7320 2864 6566 6175  reak ties (defau
-00002b00: 6c74 3a20 6077 6f72 7374 602c 2069 2e65  lt: `worst`, i.e
-00002b10: 2e2c 2061 7373 6967 6e73 2074 6865 2077  ., assigns the w
-00002b20: 6f72 7374 2072 616e 6b20 746f 2074 6865  orst rank to the
-00002b30: 2074 6573 7420 7472 6970 6c65 292e 0a20   test triple).. 
-00002b40: 2020 2020 2020 2020 2020 2043 616e 2062             Can b
-00002b50: 6520 6f6e 6520 6f66 2074 6865 2074 6872  e one of the thr
-00002b60: 6565 2074 7970 6573 2060 2262 6573 7422  ee types `"best"
-00002b70: 602c 2060 226d 6964 646c 6522 602c 2060  `, `"middle"`, `
-00002b80: 2277 6f72 7374 2260 2e0a 0a20 2020 2020  "worst"`...     
-00002b90: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00002ba0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00002bb0: 2020 2072 616e 6b3a 2074 662e 5465 6e73     rank: tf.Tens
-00002bc0: 6f72 2c20 7368 6170 6520 286e 2c20 6e75  or, shape (n, nu
-00002bd0: 6d20 6f66 2073 6964 6573 2062 6569 6e67  m of sides being
-00002be0: 2063 6f72 7275 7074 6564 290a 2020 2020   corrupted).    
-00002bf0: 2020 2020 2020 2020 5261 6e6b 696e 6720          Ranking 
-00002c00: 6167 6169 6e73 7420 7375 626a 6563 7420  against subject 
-00002c10: 636f 7272 7570 7469 6f6e 7320 616e 6420  corruptions and 
-00002c20: 6f62 6a65 6374 2063 6f72 7275 7074 696f  object corruptio
-00002c30: 6e73 0a20 2020 2020 2020 2020 2020 2028  ns.            (
-00002c40: 636f 7272 7570 7469 6f6e 7320 6465 6669  corruptions defi
-00002c50: 6e65 6420 6279 2060 656e 745f 656d 6273  ned by `ent_embs
-00002c60: 6020 6d61 7472 6978 292e 0a20 2020 2020  ` matrix)..     
-00002c70: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00002c80: 6620 6e6f 7420 7365 6c66 2e69 735f 7061  f not self.is_pa
-00002c90: 7274 6974 696f 6e65 645f 7472 6169 6e69  rtitioned_traini
-00002ca0: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
-00002cb0: 696e 7075 7473 203d 205b 0a20 2020 2020  inputs = [.     
-00002cc0: 2020 2020 2020 2020 2020 2074 662e 6e6e             tf.nn
-00002cd0: 2e65 6d62 6564 6469 6e67 5f6c 6f6f 6b75  .embedding_looku
-00002ce0: 7028 0a20 2020 2020 2020 2020 2020 2020  p(.             
-00002cf0: 2020 2020 2020 2073 656c 662e 656e 636f         self.enco
-00002d00: 6469 6e67 5f6c 6179 6572 2e65 6e74 5f65  ding_layer.ent_e
-00002d10: 6d62 2c20 696e 7075 7473 5b3a 2c20 305d  mb, inputs[:, 0]
-00002d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002d30: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00002d40: 2020 2020 7466 2e6e 6e2e 656d 6265 6464      tf.nn.embedd
-00002d50: 696e 675f 6c6f 6f6b 7570 280a 2020 2020  ing_lookup(.    
-00002d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d70: 7365 6c66 2e65 6e63 6f64 696e 675f 6c61  self.encoding_la
-00002d80: 7965 722e 7265 6c5f 656d 622c 2069 6e70  yer.rel_emb, inp
-00002d90: 7574 735b 3a2c 2031 5d0a 2020 2020 2020  uts[:, 1].      
-00002da0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-00002db0: 2020 2020 2020 2020 2020 2020 2074 662e               tf.
-00002dc0: 6e6e 2e65 6d62 6564 6469 6e67 5f6c 6f6f  nn.embedding_loo
-00002dd0: 6b75 7028 0a20 2020 2020 2020 2020 2020  kup(.           
-00002de0: 2020 2020 2020 2020 2073 656c 662e 656e           self.en
-00002df0: 636f 6469 6e67 5f6c 6179 6572 2e65 6e74  coding_layer.ent
-00002e00: 5f65 6d62 2c20 696e 7075 7473 5b3a 2c20  _emb, inputs[:, 
-00002e10: 325d 0a20 2020 2020 2020 2020 2020 2020  2].             
-00002e20: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00002e30: 2020 5d0a 0a20 2020 2020 2020 2072 6574    ]..        ret
-00002e40: 7572 6e20 7365 6c66 2e73 636f 7269 6e67  urn self.scoring
-00002e50: 5f6c 6179 6572 2e67 6574 5f72 616e 6b73  _layer.get_ranks
-00002e60: 280a 2020 2020 2020 2020 2020 2020 696e  (.            in
-00002e70: 7075 7473 2c0a 2020 2020 2020 2020 2020  puts,.          
-00002e80: 2020 656e 745f 656d 6273 2c0a 2020 2020    ent_embs,.    
-00002e90: 2020 2020 2020 2020 7374 6172 745f 6964          start_id
-00002ea0: 2c0a 2020 2020 2020 2020 2020 2020 656e  ,.            en
-00002eb0: 645f 6964 2c0a 2020 2020 2020 2020 2020  d_id,.          
-00002ec0: 2020 6669 6c74 6572 732c 0a20 2020 2020    filters,.     
-00002ed0: 2020 2020 2020 206d 6170 7069 6e67 5f64         mapping_d
-00002ee0: 6963 742c 0a20 2020 2020 2020 2020 2020  ict,.           
-00002ef0: 2063 6f72 7275 7074 5f73 6964 652c 0a20   corrupt_side,. 
-00002f00: 2020 2020 2020 2020 2020 2072 616e 6b69             ranki
-00002f10: 6e67 5f73 7472 6174 6567 792c 0a20 2020  ng_strategy,.   
-00002f20: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-00002f30: 6275 696c 6428 7365 6c66 2c20 696e 7075  build(self, inpu
-00002f40: 745f 7368 6170 6529 3a0a 2020 2020 2020  t_shape):.      
-00002f50: 2020 2222 224f 7665 7272 6964 6520 7468    """Override th
-00002f60: 6520 6275 696c 6420 6675 6e63 7469 6f6e  e build function
-00002f70: 206f 6620 7468 6520 4d6f 6465 6c20 636c   of the Model cl
-00002f80: 6173 732e 0a0a 2020 2020 2020 2020 4974  ass...        It
-00002f90: 2069 7320 6361 6c6c 6564 206f 6e20 7468   is called on th
-00002fa0: 6520 6669 7273 7420 6361 6c6c 2074 6f20  e first call to 
-00002fb0: 6060 5f5f 6361 6c6c 5f5f 6060 2e0a 2020  ``__call__``..  
-00002fc0: 2020 2020 2020 5769 7468 2074 6869 7320        With this 
-00002fd0: 6675 6e63 7469 6f6e 2077 6520 7365 7420  function we set 
-00002fe0: 736f 6d65 2069 6e74 6572 6e61 6c20 7061  some internal pa
-00002ff0: 7261 6d65 7465 7273 206f 6620 7468 6520  rameters of the 
-00003000: 656e 636f 6469 6e67 206c 6179 6572 7320  encoding layers 
-00003010: 286e 6565 6465 6420 746f 2062 7569 6c64  (needed to build
-00003020: 2074 6861 7420 6c61 7965 7273 0a20 2020   that layers.   
-00003030: 2020 2020 2074 6865 6d73 656c 7665 7329       themselves)
-00003040: 2062 6173 6564 206f 6e20 7468 6520 696e   based on the in
-00003050: 7075 7420 6461 7461 2073 7570 706c 6965  put data supplie
-00003060: 6420 6279 2074 6865 2075 7365 7220 7768  d by the user wh
-00003070: 696c 6520 6361 6c6c 696e 6720 7468 6520  ile calling the 
-00003080: 607e 5363 6f72 696e 6742 6173 6564 456d  `~ScoringBasedEm
-00003090: 6265 6464 696e 674d 6f64 656c 2e66 6974  beddingModel.fit
-000030a0: 6020 6d65 7468 6f64 2e0a 2020 2020 2020  ` method..      
-000030b0: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
-000030c0: 7365 7420 7468 6520 6d61 7820 6e75 6d62  set the max numb
-000030d0: 6572 206f 6620 7468 6520 656e 7469 7469  er of the entiti
-000030e0: 6573 2074 6861 7420 7769 6c6c 2062 6520  es that will be 
-000030f0: 7472 6169 6e65 6420 7065 7220 7061 7274  trained per part
-00003100: 6974 696f 6e0a 2020 2020 2020 2020 2320  ition.        # 
-00003110: 696e 2063 6173 6520 6f66 206e 6f6e 2d70  in case of non-p
-00003120: 6172 7469 7469 6f6e 6564 2074 7261 696e  artitioned train
-00003130: 696e 672c 2069 7420 6973 2065 7175 616c  ing, it is equal
-00003140: 2074 6f20 7468 6520 746f 7461 6c20 6e75   to the total nu
-00003150: 6d62 6572 0a20 2020 2020 2020 2023 206f  mber.        # o
-00003160: 6620 656e 7469 7469 6573 206f 6620 7468  f entities of th
-00003170: 6520 6461 7461 7365 740a 2020 2020 2020  e dataset.      
-00003180: 2020 7365 6c66 2e65 6e63 6f64 696e 675f    self.encoding_
-00003190: 6c61 7965 722e 6d61 785f 656e 745f 7369  layer.max_ent_si
-000031a0: 7a65 203d 2073 656c 662e 6d61 785f 656e  ze = self.max_en
-000031b0: 745f 7369 7a65 0a20 2020 2020 2020 2023  t_size.        #
-000031c0: 2073 6574 2074 6865 206d 6178 206e 756d   set the max num
-000031d0: 6265 7220 6f66 2072 656c 6174 696f 6e73  ber of relations
-000031e0: 2062 6569 6e67 2074 7261 696e 6564 206a   being trained j
-000031f0: 7573 7420 6c69 6b65 2061 626f 7665 0a20  ust like above. 
-00003200: 2020 2020 2020 2073 656c 662e 656e 636f         self.enco
-00003210: 6469 6e67 5f6c 6179 6572 2e6d 6178 5f72  ding_layer.max_r
-00003220: 656c 5f73 697a 6520 3d20 7365 6c66 2e6d  el_size = self.m
-00003230: 6178 5f72 656c 5f73 697a 650a 2020 2020  ax_rel_size.    
-00003240: 2020 2020 7365 6c66 2e6e 756d 5f65 6e74      self.num_ent
-00003250: 7320 3d20 7365 6c66 2e6d 6178 5f65 6e74  s = self.max_ent
-00003260: 5f73 697a 650a 2020 2020 2020 2020 7365  _size.        se
-00003270: 6c66 2e62 7569 6c74 203d 2054 7275 650a  lf.built = True.
-00003280: 0a20 2020 2064 6566 2063 6f6d 7075 7465  .    def compute
-00003290: 5f66 6f63 7573 455f 7765 6967 6874 7328  _focusE_weights(
-000032a0: 7365 6c66 2c20 7765 6967 6874 732c 2073  self, weights, s
-000032b0: 7472 7563 7475 7265 5f77 6569 6768 7429  tructure_weight)
-000032c0: 3a0a 2020 2020 2020 2020 2222 2243 6f6d  :.        """Com
-000032d0: 7075 7465 2070 6f73 6974 6976 6520 616e  pute positive an
-000032e0: 6420 6e65 6761 7469 7665 2077 6569 6768  d negative weigh
-000032f0: 7473 2074 6f20 7363 616c 6520 7363 6f72  ts to scale scor
-00003300: 6573 2069 6620 6060 7573 655f 666f 6375  es if ``use_focu
-00003310: 7345 3d54 7275 6560 602e 0a0a 2020 2020  sE=True``...    
-00003320: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00003330: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00003340: 2d0a 2020 2020 2020 2020 7765 6967 6874  -.        weight
-00003350: 733a 2061 7272 6179 2d6c 696b 652c 2073  s: array-like, s
-00003360: 6861 7065 2028 6e2c 206d 290a 2020 2020  hape (n, m).    
-00003370: 2020 2020 2020 2020 4261 7463 6820 6f66          Batch of
-00003380: 2077 6569 6768 7473 2061 7373 6f63 6961   weights associa
-00003390: 7465 6420 7472 6970 6c65 732e 0a20 2020  ted triples..   
-000033a0: 2020 2020 2073 7472 7563 7574 7572 655f       strucuture_
-000033b0: 7765 6967 6874 3a20 666c 6f61 740a 2020  weight: float.  
-000033c0: 2020 2020 2020 2020 2020 5374 7275 6374            Struct
-000033d0: 7572 616c 2069 6e66 6c75 656e 6365 2061  ural influence a
-000033e0: 7373 6967 6e65 6420 746f 2074 6865 2077  ssigned to the w
-000033f0: 6569 6768 7473 2e0a 0a20 2020 2020 2020  eights...       
-00003400: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00003410: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00003420: 206f 7574 3a20 7475 706c 6520 6f66 2074   out: tuple of t
-00003430: 776f 2074 662e 5465 6e73 6f72 732c 2028  wo tf.Tensors, (
-00003440: 7466 2e54 656e 736f 7228 7368 6170 653d  tf.Tensor(shape=
-00003450: 286e 2c20 3129 292c 2074 662e 5465 6e73  (n, 1)), tf.Tens
-00003460: 6f72 2873 6861 7065 3d28 6e20 2a20 7365  or(shape=(n * se
-00003470: 6c66 2e65 7461 2c20 3129 2929 0a20 2020  lf.eta, 1))).   
-00003480: 2020 2020 2020 2020 2054 7570 6c65 2077           Tuple w
-00003490: 6865 7265 2074 6865 2066 6972 7374 2065  here the first e
-000034a0: 6c65 6d65 6e74 7320 6973 2061 2074 656e  lements is a ten
-000034b0: 736f 7220 636f 6e74 6169 6e69 6e67 2074  sor containing t
-000034c0: 6865 2070 6f73 6974 6976 6520 7765 6967  he positive weig
-000034d0: 6874 730a 2020 2020 2020 2020 2020 2020  hts.            
-000034e0: 616e 6420 7468 6520 7365 636f 6e64 2069  and the second i
-000034f0: 7320 6120 7465 6e73 6f72 2063 6f6e 7461  s a tensor conta
-00003500: 696e 696e 6720 7468 6520 6e65 6761 7469  ining the negati
-00003510: 7665 2077 6569 6768 7473 2e0a 2020 2020  ve weights..    
-00003520: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00003530: 2023 2057 6569 6768 7473 2063 6f6d 7075   # Weights compu
-00003540: 7461 7469 6f6e 0a20 2020 2020 2020 2077  tation.        w
-00003550: 6569 6768 7473 203d 2074 662e 7265 6475  eights = tf.redu
-00003560: 6365 5f6d 6561 6e28 7765 6967 6874 732c  ce_mean(weights,
-00003570: 2031 290a 2020 2020 2020 2020 7765 6967   1).        weig
-00003580: 6874 735f 706f 7320 3d20 7374 7275 6374  hts_pos = struct
-00003590: 7572 655f 7765 6967 6874 202b 2028 3120  ure_weight + (1 
-000035a0: 2d20 7374 7275 6374 7572 655f 7765 6967  - structure_weig
-000035b0: 6874 2920 2a20 2831 202d 2077 6569 6768  ht) * (1 - weigh
-000035c0: 7473 290a 2020 2020 2020 2020 7765 6967  ts).        weig
-000035d0: 6874 735f 6e65 6720 3d20 7374 7275 6374  hts_neg = struct
-000035e0: 7572 655f 7765 6967 6874 202b 2028 3120  ure_weight + (1 
-000035f0: 2d20 7374 7275 6374 7572 655f 7765 6967  - structure_weig
-00003600: 6874 2920 2a20 280a 2020 2020 2020 2020  ht) * (.        
-00003610: 2020 2020 7466 2e72 6573 6861 7065 280a      tf.reshape(.
-00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003630: 7466 2e74 696c 6528 7765 6967 6874 732c  tf.tile(weights,
-00003640: 205b 7365 6c66 2e65 7461 5d29 2c20 5b74   [self.eta]), [t
-00003650: 662e 7368 6170 6528 7765 6967 6874 7329  f.shape(weights)
-00003660: 5b30 5d20 2a20 7365 6c66 2e65 7461 5d0a  [0] * self.eta].
-00003670: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00003680: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00003690: 2072 6574 7572 6e20 7765 6967 6874 735f   return weights_
-000036a0: 706f 732c 2077 6569 6768 7473 5f6e 6567  pos, weights_neg
-000036b0: 0a0a 2020 2020 6465 6620 7472 6169 6e5f  ..    def train_
-000036c0: 7374 6570 2873 656c 662c 2064 6174 6129  step(self, data)
-000036d0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000036e0: 2020 2020 2020 5472 6169 6e69 6e67 2073        Training s
-000036f0: 7465 702e 0a0a 2020 2020 2020 2020 5061  tep...        Pa
-00003700: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00003710: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00003720: 2020 2020 6461 7461 3a20 6172 7261 792d      data: array-
-00003730: 6c69 6b65 2c20 7368 6170 6520 286e 2c20  like, shape (n, 
-00003740: 6d29 0a20 2020 2020 2020 2020 2020 2042  m).            B
-00003750: 6174 6368 206f 6620 696e 7075 7420 7472  atch of input tr
-00003760: 6970 6c65 7320 2874 7275 6520 706f 7369  iples (true posi
-00003770: 7469 7665 7329 2077 6974 6820 7765 6967  tives) with weig
-00003780: 6874 7320 6173 736f 6369 6174 6564 2069  hts associated i
-00003790: 6620 6d3e 332e 0a0a 2020 2020 2020 2020  f m>3...        
-000037a0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-000037b0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-000037c0: 6f75 743a 2064 6963 740a 2020 2020 2020  out: dict.      
-000037d0: 2020 2020 2020 4469 6374 696f 6e61 7279        Dictionary
-000037e0: 206f 6620 6d65 7472 6963 7320 636f 6d70   of metrics comp
-000037f0: 7574 6564 206f 6e20 7468 6520 6f75 7470  uted on the outp
-00003800: 7574 7320 2865 2e67 2e2c 206c 6f73 7329  uts (e.g., loss)
-00003810: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00003820: 2020 2020 2020 6966 2073 656c 662e 6461        if self.da
-00003830: 7461 5f73 6861 7065 203e 2033 3a0a 2020  ta_shape > 3:.  
-00003840: 2020 2020 2020 2020 2020 7472 6970 6c65            triple
-00003850: 7320 3d20 6461 7461 5b30 5d0a 2020 2020  s = data[0].    
-00003860: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00003870: 6461 7461 5f68 616e 646c 6572 2e5f 6164  data_handler._ad
-00003880: 6170 7465 722e 7573 655f 6669 6c74 6572  apter.use_filter
-00003890: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000038a0: 2020 7765 6967 6874 7320 3d20 6461 7461    weights = data
-000038b0: 5b32 5d0a 2020 2020 2020 2020 2020 2020  [2].            
-000038c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000038d0: 2020 2020 2020 7765 6967 6874 7320 3d20        weights = 
-000038e0: 6461 7461 5b31 5d0a 2020 2020 2020 2020  data[1].        
-000038f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00003900: 2020 7472 6970 6c65 7320 3d20 6461 7461    triples = data
-00003910: 0a20 2020 2020 2020 2077 6974 6820 7466  .        with tf
-00003920: 2e47 7261 6469 656e 7454 6170 6528 2920  .GradientTape() 
-00003930: 6173 2074 6170 653a 0a20 2020 2020 2020  as tape:.       
-00003940: 2020 2020 2023 2067 6574 2074 6865 206d       # get the m
-00003950: 6f64 656c 2070 7265 6469 6374 696f 6e73  odel predictions
-00003960: 0a20 2020 2020 2020 2020 2020 2073 636f  .            sco
-00003970: 7265 5f70 6f73 2c20 7363 6f72 655f 6e65  re_pos, score_ne
-00003980: 6720 3d20 7365 6c66 2874 662e 6361 7374  g = self(tf.cast
-00003990: 2874 7269 706c 6573 2c20 7466 2e69 6e74  (triples, tf.int
-000039a0: 3332 292c 2074 7261 696e 696e 673d 3129  32), training=1)
-000039b0: 0a20 2020 2020 2020 2020 2020 2023 2066  .            # f
-000039c0: 6f63 7573 4520 6c61 7965 720a 2020 2020  ocusE layer.    
-000039d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000039e0: 7573 655f 666f 6375 7345 3a0a 2020 2020  use_focusE:.    
-000039f0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00003a00: 6572 2e64 6562 7567 2822 5573 696e 6720  er.debug("Using 
-00003a10: 466f 6375 7345 2229 0a20 2020 2020 2020  FocusE").       
-00003a20: 2020 2020 2020 2020 206e 6f6e 5f6c 696e           non_lin
-00003a30: 6561 7269 7479 203d 2073 656c 662e 666f  earity = self.fo
-00003a40: 6375 7345 5f70 6172 616d 735b 226e 6f6e  cusE_params["non
-00003a50: 5f6c 696e 6561 7269 7479 225d 0a20 2020  _linearity"].   
-00003a60: 2020 2020 2020 2020 2020 2020 2073 7472               str
-00003a70: 7563 7475 7265 5f77 6569 6768 7420 3d20  ucture_weight = 
-00003a80: 7365 6c66 2e66 6f63 7573 455f 7061 7261  self.focusE_para
-00003a90: 6d73 5b22 7374 7275 6374 7572 616c 5f77  ms["structural_w
-00003aa0: 7422 5d0a 0a20 2020 2020 2020 2020 2020  t"]..           
-00003ab0: 2020 2020 2077 6569 6768 7473 5f70 6f73       weights_pos
-00003ac0: 2c20 7765 6967 6874 735f 6e65 6720 3d20  , weights_neg = 
-00003ad0: 7365 6c66 2e63 6f6d 7075 7465 5f66 6f63  self.compute_foc
-00003ae0: 7573 455f 7765 6967 6874 7328 0a20 2020  usE_weights(.   
-00003af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b00: 2077 6569 6768 7473 3d77 6569 6768 7473   weights=weights
-00003b10: 2c20 7374 7275 6374 7572 655f 7765 6967  , structure_weig
-00003b20: 6874 3d73 7472 7563 7475 7265 5f77 6569  ht=structure_wei
-00003b30: 6768 740a 2020 2020 2020 2020 2020 2020  ght.            
-00003b40: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00003b50: 2020 2020 2020 2320 436f 6d70 7574 6174        # Computat
-00003b60: 696f 6e20 6f66 2073 636f 7265 730a 2020  ion of scores.  
-00003b70: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-00003b80: 6f72 655f 706f 7320 3d20 6e6f 6e5f 6c69  ore_pos = non_li
-00003b90: 6e65 6172 6974 7928 7363 6f72 655f 706f  nearity(score_po
-00003ba0: 7329 202a 2077 6569 6768 7473 5f70 6f73  s) * weights_pos
-00003bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003bc0: 2073 636f 7265 5f6e 6567 203d 206e 6f6e   score_neg = non
-00003bd0: 5f6c 696e 6561 7269 7479 2873 636f 7265  _linearity(score
-00003be0: 5f6e 6567 2920 2a20 7765 6967 6874 735f  _neg) * weights_
-00003bf0: 6e65 670a 0a20 2020 2020 2020 2020 2020  neg..           
-00003c00: 2023 2063 6f6d 7075 7465 2074 6865 206c   # compute the l
-00003c10: 6f73 730a 2020 2020 2020 2020 2020 2020  oss.            
-00003c20: 6c6f 7373 203d 2073 656c 662e 636f 6d70  loss = self.comp
-00003c30: 696c 6564 5f6c 6f73 7328 0a20 2020 2020  iled_loss(.     
-00003c40: 2020 2020 2020 2020 2020 2073 636f 7265             score
-00003c50: 5f70 6f73 2c0a 2020 2020 2020 2020 2020  _pos,.          
-00003c60: 2020 2020 2020 7363 6f72 655f 6e65 672c        score_neg,
-00003c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003c80: 2073 656c 662e 6574 612c 0a20 2020 2020   self.eta,.     
-00003c90: 2020 2020 2020 2020 2020 2072 6567 756c             regul
-00003ca0: 6172 697a 6174 696f 6e5f 6c6f 7373 6573  arization_losses
-00003cb0: 3d73 656c 662e 6c6f 7373 6573 2c0a 2020  =self.losses,.  
-00003cc0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00003cd0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00003ce0: 2020 2020 2023 206d 696e 696d 697a 6520       # minimize 
-00003cf0: 7468 6520 6c6f 7373 2061 6e64 2075 7064  the loss and upd
-00003d00: 6174 6520 7468 6520 7472 6169 6e61 626c  ate the trainabl
-00003d10: 6520 7661 7269 6162 6c65 730a 2020 2020  e variables.    
-00003d20: 2020 2020 2020 2020 7365 6c66 2e6f 7074          self.opt
-00003d30: 696d 697a 6572 2e6d 696e 696d 697a 6528  imizer.minimize(
-00003d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003d50: 206c 6f73 732c 0a20 2020 2020 2020 2020   loss,.         
-00003d60: 2020 2020 2020 2073 656c 662e 656e 636f         self.enco
-00003d70: 6469 6e67 5f6c 6179 6572 2e65 6e74 5f65  ding_layer.ent_e
-00003d80: 6d62 2c0a 2020 2020 2020 2020 2020 2020  mb,.            
-00003d90: 2020 2020 7365 6c66 2e65 6e63 6f64 696e      self.encodin
-00003da0: 675f 6c61 7965 722e 7265 6c5f 656d 622c  g_layer.rel_emb,
-00003db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003dc0: 2074 6170 652c 0a20 2020 2020 2020 2020   tape,.         
-00003dd0: 2020 2029 0a20 2020 2020 2020 2065 7863     ).        exc
-00003de0: 6570 7420 5661 6c75 6545 7272 6f72 2061  ept ValueError a
-00003df0: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-00003e00: 2069 6620 7365 6c66 2e73 636f 7269 6e67   if self.scoring
-00003e10: 5f6c 6179 6572 2e6e 616d 6520 3d3d 2022  _layer.name == "
-00003e20: 5261 6e64 6f6d 223a 0a20 2020 2020 2020  Random":.       
-00003e30: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
-00003e40: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00003e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e60: 7261 6973 6520 650a 0a20 2020 2020 2020  raise e..       
-00003e70: 2072 6574 7572 6e20 7b6d 2e6e 616d 653a   return {m.name:
-00003e80: 206d 2e72 6573 756c 7428 2920 666f 7220   m.result() for 
-00003e90: 6d20 696e 2073 656c 662e 6d65 7472 6963  m in self.metric
-00003ea0: 737d 0a0a 2020 2020 6465 6620 6d61 6b65  s}..    def make
-00003eb0: 5f74 7261 696e 5f66 756e 6374 696f 6e28  _train_function(
-00003ec0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00003ed0: 2222 5369 6d69 6c61 7220 746f 206b 6572  ""Similar to ker
-00003ee0: 6173 206c 6962 2c20 7468 6973 2066 756e  as lib, this fun
-00003ef0: 6374 696f 6e20 7265 7475 726e 7320 7468  ction returns th
-00003f00: 6520 6861 6e64 6c65 2074 6f20 7468 6520  e handle to the 
-00003f10: 7472 6169 6e69 6e67 2073 7465 7020 6675  training step fu
-00003f20: 6e63 7469 6f6e 2e0a 2020 2020 2020 2020  nction..        
-00003f30: 4974 2070 726f 6365 7373 6573 206f 6e65  It processes one
-00003f40: 2062 6174 6368 206f 6620 6461 7461 2062   batch of data b
-00003f50: 7920 6974 6572 6174 696e 6720 6f76 6572  y iterating over
-00003f60: 2074 6865 2064 6174 6173 6574 2069 7465   the dataset ite
-00003f70: 7261 746f 722c 2069 7420 636f 6d70 7574  rator, it comput
-00003f80: 6573 2074 6865 206c 6f73 7320 616e 6420  es the loss and 
-00003f90: 6f70 7469 6d69 7a65 7320 6f6e 2069 742e  optimizes on it.
-00003fa0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00003fb0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00003fc0: 2d0a 2020 2020 2020 2020 6f75 743a 2046  -.        out: F
-00003fd0: 756e 6374 696f 6e20 6861 6e64 6c65 0a20  unction handle. 
-00003fe0: 2020 2020 2020 2020 2020 2020 2048 616e               Han
-00003ff0: 646c 6520 746f 2074 6865 2074 7261 696e  dle to the train
-00004000: 696e 6720 7374 6570 2066 756e 6374 696f  ing step functio
-00004010: 6e2e 0a20 2020 2020 2020 2022 2222 0a20  n..        """. 
-00004020: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
-00004030: 7261 696e 5f66 756e 6374 696f 6e20 6973  rain_function is
-00004040: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00004050: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00004060: 6c66 2e74 7261 696e 5f66 756e 6374 696f  lf.train_functio
-00004070: 6e0a 0a20 2020 2020 2020 2064 6566 2074  n..        def t
-00004080: 7261 696e 5f66 756e 6374 696f 6e28 6974  rain_function(it
-00004090: 6572 6174 6f72 293a 0a20 2020 2020 2020  erator):.       
-000040a0: 2020 2020 2022 2222 5468 6973 2069 7320       """This is 
-000040b0: 7468 6520 6675 6e63 7469 6f6e 2077 686f  the function who
-000040c0: 7365 2068 616e 646c 6520 7769 6c6c 2062  se handle will b
-000040d0: 6520 7265 7475 726e 6564 2e0a 0a20 2020  e returned...   
-000040e0: 2020 2020 2020 2020 2050 6172 616d 6574           Paramet
-000040f0: 6572 730a 2020 2020 2020 2020 2020 2020  ers.            
-00004100: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00004110: 2020 2020 2020 2069 7465 7261 746f 723a         iterator:
-00004120: 2074 662e 6461 7461 2e49 7465 7261 746f   tf.data.Iterato
-00004130: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00004140: 2020 4461 7461 2069 7465 7261 746f 722e    Data iterator.
-00004150: 0a0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
-00004160: 7475 726e 730a 2020 2020 2020 2020 2020  turns.          
-00004170: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00004180: 2020 2020 2020 6f75 7470 7574 3a20 6469        output: di
-00004190: 6374 0a20 2020 2020 2020 2020 2020 2020  ct.             
-000041a0: 2052 6574 7572 6e20 6120 6469 6374 696f   Return a dictio
-000041b0: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
-000041c0: 7661 6c75 6573 2074 6861 7420 7769 6c6c  values that will
-000041d0: 2062 6520 7061 7373 6564 2074 6f20 6060   be passed to ``
-000041e0: 7466 2e6b 6572 6173 2e43 616c 6c62 6163  tf.keras.Callbac
-000041f0: 6b73 2e6f 6e5f 7472 6169 6e5f 6261 7463  ks.on_train_batc
-00004200: 685f 656e 6460 602e 0a20 2020 2020 2020  h_end``..       
-00004210: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00004220: 2020 2020 2064 6174 6120 3d20 6e65 7874       data = next
-00004230: 2869 7465 7261 746f 7229 0a20 2020 2020  (iterator).     
-00004240: 2020 2020 2020 206f 7574 7075 7420 3d20         output = 
-00004250: 7365 6c66 2e74 7261 696e 5f73 7465 7028  self.train_step(
-00004260: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
-00004270: 2020 7265 7475 726e 206f 7574 7075 740a    return output.
-00004280: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00004290: 7365 6c66 2e72 756e 5f65 6167 6572 6c79  self.run_eagerly
-000042a0: 2061 6e64 206e 6f74 2073 656c 662e 6973   and not self.is
-000042b0: 5f70 6172 7469 7469 6f6e 6564 5f74 7261  _partitioned_tra
-000042c0: 696e 696e 673a 0a20 2020 2020 2020 2020  ining:.         
-000042d0: 2020 2074 7261 696e 5f66 756e 6374 696f     train_functio
-000042e0: 6e20 3d20 6465 665f 6675 6e63 7469 6f6e  n = def_function
-000042f0: 2e66 756e 6374 696f 6e28 0a20 2020 2020  .function(.     
-00004300: 2020 2020 2020 2020 2020 2074 7261 696e             train
-00004310: 5f66 756e 6374 696f 6e2c 2065 7870 6572  _function, exper
-00004320: 696d 656e 7461 6c5f 7265 6c61 785f 7368  imental_relax_sh
-00004330: 6170 6573 3d54 7275 650a 2020 2020 2020  apes=True.      
-00004340: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00004350: 2073 656c 662e 7472 6169 6e5f 6675 6e63   self.train_func
-00004360: 7469 6f6e 203d 2074 7261 696e 5f66 756e  tion = train_fun
-00004370: 6374 696f 6e0a 2020 2020 2020 2020 7265  ction.        re
-00004380: 7475 726e 2073 656c 662e 7472 6169 6e5f  turn self.train_
-00004390: 6675 6e63 7469 6f6e 0a0a 2020 2020 6465  function..    de
-000043a0: 6620 6765 745f 666f 6375 7345 5f70 6172  f get_focusE_par
-000043b0: 616d 7328 7365 6c66 2c20 6469 6374 5f70  ams(self, dict_p
-000043c0: 6172 616d 733d 7b7d 293a 0a20 2020 2020  arams={}):.     
-000043d0: 2020 2022 2222 4765 7420 7061 7261 6d65     """Get parame
-000043e0: 7465 7273 2066 6f72 2066 6f63 7573 452e  ters for focusE.
-000043f0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00004400: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00004410: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00004420: 6469 6374 5f70 6172 616d 733a 2064 6963  dict_params: dic
-00004430: 740a 2020 2020 2020 2020 2020 2020 5468  t.            Th
-00004440: 6520 666f 6c6c 6f77 696e 6720 6879 7065  e following hype
-00004450: 722d 7061 7261 6d73 2063 616e 2062 6520  r-params can be 
-00004460: 7061 7373 6564 3a0a 0a20 2020 2020 2020  passed:..       
-00004470: 2020 2020 202d 2022 6e6f 6e5f 6c69 6e65       - "non_line
-00004480: 6172 6974 7922 3a20 6361 6e20 6173 7375  arity": can assu
-00004490: 6d65 206f 6620 7468 6520 666f 6c6c 6f77  me of the follow
-000044a0: 696e 6720 7661 6c75 6573 2060 226c 696e  ing values `"lin
-000044b0: 6561 7222 602c 2060 2273 6f66 7470 6c75  ear"`, `"softplu
-000044c0: 7322 602c 2060 2273 6967 6d6f 6964 2260  s"`, `"sigmoid"`
-000044d0: 2c20 6022 7461 6e68 2260 2e0a 2020 2020  , `"tanh"`..    
-000044e0: 2020 2020 2020 2020 2d20 2273 746f 705f          - "stop_
-000044f0: 6570 6f63 6822 3a20 7370 6563 6966 6965  epoch": specifie
-00004500: 7320 686f 7720 6c6f 6e67 2074 6f20 6465  s how long to de
-00004510: 6361 7920 286c 696e 6561 726c 7929 2074  cay (linearly) t
-00004520: 6865 2073 7472 7563 7475 7261 6c20 696e  he structural in
-00004530: 666c 7565 6e63 6520 6879 7065 722d 7061  fluence hyper-pa
-00004540: 7261 6d65 7465 7220 5c0a 2020 2020 2020  rameter \.      
-00004550: 2020 2020 2020 6672 6f6d 2031 2075 6e74        from 1 unt
-00004560: 696c 2069 7420 7265 6163 6865 7320 6974  il it reaches it
-00004570: 7320 6f72 6967 696e 616c 2076 616c 7565  s original value
-00004580: 2e0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
-00004590: 2273 7472 7563 7475 7261 6c5f 7774 223a  "structural_wt":
-000045a0: 2073 7472 7563 7475 7261 6c20 696e 666c   structural infl
-000045b0: 7565 6e63 6520 6879 7065 7270 6172 616d  uence hyperparam
-000045c0: 6574 6572 205b 302c 2031 5d20 7468 6174  eter [0, 1] that
-000045d0: 206d 6f64 756c 6174 6573 2074 6865 2069   modulates the i
-000045e0: 6e66 6c75 656e 6365 206f 6620 6772 6170  nfluence of grap
-000045f0: 6820 5c0a 2020 2020 2020 2020 2020 2020  h \.            
-00004600: 746f 706f 6c6f 6779 2e0a 0a20 2020 2020  topology...     
-00004610: 2020 2020 2020 2049 6620 7468 6520 7265         If the re
-00004620: 7370 6563 7469 7665 206b 6579 2069 7320  spective key is 
-00004630: 6d69 7373 696e 673a 2060 606e 6f6e 5f6c  missing: ``non_l
-00004640: 696e 6561 7269 7479 3d22 6c69 6e65 6172  inearity="linear
-00004650: 2260 602c 2060 6073 746f 705f 6570 6f63  "``, ``stop_epoc
-00004660: 683d 3235 3160 6020 616e 6420 6060 7374  h=251`` and ``st
-00004670: 7275 6374 7572 616c 5f77 743d 302e 3030  ructural_wt=0.00
-00004680: 3160 602e 0a0a 2020 2020 2020 2020 5265  1``...        Re
-00004690: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-000046a0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 666f  -----.        fo
-000046b0: 6375 7345 5f70 6172 616d 7320 3a20 7475  cusE_params : tu
-000046c0: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
-000046d0: 4120 7475 706c 6520 636f 6e74 6169 6e69  A tuple containi
-000046e0: 6e67 2074 6872 6565 2076 616c 7565 733a  ng three values:
-000046f0: 2074 6865 206e 6f6e 2d6c 696e 6561 7269   the non-lineari
-00004700: 7479 2066 756e 6374 696f 6e20 2860 7374  ty function (`st
-00004710: 7260 292c 2074 6865 2060 7374 6f70 5f65  r`), the `stop_e
-00004720: 706f 6368 6020 2860 696e 7460 2920 616e  poch` (`int`) an
-00004730: 6420 7468 650a 2020 2020 2020 2020 2020  d the.          
-00004740: 2020 7374 7275 6374 7572 6520 7765 6967    structure weig
-00004750: 6874 2028 6066 6c6f 6174 6029 2e0a 0a20  ht (`float`)... 
-00004760: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00004770: 2020 2023 2047 6574 2074 6865 206e 6f6e     # Get the non
-00004780: 2d6c 696e 6561 7269 7479 2066 756e 6374  -linearity funct
-00004790: 696f 6e0a 2020 2020 2020 2020 6e6f 6e5f  ion.        non_
-000047a0: 6c69 6e65 6172 6974 7920 3d20 6469 6374  linearity = dict
-000047b0: 5f70 6172 616d 732e 6765 7428 226e 6f6e  _params.get("non
-000047c0: 5f6c 696e 6561 7269 7479 222c 2022 6c69  _linearity", "li
-000047d0: 6e65 6172 2229 0a20 2020 2020 2020 2069  near").        i
-000047e0: 6620 6e6f 6e5f 6c69 6e65 6172 6974 7920  f non_linearity 
-000047f0: 3d3d 2022 6c69 6e65 6172 223a 0a20 2020  == "linear":.   
-00004800: 2020 2020 2020 2020 206e 6f6e 5f6c 696e           non_lin
-00004810: 6561 7269 7479 203d 2074 662e 6964 656e  earity = tf.iden
-00004820: 7469 7479 0a20 2020 2020 2020 2065 6c69  tity.        eli
-00004830: 6620 6e6f 6e5f 6c69 6e65 6172 6974 7920  f non_linearity 
-00004840: 3d3d 2022 7461 6e68 223a 0a20 2020 2020  == "tanh":.     
-00004850: 2020 2020 2020 206e 6f6e 5f6c 696e 6561         non_linea
-00004860: 7269 7479 203d 2074 662e 7461 6e68 0a20  rity = tf.tanh. 
-00004870: 2020 2020 2020 2065 6c69 6620 6e6f 6e5f         elif non_
-00004880: 6c69 6e65 6172 6974 7920 3d3d 2022 7369  linearity == "si
-00004890: 676d 6f69 6422 3a0a 2020 2020 2020 2020  gmoid":.        
-000048a0: 2020 2020 6e6f 6e5f 6c69 6e65 6172 6974      non_linearit
-000048b0: 7920 3d20 7466 2e73 6967 6d6f 6964 0a20  y = tf.sigmoid. 
-000048c0: 2020 2020 2020 2065 6c69 6620 6e6f 6e5f         elif non_
-000048d0: 6c69 6e65 6172 6974 7920 3d3d 2022 736f  linearity == "so
-000048e0: 6674 706c 7573 223a 0a0a 2020 2020 2020  ftplus":..      
-000048f0: 2020 2020 2020 6465 6620 6e6f 6e5f 6c69        def non_li
-00004900: 6e65 6172 6974 7928 7829 3a0a 2020 2020  nearity(x):.    
-00004910: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00004920: 726e 2074 662e 6d61 7468 2e6c 6f67 2831  rn tf.math.log(1
-00004930: 202b 2039 3939 3920 2a20 7466 2e65 7870   + 9999 * tf.exp
-00004940: 2878 2929 0a0a 2020 2020 2020 2020 656c  (x))..        el
-00004950: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00004960: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00004970: 2822 496e 7661 6c69 6420 666f 6375 7345  ("Invalid focusE
-00004980: 206e 6f6e 2d6c 696e 6561 7269 7479 2229   non-linearity")
-00004990: 0a0a 2020 2020 2020 2020 2320 4765 7420  ..        # Get 
-000049a0: 7468 6520 7374 6f70 5f65 706f 6368 2066  the stop_epoch f
-000049b0: 6f72 2074 6865 2064 6563 6179 0a20 2020  or the decay.   
-000049c0: 2020 2020 2073 746f 705f 6570 6f63 6820       stop_epoch 
-000049d0: 3d20 6469 6374 5f70 6172 616d 732e 6765  = dict_params.ge
-000049e0: 7428 2273 746f 705f 6570 6f63 6822 2c20  t("stop_epoch", 
-000049f0: 3235 3129 0a20 2020 2020 2020 206d 7367  251).        msg
-00004a00: 203d 2022 496e 7661 6c69 6420 7661 6c75   = "Invalid valu
-00004a10: 6520 666f 7220 666f 6375 7345 2073 746f  e for focusE sto
-00004a20: 705f 6570 6f63 683a 2065 7870 6563 7465  p_epoch: expecte
-00004a30: 6420 6120 7661 6c75 6520 3e3d 3020 6275  d a value >=0 bu
-00004a40: 7420 676f 7420 7b7d 222e 666f 726d 6174  t got {}".format
-00004a50: 280a 2020 2020 2020 2020 2020 2020 7374  (.            st
-00004a60: 6f70 5f65 706f 6368 0a20 2020 2020 2020  op_epoch.       
-00004a70: 2029 0a20 2020 2020 2020 2061 7373 6572   ).        asser
-00004a80: 7420 7374 6f70 5f65 706f 6368 203e 3d20  t stop_epoch >= 
-00004a90: 302c 206d 7367 0a0a 2020 2020 2020 2020  0, msg..        
-00004aa0: 2320 4765 7420 7374 7275 6374 7572 616c  # Get structural
-00004ab0: 5f77 740a 2020 2020 2020 2020 7374 7275  _wt.        stru
-00004ac0: 6374 7572 655f 7765 6967 6874 203d 2064  cture_weight = d
-00004ad0: 6963 745f 7061 7261 6d73 2e67 6574 2822  ict_params.get("
-00004ae0: 7374 7275 6374 7572 616c 5f77 7422 2c20  structural_wt", 
-00004af0: 302e 3030 3129 0a20 2020 2020 2020 2061  0.001).        a
-00004b00: 7373 6572 7420 2873 7472 7563 7475 7265  ssert (structure
-00004b10: 5f77 6569 6768 7420 3c3d 2031 2920 616e  _weight <= 1) an
-00004b20: 6420 280a 2020 2020 2020 2020 2020 2020  d (.            
-00004b30: 7374 7275 6374 7572 655f 7765 6967 6874  structure_weight
-00004b40: 203e 3d20 300a 2020 2020 2020 2020 292c   >= 0.        ),
-00004b50: 2022 496e 7661 6c69 6420 666f 6375 7345   "Invalid focusE
-00004b60: 2027 7374 7275 6374 7572 616c 5f77 7427   'structural_wt'
-00004b70: 2070 6173 7365 6421 2049 7420 6861 7320   passed! It has 
-00004b80: 746f 2062 656c 6f6e 6720 746f 205b 302c  to belong to [0,
-00004b90: 315d 2e22 0a0a 2020 2020 2020 2020 2320  1]."..        # 
-00004ba0: 6966 2073 746f 705f 6570 6f63 6820 3d3d  if stop_epoch ==
-00004bb0: 2030 2c20 6669 7865 6420 7374 7275 6374   0, fixed struct
-00004bc0: 7572 6520 7765 6967 6874 7320 6973 2075  ure weights is u
-00004bd0: 7365 640a 2020 2020 2020 2020 6966 2073  sed.        if s
-00004be0: 746f 705f 6570 6f63 6820 3e20 303a 0a20  top_epoch > 0:. 
-00004bf0: 2020 2020 2020 2020 2020 2023 206c 696e             # lin
-00004c00: 6561 7220 6465 6361 7920 6f66 206e 756d  ear decay of num
-00004c10: 6572 6963 2076 616c 7565 730a 2020 2020  eric values.    
-00004c20: 2020 2020 2020 2020 7374 7275 6374 7572          structur
-00004c30: 655f 7765 6967 6874 203d 2074 662e 6d61  e_weight = tf.ma
-00004c40: 7869 6d75 6d28 0a20 2020 2020 2020 2020  ximum(.         
-00004c50: 2020 2020 2020 2031 202d 2073 656c 662e         1 - self.
-00004c60: 6375 7272 656e 745f 6570 6f63 6820 2f20  current_epoch / 
-00004c70: 7374 6f70 5f65 706f 6368 2c20 302e 3030  stop_epoch, 0.00
-00004c80: 310a 2020 2020 2020 2020 2020 2020 290a  1.            ).
-00004c90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004ca0: 6e6f 6e5f 6c69 6e65 6172 6974 792c 2073  non_linearity, s
-00004cb0: 746f 705f 6570 6f63 682c 2073 7472 7563  top_epoch, struc
-00004cc0: 7475 7265 5f77 6569 6768 740a 0a20 2020  ture_weight..   
-00004cd0: 2064 6566 2075 7064 6174 655f 666f 6375   def update_focu
-00004ce0: 7345 5f70 6172 616d 7328 7365 6c66 293a  sE_params(self):
-00004cf0: 0a20 2020 2020 2020 2022 2222 5570 6461  .        """Upda
-00004d00: 7465 2074 6865 2073 7472 7563 7475 7261  te the structura
-00004d10: 6c20 7765 6967 6874 2061 6674 6572 2064  l weight after d
-00004d20: 6563 6179 2e22 2222 0a20 2020 2020 2020  ecay.""".       
-00004d30: 2069 6620 7365 6c66 2e66 6f63 7573 455f   if self.focusE_
-00004d40: 7061 7261 6d73 5b22 7374 6f70 5f65 706f  params["stop_epo
-00004d50: 6368 225d 203e 2030 3a0a 2020 2020 2020  ch"] > 0:.      
-00004d60: 2020 2020 2020 7374 6f70 5f65 706f 6368        stop_epoch
-00004d70: 203d 2073 656c 662e 666f 6375 7345 5f70   = self.focusE_p
-00004d80: 6172 616d 735b 2273 746f 705f 6570 6f63  arams["stop_epoc
-00004d90: 6822 5d0a 2020 2020 2020 2020 2020 2020  h"].            
-00004da0: 7365 6c66 2e66 6f63 7573 455f 7061 7261  self.focusE_para
-00004db0: 6d73 5b22 7374 7275 6374 7572 616c 5f77  ms["structural_w
-00004dc0: 7422 5d20 3d20 7466 2e6d 6178 696d 756d  t"] = tf.maximum
-00004dd0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00004de0: 2020 3120 2d20 7365 6c66 2e63 7572 7265    1 - self.curre
-00004df0: 6e74 5f65 706f 6368 202f 2073 746f 705f  nt_epoch / stop_
-00004e00: 6570 6f63 682c 2030 2e30 3031 0a20 2020  epoch, 0.001.   
-00004e10: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00004e20: 6465 6620 6669 7428 0a20 2020 2020 2020  def fit(.       
-00004e30: 2073 656c 662c 0a20 2020 2020 2020 2078   self,.        x
-00004e40: 3d4e 6f6e 652c 0a20 2020 2020 2020 2062  =None,.        b
-00004e50: 6174 6368 5f73 697a 653d 312c 0a20 2020  atch_size=1,.   
-00004e60: 2020 2020 2065 706f 6368 733d 312c 0a20       epochs=1,. 
-00004e70: 2020 2020 2020 2076 6572 626f 7365 3d54         verbose=T
-00004e80: 7275 652c 0a20 2020 2020 2020 2063 616c  rue,.        cal
-00004e90: 6c62 6163 6b73 3d4e 6f6e 652c 0a20 2020  lbacks=None,.   
-00004ea0: 2020 2020 2076 616c 6964 6174 696f 6e5f       validation_
-00004eb0: 7370 6c69 743d 302e 302c 0a20 2020 2020  split=0.0,.     
-00004ec0: 2020 2076 616c 6964 6174 696f 6e5f 6461     validation_da
-00004ed0: 7461 3d4e 6f6e 652c 0a20 2020 2020 2020  ta=None,.       
-00004ee0: 2073 6875 6666 6c65 3d54 7275 652c 0a20   shuffle=True,. 
-00004ef0: 2020 2020 2020 2069 6e69 7469 616c 5f65         initial_e
-00004f00: 706f 6368 3d30 2c0a 2020 2020 2020 2020  poch=0,.        
-00004f10: 7661 6c69 6461 7469 6f6e 5f62 6174 6368  validation_batch
-00004f20: 5f73 697a 653d 3130 302c 0a20 2020 2020  _size=100,.     
-00004f30: 2020 2076 616c 6964 6174 696f 6e5f 636f     validation_co
-00004f40: 7272 7570 745f 7369 6465 3d22 732c 6f22  rrupt_side="s,o"
-00004f50: 2c0a 2020 2020 2020 2020 7661 6c69 6461  ,.        valida
-00004f60: 7469 6f6e 5f66 7265 713d 3530 2c0a 2020  tion_freq=50,.  
-00004f70: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
-00004f80: 5f62 7572 6e5f 696e 3d31 3030 2c0a 2020  _burn_in=100,.  
-00004f90: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
-00004fa0: 5f66 696c 7465 723d 4661 6c73 652c 0a20  _filter=False,. 
-00004fb0: 2020 2020 2020 2076 616c 6964 6174 696f         validatio
-00004fc0: 6e5f 656e 7469 7469 6573 5f73 7562 7365  n_entities_subse
-00004fd0: 743d 4e6f 6e65 2c0a 2020 2020 2020 2020  t=None,.        
-00004fe0: 7061 7274 6974 696f 6e69 6e67 5f6b 3d31  partitioning_k=1
-00004ff0: 2c0a 2020 2020 2020 2020 666f 6375 7345  ,.        focusE
-00005000: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00005010: 666f 6375 7345 5f70 6172 616d 733d 7b7d  focusE_params={}
-00005020: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-00005030: 2022 2222 4669 7420 7468 6520 6d6f 6465   """Fit the mode
-00005040: 6c20 6f6e 2074 6865 2070 726f 7669 6465  l on the provide
-00005050: 6420 6461 7461 2e0a 0a20 2020 2020 2020  d data...       
-00005060: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00005070: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00005080: 2020 2020 2020 2078 3a20 6e70 2e61 7272         x: np.arr
-00005090: 6179 2c20 7368 6170 6520 286e 2c20 3329  ay, shape (n, 3)
-000050a0: 2c20 6f72 2073 7472 206f 7220 4772 6170  , or str or Grap
-000050b0: 6844 6174 614c 6f61 6465 7220 6f72 2041  hDataLoader or A
-000050c0: 6273 7472 6163 7447 7261 7068 5061 7274  bstractGraphPart
-000050d0: 6974 696f 6e65 720a 2020 2020 2020 2020  itioner.        
-000050e0: 2020 2020 4461 7461 204f 5220 4669 6c65      Data OR File
-000050f0: 6e61 6d65 206f 6620 7468 6520 6461 7461  name of the data
-00005100: 2066 696c 6520 4f52 2044 6174 6120 4861   file OR Data Ha
-00005110: 6e64 6c65 2074 6f20 6265 2075 7365 6420  ndle to be used 
-00005120: 666f 7220 7472 6169 6e69 6e67 2e0a 2020  for training..  
-00005130: 2020 2020 2020 6261 7463 685f 7369 7a65        batch_size
-00005140: 3a20 696e 740a 2020 2020 2020 2020 2020  : int.          
-00005150: 2020 4261 7463 6820 7369 7a65 2074 6f20    Batch size to 
-00005160: 7573 6520 6475 7269 6e67 2074 7261 696e  use during train
-00005170: 696e 672e 0a20 2020 2020 2020 2020 2020  ing..           
-00005180: 204d 6179 2062 6520 6f76 6572 7269 6464   May be overridd
-00005190: 656e 2069 6620 2a2a 782a 2a20 6973 2061  en if **x** is a
-000051a0: 2047 7261 7068 4461 7461 4c6f 6164 6572   GraphDataLoader
-000051b0: 206f 7220 4162 7374 7261 6374 4772 6170   or AbstractGrap
-000051c0: 6850 6172 7469 7469 6f6e 6572 2069 6e73  hPartitioner ins
-000051d0: 7461 6e63 652e 0a20 2020 2020 2020 2065  tance..        e
-000051e0: 706f 6368 733a 2069 6e74 0a20 2020 2020  pochs: int.     
-000051f0: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
-00005200: 2065 706f 6368 7320 746f 2074 7261 696e   epochs to train
-00005210: 2028 6465 6661 756c 743a 2031 292e 0a20   (default: 1).. 
-00005220: 2020 2020 2020 2076 6572 626f 7365 3a20         verbose: 
-00005230: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
-00005240: 2056 6572 626f 7369 7479 2028 6465 6661   Verbosity (defa
-00005250: 756c 743a 2060 5472 7565 6029 2e0a 2020  ult: `True`)..  
-00005260: 2020 2020 2020 6361 6c6c 6261 636b 733a        callbacks:
-00005270: 206c 6973 7420 6f66 2074 662e 6b65 7261   list of tf.kera
-00005280: 732e 6361 6c6c 6261 636b 732e 4361 6c6c  s.callbacks.Call
-00005290: 6261 636b 0a20 2020 2020 2020 2020 2020  back.           
-000052a0: 204c 6973 7420 6f66 2063 616c 6c62 6163   List of callbac
-000052b0: 6b73 2074 6f20 6265 2075 7365 6420 6475  ks to be used du
-000052c0: 7269 6e67 2074 7261 696e 696e 6720 2864  ring training (d
-000052d0: 6566 6175 6c74 3a20 604e 6f6e 6560 292e  efault: `None`).
-000052e0: 0a20 2020 2020 2020 2076 616c 6964 6174  .        validat
-000052f0: 696f 6e5f 7370 6c69 743a 2066 6c6f 6174  ion_split: float
-00005300: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
-00005310: 6964 6174 696f 6e20 7370 6c69 7420 746f  idation split to
-00005320: 2063 6172 7665 206f 7574 206f 6620 2a2a   carve out of **
-00005330: 782a 2a20 2864 6566 6175 6c74 3a20 302e  x** (default: 0.
-00005340: 3029 2028 6375 7272 656e 746c 7920 7375  0) (currently su
-00005350: 7070 6f72 7465 6420 6f6e 6c79 2077 6865  pported only whe
-00005360: 6e20 2a2a 782a 2a20 6973 2061 206e 702e  n **x** is a np.
-00005370: 6172 7261 7929 2e0a 2020 2020 2020 2020  array)..        
-00005380: 7661 6c69 6461 7469 6f6e 5f64 6174 613a  validation_data:
-00005390: 206e 702e 6172 7261 792c 2073 6861 7065   np.array, shape
-000053a0: 2028 6e2c 2033 2920 6f72 2073 7472 206f   (n, 3) or str o
-000053b0: 7220 6047 7261 7068 4461 7461 4c6f 6164  r `GraphDataLoad
-000053c0: 6572 6020 6f72 2060 4162 7374 7261 6374  er` or `Abstract
-000053d0: 4772 6170 6850 6172 7469 7469 6f6e 6572  GraphPartitioner
-000053e0: 600a 2020 2020 2020 2020 2020 2020 4461  `.            Da
-000053f0: 7461 204f 5220 4669 6c65 6e61 6d65 206f  ta OR Filename o
-00005400: 6620 7468 6520 6461 7461 2066 696c 6520  f the data file 
-00005410: 4f52 2044 6174 6120 4861 6e64 6c65 2074  OR Data Handle t
-00005420: 6f20 6265 2075 7365 6420 666f 7220 7661  o be used for va
-00005430: 6c69 6461 7469 6f6e 2e0a 2020 2020 2020  lidation..      
-00005440: 2020 7368 7566 666c 653a 2062 6f6f 6c0a    shuffle: bool.
-00005450: 2020 2020 2020 2020 2020 2020 496e 6469              Indi
-00005460: 6361 7465 7320 7768 6574 6865 7220 746f  cates whether to
-00005470: 2073 6875 6666 6c65 2074 6865 2064 6174   shuffle the dat
-00005480: 6120 6166 7465 7220 6576 6572 7920 6570  a after every ep
-00005490: 6f63 6820 6475 7269 6e67 2074 7261 696e  och during train
-000054a0: 696e 6720 2864 6566 6175 6c74 3a20 6054  ing (default: `T
-000054b0: 7275 6560 292e 0a20 2020 2020 2020 2069  rue`)..        i
-000054c0: 6e69 7469 616c 2065 706f 6368 3a20 696e  nitial epoch: in
-000054d0: 740a 2020 2020 2020 2020 2020 2020 496e  t.            In
-000054e0: 6974 6961 6c20 6570 6f63 6820 6e75 6d62  itial epoch numb
-000054f0: 6572 2028 6465 6661 756c 743a 2031 292e  er (default: 1).
-00005500: 0a20 2020 2020 2020 2076 616c 6964 6174  .        validat
-00005510: 696f 6e5f 6261 7463 685f 7369 7a65 3a20  ion_batch_size: 
-00005520: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00005530: 4261 7463 6820 7369 7a65 2074 6f20 7573  Batch size to us
-00005540: 6520 6475 7269 6e67 2076 616c 6964 6174  e during validat
-00005550: 696f 6e20 2864 6566 6175 6c74 3a20 3130  ion (default: 10
-00005560: 3029 2e0a 2020 2020 2020 2020 2020 2020  0)..            
-00005570: 4d61 7920 6265 206f 7665 7272 6964 6465  May be overridde
-00005580: 6e20 6966 2060 6076 616c 6964 6174 696f  n if ``validatio
-00005590: 6e5f 6461 7461 6060 2069 7320 6047 7261  n_data`` is `Gra
-000055a0: 7068 4461 7461 4c6f 6164 6572 6020 6f72  phDataLoader` or
-000055b0: 2060 4162 7374 7261 6374 4772 6170 6850   `AbstractGraphP
-000055c0: 6172 7469 7469 6f6e 6572 6020 696e 7374  artitioner` inst
-000055d0: 616e 6365 2e0a 2020 2020 2020 2020 7661  ance..        va
-000055e0: 6c69 6461 7469 6f6e 5f66 7265 713a 2069  lidation_freq: i
-000055f0: 6e74 0a20 2020 2020 2020 2020 2020 2049  nt.            I
-00005600: 6e64 6963 6174 6573 2068 6f77 206f 6674  ndicates how oft
-00005610: 656e 2074 6f20 7661 6c69 6461 7465 2028  en to validate (
-00005620: 6465 6661 756c 743a 2035 3029 2e0a 2020  default: 50)..  
-00005630: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
-00005640: 5f62 7572 6e5f 696e 3a20 696e 740a 2020  _burn_in: int.  
-00005650: 2020 2020 2020 2020 2020 5468 6520 6275            The bu
-00005660: 726e 2d69 6e20 7469 6d65 2061 6674 6572  rn-in time after
-00005670: 2077 6869 6368 2074 6865 2076 616c 6964   which the valid
-00005680: 6174 696f 6e20 6b69 636b 7320 696e 2e0a  ation kicks in..
-00005690: 2020 2020 2020 2020 7661 6c69 6461 7469          validati
-000056a0: 6f6e 5f66 696c 7465 723a 2062 6f6f 6c20  on_filter: bool 
-000056b0: 6f72 2064 6963 740a 2020 2020 2020 2020  or dict.        
-000056c0: 2020 2020 5661 6c69 6461 7469 6f6e 2066      Validation f
-000056d0: 696c 7465 7220 746f 2062 6520 7573 6564  ilter to be used
-000056e0: 2e0a 2020 2020 2020 2020 7661 6c69 6461  ..        valida
-000056f0: 7469 6f6e 5f65 6e74 6974 6965 735f 7375  tion_entities_su
-00005700: 6273 6574 3a20 6c69 7374 206f 7220 6e70  bset: list or np
-00005710: 2e61 7272 6179 0a20 2020 2020 2020 2020  .array.         
-00005720: 2020 2053 7562 7365 7420 6f66 2065 6e74     Subset of ent
-00005730: 6974 6965 7320 746f 2062 6520 7573 6564  ities to be used
-00005740: 2066 6f72 2067 656e 6572 6174 696e 6720   for generating 
-00005750: 636f 7272 7570 7469 6f6e 732e 0a0a 2020  corruptions...  
-00005760: 2020 2020 2020 2020 2020 2e2e 204e 6f74            .. Not
-00005770: 6520 3a3a 0a0a 2020 2020 2020 2020 2020  e ::..          
-00005780: 2020 2020 2020 4f6e 6520 6361 6e20 7065        One can pe
-00005790: 7266 6f72 6d20 6561 726c 7920 7374 6f70  rform early stop
-000057a0: 7069 6e67 2075 7369 6e67 2074 6865 2074  ping using the t
-000057b0: 656e 736f 7266 6c6f 7720 6361 6c6c 6261  ensorflow callba
-000057c0: 636b 2060 6074 662e 6b65 7261 732e 6361  ck ``tf.keras.ca
-000057d0: 6c6c 6261 636b 732e 4561 726c 7953 746f  llbacks.EarlySto
-000057e0: 7070 696e 6760 600a 2020 2020 2020 2020  pping``.        
-000057f0: 2020 2020 2020 2020 6173 2073 686f 776e          as shown
-00005800: 2069 6e20 7468 6520 6163 636f 6d70 616e   in the accompan
-00005810: 7969 6e67 2065 7861 6d70 6c65 2062 656c  ying example bel
-00005820: 6f77 2e0a 0a20 2020 2020 2020 2066 6f63  ow...        foc
-00005830: 7573 453a 2062 6f6f 6c0a 2020 2020 2020  usE: bool.      
-00005840: 2020 2020 2020 5370 6563 6966 7920 7768        Specify wh
-00005850: 6574 6865 7220 746f 2069 6e63 6c75 6465  ether to include
-00005860: 2074 6865 2046 6f63 7573 4520 6c61 7965   the FocusE laye
-00005870: 7220 2864 6566 6175 6c74 3a20 6046 616c  r (default: `Fal
-00005880: 7365 6029 2e0a 2020 2020 2020 2020 2020  se`)..          
-00005890: 2020 5468 6520 466f 6375 7345 206c 6179    The FocusE lay
-000058a0: 6572 203a 6369 7465 3a60 7061 6932 3032  er :cite:`pai202
-000058b0: 316c 6561 726e 696e 6760 2061 6c6c 6f77  1learning` allow
-000058c0: 7320 746f 2069 6e6a 6563 7420 6e75 6d65  s to inject nume
-000058d0: 7269 6320 6564 6765 2061 7474 7269 6275  ric edge attribu
-000058e0: 7465 7320 696e 746f 2074 6865 2073 636f  tes into the sco
-000058f0: 7269 6e67 206c 6179 6572 0a20 2020 2020  ring layer.     
-00005900: 2020 2020 2020 206f 6620 6120 7472 6164         of a trad
-00005910: 6974 696f 6e61 6c20 6b6e 6f77 6c65 6467  itional knowledg
-00005920: 6520 6772 6170 6820 656d 6265 6464 696e  e graph embeddin
-00005930: 6720 6172 6368 6974 6563 7475 7265 2e0a  g architecture..
-00005940: 2020 2020 2020 2020 2020 2020 5365 6d61              Sema
-00005950: 6e74 6963 616c 6c79 2c20 7468 6520 6e75  ntically, the nu
-00005960: 6d65 7269 6320 7661 6c75 6520 6361 6e20  meric value can 
-00005970: 7369 676e 6966 7920 696d 706f 7274 616e  signify importan
-00005980: 6365 2c20 756e 6365 7274 6169 6e69 7479  ce, uncertainity
-00005990: 2c20 7369 676e 6966 6963 616e 6365 2c20  , significance, 
-000059a0: 636f 6e66 6964 656e 6365 2e2e 2e0a 2020  confidence....  
-000059b0: 2020 2020 2020 2020 2020 6f66 2061 2074            of a t
-000059c0: 7269 706c 652e 0a0a 2020 2020 2020 2020  riple...        
-000059d0: 2020 2020 2e2e 204e 6f74 6520 3a3a 0a0a      .. Note ::..
-000059e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059f0: 496e 206f 7264 6572 2074 6f20 6163 7469  In order to acti
-00005a00: 7661 7465 2066 6f63 7573 452c 2074 6865  vate focusE, the
-00005a10: 2074 7261 696e 696e 6720 6461 7461 206d   training data m
-00005a20: 7573 7420 6861 7665 2073 6861 7065 2028  ust have shape (
-00005a30: 6e2c 2034 292c 2077 6865 7265 2074 6865  n, 4), where the
-00005a40: 2066 6972 7374 2074 6872 6565 2063 6f6c   first three col
-00005a50: 756d 6e73 0a20 2020 2020 2020 2020 2020  umns.           
-00005a60: 2020 2020 2073 746f 7265 2073 7562 6a65       store subje
-00005a70: 6374 2c20 7072 6564 6963 6174 6520 616e  ct, predicate an
-00005a80: 6420 6f62 6a65 6374 206f 6620 7472 6970  d object of trip
-00005a90: 6c65 732c 2061 6e64 2074 6865 2034 2d74  les, and the 4-t
-00005aa0: 6820 636f 6c75 6d6e 2073 746f 7265 7320  h column stores 
-00005ab0: 7468 6520 6e75 6d65 7269 6361 6c20 6564  the numerical ed
-00005ac0: 6765 2076 616c 7565 0a20 2020 2020 2020  ge value.       
-00005ad0: 2020 2020 2020 2020 2061 7373 6f63 6961           associa
-00005ae0: 7465 6420 7769 7468 2065 6163 6820 7472  ted with each tr
-00005af0: 6970 6c65 2e0a 0a20 2020 2020 2020 2066  iple...        f
-00005b00: 6f63 7573 455f 7061 7261 6d73 3a20 6469  ocusE_params: di
-00005b10: 6374 0a20 2020 2020 2020 2020 2020 2049  ct.            I
-00005b20: 6620 466f 6375 7345 206c 6179 6572 2069  f FocusE layer i
-00005b30: 7320 696e 636c 7564 6564 2c20 7370 6563  s included, spec
-00005b40: 6966 7920 6974 7320 6879 7065 722d 7061  ify its hyper-pa
-00005b50: 7261 6d65 7465 7273 2e0a 2020 2020 2020  rameters..      
-00005b60: 2020 2020 2020 5468 6520 666f 6c6c 6f77        The follow
-00005b70: 696e 6720 6879 7065 722d 7061 7261 6d73  ing hyper-params
-00005b80: 2063 616e 2062 6520 7061 7373 6564 3a0a   can be passed:.
-00005b90: 0a20 2020 2020 2020 2020 2020 202b 2060  .            + `
-00005ba0: 226e 6f6e 5f6c 696e 6561 7269 7479 2260  "non_linearity"`
-00005bb0: 3a20 6361 6e20 6265 206f 6e65 206f 6620  : can be one of 
-00005bc0: 7468 6520 666f 6c6c 6f77 696e 6720 7661  the following va
-00005bd0: 6c75 6573 2060 226c 696e 6561 7222 602c  lues `"linear"`,
-00005be0: 2060 2273 6f66 7470 6c75 7322 602c 2060   `"softplus"`, `
-00005bf0: 2273 6967 6d6f 6964 2260 2c20 6022 7461  "sigmoid"`, `"ta
-00005c00: 6e68 2260 2e0a 2020 2020 2020 2020 2020  nh"`..          
-00005c10: 2020 2b20 6022 7374 6f70 5f65 706f 6368    + `"stop_epoch
-00005c20: 2260 3a20 7370 6563 6966 6965 7320 686f  "`: specifies ho
-00005c30: 7720 6c6f 6e67 2074 6f20 6465 6361 7920  w long to decay 
-00005c40: 286c 696e 6561 726c 7929 2074 6865 206e  (linearly) the n
-00005c50: 756d 6572 6963 2076 616c 7565 7320 6672  umeric values fr
-00005c60: 6f6d 2031 2074 6f20 6f72 6967 696e 616c  om 1 to original
-00005c70: 2076 616c 7565 2e0a 2020 2020 2020 2020   value..        
-00005c80: 2020 2020 2b20 6022 7374 7275 6374 7572      + `"structur
-00005c90: 616c 5f77 7422 603a 2073 7472 7563 7475  al_wt"`: structu
-00005ca0: 7261 6c20 696e 666c 7565 6e63 6520 6879  ral influence hy
-00005cb0: 7065 7270 6172 616d 6574 6572 203a 6d61  perparameter :ma
-00005cc0: 7468 3a60 5c5c 696e 205b 302c 2031 5d60  th:`\\in [0, 1]`
-00005cd0: 2074 6861 7420 6d6f 6475 6c61 7465 7320   that modulates 
-00005ce0: 7468 6520 696e 666c 7565 6e63 6520 6f66  the influence of
-00005cf0: 2067 7261 7068 2074 6f70 6f6c 6f67 792e   graph topology.
-00005d00: 0a0a 2020 2020 2020 2020 2020 2020 4966  ..            If
-00005d10: 2060 6066 6f63 7573 453d 3d54 7275 6560   ``focusE==True`
-00005d20: 6020 616e 6420 6060 666f 6375 7345 5f70  ` and ``focusE_p
-00005d30: 6172 616d 733d 3d64 6963 7428 2960 602c  arams==dict()``,
-00005d40: 2074 6865 6e20 7468 6520 6465 6661 756c   then the defaul
-00005d50: 7420 7661 6c75 6573 2061 7265 2070 6173  t values are pas
-00005d60: 7365 643a 0a20 2020 2020 2020 2020 2020  sed:.           
-00005d70: 2060 606e 6f6e 5f6c 696e 6561 7269 7479   ``non_linearity
-00005d80: 3d22 6c69 6e65 6172 2260 602c 2060 6073  ="linear"``, ``s
-00005d90: 746f 705f 6570 6f63 683d 3235 3160 6020  top_epoch=251`` 
-00005da0: 616e 6420 6060 7374 7275 6374 7572 616c  and ``structural
-00005db0: 5f77 743d 302e 3030 3160 602e 0a0a 2020  _wt=0.001``...  
-00005dc0: 2020 2020 2020 7061 7274 6974 696f 6e69        partitioni
-00005dd0: 6e67 5f6b 3a20 696e 740a 2020 2020 2020  ng_k: int.      
-00005de0: 2020 2020 2020 4e75 6d20 6f66 2070 6172        Num of par
-00005df0: 7469 7469 6f6e 7320 746f 2075 7365 2077  titions to use w
-00005e00: 6869 6c65 2074 7261 696e 696e 6720 2864  hile training (d
-00005e10: 6566 6175 6c74 3a20 312c 2069 2e65 2e2c  efault: 1, i.e.,
-00005e20: 2074 6865 2064 6174 6120 6973 206e 6f74   the data is not
-00005e30: 2070 6172 7469 7469 6f6e 6564 292e 0a20   partitioned).. 
-00005e40: 2020 2020 2020 2020 2020 204d 6179 2062             May b
-00005e50: 6520 6f76 6572 7269 6464 656e 2069 6620  e overridden if 
-00005e60: 6060 7860 6020 6973 2061 6e20 6041 6273  ``x`` is an `Abs
-00005e70: 7472 6163 7447 7261 7068 5061 7274 6974  tractGraphPartit
-00005e80: 696f 6e65 7260 2069 6e73 7461 6e63 652e  ioner` instance.
-00005e90: 0a0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
-00005ea0: 204e 6f74 6520 3a3a 0a0a 2020 2020 2020   Note ::..      
-00005eb0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00005ec0: 756e 6374 696f 6e20 6973 2071 7569 7465  unction is quite
-00005ed0: 2075 7365 6675 6c20 7768 656e 2074 6865   useful when the
-00005ee0: 2073 697a 6520 6f66 2079 6f75 7220 6461   size of your da
-00005ef0: 7461 7365 7420 6973 2065 7874 7265 6d65  taset is extreme
-00005f00: 6c79 206c 6172 6765 2061 6e64 2063 616e  ly large and can
-00005f10: 6e6f 7420 6669 7420 696e 206d 656d 6f72  not fit in memor
-00005f20: 792e 0a20 2020 2020 2020 2020 2020 2020  y..             
-00005f30: 2020 2053 6574 7469 6e67 2074 6869 7320     Setting this 
-00005f40: 746f 2061 206e 756d 6265 7220 7374 7269  to a number stri
-00005f50: 6374 6c79 206c 6172 6765 7220 7468 616e  ctly larger than
-00005f60: 2031 2077 696c 6c20 6175 746f 6d61 7469   1 will automati
-00005f70: 6361 6c6c 7920 7061 7274 6974 696f 6e20  cally partition 
-00005f80: 7468 6520 6461 7461 2075 7369 6e67 0a20  the data using. 
-00005f90: 2020 2020 2020 2020 2020 2020 2020 2060                 `
-00005fa0: 6042 7563 6b65 7447 7261 7068 5061 7274  `BucketGraphPart
-00005fb0: 6974 696f 6e65 7260 602e 0a20 2020 2020  itioner``..     
-00005fc0: 2020 2020 2020 2020 2020 204b 696e 646c             Kindl
-00005fd0: 7920 6368 6563 6b6f 7574 2074 6865 2074  y checkout the t
-00005fe0: 7574 6f72 6961 6c73 2066 6f72 2075 7361  utorials for usa
-00005ff0: 6765 2069 6e20 4164 7661 6e63 6564 206d  ge in Advanced m
-00006000: 6f64 652e 0a0a 2020 2020 2020 2020 5265  ode...        Re
-00006010: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-00006020: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6869  -----.        hi
-00006030: 7374 6f72 793a 2048 6973 746f 7279 206f  story: History o
-00006040: 626a 6563 740a 2020 2020 2020 2020 2020  bject.          
-00006050: 2020 4974 7320 6048 6973 746f 7279 2e68    Its `History.h
-00006060: 6973 746f 7279 6020 6174 7472 6962 7574  istory` attribut
-00006070: 6520 6973 2061 2072 6563 6f72 6420 6f66  e is a record of
-00006080: 2074 7261 696e 696e 6720 6c6f 7373 2076   training loss v
-00006090: 616c 7565 732c 2061 7320 7765 6c6c 2061  alues, as well a
-000060a0: 7320 7661 6c69 6461 7469 6f6e 206c 6f73  s validation los
-000060b0: 730a 2020 2020 2020 2020 2020 2020 616e  s.            an
-000060c0: 6420 7661 6c69 6461 7469 6f6e 206d 6574  d validation met
-000060d0: 7269 6373 2076 616c 7565 732e 0a0a 2020  rics values...  
-000060e0: 2020 2020 2020 4578 616d 706c 650a 2020        Example.  
-000060f0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00006100: 2020 2020 2020 3e3e 3e20 6672 6f6d 2061        >>> from a
-00006110: 6d70 6c69 6772 6170 682e 6461 7461 7365  mpligraph.datase
-00006120: 7473 2069 6d70 6f72 7420 6c6f 6164 5f66  ts import load_f
-00006130: 6231 356b 5f32 3337 0a20 2020 2020 2020  b15k_237.       
-00006140: 203e 3e3e 2066 726f 6d20 616d 706c 6967   >>> from amplig
-00006150: 7261 7068 2e6c 6174 656e 745f 6665 6174  raph.latent_feat
-00006160: 7572 6573 2069 6d70 6f72 7420 5363 6f72  ures import Scor
-00006170: 696e 6742 6173 6564 456d 6265 6464 696e  ingBasedEmbeddin
-00006180: 674d 6f64 656c 0a20 2020 2020 2020 203e  gModel.        >
-00006190: 3e3e 2058 203d 206c 6f61 645f 6662 3135  >> X = load_fb15
-000061a0: 6b5f 3233 3728 290a 2020 2020 2020 2020  k_237().        
-000061b0: 3e3e 3e20 6d6f 6465 6c20 3d20 5363 6f72  >>> model = Scor
-000061c0: 696e 6742 6173 6564 456d 6265 6464 696e  ingBasedEmbeddin
-000061d0: 674d 6f64 656c 2865 7461 3d35 2c0a 2020  gModel(eta=5,.  
-000061e0: 2020 2020 2020 3e3e 3e20 2020 2020 2020        >>>       
-000061f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006200: 2020 2020 2020 2020 2020 2020 206b 3d33               k=3
-00006210: 3030 2c0a 2020 2020 2020 2020 3e3e 3e20  00,.        >>> 
-00006220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006240: 2020 2073 636f 7269 6e67 5f74 7970 653d     scoring_type=
-00006250: 2743 6f6d 706c 4578 272c 0a20 2020 2020  'ComplEx',.     
-00006260: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
-00006270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006280: 2020 2020 2020 2020 2020 7365 6564 3d30            seed=0
-00006290: 290a 2020 2020 2020 2020 3e3e 3e20 6d6f  ).        >>> mo
-000062a0: 6465 6c2e 636f 6d70 696c 6528 6f70 7469  del.compile(opti
-000062b0: 6d69 7a65 723d 2761 6461 6d27 2c20 6c6f  mizer='adam', lo
-000062c0: 7373 3d27 6e6c 6c27 290a 2020 2020 2020  ss='nll').      
-000062d0: 2020 3e3e 3e20 6d6f 6465 6c2e 6669 7428    >>> model.fit(
-000062e0: 585b 2774 7261 696e 275d 2c0a 2020 2020  X['train'],.    
-000062f0: 2020 2020 3e3e 3e20 2020 2020 2020 2020      >>>         
-00006300: 2020 6261 7463 685f 7369 7a65 3d31 3030    batch_size=100
-00006310: 3030 2c0a 2020 2020 2020 2020 3e3e 3e20  00,.        >>> 
-00006320: 2020 2020 2020 2020 2020 6570 6f63 6873            epochs
-00006330: 3d35 290a 2020 2020 2020 2020 4570 6f63  =5).        Epoc
-00006340: 6820 312f 350a 2020 2020 2020 2020 3239  h 1/5.        29
-00006350: 2f32 3920 5b3d 3d3d 3d3d 3d3d 3d3d 3d3d  /29 [===========
-00006360: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006370: 3d3d 3d5d 202d 2032 7320 3731 6d73 2f73  ===] - 2s 71ms/s
-00006380: 7465 7020 2d20 6c6f 7373 3a20 3637 3336  tep - loss: 6736
-00006390: 312e 3330 3437 0a20 2020 2020 2020 2045  1.3047.        E
-000063a0: 706f 6368 2032 2f35 0a20 2020 2020 2020  poch 2/5.       
-000063b0: 2032 392f 3239 205b 3d3d 3d3d 3d3d 3d3d   29/29 [========
-000063c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000063d0: 3d3d 3d3d 3d3d 5d20 2d20 3173 2033 356d  ======] - 1s 35m
-000063e0: 732f 7374 6570 202d 206c 6f73 733a 2036  s/step - loss: 6
-000063f0: 3733 3138 2e36 3039 340a 2020 2020 2020  7318.6094.      
-00006400: 2020 4570 6f63 6820 332f 350a 2020 2020    Epoch 3/5.    
-00006410: 2020 2020 3239 2f32 3920 5b3d 3d3d 3d3d      29/29 [=====
-00006420: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006430: 3d3d 3d3d 3d3d 3d3d 3d5d 202d 2031 7320  =========] - 1s 
-00006440: 3337 6d73 2f73 7465 7020 2d20 6c6f 7373  37ms/step - loss
-00006450: 3a20 3637 3032 302e 3037 3033 0a20 2020  : 67020.0703.   
-00006460: 2020 2020 2045 706f 6368 2034 2f35 0a20       Epoch 4/5. 
-00006470: 2020 2020 2020 2032 392f 3239 205b 3d3d         29/29 [==
-00006480: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006490: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 5d20 2d20  ============] - 
-000064a0: 3173 2033 356d 732f 7374 6570 202d 206c  1s 35ms/step - l
-000064b0: 6f73 733a 2036 3538 3637 2e33 3735 300a  oss: 65867.3750.
-000064c0: 2020 2020 2020 2020 4570 6f63 6820 352f          Epoch 5/
-000064d0: 350a 2020 2020 2020 2020 3239 2f32 3920  5.        29/29 
-000064e0: 5b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  [===============
-000064f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d5d  ===============]
-00006500: 202d 2031 7320 3335 6d73 2f73 7465 7020   - 1s 35ms/step 
-00006510: 2d20 6c6f 7373 3a20 3633 3531 372e 3930  - loss: 63517.90
-00006520: 3632 0a0a 2020 2020 2020 2020 3e3e 3e20  62..        >>> 
-00006530: 2320 4561 726c 7920 7374 6f70 7069 6e67  # Early stopping
-00006540: 2065 7861 6d70 6c65 0a20 2020 2020 2020   example.       
-00006550: 203e 3e3e 2066 726f 6d20 616d 706c 6967   >>> from amplig
-00006560: 7261 7068 2e6c 6174 656e 745f 6665 6174  raph.latent_feat
-00006570: 7572 6573 2069 6d70 6f72 7420 5363 6f72  ures import Scor
-00006580: 696e 6742 6173 6564 456d 6265 6464 696e  ingBasedEmbeddin
-00006590: 674d 6f64 656c 0a20 2020 2020 2020 203e  gModel.        >
-000065a0: 3e3e 2066 726f 6d20 616d 706c 6967 7261  >> from ampligra
-000065b0: 7068 2e64 6174 6173 6574 7320 696d 706f  ph.datasets impo
-000065c0: 7274 206c 6f61 645f 6662 3135 6b5f 3233  rt load_fb15k_23
-000065d0: 370a 2020 2020 2020 2020 3e3e 3e20 6461  7.        >>> da
-000065e0: 7461 7365 7420 3d20 6c6f 6164 5f66 6231  taset = load_fb1
-000065f0: 356b 5f32 3337 2829 0a20 2020 2020 2020  5k_237().       
-00006600: 203e 3e3e 206d 6f64 656c 203d 2053 636f   >>> model = Sco
-00006610: 7269 6e67 4261 7365 6445 6d62 6564 6469  ringBasedEmbeddi
-00006620: 6e67 4d6f 6465 6c28 6574 613d 312c 0a20  ngModel(eta=1,. 
-00006630: 2020 2020 2020 203e 3e3e 2020 2020 2020         >>>      
-00006640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006650: 2020 2020 2020 2020 2020 2020 2020 6b3d                k=
-00006660: 3130 2c0a 2020 2020 2020 2020 3e3e 3e20  10,.        >>> 
-00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006690: 2020 2073 636f 7269 6e67 5f74 7970 653d     scoring_type=
-000066a0: 2754 7261 6e73 4527 290a 2020 2020 2020  'TransE').      
-000066b0: 2020 3e3e 3e20 6d6f 6465 6c2e 636f 6d70    >>> model.comp
-000066c0: 696c 6528 6f70 7469 6d69 7a65 723d 2761  ile(optimizer='a
-000066d0: 6461 6d27 2c20 6c6f 7373 3d27 6d75 6c74  dam', loss='mult
-000066e0: 6963 6c61 7373 5f6e 6c6c 2729 0a20 2020  iclass_nll').   
-000066f0: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
-00006700: 7465 6e73 6f72 666c 6f77 2061 7320 7466  tensorflow as tf
-00006710: 0a20 2020 2020 2020 203e 3e3e 2065 6172  .        >>> ear
-00006720: 6c79 5f73 746f 7020 3d20 7466 2e6b 6572  ly_stop = tf.ker
-00006730: 6173 2e63 616c 6c62 6163 6b73 2e45 6172  as.callbacks.Ear
-00006740: 6c79 5374 6f70 7069 6e67 286d 6f6e 6974  lyStopping(monit
-00006750: 6f72 3d22 7661 6c5f 6d72 7222 2c20 2020  or="val_mrr",   
-00006760: 2020 2020 2020 2020 2023 2077 6869 6368           # which
-00006770: 206d 6574 7269 6373 2074 6f20 6d6f 6e69   metrics to moni
-00006780: 746f 720a 2020 2020 2020 2020 3e3e 3e20  tor.        >>> 
-00006790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067b0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-000067c0: 7469 656e 6365 3d33 2c20 2020 2020 2020  tience=3,       
-000067d0: 2020 2020 2020 2020 2020 2020 2320 4966              # If
-000067e0: 2074 6865 206d 6f6e 6974 6f72 6564 206d   the monitored m
-000067f0: 6574 7269 6320 646f 6573 6e74 2069 6d70  etric doesnt imp
-00006800: 726f 7665 2066 6f72 2074 6865 7365 206d  rove for these m
-00006810: 616e 7920 6368 6563 6b73 2074 6865 206d  any checks the m
-00006820: 6f64 656c 2065 6172 6c79 2073 746f 7073  odel early stops
-00006830: 0a20 2020 2020 2020 203e 3e3e 2020 2020  .        >>>    
-00006840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006860: 2020 2020 2020 2020 2020 2076 6572 626f             verbo
-00006870: 7365 3d31 2c20 2020 2020 2020 2020 2020  se=1,           
-00006880: 2020 2020 2020 2020 2023 2076 6572 626f           # verbo
-00006890: 7369 7479 0a20 2020 2020 2020 203e 3e3e  sity.        >>>
-000068a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000068d0: 6f64 653d 226d 6178 222c 2020 2020 2020  ode="max",      
-000068e0: 2020 2020 2020 2020 2020 2020 2023 2068               # h
-000068f0: 6f77 2074 6f20 636f 6d70 6172 6520 7468  ow to compare th
-00006900: 6520 6d6f 6e69 746f 7265 6420 6d65 7472  e monitored metr
-00006910: 6963 733b 2022 6d61 7822 206d 6561 6e73  ics; "max" means
-00006920: 2068 6967 6865 7220 6973 2062 6574 7465   higher is bette
-00006930: 720a 2020 2020 2020 2020 3e3e 3e20 2020  r.        >>>   
-00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006960: 2020 2020 2020 2020 2020 2020 7265 7374              rest
-00006970: 6f72 655f 6265 7374 5f77 6569 6768 7473  ore_best_weights
-00006980: 3d54 7275 6529 2020 2020 2320 7265 7374  =True)    # rest
-00006990: 6f72 6520 7468 6520 7765 6967 6874 7320  ore the weights 
-000069a0: 7769 7468 2062 6573 7420 7661 6c75 650a  with best value.
-000069b0: 2020 2020 2020 2020 3e3e 3e20 2320 7468          >>> # th
-000069c0: 6520 6561 726c 7920 7374 6f70 7069 6e67  e early stopping
-000069d0: 2069 6e73 7461 6e63 6520 6e65 6564 7320   instance needs 
-000069e0: 746f 2062 6520 7061 7373 6564 2061 7320  to be passed as 
-000069f0: 6361 6c6c 6261 636b 2074 6f20 6669 7420  callback to fit 
-00006a00: 6675 6e63 7469 6f6e 0a20 2020 2020 2020  function.       
-00006a10: 203e 3e3e 206d 6f64 656c 2e66 6974 2864   >>> model.fit(d
-00006a20: 6174 6173 6574 5b27 7472 6169 6e27 5d2c  ataset['train'],
-00006a30: 0a20 2020 2020 2020 203e 3e3e 2020 2020  .        >>>    
-00006a40: 2020 2020 2020 2062 6174 6368 5f73 697a         batch_siz
-00006a50: 653d 3130 3030 302c 0a20 2020 2020 2020  e=10000,.       
-00006a60: 203e 3e3e 2020 2020 2020 2020 2020 2065   >>>           e
-00006a70: 706f 6368 733d 352c 0a20 2020 2020 2020  pochs=5,.       
-00006a80: 203e 3e3e 2020 2020 2020 2020 2020 2076   >>>           v
-00006a90: 616c 6964 6174 696f 6e5f 6672 6571 3d31  alidation_freq=1
-00006aa0: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
-00006ab0: 2020 2020 2020 2020 2320 7661 6c69 6461          # valida
-00006ac0: 7469 6f6e 2066 7265 7175 656e 6379 0a20  tion frequency. 
-00006ad0: 2020 2020 2020 203e 3e3e 2020 2020 2020         >>>      
-00006ae0: 2020 2020 2076 616c 6964 6174 696f 6e5f       validation_
-00006af0: 6261 7463 685f 7369 7a65 3d31 3030 2c20  batch_size=100, 
-00006b00: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00006b10: 7661 6c69 6461 7469 6f6e 2062 6174 6368  validation batch
-00006b20: 2073 697a 650a 2020 2020 2020 2020 3e3e   size.        >>
-00006b30: 3e20 2020 2020 2020 2020 2020 7661 6c69  >           vali
-00006b40: 6461 7469 6f6e 5f62 7572 6e5f 696e 3d33  dation_burn_in=3
-00006b50: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
-00006b60: 2020 2020 2023 2062 7572 6e20 696e 2074       # burn in t
-00006b70: 696d 650a 2020 2020 2020 2020 3e3e 3e20  ime.        >>> 
-00006b80: 2020 2020 2020 2020 2020 7661 6c69 6461            valida
-00006b90: 7469 6f6e 5f63 6f72 7275 7074 5f73 6964  tion_corrupt_sid
-00006ba0: 653d 2773 2c6f 272c 2020 2020 2020 2020  e='s,o',        
-00006bb0: 2020 2023 2077 6869 6368 2073 6964 6520     # which side 
-00006bc0: 746f 2063 6f72 7275 7074 0a20 2020 2020  to corrupt.     
-00006bd0: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
-00006be0: 2076 616c 6964 6174 696f 6e5f 6461 7461   validation_data
-00006bf0: 3d64 6174 6173 6574 5b27 7661 6c69 6427  =dataset['valid'
-00006c00: 5d5b 3a3a 3130 305d 2c20 2320 5661 6c69  ][::100], # Vali
-00006c10: 6461 7469 6f6e 2064 6174 610a 2020 2020  dation data.    
-00006c20: 2020 2020 3e3e 3e20 2020 2020 2020 2020      >>>         
-00006c30: 2020 6361 6c6c 6261 636b 733d 5b65 6172    callbacks=[ear
-00006c40: 6c79 5f73 746f 705d 2920 2020 2020 2020  ly_stop])       
-00006c50: 2020 2020 2020 2020 2020 2023 2050 6173             # Pas
-00006c60: 7320 7468 6520 6561 726c 7920 7374 6f70  s the early stop
-00006c70: 7069 6e67 206f 626a 6563 7420 6173 2061  ping object as a
-00006c80: 2063 616c 6c62 6163 6b0a 2020 2020 2020   callback.      
-00006c90: 2020 4570 6f63 6820 312f 350a 2020 2020    Epoch 1/5.    
-00006ca0: 2020 2020 3239 2f32 3920 5b3d 3d3d 3d3d      29/29 [=====
-00006cb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006cc0: 3d3d 3d3d 3d3d 3d3d 3d5d 202d 2032 7320  =========] - 2s 
-00006cd0: 3832 6d73 2f73 7465 7020 2d20 6c6f 7373  82ms/step - loss
-00006ce0: 3a20 3636 3938 2e32 3138 380a 2020 2020  : 6698.2188.    
-00006cf0: 2020 2020 4570 6f63 6820 322f 350a 2020      Epoch 2/5.  
-00006d00: 2020 2020 2020 3239 2f32 3920 5b3d 3d3d        29/29 [===
-00006d10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006d20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d5d 202d 2031  ===========] - 1
-00006d30: 7320 3334 6d73 2f73 7465 7020 2d20 6c6f  s 34ms/step - lo
-00006d40: 7373 3a20 3636 3438 2e38 3836 320a 2020  ss: 6648.8862.  
-00006d50: 2020 2020 2020 4570 6f63 6820 332f 350a        Epoch 3/5.
-00006d60: 2020 2020 2020 2020 332f 3320 5b3d 3d3d          3/3 [===
-00006d70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006d80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d5d 202d 2031  ===========] - 1
-00006d90: 7320 3434 366d 732f 7374 6570 6f73 733a  s 446ms/steposs:
-00006da0: 2036 3635 322e 3839 350a 2020 2020 2020   6652.895.      
-00006db0: 2020 3239 2f32 3920 5b3d 3d3d 3d3d 3d3d    29/29 [=======
-00006dc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006dd0: 3d3d 3d3d 3d3d 3d5d 202d 2032 7320 3834  =======] - 2s 84
-00006de0: 6d73 2f73 7465 7020 2d20 6c6f 7373 3a20  ms/step - loss: 
-00006df0: 3635 3930 2e32 3834 3220 2d20 7661 6c5f  6590.2842 - val_
-00006e00: 6d72 723a 2030 2e30 3831 3120 2d0a 2020  mrr: 0.0811 -.  
-00006e10: 2020 2020 2020 7661 6c5f 6d72 3a20 3137        val_mr: 17
-00006e20: 3736 2e34 3534 3520 2d20 7661 6c5f 6869  76.4545 - val_hi
-00006e30: 7473 4031 3a20 302e 3030 3030 652b 3030  ts@1: 0.0000e+00
-00006e40: 202d 2076 616c 5f68 6974 7340 3130 3a20   - val_hits@10: 
-00006e50: 302e 3233 3031 202d 2076 616c 5f68 6974  0.2301 - val_hit
-00006e60: 7340 3130 303a 2030 2e34 3134 380a 2020  s@100: 0.4148.  
-00006e70: 2020 2020 2020 4570 6f63 6820 342f 350a        Epoch 4/5.
-00006e80: 2020 2020 2020 2020 332f 3320 5b3d 3d3d          3/3 [===
-00006e90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006ea0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d5d 202d 2030  ===========] - 0
-00006eb0: 7320 3130 326d 732f 7374 6570 6f73 733a  s 102ms/steposs:
-00006ec0: 2036 3536 342e 3032 310a 2020 2020 2020   6564.021.      
-00006ed0: 2020 3239 2f32 3920 5b3d 3d3d 3d3d 3d3d    29/29 [=======
-00006ee0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006ef0: 3d3d 3d3d 3d3d 3d5d 202d 2031 7320 3437  =======] - 1s 47
-00006f00: 6d73 2f73 7465 7020 2d20 6c6f 7373 3a20  ms/step - loss: 
-00006f10: 3635 3137 2e34 3531 3720 2d20 7661 6c5f  6517.4517 - val_
-00006f20: 6d72 723a 2030 2e30 3931 3820 2d0a 2020  mrr: 0.0918 -.  
-00006f30: 2020 2020 2020 7661 6c5f 6d72 3a20 3133        val_mr: 13
-00006f40: 3136 2e36 3333 3520 2d20 7661 6c5f 6869  16.6335 - val_hi
-00006f50: 7473 4031 3a20 302e 3030 3030 652b 3030  ts@1: 0.0000e+00
-00006f60: 202d 2076 616c 5f68 6974 7340 3130 3a20   - val_hits@10: 
-00006f70: 302e 3235 3238 202d 2076 616c 5f68 6974  0.2528 - val_hit
-00006f80: 7340 3130 303a 2030 2e34 3731 360a 2020  s@100: 0.4716.  
-00006f90: 2020 2020 2020 4570 6f63 6820 352f 350a        Epoch 5/5.
-00006fa0: 2020 2020 2020 2020 332f 3320 5b3d 3d3d          3/3 [===
-00006fb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006fc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d5d 202d 2031  ===========] - 1
-00006fd0: 7320 3137 376d 732f 7374 6570 6f73 733a  s 177ms/steposs:
-00006fe0: 2036 3436 382e 3739 380a 2020 2020 2020   6468.798.      
-00006ff0: 2020 3239 2f32 3920 5b3d 3d3d 3d3d 3d3d    29/29 [=======
-00007000: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007010: 3d3d 3d3d 3d3d 3d5d 202d 2032 7320 3632  =======] - 2s 62
-00007020: 6d73 2f73 7465 7020 2d20 6c6f 7373 3a20  ms/step - loss: 
-00007030: 3634 3331 2e38 3639 3620 2d20 7661 6c5f  6431.8696 - val_
-00007040: 6d72 723a 2030 2e30 3930 3120 2d0a 2020  mrr: 0.0901 -.  
-00007050: 2020 2020 2020 7661 6c5f 6d72 3a20 3130        val_mr: 10
-00007060: 3734 2e38 3932 3020 2d20 7661 6c5f 6869  74.8920 - val_hi
-00007070: 7473 4031 3a20 302e 3030 3030 652b 3030  ts@1: 0.0000e+00
-00007080: 202d 2076 616c 5f68 6974 7340 3130 3a20   - val_hits@10: 
-00007090: 302e 3233 3836 202d 2076 616c 5f68 6974  0.2386 - val_hit
-000070a0: 7340 3130 303a 2030 2e34 3737 330a 0a20  s@100: 0.4773.. 
-000070b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000070c0: 2020 2023 2076 6572 6966 6965 7320 6966     # verifies if
-000070d0: 2063 6f6d 7069 6c65 2068 6173 2062 6565   compile has bee
-000070e0: 6e20 6361 6c6c 6564 2062 6566 6f72 6520  n called before 
-000070f0: 6361 6c6c 696e 6720 6669 740a 2020 2020  calling fit.    
-00007100: 2020 2020 7365 6c66 2e5f 6173 7365 7274      self._assert
-00007110: 5f63 6f6d 7069 6c65 5f77 6173 5f63 616c  _compile_was_cal
-00007120: 6c65 6428 290a 2020 2020 2020 2020 2320  led().        # 
-00007130: 666f 6375 7345 0a20 2020 2020 2020 2073  focusE.        s
-00007140: 656c 662e 6375 7272 656e 745f 6570 6f63  elf.current_epoc
-00007150: 6820 3d20 300a 2020 2020 2020 2020 7365  h = 0.        se
-00007160: 6c66 2e75 7365 5f66 6f63 7573 4520 3d20  lf.use_focusE = 
-00007170: 666f 6375 7345 0a0a 2020 2020 2020 2020  focusE..        
-00007180: 2320 7573 6520 7472 6169 6e20 7465 7374  # use train test
-00007190: 2075 6e73 6565 6e20 746f 2073 706c 6974   unseen to split
-000071a0: 2074 7261 696e 696e 6720 7365 740a 2020   training set.  
-000071b0: 2020 2020 2020 6966 2076 616c 6964 6174        if validat
-000071c0: 696f 6e5f 7370 6c69 743a 0a20 2020 2020  ion_split:.     
-000071d0: 2020 2020 2020 2061 7373 6572 7420 6973         assert is
-000071e0: 696e 7374 616e 6365 280a 2020 2020 2020  instance(.      
-000071f0: 2020 2020 2020 2020 2020 782c 206e 702e            x, np.
-00007200: 6e64 6172 7261 790a 2020 2020 2020 2020  ndarray.        
-00007210: 2020 2020 292c 2022 5661 6c69 6461 7469      ), "Validati
-00007220: 6f6e 2073 706c 6974 2073 7570 706f 7274  on split support
-00007230: 6564 2066 6f72 206e 756d 7079 2061 7272  ed for numpy arr
-00007240: 6179 7320 6f6e 6c79 2122 0a20 2020 2020  ays only!".     
-00007250: 2020 2020 2020 2078 2c20 7661 6c69 6461         x, valida
-00007260: 7469 6f6e 5f64 6174 6120 3d20 7472 6169  tion_data = trai
-00007270: 6e5f 7465 7374 5f73 706c 6974 5f6e 6f5f  n_test_split_no_
-00007280: 756e 7365 656e 280a 2020 2020 2020 2020  unseen(.        
-00007290: 2020 2020 2020 2020 782c 0a20 2020 2020          x,.     
-000072a0: 2020 2020 2020 2020 2020 2074 6573 745f             test_
-000072b0: 7369 7a65 3d76 616c 6964 6174 696f 6e5f  size=validation_
-000072c0: 7370 6c69 742c 0a20 2020 2020 2020 2020  split,.         
-000072d0: 2020 2020 2020 2073 6565 643d 7365 6c66         seed=self
-000072e0: 2e73 6565 642c 0a20 2020 2020 2020 2020  .seed,.         
-000072f0: 2020 2020 2020 2061 6c6c 6f77 5f64 7570         allow_dup
-00007300: 6c69 6361 7469 6f6e 3d46 616c 7365 2c0a  lication=False,.
-00007310: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00007320: 2020 2020 2020 2077 6974 6820 7472 6169         with trai
-00007330: 6e69 6e67 5f75 7469 6c73 2e52 6573 7065  ning_utils.Respe
-00007340: 6374 436f 6d70 696c 6564 5472 6169 6e61  ctCompiledTraina
-00007350: 626c 6553 7461 7465 2873 656c 6629 3a0a  bleState(self):.
-00007360: 2020 2020 2020 2020 2020 2020 2320 6372              # cr
-00007370: 6561 7465 2064 6174 6120 6861 6e64 6c65  eate data handle
-00007380: 7220 666f 7220 7468 6520 6461 7461 0a20  r for the data. 
-00007390: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000073a0: 6461 7461 5f68 616e 646c 6572 203d 2064  data_handler = d
-000073b0: 6174 615f 6164 6170 7465 722e 4461 7461  ata_adapter.Data
-000073c0: 4861 6e64 6c65 7228 0a20 2020 2020 2020  Handler(.       
-000073d0: 2020 2020 2020 2020 2078 2c0a 2020 2020           x,.    
-000073e0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-000073f0: 6c3d 7365 6c66 2c0a 2020 2020 2020 2020  l=self,.        
-00007400: 2020 2020 2020 2020 6261 7463 685f 7369          batch_si
-00007410: 7a65 3d62 6174 6368 5f73 697a 652c 0a20  ze=batch_size,. 
-00007420: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00007430: 6174 6173 6574 5f74 7970 653d 2274 7261  ataset_type="tra
-00007440: 696e 222c 0a20 2020 2020 2020 2020 2020  in",.           
-00007450: 2020 2020 2065 706f 6368 733d 6570 6f63       epochs=epoc
-00007460: 6873 2c0a 2020 2020 2020 2020 2020 2020  hs,.            
-00007470: 2020 2020 696e 6974 6961 6c5f 6570 6f63      initial_epoc
-00007480: 683d 696e 6974 6961 6c5f 6570 6f63 682c  h=initial_epoch,
-00007490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000074a0: 2075 7365 5f66 696c 7465 723d 4661 6c73   use_filter=Fals
-000074b0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000074c0: 2020 2023 2069 6620 6d6f 6465 6c20 6973     # if model is
-000074d0: 2061 6c72 6561 6479 0a20 2020 2020 2020   already.       
-000074e0: 2020 2020 2020 2020 2023 2074 7261 696e           # train
-000074f0: 6564 2075 7365 2074 6865 206f 6c64 0a20  ed use the old. 
-00007500: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00007510: 2069 6e64 6578 6572 0a20 2020 2020 2020   indexer.       
-00007520: 2020 2020 2020 2020 2075 7365 5f69 6e64           use_ind
-00007530: 6578 6572 3d73 656c 662e 6461 7461 5f69  exer=self.data_i
-00007540: 6e64 6578 6572 2c0a 2020 2020 2020 2020  ndexer,.        
-00007550: 2020 2020 2020 2020 7061 7274 6974 696f          partitio
-00007560: 6e69 6e67 5f6b 3d70 6172 7469 7469 6f6e  ning_k=partition
-00007570: 696e 675f 6b2c 0a20 2020 2020 2020 2020  ing_k,.         
-00007580: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-00007590: 2020 7365 6c66 2e70 6172 7469 7469 6f6e    self.partition
-000075a0: 6572 5f6d 6574 6164 6174 6120 3d20 280a  er_metadata = (.
-000075b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075c0: 7365 6c66 2e64 6174 615f 6861 6e64 6c65  self.data_handle
-000075d0: 722e 6765 745f 7570 6461 7465 5f70 6172  r.get_update_par
-000075e0: 7469 7469 6f6e 6572 5f6d 6574 6164 6174  titioner_metadat
-000075f0: 6128 0a20 2020 2020 2020 2020 2020 2020  a(.             
-00007600: 2020 2020 2020 2073 656c 662e 6261 7365         self.base
-00007610: 5f64 6972 0a20 2020 2020 2020 2020 2020  _dir.           
-00007620: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00007630: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00007640: 2023 2067 6574 2074 6865 206d 6170 7069   # get the mappi
-00007650: 6e67 2064 6574 6169 6c73 0a20 2020 2020  ng details.     
-00007660: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
-00007670: 5f69 6e64 6578 6572 203d 2073 656c 662e  _indexer = self.
-00007680: 6461 7461 5f68 616e 646c 6572 2e67 6574  data_handler.get
-00007690: 5f6d 6170 7065 7228 290a 2020 2020 2020  _mapper().      
-000076a0: 2020 2020 2020 2320 6765 7420 7468 6520        # get the 
-000076b0: 6d61 7869 6d75 6d20 656e 7469 7469 6573  maximum entities
-000076c0: 2061 6e64 2072 656c 6174 696f 6e73 2074   and relations t
-000076d0: 6861 7420 7769 6c6c 2062 6520 7472 6169  hat will be trai
-000076e0: 6e65 640a 2020 2020 2020 2020 2020 2020  ned.            
-000076f0: 2320 2875 7365 6675 6c20 6475 7269 6e67  # (useful during
-00007700: 2070 6172 7469 7469 6f6e 696e 6729 0a20   partitioning). 
-00007710: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007720: 6d61 785f 656e 745f 7369 7a65 203d 2073  max_ent_size = s
-00007730: 656c 662e 6461 7461 5f68 616e 646c 6572  elf.data_handler
-00007740: 2e5f 6164 6170 7465 722e 6d61 785f 656e  ._adapter.max_en
-00007750: 7469 7469 6573 0a20 2020 2020 2020 2020  tities.         
-00007760: 2020 2073 656c 662e 6d61 785f 7265 6c5f     self.max_rel_
-00007770: 7369 7a65 203d 2073 656c 662e 6461 7461  size = self.data
-00007780: 5f68 616e 646c 6572 2e5f 6164 6170 7465  _handler._adapte
-00007790: 722e 6d61 785f 7265 6c61 7469 6f6e 730a  r.max_relations.
-000077a0: 2020 2020 2020 2020 2020 2020 2320 4e75              # Nu
-000077b0: 6d62 6572 206f 6620 636f 6c75 6d6e 7320  mber of columns 
-000077c0: 2869 2e65 2e2c 206f 6e6c 7920 7472 6970  (i.e., only trip
-000077d0: 6c65 7320 6f72 2061 6c73 6f20 7765 6967  les or also weig
-000077e0: 6874 733f 290a 2020 2020 2020 2020 2020  hts?).          
-000077f0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00007800: 7365 6c66 2e64 6174 615f 6861 6e64 6c65  self.data_handle
-00007810: 722e 5f61 6461 7074 6572 2c20 5061 7274  r._adapter, Part
-00007820: 6974 696f 6e44 6174 614d 616e 6167 6572  itionDataManager
-00007830: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00007840: 2020 2073 656c 662e 6461 7461 5f73 6861     self.data_sha
-00007850: 7065 203d 2028 0a20 2020 2020 2020 2020  pe = (.         
-00007860: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007870: 6461 7461 5f68 616e 646c 6572 2e5f 7061  data_handler._pa
-00007880: 7265 6e74 5f61 6461 7074 6572 2e62 6163  rent_adapter.bac
-00007890: 6b65 6e64 2e64 6174 615f 7368 6170 650a  kend.data_shape.
-000078a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078b0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-000078c0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000078d0: 2020 2020 7365 6c66 2e64 6174 615f 7368      self.data_sh
-000078e0: 6170 6520 3d20 7365 6c66 2e64 6174 615f  ape = self.data_
-000078f0: 6861 6e64 6c65 722e 5f61 6461 7074 6572  handler._adapter
-00007900: 2e62 6163 6b65 6e64 2e64 6174 615f 7368  .backend.data_sh
-00007910: 6170 650a 0a20 2020 2020 2020 2020 2020  ape..           
-00007920: 2023 2046 6f63 7573 450a 2020 2020 2020   # FocusE.      
-00007930: 2020 2020 2020 6966 2073 656c 662e 6461        if self.da
-00007940: 7461 5f73 6861 7065 203c 2034 3a0a 2020  ta_shape < 4:.  
-00007950: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00007960: 6c66 2e75 7365 5f66 6f63 7573 4520 3d20  lf.use_focusE = 
-00007970: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-00007980: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00007990: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000079a0: 7573 655f 666f 6375 7345 3a0a 2020 2020  use_focusE:.    
-000079b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079c0: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
-000079d0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-000079e0: 2020 2020 2020 2020 2020 2066 6f63 7573             focus
-000079f0: 455f 7061 7261 6d73 2c20 6469 6374 0a20  E_params, dict. 
-00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a10: 2020 2029 2c20 2266 6f63 7573 4520 7061     ), "focusE pa
-00007a20: 7261 6d65 7465 7273 206e 6565 6420 746f  rameters need to
-00007a30: 2062 6520 696e 2061 2064 6963 7421 220a   be in a dict!".
-00007a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a50: 2020 2020 2320 4465 6669 6e65 2046 6f63      # Define Foc
-00007a60: 7573 4520 7061 7261 6d73 0a20 2020 2020  usE params.     
-00007a70: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00007a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007a90: 2020 2020 2020 2020 206e 6f6e 5f6c 696e           non_lin
-00007aa0: 6561 7269 7479 2c0a 2020 2020 2020 2020  earity,.        
+00001a20: 2020 2020 2073 656c 662e 6461 7461 5f73       self.data_s
+00001a30: 6861 7065 203d 204e 6f6e 650a 0a20 2020  hape = None..   
+00001a40: 2020 2020 2073 656c 662e 7365 6564 203d       self.seed =
+00001a50: 2073 6565 640a 2020 2020 2020 2020 7365   seed.        se
+00001a60: 6c66 2e62 6173 655f 6469 7220 3d20 7465  lf.base_dir = te
+00001a70: 6d70 6669 6c65 2e67 6574 7465 6d70 6469  mpfile.gettempdi
+00001a80: 7228 290a 2020 2020 2020 2020 7365 6c66  r().        self
+00001a90: 2e70 6172 7469 7469 6f6e 6572 5f6d 6574  .partitioner_met
+00001aa0: 6164 6174 6120 3d20 7b7d 0a0a 2020 2020  adata = {}..    
+00001ab0: 6465 6620 6973 5f66 6974 2873 656c 6629  def is_fit(self)
+00001ac0: 3a0a 2020 2020 2020 2020 2222 2243 6865  :.        """Che
+00001ad0: 636b 2077 6865 7468 6572 2074 6865 206d  ck whether the m
+00001ae0: 6f64 656c 2068 6173 2062 6565 6e20 6669  odel has been fi
+00001af0: 7474 6564 2061 6c72 6561 6479 2e22 2222  tted already."""
+00001b00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001b10: 7365 6c66 2e69 735f 6669 7474 6564 0a0a  self.is_fitted..
+00001b20: 2020 2020 6465 6620 636f 6d70 7574 655f      def compute_
+00001b30: 6f75 7470 7574 5f73 6861 7065 2873 656c  output_shape(sel
+00001b40: 662c 2069 6e70 7574 5368 6170 6529 3a0a  f, inputShape):.
+00001b50: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+00001b60: 6e73 2074 6865 206f 7574 7075 7420 7368  ns the output sh
+00001b70: 6170 6520 6f66 2074 6865 206f 7574 7075  ape of the outpu
+00001b80: 7473 206f 6620 7468 6520 6361 6c6c 2066  ts of the call f
+00001b90: 756e 6374 696f 6e2e 0a0a 2020 2020 2020  unction...      
+00001ba0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00001bb0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+00001bc0: 2020 2020 2020 2020 696e 7075 745f 7368          input_sh
+00001bd0: 6170 653a 2074 7570 6c65 0a20 2020 2020  ape: tuple.     
+00001be0: 2020 2020 2020 2053 6861 7065 206f 6620         Shape of 
+00001bf0: 696e 7075 7473 206f 6620 6361 6c6c 2066  inputs of call f
+00001c00: 756e 6374 696f 6e2e 0a0a 2020 2020 2020  unction...      
+00001c10: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00001c20: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00001c30: 2020 6f75 7470 7574 5f73 6861 7065 3a20    output_shape: 
+00001c40: 6c69 7374 206f 6620 7475 706c 6573 0a20  list of tuples. 
+00001c50: 2020 2020 2020 2020 2020 204c 6973 7420             List 
+00001c60: 7769 7468 2074 6865 2073 6861 7065 206f  with the shape o
+00001c70: 6620 6f75 7470 7574 7320 6f66 2063 616c  f outputs of cal
+00001c80: 6c20 6675 6e63 7469 6f6e 2066 6f72 2074  l function for t
+00001c90: 6865 2069 6e70 7574 2074 7269 706c 6573  he input triples
+00001ca0: 2061 6e64 2074 6865 2063 6f72 7275 7074   and the corrupt
+00001cb0: 696f 6e20 7363 6f72 6573 2e0a 2020 2020  ion scores..    
+00001cc0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00001cd0: 2320 696e 7075 7420 7472 6970 6c65 2073  # input triple s
+00001ce0: 636f 7265 2028 6261 7463 685f 7369 7a65  core (batch_size
+00001cf0: 2c20 3129 2061 6e64 2063 6f72 7275 7074  , 1) and corrupt
+00001d00: 696f 6e20 7363 6f72 6520 2862 6174 6368  ion score (batch
+00001d10: 5f73 697a 6520 2a0a 2020 2020 2020 2020  _size *.        
+00001d20: 2320 6574 612c 2031 290a 2020 2020 2020  # eta, 1).      
+00001d30: 2020 7265 7475 726e 205b 284e 6f6e 652c    return [(None,
+00001d40: 2031 292c 2028 4e6f 6e65 2c20 3129 5d0a   1), (None, 1)].
+00001d50: 0a20 2020 2064 6566 2070 6172 7469 7469  .    def partiti
+00001d60: 6f6e 5f63 6861 6e67 655f 7570 6461 7465  on_change_update
+00001d70: 7328 7365 6c66 2c20 6e75 6d5f 656e 7473  s(self, num_ents
+00001d80: 2c20 656e 745f 656d 622c 2072 656c 5f65  , ent_emb, rel_e
+00001d90: 6d62 293a 0a20 2020 2020 2020 2022 2222  mb):.        """
+00001da0: 5065 7266 6f72 6d20 7468 6520 6368 616e  Perform the chan
+00001db0: 6765 7320 7468 6174 2061 7265 2072 6571  ges that are req
+00001dc0: 7569 7265 6420 7768 656e 2074 6865 2070  uired when the p
+00001dd0: 6172 7469 7469 6f6e 2069 7320 6d6f 6469  artition is modi
+00001de0: 6669 6564 2064 7572 696e 6720 7472 6169  fied during trai
+00001df0: 6e69 6e67 2e0a 0a20 2020 2020 2020 2050  ning...        P
+00001e00: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00001e10: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00001e20: 2020 2020 206e 756d 5f65 6e74 733a 2069       num_ents: i
+00001e30: 6e74 0a20 2020 2020 2020 2020 2020 204e  nt.            N
+00001e40: 756d 6265 7220 6f66 2075 6e69 7175 6520  umber of unique 
+00001e50: 656e 7469 7469 6573 2069 6e20 7468 6520  entities in the 
+00001e60: 7061 7274 6974 696f 6e2e 0a20 2020 2020  partition..     
+00001e70: 2020 2065 6e74 5f65 6d62 3a20 6172 7261     ent_emb: arra
+00001e80: 792d 6c69 6b65 0a20 2020 2020 2020 2020  y-like.         
+00001e90: 2020 2045 6e74 6974 7920 656d 6265 6464     Entity embedd
+00001ea0: 696e 6773 2074 6861 7420 6e65 6564 2074  ings that need t
+00001eb0: 6f20 6265 2074 7261 696e 6564 2066 6f72  o be trained for
+00001ec0: 2074 6865 2070 6172 7469 7469 6f6e 0a20   the partition. 
+00001ed0: 2020 2020 2020 2020 2020 2028 616c 6c20             (all 
+00001ee0: 7472 6970 6c65 7320 6f66 2074 6865 2070  triples of the p
+00001ef0: 6172 7469 7469 6f6e 2077 696c 6c20 6861  artition will ha
+00001f00: 7665 2065 6d62 6564 6469 6e67 7320 696e  ve embeddings in
+00001f10: 2074 6869 7320 6d61 7472 6978 292e 0a20   this matrix).. 
+00001f20: 2020 2020 2020 2072 656c 5f65 6d62 3a20         rel_emb: 
+00001f30: 6172 7261 792d 6c69 6b65 0a20 2020 2020  array-like.     
+00001f40: 2020 2020 2020 2072 656c 6174 696f 6e20         relation 
+00001f50: 656d 6265 6464 696e 6773 2074 6861 7420  embeddings that 
+00001f60: 6e65 6564 2074 6f20 6265 2074 7261 696e  need to be train
+00001f70: 6564 2066 6f72 2074 6865 2070 6172 7469  ed for the parti
+00001f80: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00001f90: 2028 616c 6c20 7472 6970 6c65 7320 6f66   (all triples of
+00001fa0: 2074 6865 2070 6172 7469 7469 6f6e 2077   the partition w
+00001fb0: 696c 6c20 6861 7665 2065 6d62 6564 6469  ill have embeddi
+00001fc0: 6e67 7320 696e 2074 6869 7320 6d61 7472  ngs in this matr
+00001fd0: 6978 292e 0a0a 2020 2020 2020 2020 2222  ix)...        ""
+00001fe0: 220a 2020 2020 2020 2020 2320 7361 7665  ".        # save
+00001ff0: 2074 6865 2075 6e69 7175 6520 656e 7469   the unique enti
+00002000: 7469 6573 206f 6620 7468 6520 7061 7274  ties of the part
+00002010: 6974 696f 6e20 3a20 7769 6c6c 2062 6520  ition : will be 
+00002020: 7573 6564 2066 6f72 0a20 2020 2020 2020  used for.       
+00002030: 2023 2063 6f72 7275 7074 696f 6e20 6765   # corruption ge
+00002040: 6e65 7261 7469 6f6e 0a20 2020 2020 2020  neration.       
+00002050: 2073 656c 662e 6e75 6d5f 656e 7473 203d   self.num_ents =
+00002060: 206e 756d 5f65 6e74 730a 2020 2020 2020   num_ents.      
+00002070: 2020 6966 2073 656c 662e 656e 636f 6469    if self.encodi
+00002080: 6e67 5f6c 6179 6572 2e62 7569 6c74 3a0a  ng_layer.built:.
+00002090: 2020 2020 2020 2020 2020 2020 2320 7570              # up
+000020a0: 6461 7465 2074 6865 2074 7261 696e 6162  date the trainab
+000020b0: 6c65 2076 6172 6961 626c 6520 696e 2074  le variable in t
+000020c0: 6865 2065 6e63 6f64 696e 6720 6c61 7965  he encoding laye
+000020d0: 720a 2020 2020 2020 2020 2020 2020 7365  r.            se
+000020e0: 6c66 2e65 6e63 6f64 696e 675f 6c61 7965  lf.encoding_laye
+000020f0: 722e 7061 7274 6974 696f 6e5f 6368 616e  r.partition_chan
+00002100: 6765 5f75 7064 6174 6573 2865 6e74 5f65  ge_updates(ent_e
+00002110: 6d62 2c20 7265 6c5f 656d 6229 0a20 2020  mb, rel_emb).   
+00002120: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00002130: 2020 2020 2020 2023 2069 6620 7468 6520         # if the 
+00002140: 656e 636f 6469 6e67 206c 6179 6572 2068  encoding layer h
+00002150: 6173 206e 6f74 2062 6565 6e20 6275 696c  as not been buil
+00002160: 7420 7468 656e 2073 746f 7265 2069 7420  t then store it 
+00002170: 6173 2061 6e20 696e 6974 6961 6c69 7a65  as an initialize
+00002180: 720a 2020 2020 2020 2020 2020 2020 2320  r.            # 
+00002190: 7468 6973 2077 6f75 6c64 2062 6520 7468  this would be th
+000021a0: 6520 6361 7365 206f 6620 6475 7269 6e67  e case of during
+000021b0: 2070 6172 7469 7469 6f6e 6564 2074 7261   partitioned tra
+000021c0: 696e 696e 6720 2866 6972 7374 0a20 2020  ining (first.   
+000021d0: 2020 2020 2020 2020 2023 2062 6174 6368           # batch
+000021e0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000021f0: 6c66 2e65 6e63 6f64 696e 675f 6c61 7965  lf.encoding_laye
+00002200: 722e 7365 745f 656e 745f 7265 6c5f 696e  r.set_ent_rel_in
+00002210: 6974 6961 6c5f 7661 6c75 6528 656e 745f  itial_value(ent_
+00002220: 656d 622c 2072 656c 5f65 6d62 290a 0a20  emb, rel_emb).. 
+00002230: 2020 2064 6566 2063 616c 6c28 7365 6c66     def call(self
+00002240: 2c20 696e 7075 7473 2c20 7472 6169 6e69  , inputs, traini
+00002250: 6e67 3d46 616c 7365 293a 0a20 2020 2020  ng=False):.     
+00002260: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+00002270: 6f6d 7075 7465 7320 7468 6520 7363 6f72  omputes the scor
+00002280: 6573 206f 6620 7468 6520 7472 6970 6c65  es of the triple
+00002290: 7320 616e 6420 7265 7475 726e 7320 7468  s and returns th
+000022a0: 6520 636f 7272 7570 7469 6f6e 2073 636f  e corruption sco
+000022b0: 7265 7320 6173 2077 656c 6c2e 0a0a 2020  res as well...  
+000022c0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+000022d0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000022e0: 2d2d 2d0a 2020 2020 2020 2020 696e 7075  ---.        inpu
+000022f0: 7473 3a20 6e64 6172 7261 792c 2073 6861  ts: ndarray, sha
+00002300: 7065 2028 6e2c 2033 290a 2020 2020 2020  pe (n, 3).      
+00002310: 2020 2020 2020 4261 7463 6820 6f66 2069        Batch of i
+00002320: 6e70 7574 2074 7269 706c 6573 2e0a 0a20  nput triples... 
+00002330: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00002340: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00002350: 2020 2020 2020 206f 7574 3a20 6c69 7374         out: list
+00002360: 0a20 2020 2020 2020 2020 2020 204c 6973  .            Lis
+00002370: 7420 6f66 2069 6e70 7574 2073 636f 7265  t of input score
+00002380: 7320 616c 6f6e 6720 7769 7468 2074 6865  s along with the
+00002390: 6972 2063 6f72 7275 7074 696f 6e73 2e0a  ir corruptions..
+000023a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000023b0: 2020 2020 2320 6c6f 6f6b 7570 2065 6d62      # lookup emb
+000023c0: 6564 6469 6e67 7320 6f66 2074 6865 2069  eddings of the i
+000023d0: 6e70 7574 730a 2020 2020 2020 2020 696e  nputs.        in
+000023e0: 705f 656d 6220 3d20 7365 6c66 2e65 6e63  p_emb = self.enc
+000023f0: 6f64 696e 675f 6c61 7965 7228 696e 7075  oding_layer(inpu
+00002400: 7473 290a 2020 2020 2020 2020 2320 7363  ts).        # sc
+00002410: 6f72 6520 7468 6520 696e 7075 7473 0a20  ore the inputs. 
+00002420: 2020 2020 2020 2069 6e70 5f73 636f 7265         inp_score
+00002430: 203d 2073 656c 662e 7363 6f72 696e 675f   = self.scoring_
+00002440: 6c61 7965 7228 696e 705f 656d 6229 0a20  layer(inp_emb). 
+00002450: 2020 2020 2020 2023 2073 636f 7265 2074         # score t
+00002460: 6865 2063 6f72 7275 7074 696f 6e73 0a0a  he corruptions..
+00002470: 2020 2020 2020 2020 6966 2074 7261 696e          if train
+00002480: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
+00002490: 2023 2067 656e 6572 6174 6520 7468 6520   # generate the 
+000024a0: 636f 7272 7570 7469 6f6e 7320 666f 7220  corruptions for 
+000024b0: 7468 6520 696e 7075 7420 7472 6970 6c65  the input triple
+000024c0: 730a 2020 2020 2020 2020 2020 2020 636f  s.            co
+000024d0: 7272 7570 7469 6f6e 7320 3d20 7365 6c66  rruptions = self
+000024e0: 2e63 6f72 7275 7074 696f 6e5f 6c61 7965  .corruption_laye
+000024f0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00002500: 2020 2069 6e70 7574 732c 2073 656c 662e     inputs, self.
+00002510: 6e75 6d5f 656e 7473 2c20 7365 6c66 2e65  num_ents, self.e
+00002520: 7461 0a20 2020 2020 2020 2020 2020 2029  ta.            )
+00002530: 0a20 2020 2020 2020 2020 2020 2023 206c  .            # l
+00002540: 6f6f 6b75 7020 656d 6265 6464 696e 6773  ookup embeddings
+00002550: 206f 6620 7468 6520 696e 7075 7473 0a20   of the inputs. 
+00002560: 2020 2020 2020 2020 2020 2063 6f72 725f             corr_
+00002570: 656d 6220 3d20 7365 6c66 2e65 6e63 6f64  emb = self.encod
+00002580: 696e 675f 6c61 7965 7228 636f 7272 7570  ing_layer(corrup
+00002590: 7469 6f6e 7329 0a20 2020 2020 2020 2020  tions).         
+000025a0: 2020 2063 6f72 725f 7363 6f72 6520 3d20     corr_score = 
+000025b0: 7365 6c66 2e73 636f 7269 6e67 5f6c 6179  self.scoring_lay
+000025c0: 6572 2863 6f72 725f 656d 6229 0a0a 2020  er(corr_emb)..  
+000025d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000025e0: 2069 6e70 5f73 636f 7265 2c20 636f 7272   inp_score, corr
+000025f0: 5f73 636f 7265 0a0a 2020 2020 2020 2020  _score..        
+00002600: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00002610: 2020 7265 7475 726e 2069 6e70 5f73 636f    return inp_sco
+00002620: 7265 0a0a 2020 2020 4074 662e 6675 6e63  re..    @tf.func
+00002630: 7469 6f6e 2865 7870 6572 696d 656e 7461  tion(experimenta
+00002640: 6c5f 7265 6c61 785f 7368 6170 6573 3d54  l_relax_shapes=T
+00002650: 7275 6529 0a20 2020 2064 6566 205f 6765  rue).    def _ge
+00002660: 745f 7261 6e6b 7328 0a20 2020 2020 2020  t_ranks(.       
+00002670: 2073 656c 662c 0a20 2020 2020 2020 2069   self,.        i
+00002680: 6e70 7574 732c 0a20 2020 2020 2020 2065  nputs,.        e
+00002690: 6e74 5f65 6d62 732c 0a20 2020 2020 2020  nt_embs,.       
+000026a0: 2073 7461 7274 5f69 642c 0a20 2020 2020   start_id,.     
+000026b0: 2020 2065 6e64 5f69 642c 0a20 2020 2020     end_id,.     
+000026c0: 2020 2066 696c 7465 7273 2c0a 2020 2020     filters,.    
+000026d0: 2020 2020 6d61 7070 696e 675f 6469 6374      mapping_dict
+000026e0: 2c0a 2020 2020 2020 2020 636f 7272 7570  ,.        corrup
+000026f0: 745f 7369 6465 3d22 732c 6f22 2c0a 2020  t_side="s,o",.  
+00002700: 2020 2020 2020 7261 6e6b 696e 675f 7374        ranking_st
+00002710: 7261 7465 6779 3d22 776f 7273 7422 2c0a  rategy="worst",.
+00002720: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
+00002730: 2222 0a20 2020 2020 2020 2045 7661 6c75  "".        Evalu
+00002740: 6174 6520 7468 6520 696e 7075 7473 2061  ate the inputs a
+00002750: 6761 696e 7374 2063 6f72 7275 7074 696f  gainst corruptio
+00002760: 6e73 2061 6e64 2072 6574 7572 6e20 7261  ns and return ra
+00002770: 6e6b 732e 0a0a 2020 2020 2020 2020 5061  nks...        Pa
+00002780: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00002790: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+000027a0: 2020 2020 696e 7075 7473 3a20 6172 7261      inputs: arra
+000027b0: 792d 6c69 6b65 2c20 7368 6170 6520 286e  y-like, shape (n
+000027c0: 2c20 3329 0a20 2020 2020 2020 2020 2020  , 3).           
+000027d0: 2042 6174 6368 206f 6620 696e 7075 7420   Batch of input 
+000027e0: 7472 6970 6c65 732e 0a20 2020 2020 2020  triples..       
+000027f0: 2065 6e74 5f65 6d62 733a 2061 7272 6179   ent_embs: array
+00002800: 2d6c 696b 652c 2073 6861 7065 2028 6d2c  -like, shape (m,
+00002810: 206b 290a 2020 2020 2020 2020 2020 2020   k).            
+00002820: 536c 6963 6520 6f66 2065 6d62 6564 6469  Slice of embeddi
+00002830: 6e67 206d 6174 7269 7820 2863 6f72 7275  ng matrix (corru
+00002840: 7074 696f 6e73 292e 0a20 2020 2020 2020  ptions)..       
+00002850: 2073 7461 7274 5f69 643a 2069 6e74 0a20   start_id: int. 
+00002860: 2020 2020 2020 2020 2020 204f 7269 6769             Origi
+00002870: 6e61 6c20 6964 206f 6620 7468 6520 6669  nal id of the fi
+00002880: 7273 7420 726f 7720 6f66 2065 6d62 6564  rst row of embed
+00002890: 6469 6e67 206d 6174 7269 7820 2875 7365  ding matrix (use
+000028a0: 6420 6475 7269 6e67 2070 6172 7469 7469  d during partiti
+000028b0: 6f6e 6564 2061 7070 726f 6163 6829 2e0a  oned approach)..
+000028c0: 2020 2020 2020 2020 656e 645f 6964 3a20          end_id: 
+000028d0: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+000028e0: 4f72 6967 696e 616c 2069 6420 6f66 2074  Original id of t
+000028f0: 6865 206c 6173 7420 726f 7720 6f66 2065  he last row of e
+00002900: 6d62 6564 6469 6e67 206d 6174 7269 7820  mbedding matrix 
+00002910: 2875 7365 6420 6475 7269 6e67 2070 6172  (used during par
+00002920: 7469 7469 6f6e 6564 2061 7070 726f 6163  titioned approac
+00002930: 6829 2e0a 2020 2020 2020 2020 6669 6c74  h)..        filt
+00002940: 6572 733a 206c 6973 7420 6f66 206c 6973  ers: list of lis
+00002950: 7473 0a20 2020 2020 2020 2020 2020 2053  ts.            S
+00002960: 697a 6520 6f66 206c 6973 7420 6973 2065  ize of list is e
+00002970: 6974 6865 7220 3120 6f72 2032 2064 6570  ither 1 or 2 dep
+00002980: 656e 6469 6e67 206f 6e20 6060 636f 7272  ending on ``corr
+00002990: 7570 745f 7369 6465 6060 2e0a 2020 2020  upt_side``..    
+000029a0: 2020 2020 2020 2020 5369 7a65 206f 6620          Size of 
+000029b0: 7468 6520 696e 7465 726e 616c 206c 6973  the internal lis
+000029c0: 7420 6973 2065 7175 616c 2074 6f20 7468  t is equal to th
+000029d0: 6520 7369 7a65 206f 6620 7468 6520 696e  e size of the in
+000029e0: 7075 7420 7472 6970 6c65 732e 0a20 2020  put triples..   
+000029f0: 2020 2020 2020 2020 2045 6163 6820 6c69           Each li
+00002a00: 7374 2063 6f6e 7461 696e 7320 616e 2061  st contains an a
+00002a10: 7272 6179 206f 6620 6669 6c74 6572 7320  rray of filters 
+00002a20: 2869 2e65 2e2c 2054 7275 6520 506f 7369  (i.e., True Posi
+00002a30: 7469 7665 7329 2072 656c 6174 6564 2074  tives) related t
+00002a40: 6f20 7468 6520 7370 6563 6966 6965 6420  o the specified 
+00002a50: 7369 6465 206f 6620 7468 650a 2020 2020  side of the.    
+00002a60: 2020 2020 2020 2020 636f 7272 6573 706f          correspo
+00002a70: 6e64 696e 6720 696e 7075 7420 7472 6970  nding input trip
+00002a80: 6c65 732e 0a20 2020 2020 2020 2063 6f72  les..        cor
+00002a90: 7275 7074 5f73 6964 653a 2073 7472 0a20  rupt_side: str. 
+00002aa0: 2020 2020 2020 2020 2020 2057 6869 6368             Which
+00002ab0: 2073 6964 6520 746f 2063 6f72 7275 7074   side to corrupt
+00002ac0: 2064 7572 696e 6720 6576 616c 7561 7469   during evaluati
+00002ad0: 6f6e 2e0a 2020 2020 2020 2020 7261 6e6b  on..        rank
+00002ae0: 696e 675f 7374 7261 7465 6779 3a20 7374  ing_strategy: st
+00002af0: 720a 2020 2020 2020 2020 2020 2020 496e  r.            In
+00002b00: 6469 6361 7465 7320 686f 7720 746f 2062  dicates how to b
+00002b10: 7265 616b 2074 6965 7320 2864 6566 6175  reak ties (defau
+00002b20: 6c74 3a20 6077 6f72 7374 602c 2069 2e65  lt: `worst`, i.e
+00002b30: 2e2c 2061 7373 6967 6e73 2074 6865 2077  ., assigns the w
+00002b40: 6f72 7374 2072 616e 6b20 746f 2074 6865  orst rank to the
+00002b50: 2074 6573 7420 7472 6970 6c65 292e 0a20   test triple).. 
+00002b60: 2020 2020 2020 2020 2020 2043 616e 2062             Can b
+00002b70: 6520 6f6e 6520 6f66 2074 6865 2074 6872  e one of the thr
+00002b80: 6565 2074 7970 6573 2060 2262 6573 7422  ee types `"best"
+00002b90: 602c 2060 226d 6964 646c 6522 602c 2060  `, `"middle"`, `
+00002ba0: 2277 6f72 7374 2260 2e0a 0a20 2020 2020  "worst"`...     
+00002bb0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00002bc0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00002bd0: 2020 2072 616e 6b3a 2074 662e 5465 6e73     rank: tf.Tens
+00002be0: 6f72 2c20 7368 6170 6520 286e 2c20 6e75  or, shape (n, nu
+00002bf0: 6d20 6f66 2073 6964 6573 2062 6569 6e67  m of sides being
+00002c00: 2063 6f72 7275 7074 6564 290a 2020 2020   corrupted).    
+00002c10: 2020 2020 2020 2020 5261 6e6b 696e 6720          Ranking 
+00002c20: 6167 6169 6e73 7420 7375 626a 6563 7420  against subject 
+00002c30: 636f 7272 7570 7469 6f6e 7320 616e 6420  corruptions and 
+00002c40: 6f62 6a65 6374 2063 6f72 7275 7074 696f  object corruptio
+00002c50: 6e73 0a20 2020 2020 2020 2020 2020 2028  ns.            (
+00002c60: 636f 7272 7570 7469 6f6e 7320 6465 6669  corruptions defi
+00002c70: 6e65 6420 6279 2060 656e 745f 656d 6273  ned by `ent_embs
+00002c80: 6020 6d61 7472 6978 292e 0a20 2020 2020  ` matrix)..     
+00002c90: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00002ca0: 6620 6e6f 7420 7365 6c66 2e69 735f 7061  f not self.is_pa
+00002cb0: 7274 6974 696f 6e65 645f 7472 6169 6e69  rtitioned_traini
+00002cc0: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+00002cd0: 696e 7075 7473 203d 205b 0a20 2020 2020  inputs = [.     
+00002ce0: 2020 2020 2020 2020 2020 2074 662e 6e6e             tf.nn
+00002cf0: 2e65 6d62 6564 6469 6e67 5f6c 6f6f 6b75  .embedding_looku
+00002d00: 7028 0a20 2020 2020 2020 2020 2020 2020  p(.             
+00002d10: 2020 2020 2020 2073 656c 662e 656e 636f         self.enco
+00002d20: 6469 6e67 5f6c 6179 6572 2e65 6e74 5f65  ding_layer.ent_e
+00002d30: 6d62 2c20 696e 7075 7473 5b3a 2c20 305d  mb, inputs[:, 0]
+00002d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002d50: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00002d60: 2020 2020 7466 2e6e 6e2e 656d 6265 6464      tf.nn.embedd
+00002d70: 696e 675f 6c6f 6f6b 7570 280a 2020 2020  ing_lookup(.    
+00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d90: 7365 6c66 2e65 6e63 6f64 696e 675f 6c61  self.encoding_la
+00002da0: 7965 722e 7265 6c5f 656d 622c 2069 6e70  yer.rel_emb, inp
+00002db0: 7574 735b 3a2c 2031 5d0a 2020 2020 2020  uts[:, 1].      
+00002dc0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+00002dd0: 2020 2020 2020 2020 2020 2020 2074 662e               tf.
+00002de0: 6e6e 2e65 6d62 6564 6469 6e67 5f6c 6f6f  nn.embedding_loo
+00002df0: 6b75 7028 0a20 2020 2020 2020 2020 2020  kup(.           
+00002e00: 2020 2020 2020 2020 2073 656c 662e 656e           self.en
+00002e10: 636f 6469 6e67 5f6c 6179 6572 2e65 6e74  coding_layer.ent
+00002e20: 5f65 6d62 2c20 696e 7075 7473 5b3a 2c20  _emb, inputs[:, 
+00002e30: 325d 0a20 2020 2020 2020 2020 2020 2020  2].             
+00002e40: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+00002e50: 2020 5d0a 0a20 2020 2020 2020 2072 6574    ]..        ret
+00002e60: 7572 6e20 7365 6c66 2e73 636f 7269 6e67  urn self.scoring
+00002e70: 5f6c 6179 6572 2e67 6574 5f72 616e 6b73  _layer.get_ranks
+00002e80: 280a 2020 2020 2020 2020 2020 2020 696e  (.            in
+00002e90: 7075 7473 2c0a 2020 2020 2020 2020 2020  puts,.          
+00002ea0: 2020 656e 745f 656d 6273 2c0a 2020 2020    ent_embs,.    
+00002eb0: 2020 2020 2020 2020 7374 6172 745f 6964          start_id
+00002ec0: 2c0a 2020 2020 2020 2020 2020 2020 656e  ,.            en
+00002ed0: 645f 6964 2c0a 2020 2020 2020 2020 2020  d_id,.          
+00002ee0: 2020 6669 6c74 6572 732c 0a20 2020 2020    filters,.     
+00002ef0: 2020 2020 2020 206d 6170 7069 6e67 5f64         mapping_d
+00002f00: 6963 742c 0a20 2020 2020 2020 2020 2020  ict,.           
+00002f10: 2063 6f72 7275 7074 5f73 6964 652c 0a20   corrupt_side,. 
+00002f20: 2020 2020 2020 2020 2020 2072 616e 6b69             ranki
+00002f30: 6e67 5f73 7472 6174 6567 792c 0a20 2020  ng_strategy,.   
+00002f40: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00002f50: 6275 696c 6428 7365 6c66 2c20 696e 7075  build(self, inpu
+00002f60: 745f 7368 6170 6529 3a0a 2020 2020 2020  t_shape):.      
+00002f70: 2020 2222 224f 7665 7272 6964 6520 7468    """Override th
+00002f80: 6520 6275 696c 6420 6675 6e63 7469 6f6e  e build function
+00002f90: 206f 6620 7468 6520 4d6f 6465 6c20 636c   of the Model cl
+00002fa0: 6173 732e 0a0a 2020 2020 2020 2020 4974  ass...        It
+00002fb0: 2069 7320 6361 6c6c 6564 206f 6e20 7468   is called on th
+00002fc0: 6520 6669 7273 7420 6361 6c6c 2074 6f20  e first call to 
+00002fd0: 6060 5f5f 6361 6c6c 5f5f 6060 2e0a 2020  ``__call__``..  
+00002fe0: 2020 2020 2020 5769 7468 2074 6869 7320        With this 
+00002ff0: 6675 6e63 7469 6f6e 2077 6520 7365 7420  function we set 
+00003000: 736f 6d65 2069 6e74 6572 6e61 6c20 7061  some internal pa
+00003010: 7261 6d65 7465 7273 206f 6620 7468 6520  rameters of the 
+00003020: 656e 636f 6469 6e67 206c 6179 6572 7320  encoding layers 
+00003030: 286e 6565 6465 6420 746f 2062 7569 6c64  (needed to build
+00003040: 2074 6861 7420 6c61 7965 7273 0a20 2020   that layers.   
+00003050: 2020 2020 2074 6865 6d73 656c 7665 7329       themselves)
+00003060: 2062 6173 6564 206f 6e20 7468 6520 696e   based on the in
+00003070: 7075 7420 6461 7461 2073 7570 706c 6965  put data supplie
+00003080: 6420 6279 2074 6865 2075 7365 7220 7768  d by the user wh
+00003090: 696c 6520 6361 6c6c 696e 6720 7468 6520  ile calling the 
+000030a0: 607e 5363 6f72 696e 6742 6173 6564 456d  `~ScoringBasedEm
+000030b0: 6265 6464 696e 674d 6f64 656c 2e66 6974  beddingModel.fit
+000030c0: 6020 6d65 7468 6f64 2e0a 2020 2020 2020  ` method..      
+000030d0: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
+000030e0: 7365 7420 7468 6520 6d61 7820 6e75 6d62  set the max numb
+000030f0: 6572 206f 6620 7468 6520 656e 7469 7469  er of the entiti
+00003100: 6573 2074 6861 7420 7769 6c6c 2062 6520  es that will be 
+00003110: 7472 6169 6e65 6420 7065 7220 7061 7274  trained per part
+00003120: 6974 696f 6e0a 2020 2020 2020 2020 2320  ition.        # 
+00003130: 696e 2063 6173 6520 6f66 206e 6f6e 2d70  in case of non-p
+00003140: 6172 7469 7469 6f6e 6564 2074 7261 696e  artitioned train
+00003150: 696e 672c 2069 7420 6973 2065 7175 616c  ing, it is equal
+00003160: 2074 6f20 7468 6520 746f 7461 6c20 6e75   to the total nu
+00003170: 6d62 6572 0a20 2020 2020 2020 2023 206f  mber.        # o
+00003180: 6620 656e 7469 7469 6573 206f 6620 7468  f entities of th
+00003190: 6520 6461 7461 7365 740a 2020 2020 2020  e dataset.      
+000031a0: 2020 7365 6c66 2e65 6e63 6f64 696e 675f    self.encoding_
+000031b0: 6c61 7965 722e 6d61 785f 656e 745f 7369  layer.max_ent_si
+000031c0: 7a65 203d 2073 656c 662e 6d61 785f 656e  ze = self.max_en
+000031d0: 745f 7369 7a65 0a20 2020 2020 2020 2023  t_size.        #
+000031e0: 2073 6574 2074 6865 206d 6178 206e 756d   set the max num
+000031f0: 6265 7220 6f66 2072 656c 6174 696f 6e73  ber of relations
+00003200: 2062 6569 6e67 2074 7261 696e 6564 206a   being trained j
+00003210: 7573 7420 6c69 6b65 2061 626f 7665 0a20  ust like above. 
+00003220: 2020 2020 2020 2073 656c 662e 656e 636f         self.enco
+00003230: 6469 6e67 5f6c 6179 6572 2e6d 6178 5f72  ding_layer.max_r
+00003240: 656c 5f73 697a 6520 3d20 7365 6c66 2e6d  el_size = self.m
+00003250: 6178 5f72 656c 5f73 697a 650a 2020 2020  ax_rel_size.    
+00003260: 2020 2020 7365 6c66 2e6e 756d 5f65 6e74      self.num_ent
+00003270: 7320 3d20 7365 6c66 2e6d 6178 5f65 6e74  s = self.max_ent
+00003280: 5f73 697a 650a 2020 2020 2020 2020 7365  _size.        se
+00003290: 6c66 2e62 7569 6c74 203d 2054 7275 650a  lf.built = True.
+000032a0: 0a20 2020 2064 6566 2063 6f6d 7075 7465  .    def compute
+000032b0: 5f66 6f63 7573 455f 7765 6967 6874 7328  _focusE_weights(
+000032c0: 7365 6c66 2c20 7765 6967 6874 732c 2073  self, weights, s
+000032d0: 7472 7563 7475 7265 5f77 6569 6768 7429  tructure_weight)
+000032e0: 3a0a 2020 2020 2020 2020 2222 2243 6f6d  :.        """Com
+000032f0: 7075 7465 2070 6f73 6974 6976 6520 616e  pute positive an
+00003300: 6420 6e65 6761 7469 7665 2077 6569 6768  d negative weigh
+00003310: 7473 2074 6f20 7363 616c 6520 7363 6f72  ts to scale scor
+00003320: 6573 2069 6620 6060 7573 655f 666f 6375  es if ``use_focu
+00003330: 7345 3d54 7275 6560 602e 0a0a 2020 2020  sE=True``...    
+00003340: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00003350: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00003360: 2d0a 2020 2020 2020 2020 7765 6967 6874  -.        weight
+00003370: 733a 2061 7272 6179 2d6c 696b 652c 2073  s: array-like, s
+00003380: 6861 7065 2028 6e2c 206d 290a 2020 2020  hape (n, m).    
+00003390: 2020 2020 2020 2020 4261 7463 6820 6f66          Batch of
+000033a0: 2077 6569 6768 7473 2061 7373 6f63 6961   weights associa
+000033b0: 7465 6420 7472 6970 6c65 732e 0a20 2020  ted triples..   
+000033c0: 2020 2020 2073 7472 7563 7574 7572 655f       strucuture_
+000033d0: 7765 6967 6874 3a20 666c 6f61 740a 2020  weight: float.  
+000033e0: 2020 2020 2020 2020 2020 5374 7275 6374            Struct
+000033f0: 7572 616c 2069 6e66 6c75 656e 6365 2061  ural influence a
+00003400: 7373 6967 6e65 6420 746f 2074 6865 2077  ssigned to the w
+00003410: 6569 6768 7473 2e0a 0a20 2020 2020 2020  eights...       
+00003420: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00003430: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00003440: 206f 7574 3a20 7475 706c 6520 6f66 2074   out: tuple of t
+00003450: 776f 2074 662e 5465 6e73 6f72 732c 2028  wo tf.Tensors, (
+00003460: 7466 2e54 656e 736f 7228 7368 6170 653d  tf.Tensor(shape=
+00003470: 286e 2c20 3129 292c 2074 662e 5465 6e73  (n, 1)), tf.Tens
+00003480: 6f72 2873 6861 7065 3d28 6e20 2a20 7365  or(shape=(n * se
+00003490: 6c66 2e65 7461 2c20 3129 2929 0a20 2020  lf.eta, 1))).   
+000034a0: 2020 2020 2020 2020 2054 7570 6c65 2077           Tuple w
+000034b0: 6865 7265 2074 6865 2066 6972 7374 2065  here the first e
+000034c0: 6c65 6d65 6e74 7320 6973 2061 2074 656e  lements is a ten
+000034d0: 736f 7220 636f 6e74 6169 6e69 6e67 2074  sor containing t
+000034e0: 6865 2070 6f73 6974 6976 6520 7765 6967  he positive weig
+000034f0: 6874 730a 2020 2020 2020 2020 2020 2020  hts.            
+00003500: 616e 6420 7468 6520 7365 636f 6e64 2069  and the second i
+00003510: 7320 6120 7465 6e73 6f72 2063 6f6e 7461  s a tensor conta
+00003520: 696e 696e 6720 7468 6520 6e65 6761 7469  ining the negati
+00003530: 7665 2077 6569 6768 7473 2e0a 2020 2020  ve weights..    
+00003540: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00003550: 2023 2057 6569 6768 7473 2063 6f6d 7075   # Weights compu
+00003560: 7461 7469 6f6e 0a20 2020 2020 2020 2077  tation.        w
+00003570: 6569 6768 7473 203d 2074 662e 7265 6475  eights = tf.redu
+00003580: 6365 5f6d 6561 6e28 7765 6967 6874 732c  ce_mean(weights,
+00003590: 2031 290a 2020 2020 2020 2020 7765 6967   1).        weig
+000035a0: 6874 735f 706f 7320 3d20 7374 7275 6374  hts_pos = struct
+000035b0: 7572 655f 7765 6967 6874 202b 2028 3120  ure_weight + (1 
+000035c0: 2d20 7374 7275 6374 7572 655f 7765 6967  - structure_weig
+000035d0: 6874 2920 2a20 2831 202d 2077 6569 6768  ht) * (1 - weigh
+000035e0: 7473 290a 2020 2020 2020 2020 7765 6967  ts).        weig
+000035f0: 6874 735f 6e65 6720 3d20 7374 7275 6374  hts_neg = struct
+00003600: 7572 655f 7765 6967 6874 202b 2028 3120  ure_weight + (1 
+00003610: 2d20 7374 7275 6374 7572 655f 7765 6967  - structure_weig
+00003620: 6874 2920 2a20 280a 2020 2020 2020 2020  ht) * (.        
+00003630: 2020 2020 7466 2e72 6573 6861 7065 280a      tf.reshape(.
+00003640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003650: 7466 2e74 696c 6528 7765 6967 6874 732c  tf.tile(weights,
+00003660: 205b 7365 6c66 2e65 7461 5d29 2c20 5b74   [self.eta]), [t
+00003670: 662e 7368 6170 6528 7765 6967 6874 7329  f.shape(weights)
+00003680: 5b30 5d20 2a20 7365 6c66 2e65 7461 5d0a  [0] * self.eta].
+00003690: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000036a0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+000036b0: 2072 6574 7572 6e20 7765 6967 6874 735f   return weights_
+000036c0: 706f 732c 2077 6569 6768 7473 5f6e 6567  pos, weights_neg
+000036d0: 0a0a 2020 2020 6465 6620 7472 6169 6e5f  ..    def train_
+000036e0: 7374 6570 2873 656c 662c 2064 6174 6129  step(self, data)
+000036f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00003700: 2020 2020 2020 5472 6169 6e69 6e67 2073        Training s
+00003710: 7465 702e 0a0a 2020 2020 2020 2020 5061  tep...        Pa
+00003720: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00003730: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00003740: 2020 2020 6461 7461 3a20 6172 7261 792d      data: array-
+00003750: 6c69 6b65 2c20 7368 6170 6520 286e 2c20  like, shape (n, 
+00003760: 6d29 0a20 2020 2020 2020 2020 2020 2042  m).            B
+00003770: 6174 6368 206f 6620 696e 7075 7420 7472  atch of input tr
+00003780: 6970 6c65 7320 2874 7275 6520 706f 7369  iples (true posi
+00003790: 7469 7665 7329 2077 6974 6820 7765 6967  tives) with weig
+000037a0: 6874 7320 6173 736f 6369 6174 6564 2069  hts associated i
+000037b0: 6620 6d3e 332e 0a0a 2020 2020 2020 2020  f m>3...        
+000037c0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+000037d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+000037e0: 6f75 743a 2064 6963 740a 2020 2020 2020  out: dict.      
+000037f0: 2020 2020 2020 4469 6374 696f 6e61 7279        Dictionary
+00003800: 206f 6620 6d65 7472 6963 7320 636f 6d70   of metrics comp
+00003810: 7574 6564 206f 6e20 7468 6520 6f75 7470  uted on the outp
+00003820: 7574 7320 2865 2e67 2e2c 206c 6f73 7329  uts (e.g., loss)
+00003830: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00003840: 2020 2020 2020 6966 2073 656c 662e 6461        if self.da
+00003850: 7461 5f73 6861 7065 203e 2033 3a0a 2020  ta_shape > 3:.  
+00003860: 2020 2020 2020 2020 2020 7472 6970 6c65            triple
+00003870: 7320 3d20 6461 7461 5b30 5d0a 2020 2020  s = data[0].    
+00003880: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00003890: 6461 7461 5f68 616e 646c 6572 2e5f 6164  data_handler._ad
+000038a0: 6170 7465 722e 7573 655f 6669 6c74 6572  apter.use_filter
+000038b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000038c0: 2020 7765 6967 6874 7320 3d20 6461 7461    weights = data
+000038d0: 5b32 5d0a 2020 2020 2020 2020 2020 2020  [2].            
+000038e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000038f0: 2020 2020 2020 7765 6967 6874 7320 3d20        weights = 
+00003900: 6461 7461 5b31 5d0a 2020 2020 2020 2020  data[1].        
+00003910: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00003920: 2020 7472 6970 6c65 7320 3d20 6461 7461    triples = data
+00003930: 0a20 2020 2020 2020 2077 6974 6820 7466  .        with tf
+00003940: 2e47 7261 6469 656e 7454 6170 6528 2920  .GradientTape() 
+00003950: 6173 2074 6170 653a 0a20 2020 2020 2020  as tape:.       
+00003960: 2020 2020 2023 2067 6574 2074 6865 206d       # get the m
+00003970: 6f64 656c 2070 7265 6469 6374 696f 6e73  odel predictions
+00003980: 0a20 2020 2020 2020 2020 2020 2073 636f  .            sco
+00003990: 7265 5f70 6f73 2c20 7363 6f72 655f 6e65  re_pos, score_ne
+000039a0: 6720 3d20 7365 6c66 2874 662e 6361 7374  g = self(tf.cast
+000039b0: 2874 7269 706c 6573 2c20 7466 2e69 6e74  (triples, tf.int
+000039c0: 3332 292c 2074 7261 696e 696e 673d 3129  32), training=1)
+000039d0: 0a20 2020 2020 2020 2020 2020 2023 2066  .            # f
+000039e0: 6f63 7573 4520 6c61 7965 720a 2020 2020  ocusE layer.    
+000039f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00003a00: 7573 655f 666f 6375 7345 3a0a 2020 2020  use_focusE:.    
+00003a10: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00003a20: 6572 2e64 6562 7567 2822 5573 696e 6720  er.debug("Using 
+00003a30: 466f 6375 7345 2229 0a20 2020 2020 2020  FocusE").       
+00003a40: 2020 2020 2020 2020 206e 6f6e 5f6c 696e           non_lin
+00003a50: 6561 7269 7479 203d 2073 656c 662e 666f  earity = self.fo
+00003a60: 6375 7345 5f70 6172 616d 735b 226e 6f6e  cusE_params["non
+00003a70: 5f6c 696e 6561 7269 7479 225d 0a20 2020  _linearity"].   
+00003a80: 2020 2020 2020 2020 2020 2020 2073 7472               str
+00003a90: 7563 7475 7265 5f77 6569 6768 7420 3d20  ucture_weight = 
+00003aa0: 7365 6c66 2e66 6f63 7573 455f 7061 7261  self.focusE_para
+00003ab0: 6d73 5b22 7374 7275 6374 7572 616c 5f77  ms["structural_w
+00003ac0: 7422 5d0a 0a20 2020 2020 2020 2020 2020  t"]..           
+00003ad0: 2020 2020 2077 6569 6768 7473 5f70 6f73       weights_pos
+00003ae0: 2c20 7765 6967 6874 735f 6e65 6720 3d20  , weights_neg = 
+00003af0: 7365 6c66 2e63 6f6d 7075 7465 5f66 6f63  self.compute_foc
+00003b00: 7573 455f 7765 6967 6874 7328 0a20 2020  usE_weights(.   
+00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b20: 2077 6569 6768 7473 3d77 6569 6768 7473   weights=weights
+00003b30: 2c20 7374 7275 6374 7572 655f 7765 6967  , structure_weig
+00003b40: 6874 3d73 7472 7563 7475 7265 5f77 6569  ht=structure_wei
+00003b50: 6768 740a 2020 2020 2020 2020 2020 2020  ght.            
+00003b60: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00003b70: 2020 2020 2020 2320 436f 6d70 7574 6174        # Computat
+00003b80: 696f 6e20 6f66 2073 636f 7265 730a 2020  ion of scores.  
+00003b90: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00003ba0: 6f72 655f 706f 7320 3d20 6e6f 6e5f 6c69  ore_pos = non_li
+00003bb0: 6e65 6172 6974 7928 7363 6f72 655f 706f  nearity(score_po
+00003bc0: 7329 202a 2077 6569 6768 7473 5f70 6f73  s) * weights_pos
+00003bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003be0: 2073 636f 7265 5f6e 6567 203d 206e 6f6e   score_neg = non
+00003bf0: 5f6c 696e 6561 7269 7479 2873 636f 7265  _linearity(score
+00003c00: 5f6e 6567 2920 2a20 7765 6967 6874 735f  _neg) * weights_
+00003c10: 6e65 670a 0a20 2020 2020 2020 2020 2020  neg..           
+00003c20: 2023 2063 6f6d 7075 7465 2074 6865 206c   # compute the l
+00003c30: 6f73 730a 2020 2020 2020 2020 2020 2020  oss.            
+00003c40: 6c6f 7373 203d 2073 656c 662e 636f 6d70  loss = self.comp
+00003c50: 696c 6564 5f6c 6f73 7328 0a20 2020 2020  iled_loss(.     
+00003c60: 2020 2020 2020 2020 2020 2073 636f 7265             score
+00003c70: 5f70 6f73 2c0a 2020 2020 2020 2020 2020  _pos,.          
+00003c80: 2020 2020 2020 7363 6f72 655f 6e65 672c        score_neg,
+00003c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003ca0: 2073 656c 662e 6574 612c 0a20 2020 2020   self.eta,.     
+00003cb0: 2020 2020 2020 2020 2020 2072 6567 756c             regul
+00003cc0: 6172 697a 6174 696f 6e5f 6c6f 7373 6573  arization_losses
+00003cd0: 3d73 656c 662e 6c6f 7373 6573 2c0a 2020  =self.losses,.  
+00003ce0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00003cf0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00003d00: 2020 2020 2023 206d 696e 696d 697a 6520       # minimize 
+00003d10: 7468 6520 6c6f 7373 2061 6e64 2075 7064  the loss and upd
+00003d20: 6174 6520 7468 6520 7472 6169 6e61 626c  ate the trainabl
+00003d30: 6520 7661 7269 6162 6c65 730a 2020 2020  e variables.    
+00003d40: 2020 2020 2020 2020 7365 6c66 2e6f 7074          self.opt
+00003d50: 696d 697a 6572 2e6d 696e 696d 697a 6528  imizer.minimize(
+00003d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003d70: 206c 6f73 732c 0a20 2020 2020 2020 2020   loss,.         
+00003d80: 2020 2020 2020 2073 656c 662e 656e 636f         self.enco
+00003d90: 6469 6e67 5f6c 6179 6572 2e65 6e74 5f65  ding_layer.ent_e
+00003da0: 6d62 2c0a 2020 2020 2020 2020 2020 2020  mb,.            
+00003db0: 2020 2020 7365 6c66 2e65 6e63 6f64 696e      self.encodin
+00003dc0: 675f 6c61 7965 722e 7265 6c5f 656d 622c  g_layer.rel_emb,
+00003dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003de0: 2074 6170 652c 0a20 2020 2020 2020 2020   tape,.         
+00003df0: 2020 2029 0a20 2020 2020 2020 2065 7863     ).        exc
+00003e00: 6570 7420 5661 6c75 6545 7272 6f72 2061  ept ValueError a
+00003e10: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
+00003e20: 2069 6620 7365 6c66 2e73 636f 7269 6e67   if self.scoring
+00003e30: 5f6c 6179 6572 2e6e 616d 6520 3d3d 2022  _layer.name == "
+00003e40: 5261 6e64 6f6d 223a 0a20 2020 2020 2020  Random":.       
+00003e50: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
+00003e60: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00003e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e80: 7261 6973 6520 650a 0a20 2020 2020 2020  raise e..       
+00003e90: 2072 6574 7572 6e20 7b6d 2e6e 616d 653a   return {m.name:
+00003ea0: 206d 2e72 6573 756c 7428 2920 666f 7220   m.result() for 
+00003eb0: 6d20 696e 2073 656c 662e 6d65 7472 6963  m in self.metric
+00003ec0: 737d 0a0a 2020 2020 6465 6620 6d61 6b65  s}..    def make
+00003ed0: 5f74 7261 696e 5f66 756e 6374 696f 6e28  _train_function(
+00003ee0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00003ef0: 2222 5369 6d69 6c61 7220 746f 206b 6572  ""Similar to ker
+00003f00: 6173 206c 6962 2c20 7468 6973 2066 756e  as lib, this fun
+00003f10: 6374 696f 6e20 7265 7475 726e 7320 7468  ction returns th
+00003f20: 6520 6861 6e64 6c65 2074 6f20 7468 6520  e handle to the 
+00003f30: 7472 6169 6e69 6e67 2073 7465 7020 6675  training step fu
+00003f40: 6e63 7469 6f6e 2e0a 2020 2020 2020 2020  nction..        
+00003f50: 4974 2070 726f 6365 7373 6573 206f 6e65  It processes one
+00003f60: 2062 6174 6368 206f 6620 6461 7461 2062   batch of data b
+00003f70: 7920 6974 6572 6174 696e 6720 6f76 6572  y iterating over
+00003f80: 2074 6865 2064 6174 6173 6574 2069 7465   the dataset ite
+00003f90: 7261 746f 722c 2069 7420 636f 6d70 7574  rator, it comput
+00003fa0: 6573 2074 6865 206c 6f73 7320 616e 6420  es the loss and 
+00003fb0: 6f70 7469 6d69 7a65 7320 6f6e 2069 742e  optimizes on it.
+00003fc0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00003fd0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00003fe0: 2d0a 2020 2020 2020 2020 6f75 743a 2046  -.        out: F
+00003ff0: 756e 6374 696f 6e20 6861 6e64 6c65 0a20  unction handle. 
+00004000: 2020 2020 2020 2020 2020 2020 2048 616e               Han
+00004010: 646c 6520 746f 2074 6865 2074 7261 696e  dle to the train
+00004020: 696e 6720 7374 6570 2066 756e 6374 696f  ing step functio
+00004030: 6e2e 0a20 2020 2020 2020 2022 2222 0a20  n..        """. 
+00004040: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+00004050: 7261 696e 5f66 756e 6374 696f 6e20 6973  rain_function is
+00004060: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00004070: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00004080: 6c66 2e74 7261 696e 5f66 756e 6374 696f  lf.train_functio
+00004090: 6e0a 0a20 2020 2020 2020 2064 6566 2074  n..        def t
+000040a0: 7261 696e 5f66 756e 6374 696f 6e28 6974  rain_function(it
+000040b0: 6572 6174 6f72 293a 0a20 2020 2020 2020  erator):.       
+000040c0: 2020 2020 2022 2222 5468 6973 2069 7320       """This is 
+000040d0: 7468 6520 6675 6e63 7469 6f6e 2077 686f  the function who
+000040e0: 7365 2068 616e 646c 6520 7769 6c6c 2062  se handle will b
+000040f0: 6520 7265 7475 726e 6564 2e0a 0a20 2020  e returned...   
+00004100: 2020 2020 2020 2020 2050 6172 616d 6574           Paramet
+00004110: 6572 730a 2020 2020 2020 2020 2020 2020  ers.            
+00004120: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00004130: 2020 2020 2020 2069 7465 7261 746f 723a         iterator:
+00004140: 2074 662e 6461 7461 2e49 7465 7261 746f   tf.data.Iterato
+00004150: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+00004160: 2020 4461 7461 2069 7465 7261 746f 722e    Data iterator.
+00004170: 0a0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
+00004180: 7475 726e 730a 2020 2020 2020 2020 2020  turns.          
+00004190: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+000041a0: 2020 2020 2020 6f75 7470 7574 3a20 6469        output: di
+000041b0: 6374 0a20 2020 2020 2020 2020 2020 2020  ct.             
+000041c0: 2052 6574 7572 6e20 6120 6469 6374 696f   Return a dictio
+000041d0: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
+000041e0: 7661 6c75 6573 2074 6861 7420 7769 6c6c  values that will
+000041f0: 2062 6520 7061 7373 6564 2074 6f20 6060   be passed to ``
+00004200: 7466 2e6b 6572 6173 2e43 616c 6c62 6163  tf.keras.Callbac
+00004210: 6b73 2e6f 6e5f 7472 6169 6e5f 6261 7463  ks.on_train_batc
+00004220: 685f 656e 6460 602e 0a20 2020 2020 2020  h_end``..       
+00004230: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00004240: 2020 2020 2064 6174 6120 3d20 6e65 7874       data = next
+00004250: 2869 7465 7261 746f 7229 0a20 2020 2020  (iterator).     
+00004260: 2020 2020 2020 206f 7574 7075 7420 3d20         output = 
+00004270: 7365 6c66 2e74 7261 696e 5f73 7465 7028  self.train_step(
+00004280: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
+00004290: 2020 7265 7475 726e 206f 7574 7075 740a    return output.
+000042a0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000042b0: 7365 6c66 2e72 756e 5f65 6167 6572 6c79  self.run_eagerly
+000042c0: 2061 6e64 206e 6f74 2073 656c 662e 6973   and not self.is
+000042d0: 5f70 6172 7469 7469 6f6e 6564 5f74 7261  _partitioned_tra
+000042e0: 696e 696e 673a 0a20 2020 2020 2020 2020  ining:.         
+000042f0: 2020 2074 7261 696e 5f66 756e 6374 696f     train_functio
+00004300: 6e20 3d20 6465 665f 6675 6e63 7469 6f6e  n = def_function
+00004310: 2e66 756e 6374 696f 6e28 0a20 2020 2020  .function(.     
+00004320: 2020 2020 2020 2020 2020 2074 7261 696e             train
+00004330: 5f66 756e 6374 696f 6e2c 2065 7870 6572  _function, exper
+00004340: 696d 656e 7461 6c5f 7265 6c61 785f 7368  imental_relax_sh
+00004350: 6170 6573 3d54 7275 650a 2020 2020 2020  apes=True.      
+00004360: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00004370: 2073 656c 662e 7472 6169 6e5f 6675 6e63   self.train_func
+00004380: 7469 6f6e 203d 2074 7261 696e 5f66 756e  tion = train_fun
+00004390: 6374 696f 6e0a 2020 2020 2020 2020 7265  ction.        re
+000043a0: 7475 726e 2073 656c 662e 7472 6169 6e5f  turn self.train_
+000043b0: 6675 6e63 7469 6f6e 0a0a 2020 2020 6465  function..    de
+000043c0: 6620 6765 745f 666f 6375 7345 5f70 6172  f get_focusE_par
+000043d0: 616d 7328 7365 6c66 2c20 6469 6374 5f70  ams(self, dict_p
+000043e0: 6172 616d 733d 7b7d 293a 0a20 2020 2020  arams={}):.     
+000043f0: 2020 2022 2222 4765 7420 7061 7261 6d65     """Get parame
+00004400: 7465 7273 2066 6f72 2066 6f63 7573 452e  ters for focusE.
+00004410: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00004420: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00004430: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00004440: 6469 6374 5f70 6172 616d 733a 2064 6963  dict_params: dic
+00004450: 740a 2020 2020 2020 2020 2020 2020 5468  t.            Th
+00004460: 6520 666f 6c6c 6f77 696e 6720 6879 7065  e following hype
+00004470: 722d 7061 7261 6d73 2063 616e 2062 6520  r-params can be 
+00004480: 7061 7373 6564 3a0a 0a20 2020 2020 2020  passed:..       
+00004490: 2020 2020 202d 2022 6e6f 6e5f 6c69 6e65       - "non_line
+000044a0: 6172 6974 7922 3a20 6361 6e20 6173 7375  arity": can assu
+000044b0: 6d65 206f 6620 7468 6520 666f 6c6c 6f77  me of the follow
+000044c0: 696e 6720 7661 6c75 6573 2060 226c 696e  ing values `"lin
+000044d0: 6561 7222 602c 2060 2273 6f66 7470 6c75  ear"`, `"softplu
+000044e0: 7322 602c 2060 2273 6967 6d6f 6964 2260  s"`, `"sigmoid"`
+000044f0: 2c20 6022 7461 6e68 2260 2e0a 2020 2020  , `"tanh"`..    
+00004500: 2020 2020 2020 2020 2d20 2273 746f 705f          - "stop_
+00004510: 6570 6f63 6822 3a20 7370 6563 6966 6965  epoch": specifie
+00004520: 7320 686f 7720 6c6f 6e67 2074 6f20 6465  s how long to de
+00004530: 6361 7920 286c 696e 6561 726c 7929 2074  cay (linearly) t
+00004540: 6865 2073 7472 7563 7475 7261 6c20 696e  he structural in
+00004550: 666c 7565 6e63 6520 6879 7065 722d 7061  fluence hyper-pa
+00004560: 7261 6d65 7465 7220 5c0a 2020 2020 2020  rameter \.      
+00004570: 2020 2020 2020 6672 6f6d 2031 2075 6e74        from 1 unt
+00004580: 696c 2069 7420 7265 6163 6865 7320 6974  il it reaches it
+00004590: 7320 6f72 6967 696e 616c 2076 616c 7565  s original value
+000045a0: 2e0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
+000045b0: 2273 7472 7563 7475 7261 6c5f 7774 223a  "structural_wt":
+000045c0: 2073 7472 7563 7475 7261 6c20 696e 666c   structural infl
+000045d0: 7565 6e63 6520 6879 7065 7270 6172 616d  uence hyperparam
+000045e0: 6574 6572 205b 302c 2031 5d20 7468 6174  eter [0, 1] that
+000045f0: 206d 6f64 756c 6174 6573 2074 6865 2069   modulates the i
+00004600: 6e66 6c75 656e 6365 206f 6620 6772 6170  nfluence of grap
+00004610: 6820 5c0a 2020 2020 2020 2020 2020 2020  h \.            
+00004620: 746f 706f 6c6f 6779 2e0a 0a20 2020 2020  topology...     
+00004630: 2020 2020 2020 2049 6620 7468 6520 7265         If the re
+00004640: 7370 6563 7469 7665 206b 6579 2069 7320  spective key is 
+00004650: 6d69 7373 696e 673a 2060 606e 6f6e 5f6c  missing: ``non_l
+00004660: 696e 6561 7269 7479 3d22 6c69 6e65 6172  inearity="linear
+00004670: 2260 602c 2060 6073 746f 705f 6570 6f63  "``, ``stop_epoc
+00004680: 683d 3235 3160 6020 616e 6420 6060 7374  h=251`` and ``st
+00004690: 7275 6374 7572 616c 5f77 743d 302e 3030  ructural_wt=0.00
+000046a0: 3160 602e 0a0a 2020 2020 2020 2020 5265  1``...        Re
+000046b0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+000046c0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 666f  -----.        fo
+000046d0: 6375 7345 5f70 6172 616d 7320 3a20 7475  cusE_params : tu
+000046e0: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
+000046f0: 4120 7475 706c 6520 636f 6e74 6169 6e69  A tuple containi
+00004700: 6e67 2074 6872 6565 2076 616c 7565 733a  ng three values:
+00004710: 2074 6865 206e 6f6e 2d6c 696e 6561 7269   the non-lineari
+00004720: 7479 2066 756e 6374 696f 6e20 2860 7374  ty function (`st
+00004730: 7260 292c 2074 6865 2060 7374 6f70 5f65  r`), the `stop_e
+00004740: 706f 6368 6020 2860 696e 7460 2920 616e  poch` (`int`) an
+00004750: 6420 7468 650a 2020 2020 2020 2020 2020  d the.          
+00004760: 2020 7374 7275 6374 7572 6520 7765 6967    structure weig
+00004770: 6874 2028 6066 6c6f 6174 6029 2e0a 0a20  ht (`float`)... 
+00004780: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00004790: 2020 2023 2047 6574 2074 6865 206e 6f6e     # Get the non
+000047a0: 2d6c 696e 6561 7269 7479 2066 756e 6374  -linearity funct
+000047b0: 696f 6e0a 2020 2020 2020 2020 6e6f 6e5f  ion.        non_
+000047c0: 6c69 6e65 6172 6974 7920 3d20 6469 6374  linearity = dict
+000047d0: 5f70 6172 616d 732e 6765 7428 226e 6f6e  _params.get("non
+000047e0: 5f6c 696e 6561 7269 7479 222c 2022 6c69  _linearity", "li
+000047f0: 6e65 6172 2229 0a20 2020 2020 2020 2069  near").        i
+00004800: 6620 6e6f 6e5f 6c69 6e65 6172 6974 7920  f non_linearity 
+00004810: 3d3d 2022 6c69 6e65 6172 223a 0a20 2020  == "linear":.   
+00004820: 2020 2020 2020 2020 206e 6f6e 5f6c 696e           non_lin
+00004830: 6561 7269 7479 203d 2074 662e 6964 656e  earity = tf.iden
+00004840: 7469 7479 0a20 2020 2020 2020 2065 6c69  tity.        eli
+00004850: 6620 6e6f 6e5f 6c69 6e65 6172 6974 7920  f non_linearity 
+00004860: 3d3d 2022 7461 6e68 223a 0a20 2020 2020  == "tanh":.     
+00004870: 2020 2020 2020 206e 6f6e 5f6c 696e 6561         non_linea
+00004880: 7269 7479 203d 2074 662e 7461 6e68 0a20  rity = tf.tanh. 
+00004890: 2020 2020 2020 2065 6c69 6620 6e6f 6e5f         elif non_
+000048a0: 6c69 6e65 6172 6974 7920 3d3d 2022 7369  linearity == "si
+000048b0: 676d 6f69 6422 3a0a 2020 2020 2020 2020  gmoid":.        
+000048c0: 2020 2020 6e6f 6e5f 6c69 6e65 6172 6974      non_linearit
+000048d0: 7920 3d20 7466 2e73 6967 6d6f 6964 0a20  y = tf.sigmoid. 
+000048e0: 2020 2020 2020 2065 6c69 6620 6e6f 6e5f         elif non_
+000048f0: 6c69 6e65 6172 6974 7920 3d3d 2022 736f  linearity == "so
+00004900: 6674 706c 7573 223a 0a0a 2020 2020 2020  ftplus":..      
+00004910: 2020 2020 2020 4074 662e 6375 7374 6f6d        @tf.custom
+00004920: 5f67 7261 6469 656e 740a 2020 2020 2020  _gradient.      
+00004930: 2020 2020 2020 6465 6620 6375 7374 6f6d        def custom
+00004940: 5f73 6f66 7470 6c75 7328 7829 3a0a 2020  _softplus(x):.  
+00004950: 2020 2020 2020 2020 2020 2020 2020 6520                e 
+00004960: 3d20 3939 3939 202a 2074 662e 6578 7028  = 9999 * tf.exp(
+00004970: 7829 0a0a 2020 2020 2020 2020 2020 2020  x)..            
+00004980: 2020 2020 6465 6620 6772 6164 2864 7929      def grad(dy)
+00004990: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000049a0: 2020 2020 2020 7265 7475 726e 2064 7920        return dy 
+000049b0: 2a20 2831 202d 2031 202f 2028 3120 2b20  * (1 - 1 / (1 + 
+000049c0: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
+000049d0: 2020 2020 7265 7475 726e 2074 662e 6d61      return tf.ma
+000049e0: 7468 2e6c 6f67 2831 202b 2065 292c 2067  th.log(1 + e), g
+000049f0: 7261 640a 0a20 2020 2020 2020 2020 2020  rad..           
+00004a00: 206e 6f6e 5f6c 696e 6561 7269 7479 203d   non_linearity =
+00004a10: 2063 7573 746f 6d5f 736f 6674 706c 7573   custom_softplus
+00004a20: 0a0a 2020 2020 2020 2020 656c 7365 3a0a  ..        else:.
+00004a30: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00004a40: 6520 5661 6c75 6545 7272 6f72 2822 496e  e ValueError("In
+00004a50: 7661 6c69 6420 666f 6375 7345 206e 6f6e  valid focusE non
+00004a60: 2d6c 696e 6561 7269 7479 2229 0a0a 2020  -linearity")..  
+00004a70: 2020 2020 2020 2320 4765 7420 7468 6520        # Get the 
+00004a80: 7374 6f70 5f65 706f 6368 2066 6f72 2074  stop_epoch for t
+00004a90: 6865 2064 6563 6179 0a20 2020 2020 2020  he decay.       
+00004aa0: 2073 746f 705f 6570 6f63 6820 3d20 6469   stop_epoch = di
+00004ab0: 6374 5f70 6172 616d 732e 6765 7428 2273  ct_params.get("s
+00004ac0: 746f 705f 6570 6f63 6822 2c20 3235 3129  top_epoch", 251)
+00004ad0: 0a20 2020 2020 2020 206d 7367 203d 2022  .        msg = "
+00004ae0: 496e 7661 6c69 6420 7661 6c75 6520 666f  Invalid value fo
+00004af0: 7220 666f 6375 7345 2073 746f 705f 6570  r focusE stop_ep
+00004b00: 6f63 683a 2065 7870 6563 7465 6420 6120  och: expected a 
+00004b10: 7661 6c75 6520 3e3d 3020 6275 7420 676f  value >=0 but go
+00004b20: 7420 7b7d 222e 666f 726d 6174 280a 2020  t {}".format(.  
+00004b30: 2020 2020 2020 2020 2020 7374 6f70 5f65            stop_e
+00004b40: 706f 6368 0a20 2020 2020 2020 2029 0a20  poch.        ). 
+00004b50: 2020 2020 2020 2061 7373 6572 7420 7374         assert st
+00004b60: 6f70 5f65 706f 6368 203e 3d20 302c 206d  op_epoch >= 0, m
+00004b70: 7367 0a0a 2020 2020 2020 2020 2320 4765  sg..        # Ge
+00004b80: 7420 7374 7275 6374 7572 616c 5f77 740a  t structural_wt.
+00004b90: 2020 2020 2020 2020 7374 7275 6374 7572          structur
+00004ba0: 655f 7765 6967 6874 203d 2064 6963 745f  e_weight = dict_
+00004bb0: 7061 7261 6d73 2e67 6574 2822 7374 7275  params.get("stru
+00004bc0: 6374 7572 616c 5f77 7422 2c20 302e 3030  ctural_wt", 0.00
+00004bd0: 3129 0a20 2020 2020 2020 2061 7373 6572  1).        asser
+00004be0: 7420 2873 7472 7563 7475 7265 5f77 6569  t (structure_wei
+00004bf0: 6768 7420 3c3d 2031 2920 616e 6420 280a  ght <= 1) and (.
+00004c00: 2020 2020 2020 2020 2020 2020 7374 7275              stru
+00004c10: 6374 7572 655f 7765 6967 6874 203e 3d20  cture_weight >= 
+00004c20: 300a 2020 2020 2020 2020 292c 2022 496e  0.        ), "In
+00004c30: 7661 6c69 6420 666f 6375 7345 2027 7374  valid focusE 'st
+00004c40: 7275 6374 7572 616c 5f77 7427 2070 6173  ructural_wt' pas
+00004c50: 7365 6421 2049 7420 6861 7320 746f 2062  sed! It has to b
+00004c60: 656c 6f6e 6720 746f 205b 302c 315d 2e22  elong to [0,1]."
+00004c70: 0a0a 2020 2020 2020 2020 2320 6966 2073  ..        # if s
+00004c80: 746f 705f 6570 6f63 6820 3d3d 2030 2c20  top_epoch == 0, 
+00004c90: 6669 7865 6420 7374 7275 6374 7572 6520  fixed structure 
+00004ca0: 7765 6967 6874 7320 6973 2075 7365 640a  weights is used.
+00004cb0: 2020 2020 2020 2020 6966 2073 746f 705f          if stop_
+00004cc0: 6570 6f63 6820 3e20 303a 0a20 2020 2020  epoch > 0:.     
+00004cd0: 2020 2020 2020 2023 206c 696e 6561 7220         # linear 
+00004ce0: 6465 6361 7920 6f66 206e 756d 6572 6963  decay of numeric
+00004cf0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
+00004d00: 2020 2020 7374 7275 6374 7572 655f 7765      structure_we
+00004d10: 6967 6874 203d 2074 662e 6d61 7869 6d75  ight = tf.maximu
+00004d20: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
+00004d30: 2020 2031 202d 2073 656c 662e 6375 7272     1 - self.curr
+00004d40: 656e 745f 6570 6f63 6820 2f20 7374 6f70  ent_epoch / stop
+00004d50: 5f65 706f 6368 2c20 302e 3030 310a 2020  _epoch, 0.001.  
+00004d60: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00004d70: 2020 2020 2072 6574 7572 6e20 6e6f 6e5f       return non_
+00004d80: 6c69 6e65 6172 6974 792c 2073 746f 705f  linearity, stop_
+00004d90: 6570 6f63 682c 2073 7472 7563 7475 7265  epoch, structure
+00004da0: 5f77 6569 6768 740a 0a20 2020 2064 6566  _weight..    def
+00004db0: 2075 7064 6174 655f 666f 6375 7345 5f70   update_focusE_p
+00004dc0: 6172 616d 7328 7365 6c66 293a 0a20 2020  arams(self):.   
+00004dd0: 2020 2020 2022 2222 5570 6461 7465 2074       """Update t
+00004de0: 6865 2073 7472 7563 7475 7261 6c20 7765  he structural we
+00004df0: 6967 6874 2061 6674 6572 2064 6563 6179  ight after decay
+00004e00: 2e22 2222 0a20 2020 2020 2020 2069 6620  .""".        if 
+00004e10: 7365 6c66 2e66 6f63 7573 455f 7061 7261  self.focusE_para
+00004e20: 6d73 5b22 7374 6f70 5f65 706f 6368 225d  ms["stop_epoch"]
+00004e30: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+00004e40: 2020 7374 6f70 5f65 706f 6368 203d 2073    stop_epoch = s
+00004e50: 656c 662e 666f 6375 7345 5f70 6172 616d  elf.focusE_param
+00004e60: 735b 2273 746f 705f 6570 6f63 6822 5d0a  s["stop_epoch"].
+00004e70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00004e80: 2e66 6f63 7573 455f 7061 7261 6d73 5b22  .focusE_params["
+00004e90: 7374 7275 6374 7572 616c 5f77 7422 5d20  structural_wt"] 
+00004ea0: 3d20 7466 2e6d 6178 696d 756d 280a 2020  = tf.maximum(.  
+00004eb0: 2020 2020 2020 2020 2020 2020 2020 3120                1 
+00004ec0: 2d20 7365 6c66 2e63 7572 7265 6e74 5f65  - self.current_e
+00004ed0: 706f 6368 202f 2073 746f 705f 6570 6f63  poch / stop_epoc
+00004ee0: 682c 2030 2e30 3031 0a20 2020 2020 2020  h, 0.001.       
+00004ef0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00004f00: 6669 7428 0a20 2020 2020 2020 2073 656c  fit(.        sel
+00004f10: 662c 0a20 2020 2020 2020 2078 3d4e 6f6e  f,.        x=Non
+00004f20: 652c 0a20 2020 2020 2020 2062 6174 6368  e,.        batch
+00004f30: 5f73 697a 653d 312c 0a20 2020 2020 2020  _size=1,.       
+00004f40: 2065 706f 6368 733d 312c 0a20 2020 2020   epochs=1,.     
+00004f50: 2020 2076 6572 626f 7365 3d54 7275 652c     verbose=True,
+00004f60: 0a20 2020 2020 2020 2063 616c 6c62 6163  .        callbac
+00004f70: 6b73 3d4e 6f6e 652c 0a20 2020 2020 2020  ks=None,.       
+00004f80: 2076 616c 6964 6174 696f 6e5f 7370 6c69   validation_spli
+00004f90: 743d 302e 302c 0a20 2020 2020 2020 2076  t=0.0,.        v
+00004fa0: 616c 6964 6174 696f 6e5f 6461 7461 3d4e  alidation_data=N
+00004fb0: 6f6e 652c 0a20 2020 2020 2020 2073 6875  one,.        shu
+00004fc0: 6666 6c65 3d54 7275 652c 0a20 2020 2020  ffle=True,.     
+00004fd0: 2020 2069 6e69 7469 616c 5f65 706f 6368     initial_epoch
+00004fe0: 3d30 2c0a 2020 2020 2020 2020 7661 6c69  =0,.        vali
+00004ff0: 6461 7469 6f6e 5f62 6174 6368 5f73 697a  dation_batch_siz
+00005000: 653d 3130 302c 0a20 2020 2020 2020 2076  e=100,.        v
+00005010: 616c 6964 6174 696f 6e5f 636f 7272 7570  alidation_corrup
+00005020: 745f 7369 6465 3d22 732c 6f22 2c0a 2020  t_side="s,o",.  
+00005030: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
+00005040: 5f66 7265 713d 3530 2c0a 2020 2020 2020  _freq=50,.      
+00005050: 2020 7661 6c69 6461 7469 6f6e 5f62 7572    validation_bur
+00005060: 6e5f 696e 3d31 3030 2c0a 2020 2020 2020  n_in=100,.      
+00005070: 2020 7661 6c69 6461 7469 6f6e 5f66 696c    validation_fil
+00005080: 7465 723d 4661 6c73 652c 0a20 2020 2020  ter=False,.     
+00005090: 2020 2076 616c 6964 6174 696f 6e5f 656e     validation_en
+000050a0: 7469 7469 6573 5f73 7562 7365 743d 4e6f  tities_subset=No
+000050b0: 6e65 2c0a 2020 2020 2020 2020 7061 7274  ne,.        part
+000050c0: 6974 696f 6e69 6e67 5f6b 3d31 2c0a 2020  itioning_k=1,.  
+000050d0: 2020 2020 2020 666f 6375 7345 3d46 616c        focusE=Fal
+000050e0: 7365 2c0a 2020 2020 2020 2020 666f 6375  se,.        focu
+000050f0: 7345 5f70 6172 616d 733d 7b7d 2c0a 2020  sE_params={},.  
+00005100: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
+00005110: 4669 7420 7468 6520 6d6f 6465 6c20 6f6e  Fit the model on
+00005120: 2074 6865 2070 726f 7669 6465 6420 6461   the provided da
+00005130: 7461 2e0a 0a20 2020 2020 2020 2050 6172  ta...        Par
+00005140: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00005150: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00005160: 2020 2078 3a20 6e70 2e61 7272 6179 2c20     x: np.array, 
+00005170: 7368 6170 6520 286e 2c20 3329 2c20 6f72  shape (n, 3), or
+00005180: 2073 7472 206f 7220 4772 6170 6844 6174   str or GraphDat
+00005190: 614c 6f61 6465 7220 6f72 2041 6273 7472  aLoader or Abstr
+000051a0: 6163 7447 7261 7068 5061 7274 6974 696f  actGraphPartitio
+000051b0: 6e65 720a 2020 2020 2020 2020 2020 2020  ner.            
+000051c0: 4461 7461 204f 5220 4669 6c65 6e61 6d65  Data OR Filename
+000051d0: 206f 6620 7468 6520 6461 7461 2066 696c   of the data fil
+000051e0: 6520 4f52 2044 6174 6120 4861 6e64 6c65  e OR Data Handle
+000051f0: 2074 6f20 6265 2075 7365 6420 666f 7220   to be used for 
+00005200: 7472 6169 6e69 6e67 2e0a 2020 2020 2020  training..      
+00005210: 2020 6261 7463 685f 7369 7a65 3a20 696e    batch_size: in
+00005220: 740a 2020 2020 2020 2020 2020 2020 4261  t.            Ba
+00005230: 7463 6820 7369 7a65 2074 6f20 7573 6520  tch size to use 
+00005240: 6475 7269 6e67 2074 7261 696e 696e 672e  during training.
+00005250: 0a20 2020 2020 2020 2020 2020 204d 6179  .            May
+00005260: 2062 6520 6f76 6572 7269 6464 656e 2069   be overridden i
+00005270: 6620 2a2a 782a 2a20 6973 2061 2047 7261  f **x** is a Gra
+00005280: 7068 4461 7461 4c6f 6164 6572 206f 7220  phDataLoader or 
+00005290: 4162 7374 7261 6374 4772 6170 6850 6172  AbstractGraphPar
+000052a0: 7469 7469 6f6e 6572 2069 6e73 7461 6e63  titioner instanc
+000052b0: 652e 0a20 2020 2020 2020 2065 706f 6368  e..        epoch
+000052c0: 733a 2069 6e74 0a20 2020 2020 2020 2020  s: int.         
+000052d0: 2020 204e 756d 6265 7220 6f66 2065 706f     Number of epo
+000052e0: 6368 7320 746f 2074 7261 696e 2028 6465  chs to train (de
+000052f0: 6661 756c 743a 2031 292e 0a20 2020 2020  fault: 1)..     
+00005300: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
+00005310: 0a20 2020 2020 2020 2020 2020 2056 6572  .            Ver
+00005320: 626f 7369 7479 2028 6465 6661 756c 743a  bosity (default:
+00005330: 2060 5472 7565 6029 2e0a 2020 2020 2020   `True`)..      
+00005340: 2020 6361 6c6c 6261 636b 733a 206c 6973    callbacks: lis
+00005350: 7420 6f66 2074 662e 6b65 7261 732e 6361  t of tf.keras.ca
+00005360: 6c6c 6261 636b 732e 4361 6c6c 6261 636b  llbacks.Callback
+00005370: 0a20 2020 2020 2020 2020 2020 204c 6973  .            Lis
+00005380: 7420 6f66 2063 616c 6c62 6163 6b73 2074  t of callbacks t
+00005390: 6f20 6265 2075 7365 6420 6475 7269 6e67  o be used during
+000053a0: 2074 7261 696e 696e 6720 2864 6566 6175   training (defau
+000053b0: 6c74 3a20 604e 6f6e 6560 292e 0a20 2020  lt: `None`)..   
+000053c0: 2020 2020 2076 616c 6964 6174 696f 6e5f       validation_
+000053d0: 7370 6c69 743a 2066 6c6f 6174 0a20 2020  split: float.   
+000053e0: 2020 2020 2020 2020 2056 616c 6964 6174           Validat
+000053f0: 696f 6e20 7370 6c69 7420 746f 2063 6172  ion split to car
+00005400: 7665 206f 7574 206f 6620 2a2a 782a 2a20  ve out of **x** 
+00005410: 2864 6566 6175 6c74 3a20 302e 3029 2028  (default: 0.0) (
+00005420: 6375 7272 656e 746c 7920 7375 7070 6f72  currently suppor
+00005430: 7465 6420 6f6e 6c79 2077 6865 6e20 2a2a  ted only when **
+00005440: 782a 2a20 6973 2061 206e 702e 6172 7261  x** is a np.arra
+00005450: 7929 2e0a 2020 2020 2020 2020 7661 6c69  y)..        vali
+00005460: 6461 7469 6f6e 5f64 6174 613a 206e 702e  dation_data: np.
+00005470: 6172 7261 792c 2073 6861 7065 2028 6e2c  array, shape (n,
+00005480: 2033 2920 6f72 2073 7472 206f 7220 6047   3) or str or `G
+00005490: 7261 7068 4461 7461 4c6f 6164 6572 6020  raphDataLoader` 
+000054a0: 6f72 2060 4162 7374 7261 6374 4772 6170  or `AbstractGrap
+000054b0: 6850 6172 7469 7469 6f6e 6572 600a 2020  hPartitioner`.  
+000054c0: 2020 2020 2020 2020 2020 4461 7461 204f            Data O
+000054d0: 5220 4669 6c65 6e61 6d65 206f 6620 7468  R Filename of th
+000054e0: 6520 6461 7461 2066 696c 6520 4f52 2044  e data file OR D
+000054f0: 6174 6120 4861 6e64 6c65 2074 6f20 6265  ata Handle to be
+00005500: 2075 7365 6420 666f 7220 7661 6c69 6461   used for valida
+00005510: 7469 6f6e 2e0a 2020 2020 2020 2020 7368  tion..        sh
+00005520: 7566 666c 653a 2062 6f6f 6c0a 2020 2020  uffle: bool.    
+00005530: 2020 2020 2020 2020 496e 6469 6361 7465          Indicate
+00005540: 7320 7768 6574 6865 7220 746f 2073 6875  s whether to shu
+00005550: 6666 6c65 2074 6865 2064 6174 6120 6166  ffle the data af
+00005560: 7465 7220 6576 6572 7920 6570 6f63 6820  ter every epoch 
+00005570: 6475 7269 6e67 2074 7261 696e 696e 6720  during training 
+00005580: 2864 6566 6175 6c74 3a20 6054 7275 6560  (default: `True`
+00005590: 292e 0a20 2020 2020 2020 2069 6e69 7469  )..        initi
+000055a0: 616c 2065 706f 6368 3a20 696e 740a 2020  al epoch: int.  
+000055b0: 2020 2020 2020 2020 2020 496e 6974 6961            Initia
+000055c0: 6c20 6570 6f63 6820 6e75 6d62 6572 2028  l epoch number (
+000055d0: 6465 6661 756c 743a 2031 292e 0a20 2020  default: 1)..   
+000055e0: 2020 2020 2076 616c 6964 6174 696f 6e5f       validation_
+000055f0: 6261 7463 685f 7369 7a65 3a20 696e 740a  batch_size: int.
+00005600: 2020 2020 2020 2020 2020 2020 4261 7463              Batc
+00005610: 6820 7369 7a65 2074 6f20 7573 6520 6475  h size to use du
+00005620: 7269 6e67 2076 616c 6964 6174 696f 6e20  ring validation 
+00005630: 2864 6566 6175 6c74 3a20 3130 3029 2e0a  (default: 100)..
+00005640: 2020 2020 2020 2020 2020 2020 4d61 7920              May 
+00005650: 6265 206f 7665 7272 6964 6465 6e20 6966  be overridden if
+00005660: 2060 6076 616c 6964 6174 696f 6e5f 6461   ``validation_da
+00005670: 7461 6060 2069 7320 6047 7261 7068 4461  ta`` is `GraphDa
+00005680: 7461 4c6f 6164 6572 6020 6f72 2060 4162  taLoader` or `Ab
+00005690: 7374 7261 6374 4772 6170 6850 6172 7469  stractGraphParti
+000056a0: 7469 6f6e 6572 6020 696e 7374 616e 6365  tioner` instance
+000056b0: 2e0a 2020 2020 2020 2020 7661 6c69 6461  ..        valida
+000056c0: 7469 6f6e 5f66 7265 713a 2069 6e74 0a20  tion_freq: int. 
+000056d0: 2020 2020 2020 2020 2020 2049 6e64 6963             Indic
+000056e0: 6174 6573 2068 6f77 206f 6674 656e 2074  ates how often t
+000056f0: 6f20 7661 6c69 6461 7465 2028 6465 6661  o validate (defa
+00005700: 756c 743a 2035 3029 2e0a 2020 2020 2020  ult: 50)..      
+00005710: 2020 7661 6c69 6461 7469 6f6e 5f62 7572    validation_bur
+00005720: 6e5f 696e 3a20 696e 740a 2020 2020 2020  n_in: int.      
+00005730: 2020 2020 2020 5468 6520 6275 726e 2d69        The burn-i
+00005740: 6e20 7469 6d65 2061 6674 6572 2077 6869  n time after whi
+00005750: 6368 2074 6865 2076 616c 6964 6174 696f  ch the validatio
+00005760: 6e20 6b69 636b 7320 696e 2e0a 2020 2020  n kicks in..    
+00005770: 2020 2020 7661 6c69 6461 7469 6f6e 5f66      validation_f
+00005780: 696c 7465 723a 2062 6f6f 6c20 6f72 2064  ilter: bool or d
+00005790: 6963 740a 2020 2020 2020 2020 2020 2020  ict.            
+000057a0: 5661 6c69 6461 7469 6f6e 2066 696c 7465  Validation filte
+000057b0: 7220 746f 2062 6520 7573 6564 2e0a 2020  r to be used..  
+000057c0: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
+000057d0: 5f65 6e74 6974 6965 735f 7375 6273 6574  _entities_subset
+000057e0: 3a20 6c69 7374 206f 7220 6e70 2e61 7272  : list or np.arr
+000057f0: 6179 0a20 2020 2020 2020 2020 2020 2053  ay.            S
+00005800: 7562 7365 7420 6f66 2065 6e74 6974 6965  ubset of entitie
+00005810: 7320 746f 2062 6520 7573 6564 2066 6f72  s to be used for
+00005820: 2067 656e 6572 6174 696e 6720 636f 7272   generating corr
+00005830: 7570 7469 6f6e 732e 0a0a 2020 2020 2020  uptions...      
+00005840: 2020 2020 2020 2e2e 204e 6f74 6520 3a3a        .. Note ::
+00005850: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005860: 2020 4f6e 6520 6361 6e20 7065 7266 6f72    One can perfor
+00005870: 6d20 6561 726c 7920 7374 6f70 7069 6e67  m early stopping
+00005880: 2075 7369 6e67 2074 6865 2074 656e 736f   using the tenso
+00005890: 7266 6c6f 7720 6361 6c6c 6261 636b 2060  rflow callback `
+000058a0: 6074 662e 6b65 7261 732e 6361 6c6c 6261  `tf.keras.callba
+000058b0: 636b 732e 4561 726c 7953 746f 7070 696e  cks.EarlyStoppin
+000058c0: 6760 600a 2020 2020 2020 2020 2020 2020  g``.            
+000058d0: 2020 2020 6173 2073 686f 776e 2069 6e20      as shown in 
+000058e0: 7468 6520 6163 636f 6d70 616e 7969 6e67  the accompanying
+000058f0: 2065 7861 6d70 6c65 2062 656c 6f77 2e0a   example below..
+00005900: 0a20 2020 2020 2020 2066 6f63 7573 453a  .        focusE:
+00005910: 2062 6f6f 6c0a 2020 2020 2020 2020 2020   bool.          
+00005920: 2020 5370 6563 6966 7920 7768 6574 6865    Specify whethe
+00005930: 7220 746f 2069 6e63 6c75 6465 2074 6865  r to include the
+00005940: 2046 6f63 7573 4520 6c61 7965 7220 2864   FocusE layer (d
+00005950: 6566 6175 6c74 3a20 6046 616c 7365 6029  efault: `False`)
+00005960: 2e0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00005970: 6520 466f 6375 7345 206c 6179 6572 203a  e FocusE layer :
+00005980: 6369 7465 3a60 7061 6932 3032 316c 6561  cite:`pai2021lea
+00005990: 726e 696e 6760 2061 6c6c 6f77 7320 746f  rning` allows to
+000059a0: 2069 6e6a 6563 7420 6e75 6d65 7269 6320   inject numeric 
+000059b0: 6564 6765 2061 7474 7269 6275 7465 7320  edge attributes 
+000059c0: 696e 746f 2074 6865 2073 636f 7269 6e67  into the scoring
+000059d0: 206c 6179 6572 0a20 2020 2020 2020 2020   layer.         
+000059e0: 2020 206f 6620 6120 7472 6164 6974 696f     of a traditio
+000059f0: 6e61 6c20 6b6e 6f77 6c65 6467 6520 6772  nal knowledge gr
+00005a00: 6170 6820 656d 6265 6464 696e 6720 6172  aph embedding ar
+00005a10: 6368 6974 6563 7475 7265 2e0a 2020 2020  chitecture..    
+00005a20: 2020 2020 2020 2020 5365 6d61 6e74 6963          Semantic
+00005a30: 616c 6c79 2c20 7468 6520 6e75 6d65 7269  ally, the numeri
+00005a40: 6320 7661 6c75 6520 6361 6e20 7369 676e  c value can sign
+00005a50: 6966 7920 696d 706f 7274 616e 6365 2c20  ify importance, 
+00005a60: 756e 6365 7274 6169 6e69 7479 2c20 7369  uncertainity, si
+00005a70: 676e 6966 6963 616e 6365 2c20 636f 6e66  gnificance, conf
+00005a80: 6964 656e 6365 2e2e 2e0a 2020 2020 2020  idence....      
+00005a90: 2020 2020 2020 6f66 2061 2074 7269 706c        of a tripl
+00005aa0: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
+00005ab0: 2e2e 204e 6f74 6520 3a3a 0a0a 2020 2020  .. Note ::..    
+00005ac0: 2020 2020 2020 2020 2020 2020 496e 206f              In o
+00005ad0: 7264 6572 2074 6f20 6163 7469 7661 7465  rder to activate
+00005ae0: 2066 6f63 7573 452c 2074 6865 2074 7261   focusE, the tra
+00005af0: 696e 696e 6720 6461 7461 206d 7573 7420  ining data must 
+00005b00: 6861 7665 2073 6861 7065 2028 6e2c 2034  have shape (n, 4
+00005b10: 292c 2077 6865 7265 2074 6865 2066 6972  ), where the fir
+00005b20: 7374 2074 6872 6565 2063 6f6c 756d 6e73  st three columns
+00005b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005b40: 2073 746f 7265 2073 7562 6a65 6374 2c20   store subject, 
+00005b50: 7072 6564 6963 6174 6520 616e 6420 6f62  predicate and ob
+00005b60: 6a65 6374 206f 6620 7472 6970 6c65 732c  ject of triples,
+00005b70: 2061 6e64 2074 6865 2034 2d74 6820 636f   and the 4-th co
+00005b80: 6c75 6d6e 2073 746f 7265 7320 7468 6520  lumn stores the 
+00005b90: 6e75 6d65 7269 6361 6c20 6564 6765 2076  numerical edge v
+00005ba0: 616c 7565 0a20 2020 2020 2020 2020 2020  alue.           
+00005bb0: 2020 2020 2061 7373 6f63 6961 7465 6420       associated 
+00005bc0: 7769 7468 2065 6163 6820 7472 6970 6c65  with each triple
+00005bd0: 2e0a 0a20 2020 2020 2020 2066 6f63 7573  ...        focus
+00005be0: 455f 7061 7261 6d73 3a20 6469 6374 0a20  E_params: dict. 
+00005bf0: 2020 2020 2020 2020 2020 2049 6620 466f             If Fo
+00005c00: 6375 7345 206c 6179 6572 2069 7320 696e  cusE layer is in
+00005c10: 636c 7564 6564 2c20 7370 6563 6966 7920  cluded, specify 
+00005c20: 6974 7320 6879 7065 722d 7061 7261 6d65  its hyper-parame
+00005c30: 7465 7273 2e0a 2020 2020 2020 2020 2020  ters..          
+00005c40: 2020 5468 6520 666f 6c6c 6f77 696e 6720    The following 
+00005c50: 6879 7065 722d 7061 7261 6d73 2063 616e  hyper-params can
+00005c60: 2062 6520 7061 7373 6564 3a0a 0a20 2020   be passed:..   
+00005c70: 2020 2020 2020 2020 202b 2060 226e 6f6e           + `"non
+00005c80: 5f6c 696e 6561 7269 7479 2260 3a20 6361  _linearity"`: ca
+00005c90: 6e20 6265 206f 6e65 206f 6620 7468 6520  n be one of the 
+00005ca0: 666f 6c6c 6f77 696e 6720 7661 6c75 6573  following values
+00005cb0: 2060 226c 696e 6561 7222 602c 2060 2273   `"linear"`, `"s
+00005cc0: 6f66 7470 6c75 7322 602c 2060 2273 6967  oftplus"`, `"sig
+00005cd0: 6d6f 6964 2260 2c20 6022 7461 6e68 2260  moid"`, `"tanh"`
+00005ce0: 2e0a 2020 2020 2020 2020 2020 2020 2b20  ..            + 
+00005cf0: 6022 7374 6f70 5f65 706f 6368 2260 3a20  `"stop_epoch"`: 
+00005d00: 7370 6563 6966 6965 7320 686f 7720 6c6f  specifies how lo
+00005d10: 6e67 2074 6f20 6465 6361 7920 286c 696e  ng to decay (lin
+00005d20: 6561 726c 7929 2074 6865 206e 756d 6572  early) the numer
+00005d30: 6963 2076 616c 7565 7320 6672 6f6d 2031  ic values from 1
+00005d40: 2074 6f20 6f72 6967 696e 616c 2076 616c   to original val
+00005d50: 7565 2e0a 2020 2020 2020 2020 2020 2020  ue..            
+00005d60: 2b20 6022 7374 7275 6374 7572 616c 5f77  + `"structural_w
+00005d70: 7422 603a 2073 7472 7563 7475 7261 6c20  t"`: structural 
+00005d80: 696e 666c 7565 6e63 6520 6879 7065 7270  influence hyperp
+00005d90: 6172 616d 6574 6572 203a 6d61 7468 3a60  arameter :math:`
+00005da0: 5c5c 696e 205b 302c 2031 5d60 2074 6861  \\in [0, 1]` tha
+00005db0: 7420 6d6f 6475 6c61 7465 7320 7468 6520  t modulates the 
+00005dc0: 696e 666c 7565 6e63 6520 6f66 2067 7261  influence of gra
+00005dd0: 7068 2074 6f70 6f6c 6f67 792e 0a0a 2020  ph topology...  
+00005de0: 2020 2020 2020 2020 2020 4966 2060 6066            If ``f
+00005df0: 6f63 7573 453d 3d54 7275 6560 6020 616e  ocusE==True`` an
+00005e00: 6420 6060 666f 6375 7345 5f70 6172 616d  d ``focusE_param
+00005e10: 733d 3d64 6963 7428 2960 602c 2074 6865  s==dict()``, the
+00005e20: 6e20 7468 6520 6465 6661 756c 7420 7661  n the default va
+00005e30: 6c75 6573 2061 7265 2070 6173 7365 643a  lues are passed:
+00005e40: 0a20 2020 2020 2020 2020 2020 2060 606e  .            ``n
+00005e50: 6f6e 5f6c 696e 6561 7269 7479 3d22 6c69  on_linearity="li
+00005e60: 6e65 6172 2260 602c 2060 6073 746f 705f  near"``, ``stop_
+00005e70: 6570 6f63 683d 3235 3160 6020 616e 6420  epoch=251`` and 
+00005e80: 6060 7374 7275 6374 7572 616c 5f77 743d  ``structural_wt=
+00005e90: 302e 3030 3160 602e 0a0a 2020 2020 2020  0.001``...      
+00005ea0: 2020 7061 7274 6974 696f 6e69 6e67 5f6b    partitioning_k
+00005eb0: 3a20 696e 740a 2020 2020 2020 2020 2020  : int.          
+00005ec0: 2020 4e75 6d20 6f66 2070 6172 7469 7469    Num of partiti
+00005ed0: 6f6e 7320 746f 2075 7365 2077 6869 6c65  ons to use while
+00005ee0: 2074 7261 696e 696e 6720 2864 6566 6175   training (defau
+00005ef0: 6c74 3a20 312c 2069 2e65 2e2c 2074 6865  lt: 1, i.e., the
+00005f00: 2064 6174 6120 6973 206e 6f74 2070 6172   data is not par
+00005f10: 7469 7469 6f6e 6564 292e 0a20 2020 2020  titioned)..     
+00005f20: 2020 2020 2020 204d 6179 2062 6520 6f76         May be ov
+00005f30: 6572 7269 6464 656e 2069 6620 6060 7860  erridden if ``x`
+00005f40: 6020 6973 2061 6e20 6041 6273 7472 6163  ` is an `Abstrac
+00005f50: 7447 7261 7068 5061 7274 6974 696f 6e65  tGraphPartitione
+00005f60: 7260 2069 6e73 7461 6e63 652e 0a0a 2020  r` instance...  
+00005f70: 2020 2020 2020 2020 2020 2e2e 204e 6f74            .. Not
+00005f80: 6520 3a3a 0a0a 2020 2020 2020 2020 2020  e ::..          
+00005f90: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
+00005fa0: 696f 6e20 6973 2071 7569 7465 2075 7365  ion is quite use
+00005fb0: 6675 6c20 7768 656e 2074 6865 2073 697a  ful when the siz
+00005fc0: 6520 6f66 2079 6f75 7220 6461 7461 7365  e of your datase
+00005fd0: 7420 6973 2065 7874 7265 6d65 6c79 206c  t is extremely l
+00005fe0: 6172 6765 2061 6e64 2063 616e 6e6f 7420  arge and cannot 
+00005ff0: 6669 7420 696e 206d 656d 6f72 792e 0a20  fit in memory.. 
+00006000: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+00006010: 6574 7469 6e67 2074 6869 7320 746f 2061  etting this to a
+00006020: 206e 756d 6265 7220 7374 7269 6374 6c79   number strictly
+00006030: 206c 6172 6765 7220 7468 616e 2031 2077   larger than 1 w
+00006040: 696c 6c20 6175 746f 6d61 7469 6361 6c6c  ill automaticall
+00006050: 7920 7061 7274 6974 696f 6e20 7468 6520  y partition the 
+00006060: 6461 7461 2075 7369 6e67 0a20 2020 2020  data using.     
+00006070: 2020 2020 2020 2020 2020 2060 6042 7563             ``Buc
+00006080: 6b65 7447 7261 7068 5061 7274 6974 696f  ketGraphPartitio
+00006090: 6e65 7260 602e 0a20 2020 2020 2020 2020  ner``..         
+000060a0: 2020 2020 2020 204b 696e 646c 7920 6368         Kindly ch
+000060b0: 6563 6b6f 7574 2074 6865 2074 7574 6f72  eckout the tutor
+000060c0: 6961 6c73 2066 6f72 2075 7361 6765 2069  ials for usage i
+000060d0: 6e20 4164 7661 6e63 6564 206d 6f64 652e  n Advanced mode.
+000060e0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+000060f0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00006100: 2d0a 2020 2020 2020 2020 6869 7374 6f72  -.        histor
+00006110: 793a 2048 6973 746f 7279 206f 626a 6563  y: History objec
+00006120: 740a 2020 2020 2020 2020 2020 2020 4974  t.            It
+00006130: 7320 6048 6973 746f 7279 2e68 6973 746f  s `History.histo
+00006140: 7279 6020 6174 7472 6962 7574 6520 6973  ry` attribute is
+00006150: 2061 2072 6563 6f72 6420 6f66 2074 7261   a record of tra
+00006160: 696e 696e 6720 6c6f 7373 2076 616c 7565  ining loss value
+00006170: 732c 2061 7320 7765 6c6c 2061 7320 7661  s, as well as va
+00006180: 6c69 6461 7469 6f6e 206c 6f73 730a 2020  lidation loss.  
+00006190: 2020 2020 2020 2020 2020 616e 6420 7661            and va
+000061a0: 6c69 6461 7469 6f6e 206d 6574 7269 6373  lidation metrics
+000061b0: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
+000061c0: 2020 4578 616d 706c 650a 2020 2020 2020    Example.      
+000061d0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+000061e0: 2020 3e3e 3e20 6672 6f6d 2061 6d70 6c69    >>> from ampli
+000061f0: 6772 6170 682e 6461 7461 7365 7473 2069  graph.datasets i
+00006200: 6d70 6f72 7420 6c6f 6164 5f66 6231 356b  mport load_fb15k
+00006210: 5f32 3337 0a20 2020 2020 2020 203e 3e3e  _237.        >>>
+00006220: 2066 726f 6d20 616d 706c 6967 7261 7068   from ampligraph
+00006230: 2e6c 6174 656e 745f 6665 6174 7572 6573  .latent_features
+00006240: 2069 6d70 6f72 7420 5363 6f72 696e 6742   import ScoringB
+00006250: 6173 6564 456d 6265 6464 696e 674d 6f64  asedEmbeddingMod
+00006260: 656c 0a20 2020 2020 2020 203e 3e3e 2058  el.        >>> X
+00006270: 203d 206c 6f61 645f 6662 3135 6b5f 3233   = load_fb15k_23
+00006280: 3728 290a 2020 2020 2020 2020 3e3e 3e20  7().        >>> 
+00006290: 6d6f 6465 6c20 3d20 5363 6f72 696e 6742  model = ScoringB
+000062a0: 6173 6564 456d 6265 6464 696e 674d 6f64  asedEmbeddingMod
+000062b0: 656c 2865 7461 3d35 2c0a 2020 2020 2020  el(eta=5,.      
+000062c0: 2020 3e3e 3e20 2020 2020 2020 2020 2020    >>>           
+000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062e0: 2020 2020 2020 2020 206b 3d33 3030 2c0a           k=300,.
+000062f0: 2020 2020 2020 2020 3e3e 3e20 2020 2020          >>>     
+00006300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006310: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006320: 636f 7269 6e67 5f74 7970 653d 2743 6f6d  coring_type='Com
+00006330: 706c 4578 272c 0a20 2020 2020 2020 203e  plEx',.        >
+00006340: 3e3e 2020 2020 2020 2020 2020 2020 2020  >>              
+00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006360: 2020 2020 2020 7365 6564 3d30 290a 2020        seed=0).  
+00006370: 2020 2020 2020 3e3e 3e20 6d6f 6465 6c2e        >>> model.
+00006380: 636f 6d70 696c 6528 6f70 7469 6d69 7a65  compile(optimize
+00006390: 723d 2761 6461 6d27 2c20 6c6f 7373 3d27  r='adam', loss='
+000063a0: 6e6c 6c27 290a 2020 2020 2020 2020 3e3e  nll').        >>
+000063b0: 3e20 6d6f 6465 6c2e 6669 7428 585b 2774  > model.fit(X['t
+000063c0: 7261 696e 275d 2c0a 2020 2020 2020 2020  rain'],.        
+000063d0: 3e3e 3e20 2020 2020 2020 2020 2020 6261  >>>           ba
+000063e0: 7463 685f 7369 7a65 3d31 3030 3030 2c0a  tch_size=10000,.
+000063f0: 2020 2020 2020 2020 3e3e 3e20 2020 2020          >>>     
+00006400: 2020 2020 2020 6570 6f63 6873 3d35 290a        epochs=5).
+00006410: 2020 2020 2020 2020 4570 6f63 6820 312f          Epoch 1/
+00006420: 350a 2020 2020 2020 2020 3239 2f32 3920  5.        29/29 
+00006430: 5b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  [===============
+00006440: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d5d  ===============]
+00006450: 202d 2032 7320 3731 6d73 2f73 7465 7020   - 2s 71ms/step 
+00006460: 2d20 6c6f 7373 3a20 3637 3336 312e 3330  - loss: 67361.30
+00006470: 3437 0a20 2020 2020 2020 2045 706f 6368  47.        Epoch
+00006480: 2032 2f35 0a20 2020 2020 2020 2032 392f   2/5.        29/
+00006490: 3239 205b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  29 [============
+000064a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000064b0: 3d3d 5d20 2d20 3173 2033 356d 732f 7374  ==] - 1s 35ms/st
+000064c0: 6570 202d 206c 6f73 733a 2036 3733 3138  ep - loss: 67318
+000064d0: 2e36 3039 340a 2020 2020 2020 2020 4570  .6094.        Ep
+000064e0: 6f63 6820 332f 350a 2020 2020 2020 2020  och 3/5.        
+000064f0: 3239 2f32 3920 5b3d 3d3d 3d3d 3d3d 3d3d  29/29 [=========
+00006500: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00006510: 3d3d 3d3d 3d5d 202d 2031 7320 3337 6d73  =====] - 1s 37ms
+00006520: 2f73 7465 7020 2d20 6c6f 7373 3a20 3637  /step - loss: 67
+00006530: 3032 302e 3037 3033 0a20 2020 2020 2020  020.0703.       
+00006540: 2045 706f 6368 2034 2f35 0a20 2020 2020   Epoch 4/5.     
+00006550: 2020 2032 392f 3239 205b 3d3d 3d3d 3d3d     29/29 [======
+00006560: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00006570: 3d3d 3d3d 3d3d 3d3d 5d20 2d20 3173 2033  ========] - 1s 3
+00006580: 356d 732f 7374 6570 202d 206c 6f73 733a  5ms/step - loss:
+00006590: 2036 3538 3637 2e33 3735 300a 2020 2020   65867.3750.    
+000065a0: 2020 2020 4570 6f63 6820 352f 350a 2020      Epoch 5/5.  
+000065b0: 2020 2020 2020 3239 2f32 3920 5b3d 3d3d        29/29 [===
+000065c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000065d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d5d 202d 2031  ===========] - 1
+000065e0: 7320 3335 6d73 2f73 7465 7020 2d20 6c6f  s 35ms/step - lo
+000065f0: 7373 3a20 3633 3531 372e 3930 3632 0a0a  ss: 63517.9062..
+00006600: 2020 2020 2020 2020 3e3e 3e20 2320 4561          >>> # Ea
+00006610: 726c 7920 7374 6f70 7069 6e67 2065 7861  rly stopping exa
+00006620: 6d70 6c65 0a20 2020 2020 2020 203e 3e3e  mple.        >>>
+00006630: 2066 726f 6d20 616d 706c 6967 7261 7068   from ampligraph
+00006640: 2e6c 6174 656e 745f 6665 6174 7572 6573  .latent_features
+00006650: 2069 6d70 6f72 7420 5363 6f72 696e 6742   import ScoringB
+00006660: 6173 6564 456d 6265 6464 696e 674d 6f64  asedEmbeddingMod
+00006670: 656c 0a20 2020 2020 2020 203e 3e3e 2066  el.        >>> f
+00006680: 726f 6d20 616d 706c 6967 7261 7068 2e64  rom ampligraph.d
+00006690: 6174 6173 6574 7320 696d 706f 7274 206c  atasets import l
+000066a0: 6f61 645f 6662 3135 6b5f 3233 370a 2020  oad_fb15k_237.  
+000066b0: 2020 2020 2020 3e3e 3e20 6461 7461 7365        >>> datase
+000066c0: 7420 3d20 6c6f 6164 5f66 6231 356b 5f32  t = load_fb15k_2
+000066d0: 3337 2829 0a20 2020 2020 2020 203e 3e3e  37().        >>>
+000066e0: 206d 6f64 656c 203d 2053 636f 7269 6e67   model = Scoring
+000066f0: 4261 7365 6445 6d62 6564 6469 6e67 4d6f  BasedEmbeddingMo
+00006700: 6465 6c28 6574 613d 312c 0a20 2020 2020  del(eta=1,.     
+00006710: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
+00006720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006730: 2020 2020 2020 2020 2020 6b3d 3130 2c0a            k=10,.
+00006740: 2020 2020 2020 2020 3e3e 3e20 2020 2020          >>>     
+00006750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006760: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006770: 636f 7269 6e67 5f74 7970 653d 2754 7261  coring_type='Tra
+00006780: 6e73 4527 290a 2020 2020 2020 2020 3e3e  nsE').        >>
+00006790: 3e20 6d6f 6465 6c2e 636f 6d70 696c 6528  > model.compile(
+000067a0: 6f70 7469 6d69 7a65 723d 2761 6461 6d27  optimizer='adam'
+000067b0: 2c20 6c6f 7373 3d27 6d75 6c74 6963 6c61  , loss='multicla
+000067c0: 7373 5f6e 6c6c 2729 0a20 2020 2020 2020  ss_nll').       
+000067d0: 203e 3e3e 2069 6d70 6f72 7420 7465 6e73   >>> import tens
+000067e0: 6f72 666c 6f77 2061 7320 7466 0a20 2020  orflow as tf.   
+000067f0: 2020 2020 203e 3e3e 2065 6172 6c79 5f73       >>> early_s
+00006800: 746f 7020 3d20 7466 2e6b 6572 6173 2e63  top = tf.keras.c
+00006810: 616c 6c62 6163 6b73 2e45 6172 6c79 5374  allbacks.EarlySt
+00006820: 6f70 7069 6e67 286d 6f6e 6974 6f72 3d22  opping(monitor="
+00006830: 7661 6c5f 6d72 7222 2c20 2020 2020 2020  val_mrr",       
+00006840: 2020 2020 2023 2077 6869 6368 206d 6574       # which met
+00006850: 7269 6373 2074 6f20 6d6f 6e69 746f 720a  rics to monitor.
+00006860: 2020 2020 2020 2020 3e3e 3e20 2020 2020          >>>     
+00006870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006890: 2020 2020 2020 2020 2020 7061 7469 656e            patien
+000068a0: 6365 3d33 2c20 2020 2020 2020 2020 2020  ce=3,           
+000068b0: 2020 2020 2020 2020 2320 4966 2074 6865          # If the
+000068c0: 206d 6f6e 6974 6f72 6564 206d 6574 7269   monitored metri
+000068d0: 6320 646f 6573 6e74 2069 6d70 726f 7665  c doesnt improve
+000068e0: 2066 6f72 2074 6865 7365 206d 616e 7920   for these many 
+000068f0: 6368 6563 6b73 2074 6865 206d 6f64 656c  checks the model
+00006900: 2065 6172 6c79 2073 746f 7073 0a20 2020   early stops.   
+00006910: 2020 2020 203e 3e3e 2020 2020 2020 2020       >>>        
+00006920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006940: 2020 2020 2020 2076 6572 626f 7365 3d31         verbose=1
+00006950: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
+00006960: 2020 2020 2023 2076 6572 626f 7369 7479       # verbosity
+00006970: 0a20 2020 2020 2020 203e 3e3e 2020 2020  .        >>>    
+00006980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069a0: 2020 2020 2020 2020 2020 206d 6f64 653d             mode=
+000069b0: 226d 6178 222c 2020 2020 2020 2020 2020  "max",          
+000069c0: 2020 2020 2020 2020 2023 2068 6f77 2074           # how t
+000069d0: 6f20 636f 6d70 6172 6520 7468 6520 6d6f  o compare the mo
+000069e0: 6e69 746f 7265 6420 6d65 7472 6963 733b  nitored metrics;
+000069f0: 2022 6d61 7822 206d 6561 6e73 2068 6967   "max" means hig
+00006a00: 6865 7220 6973 2062 6574 7465 720a 2020  her is better.  
+00006a10: 2020 2020 2020 3e3e 3e20 2020 2020 2020        >>>       
+00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a40: 2020 2020 2020 2020 7265 7374 6f72 655f          restore_
+00006a50: 6265 7374 5f77 6569 6768 7473 3d54 7275  best_weights=Tru
+00006a60: 6529 2020 2020 2320 7265 7374 6f72 6520  e)    # restore 
+00006a70: 7468 6520 7765 6967 6874 7320 7769 7468  the weights with
+00006a80: 2062 6573 7420 7661 6c75 650a 2020 2020   best value.    
+00006a90: 2020 2020 3e3e 3e20 2320 7468 6520 6561      >>> # the ea
+00006aa0: 726c 7920 7374 6f70 7069 6e67 2069 6e73  rly stopping ins
+00006ab0: 7461 6e63 6520 6e65 6564 7320 746f 2062  tance needs to b
+00006ac0: 6520 7061 7373 6564 2061 7320 6361 6c6c  e passed as call
+00006ad0: 6261 636b 2074 6f20 6669 7420 6675 6e63  back to fit func
+00006ae0: 7469 6f6e 0a20 2020 2020 2020 203e 3e3e  tion.        >>>
+00006af0: 206d 6f64 656c 2e66 6974 2864 6174 6173   model.fit(datas
+00006b00: 6574 5b27 7472 6169 6e27 5d2c 0a20 2020  et['train'],.   
+00006b10: 2020 2020 203e 3e3e 2020 2020 2020 2020       >>>        
+00006b20: 2020 2062 6174 6368 5f73 697a 653d 3130     batch_size=10
+00006b30: 3030 302c 0a20 2020 2020 2020 203e 3e3e  000,.        >>>
+00006b40: 2020 2020 2020 2020 2020 2065 706f 6368             epoch
+00006b50: 733d 352c 0a20 2020 2020 2020 203e 3e3e  s=5,.        >>>
+00006b60: 2020 2020 2020 2020 2020 2076 616c 6964             valid
+00006b70: 6174 696f 6e5f 6672 6571 3d31 2c20 2020  ation_freq=1,   
+00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b90: 2020 2020 2320 7661 6c69 6461 7469 6f6e      # validation
+00006ba0: 2066 7265 7175 656e 6379 0a20 2020 2020   frequency.     
+00006bb0: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
+00006bc0: 2076 616c 6964 6174 696f 6e5f 6261 7463   validation_batc
+00006bd0: 685f 7369 7a65 3d31 3030 2c20 2020 2020  h_size=100,     
+00006be0: 2020 2020 2020 2020 2020 2320 7661 6c69            # vali
+00006bf0: 6461 7469 6f6e 2062 6174 6368 2073 697a  dation batch siz
+00006c00: 650a 2020 2020 2020 2020 3e3e 3e20 2020  e.        >>>   
+00006c10: 2020 2020 2020 2020 7661 6c69 6461 7469          validati
+00006c20: 6f6e 5f62 7572 6e5f 696e 3d33 2c20 2020  on_burn_in=3,   
+00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c40: 2023 2062 7572 6e20 696e 2074 696d 650a   # burn in time.
+00006c50: 2020 2020 2020 2020 3e3e 3e20 2020 2020          >>>     
+00006c60: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
+00006c70: 5f63 6f72 7275 7074 5f73 6964 653d 2773  _corrupt_side='s
+00006c80: 2c6f 272c 2020 2020 2020 2020 2020 2023  ,o',           #
+00006c90: 2077 6869 6368 2073 6964 6520 746f 2063   which side to c
+00006ca0: 6f72 7275 7074 0a20 2020 2020 2020 203e  orrupt.        >
+00006cb0: 3e3e 2020 2020 2020 2020 2020 2076 616c  >>           val
+00006cc0: 6964 6174 696f 6e5f 6461 7461 3d64 6174  idation_data=dat
+00006cd0: 6173 6574 5b27 7661 6c69 6427 5d5b 3a3a  aset['valid'][::
+00006ce0: 3130 305d 2c20 2320 5661 6c69 6461 7469  100], # Validati
+00006cf0: 6f6e 2064 6174 610a 2020 2020 2020 2020  on data.        
+00006d00: 3e3e 3e20 2020 2020 2020 2020 2020 6361  >>>           ca
+00006d10: 6c6c 6261 636b 733d 5b65 6172 6c79 5f73  llbacks=[early_s
+00006d20: 746f 705d 2920 2020 2020 2020 2020 2020  top])           
+00006d30: 2020 2020 2020 2023 2050 6173 7320 7468         # Pass th
+00006d40: 6520 6561 726c 7920 7374 6f70 7069 6e67  e early stopping
+00006d50: 206f 626a 6563 7420 6173 2061 2063 616c   object as a cal
+00006d60: 6c62 6163 6b0a 2020 2020 2020 2020 4570  lback.        Ep
+00006d70: 6f63 6820 312f 350a 2020 2020 2020 2020  och 1/5.        
+00006d80: 3239 2f32 3920 5b3d 3d3d 3d3d 3d3d 3d3d  29/29 [=========
+00006d90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00006da0: 3d3d 3d3d 3d5d 202d 2032 7320 3832 6d73  =====] - 2s 82ms
+00006db0: 2f73 7465 7020 2d20 6c6f 7373 3a20 3636  /step - loss: 66
+00006dc0: 3938 2e32 3138 380a 2020 2020 2020 2020  98.2188.        
+00006dd0: 4570 6f63 6820 322f 350a 2020 2020 2020  Epoch 2/5.      
+00006de0: 2020 3239 2f32 3920 5b3d 3d3d 3d3d 3d3d    29/29 [=======
+00006df0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00006e00: 3d3d 3d3d 3d3d 3d5d 202d 2031 7320 3334  =======] - 1s 34
+00006e10: 6d73 2f73 7465 7020 2d20 6c6f 7373 3a20  ms/step - loss: 
+00006e20: 3636 3438 2e38 3836 320a 2020 2020 2020  6648.8862.      
+00006e30: 2020 4570 6f63 6820 332f 350a 2020 2020    Epoch 3/5.    
+00006e40: 2020 2020 332f 3320 5b3d 3d3d 3d3d 3d3d      3/3 [=======
+00006e50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00006e60: 3d3d 3d3d 3d3d 3d5d 202d 2031 7320 3434  =======] - 1s 44
+00006e70: 366d 732f 7374 6570 6f73 733a 2036 3635  6ms/steposs: 665
+00006e80: 322e 3839 350a 2020 2020 2020 2020 3239  2.895.        29
+00006e90: 2f32 3920 5b3d 3d3d 3d3d 3d3d 3d3d 3d3d  /29 [===========
+00006ea0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00006eb0: 3d3d 3d5d 202d 2032 7320 3834 6d73 2f73  ===] - 2s 84ms/s
+00006ec0: 7465 7020 2d20 6c6f 7373 3a20 3635 3930  tep - loss: 6590
+00006ed0: 2e32 3834 3220 2d20 7661 6c5f 6d72 723a  .2842 - val_mrr:
+00006ee0: 2030 2e30 3831 3120 2d0a 2020 2020 2020   0.0811 -.      
+00006ef0: 2020 7661 6c5f 6d72 3a20 3137 3736 2e34    val_mr: 1776.4
+00006f00: 3534 3520 2d20 7661 6c5f 6869 7473 4031  545 - val_hits@1
+00006f10: 3a20 302e 3030 3030 652b 3030 202d 2076  : 0.0000e+00 - v
+00006f20: 616c 5f68 6974 7340 3130 3a20 302e 3233  al_hits@10: 0.23
+00006f30: 3031 202d 2076 616c 5f68 6974 7340 3130  01 - val_hits@10
+00006f40: 303a 2030 2e34 3134 380a 2020 2020 2020  0: 0.4148.      
+00006f50: 2020 4570 6f63 6820 342f 350a 2020 2020    Epoch 4/5.    
+00006f60: 2020 2020 332f 3320 5b3d 3d3d 3d3d 3d3d      3/3 [=======
+00006f70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00006f80: 3d3d 3d3d 3d3d 3d5d 202d 2030 7320 3130  =======] - 0s 10
+00006f90: 326d 732f 7374 6570 6f73 733a 2036 3536  2ms/steposs: 656
+00006fa0: 342e 3032 310a 2020 2020 2020 2020 3239  4.021.        29
+00006fb0: 2f32 3920 5b3d 3d3d 3d3d 3d3d 3d3d 3d3d  /29 [===========
+00006fc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00006fd0: 3d3d 3d5d 202d 2031 7320 3437 6d73 2f73  ===] - 1s 47ms/s
+00006fe0: 7465 7020 2d20 6c6f 7373 3a20 3635 3137  tep - loss: 6517
+00006ff0: 2e34 3531 3720 2d20 7661 6c5f 6d72 723a  .4517 - val_mrr:
+00007000: 2030 2e30 3931 3820 2d0a 2020 2020 2020   0.0918 -.      
+00007010: 2020 7661 6c5f 6d72 3a20 3133 3136 2e36    val_mr: 1316.6
+00007020: 3333 3520 2d20 7661 6c5f 6869 7473 4031  335 - val_hits@1
+00007030: 3a20 302e 3030 3030 652b 3030 202d 2076  : 0.0000e+00 - v
+00007040: 616c 5f68 6974 7340 3130 3a20 302e 3235  al_hits@10: 0.25
+00007050: 3238 202d 2076 616c 5f68 6974 7340 3130  28 - val_hits@10
+00007060: 303a 2030 2e34 3731 360a 2020 2020 2020  0: 0.4716.      
+00007070: 2020 4570 6f63 6820 352f 350a 2020 2020    Epoch 5/5.    
+00007080: 2020 2020 332f 3320 5b3d 3d3d 3d3d 3d3d      3/3 [=======
+00007090: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000070a0: 3d3d 3d3d 3d3d 3d5d 202d 2031 7320 3137  =======] - 1s 17
+000070b0: 376d 732f 7374 6570 6f73 733a 2036 3436  7ms/steposs: 646
+000070c0: 382e 3739 380a 2020 2020 2020 2020 3239  8.798.        29
+000070d0: 2f32 3920 5b3d 3d3d 3d3d 3d3d 3d3d 3d3d  /29 [===========
+000070e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000070f0: 3d3d 3d5d 202d 2032 7320 3632 6d73 2f73  ===] - 2s 62ms/s
+00007100: 7465 7020 2d20 6c6f 7373 3a20 3634 3331  tep - loss: 6431
+00007110: 2e38 3639 3620 2d20 7661 6c5f 6d72 723a  .8696 - val_mrr:
+00007120: 2030 2e30 3930 3120 2d0a 2020 2020 2020   0.0901 -.      
+00007130: 2020 7661 6c5f 6d72 3a20 3130 3734 2e38    val_mr: 1074.8
+00007140: 3932 3020 2d20 7661 6c5f 6869 7473 4031  920 - val_hits@1
+00007150: 3a20 302e 3030 3030 652b 3030 202d 2076  : 0.0000e+00 - v
+00007160: 616c 5f68 6974 7340 3130 3a20 302e 3233  al_hits@10: 0.23
+00007170: 3836 202d 2076 616c 5f68 6974 7340 3130  86 - val_hits@10
+00007180: 303a 2030 2e34 3737 330a 0a20 2020 2020  0: 0.4773..     
+00007190: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
+000071a0: 2076 6572 6966 6965 7320 6966 2063 6f6d   verifies if com
+000071b0: 7069 6c65 2068 6173 2062 6565 6e20 6361  pile has been ca
+000071c0: 6c6c 6564 2062 6566 6f72 6520 6361 6c6c  lled before call
+000071d0: 696e 6720 6669 740a 2020 2020 2020 2020  ing fit.        
+000071e0: 7365 6c66 2e5f 6173 7365 7274 5f63 6f6d  self._assert_com
+000071f0: 7069 6c65 5f77 6173 5f63 616c 6c65 6428  pile_was_called(
+00007200: 290a 2020 2020 2020 2020 2320 666f 6375  ).        # focu
+00007210: 7345 0a20 2020 2020 2020 2073 656c 662e  sE.        self.
+00007220: 6375 7272 656e 745f 6570 6f63 6820 3d20  current_epoch = 
+00007230: 300a 2020 2020 2020 2020 7365 6c66 2e75  0.        self.u
+00007240: 7365 5f66 6f63 7573 4520 3d20 666f 6375  se_focusE = focu
+00007250: 7345 0a0a 2020 2020 2020 2020 2320 7573  sE..        # us
+00007260: 6520 7472 6169 6e20 7465 7374 2075 6e73  e train test uns
+00007270: 6565 6e20 746f 2073 706c 6974 2074 7261  een to split tra
+00007280: 696e 696e 6720 7365 740a 2020 2020 2020  ining set.      
+00007290: 2020 6966 2076 616c 6964 6174 696f 6e5f    if validation_
+000072a0: 7370 6c69 743a 0a20 2020 2020 2020 2020  split:.         
+000072b0: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
+000072c0: 616e 6365 280a 2020 2020 2020 2020 2020  ance(.          
+000072d0: 2020 2020 2020 782c 206e 702e 6e64 6172        x, np.ndar
+000072e0: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
+000072f0: 292c 2022 5661 6c69 6461 7469 6f6e 2073  ), "Validation s
+00007300: 706c 6974 2073 7570 706f 7274 6564 2066  plit supported f
+00007310: 6f72 206e 756d 7079 2061 7272 6179 7320  or numpy arrays 
+00007320: 6f6e 6c79 2122 0a20 2020 2020 2020 2020  only!".         
+00007330: 2020 2078 2c20 7661 6c69 6461 7469 6f6e     x, validation
+00007340: 5f64 6174 6120 3d20 7472 6169 6e5f 7465  _data = train_te
+00007350: 7374 5f73 706c 6974 5f6e 6f5f 756e 7365  st_split_no_unse
+00007360: 656e 280a 2020 2020 2020 2020 2020 2020  en(.            
+00007370: 2020 2020 782c 0a20 2020 2020 2020 2020      x,.         
+00007380: 2020 2020 2020 2074 6573 745f 7369 7a65         test_size
+00007390: 3d76 616c 6964 6174 696f 6e5f 7370 6c69  =validation_spli
+000073a0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+000073b0: 2020 2073 6565 643d 7365 6c66 2e73 6565     seed=self.see
+000073c0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+000073d0: 2020 2061 6c6c 6f77 5f64 7570 6c69 6361     allow_duplica
+000073e0: 7469 6f6e 3d46 616c 7365 2c0a 2020 2020  tion=False,.    
+000073f0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00007400: 2020 2077 6974 6820 7472 6169 6e69 6e67     with training
+00007410: 5f75 7469 6c73 2e52 6573 7065 6374 436f  _utils.RespectCo
+00007420: 6d70 696c 6564 5472 6169 6e61 626c 6553  mpiledTrainableS
+00007430: 7461 7465 2873 656c 6629 3a0a 2020 2020  tate(self):.    
+00007440: 2020 2020 2020 2020 2320 6372 6561 7465          # create
+00007450: 2064 6174 6120 6861 6e64 6c65 7220 666f   data handler fo
+00007460: 7220 7468 6520 6461 7461 0a20 2020 2020  r the data.     
+00007470: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
+00007480: 5f68 616e 646c 6572 203d 2064 6174 615f  _handler = data_
+00007490: 6164 6170 7465 722e 4461 7461 4861 6e64  adapter.DataHand
+000074a0: 6c65 7228 0a20 2020 2020 2020 2020 2020  ler(.           
+000074b0: 2020 2020 2078 2c0a 2020 2020 2020 2020       x,.        
+000074c0: 2020 2020 2020 2020 6d6f 6465 6c3d 7365          model=se
+000074d0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+000074e0: 2020 2020 6261 7463 685f 7369 7a65 3d62      batch_size=b
+000074f0: 6174 6368 5f73 697a 652c 0a20 2020 2020  atch_size,.     
+00007500: 2020 2020 2020 2020 2020 2064 6174 6173             datas
+00007510: 6574 5f74 7970 653d 2274 7261 696e 222c  et_type="train",
+00007520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007530: 2065 706f 6368 733d 6570 6f63 6873 2c0a   epochs=epochs,.
+00007540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007550: 696e 6974 6961 6c5f 6570 6f63 683d 696e  initial_epoch=in
+00007560: 6974 6961 6c5f 6570 6f63 682c 0a20 2020  itial_epoch,.   
+00007570: 2020 2020 2020 2020 2020 2020 2075 7365               use
+00007580: 5f66 696c 7465 723d 4661 6c73 652c 0a20  _filter=False,. 
+00007590: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000075a0: 2069 6620 6d6f 6465 6c20 6973 2061 6c72   if model is alr
+000075b0: 6561 6479 0a20 2020 2020 2020 2020 2020  eady.           
+000075c0: 2020 2020 2023 2074 7261 696e 6564 2075       # trained u
+000075d0: 7365 2074 6865 206f 6c64 0a20 2020 2020  se the old.     
+000075e0: 2020 2020 2020 2020 2020 2023 2069 6e64             # ind
+000075f0: 6578 6572 0a20 2020 2020 2020 2020 2020  exer.           
+00007600: 2020 2020 2075 7365 5f69 6e64 6578 6572       use_indexer
+00007610: 3d73 656c 662e 6461 7461 5f69 6e64 6578  =self.data_index
+00007620: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+00007630: 2020 2020 7061 7274 6974 696f 6e69 6e67      partitioning
+00007640: 5f6b 3d70 6172 7469 7469 6f6e 696e 675f  _k=partitioning_
+00007650: 6b2c 0a20 2020 2020 2020 2020 2020 2029  k,.            )
+00007660: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00007670: 6c66 2e70 6172 7469 7469 6f6e 6572 5f6d  lf.partitioner_m
+00007680: 6574 6164 6174 6120 3d20 280a 2020 2020  etadata = (.    
+00007690: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000076a0: 2e64 6174 615f 6861 6e64 6c65 722e 6765  .data_handler.ge
+000076b0: 745f 7570 6461 7465 5f70 6172 7469 7469  t_update_partiti
+000076c0: 6f6e 6572 5f6d 6574 6164 6174 6128 0a20  oner_metadata(. 
+000076d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076e0: 2020 2073 656c 662e 6261 7365 5f64 6972     self.base_dir
+000076f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007700: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
+00007710: 0a20 2020 2020 2020 2020 2020 2023 2067  .            # g
+00007720: 6574 2074 6865 206d 6170 7069 6e67 2064  et the mapping d
+00007730: 6574 6169 6c73 0a20 2020 2020 2020 2020  etails.         
+00007740: 2020 2073 656c 662e 6461 7461 5f69 6e64     self.data_ind
+00007750: 6578 6572 203d 2073 656c 662e 6461 7461  exer = self.data
+00007760: 5f68 616e 646c 6572 2e67 6574 5f6d 6170  _handler.get_map
+00007770: 7065 7228 290a 2020 2020 2020 2020 2020  per().          
+00007780: 2020 2320 6765 7420 7468 6520 6d61 7869    # get the maxi
+00007790: 6d75 6d20 656e 7469 7469 6573 2061 6e64  mum entities and
+000077a0: 2072 656c 6174 696f 6e73 2074 6861 7420   relations that 
+000077b0: 7769 6c6c 2062 6520 7472 6169 6e65 640a  will be trained.
+000077c0: 2020 2020 2020 2020 2020 2020 2320 2875              # (u
+000077d0: 7365 6675 6c20 6475 7269 6e67 2070 6172  seful during par
+000077e0: 7469 7469 6f6e 696e 6729 0a20 2020 2020  titioning).     
+000077f0: 2020 2020 2020 2073 656c 662e 6d61 785f         self.max_
+00007800: 656e 745f 7369 7a65 203d 2073 656c 662e  ent_size = self.
+00007810: 6461 7461 5f68 616e 646c 6572 2e5f 6164  data_handler._ad
+00007820: 6170 7465 722e 6d61 785f 656e 7469 7469  apter.max_entiti
+00007830: 6573 0a20 2020 2020 2020 2020 2020 2073  es.            s
+00007840: 656c 662e 6d61 785f 7265 6c5f 7369 7a65  elf.max_rel_size
+00007850: 203d 2073 656c 662e 6461 7461 5f68 616e   = self.data_han
+00007860: 646c 6572 2e5f 6164 6170 7465 722e 6d61  dler._adapter.ma
+00007870: 785f 7265 6c61 7469 6f6e 730a 2020 2020  x_relations.    
+00007880: 2020 2020 2020 2020 2320 4e75 6d62 6572          # Number
+00007890: 206f 6620 636f 6c75 6d6e 7320 2869 2e65   of columns (i.e
+000078a0: 2e2c 206f 6e6c 7920 7472 6970 6c65 7320  ., only triples 
+000078b0: 6f72 2061 6c73 6f20 7765 6967 6874 733f  or also weights?
+000078c0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+000078d0: 2069 7369 6e73 7461 6e63 6528 7365 6c66   isinstance(self
+000078e0: 2e64 6174 615f 6861 6e64 6c65 722e 5f61  .data_handler._a
+000078f0: 6461 7074 6572 2c20 5061 7274 6974 696f  dapter, Partitio
+00007900: 6e44 6174 614d 616e 6167 6572 293a 0a20  nDataManager):. 
+00007910: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007920: 656c 662e 6461 7461 5f73 6861 7065 203d  elf.data_shape =
+00007930: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00007940: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
+00007950: 5f68 616e 646c 6572 2e5f 7061 7265 6e74  _handler._parent
+00007960: 5f61 6461 7074 6572 2e62 6163 6b65 6e64  _adapter.backend
+00007970: 2e64 6174 615f 7368 6170 650a 2020 2020  .data_shape.    
+00007980: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00007990: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000079a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079b0: 7365 6c66 2e64 6174 615f 7368 6170 6520  self.data_shape 
+000079c0: 3d20 7365 6c66 2e64 6174 615f 6861 6e64  = self.data_hand
+000079d0: 6c65 722e 5f61 6461 7074 6572 2e62 6163  ler._adapter.bac
+000079e0: 6b65 6e64 2e64 6174 615f 7368 6170 650a  kend.data_shape.
+000079f0: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
+00007a00: 6f63 7573 450a 2020 2020 2020 2020 2020  ocusE.          
+00007a10: 2020 6966 2073 656c 662e 6461 7461 5f73    if self.data_s
+00007a20: 6861 7065 203c 2034 3a0a 2020 2020 2020  hape < 4:.      
+00007a30: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00007a40: 7365 5f66 6f63 7573 4520 3d20 4661 6c73  se_focusE = Fals
+00007a50: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
+00007a60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00007a70: 2020 2020 6966 2073 656c 662e 7573 655f      if self.use_
+00007a80: 666f 6375 7345 3a0a 2020 2020 2020 2020  focusE:.        
+00007a90: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00007aa0: 7274 2069 7369 6e73 7461 6e63 6528 0a20  rt isinstance(. 
 00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ac0: 7374 6f70 5f65 706f 6368 2c0a 2020 2020  stop_epoch,.    
-00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ae0: 2020 2020 7374 7275 6374 7572 655f 7765      structure_we
-00007af0: 6967 6874 2c0a 2020 2020 2020 2020 2020  ight,.          
-00007b00: 2020 2020 2020 2020 2020 2920 3d20 7365            ) = se
-00007b10: 6c66 2e67 6574 5f66 6f63 7573 455f 7061  lf.get_focusE_pa
-00007b20: 7261 6d73 2866 6f63 7573 455f 7061 7261  rams(focusE_para
-00007b30: 6d73 290a 2020 2020 2020 2020 2020 2020  ms).            
-00007b40: 2020 2020 2020 2020 7365 6c66 2e66 6f63          self.foc
-00007b50: 7573 455f 7061 7261 6d73 203d 207b 0a20  usE_params = {. 
+00007ac0: 2020 2020 2020 2066 6f63 7573 455f 7061         focusE_pa
+00007ad0: 7261 6d73 2c20 6469 6374 0a20 2020 2020  rams, dict.     
+00007ae0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00007af0: 2c20 2266 6f63 7573 4520 7061 7261 6d65  , "focusE parame
+00007b00: 7465 7273 206e 6565 6420 746f 2062 6520  ters need to be 
+00007b10: 696e 2061 2064 6963 7421 220a 2020 2020  in a dict!".    
+00007b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b30: 2320 4465 6669 6e65 2046 6f63 7573 4520  # Define FocusE 
+00007b40: 7061 7261 6d73 0a20 2020 2020 2020 2020  params.         
+00007b50: 2020 2020 2020 2020 2020 2028 0a20 2020             (.   
 00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b70: 2020 2020 2020 2022 6e6f 6e5f 6c69 6e65         "non_line
-00007b80: 6172 6974 7922 3a20 6e6f 6e5f 6c69 6e65  arity": non_line
-00007b90: 6172 6974 792c 0a20 2020 2020 2020 2020  arity,.         
-00007ba0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00007bb0: 7374 6f70 5f65 706f 6368 223a 2073 746f  stop_epoch": sto
-00007bc0: 705f 6570 6f63 682c 0a20 2020 2020 2020  p_epoch,.       
-00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007be0: 2022 7374 7275 6374 7572 616c 5f77 7422   "structural_wt"
-00007bf0: 3a20 7374 7275 6374 7572 655f 7765 6967  : structure_weig
-00007c00: 6874 2c0a 2020 2020 2020 2020 2020 2020  ht,.            
-00007c10: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00007c20: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c40: 2020 2020 7072 696e 7428 0a20 2020 2020      print(.     
-00007c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c60: 2020 2022 4461 7461 2073 6861 7065 2069     "Data shape i
-00007c70: 7320 7b7d 3a20 6e6f 7420 6f6e 6c79 2074  s {}: not only t
-00007c80: 7269 706c 6573 2077 6572 6520 6769 7665  riples were give
-00007c90: 6e2c 2062 7574 2066 6f63 7573 4520 6973  n, but focusE is
-00007ca0: 206e 6f74 2061 6374 6976 6521 222e 666f   not active!".fo
-00007cb0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cd0: 2020 7365 6c66 2e64 6174 615f 7368 6170    self.data_shap
-00007ce0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00007cf0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00007d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d10: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00007d20: 2043 6f6e 7461 696e 6572 2074 6861 7420   Container that 
-00007d30: 636f 6e66 6967 7572 6573 2061 6e64 2063  configures and c
-00007d40: 616c 6c73 2060 7466 2e6b 6572 6173 2e43  alls `tf.keras.C
-00007d50: 616c 6c62 6163 6b60 732e 0a20 2020 2020  allback`s..     
-00007d60: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-00007d70: 696e 7374 616e 6365 2863 616c 6c62 6163  instance(callbac
-00007d80: 6b73 2c20 6361 6c6c 6261 636b 735f 6d6f  ks, callbacks_mo
-00007d90: 6475 6c65 2e43 616c 6c62 6163 6b4c 6973  dule.CallbackLis
-00007da0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00007db0: 2020 2020 6361 6c6c 6261 636b 7320 3d20      callbacks = 
-00007dc0: 6361 6c6c 6261 636b 735f 6d6f 6475 6c65  callbacks_module
-00007dd0: 2e43 616c 6c62 6163 6b4c 6973 7428 0a20  .CallbackList(. 
-00007de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007df0: 2020 2063 616c 6c62 6163 6b73 2c0a 2020     callbacks,.  
-00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e10: 2020 6164 645f 6869 7374 6f72 793d 5472    add_history=Tr
-00007e20: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00007e30: 2020 2020 2020 2020 6164 645f 7072 6f67          add_prog
-00007e40: 6261 723d 7665 7262 6f73 6520 213d 2030  bar=verbose != 0
-00007e50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007e60: 2020 2020 2020 6d6f 6465 6c3d 7365 6c66        model=self
-00007e70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007e80: 2020 2020 2020 7665 7262 6f73 653d 7665        verbose=ve
-00007e90: 7262 6f73 652c 0a20 2020 2020 2020 2020  rbose,.         
-00007ea0: 2020 2020 2020 2020 2020 2065 706f 6368             epoch
-00007eb0: 733d 6570 6f63 6873 2c0a 2020 2020 2020  s=epochs,.      
-00007ec0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00007ed0: 2020 2020 2020 2020 2023 2054 6869 7320           # This 
-00007ee0: 7661 7269 6162 6c65 2069 7320 7573 6564  variable is used
-00007ef0: 2062 7920 6361 6c6c 6261 636b 7320 746f   by callbacks to
-00007f00: 2073 746f 7020 7472 6169 6e69 6e67 2069   stop training i
-00007f10: 6e20 6361 7365 206f 660a 2020 2020 2020  n case of.      
-00007f20: 2020 2020 2020 2320 616e 7920 6572 726f        # any erro
-00007f30: 720a 2020 2020 2020 2020 2020 2020 7365  r.            se
-00007f40: 6c66 2e73 746f 705f 7472 6169 6e69 6e67  lf.stop_training
-00007f50: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-00007f60: 2020 2020 2073 656c 662e 6973 5f70 6172       self.is_par
-00007f70: 7469 7469 6f6e 6564 5f74 7261 696e 696e  titioned_trainin
-00007f80: 6720 3d20 7365 6c66 2e64 6174 615f 6861  g = self.data_ha
-00007f90: 6e64 6c65 722e 7573 696e 675f 7061 7274  ndler.using_part
-00007fa0: 6974 696f 6e69 6e67 0a20 2020 2020 2020  itioning.       
-00007fb0: 2020 2020 2073 656c 662e 6f70 7469 6d69       self.optimi
-00007fc0: 7a65 722e 7365 745f 7061 7274 6974 696f  zer.set_partitio
-00007fd0: 6e65 645f 7472 6169 6e69 6e67 280a 2020  ned_training(.  
-00007fe0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00007ff0: 6c66 2e69 735f 7061 7274 6974 696f 6e65  lf.is_partitione
-00008000: 645f 7472 6169 6e69 6e67 0a20 2020 2020  d_training.     
-00008010: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00008020: 2020 2020 2020 2320 7365 7420 736f 6d65        # set some
-00008030: 2070 6172 7469 7469 6f6e 2072 656c 6174   partition relat
-00008040: 6564 2070 6172 616d 7320 6966 2069 7420  ed params if it 
-00008050: 6973 2070 6172 7469 7469 6f6e 6564 2074  is partitioned t
-00008060: 7261 696e 696e 670a 2020 2020 2020 2020  raining.        
-00008070: 2020 2020 6966 2073 656c 662e 6973 5f70      if self.is_p
-00008080: 6172 7469 7469 6f6e 6564 5f74 7261 696e  artitioned_train
-00008090: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
-000080a0: 2020 2020 2073 656c 662e 7061 7274 6974       self.partit
-000080b0: 696f 6e65 725f 6b20 3d20 7365 6c66 2e64  ioner_k = self.d
-000080c0: 6174 615f 6861 6e64 6c65 722e 5f61 6461  ata_handler._ada
-000080d0: 7074 6572 2e70 6172 7469 7469 6f6e 6572  pter.partitioner
-000080e0: 5f6b 0a20 2020 2020 2020 2020 2020 2020  _k.             
-000080f0: 2020 2073 656c 662e 656e 636f 6469 6e67     self.encoding
-00008100: 5f6c 6179 6572 2e6d 6178 5f65 6e74 5f73  _layer.max_ent_s
-00008110: 697a 6520 3d20 7365 6c66 2e6d 6178 5f65  ize = self.max_e
-00008120: 6e74 5f73 697a 650a 2020 2020 2020 2020  nt_size.        
-00008130: 2020 2020 2020 2020 7365 6c66 2e65 6e63          self.enc
-00008140: 6f64 696e 675f 6c61 7965 722e 6d61 785f  oding_layer.max_
-00008150: 7265 6c5f 7369 7a65 203d 2073 656c 662e  rel_size = self.
-00008160: 6d61 785f 7265 6c5f 7369 7a65 0a0a 2020  max_rel_size..  
-00008170: 2020 2020 2020 2020 2020 2320 6d61 6b65            # make
-00008180: 2074 6865 2074 7261 696e 2066 756e 6374   the train funct
-00008190: 696f 6e20 7468 6174 2077 696c 6c20 6265  ion that will be
-000081a0: 2075 7365 6420 746f 2070 726f 6365 7373   used to process
-000081b0: 2065 6163 6820 6261 7463 680a 2020 2020   each batch.    
-000081c0: 2020 2020 2020 2020 2320 6f66 2064 6174          # of dat
-000081d0: 610a 2020 2020 2020 2020 2020 2020 7472  a.            tr
-000081e0: 6169 6e5f 6675 6e63 7469 6f6e 203d 2073  ain_function = s
-000081f0: 656c 662e 6d61 6b65 5f74 7261 696e 5f66  elf.make_train_f
-00008200: 756e 6374 696f 6e28 290a 2020 2020 2020  unction().      
-00008210: 2020 2020 2020 2320 6265 666f 7265 2074        # before t
-00008220: 7261 696e 696e 6720 6265 6769 6e73 2063  raining begins c
-00008230: 616c 6c20 7468 6973 2063 616c 6c62 6163  all this callbac
-00008240: 6b20 6675 6e63 7469 6f6e 0a20 2020 2020  k function.     
-00008250: 2020 2020 2020 2063 616c 6c62 6163 6b73         callbacks
-00008260: 2e6f 6e5f 7472 6169 6e5f 6265 6769 6e28  .on_train_begin(
-00008270: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00008280: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-00008290: 2020 2020 6973 696e 7374 616e 6365 2876      isinstance(v
-000082a0: 616c 6964 6174 696f 6e5f 656e 7469 7469  alidation_entiti
-000082b0: 6573 5f73 7562 7365 742c 2073 7472 290a  es_subset, str).
-000082c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082d0: 616e 6420 7661 6c69 6461 7469 6f6e 5f65  and validation_e
-000082e0: 6e74 6974 6965 735f 7375 6273 6574 203d  ntities_subset =
-000082f0: 3d20 2261 6c6c 220a 2020 2020 2020 2020  = "all".        
-00008300: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-00008310: 2020 2020 2020 2023 2069 6620 7468 6520         # if the 
-00008320: 7375 6273 6574 2069 7320 7365 7420 746f  subset is set to
-00008330: 206e 6f6e 652c 2069 7420 7769 6c6c 2075   none, it will u
-00008340: 7365 2061 6c6c 2065 6e74 6974 6965 7320  se all entities 
-00008350: 696e 2074 6865 0a20 2020 2020 2020 2020  in the.         
-00008360: 2020 2020 2020 2023 2067 7261 7068 2066         # graph f
-00008370: 6f72 2067 656e 6572 6174 696e 6720 636f  or generating co
-00008380: 7272 7570 7469 6f6e 730a 2020 2020 2020  rruptions.      
-00008390: 2020 2020 2020 2020 2020 7661 6c69 6461            valida
-000083a0: 7469 6f6e 5f65 6e74 6974 6965 735f 7375  tion_entities_su
-000083b0: 6273 6574 203d 204e 6f6e 650a 0a20 2020  bset = None..   
-000083c0: 2020 2020 2020 2020 2023 2065 6e75 6d65           # enume
-000083d0: 7261 7465 206f 7665 7220 7468 6520 6461  rate over the da
-000083e0: 7461 0a20 2020 2020 2020 2020 2020 2066  ta.            f
-000083f0: 6f72 2065 706f 6368 2c20 6974 6572 6174  or epoch, iterat
-00008400: 6f72 2069 6e20 7365 6c66 2e64 6174 615f  or in self.data_
-00008410: 6861 6e64 6c65 722e 656e 756d 6572 6174  handler.enumerat
-00008420: 655f 6570 6f63 6873 2829 3a0a 2020 2020  e_epochs():.    
-00008430: 2020 2020 2020 2020 2020 2020 2320 6375              # cu
-00008440: 7272 656e 7420 6570 6f63 6820 6e75 6d62  rrent epoch numb
-00008450: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
-00008460: 2020 2073 656c 662e 6375 7272 656e 745f     self.current_
-00008470: 6570 6f63 6820 3d20 6570 6f63 680a 2020  epoch = epoch.  
-00008480: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00008490: 6265 666f 7265 2065 706f 6368 2062 6567  before epoch beg
-000084a0: 696e 7320 6361 6c6c 2074 6869 7320 6361  ins call this ca
-000084b0: 6c6c 6261 636b 2066 756e 6374 696f 6e0a  llback function.
-000084c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084d0: 6361 6c6c 6261 636b 732e 6f6e 5f65 706f  callbacks.on_epo
-000084e0: 6368 5f62 6567 696e 2865 706f 6368 290a  ch_begin(epoch).
-000084f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008500: 2320 5570 6461 7465 2066 6f63 7573 4520  # Update focusE 
-00008510: 7061 7261 6d65 7465 720a 2020 2020 2020  parameter.      
-00008520: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00008530: 662e 7573 655f 666f 6375 7345 3a0a 2020  f.use_focusE:.  
-00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008550: 2020 7365 6c66 2e75 7064 6174 655f 666f    self.update_fo
-00008560: 6375 7345 5f70 6172 616d 7328 290a 2020  cusE_params().  
-00008570: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00008580: 6861 6e64 6c65 2074 6865 2073 746f 7020  handle the stop 
-00008590: 6974 6572 6174 696f 6e20 6f66 2064 6174  iteration of dat
-000085a0: 6120 6974 6572 6174 6f72 2069 6e20 7468  a iterator in th
-000085b0: 6973 2073 636f 7065 0a20 2020 2020 2020  is scope.       
-000085c0: 2020 2020 2020 2020 2077 6974 6820 7365           with se
-000085d0: 6c66 2e64 6174 615f 6861 6e64 6c65 722e  lf.data_handler.
-000085e0: 6361 7463 685f 7374 6f70 5f69 7465 7261  catch_stop_itera
-000085f0: 7469 6f6e 2829 3a0a 2020 2020 2020 2020  tion():.        
-00008600: 2020 2020 2020 2020 2020 2020 2320 6974              # it
-00008610: 6572 6174 6520 6f76 6572 2074 6865 2064  erate over the d
-00008620: 6174 6173 6574 0a20 2020 2020 2020 2020  ataset.         
-00008630: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-00008640: 7465 7020 696e 2073 656c 662e 6461 7461  tep in self.data
-00008650: 5f68 616e 646c 6572 2e73 7465 7073 2829  _handler.steps()
-00008660: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008670: 2020 2020 2020 2020 2020 2320 6265 666f            # befo
-00008680: 7265 2061 2062 6174 6368 2069 7320 7072  re a batch is pr
-00008690: 6f63 6573 7365 6420 6361 6c6c 2074 6869  ocessed call thi
-000086a0: 7320 6361 6c6c 6261 636b 0a20 2020 2020  s callback.     
-000086b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086c0: 2020 2023 2066 756e 6374 696f 6e0a 2020     # function.  
-000086d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086e0: 2020 2020 2020 6361 6c6c 6261 636b 732e        callbacks.
-000086f0: 6f6e 5f74 7261 696e 5f62 6174 6368 5f62  on_train_batch_b
-00008700: 6567 696e 2873 7465 7029 0a0a 2020 2020  egin(step)..    
-00008710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008720: 2020 2020 2320 7072 6f63 6573 7320 7468      # process th
-00008730: 6973 2062 6174 6368 0a20 2020 2020 2020  is batch.       
+00007b70: 2020 2020 206e 6f6e 5f6c 696e 6561 7269       non_lineari
+00007b80: 7479 2c0a 2020 2020 2020 2020 2020 2020  ty,.            
+00007b90: 2020 2020 2020 2020 2020 2020 7374 6f70              stop
+00007ba0: 5f65 706f 6368 2c0a 2020 2020 2020 2020  _epoch,.        
+00007bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bc0: 7374 7275 6374 7572 655f 7765 6967 6874  structure_weight
+00007bd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007be0: 2020 2020 2020 2920 3d20 7365 6c66 2e67        ) = self.g
+00007bf0: 6574 5f66 6f63 7573 455f 7061 7261 6d73  et_focusE_params
+00007c00: 2866 6f63 7573 455f 7061 7261 6d73 290a  (focusE_params).
+00007c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c20: 2020 2020 7365 6c66 2e66 6f63 7573 455f      self.focusE_
+00007c30: 7061 7261 6d73 203d 207b 0a20 2020 2020  params = {.     
+00007c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c50: 2020 2022 6e6f 6e5f 6c69 6e65 6172 6974     "non_linearit
+00007c60: 7922 3a20 6e6f 6e5f 6c69 6e65 6172 6974  y": non_linearit
+00007c70: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
+00007c80: 2020 2020 2020 2020 2020 2022 7374 6f70             "stop
+00007c90: 5f65 706f 6368 223a 2073 746f 705f 6570  _epoch": stop_ep
+00007ca0: 6f63 682c 0a20 2020 2020 2020 2020 2020  och,.           
+00007cb0: 2020 2020 2020 2020 2020 2020 2022 7374               "st
+00007cc0: 7275 6374 7572 616c 5f77 7422 3a20 7374  ructural_wt": st
+00007cd0: 7275 6374 7572 655f 7765 6967 6874 2c0a  ructure_weight,.
+00007ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cf0: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00007d00: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d20: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
+00007d30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00007d40: 4461 7461 2073 6861 7065 2069 7320 7b7d  Data shape is {}
+00007d50: 3a20 6e6f 7420 6f6e 6c79 2074 7269 706c  : not only tripl
+00007d60: 6573 2077 6572 6520 6769 7665 6e2c 2062  es were given, b
+00007d70: 7574 2066 6f63 7573 4520 6973 206e 6f74  ut focusE is not
+00007d80: 2061 6374 6976 6521 222e 666f 726d 6174   active!".format
+00007d90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00007da0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00007db0: 6c66 2e64 6174 615f 7368 6170 650a 2020  lf.data_shape.  
+00007dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007dd0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00007de0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00007df0: 2020 2020 2020 2020 2020 2023 2043 6f6e             # Con
+00007e00: 7461 696e 6572 2074 6861 7420 636f 6e66  tainer that conf
+00007e10: 6967 7572 6573 2061 6e64 2063 616c 6c73  igures and calls
+00007e20: 2060 7466 2e6b 6572 6173 2e43 616c 6c62   `tf.keras.Callb
+00007e30: 6163 6b60 732e 0a20 2020 2020 2020 2020  ack`s..         
+00007e40: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+00007e50: 616e 6365 2863 616c 6c62 6163 6b73 2c20  ance(callbacks, 
+00007e60: 6361 6c6c 6261 636b 735f 6d6f 6475 6c65  callbacks_module
+00007e70: 2e43 616c 6c62 6163 6b4c 6973 7429 3a0a  .CallbackList):.
+00007e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e90: 6361 6c6c 6261 636b 7320 3d20 6361 6c6c  callbacks = call
+00007ea0: 6261 636b 735f 6d6f 6475 6c65 2e43 616c  backs_module.Cal
+00007eb0: 6c62 6163 6b4c 6973 7428 0a20 2020 2020  lbackList(.     
+00007ec0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00007ed0: 616c 6c62 6163 6b73 2c0a 2020 2020 2020  allbacks,.      
+00007ee0: 2020 2020 2020 2020 2020 2020 2020 6164                ad
+00007ef0: 645f 6869 7374 6f72 793d 5472 7565 2c0a  d_history=True,.
+00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f10: 2020 2020 6164 645f 7072 6f67 6261 723d      add_progbar=
+00007f20: 7665 7262 6f73 6520 213d 2030 2c0a 2020  verbose != 0,.  
+00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f40: 2020 6d6f 6465 6c3d 7365 6c66 2c0a 2020    model=self,.  
+00007f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f60: 2020 7665 7262 6f73 653d 7665 7262 6f73    verbose=verbos
+00007f70: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00007f80: 2020 2020 2020 2065 706f 6368 733d 6570         epochs=ep
+00007f90: 6f63 6873 2c0a 2020 2020 2020 2020 2020  ochs,.          
+00007fa0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00007fb0: 2020 2020 2023 2054 6869 7320 7661 7269       # This vari
+00007fc0: 6162 6c65 2069 7320 7573 6564 2062 7920  able is used by 
+00007fd0: 6361 6c6c 6261 636b 7320 746f 2073 746f  callbacks to sto
+00007fe0: 7020 7472 6169 6e69 6e67 2069 6e20 6361  p training in ca
+00007ff0: 7365 206f 660a 2020 2020 2020 2020 2020  se of.          
+00008000: 2020 2320 616e 7920 6572 726f 720a 2020    # any error.  
+00008010: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00008020: 746f 705f 7472 6169 6e69 6e67 203d 2046  top_training = F
+00008030: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+00008040: 2073 656c 662e 6973 5f70 6172 7469 7469   self.is_partiti
+00008050: 6f6e 6564 5f74 7261 696e 696e 6720 3d20  oned_training = 
+00008060: 7365 6c66 2e64 6174 615f 6861 6e64 6c65  self.data_handle
+00008070: 722e 7573 696e 675f 7061 7274 6974 696f  r.using_partitio
+00008080: 6e69 6e67 0a20 2020 2020 2020 2020 2020  ning.           
+00008090: 2073 656c 662e 6f70 7469 6d69 7a65 722e   self.optimizer.
+000080a0: 7365 745f 7061 7274 6974 696f 6e65 645f  set_partitioned_
+000080b0: 7472 6169 6e69 6e67 280a 2020 2020 2020  training(.      
+000080c0: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
+000080d0: 735f 7061 7274 6974 696f 6e65 645f 7472  s_partitioned_tr
+000080e0: 6169 6e69 6e67 0a20 2020 2020 2020 2020  aining.         
+000080f0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+00008100: 2020 2320 7365 7420 736f 6d65 2070 6172    # set some par
+00008110: 7469 7469 6f6e 2072 656c 6174 6564 2070  tition related p
+00008120: 6172 616d 7320 6966 2069 7420 6973 2070  arams if it is p
+00008130: 6172 7469 7469 6f6e 6564 2074 7261 696e  artitioned train
+00008140: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00008150: 6966 2073 656c 662e 6973 5f70 6172 7469  if self.is_parti
+00008160: 7469 6f6e 6564 5f74 7261 696e 696e 673a  tioned_training:
+00008170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008180: 2073 656c 662e 7061 7274 6974 696f 6e65   self.partitione
+00008190: 725f 6b20 3d20 7365 6c66 2e64 6174 615f  r_k = self.data_
+000081a0: 6861 6e64 6c65 722e 5f61 6461 7074 6572  handler._adapter
+000081b0: 2e70 6172 7469 7469 6f6e 6572 5f6b 0a20  .partitioner_k. 
+000081c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000081d0: 656c 662e 656e 636f 6469 6e67 5f6c 6179  elf.encoding_lay
+000081e0: 6572 2e6d 6178 5f65 6e74 5f73 697a 6520  er.max_ent_size 
+000081f0: 3d20 7365 6c66 2e6d 6178 5f65 6e74 5f73  = self.max_ent_s
+00008200: 697a 650a 2020 2020 2020 2020 2020 2020  ize.            
+00008210: 2020 2020 7365 6c66 2e65 6e63 6f64 696e      self.encodin
+00008220: 675f 6c61 7965 722e 6d61 785f 7265 6c5f  g_layer.max_rel_
+00008230: 7369 7a65 203d 2073 656c 662e 6d61 785f  size = self.max_
+00008240: 7265 6c5f 7369 7a65 0a0a 2020 2020 2020  rel_size..      
+00008250: 2020 2020 2020 2320 6d61 6b65 2074 6865        # make the
+00008260: 2074 7261 696e 2066 756e 6374 696f 6e20   train function 
+00008270: 7468 6174 2077 696c 6c20 6265 2075 7365  that will be use
+00008280: 6420 746f 2070 726f 6365 7373 2065 6163  d to process eac
+00008290: 6820 6261 7463 680a 2020 2020 2020 2020  h batch.        
+000082a0: 2020 2020 2320 6f66 2064 6174 610a 2020      # of data.  
+000082b0: 2020 2020 2020 2020 2020 7472 6169 6e5f            train_
+000082c0: 6675 6e63 7469 6f6e 203d 2073 656c 662e  function = self.
+000082d0: 6d61 6b65 5f74 7261 696e 5f66 756e 6374  make_train_funct
+000082e0: 696f 6e28 290a 2020 2020 2020 2020 2020  ion().          
+000082f0: 2020 2320 6265 666f 7265 2074 7261 696e    # before train
+00008300: 696e 6720 6265 6769 6e73 2063 616c 6c20  ing begins call 
+00008310: 7468 6973 2063 616c 6c62 6163 6b20 6675  this callback fu
+00008320: 6e63 7469 6f6e 0a20 2020 2020 2020 2020  nction.         
+00008330: 2020 2063 616c 6c62 6163 6b73 2e6f 6e5f     callbacks.on_
+00008340: 7472 6169 6e5f 6265 6769 6e28 290a 0a20  train_begin().. 
+00008350: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
+00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008370: 6973 696e 7374 616e 6365 2876 616c 6964  isinstance(valid
+00008380: 6174 696f 6e5f 656e 7469 7469 6573 5f73  ation_entities_s
+00008390: 7562 7365 742c 2073 7472 290a 2020 2020  ubset, str).    
+000083a0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+000083b0: 7661 6c69 6461 7469 6f6e 5f65 6e74 6974  validation_entit
+000083c0: 6965 735f 7375 6273 6574 203d 3d20 2261  ies_subset == "a
+000083d0: 6c6c 220a 2020 2020 2020 2020 2020 2020  ll".            
+000083e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000083f0: 2020 2023 2069 6620 7468 6520 7375 6273     # if the subs
+00008400: 6574 2069 7320 7365 7420 746f 206e 6f6e  et is set to non
+00008410: 652c 2069 7420 7769 6c6c 2075 7365 2061  e, it will use a
+00008420: 6c6c 2065 6e74 6974 6965 7320 696e 2074  ll entities in t
+00008430: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
+00008440: 2020 2023 2067 7261 7068 2066 6f72 2067     # graph for g
+00008450: 656e 6572 6174 696e 6720 636f 7272 7570  enerating corrup
+00008460: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
+00008470: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
+00008480: 5f65 6e74 6974 6965 735f 7375 6273 6574  _entities_subset
+00008490: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+000084a0: 2020 2020 2023 2065 6e75 6d65 7261 7465       # enumerate
+000084b0: 206f 7665 7220 7468 6520 6461 7461 0a20   over the data. 
+000084c0: 2020 2020 2020 2020 2020 2066 6f72 2065             for e
+000084d0: 706f 6368 2c20 6974 6572 6174 6f72 2069  poch, iterator i
+000084e0: 6e20 7365 6c66 2e64 6174 615f 6861 6e64  n self.data_hand
+000084f0: 6c65 722e 656e 756d 6572 6174 655f 6570  ler.enumerate_ep
+00008500: 6f63 6873 2829 3a0a 2020 2020 2020 2020  ochs():.        
+00008510: 2020 2020 2020 2020 2320 6375 7272 656e          # curren
+00008520: 7420 6570 6f63 6820 6e75 6d62 6572 0a20  t epoch number. 
+00008530: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00008540: 656c 662e 6375 7272 656e 745f 6570 6f63  elf.current_epoc
+00008550: 6820 3d20 6570 6f63 680a 2020 2020 2020  h = epoch.      
+00008560: 2020 2020 2020 2020 2020 2320 6265 666f            # befo
+00008570: 7265 2065 706f 6368 2062 6567 696e 7320  re epoch begins 
+00008580: 6361 6c6c 2074 6869 7320 6361 6c6c 6261  call this callba
+00008590: 636b 2066 756e 6374 696f 6e0a 2020 2020  ck function.    
+000085a0: 2020 2020 2020 2020 2020 2020 6361 6c6c              call
+000085b0: 6261 636b 732e 6f6e 5f65 706f 6368 5f62  backs.on_epoch_b
+000085c0: 6567 696e 2865 706f 6368 290a 2020 2020  egin(epoch).    
+000085d0: 2020 2020 2020 2020 2020 2020 2320 5570              # Up
+000085e0: 6461 7465 2066 6f63 7573 4520 7061 7261  date focusE para
+000085f0: 6d65 7465 720a 2020 2020 2020 2020 2020  meter.          
+00008600: 2020 2020 2020 6966 2073 656c 662e 7573        if self.us
+00008610: 655f 666f 6375 7345 3a0a 2020 2020 2020  e_focusE:.      
+00008620: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00008630: 6c66 2e75 7064 6174 655f 666f 6375 7345  lf.update_focusE
+00008640: 5f70 6172 616d 7328 290a 2020 2020 2020  _params().      
+00008650: 2020 2020 2020 2020 2020 2320 6861 6e64            # hand
+00008660: 6c65 2074 6865 2073 746f 7020 6974 6572  le the stop iter
+00008670: 6174 696f 6e20 6f66 2064 6174 6120 6974  ation of data it
+00008680: 6572 6174 6f72 2069 6e20 7468 6973 2073  erator in this s
+00008690: 636f 7065 0a20 2020 2020 2020 2020 2020  cope.           
+000086a0: 2020 2020 2077 6974 6820 7365 6c66 2e64       with self.d
+000086b0: 6174 615f 6861 6e64 6c65 722e 6361 7463  ata_handler.catc
+000086c0: 685f 7374 6f70 5f69 7465 7261 7469 6f6e  h_stop_iteration
+000086d0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000086e0: 2020 2020 2020 2020 2320 6974 6572 6174          # iterat
+000086f0: 6520 6f76 6572 2074 6865 2064 6174 6173  e over the datas
+00008700: 6574 0a20 2020 2020 2020 2020 2020 2020  et.             
+00008710: 2020 2020 2020 2066 6f72 2073 7465 7020         for step 
+00008720: 696e 2073 656c 662e 6461 7461 5f68 616e  in self.data_han
+00008730: 646c 6572 2e73 7465 7073 2829 3a0a 2020  dler.steps():.  
 00008740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008750: 206c 6f67 7320 3d20 7472 6169 6e5f 6675   logs = train_fu
-00008760: 6e63 7469 6f6e 2869 7465 7261 746f 7229  nction(iterator)
-00008770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008780: 2020 2020 2020 2020 2023 2061 6674 6572           # after
-00008790: 2061 2062 6174 6368 2069 7320 7072 6f63   a batch is proc
-000087a0: 6573 7365 6420 6361 6c6c 2074 6869 7320  essed call this 
-000087b0: 6361 6c6c 6261 636b 0a20 2020 2020 2020  callback.       
-000087c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087d0: 2023 2066 756e 6374 696f 6e0a 2020 2020   # function.    
-000087e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087f0: 2020 2020 6361 6c6c 6261 636b 732e 6f6e      callbacks.on
-00008800: 5f74 7261 696e 5f62 6174 6368 5f65 6e64  _train_batch_end
-00008810: 2873 7465 702c 206c 6f67 7329 0a0a 2020  (step, logs)..  
-00008820: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00008830: 7374 6f72 6520 7468 6520 6c6f 6773 206f  store the logs o
-00008840: 6620 7468 6520 6c61 7374 2062 6174 6368  f the last batch
-00008850: 206f 6620 7468 6520 6570 6f63 680a 2020   of the epoch.  
-00008860: 2020 2020 2020 2020 2020 2020 2020 6570                ep
-00008870: 6f63 685f 6c6f 6773 203d 2063 6f70 792e  och_logs = copy.
-00008880: 636f 7079 286c 6f67 7329 0a20 2020 2020  copy(logs).     
-00008890: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
-000088a0: 7661 6c69 6461 7469 6f6e 2069 7320 656e  validation is en
-000088b0: 6162 6c65 640a 2020 2020 2020 2020 2020  abled.          
-000088c0: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
-000088d0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000088e0: 706f 6368 203e 3d20 2876 616c 6964 6174  poch >= (validat
-000088f0: 696f 6e5f 6275 726e 5f69 6e20 2d20 3129  ion_burn_in - 1)
-00008900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008910: 2020 2020 2061 6e64 2076 616c 6964 6174       and validat
-00008920: 696f 6e5f 6461 7461 2069 7320 6e6f 7420  ion_data is not 
-00008930: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00008940: 2020 2020 2020 2020 2061 6e64 2073 656c           and sel
-00008950: 662e 5f73 686f 756c 645f 6576 616c 2865  f._should_eval(e
-00008960: 706f 6368 2c20 7661 6c69 6461 7469 6f6e  poch, validation
-00008970: 5f66 7265 7129 0a20 2020 2020 2020 2020  _freq).         
-00008980: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00008990: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000089a0: 2073 656c 662e 6461 7461 5f73 6861 7065   self.data_shape
-000089b0: 203e 2033 2061 6e64 2076 616c 6964 6174   > 3 and validat
-000089c0: 696f 6e5f 6461 7461 2e73 6861 7065 5b31  ion_data.shape[1
-000089d0: 5d20 3d3d 2033 3a0a 2020 2020 2020 2020  ] == 3:.        
+00008750: 2020 2020 2020 2320 6265 666f 7265 2061        # before a
+00008760: 2062 6174 6368 2069 7320 7072 6f63 6573   batch is proces
+00008770: 7365 6420 6361 6c6c 2074 6869 7320 6361  sed call this ca
+00008780: 6c6c 6261 636b 0a20 2020 2020 2020 2020  llback.         
+00008790: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000087a0: 2066 756e 6374 696f 6e0a 2020 2020 2020   function.      
+000087b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087c0: 2020 6361 6c6c 6261 636b 732e 6f6e 5f74    callbacks.on_t
+000087d0: 7261 696e 5f62 6174 6368 5f62 6567 696e  rain_batch_begin
+000087e0: 2873 7465 7029 0a0a 2020 2020 2020 2020  (step)..        
+000087f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008800: 2320 7072 6f63 6573 7320 7468 6973 2062  # process this b
+00008810: 6174 6368 0a20 2020 2020 2020 2020 2020  atch.           
+00008820: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00008830: 7320 3d20 7472 6169 6e5f 6675 6e63 7469  s = train_functi
+00008840: 6f6e 2869 7465 7261 746f 7229 0a20 2020  on(iterator).   
+00008850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008860: 2020 2020 2023 2061 6674 6572 2061 2062       # after a b
+00008870: 6174 6368 2069 7320 7072 6f63 6573 7365  atch is processe
+00008880: 6420 6361 6c6c 2074 6869 7320 6361 6c6c  d call this call
+00008890: 6261 636b 0a20 2020 2020 2020 2020 2020  back.           
+000088a0: 2020 2020 2020 2020 2020 2020 2023 2066               # f
+000088b0: 756e 6374 696f 6e0a 2020 2020 2020 2020  unction.        
+000088c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088d0: 6361 6c6c 6261 636b 732e 6f6e 5f74 7261  callbacks.on_tra
+000088e0: 696e 5f62 6174 6368 5f65 6e64 2873 7465  in_batch_end(ste
+000088f0: 702c 206c 6f67 7329 0a0a 2020 2020 2020  p, logs)..      
+00008900: 2020 2020 2020 2020 2020 2320 7374 6f72            # stor
+00008910: 6520 7468 6520 6c6f 6773 206f 6620 7468  e the logs of th
+00008920: 6520 6c61 7374 2062 6174 6368 206f 6620  e last batch of 
+00008930: 7468 6520 6570 6f63 680a 2020 2020 2020  the epoch.      
+00008940: 2020 2020 2020 2020 2020 6570 6f63 685f            epoch_
+00008950: 6c6f 6773 203d 2063 6f70 792e 636f 7079  logs = copy.copy
+00008960: 286c 6f67 7329 0a20 2020 2020 2020 2020  (logs).         
+00008970: 2020 2020 2020 2023 2069 6620 7661 6c69         # if vali
+00008980: 6461 7469 6f6e 2069 7320 656e 6162 6c65  dation is enable
+00008990: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+000089a0: 2020 6966 2028 0a20 2020 2020 2020 2020    if (.         
+000089b0: 2020 2020 2020 2020 2020 2065 706f 6368             epoch
+000089c0: 203e 3d20 2876 616c 6964 6174 696f 6e5f   >= (validation_
+000089d0: 6275 726e 5f69 6e20 2d20 3129 0a20 2020  burn_in - 1).   
 000089e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089f0: 6e61 6e5f 7765 6967 6874 7320 3d20 6e70  nan_weights = np
-00008a00: 2e65 6d70 7479 2876 616c 6964 6174 696f  .empty(validatio
-00008a10: 6e5f 6461 7461 2e73 6861 7065 5b30 5d29  n_data.shape[0])
-00008a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008a30: 2020 2020 2020 2020 206e 616e 5f77 6569           nan_wei
-00008a40: 6768 7473 2e66 696c 6c28 6e70 2e6e 616e  ghts.fill(np.nan
-00008a50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00008a60: 2020 2020 2020 2020 2020 7661 6c69 6461            valida
-00008a70: 7469 6f6e 5f64 6174 6120 3d20 6e70 2e63  tion_data = np.c
-00008a80: 6f6e 6361 7465 6e61 7465 280a 2020 2020  oncatenate(.    
-00008a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008aa0: 2020 2020 2020 2020 5b76 616c 6964 6174          [validat
-00008ab0: 696f 6e5f 6461 7461 2c20 6e61 6e5f 7765  ion_data, nan_we
-00008ac0: 6967 6874 735d 2c20 6178 6973 3d31 0a20  ights], axis=1. 
-00008ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ae0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00008af0: 2020 2020 2020 2020 2020 2020 2023 2065               # e
-00008b00: 7661 6c75 6174 6520 6f6e 2074 6865 2076  valuate on the v
-00008b10: 616c 6964 6174 696f 6e0a 2020 2020 2020  alidation.      
-00008b20: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00008b30: 6e6b 7320 3d20 7365 6c66 2e65 7661 6c75  nks = self.evalu
-00008b40: 6174 6528 0a20 2020 2020 2020 2020 2020  ate(.           
-00008b50: 2020 2020 2020 2020 2020 2020 2076 616c               val
-00008b60: 6964 6174 696f 6e5f 6461 7461 2c0a 2020  idation_data,.  
+000089f0: 2061 6e64 2076 616c 6964 6174 696f 6e5f   and validation_
+00008a00: 6461 7461 2069 7320 6e6f 7420 4e6f 6e65  data is not None
+00008a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008a20: 2020 2020 2061 6e64 2073 656c 662e 5f73       and self._s
+00008a30: 686f 756c 645f 6576 616c 2865 706f 6368  hould_eval(epoch
+00008a40: 2c20 7661 6c69 6461 7469 6f6e 5f66 7265  , validation_fre
+00008a50: 7129 0a20 2020 2020 2020 2020 2020 2020  q).             
+00008a60: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00008a70: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00008a80: 662e 6461 7461 5f73 6861 7065 203e 2033  f.data_shape > 3
+00008a90: 2061 6e64 2076 616c 6964 6174 696f 6e5f   and validation_
+00008aa0: 6461 7461 2e73 6861 7065 5b31 5d20 3d3d  data.shape[1] ==
+00008ab0: 2033 3a0a 2020 2020 2020 2020 2020 2020   3:.            
+00008ac0: 2020 2020 2020 2020 2020 2020 6e61 6e5f              nan_
+00008ad0: 7765 6967 6874 7320 3d20 6e70 2e65 6d70  weights = np.emp
+00008ae0: 7479 2876 616c 6964 6174 696f 6e5f 6461  ty(validation_da
+00008af0: 7461 2e73 6861 7065 5b30 5d29 0a20 2020  ta.shape[0]).   
+00008b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b10: 2020 2020 206e 616e 5f77 6569 6768 7473       nan_weights
+00008b20: 2e66 696c 6c28 6e70 2e6e 616e 290a 2020  .fill(np.nan).  
+00008b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b40: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
+00008b50: 5f64 6174 6120 3d20 6e70 2e63 6f6e 6361  _data = np.conca
+00008b60: 7465 6e61 7465 280a 2020 2020 2020 2020  tenate(.        
 00008b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b80: 2020 2020 2020 6261 7463 685f 7369 7a65        batch_size
-00008b90: 3d76 616c 6964 6174 696f 6e5f 6261 7463  =validation_batc
-00008ba0: 685f 7369 7a65 206f 7220 6261 7463 685f  h_size or batch_
-00008bb0: 7369 7a65 2c0a 2020 2020 2020 2020 2020  size,.          
-00008bc0: 2020 2020 2020 2020 2020 2020 2020 7573                us
-00008bd0: 655f 6669 6c74 6572 3d76 616c 6964 6174  e_filter=validat
-00008be0: 696f 6e5f 6669 6c74 6572 2c0a 2020 2020  ion_filter,.    
-00008bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c00: 2020 2020 6461 7461 7365 745f 7479 7065      dataset_type
-00008c10: 3d22 7661 6c69 6422 2c0a 2020 2020 2020  ="valid",.      
-00008c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c30: 2020 636f 7272 7570 745f 7369 6465 3d76    corrupt_side=v
-00008c40: 616c 6964 6174 696f 6e5f 636f 7272 7570  alidation_corrup
-00008c50: 745f 7369 6465 2c0a 2020 2020 2020 2020  t_side,.        
-00008c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c70: 656e 7469 7469 6573 5f73 7562 7365 743d  entities_subset=
-00008c80: 7661 6c69 6461 7469 6f6e 5f65 6e74 6974  validation_entit
-00008c90: 6965 735f 7375 6273 6574 2c0a 2020 2020  ies_subset,.    
-00008ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00008cc0: 2020 2020 2020 2320 636f 6d70 7574 6520        # compute 
-00008cd0: 616c 6c20 7468 6520 6d65 7472 6963 730a  all the metrics.
-00008ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cf0: 2020 2020 7661 6c5f 6c6f 6773 203d 207b      val_logs = {
-00008d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008d10: 2020 2020 2020 2020 2022 7661 6c5f 6d72           "val_mr
-00008d20: 7222 3a20 6d72 725f 7363 6f72 6528 7261  r": mrr_score(ra
-00008d30: 6e6b 7329 2c0a 2020 2020 2020 2020 2020  nks),.          
-00008d40: 2020 2020 2020 2020 2020 2020 2020 2276                "v
-00008d50: 616c 5f6d 7222 3a20 6d72 5f73 636f 7265  al_mr": mr_score
-00008d60: 2872 616e 6b73 292c 0a20 2020 2020 2020  (ranks),.       
-00008d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d80: 2022 7661 6c5f 6869 7473 4031 223a 2068   "val_hits@1": h
-00008d90: 6974 735f 6174 5f6e 5f73 636f 7265 2872  its_at_n_score(r
-00008da0: 616e 6b73 2c20 3129 2c0a 2020 2020 2020  anks, 1),.      
-00008db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008dc0: 2020 2276 616c 5f68 6974 7340 3130 223a    "val_hits@10":
-00008dd0: 2068 6974 735f 6174 5f6e 5f73 636f 7265   hits_at_n_score
-00008de0: 2872 616e 6b73 2c20 3130 292c 0a20 2020  (ranks, 10),.   
-00008df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e00: 2020 2020 2022 7661 6c5f 6869 7473 4031       "val_hits@1
-00008e10: 3030 223a 2068 6974 735f 6174 5f6e 5f73  00": hits_at_n_s
-00008e20: 636f 7265 2872 616e 6b73 2c20 3130 3029  core(ranks, 100)
-00008e30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008e40: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00008e50: 2020 2020 2020 2020 2020 2020 2320 7570              # up
-00008e60: 6461 7465 2074 6865 2065 706f 6368 206c  date the epoch l
-00008e70: 6f67 7320 7769 7468 2076 616c 6964 6174  ogs with validat
-00008e80: 696f 6e20 6465 7461 696c 730a 2020 2020  ion details.    
-00008e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ea0: 6570 6f63 685f 6c6f 6773 2e75 7064 6174  epoch_logs.updat
-00008eb0: 6528 7661 6c5f 6c6f 6773 290a 0a20 2020  e(val_logs)..   
-00008ec0: 2020 2020 2020 2020 2020 2020 2023 2061               # a
-00008ed0: 6674 6572 2061 6e20 6570 6f63 6820 6973  fter an epoch is
-00008ee0: 2063 6f6d 706c 6574 6564 2c20 6361 6c6c   completed, call
-00008ef0: 2074 6869 7320 6361 6c6c 6261 636b 2066   this callback f
-00008f00: 756e 6374 696f 6e0a 2020 2020 2020 2020  unction.        
-00008f10: 2020 2020 2020 2020 6361 6c6c 6261 636b          callback
-00008f20: 732e 6f6e 5f65 706f 6368 5f65 6e64 2865  s.on_epoch_end(e
-00008f30: 706f 6368 2c20 6570 6f63 685f 6c6f 6773  poch, epoch_logs
-00008f40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00008f50: 2020 6966 2073 656c 662e 7374 6f70 5f74    if self.stop_t
-00008f60: 7261 696e 696e 673a 0a20 2020 2020 2020  raining:.       
-00008f70: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-00008f80: 616b 0a0a 2020 2020 2020 2020 2020 2020  ak..            
-00008f90: 2320 6f6e 2074 7261 696e 696e 6720 656e  # on training en
-00008fa0: 6420 6361 6c6c 2074 6869 7320 6d65 7468  d call this meth
-00008fb0: 6f64 0a20 2020 2020 2020 2020 2020 2063  od.            c
-00008fc0: 616c 6c62 6163 6b73 2e6f 6e5f 7472 6169  allbacks.on_trai
-00008fd0: 6e5f 656e 6428 290a 2020 2020 2020 2020  n_end().        
-00008fe0: 2020 2020 7365 6c66 2e69 735f 6669 7474      self.is_fitt
-00008ff0: 6564 203d 2054 7275 650a 2020 2020 2020  ed = True.      
-00009000: 2020 2020 2020 2320 616c 6c20 7468 6520        # all the 
-00009010: 7472 6169 6e69 6e67 2061 6e64 2076 616c  training and val
-00009020: 6964 6174 696f 6e20 6c6f 6773 2061 7265  idation logs are
-00009030: 2073 746f 7265 6420 696e 2074 6865 2068   stored in the h
-00009040: 6973 746f 7279 0a20 2020 2020 2020 2020  istory.         
-00009050: 2020 2023 206f 626a 6563 7420 6279 206b     # object by k
-00009060: 6572 6173 2e4d 6f64 656c 0a20 2020 2020  eras.Model.     
-00009070: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00009080: 6c66 2e68 6973 746f 7279 0a0a 2020 2020  lf.history..    
-00009090: 6465 6620 6765 745f 696e 6465 7865 7328  def get_indexes(
-000090a0: 7365 6c66 2c20 582c 2074 7970 655f 6f66  self, X, type_of
-000090b0: 3d22 7422 2c20 6f72 6465 723d 2272 6177  ="t", order="raw
-000090c0: 3269 6e64 2229 3a0a 2020 2020 2020 2020  2ind"):.        
-000090d0: 2222 2243 6f6e 7665 7274 7320 6769 7665  """Converts give
-000090e0: 6e20 6461 7461 2074 6f20 696e 6465 7865  n data to indexe
-000090f0: 7320 6f72 2074 6f20 7261 7720 6461 7461  s or to raw data
-00009100: 2028 6163 636f 7264 696e 6720 746f 2060   (according to `
-00009110: 606f 7264 6572 6060 292e 0a0a 2020 2020  `order``)...    
-00009120: 2020 2020 2049 7420 776f 726b 7320 666f       It works fo
-00009130: 7220 6060 5860 6020 636f 6e74 6169 6e69  r ``X`` containi
-00009140: 6e67 2074 7269 706c 6573 2c20 656e 7469  ng triples, enti
-00009150: 7469 6573 2c20 6f72 2072 656c 6174 696f  ties, or relatio
-00009160: 6e73 2e0a 0a20 2020 2020 2020 2050 6172  ns...        Par
-00009170: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00009180: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00009190: 2020 2058 3a20 6e70 2e61 7272 6179 206f     X: np.array o
-000091a0: 7220 6c69 7374 0a20 2020 2020 2020 2020  r list.         
-000091b0: 2020 2044 6174 6120 746f 2062 6520 696e     Data to be in
-000091c0: 6465 7865 642e 0a20 2020 2020 2020 2074  dexed..        t
-000091d0: 7970 655f 6f66 3a20 7374 720a 2020 2020  ype_of: str.    
-000091e0: 2020 2020 2020 2020 5370 6563 6966 6965          Specifie
-000091f0: 7320 7768 6574 6865 7220 746f 2067 6574  s whether to get
-00009200: 2069 6e64 6578 6573 2f72 6177 2064 6174   indexes/raw dat
-00009210: 6120 666f 7220 7472 6970 6c65 7320 2860  a for triples (`
-00009220: 6074 7970 655f 6f66 3d27 7427 6060 292c  `type_of='t'``),
-00009230: 2065 6e74 6974 6965 7320 2860 6074 7970   entities (``typ
-00009240: 655f 6f66 3d27 6527 6060 292c 0a20 2020  e_of='e'``),.   
-00009250: 2020 2020 2020 2020 206f 7220 7265 6c61           or rela
-00009260: 7469 6f6e 7320 2860 6074 7970 655f 6f66  tions (``type_of
-00009270: 3d27 7227 6060 292e 0a20 2020 2020 2020  ='r'``)..       
-00009280: 206f 7264 6572 3a20 7374 720a 2020 2020   order: str.    
-00009290: 2020 2020 2020 2020 5370 6563 6966 6965          Specifie
-000092a0: 7320 7768 6574 6865 7220 746f 2067 6574  s whether to get
-000092b0: 2069 6e64 6578 6573 2066 726f 6d20 7261   indexes from ra
-000092c0: 7720 6461 7461 2028 6060 6f72 6465 723d  w data (``order=
-000092d0: 2772 6177 3269 6e64 2760 6029 206f 720a  'raw2ind'``) or.
-000092e0: 2020 2020 2020 2020 2020 2020 7261 7720              raw 
-000092f0: 6461 7461 2066 726f 6d20 696e 6465 7865  data from indexe
-00009300: 7320 2860 606f 7264 6572 3d27 696e 6432  s (``order='ind2
-00009310: 7261 7727 6060 292e 0a0a 2020 2020 2020  raw'``)...      
-00009320: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-00009330: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00009340: 2020 593a 206e 702e 6172 7261 790a 2020    Y: np.array.  
-00009350: 2020 2020 2020 2020 2020 496e 6465 7865            Indexe
-00009360: 6420 6461 7461 206f 7220 7261 7720 6461  d data or raw da
-00009370: 7461 2e0a 0a20 2020 2020 2020 2045 7861  ta...        Exa
-00009380: 6d70 6c65 0a20 2020 2020 2020 202d 2d2d  mple.        ---
-00009390: 2d2d 2d2d 0a20 2020 2020 2020 203e 3e3e  ----.        >>>
-000093a0: 2066 726f 6d20 616d 706c 6967 7261 7068   from ampligraph
-000093b0: 2e6c 6174 656e 745f 6665 6174 7572 6573  .latent_features
-000093c0: 2069 6d70 6f72 7420 5363 6f72 696e 6742   import ScoringB
-000093d0: 6173 6564 456d 6265 6464 696e 674d 6f64  asedEmbeddingMod
-000093e0: 656c 0a20 2020 2020 2020 203e 3e3e 2066  el.        >>> f
-000093f0: 726f 6d20 616d 706c 6967 7261 7068 2e64  rom ampligraph.d
-00009400: 6174 6173 6574 7320 696d 706f 7274 206c  atasets import l
-00009410: 6f61 645f 6662 3135 6b5f 3233 370a 2020  oad_fb15k_237.  
-00009420: 2020 2020 2020 3e3e 3e20 5820 3d20 6c6f        >>> X = lo
-00009430: 6164 5f66 6231 356b 5f32 3337 2829 0a20  ad_fb15k_237(). 
-00009440: 2020 2020 2020 203e 3e3e 206d 6f64 656c         >>> model
-00009450: 203d 2053 636f 7269 6e67 4261 7365 6445   = ScoringBasedE
-00009460: 6d62 6564 6469 6e67 4d6f 6465 6c28 6574  mbeddingModel(et
-00009470: 613d 352c 0a20 2020 2020 2020 203e 3e3e  a=5,.        >>>
-00009480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094a0: 2020 2020 6b3d 3330 302c 0a20 2020 2020      k=300,.     
-000094b0: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
-000094c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094d0: 2020 2020 2020 2020 2020 7363 6f72 696e            scorin
-000094e0: 675f 7479 7065 3d27 436f 6d70 6c45 7827  g_type='ComplEx'
-000094f0: 2c0a 2020 2020 2020 2020 3e3e 3e20 2020  ,.        >>>   
-00009500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009520: 2073 6565 643d 3029 0a20 2020 2020 2020   seed=0).       
-00009530: 203e 3e3e 206d 6f64 656c 2e63 6f6d 7069   >>> model.compi
-00009540: 6c65 286f 7074 696d 697a 6572 3d27 6164  le(optimizer='ad
-00009550: 616d 272c 206c 6f73 733d 276e 6c6c 2729  am', loss='nll')
-00009560: 0a20 2020 2020 2020 203e 3e3e 206d 6f64  .        >>> mod
-00009570: 656c 2e66 6974 2858 5b27 7472 6169 6e27  el.fit(X['train'
-00009580: 5d2c 0a20 2020 2020 2020 203e 3e3e 2020  ],.        >>>  
-00009590: 2020 2020 2020 2020 2062 6174 6368 5f73           batch_s
-000095a0: 697a 653d 3130 3030 302c 0a20 2020 2020  ize=10000,.     
-000095b0: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
-000095c0: 2065 706f 6368 733d 352c 0a20 2020 2020   epochs=5,.     
-000095d0: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
-000095e0: 2076 6572 626f 7365 3d46 616c 7365 290a   verbose=False).
-000095f0: 2020 2020 2020 2020 3e3e 3e20 7072 696e          >>> prin
-00009600: 7428 6d6f 6465 6c2e 6765 745f 696e 6465  t(model.get_inde
-00009610: 7865 7328 5b27 2f6d 2f30 3237 726e 272c  xes(['/m/027rn',
-00009620: 2027 2f6d 2f30 3676 3873 3027 5d2c 2027   '/m/06v8s0'], '
-00009630: 6527 2c20 2772 6177 3269 6e64 2729 290a  e', 'raw2ind')).
-00009640: 2020 2020 2020 2020 3e3e 3e20 7072 696e          >>> prin
-00009650: 7428 6d6f 6465 6c2e 6765 745f 696e 6465  t(model.get_inde
-00009660: 7865 7328 5b33 3837 372c 2030 5d2c 2027  xes([3877, 0], '
-00009670: 6527 2c20 2769 6e64 3272 6177 2729 290a  e', 'ind2raw')).
-00009680: 2020 2020 2020 2020 5b30 2c20 3338 3737          [0, 3877
-00009690: 5d0a 2020 2020 2020 2020 5b27 2f6d 2f30  ].        ['/m/0
-000096a0: 3676 3873 3027 2c20 272f 6d2f 3032 3772  6v8s0', '/m/027r
-000096b0: 6e27 5d0a 2020 2020 2020 2020 2222 220a  n'].        """.
-000096c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000096d0: 656c 662e 6461 7461 5f69 6e64 6578 6572  elf.data_indexer
-000096e0: 2e67 6574 5f69 6e64 6578 6573 2858 2c20  .get_indexes(X, 
-000096f0: 7479 7065 5f6f 662c 206f 7264 6572 290a  type_of, order).
-00009700: 0a20 2020 2064 6566 2067 6574 5f63 6f75  .    def get_cou
-00009710: 6e74 2873 656c 662c 2063 6f6e 6365 7074  nt(self, concept
-00009720: 5f74 7970 653d 2265 2229 3a0a 2020 2020  _type="e"):.    
-00009730: 2020 2020 2222 2252 6574 7572 6e73 2074      """Returns t
-00009740: 6865 2063 6f75 6e74 206f 6620 656e 7469  he count of enti
-00009750: 7469 6573 2061 6e64 2072 656c 6174 696f  ties and relatio
-00009760: 6e73 2074 6861 7420 7765 7265 2070 7265  ns that were pre
-00009770: 7365 6e74 2064 7572 696e 6720 7472 6169  sent during trai
-00009780: 6e69 6e67 2e0a 0a20 2020 2020 2020 2050  ning...        P
-00009790: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-000097a0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-000097b0: 2020 2020 2063 6f6e 6365 7074 5f74 7970       concept_typ
-000097c0: 653a 2073 7472 0a20 2020 2020 2020 2020  e: str.         
-000097d0: 2020 2049 6e64 6963 6174 6573 2077 6865     Indicates whe
-000097e0: 7468 6572 2074 6f20 636f 756e 7420 656e  ther to count en
-000097f0: 7469 7469 6573 2028 6060 636f 6e63 6570  tities (``concep
-00009800: 745f 7479 7065 3d27 6527 6060 2920 6f72  t_type='e'``) or
-00009810: 0a20 2020 2020 2020 2020 2020 2072 656c  .            rel
-00009820: 6174 696f 6e73 2028 6060 636f 6e63 6570  ations (``concep
-00009830: 745f 7479 7065 3d27 7227 6060 2920 2864  t_type='r'``) (d
-00009840: 6566 6175 6c74 3a20 6027 6527 6029 2e0a  efault: `'e'`)..
-00009850: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00009860: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00009870: 0a20 2020 2020 2020 2063 6f75 6e74 3a20  .        count: 
-00009880: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00009890: 436f 756e 7420 6f66 2074 6865 2065 6e74  Count of the ent
-000098a0: 6974 6965 7320 6f72 2072 656c 6174 696f  ities or relatio
-000098b0: 6e73 2e0a 0a20 2020 2020 2020 2045 7861  ns...        Exa
-000098c0: 6d70 6c65 0a20 2020 2020 2020 202d 2d2d  mple.        ---
-000098d0: 2d2d 2d2d 0a20 2020 2020 2020 203e 3e3e  ----.        >>>
-000098e0: 2066 726f 6d20 616d 706c 6967 7261 7068   from ampligraph
-000098f0: 2e64 6174 6173 6574 7320 696d 706f 7274  .datasets import
-00009900: 206c 6f61 645f 6662 3135 6b5f 3233 370a   load_fb15k_237.
-00009910: 2020 2020 2020 2020 3e3e 3e20 6672 6f6d          >>> from
-00009920: 2061 6d70 6c69 6772 6170 682e 6c61 7465   ampligraph.late
-00009930: 6e74 5f66 6561 7475 7265 7320 696d 706f  nt_features impo
-00009940: 7274 2053 636f 7269 6e67 4261 7365 6445  rt ScoringBasedE
-00009950: 6d62 6564 6469 6e67 4d6f 6465 6c0a 2020  mbeddingModel.  
-00009960: 2020 2020 2020 3e3e 3e20 5820 3d20 6c6f        >>> X = lo
-00009970: 6164 5f66 6231 356b 5f32 3337 2829 0a20  ad_fb15k_237(). 
-00009980: 2020 2020 2020 203e 3e3e 206d 6f64 656c         >>> model
-00009990: 203d 2053 636f 7269 6e67 4261 7365 6445   = ScoringBasedE
-000099a0: 6d62 6564 6469 6e67 4d6f 6465 6c28 6574  mbeddingModel(et
-000099b0: 613d 352c 0a20 2020 2020 2020 203e 3e3e  a=5,.        >>>
-000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099e0: 2020 2020 6b3d 3330 302c 0a20 2020 2020      k=300,.     
-000099f0: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
-00009a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a10: 2020 2020 2020 2020 2020 7363 6f72 696e            scorin
-00009a20: 675f 7479 7065 3d27 436f 6d70 6c45 7827  g_type='ComplEx'
-00009a30: 2c0a 2020 2020 2020 2020 3e3e 3e20 2020  ,.        >>>   
-00009a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a60: 2073 6565 643d 3029 0a20 2020 2020 2020   seed=0).       
-00009a70: 203e 3e3e 206d 6f64 656c 2e63 6f6d 7069   >>> model.compi
-00009a80: 6c65 286f 7074 696d 697a 6572 3d27 6164  le(optimizer='ad
-00009a90: 616d 272c 206c 6f73 733d 276e 6c6c 2729  am', loss='nll')
-00009aa0: 0a20 2020 2020 2020 203e 3e3e 206d 6f64  .        >>> mod
-00009ab0: 656c 2e66 6974 2858 5b27 7472 6169 6e27  el.fit(X['train'
-00009ac0: 5d2c 0a20 2020 2020 2020 203e 3e3e 2020  ],.        >>>  
-00009ad0: 2020 2020 2020 2020 2062 6174 6368 5f73           batch_s
-00009ae0: 697a 653d 3130 3030 302c 0a20 2020 2020  ize=10000,.     
-00009af0: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
-00009b00: 2065 706f 6368 733d 352c 0a20 2020 2020   epochs=5,.     
-00009b10: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
-00009b20: 2076 6572 626f 7365 3d46 616c 7365 290a   verbose=False).
-00009b30: 2020 2020 2020 2020 3e3e 3e20 7072 696e          >>> prin
-00009b40: 7428 2745 6e74 6974 6965 733a 272c 206d  t('Entities:', m
-00009b50: 6f64 656c 2e67 6574 5f63 6f75 6e74 2827  odel.get_count('
-00009b60: 6527 2929 0a20 2020 2020 2020 203e 3e3e  e')).        >>>
-00009b70: 2070 7269 6e74 2827 5265 6c61 7469 6f6e   print('Relation
-00009b80: 733a 272c 206d 6f64 656c 2e67 6574 5f63  s:', model.get_c
-00009b90: 6f75 6e74 2827 7227 2929 0a20 2020 2020  ount('r')).     
-00009ba0: 2020 2045 6e74 6974 6965 733a 2031 3435     Entities: 145
-00009bb0: 3035 0a20 2020 2020 2020 2052 656c 6174  05.        Relat
-00009bc0: 696f 6e73 3a20 3233 370a 2020 2020 2020  ions: 237.      
-00009bd0: 2020 2222 220a 2020 2020 2020 2020 6173    """.        as
-00009be0: 7365 7274 2073 656c 662e 6973 5f66 6974  sert self.is_fit
-00009bf0: 7465 642c 2022 4d6f 6465 6c20 6973 206e  ted, "Model is n
-00009c00: 6f74 2066 6974 206f 6e20 7468 6520 6461  ot fit on the da
-00009c10: 7461 2079 6574 2122 0a20 2020 2020 2020  ta yet!".       
-00009c20: 2069 6620 636f 6e63 6570 745f 7479 7065   if concept_type
-00009c30: 203d 3d20 2265 223a 0a20 2020 2020 2020   == "e":.       
-00009c40: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00009c50: 2e64 6174 615f 696e 6465 7865 722e 6765  .data_indexer.ge
-00009c60: 745f 656e 7469 7469 6573 5f63 6f75 6e74  t_entities_count
-00009c70: 2829 0a20 2020 2020 2020 2065 6c69 6620  ().        elif 
-00009c80: 636f 6e63 6570 745f 7479 7065 203d 3d20  concept_type == 
-00009c90: 2272 223a 0a20 2020 2020 2020 2020 2020  "r":.           
-00009ca0: 2072 6574 7572 6e20 7365 6c66 2e64 6174   return self.dat
-00009cb0: 615f 696e 6465 7865 722e 6765 745f 7265  a_indexer.get_re
-00009cc0: 6c61 7469 6f6e 735f 636f 756e 7428 290a  lations_count().
-00009cd0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00009ce0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00009cf0: 5661 6c75 6545 7272 6f72 2822 496e 7661  ValueError("Inva
-00009d00: 6c69 6420 436f 6e63 6570 7420 5479 7065  lid Concept Type
-00009d10: 2028 6578 7065 6374 6564 2027 6527 206f   (expected 'e' o
-00009d20: 7220 2772 2729 2229 0a0a 2020 2020 6465  r 'r')")..    de
-00009d30: 6620 6765 745f 7472 6169 6e5f 656d 6265  f get_train_embe
-00009d40: 6464 696e 675f 6d61 7472 6978 5f73 697a  dding_matrix_siz
-00009d50: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00009d60: 2022 2222 5265 7475 726e 7320 7468 6520   """Returns the 
-00009d70: 7369 7a65 206f 6620 7468 6520 656d 6265  size of the embe
-00009d80: 6464 696e 6720 6d61 7472 6978 2075 7365  dding matrix use
-00009d90: 6420 666f 7220 7472 6169 6e69 6e67 2e0a  d for training..
-00009da0: 0a20 2020 2020 2020 2054 6869 7320 6d61  .        This ma
-00009db0: 7920 6e6f 7420 6265 2073 616d 6520 6173  y not be same as
-00009dc0: 2028 6e2c 206b 2920 6475 7269 6e67 2070   (n, k) during p
-00009dd0: 6172 7469 7469 6f6e 6564 2074 7261 696e  artitioned train
-00009de0: 696e 6720 2877 6865 7265 2060 6e60 2069  ing (where `n` i
-00009df0: 7320 7468 6520 6e75 6d62 6572 206f 6620  s the number of 
-00009e00: 7472 6970 6c65 7320 696e 2074 6865 0a20  triples in the. 
-00009e10: 2020 2020 2020 2077 686f 6c65 2074 7261         whole tra
-00009e20: 696e 696e 6720 7365 7429 2e0a 2020 2020  ining set)..    
-00009e30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00009e40: 6173 7365 7274 2073 656c 662e 6973 5f66  assert self.is_f
-00009e50: 6974 7465 642c 2022 4d6f 6465 6c20 6973  itted, "Model is
-00009e60: 206e 6f74 2066 6974 206f 6e20 7468 6520   not fit on the 
-00009e70: 6461 7461 2079 6574 2122 0a20 2020 2020  data yet!".     
-00009e80: 2020 2072 6574 7572 6e20 7b0a 2020 2020     return {.    
-00009e90: 2020 2020 2020 2020 2265 223a 2073 656c          "e": sel
-00009ea0: 662e 656e 636f 6469 6e67 5f6c 6179 6572  f.encoding_layer
-00009eb0: 2e65 6e74 5f65 6d62 2e73 6861 7065 2c0a  .ent_emb.shape,.
-00009ec0: 2020 2020 2020 2020 2020 2020 2272 223a              "r":
-00009ed0: 2073 656c 662e 656e 636f 6469 6e67 5f6c   self.encoding_l
-00009ee0: 6179 6572 2e72 656c 5f65 6d62 2e73 6861  ayer.rel_emb.sha
-00009ef0: 7065 2c0a 2020 2020 2020 2020 7d0a 0a20  pe,.        }.. 
-00009f00: 2020 2064 6566 2073 6176 6528 0a20 2020     def save(.   
-00009f10: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00009f20: 2020 2066 696c 6570 6174 682c 0a20 2020     filepath,.   
-00009f30: 2020 2020 206f 7665 7277 7269 7465 3d54       overwrite=T
-00009f40: 7275 652c 0a20 2020 2020 2020 2069 6e63  rue,.        inc
-00009f50: 6c75 6465 5f6f 7074 696d 697a 6572 3d54  lude_optimizer=T
-00009f60: 7275 652c 0a20 2020 2020 2020 2073 6176  rue,.        sav
-00009f70: 655f 666f 726d 6174 3d4e 6f6e 652c 0a20  e_format=None,. 
-00009f80: 2020 2020 2020 2073 6967 6e61 7475 7265         signature
-00009f90: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-00009fa0: 6f70 7469 6f6e 733d 4e6f 6e65 2c0a 2020  options=None,.  
-00009fb0: 2020 2020 2020 7361 7665 5f74 7261 6365        save_trace
-00009fc0: 733d 5472 7565 2c0a 2020 2020 293a 0a20  s=True,.    ):. 
-00009fd0: 2020 2020 2020 2022 2222 5361 7665 2074         """Save t
-00009fe0: 6865 206d 6f64 656c 2e22 2222 0a20 2020  he model.""".   
-00009ff0: 2020 2020 2073 7570 6572 2853 636f 7269       super(Scori
-0000a000: 6e67 4261 7365 6445 6d62 6564 6469 6e67  ngBasedEmbedding
-0000a010: 4d6f 6465 6c2c 2073 656c 6629 2e73 6176  Model, self).sav
-0000a020: 6528 0a20 2020 2020 2020 2020 2020 2066  e(.            f
-0000a030: 696c 6570 6174 682c 0a20 2020 2020 2020  ilepath,.       
-0000a040: 2020 2020 206f 7665 7277 7269 7465 2c0a       overwrite,.
-0000a050: 2020 2020 2020 2020 2020 2020 696e 636c              incl
-0000a060: 7564 655f 6f70 7469 6d69 7a65 722c 0a20  ude_optimizer,. 
-0000a070: 2020 2020 2020 2020 2020 2073 6176 655f             save_
-0000a080: 666f 726d 6174 2c0a 2020 2020 2020 2020  format,.        
-0000a090: 2020 2020 7369 676e 6174 7572 6573 2c0a      signatures,.
-0000a0a0: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
-0000a0b0: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
-0000a0c0: 2073 6176 655f 7472 6163 6573 2c0a 2020   save_traces,.  
-0000a0d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000a0e0: 7365 6c66 2e73 6176 655f 6d65 7461 6461  self.save_metada
-0000a0f0: 7461 2866 696c 6564 6972 3d66 696c 6570  ta(filedir=filep
-0000a100: 6174 6829 0a0a 2020 2020 6465 6620 7361  ath)..    def sa
-0000a110: 7665 5f6d 6574 6164 6174 6128 7365 6c66  ve_metadata(self
-0000a120: 2c20 6669 6c65 7061 7468 3d4e 6f6e 652c  , filepath=None,
-0000a130: 2066 696c 6564 6972 3d4e 6f6e 6529 3a0a   filedir=None):.
-0000a140: 2020 2020 2020 2020 2222 2253 6176 6520          """Save 
-0000a150: 6d65 7461 6461 7461 2e22 2222 0a20 2020  metadata.""".   
-0000a160: 2020 2020 2023 2073 746f 7265 2061 6d70       # store amp
-0000a170: 6c69 6772 6170 6820 7370 6563 6966 6963  ligraph specific
-0000a180: 206d 6574 6164 6174 610a 2020 2020 2020   metadata.      
-0000a190: 2020 6966 2066 696c 6570 6174 6820 6973    if filepath is
-0000a1a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000a1b0: 2020 2020 2020 2062 6173 655f 6469 7220         base_dir 
-0000a1c0: 3d20 6f73 2e70 6174 682e 6469 726e 616d  = os.path.dirnam
-0000a1d0: 6528 6669 6c65 6469 7229 0a20 2020 2020  e(filedir).     
-0000a1e0: 2020 2020 2020 2062 6173 655f 6469 7220         base_dir 
-0000a1f0: 3d20 222e 2220 6966 2062 6173 655f 6469  = "." if base_di
-0000a200: 7220 3d3d 2022 2220 656c 7365 2062 6173  r == "" else bas
-0000a210: 655f 6469 720a 2020 2020 2020 2020 2020  e_dir.          
-0000a220: 2020 6669 6c65 7061 7468 203d 206f 732e    filepath = os.
-0000a230: 7061 7468 2e62 6173 656e 616d 6528 6669  path.basename(fi
-0000a240: 6c65 7061 7468 290a 0a20 2020 2020 2020  lepath)..       
-0000a250: 2069 6620 6669 6c65 6469 7220 6973 206e   if filedir is n
-0000a260: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000a270: 2020 2020 2062 6173 655f 6469 7220 3d20       base_dir = 
-0000a280: 6669 6c65 6469 720a 2020 2020 2020 2020  filedir.        
-0000a290: 2020 2020 6669 6c65 7061 7468 203d 206f      filepath = o
-0000a2a0: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
-0000a2b0: 6669 6c65 6469 7229 0a0a 2020 2020 2020  filedir)..      
-0000a2c0: 2020 7769 7468 206f 7065 6e28 0a20 2020    with open(.   
-0000a2d0: 2020 2020 2020 2020 206f 732e 7061 7468           os.path
-0000a2e0: 2e6a 6f69 6e28 6261 7365 5f64 6972 2c20  .join(base_dir, 
-0000a2f0: 6669 6c65 7061 7468 202b 2022 5f6d 6574  filepath + "_met
-0000a300: 6164 6174 612e 616d 706b 6c22 292c 2022  adata.ampkl"), "
-0000a310: 7762 220a 2020 2020 2020 2020 2920 6173  wb".        ) as
-0000a320: 2066 3a0a 2020 2020 2020 2020 2020 2020   f:.            
-0000a330: 6d65 7461 6461 7461 203d 207b 0a20 2020  metadata = {.   
-0000a340: 2020 2020 2020 2020 2020 2020 2022 6973               "is
-0000a350: 5f70 6172 7469 7469 6f6e 6564 5f74 7261  _partitioned_tra
-0000a360: 696e 696e 6722 3a20 7365 6c66 2e69 735f  ining": self.is_
-0000a370: 7061 7274 6974 696f 6e65 645f 7472 6169  partitioned_trai
-0000a380: 6e69 6e67 2c0a 2020 2020 2020 2020 2020  ning,.          
-0000a390: 2020 2020 2020 226d 6178 5f65 6e74 5f73        "max_ent_s
-0000a3a0: 697a 6522 3a20 7365 6c66 2e6d 6178 5f65  ize": self.max_e
-0000a3b0: 6e74 5f73 697a 652c 0a20 2020 2020 2020  nt_size,.       
-0000a3c0: 2020 2020 2020 2020 2022 6d61 785f 7265           "max_re
-0000a3d0: 6c5f 7369 7a65 223a 2073 656c 662e 6d61  l_size": self.ma
-0000a3e0: 785f 7265 6c5f 7369 7a65 2c0a 2020 2020  x_rel_size,.    
-0000a3f0: 2020 2020 2020 2020 2020 2020 2265 7461              "eta
-0000a400: 223a 2073 656c 662e 6574 612c 0a20 2020  ": self.eta,.   
-0000a410: 2020 2020 2020 2020 2020 2020 2022 6b22               "k"
-0000a420: 3a20 7365 6c66 2e6b 2c0a 2020 2020 2020  : self.k,.      
-0000a430: 2020 2020 2020 2020 2020 2269 735f 6669            "is_fi
-0000a440: 7474 6564 223a 2073 656c 662e 6973 5f66  tted": self.is_f
-0000a450: 6974 7465 642c 0a20 2020 2020 2020 2020  itted,.         
-0000a460: 2020 2020 2020 2022 6973 5f63 616c 6962         "is_calib
-0000a470: 7261 7465 6422 3a20 7365 6c66 2e69 735f  rated": self.is_
-0000a480: 6361 6c69 6272 6174 6564 2c0a 2020 2020  calibrated,.    
-0000a490: 2020 2020 2020 2020 2020 2020 2269 735f              "is_
-0000a4a0: 6261 636b 7761 7264 223a 2073 656c 662e  backward": self.
-0000a4b0: 6973 5f62 6163 6b77 6172 642c 0a20 2020  is_backward,.   
-0000a4c0: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
-0000a4d0: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-0000a4e0: 2e75 7064 6174 6528 7365 6c66 2e64 6174  .update(self.dat
-0000a4f0: 615f 696e 6465 7865 722e 6765 745f 7570  a_indexer.get_up
-0000a500: 6461 7465 5f6d 6574 6164 6174 6128 6261  date_metadata(ba
-0000a510: 7365 5f64 6972 2929 0a20 2020 2020 2020  se_dir)).       
-0000a520: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
-0000a530: 7061 7274 6974 696f 6e65 645f 7472 6169  partitioned_trai
-0000a540: 6e69 6e67 3a0a 2020 2020 2020 2020 2020  ning:.          
-0000a550: 2020 2020 2020 7365 6c66 2e70 6172 7469        self.parti
-0000a560: 7469 6f6e 6572 5f6d 6574 6164 6174 6120  tioner_metadata 
-0000a570: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0000a580: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
-0000a590: 615f 6861 6e64 6c65 722e 6765 745f 7570  a_handler.get_up
-0000a5a0: 6461 7465 5f70 6172 7469 7469 6f6e 6572  date_partitioner
-0000a5b0: 5f6d 6574 6164 6174 6128 6261 7365 5f64  _metadata(base_d
-0000a5c0: 6972 290a 2020 2020 2020 2020 2020 2020  ir).            
-0000a5d0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000a5e0: 2020 2020 2020 6d65 7461 6461 7461 2e75        metadata.u
-0000a5f0: 7064 6174 6528 7365 6c66 2e70 6172 7469  pdate(self.parti
-0000a600: 7469 6f6e 6572 5f6d 6574 6164 6174 6129  tioner_metadata)
-0000a610: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000a620: 2073 656c 662e 6973 5f63 616c 6962 7261   self.is_calibra
-0000a630: 7465 643a 0a20 2020 2020 2020 2020 2020  ted:.           
-0000a640: 2020 2020 206d 6574 6164 6174 615b 2263       metadata["c
-0000a650: 616c 6962 5f77 225d 203d 2073 656c 662e  alib_w"] = self.
-0000a660: 6361 6c69 6272 6174 696f 6e5f 6c61 7965  calibration_laye
-0000a670: 722e 6361 6c69 625f 772e 6e75 6d70 7928  r.calib_w.numpy(
-0000a680: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000a690: 2020 6d65 7461 6461 7461 5b22 6361 6c69    metadata["cali
-0000a6a0: 625f 6222 5d20 3d20 7365 6c66 2e63 616c  b_b"] = self.cal
-0000a6b0: 6962 7261 7469 6f6e 5f6c 6179 6572 2e63  ibration_layer.c
-0000a6c0: 616c 6962 5f62 2e6e 756d 7079 2829 0a20  alib_b.numpy(). 
-0000a6d0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000a6e0: 6574 6164 6174 615b 2270 6f73 5f73 697a  etadata["pos_siz
-0000a6f0: 6522 5d20 3d20 7365 6c66 2e63 616c 6962  e"] = self.calib
-0000a700: 7261 7469 6f6e 5f6c 6179 6572 2e70 6f73  ration_layer.pos
-0000a710: 5f73 697a 650a 2020 2020 2020 2020 2020  _size.          
-0000a720: 2020 2020 2020 6d65 7461 6461 7461 5b22        metadata["
-0000a730: 6e65 675f 7369 7a65 225d 203d 2073 656c  neg_size"] = sel
-0000a740: 662e 6361 6c69 6272 6174 696f 6e5f 6c61  f.calibration_la
-0000a750: 7965 722e 6e65 675f 7369 7a65 0a20 2020  yer.neg_size.   
-0000a760: 2020 2020 2020 2020 2020 2020 206d 6574               met
-0000a770: 6164 6174 615b 0a20 2020 2020 2020 2020  adata[.         
-0000a780: 2020 2020 2020 2020 2020 2022 706f 7369             "posi
-0000a790: 7469 7665 5f62 6173 655f 7261 7465 220a  tive_base_rate".
-0000a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7b0: 5d20 3d20 7365 6c66 2e63 616c 6962 7261  ] = self.calibra
-0000a7c0: 7469 6f6e 5f6c 6179 6572 2e70 6f73 6974  tion_layer.posit
-0000a7d0: 6976 655f 6261 7365 5f72 6174 650a 2020  ive_base_rate.  
-0000a7e0: 2020 2020 2020 2020 2020 7069 636b 6c65            pickle
-0000a7f0: 2e64 756d 7028 6d65 7461 6461 7461 2c20  .dump(metadata, 
-0000a800: 6629 0a0a 2020 2020 6465 6620 7361 7665  f)..    def save
-0000a810: 5f77 6569 6768 7473 2873 656c 662c 2066  _weights(self, f
-0000a820: 696c 6570 6174 682c 206f 7665 7277 7269  ilepath, overwri
-0000a830: 7465 3d54 7275 6529 3a0a 2020 2020 2020  te=True):.      
-0000a840: 2020 2222 2253 6176 6520 7468 6520 7472    """Save the tr
-0000a850: 6169 6e61 626c 6520 7765 6967 6874 732e  ainable weights.
-0000a860: 0a0a 2020 2020 2020 2020 2055 7365 2074  ..         Use t
-0000a870: 6869 7320 6675 6e63 7469 6f6e 2069 6620  his function if 
-0000a880: 7468 6520 7472 6169 6e69 6e67 2070 726f  the training pro
-0000a890: 6365 7373 2069 7320 636f 6d70 6c65 7465  cess is complete
-0000a8a0: 2061 6e64 2079 6f75 2077 616e 7420 746f   and you want to
-0000a8b0: 0a20 2020 2020 2020 2020 7573 6520 7468  .         use th
-0000a8c0: 6520 6d6f 6465 6c20 6f6e 6c79 2066 6f72  e model only for
-0000a8d0: 2069 6e66 6572 656e 6365 2e20 5573 6520   inference. Use 
-0000a8e0: 3a6d 6574 683a 606c 6f61 645f 7765 6967  :meth:`load_weig
-0000a8f0: 6874 7360 2074 6f20 6c6f 6164 2074 6865  hts` to load the
-0000a900: 206d 6f64 656c 2077 6569 6768 7473 2062   model weights b
-0000a910: 6163 6b2e 0a0a 2020 2020 2020 2020 202e  ack...         .
-0000a920: 2e20 4e6f 7465 203a 3a0a 2020 2020 2020  . Note ::.      
-0000a930: 2020 2020 2020 2049 6620 796f 7520 7761         If you wa
-0000a940: 6e74 2074 6f20 6265 2061 626c 6520 6f66  nt to be able of
-0000a950: 2063 6f6e 7469 6e75 696e 6720 7468 6520   continuing the 
-0000a960: 7472 6169 6e69 6e67 2c20 796f 7520 6361  training, you ca
-0000a970: 6e20 7573 6520 7468 6520 3a6d 6574 683a  n use the :meth:
-0000a980: 6061 6d70 6c69 6772 6170 682e 7574 696c  `ampligraph.util
-0000a990: 732e 7361 7665 5f6d 6f64 656c 600a 2020  s.save_model`.  
-0000a9a0: 2020 2020 2020 2020 2020 2061 6e64 203a             and :
-0000a9b0: 6d65 7468 3a60 616d 706c 6967 7261 7068  meth:`ampligraph
-0000a9c0: 2e75 7469 6c73 2e72 6573 746f 7265 5f6d  .utils.restore_m
-0000a9d0: 6f64 656c 602e 5468 6573 6520 6675 6e63  odel`.These func
-0000a9e0: 7469 6f6e 7320 7361 7665 2061 6e64 2072  tions save and r
-0000a9f0: 6573 746f 7265 2074 6865 2065 6e74 6972  estore the entir
-0000aa00: 6520 7374 6174 650a 2020 2020 2020 2020  e state.        
-0000aa10: 2020 2020 206f 6620 7468 6520 6772 6170       of the grap
-0000aa20: 682c 2077 6869 6368 2061 6c6c 6f77 7320  h, which allows 
-0000aa30: 746f 2063 6f6e 7469 6e75 6520 7468 6520  to continue the 
-0000aa40: 7472 6169 6e69 6e67 2066 726f 6d20 7768  training from wh
-0000aa50: 6572 6520 6974 2077 6173 2073 746f 7070  ere it was stopp
-0000aa60: 6564 2e0a 0a20 2020 2020 2020 2050 6172  ed...        Par
-0000aa70: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-0000aa80: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-0000aa90: 2020 2066 696c 6570 6174 683a 2073 7472     filepath: str
-0000aaa0: 0a20 2020 2020 2020 2020 2020 2050 6174  .            Pat
-0000aab0: 6820 746f 2073 6176 6520 7468 6520 6d6f  h to save the mo
-0000aac0: 6465 6c2e 0a20 2020 2020 2020 206f 7665  del..        ove
-0000aad0: 7277 7269 7465 3a20 626f 6f6c 0a20 2020  rwrite: bool.   
-0000aae0: 2020 2020 2020 2020 2046 6c61 6720 7768           Flag wh
-0000aaf0: 6963 6820 696e 6469 6361 7465 7320 7768  ich indicates wh
-0000ab00: 6574 6865 7220 7468 6520 6d6f 6465 6c2c  ether the model,
-0000ab10: 2069 6620 7072 6573 656e 742c 206e 6565   if present, nee
-0000ab20: 6473 2074 6f20 6265 206f 7665 7277 7269  ds to be overwri
-0000ab30: 7474 656e 206f 7220 6e6f 7420 2864 6566  tten or not (def
-0000ab40: 6175 6c74 3a20 6054 7275 6560 292e 0a20  ault: `True`).. 
-0000ab50: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000ab60: 2020 2023 2054 4f44 4f3a 2076 6572 6966     # TODO: verif
-0000ab70: 7920 6f74 6865 7220 666f 726d 6174 730a  y other formats.
-0000ab80: 0a20 2020 2020 2020 2023 2063 616c 6c20  .        # call 
-0000ab90: 7468 6520 6261 7365 2063 6c61 7373 206d  the base class m
-0000aba0: 6574 686f 6420 746f 2073 6176 6520 7468  ethod to save th
-0000abb0: 6520 7765 6967 6874 730a 2020 2020 2020  e weights.      
-0000abc0: 2020 6966 206e 6f74 2073 656c 662e 6973    if not self.is
-0000abd0: 5f70 6172 7469 7469 6f6e 6564 5f74 7261  _partitioned_tra
-0000abe0: 696e 696e 673a 0a20 2020 2020 2020 2020  ining:.         
-0000abf0: 2020 2073 7570 6572 2853 636f 7269 6e67     super(Scoring
-0000ac00: 4261 7365 6445 6d62 6564 6469 6e67 4d6f  BasedEmbeddingMo
-0000ac10: 6465 6c2c 2073 656c 6629 2e73 6176 655f  del, self).save_
-0000ac20: 7765 6967 6874 7328 0a20 2020 2020 2020  weights(.       
-0000ac30: 2020 2020 2020 2020 2066 696c 6570 6174           filepat
-0000ac40: 682c 206f 7665 7277 7269 7465 0a20 2020  h, overwrite.   
-0000ac50: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000ac60: 2020 2073 656c 662e 7361 7665 5f6d 6574     self.save_met
-0000ac70: 6164 6174 6128 6669 6c65 7061 7468 290a  adata(filepath).
-0000ac80: 0a20 2020 2064 6566 2062 7569 6c64 5f66  .    def build_f
-0000ac90: 756c 6c5f 6d6f 6465 6c28 7365 6c66 2c20  ull_model(self, 
-0000aca0: 6261 7463 685f 7369 7a65 3d31 3030 293a  batch_size=100):
-0000acb0: 0a20 2020 2020 2020 2022 2222 5468 6973  .        """This
-0000acc0: 206d 6574 686f 6420 6973 2063 616c 6c65   method is calle
-0000acd0: 6420 7768 696c 6520 6c6f 6164 696e 6720  d while loading 
-0000ace0: 7468 6520 7765 6967 6874 7320 746f 2062  the weights to b
-0000acf0: 7569 6c64 2074 6865 206d 6f64 656c 2e22  uild the model."
-0000ad00: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-0000ad10: 6275 696c 6428 2862 6174 6368 5f73 697a  build((batch_siz
-0000ad20: 652c 2033 2929 0a20 2020 2020 2020 2066  e, 3)).        f
-0000ad30: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-0000ad40: 6e28 7365 6c66 2e6c 6179 6572 7329 293a  n(self.layers)):
-0000ad50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000ad60: 662e 6c61 7965 7273 5b69 5d2e 6275 696c  f.layers[i].buil
-0000ad70: 6428 2862 6174 6368 5f73 697a 652c 2033  d((batch_size, 3
-0000ad80: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
-0000ad90: 656c 662e 6c61 7965 7273 5b69 5d2e 6275  elf.layers[i].bu
-0000ada0: 696c 7420 3d20 5472 7565 0a0a 2020 2020  ilt = True..    
-0000adb0: 6465 6620 6c6f 6164 5f6d 6574 6164 6174  def load_metadat
-0000adc0: 6128 7365 6c66 2c20 6669 6c65 7061 7468  a(self, filepath
-0000add0: 3d4e 6f6e 652c 2066 696c 6564 6972 3d4e  =None, filedir=N
-0000ade0: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
-0000adf0: 2066 696c 6564 6972 2069 7320 6e6f 7420   filedir is not 
-0000ae00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000ae10: 2020 6669 6c65 7061 7468 203d 206f 732e    filepath = os.
-0000ae20: 7061 7468 2e6a 6f69 6e28 6669 6c65 6469  path.join(filedi
-0000ae30: 722c 206f 732e 7061 7468 2e62 6173 656e  r, os.path.basen
-0000ae40: 616d 6528 6669 6c65 6469 7229 290a 0a20  ame(filedir)).. 
-0000ae50: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-0000ae60: 2866 696c 6570 6174 6820 2b20 225f 6d65  (filepath + "_me
-0000ae70: 7461 6461 7461 2e61 6d70 6b6c 222c 2022  tadata.ampkl", "
-0000ae80: 7262 2229 2061 7320 663a 0a20 2020 2020  rb") as f:.     
-0000ae90: 2020 2020 2020 206d 6574 6164 6174 6120         metadata 
-0000aea0: 3d20 7069 636b 6c65 2e6c 6f61 6428 6629  = pickle.load(f)
-0000aeb0: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
-0000aec0: 6164 6174 615b 2272 6f6f 745f 6469 7265  adata["root_dire
-0000aed0: 6374 6f72 7922 5d20 3d20 6f73 2e70 6174  ctory"] = os.pat
-0000aee0: 682e 6469 726e 616d 6528 6669 6c65 7061  h.dirname(filepa
-0000aef0: 7468 290a 2020 2020 2020 2020 2020 2020  th).            
-0000af00: 6d65 7461 6461 7461 5b22 726f 6f74 5f64  metadata["root_d
-0000af10: 6972 6563 746f 7279 225d 203d 2028 0a20  irectory"] = (. 
-0000af20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000af30: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
-0000af40: 2020 2069 6620 6d65 7461 6461 7461 5b22     if metadata["
-0000af50: 726f 6f74 5f64 6972 6563 746f 7279 225d  root_directory"]
-0000af60: 203d 3d20 2222 0a20 2020 2020 2020 2020   == "".         
-0000af70: 2020 2020 2020 2065 6c73 6520 6d65 7461         else meta
-0000af80: 6461 7461 5b22 726f 6f74 5f64 6972 6563  data["root_direc
-0000af90: 746f 7279 225d 0a20 2020 2020 2020 2020  tory"].         
-0000afa0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000afb0: 2073 656c 662e 6261 7365 5f64 6972 203d   self.base_dir =
-0000afc0: 206d 6574 6164 6174 615b 2272 6f6f 745f   metadata["root_
-0000afd0: 6469 7265 6374 6f72 7922 5d0a 2020 2020  directory"].    
-0000afe0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000aff0: 2020 2020 2020 2020 2020 2020 206d 6574               met
-0000b000: 6164 6174 615b 2264 625f 6669 6c65 225d  adata["db_file"]
-0000b010: 203d 206f 732e 7061 7468 2e62 6173 656e   = os.path.basen
-0000b020: 616d 6528 6d65 7461 6461 7461 5b22 6462  ame(metadata["db
-0000b030: 5f66 696c 6522 5d29 0a20 2020 2020 2020  _file"]).       
-0000b040: 2020 2020 2065 7863 6570 7420 4b65 7945       except KeyE
-0000b050: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
-0000b060: 2020 2020 2020 7072 696e 7428 2253 6176        print("Sav
-0000b070: 6564 206d 6f64 656c 2064 6f65 7320 6e6f  ed model does no
-0000b080: 7420 696e 636c 7564 6520 6120 6462 2066  t include a db f
-0000b090: 696c 652e 2053 6b69 7070 696e 672e 2229  ile. Skipping.")
-0000b0a0: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000b0b0: 6c66 2e64 6174 615f 696e 6465 7865 7220  lf.data_indexer 
-0000b0c0: 3d20 4461 7461 496e 6465 7865 7228 5b5d  = DataIndexer([]
-0000b0d0: 2c20 2a2a 6d65 7461 6461 7461 290a 2020  , **metadata).  
-0000b0e0: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
-0000b0f0: 735f 7061 7274 6974 696f 6e65 645f 7472  s_partitioned_tr
-0000b100: 6169 6e69 6e67 203d 206d 6574 6164 6174  aining = metadat
-0000b110: 615b 2269 735f 7061 7274 6974 696f 6e65  a["is_partitione
-0000b120: 645f 7472 6169 6e69 6e67 225d 0a20 2020  d_training"].   
-0000b130: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-0000b140: 785f 656e 745f 7369 7a65 203d 206d 6574  x_ent_size = met
-0000b150: 6164 6174 615b 226d 6178 5f65 6e74 5f73  adata["max_ent_s
-0000b160: 697a 6522 5d0a 2020 2020 2020 2020 2020  ize"].          
-0000b170: 2020 7365 6c66 2e6d 6178 5f72 656c 5f73    self.max_rel_s
-0000b180: 697a 6520 3d20 6d65 7461 6461 7461 5b22  ize = metadata["
-0000b190: 6d61 785f 7265 6c5f 7369 7a65 225d 0a20  max_rel_size"]. 
-0000b1a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b1b0: 6973 5f66 6974 7465 6420 3d20 6d65 7461  is_fitted = meta
-0000b1c0: 6461 7461 5b22 6973 5f66 6974 7465 6422  data["is_fitted"
-0000b1d0: 5d0a 2020 2020 2020 2020 2020 2020 7365  ].            se
-0000b1e0: 6c66 2e69 735f 6261 636b 7761 7264 203d  lf.is_backward =
-0000b1f0: 206d 6574 6164 6174 612e 6765 7428 2269   metadata.get("i
-0000b200: 735f 6261 636b 7761 7264 222c 2046 616c  s_backward", Fal
-0000b210: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
-0000b220: 6966 2073 656c 662e 6973 5f70 6172 7469  if self.is_parti
-0000b230: 7469 6f6e 6564 5f74 7261 696e 696e 673a  tioned_training:
-0000b240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b250: 2073 656c 662e 7061 7274 6974 696f 6e65   self.partitione
-0000b260: 725f 6b20 3d20 6d65 7461 6461 7461 5b22  r_k = metadata["
-0000b270: 7061 7274 6974 696f 6e65 725f 6b22 5d0a  partitioner_k"].
-0000b280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b290: 7365 6c66 2e70 6172 7469 7469 6f6e 6572  self.partitioner
-0000b2a0: 5f6d 6574 6164 6174 6120 3d20 7b7d 0a20  _metadata = {}. 
-0000b2b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000b2c0: 656c 662e 7061 7274 6974 696f 6e65 725f  elf.partitioner_
-0000b2d0: 6d65 7461 6461 7461 5b22 656e 745f 6d61  metadata["ent_ma
-0000b2e0: 705f 666e 616d 6522 5d20 3d20 6d65 7461  p_fname"] = meta
-0000b2f0: 6461 7461 5b0a 2020 2020 2020 2020 2020  data[.          
-0000b300: 2020 2020 2020 2020 2020 2265 6e74 5f6d            "ent_m
-0000b310: 6170 5f66 6e61 6d65 220a 2020 2020 2020  ap_fname".      
-0000b320: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-0000b330: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b340: 2e70 6172 7469 7469 6f6e 6572 5f6d 6574  .partitioner_met
-0000b350: 6164 6174 615b 2272 656c 5f6d 6170 5f66  adata["rel_map_f
-0000b360: 6e61 6d65 225d 203d 206d 6574 6164 6174  name"] = metadat
-0000b370: 615b 0a20 2020 2020 2020 2020 2020 2020  a[.             
-0000b380: 2020 2020 2020 2022 7265 6c5f 6d61 705f         "rel_map_
-0000b390: 666e 616d 6522 0a20 2020 2020 2020 2020  fname".         
-0000b3a0: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
-0000b3b0: 2020 2020 2020 7365 6c66 2e69 735f 6361        self.is_ca
-0000b3c0: 6c69 6272 6174 6564 203d 206d 6574 6164  librated = metad
-0000b3d0: 6174 615b 2269 735f 6361 6c69 6272 6174  ata["is_calibrat
-0000b3e0: 6564 225d 0a20 2020 2020 2020 2020 2020  ed"].           
-0000b3f0: 2069 6620 7365 6c66 2e69 735f 6361 6c69   if self.is_cali
-0000b400: 6272 6174 6564 3a0a 2020 2020 2020 2020  brated:.        
-0000b410: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
-0000b420: 6962 7261 7469 6f6e 5f6c 6179 6572 203d  ibration_layer =
-0000b430: 2043 616c 6962 7261 7469 6f6e 4c61 7965   CalibrationLaye
-0000b440: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-0000b450: 2020 2020 2020 206d 6574 6164 6174 615b         metadata[
-0000b460: 2270 6f73 5f73 697a 6522 5d2c 0a20 2020  "pos_size"],.   
-0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b480: 206d 6574 6164 6174 615b 226e 6567 5f73   metadata["neg_s
-0000b490: 697a 6522 5d2c 0a20 2020 2020 2020 2020  ize"],.         
-0000b4a0: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-0000b4b0: 6174 615b 2270 6f73 6974 6976 655f 6261  ata["positive_ba
-0000b4c0: 7365 5f72 6174 6522 5d2c 0a20 2020 2020  se_rate"],.     
-0000b4d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000b4e0: 616c 6962 5f77 3d6d 6574 6164 6174 615b  alib_w=metadata[
-0000b4f0: 2263 616c 6962 5f77 225d 2c0a 2020 2020  "calib_w"],.    
-0000b500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b510: 6361 6c69 625f 623d 6d65 7461 6461 7461  calib_b=metadata
-0000b520: 5b22 6361 6c69 625f 6222 5d2c 0a20 2020  ["calib_b"],.   
-0000b530: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-0000b540: 2020 2020 6465 6620 6c6f 6164 5f77 6569      def load_wei
-0000b550: 6768 7473 2873 656c 662c 2066 696c 6570  ghts(self, filep
-0000b560: 6174 6829 3a0a 2020 2020 2020 2020 2222  ath):.        ""
-0000b570: 224c 6f61 6473 2074 6865 206d 6f64 656c  "Loads the model
-0000b580: 2077 6569 6768 7473 2e0a 0a20 2020 2020   weights...     
-0000b590: 2020 2020 5573 6520 7468 6973 2066 756e      Use this fun
-0000b5a0: 6374 696f 6e20 6966 2060 6073 6176 655f  ction if ``save_
-0000b5b0: 7765 6967 6874 7360 6020 7761 7320 7573  weights`` was us
-0000b5c0: 6564 2074 6f20 7361 7665 2074 6865 206d  ed to save the m
-0000b5d0: 6f64 656c 2e0a 0a20 2020 2020 2020 2020  odel...         
-0000b5e0: 2e2e 204e 6f74 6520 3a3a 0a20 2020 2020  .. Note ::.     
-0000b5f0: 2020 2020 2020 2020 4966 2079 6f75 2077          If you w
-0000b600: 616e 7420 746f 2063 6f6e 7469 6e75 6520  ant to continue 
-0000b610: 7472 6169 6e69 6e67 2c20 796f 7520 6361  training, you ca
-0000b620: 6e20 7573 6520 7468 6520 3a6d 6574 683a  n use the :meth:
-0000b630: 6061 6d70 6c69 6772 6170 682e 7574 696c  `ampligraph.util
-0000b640: 732e 7361 7665 5f6d 6f64 656c 6020 616e  s.save_model` an
-0000b650: 640a 2020 2020 2020 2020 2020 2020 203a  d.             :
-0000b660: 6d65 7468 3a60 616d 706c 6967 7261 7068  meth:`ampligraph
-0000b670: 2e75 7469 6c73 2e6c 6f61 645f 6d6f 6465  .utils.load_mode
-0000b680: 6c60 2e20 5468 6573 6520 6675 6e63 7469  l`. These functi
-0000b690: 6f6e 7320 7361 7665 2074 6865 2065 6e74  ons save the ent
-0000b6a0: 6972 6520 7374 6174 6520 6f66 2074 6865  ire state of the
-0000b6b0: 2067 7261 7068 0a20 2020 2020 2020 2020   graph.         
-0000b6c0: 2020 2020 7768 6963 6820 616c 6c6f 7773      which allows
-0000b6d0: 2074 6f20 636f 6e74 696e 7565 2074 6865   to continue the
-0000b6e0: 2074 7261 696e 696e 6720 6672 6f6d 2077   training from w
-0000b6f0: 6865 7265 2069 7420 7374 6f70 7065 642e  here it stopped.
-0000b700: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0000b710: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-0000b720: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000b730: 6669 6c65 7061 7468 3a20 7374 720a 2020  filepath: str.  
-0000b740: 2020 2020 2020 2020 2020 5061 7468 2074            Path t
-0000b750: 6f20 7361 7665 2074 6865 206d 6f64 656c  o save the model
-0000b760: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000b770: 2020 2020 2020 7365 6c66 2e6c 6f61 645f        self.load_
-0000b780: 6d65 7461 6461 7461 2866 696c 6570 6174  metadata(filepat
-0000b790: 6829 0a20 2020 2020 2020 2073 656c 662e  h).        self.
-0000b7a0: 6275 696c 645f 6675 6c6c 5f6d 6f64 656c  build_full_model
-0000b7b0: 2829 0a20 2020 2020 2020 2069 6620 6e6f  ().        if no
-0000b7c0: 7420 7365 6c66 2e69 735f 7061 7274 6974  t self.is_partit
-0000b7d0: 696f 6e65 645f 7472 6169 6e69 6e67 3a0a  ioned_training:.
-0000b7e0: 2020 2020 2020 2020 2020 2020 7375 7065              supe
-0000b7f0: 7228 5363 6f72 696e 6742 6173 6564 456d  r(ScoringBasedEm
-0000b800: 6265 6464 696e 674d 6f64 656c 2c20 7365  beddingModel, se
-0000b810: 6c66 292e 6c6f 6164 5f77 6569 6768 7473  lf).load_weights
-0000b820: 2866 696c 6570 6174 6829 0a0a 2020 2020  (filepath)..    
-0000b830: 6465 6620 636f 6d70 696c 6528 0a20 2020  def compile(.   
-0000b840: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000b850: 2020 206f 7074 696d 697a 6572 3d22 6164     optimizer="ad
-0000b860: 616d 222c 0a20 2020 2020 2020 206c 6f73  am",.        los
-0000b870: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-0000b880: 656e 7469 7479 5f72 656c 6174 696f 6e5f  entity_relation_
-0000b890: 696e 6974 6961 6c69 7a65 723d 2267 6c6f  initializer="glo
-0000b8a0: 726f 745f 756e 6966 6f72 6d22 2c0a 2020  rot_uniform",.  
-0000b8b0: 2020 2020 2020 656e 7469 7479 5f72 656c        entity_rel
-0000b8c0: 6174 696f 6e5f 7265 6775 6c61 7269 7a65  ation_regularize
-0000b8d0: 723d 4e6f 6e65 2c0a 2020 2020 2020 2020  r=None,.        
-0000b8e0: 2a2a 6b77 6172 6773 0a20 2020 2029 3a0a  **kwargs.    ):.
-0000b8f0: 2020 2020 2020 2020 2222 2220 436f 6d70          """ Comp
-0000b900: 696c 6520 7468 6520 6d6f 6465 6c2e 0a0a  ile the model...
-0000b910: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0000b920: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0000b930: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6f70  -----.        op
-0000b940: 7469 6d69 7a65 723a 2073 7472 2028 6e61  timizer: str (na
-0000b950: 6d65 206f 6620 6f70 7469 6d69 7a65 7229  me of optimizer)
-0000b960: 206f 7220 6f70 7469 6d69 7a65 7220 696e   or optimizer in
-0000b970: 7374 616e 6365 0a20 2020 2020 2020 2020  stance.         
-0000b980: 2020 2054 6865 206f 7074 696d 697a 6572     The optimizer
-0000b990: 2075 7365 6420 746f 206d 696e 696d 697a   used to minimiz
-0000b9a0: 6520 7468 6520 6c6f 7373 2066 756e 6374  e the loss funct
-0000b9b0: 696f 6e2e 2046 6f72 2070 7265 2d64 6566  ion. For pre-def
-0000b9c0: 696e 6564 206f 7074 696f 6e73 2c20 6368  ined options, ch
-0000b9d0: 6f6f 7365 2062 6574 7765 656e 0a20 2020  oose between.   
-0000b9e0: 2020 2020 2020 2020 2060 2273 6764 2260           `"sgd"`
-0000b9f0: 2c20 6022 6164 6167 7261 6422 602c 2060  , `"adagrad"`, `
-0000ba00: 2261 6461 6d22 602c 2060 2272 6d73 7072  "adam"`, `"rmspr
-0000ba10: 6f70 2260 2c20 6574 632e 0a20 2020 2020  op"`, etc..     
-0000ba20: 2020 2020 2020 2053 6565 2060 7466 2e6b         See `tf.k
-0000ba30: 6572 6173 2e6f 7074 696d 697a 6572 7320  eras.optimizers 
-0000ba40: 3c68 7474 7073 3a2f 2f77 7777 2e74 656e  <https://www.ten
-0000ba50: 736f 7266 6c6f 772e 6f72 672f 6170 695f  sorflow.org/api_
-0000ba60: 646f 6373 2f70 7974 686f 6e2f 7466 2f6b  docs/python/tf/k
-0000ba70: 6572 6173 2f6f 7074 696d 697a 6572 733e  eras/optimizers>
-0000ba80: 605f 0a20 2020 2020 2020 2020 2020 2066  `_.            f
-0000ba90: 6f72 2075 702d 746f 2d64 6174 6520 6465  or up-to-date de
-0000baa0: 7461 696c 732e 0a0a 2020 2020 2020 2020  tails...        
-0000bab0: 2020 2020 4966 2061 2073 7472 696e 6720      If a string 
-0000bac0: 6973 2070 6173 7365 642c 2074 6865 6e20  is passed, then 
-0000bad0: 7468 6520 6465 6661 756c 7420 7061 7261  the default para
-0000bae0: 6d65 7465 7273 206f 6620 7468 6520 6f70  meters of the op
-0000baf0: 7469 6d69 7a65 7220 7769 6c6c 2062 6520  timizer will be 
-0000bb00: 7573 6564 2e0a 0a20 2020 2020 2020 2020  used...         
-0000bb10: 2020 2049 6620 796f 7520 7761 6e74 2074     If you want t
-0000bb20: 6f20 7573 6520 6375 7374 6f6d 2068 7970  o use custom hyp
-0000bb30: 6572 7061 7261 6d65 7465 7273 2079 6f75  erparameters you
-0000bb40: 206e 6565 6420 746f 2063 7265 6174 6520   need to create 
-0000bb50: 616e 2069 6e73 7461 6e63 6520 6f66 2074  an instance of t
-0000bb60: 6865 206f 7074 696d 697a 6572 2061 6e64  he optimizer and
-0000bb70: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
-0000bb80: 7320 7468 6520 696e 7374 616e 6365 2074  s the instance t
-0000bb90: 6f20 7468 6520 636f 6d70 696c 6520 6675  o the compile fu
-0000bba0: 6e63 7469 6f6e 203a 3a0a 0a20 2020 2020  nction ::..     
-0000bbb0: 2020 2020 2020 2020 2020 2069 6d70 6f72             impor
-0000bbc0: 7420 7465 6e73 6f72 666c 6f77 2061 7320  t tensorflow as 
-0000bbd0: 7466 0a20 2020 2020 2020 2020 2020 2020  tf.             
-0000bbe0: 2020 2061 6461 6d5f 6f70 7420 3d20 7466     adam_opt = tf
-0000bbf0: 2e6b 6572 6173 2e6f 7074 696d 697a 6572  .keras.optimizer
-0000bc00: 732e 4164 616d 286c 6561 726e 696e 675f  s.Adam(learning_
-0000bc10: 7261 7465 3d30 2e30 3033 290a 2020 2020  rate=0.003).    
-0000bc20: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-0000bc30: 6c2e 636f 6d70 696c 6528 6c6f 7373 3d27  l.compile(loss='
-0000bc40: 7061 6972 7769 7365 272c 206f 7074 696d  pairwise', optim
-0000bc50: 3d61 6461 6d5f 6f70 7429 0a0a 2020 2020  =adam_opt)..    
-0000bc60: 2020 2020 6c6f 7373 3a20 7374 7220 286e      loss: str (n
-0000bc70: 616d 6520 6f66 206f 626a 6563 7469 7665  ame of objective
-0000bc80: 2066 756e 6374 696f 6e29 2c20 6f62 6a65   function), obje
-0000bc90: 6374 6976 6520 6675 6e63 7469 6f6e 206f  ctive function o
-0000bca0: 7220 6061 6d70 6c69 6772 6170 682e 6c61  r `ampligraph.la
-0000bcb0: 7465 6e74 5f66 6561 7475 7265 732e 6c6f  tent_features.lo
-0000bcc0: 7373 5f66 756e 6374 696f 6e73 2e4c 6f73  ss_functions.Los
-0000bcd0: 7360 0a0a 2020 2020 2020 2020 2020 2020  s`..            
-0000bce0: 4966 2061 2073 7472 696e 6720 6973 2070  If a string is p
-0000bcf0: 6173 7365 642c 2079 6f75 2063 616e 2075  assed, you can u
-0000bd00: 7365 206f 6e65 206f 6620 7468 6520 666f  se one of the fo
-0000bd10: 6c6c 6f77 696e 6720 6c6f 7373 6573 2077  llowing losses w
-0000bd20: 6869 6368 2077 696c 6c20 6265 2075 7365  hich will be use
-0000bd30: 6420 7769 7468 2074 6865 6972 0a20 2020  d with their.   
-0000bd40: 2020 2020 2020 2020 2064 6566 6175 6c74           default
-0000bd50: 2073 6574 7469 6e67 3a0a 0a20 2020 2020   setting:..     
-0000bd60: 2020 2020 2020 202d 2060 2270 6169 7277         - `"pairw
-0000bd70: 6973 6522 603a 2020 7468 6520 6d6f 6465  ise"`:  the mode
-0000bd80: 6c20 7769 6c6c 2075 7365 2074 6865 2070  l will use the p
-0000bd90: 6169 7277 6973 6520 6d61 7267 696e 2d62  airwise margin-b
-0000bda0: 6173 6564 206c 6f73 7320 6675 6e63 7469  ased loss functi
-0000bdb0: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-0000bdc0: 2d20 6022 6e6c 6c22 603a 2074 6865 206d  - `"nll"`: the m
-0000bdd0: 6f64 656c 2077 696c 6c20 7573 6520 7468  odel will use th
-0000bde0: 6520 6e65 6761 7469 7665 206c 6f73 7320  e negative loss 
-0000bdf0: 6c69 6b65 6c69 686f 6f64 2e0a 2020 2020  likelihood..    
-0000be00: 2020 2020 2020 2020 2d20 6022 6162 736f          - `"abso
-0000be10: 6c75 7465 5f6d 6172 6769 6e22 603a 2074  lute_margin"`: t
-0000be20: 6865 206d 6f64 656c 2077 696c 6c20 7573  he model will us
-0000be30: 6520 7468 6520 6162 736f 6c75 7465 206d  e the absolute m
-0000be40: 6172 6769 6e20 6c69 6b65 6c69 686f 6f64  argin likelihood
-0000be50: 2e0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
-0000be60: 6022 7365 6c66 5f61 6476 6572 7361 7269  `"self_adversari
-0000be70: 616c 2260 3a20 7468 6520 6d6f 6465 6c20  al"`: the model 
-0000be80: 7769 6c6c 2075 7365 2074 6865 2061 6476  will use the adv
-0000be90: 6572 7361 7269 616c 2073 616d 706c 696e  ersarial samplin
-0000bea0: 6720 6c6f 7373 2066 756e 6374 696f 6e2e  g loss function.
-0000beb0: 0a20 2020 2020 2020 2020 2020 202d 2060  .            - `
-0000bec0: 226d 756c 7469 636c 6173 735f 6e6c 6c22  "multiclass_nll"
-0000bed0: 603a 2074 6865 206d 6f64 656c 2077 696c  `: the model wil
-0000bee0: 6c20 7573 6520 7468 6520 6d75 6c74 6963  l use the multic
-0000bef0: 6c61 7373 206e 6c6c 206c 6f73 732e 203a  lass nll loss. :
-0000bf00: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000bf10: 2020 206d 6f64 656c 2e63 6f6d 7069 6c65     model.compile
-0000bf20: 286c 6f73 733d 2761 6273 6f6c 7574 655f  (loss='absolute_
-0000bf30: 6d61 7267 696e 272c 206f 7074 696d 3d27  margin', optim='
-0000bf40: 6164 616d 2729 0a0a 2020 2020 2020 2020  adam')..        
-0000bf50: 2020 2020 4966 2079 6f75 2077 616e 7420      If you want 
-0000bf60: 746f 206d 6f64 6966 7920 7468 6520 6465  to modify the de
-0000bf70: 6661 756c 7420 7061 7261 6d65 7465 7273  fault parameters
-0000bf80: 206f 6620 7468 6520 6c6f 7373 2066 756e   of the loss fun
-0000bf90: 6374 696f 6e2c 2079 6f75 206e 6565 6420  ction, you need 
-0000bfa0: 746f 2065 7870 6c69 6374 6c79 2063 7265  to explictly cre
-0000bfb0: 6174 6520 616e 2069 6e73 7461 6e63 650a  ate an instance.
-0000bfc0: 2020 2020 2020 2020 2020 2020 6f66 2074              of t
-0000bfd0: 6865 206c 6f73 7320 7769 7468 2072 6571  he loss with req
-0000bfe0: 7569 7265 6420 6879 7065 7270 6172 616d  uired hyperparam
-0000bff0: 6574 6572 7320 616e 6420 7468 656e 2070  eters and then p
-0000c000: 6173 7320 7468 6973 2069 6e73 7461 6e63  ass this instanc
-0000c010: 652e 203a 3a0a 0a20 2020 2020 2020 2020  e. ::..         
-0000c020: 2020 2020 2020 2066 726f 6d20 616d 706c         from ampl
-0000c030: 6967 7261 7068 2e6c 6174 656e 745f 6665  igraph.latent_fe
-0000c040: 6174 7572 6573 2069 6d70 6f72 7420 4162  atures import Ab
-0000c050: 736f 6c75 7465 4d61 7267 696e 4c6f 7373  soluteMarginLoss
-0000c060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c070: 2061 625f 6c6f 7373 203d 2041 6273 6f6c   ab_loss = Absol
-0000c080: 7574 654d 6172 6769 6e4c 6f73 7328 6c6f  uteMarginLoss(lo
-0000c090: 7373 5f70 6172 616d 733d 7b27 6d61 7267  ss_params={'marg
-0000c0a0: 696e 273a 2033 7d29 0a20 2020 2020 2020  in': 3}).       
-0000c0b0: 2020 2020 2020 2020 206d 6f64 656c 2e63           model.c
-0000c0c0: 6f6d 7069 6c65 286c 6f73 733d 6162 5f6c  ompile(loss=ab_l
-0000c0d0: 6f73 732c 206f 7074 696d 3d27 6164 616d  oss, optim='adam
-0000c0e0: 2729 0a0a 2020 2020 2020 2020 2020 2020  ')..            
-0000c0f0: 416e 206f 626a 6563 7469 7665 2066 756e  An objective fun
-0000c100: 6374 696f 6e20 6973 2061 6e79 2063 616c  ction is any cal
-0000c110: 6c61 626c 6520 7769 7468 2074 6865 2073  lable with the s
-0000c120: 6967 6e61 7475 7265 0a20 2020 2020 2020  ignature.       
-0000c130: 2020 2020 2060 606c 6f73 7320 3d20 666e       ``loss = fn
-0000c140: 2873 636f 7265 5f74 7275 652c 2073 636f  (score_true, sco
-0000c150: 7265 5f63 6f72 722c 2065 7461 2960 6020  re_corr, eta)`` 
-0000c160: 3a3a 0a0a 2020 2020 2020 2020 2020 2020  ::..            
-0000c170: 2020 2020 2320 4372 6561 7465 2061 2075      # Create a u
-0000c180: 7365 7220 6465 6669 6e65 6420 6c6f 7373  ser defined loss
-0000c190: 2066 756e 6374 696f 6e20 7769 7468 2074   function with t
-0000c1a0: 6865 2061 626f 7665 2073 6967 6e61 7475  he above signatu
-0000c1b0: 7265 0a20 2020 2020 2020 2020 2020 2020  re.             
-0000c1c0: 2020 2064 6566 2075 7365 724c 6f73 7328     def userLoss(
-0000c1d0: 7363 6f72 6573 5f70 6f73 2c20 7363 6f72  scores_pos, scor
-0000c1e0: 6573 5f6e 6567 293a 0a20 2020 2020 2020  es_neg):.       
-0000c1f0: 2020 2020 2020 2020 2020 2020 2023 2075               # u
-0000c200: 7365 7220 6465 6669 6e65 6420 6c6f 7373  ser defined loss
-0000c210: 202d 2074 616b 6573 2069 6e20 3220 7061   - takes in 2 pa
-0000c220: 7261 6d73 2061 6e64 2072 6574 7572 6e73  rams and returns
-0000c230: 206c 6f73 730a 2020 2020 2020 2020 2020   loss.          
-0000c240: 2020 2020 2020 2020 2020 6e65 675f 6578            neg_ex
-0000c250: 7020 3d20 7466 2e65 7870 2873 636f 7265  p = tf.exp(score
-0000c260: 735f 6e65 6729 0a20 2020 2020 2020 2020  s_neg).         
-0000c270: 2020 2020 2020 2020 2020 2070 6f73 5f65             pos_e
-0000c280: 7870 203d 2074 662e 6578 7028 7363 6f72  xp = tf.exp(scor
-0000c290: 6573 5f70 6f73 290a 2020 2020 2020 2020  es_pos).        
-0000c2a0: 2020 2020 2020 2020 2020 2020 2320 4170              # Ap
-0000c2b0: 706c 7920 736f 6674 6d61 7820 746f 2074  ply softmax to t
-0000c2c0: 6865 2073 636f 7265 730a 2020 2020 2020  he scores.      
-0000c2d0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-0000c2e0: 6f72 6520 3d20 706f 735f 6578 7020 2f20  ore = pos_exp / 
-0000c2f0: 2874 662e 7265 6475 6365 5f73 756d 286e  (tf.reduce_sum(n
-0000c300: 6567 5f65 7870 2c20 6178 6973 3d30 2920  eg_exp, axis=0) 
-0000c310: 2b20 706f 735f 6578 7029 0a20 2020 2020  + pos_exp).     
-0000c320: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000c330: 6f73 7320 3d20 2d74 662e 6d61 7468 2e6c  oss = -tf.math.l
-0000c340: 6f67 2873 636f 7265 290a 2020 2020 2020  og(score).      
-0000c350: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000c360: 7475 726e 206c 6f73 730a 2020 2020 2020  turn loss.      
-0000c370: 2020 2020 2020 2020 2020 2320 5061 7373            # Pass
-0000c380: 2074 6869 7320 6c6f 7373 2077 6869 6c65   this loss while
-0000c390: 2063 6f6d 7069 6c69 6e67 2074 6865 206d   compiling the m
-0000c3a0: 6f64 656c 0a20 2020 2020 2020 2020 2020  odel.           
-0000c3b0: 2020 2020 206d 6f64 656c 2e63 6f6d 7069       model.compi
-0000c3c0: 6c65 286c 6f73 733d 7573 6572 4c6f 7373  le(loss=userLoss
-0000c3d0: 2c20 6f70 7469 6d3d 2761 6461 6d27 290a  , optim='adam').
-0000c3e0: 0a20 2020 2020 2020 2065 6e74 6974 795f  .        entity_
-0000c3f0: 7265 6c61 7469 6f6e 5f69 6e69 7469 616c  relation_initial
-0000c400: 697a 6572 3a20 7374 7220 286e 616d 6520  izer: str (name 
-0000c410: 6f66 2069 6e69 7469 616c 697a 6572 2066  of initializer f
-0000c420: 756e 6374 696f 6e29 2c20 696e 6974 6961  unction), initia
-0000c430: 6c69 7a65 7220 6675 6e63 7469 6f6e 206f  lizer function o
-0000c440: 7220 5c0a 2020 2020 2020 2020 6074 662e  r \.        `tf.
-0000c450: 6b65 7261 732e 696e 6974 6961 6c69 7a65  keras.initialize
-0000c460: 7273 2e49 6e69 7469 616c 697a 6572 6020  rs.Initializer` 
-0000c470: 6f72 206c 6973 742e 0a0a 2020 2020 2020  or list...      
-0000c480: 2020 2020 2020 496e 6974 6961 6c69 7a65        Initialize
-0000c490: 7220 6f66 2074 6865 2065 6e74 6974 7920  r of the entity 
-0000c4a0: 616e 6420 7265 6c61 7469 6f6e 2065 6d62  and relation emb
-0000c4b0: 6564 6469 6e67 732e 2054 6869 7320 6973  eddings. This is
-0000c4c0: 2065 6974 6865 7220 6120 7369 6e67 6c65   either a single
-0000c4d0: 2076 616c 7565 206f 7220 6120 6c69 7374   value or a list
-0000c4e0: 206f 6620 7369 7a65 2032 2e0a 2020 2020   of size 2..    
-0000c4f0: 2020 2020 2020 2020 4966 2061 2073 696e          If a sin
-0000c500: 676c 6520 7661 6c75 6520 6973 2070 6173  gle value is pas
-0000c510: 7365 642c 2074 6865 6e20 626f 7468 2074  sed, then both t
-0000c520: 6865 2065 6e74 6974 6965 7320 616e 6420  he entities and 
-0000c530: 7265 6c61 7469 6f6e 7320 7769 6c6c 2062  relations will b
-0000c540: 6520 696e 6974 6961 6c69 7a65 6420 6261  e initialized ba
-0000c550: 7365 6420 6f6e 0a20 2020 2020 2020 2020  sed on.         
-0000c560: 2020 2074 6865 2073 616d 6520 696e 6974     the same init
-0000c570: 6961 6c69 7a65 723b 2069 6620 6120 6c69  ializer; if a li
-0000c580: 7374 2c20 7468 6520 6669 7273 7420 696e  st, the first in
-0000c590: 6974 6961 6c69 7a65 7220 7769 6c6c 2062  itializer will b
-0000c5a0: 6520 7573 6564 2066 6f72 2065 6e74 6974  e used for entit
-0000c5b0: 6965 7320 616e 6420 7468 6520 7365 636f  ies and the seco
-0000c5c0: 6e64 0a20 2020 2020 2020 2020 2020 2066  nd.            f
-0000c5d0: 6f72 2072 656c 6174 696f 6e73 2e0a 0a20  or relations... 
-0000c5e0: 2020 2020 2020 2020 2020 2049 6620 6120             If a 
-0000c5f0: 7374 7269 6e67 2069 7320 7061 7373 6564  string is passed
-0000c600: 2c20 7468 656e 2074 6865 2064 6566 6175  , then the defau
-0000c610: 6c74 2070 6172 616d 6574 6572 7320 7769  lt parameters wi
-0000c620: 6c6c 2062 6520 7573 6564 2e20 4368 6f6f  ll be used. Choo
-0000c630: 7365 2062 6574 7765 656e 0a20 2020 2020  se between.     
-0000c640: 2020 2020 2020 2060 2272 616e 646f 6d5f         `"random_
-0000c650: 6e6f 726d 616c 2260 2c20 6022 7261 6e64  normal"`, `"rand
-0000c660: 6f6d 5f75 6e69 666f 726d 2260 2c20 6022  om_uniform"`, `"
-0000c670: 676c 6f72 6f74 5f6e 6f72 6d61 6c22 602c  glorot_normal"`,
-0000c680: 2060 2268 655f 6e6f 726d 616c 2260 2c20   `"he_normal"`, 
-0000c690: 6574 632e 0a0a 2020 2020 2020 2020 2020  etc...          
-0000c6a0: 2020 5365 6520 6074 662e 6b65 7261 732e    See `tf.keras.
-0000c6b0: 696e 6974 6961 6c69 7a65 7273 203c 6874  initializers <ht
-0000c6c0: 7470 733a 2f2f 7777 772e 7465 6e73 6f72  tps://www.tensor
-0000c6d0: 666c 6f77 2e6f 7267 2f61 7069 5f64 6f63  flow.org/api_doc
-0000c6e0: 732f 7079 7468 6f6e 2f74 662f 6b65 7261  s/python/tf/kera
-0000c6f0: 732f 696e 6974 6961 6c69 7a65 7273 3e60  s/initializers>`
-0000c700: 5f0a 2020 2020 2020 2020 2020 2020 666f  _.            fo
-0000c710: 7220 7570 2d74 6f2d 6461 7465 2064 6574  r up-to-date det
-0000c720: 6169 6c73 2e20 3a3a 0a0a 2020 2020 2020  ails. ::..      
-0000c730: 2020 2020 2020 2020 2020 6d6f 6465 6c2e            model.
-0000c740: 636f 6d70 696c 6528 6c6f 7373 3d27 7061  compile(loss='pa
-0000c750: 6972 7769 7365 272c 206f 7074 696d 3d27  irwise', optim='
-0000c760: 6164 616d 272c 0a20 2020 2020 2020 2020  adam',.         
-0000c770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c780: 2020 2020 2065 6e74 6974 795f 7265 6c61       entity_rela
-0000c790: 7469 6f6e 5f69 6e69 7469 616c 697a 6572  tion_initializer
-0000c7a0: 3d27 7261 6e64 6f6d 5f6e 6f72 6d61 6c27  ='random_normal'
-0000c7b0: 290a 0a20 2020 2020 2020 2020 2020 2049  )..            I
-0000c7c0: 6620 7468 6520 7573 6572 2077 616e 7473  f the user wants
-0000c7d0: 2074 6f20 7573 6520 6375 7374 6f6d 2068   to use custom h
-0000c7e0: 7970 6572 7061 7261 6d65 7465 7273 2c20  yperparameters, 
-0000c7f0: 7468 656e 2061 6e20 696e 7374 616e 6365  then an instance
-0000c800: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
-0000c810: 2020 2020 6060 7466 2e6b 6572 6173 2e69      ``tf.keras.i
-0000c820: 6e69 7469 616c 697a 6572 732e 496e 6974  nitializers.Init
-0000c830: 6961 6c69 7a65 7260 6020 6e65 6564 7320  ializer`` needs 
-0000c840: 746f 2062 6520 7061 7373 6564 2e20 3a3a  to be passed. ::
-0000c850: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c860: 2020 696d 706f 7274 2074 656e 736f 7266    import tensorf
-0000c870: 6c6f 7720 6173 2074 660a 2020 2020 2020  low as tf.      
-0000c880: 2020 2020 2020 2020 2020 696e 6974 203d            init =
-0000c890: 2074 662e 6b65 7261 732e 696e 6974 6961   tf.keras.initia
-0000c8a0: 6c69 7a65 7273 2e52 616e 646f 6d4e 6f72  lizers.RandomNor
-0000c8b0: 6d61 6c28 7374 6464 6576 3d30 2e30 3030  mal(stddev=0.000
-0000c8c0: 3033 290a 2020 2020 2020 2020 2020 2020  03).            
-0000c8d0: 2020 2020 6d6f 6465 6c2e 636f 6d70 696c      model.compil
-0000c8e0: 6528 6c6f 7373 3d27 7061 6972 7769 7365  e(loss='pairwise
-0000c8f0: 272c 206f 7074 696d 3d27 6164 616d 272c  ', optim='adam',
-0000c900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c910: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000c920: 6e74 6974 795f 7265 6c61 7469 6f6e 5f69  ntity_relation_i
-0000c930: 6e69 7469 616c 697a 6572 3d69 6e69 7429  nitializer=init)
-0000c940: 0a0a 2020 2020 2020 2020 2020 2020 4966  ..            If
-0000c950: 2074 6865 2075 7365 7220 7761 6e74 7320   the user wants 
-0000c960: 746f 2064 6566 696e 6520 6375 7374 6f6d  to define custom
-0000c970: 2069 6e69 7469 616c 697a 6572 2069 7420   initializer it 
-0000c980: 6361 6e20 6265 2061 6e79 2063 616c 6c61  can be any calla
-0000c990: 626c 6520 7769 7468 2074 6865 2073 6967  ble with the sig
-0000c9a0: 6e61 7475 7265 2060 696e 6974 203d 2066  nature `init = f
-0000c9b0: 6e28 7368 6170 6529 6020 3a3a 0a0a 2020  n(shape)` ::..  
-0000c9c0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-0000c9d0: 6620 6d79 5f69 6e69 7428 7368 6170 6529  f my_init(shape)
-0000c9e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c9f0: 2020 2020 2020 7265 7475 726e 2074 662e        return tf.
-0000ca00: 7261 6e64 6f6d 2e6e 6f72 6d61 6c28 7368  random.normal(sh
-0000ca10: 6170 6529 0a20 2020 2020 2020 2020 2020  ape).           
-0000ca20: 2020 2020 206d 6f64 656c 2e63 6f6d 7069       model.compi
-0000ca30: 6c65 286c 6f73 733d 2770 6169 7277 6973  le(loss='pairwis
-0000ca40: 6527 2c20 6f70 7469 6d3d 2761 6461 6d27  e', optim='adam'
-0000ca50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ca60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca70: 656e 7469 7479 5f72 656c 6174 696f 6e5f  entity_relation_
-0000ca80: 696e 6974 6961 6c69 7a65 723d 6d79 5f69  initializer=my_i
-0000ca90: 6e69 7429 0a0a 2020 2020 2020 2020 656e  nit)..        en
-0000caa0: 7469 7479 5f72 656c 6174 696f 6e5f 7265  tity_relation_re
-0000cab0: 6775 6c61 7269 7a65 723a 2073 7472 2028  gularizer: str (
-0000cac0: 6e61 6d65 206f 6620 7265 6775 6c61 7269  name of regulari
-0000cad0: 7a65 7220 6675 6e63 7469 6f6e 2920 6f72  zer function) or
-0000cae0: 2072 6567 756c 6172 697a 6572 2066 756e   regularizer fun
-0000caf0: 6374 696f 6e20 6f72 205c 0a20 2020 2020  ction or \.     
-0000cb00: 2020 2060 7466 2e6b 6572 6173 2e72 6567     `tf.keras.reg
-0000cb10: 756c 6172 697a 6572 732e 5265 6775 6c61  ularizers.Regula
-0000cb20: 7269 7a65 7260 2069 6e73 7461 6e63 6520  rizer` instance 
-0000cb30: 6f72 206c 6973 740a 2020 2020 2020 2020  or list.        
-0000cb40: 2020 2020 5265 6775 6c61 7269 7a65 7220      Regularizer 
-0000cb50: 6f66 2065 6e74 6974 6965 7320 616e 6420  of entities and 
-0000cb60: 7265 6c61 7469 6f6e 732e 0a20 2020 2020  relations..     
-0000cb70: 2020 2020 2020 2049 6620 6120 7369 6e67         If a sing
-0000cb80: 6c65 2076 616c 7565 2069 7320 7061 7373  le value is pass
-0000cb90: 6564 2c20 7468 656e 2062 6f74 6820 7468  ed, then both th
-0000cba0: 6520 656e 7469 7469 6573 2061 6e64 2072  e entities and r
-0000cbb0: 656c 6174 696f 6e73 2077 696c 6c20 6265  elations will be
-0000cbc0: 2072 6567 756c 6172 697a 6564 2062 6173   regularized bas
-0000cbd0: 6564 206f 6e0a 2020 2020 2020 2020 2020  ed on.          
-0000cbe0: 2020 7468 6520 7361 6d65 2072 6567 756c    the same regul
-0000cbf0: 6172 697a 6572 3b20 6966 2061 206c 6973  arizer; if a lis
-0000cc00: 742c 2074 6865 2066 6972 7374 2072 6567  t, the first reg
-0000cc10: 756c 6172 697a 6572 2077 696c 6c20 6265  ularizer will be
-0000cc20: 2075 7365 6420 666f 7220 656e 7469 7469   used for entiti
-0000cc30: 6573 2061 6e64 2073 6563 6f6e 640a 2020  es and second.  
-0000cc40: 2020 2020 2020 2020 2020 666f 7220 7265            for re
-0000cc50: 6c61 7469 6f6e 732e 0a0a 2020 2020 2020  lations...      
-0000cc60: 2020 2020 2020 4966 2061 2073 7472 696e        If a strin
-0000cc70: 6720 6973 2070 6173 7365 642c 2074 6865  g is passed, the
-0000cc80: 6e20 7468 6520 6465 6661 756c 7420 7061  n the default pa
-0000cc90: 7261 6d65 7465 7273 206f 6620 7468 6520  rameters of the 
-0000cca0: 7265 6775 6c61 7269 7a65 7273 2077 696c  regularizers wil
-0000ccb0: 6c20 6265 2075 7365 642e 2043 686f 6f73  l be used. Choos
-0000ccc0: 6520 6265 7477 6565 6e0a 2020 2020 2020  e between.      
-0000ccd0: 2020 2020 2020 6022 6c31 2260 2c20 6022        `"l1"`, `"
-0000cce0: 6c32 2260 2c20 6022 6c31 5f6c 3222 602c  l2"`, `"l1_l2"`,
-0000ccf0: 2065 7463 2e0a 0a20 2020 2020 2020 2020   etc...         
-0000cd00: 2020 2053 6565 2060 7466 2e6b 6572 6173     See `tf.keras
-0000cd10: 2e72 6567 756c 6172 697a 6572 7320 3c68  .regularizers <h
-0000cd20: 7474 7073 3a2f 2f77 7777 2e74 656e 736f  ttps://www.tenso
-0000cd30: 7266 6c6f 772e 6f72 672f 6170 695f 646f  rflow.org/api_do
-0000cd40: 6373 2f70 7974 686f 6e2f 7466 2f6b 6572  cs/python/tf/ker
-0000cd50: 6173 2f72 6567 756c 6172 697a 6572 733e  as/regularizers>
-0000cd60: 605f 0a20 2020 2020 2020 2020 2020 2066  `_.            f
-0000cd70: 6f72 2075 702d 746f 2d64 6174 6520 6465  or up-to-date de
-0000cd80: 7461 696c 732e 203a 3a0a 0a20 2020 2020  tails. ::..     
-0000cd90: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-0000cda0: 2e63 6f6d 7069 6c65 286c 6f73 733d 2770  .compile(loss='p
-0000cdb0: 6169 7277 6973 6527 2c20 6f70 7469 6d3d  airwise', optim=
-0000cdc0: 2761 6461 6d27 2c0a 2020 2020 2020 2020  'adam',.        
-0000cdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cde0: 2020 2020 2020 656e 7469 7479 5f72 656c        entity_rel
-0000cdf0: 6174 696f 6e5f 7265 6775 6c61 7269 7a65  ation_regularize
-0000ce00: 723d 276c 3227 290a 0a20 2020 2020 2020  r='l2')..       
-0000ce10: 2020 2020 2049 6620 7468 6520 7573 6572       If the user
-0000ce20: 2077 616e 7473 2074 6f20 7573 6520 6375   wants to use cu
-0000ce30: 7374 6f6d 2068 7970 6572 7061 7261 6d65  stom hyperparame
-0000ce40: 7465 7273 2c20 7468 656e 2061 6e20 696e  ters, then an in
-0000ce50: 7374 616e 6365 206f 6620 7468 650a 2020  stance of the.  
-0000ce60: 2020 2020 2020 2020 2020 6060 7466 2e6b            ``tf.k
-0000ce70: 6572 6173 2e72 6567 756c 6172 697a 6572  eras.regularizer
-0000ce80: 732e 5265 6775 6c61 7269 7a65 7260 6020  s.Regularizer`` 
-0000ce90: 6e65 6564 7320 746f 2062 6520 7061 7373  needs to be pass
-0000cea0: 6564 2e20 3a3a 0a0a 2020 2020 2020 2020  ed. ::..        
-0000ceb0: 2020 2020 2020 2020 696d 706f 7274 2074          import t
-0000cec0: 656e 736f 7266 6c6f 7720 6173 2074 660a  ensorflow as tf.
-0000ced0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cee0: 7265 6720 3d20 7466 2e6b 6572 6173 2e72  reg = tf.keras.r
-0000cef0: 6567 756c 6172 697a 6572 732e 4c31 4c32  egularizers.L1L2
-0000cf00: 286c 313d 302e 3030 312c 206c 323d 302e  (l1=0.001, l2=0.
-0000cf10: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
-0000cf20: 2020 206d 6f64 656c 2e63 6f6d 7069 6c65     model.compile
-0000cf30: 286c 6f73 733d 2770 6169 7277 6973 6527  (loss='pairwise'
-0000cf40: 2c20 6f70 7469 6d3d 2761 6461 6d27 2c0a  , optim='adam',.
-0000cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf60: 2020 2020 2020 2020 2020 2020 2020 656e                en
-0000cf70: 7469 7479 5f72 656c 6174 696f 6e5f 7265  tity_relation_re
-0000cf80: 6775 6c61 7269 7a65 723d 7265 6729 0a0a  gularizer=reg)..
-0000cf90: 2020 2020 2020 2020 2020 2020 4966 2074              If t
-0000cfa0: 6865 2075 7365 7220 7761 6e74 7320 746f  he user wants to
-0000cfb0: 2064 6566 696e 6520 6375 7374 6f6d 2072   define custom r
-0000cfc0: 6567 756c 6172 697a 6572 2069 7420 6361  egularizer it ca
-0000cfd0: 6e20 6265 2061 6e79 2063 616c 6c61 626c  n be any callabl
-0000cfe0: 6520 7769 7468 2073 6967 6e61 7475 7265  e with signature
-0000cff0: 0a20 2020 2020 2020 2020 2020 2060 6072  .            ``r
-0000d000: 6567 203d 2066 6e28 7765 6967 6874 5f6d  eg = fn(weight_m
-0000d010: 6174 7269 7829 6060 2e20 3a3a 0a0a 2020  atrix)``. ::..  
-0000d020: 2020 2020 2020 2020 2020 2020 2020 6465                de
-0000d030: 6620 6d79 5f72 6567 2877 6569 6768 745f  f my_reg(weight_
-0000d040: 6d78 293a 0a20 2020 2020 2020 2020 2020  mx):.           
-0000d050: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000d060: 6e20 302e 3031 202a 2074 662e 6d61 7468  n 0.01 * tf.math
-0000d070: 2e72 6564 7563 655f 7375 6d28 7466 2e6d  .reduce_sum(tf.m
-0000d080: 6174 682e 6162 7328 7765 6967 6874 5f6d  ath.abs(weight_m
-0000d090: 7829 290a 2020 2020 2020 2020 2020 2020  x)).            
-0000d0a0: 2020 2020 6d6f 6465 6c2e 636f 6d70 696c      model.compil
-0000d0b0: 6528 6c6f 7373 3d27 7061 6972 7769 7365  e(loss='pairwise
-0000d0c0: 272c 206f 7074 696d 3d27 6164 616d 272c  ', optim='adam',
-0000d0d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000d0f0: 6e74 6974 795f 7265 6c61 7469 6f6e 5f72  ntity_relation_r
-0000d100: 6567 756c 6172 697a 6572 3d6d 795f 7265  egularizer=my_re
-0000d110: 6729 0a0a 2020 2020 2020 2020 4578 616d  g)..        Exam
-0000d120: 706c 650a 2020 2020 2020 2020 2d2d 2d2d  ple.        ----
-0000d130: 2d2d 2d0a 2020 2020 2020 2020 3e3e 3e20  ---.        >>> 
-0000d140: 6672 6f6d 2061 6d70 6c69 6772 6170 682e  from ampligraph.
-0000d150: 6461 7461 7365 7473 2069 6d70 6f72 7420  datasets import 
-0000d160: 6c6f 6164 5f66 6231 356b 5f32 3337 0a20  load_fb15k_237. 
-0000d170: 2020 2020 2020 203e 3e3e 2066 726f 6d20         >>> from 
-0000d180: 616d 706c 6967 7261 7068 2e6c 6174 656e  ampligraph.laten
-0000d190: 745f 6665 6174 7572 6573 2069 6d70 6f72  t_features impor
-0000d1a0: 7420 5363 6f72 696e 6742 6173 6564 456d  t ScoringBasedEm
-0000d1b0: 6265 6464 696e 674d 6f64 656c 0a20 2020  beddingModel.   
-0000d1c0: 2020 2020 203e 3e3e 2058 203d 206c 6f61       >>> X = loa
-0000d1d0: 645f 6662 3135 6b5f 3233 3728 290a 2020  d_fb15k_237().  
-0000d1e0: 2020 2020 2020 3e3e 3e20 6d6f 6465 6c20        >>> model 
-0000d1f0: 3d20 5363 6f72 696e 6742 6173 6564 456d  = ScoringBasedEm
-0000d200: 6265 6464 696e 674d 6f64 656c 2865 7461  beddingModel(eta
-0000d210: 3d35 2c0a 2020 2020 2020 2020 3e3e 3e20  =5,.        >>> 
+00008b80: 2020 2020 5b76 616c 6964 6174 696f 6e5f      [validation_
+00008b90: 6461 7461 2c20 6e61 6e5f 7765 6967 6874  data, nan_weight
+00008ba0: 735d 2c20 6178 6973 3d31 0a20 2020 2020  s], axis=1.     
+00008bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bc0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00008bd0: 2020 2020 2020 2020 2023 2065 7661 6c75           # evalu
+00008be0: 6174 6520 6f6e 2074 6865 2076 616c 6964  ate on the valid
+00008bf0: 6174 696f 6e0a 2020 2020 2020 2020 2020  ation.          
+00008c00: 2020 2020 2020 2020 2020 7261 6e6b 7320            ranks 
+00008c10: 3d20 7365 6c66 2e65 7661 6c75 6174 6528  = self.evaluate(
+00008c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008c30: 2020 2020 2020 2020 2076 616c 6964 6174           validat
+00008c40: 696f 6e5f 6461 7461 2c0a 2020 2020 2020  ion_data,.      
+00008c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c60: 2020 6261 7463 685f 7369 7a65 3d76 616c    batch_size=val
+00008c70: 6964 6174 696f 6e5f 6261 7463 685f 7369  idation_batch_si
+00008c80: 7a65 206f 7220 6261 7463 685f 7369 7a65  ze or batch_size
+00008c90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008ca0: 2020 2020 2020 2020 2020 7573 655f 6669            use_fi
+00008cb0: 6c74 6572 3d76 616c 6964 6174 696f 6e5f  lter=validation_
+00008cc0: 6669 6c74 6572 2c0a 2020 2020 2020 2020  filter,.        
+00008cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ce0: 6461 7461 7365 745f 7479 7065 3d22 7661  dataset_type="va
+00008cf0: 6c69 6422 2c0a 2020 2020 2020 2020 2020  lid",.          
+00008d00: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00008d10: 7272 7570 745f 7369 6465 3d76 616c 6964  rrupt_side=valid
+00008d20: 6174 696f 6e5f 636f 7272 7570 745f 7369  ation_corrupt_si
+00008d30: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
+00008d40: 2020 2020 2020 2020 2020 2020 656e 7469              enti
+00008d50: 7469 6573 5f73 7562 7365 743d 7661 6c69  ties_subset=vali
+00008d60: 6461 7469 6f6e 5f65 6e74 6974 6965 735f  dation_entities_
+00008d70: 7375 6273 6574 2c0a 2020 2020 2020 2020  subset,.        
+00008d80: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00008d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008da0: 2020 2320 636f 6d70 7574 6520 616c 6c20    # compute all 
+00008db0: 7468 6520 6d65 7472 6963 730a 2020 2020  the metrics.    
+00008dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008dd0: 7661 6c5f 6c6f 6773 203d 207b 0a20 2020  val_logs = {.   
+00008de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008df0: 2020 2020 2022 7661 6c5f 6d72 7222 3a20       "val_mrr": 
+00008e00: 6d72 725f 7363 6f72 6528 7261 6e6b 7329  mrr_score(ranks)
+00008e10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008e20: 2020 2020 2020 2020 2020 2276 616c 5f6d            "val_m
+00008e30: 7222 3a20 6d72 5f73 636f 7265 2872 616e  r": mr_score(ran
+00008e40: 6b73 292c 0a20 2020 2020 2020 2020 2020  ks),.           
+00008e50: 2020 2020 2020 2020 2020 2020 2022 7661               "va
+00008e60: 6c5f 6869 7473 4031 223a 2068 6974 735f  l_hits@1": hits_
+00008e70: 6174 5f6e 5f73 636f 7265 2872 616e 6b73  at_n_score(ranks
+00008e80: 2c20 3129 2c0a 2020 2020 2020 2020 2020  , 1),.          
+00008e90: 2020 2020 2020 2020 2020 2020 2020 2276                "v
+00008ea0: 616c 5f68 6974 7340 3130 223a 2068 6974  al_hits@10": hit
+00008eb0: 735f 6174 5f6e 5f73 636f 7265 2872 616e  s_at_n_score(ran
+00008ec0: 6b73 2c20 3130 292c 0a20 2020 2020 2020  ks, 10),.       
+00008ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ee0: 2022 7661 6c5f 6869 7473 4031 3030 223a   "val_hits@100":
+00008ef0: 2068 6974 735f 6174 5f6e 5f73 636f 7265   hits_at_n_score
+00008f00: 2872 616e 6b73 2c20 3130 3029 2c0a 2020  (ranks, 100),.  
+00008f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f20: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00008f30: 2020 2020 2020 2020 2320 7570 6461 7465          # update
+00008f40: 2074 6865 2065 706f 6368 206c 6f67 7320   the epoch logs 
+00008f50: 7769 7468 2076 616c 6964 6174 696f 6e20  with validation 
+00008f60: 6465 7461 696c 730a 2020 2020 2020 2020  details.        
+00008f70: 2020 2020 2020 2020 2020 2020 6570 6f63              epoc
+00008f80: 685f 6c6f 6773 2e75 7064 6174 6528 7661  h_logs.update(va
+00008f90: 6c5f 6c6f 6773 290a 0a20 2020 2020 2020  l_logs)..       
+00008fa0: 2020 2020 2020 2020 2023 2061 6674 6572           # after
+00008fb0: 2061 6e20 6570 6f63 6820 6973 2063 6f6d   an epoch is com
+00008fc0: 706c 6574 6564 2c20 6361 6c6c 2074 6869  pleted, call thi
+00008fd0: 7320 6361 6c6c 6261 636b 2066 756e 6374  s callback funct
+00008fe0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+00008ff0: 2020 2020 6361 6c6c 6261 636b 732e 6f6e      callbacks.on
+00009000: 5f65 706f 6368 5f65 6e64 2865 706f 6368  _epoch_end(epoch
+00009010: 2c20 6570 6f63 685f 6c6f 6773 290a 2020  , epoch_logs).  
+00009020: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00009030: 2073 656c 662e 7374 6f70 5f74 7261 696e   self.stop_train
+00009040: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
+00009050: 2020 2020 2020 2020 2062 7265 616b 0a0a           break..
+00009060: 2020 2020 2020 2020 2020 2020 2320 6f6e              # on
+00009070: 2074 7261 696e 696e 6720 656e 6420 6361   training end ca
+00009080: 6c6c 2074 6869 7320 6d65 7468 6f64 0a20  ll this method. 
+00009090: 2020 2020 2020 2020 2020 2063 616c 6c62             callb
+000090a0: 6163 6b73 2e6f 6e5f 7472 6169 6e5f 656e  acks.on_train_en
+000090b0: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
+000090c0: 7365 6c66 2e69 735f 6669 7474 6564 203d  self.is_fitted =
+000090d0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+000090e0: 2020 2320 616c 6c20 7468 6520 7472 6169    # all the trai
+000090f0: 6e69 6e67 2061 6e64 2076 616c 6964 6174  ning and validat
+00009100: 696f 6e20 6c6f 6773 2061 7265 2073 746f  ion logs are sto
+00009110: 7265 6420 696e 2074 6865 2068 6973 746f  red in the histo
+00009120: 7279 0a20 2020 2020 2020 2020 2020 2023  ry.            #
+00009130: 206f 626a 6563 7420 6279 206b 6572 6173   object by keras
+00009140: 2e4d 6f64 656c 0a20 2020 2020 2020 2020  .Model.         
+00009150: 2020 2072 6574 7572 6e20 7365 6c66 2e68     return self.h
+00009160: 6973 746f 7279 0a0a 2020 2020 6465 6620  istory..    def 
+00009170: 6765 745f 696e 6465 7865 7328 7365 6c66  get_indexes(self
+00009180: 2c20 582c 2074 7970 655f 6f66 3d22 7422  , X, type_of="t"
+00009190: 2c20 6f72 6465 723d 2272 6177 3269 6e64  , order="raw2ind
+000091a0: 2229 3a0a 2020 2020 2020 2020 2222 2243  "):.        """C
+000091b0: 6f6e 7665 7274 7320 6769 7665 6e20 6461  onverts given da
+000091c0: 7461 2074 6f20 696e 6465 7865 7320 6f72  ta to indexes or
+000091d0: 2074 6f20 7261 7720 6461 7461 2028 6163   to raw data (ac
+000091e0: 636f 7264 696e 6720 746f 2060 606f 7264  cording to ``ord
+000091f0: 6572 6060 292e 0a0a 2020 2020 2020 2020  er``)...        
+00009200: 2049 7420 776f 726b 7320 666f 7220 6060   It works for ``
+00009210: 5860 6020 636f 6e74 6169 6e69 6e67 2074  X`` containing t
+00009220: 7269 706c 6573 2c20 656e 7469 7469 6573  riples, entities
+00009230: 2c20 6f72 2072 656c 6174 696f 6e73 2e0a  , or relations..
+00009240: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00009250: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00009260: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2058  ------.        X
+00009270: 3a20 6e70 2e61 7272 6179 206f 7220 6c69  : np.array or li
+00009280: 7374 0a20 2020 2020 2020 2020 2020 2044  st.            D
+00009290: 6174 6120 746f 2062 6520 696e 6465 7865  ata to be indexe
+000092a0: 642e 0a20 2020 2020 2020 2074 7970 655f  d..        type_
+000092b0: 6f66 3a20 7374 720a 2020 2020 2020 2020  of: str.        
+000092c0: 2020 2020 5370 6563 6966 6965 7320 7768      Specifies wh
+000092d0: 6574 6865 7220 746f 2067 6574 2069 6e64  ether to get ind
+000092e0: 6578 6573 2f72 6177 2064 6174 6120 666f  exes/raw data fo
+000092f0: 7220 7472 6970 6c65 7320 2860 6074 7970  r triples (``typ
+00009300: 655f 6f66 3d27 7427 6060 292c 2065 6e74  e_of='t'``), ent
+00009310: 6974 6965 7320 2860 6074 7970 655f 6f66  ities (``type_of
+00009320: 3d27 6527 6060 292c 0a20 2020 2020 2020  ='e'``),.       
+00009330: 2020 2020 206f 7220 7265 6c61 7469 6f6e       or relation
+00009340: 7320 2860 6074 7970 655f 6f66 3d27 7227  s (``type_of='r'
+00009350: 6060 292e 0a20 2020 2020 2020 206f 7264  ``)..        ord
+00009360: 6572 3a20 7374 720a 2020 2020 2020 2020  er: str.        
+00009370: 2020 2020 5370 6563 6966 6965 7320 7768      Specifies wh
+00009380: 6574 6865 7220 746f 2067 6574 2069 6e64  ether to get ind
+00009390: 6578 6573 2066 726f 6d20 7261 7720 6461  exes from raw da
+000093a0: 7461 2028 6060 6f72 6465 723d 2772 6177  ta (``order='raw
+000093b0: 3269 6e64 2760 6029 206f 720a 2020 2020  2ind'``) or.    
+000093c0: 2020 2020 2020 2020 7261 7720 6461 7461          raw data
+000093d0: 2066 726f 6d20 696e 6465 7865 7320 2860   from indexes (`
+000093e0: 606f 7264 6572 3d27 696e 6432 7261 7727  `order='ind2raw'
+000093f0: 6060 292e 0a0a 2020 2020 2020 2020 5265  ``)...        Re
+00009400: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00009410: 2d2d 2d2d 2d0a 2020 2020 2020 2020 593a  -----.        Y:
+00009420: 206e 702e 6172 7261 790a 2020 2020 2020   np.array.      
+00009430: 2020 2020 2020 496e 6465 7865 6420 6461        Indexed da
+00009440: 7461 206f 7220 7261 7720 6461 7461 2e0a  ta or raw data..
+00009450: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+00009460: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00009470: 0a20 2020 2020 2020 203e 3e3e 2066 726f  .        >>> fro
+00009480: 6d20 616d 706c 6967 7261 7068 2e6c 6174  m ampligraph.lat
+00009490: 656e 745f 6665 6174 7572 6573 2069 6d70  ent_features imp
+000094a0: 6f72 7420 5363 6f72 696e 6742 6173 6564  ort ScoringBased
+000094b0: 456d 6265 6464 696e 674d 6f64 656c 0a20  EmbeddingModel. 
+000094c0: 2020 2020 2020 203e 3e3e 2066 726f 6d20         >>> from 
+000094d0: 616d 706c 6967 7261 7068 2e64 6174 6173  ampligraph.datas
+000094e0: 6574 7320 696d 706f 7274 206c 6f61 645f  ets import load_
+000094f0: 6662 3135 6b5f 3233 370a 2020 2020 2020  fb15k_237.      
+00009500: 2020 3e3e 3e20 5820 3d20 6c6f 6164 5f66    >>> X = load_f
+00009510: 6231 356b 5f32 3337 2829 0a20 2020 2020  b15k_237().     
+00009520: 2020 203e 3e3e 206d 6f64 656c 203d 2053     >>> model = S
+00009530: 636f 7269 6e67 4261 7365 6445 6d62 6564  coringBasedEmbed
+00009540: 6469 6e67 4d6f 6465 6c28 6574 613d 352c  dingModel(eta=5,
+00009550: 0a20 2020 2020 2020 203e 3e3e 2020 2020  .        >>>    
+00009560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009580: 6b3d 3330 302c 0a20 2020 2020 2020 203e  k=300,.        >
+00009590: 3e3e 2020 2020 2020 2020 2020 2020 2020  >>              
+000095a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095b0: 2020 2020 2020 7363 6f72 696e 675f 7479        scoring_ty
+000095c0: 7065 3d27 436f 6d70 6c45 7827 2c0a 2020  pe='ComplEx',.  
+000095d0: 2020 2020 2020 3e3e 3e20 2020 2020 2020        >>>       
+000095e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095f0: 2020 2020 2020 2020 2020 2020 2073 6565               see
+00009600: 643d 3029 0a20 2020 2020 2020 203e 3e3e  d=0).        >>>
+00009610: 206d 6f64 656c 2e63 6f6d 7069 6c65 286f   model.compile(o
+00009620: 7074 696d 697a 6572 3d27 6164 616d 272c  ptimizer='adam',
+00009630: 206c 6f73 733d 276e 6c6c 2729 0a20 2020   loss='nll').   
+00009640: 2020 2020 203e 3e3e 206d 6f64 656c 2e66       >>> model.f
+00009650: 6974 2858 5b27 7472 6169 6e27 5d2c 0a20  it(X['train'],. 
+00009660: 2020 2020 2020 203e 3e3e 2020 2020 2020         >>>      
+00009670: 2020 2020 2062 6174 6368 5f73 697a 653d       batch_size=
+00009680: 3130 3030 302c 0a20 2020 2020 2020 203e  10000,.        >
+00009690: 3e3e 2020 2020 2020 2020 2020 2065 706f  >>           epo
+000096a0: 6368 733d 352c 0a20 2020 2020 2020 203e  chs=5,.        >
+000096b0: 3e3e 2020 2020 2020 2020 2020 2076 6572  >>           ver
+000096c0: 626f 7365 3d46 616c 7365 290a 2020 2020  bose=False).    
+000096d0: 2020 2020 3e3e 3e20 7072 696e 7428 6d6f      >>> print(mo
+000096e0: 6465 6c2e 6765 745f 696e 6465 7865 7328  del.get_indexes(
+000096f0: 5b27 2f6d 2f30 3237 726e 272c 2027 2f6d  ['/m/027rn', '/m
+00009700: 2f30 3676 3873 3027 5d2c 2027 6527 2c20  /06v8s0'], 'e', 
+00009710: 2772 6177 3269 6e64 2729 290a 2020 2020  'raw2ind')).    
+00009720: 2020 2020 3e3e 3e20 7072 696e 7428 6d6f      >>> print(mo
+00009730: 6465 6c2e 6765 745f 696e 6465 7865 7328  del.get_indexes(
+00009740: 5b33 3837 372c 2030 5d2c 2027 6527 2c20  [3877, 0], 'e', 
+00009750: 2769 6e64 3272 6177 2729 290a 2020 2020  'ind2raw')).    
+00009760: 2020 2020 5b30 2c20 3338 3737 5d0a 2020      [0, 3877].  
+00009770: 2020 2020 2020 5b27 2f6d 2f30 3676 3873        ['/m/06v8s
+00009780: 3027 2c20 272f 6d2f 3032 3772 6e27 5d0a  0', '/m/027rn'].
+00009790: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000097a0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000097b0: 6461 7461 5f69 6e64 6578 6572 2e67 6574  data_indexer.get
+000097c0: 5f69 6e64 6578 6573 2858 2c20 7479 7065  _indexes(X, type
+000097d0: 5f6f 662c 206f 7264 6572 290a 0a20 2020  _of, order)..   
+000097e0: 2064 6566 2067 6574 5f63 6f75 6e74 2873   def get_count(s
+000097f0: 656c 662c 2063 6f6e 6365 7074 5f74 7970  elf, concept_typ
+00009800: 653d 2265 2229 3a0a 2020 2020 2020 2020  e="e"):.        
+00009810: 2222 2252 6574 7572 6e73 2074 6865 2063  """Returns the c
+00009820: 6f75 6e74 206f 6620 656e 7469 7469 6573  ount of entities
+00009830: 2061 6e64 2072 656c 6174 696f 6e73 2074   and relations t
+00009840: 6861 7420 7765 7265 2070 7265 7365 6e74  hat were present
+00009850: 2064 7572 696e 6720 7472 6169 6e69 6e67   during training
+00009860: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00009870: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00009880: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00009890: 2063 6f6e 6365 7074 5f74 7970 653a 2073   concept_type: s
+000098a0: 7472 0a20 2020 2020 2020 2020 2020 2049  tr.            I
+000098b0: 6e64 6963 6174 6573 2077 6865 7468 6572  ndicates whether
+000098c0: 2074 6f20 636f 756e 7420 656e 7469 7469   to count entiti
+000098d0: 6573 2028 6060 636f 6e63 6570 745f 7479  es (``concept_ty
+000098e0: 7065 3d27 6527 6060 2920 6f72 0a20 2020  pe='e'``) or.   
+000098f0: 2020 2020 2020 2020 2072 656c 6174 696f           relatio
+00009900: 6e73 2028 6060 636f 6e63 6570 745f 7479  ns (``concept_ty
+00009910: 7065 3d27 7227 6060 2920 2864 6566 6175  pe='r'``) (defau
+00009920: 6c74 3a20 6027 6527 6029 2e0a 0a20 2020  lt: `'e'`)...   
+00009930: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00009940: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00009950: 2020 2020 2063 6f75 6e74 3a20 696e 740a       count: int.
+00009960: 2020 2020 2020 2020 2020 2020 436f 756e              Coun
+00009970: 7420 6f66 2074 6865 2065 6e74 6974 6965  t of the entitie
+00009980: 7320 6f72 2072 656c 6174 696f 6e73 2e0a  s or relations..
+00009990: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+000099a0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000099b0: 0a20 2020 2020 2020 203e 3e3e 2066 726f  .        >>> fro
+000099c0: 6d20 616d 706c 6967 7261 7068 2e64 6174  m ampligraph.dat
+000099d0: 6173 6574 7320 696d 706f 7274 206c 6f61  asets import loa
+000099e0: 645f 6662 3135 6b5f 3233 370a 2020 2020  d_fb15k_237.    
+000099f0: 2020 2020 3e3e 3e20 6672 6f6d 2061 6d70      >>> from amp
+00009a00: 6c69 6772 6170 682e 6c61 7465 6e74 5f66  ligraph.latent_f
+00009a10: 6561 7475 7265 7320 696d 706f 7274 2053  eatures import S
+00009a20: 636f 7269 6e67 4261 7365 6445 6d62 6564  coringBasedEmbed
+00009a30: 6469 6e67 4d6f 6465 6c0a 2020 2020 2020  dingModel.      
+00009a40: 2020 3e3e 3e20 5820 3d20 6c6f 6164 5f66    >>> X = load_f
+00009a50: 6231 356b 5f32 3337 2829 0a20 2020 2020  b15k_237().     
+00009a60: 2020 203e 3e3e 206d 6f64 656c 203d 2053     >>> model = S
+00009a70: 636f 7269 6e67 4261 7365 6445 6d62 6564  coringBasedEmbed
+00009a80: 6469 6e67 4d6f 6465 6c28 6574 613d 352c  dingModel(eta=5,
+00009a90: 0a20 2020 2020 2020 203e 3e3e 2020 2020  .        >>>    
+00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ac0: 6b3d 3330 302c 0a20 2020 2020 2020 203e  k=300,.        >
+00009ad0: 3e3e 2020 2020 2020 2020 2020 2020 2020  >>              
+00009ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009af0: 2020 2020 2020 7363 6f72 696e 675f 7479        scoring_ty
+00009b00: 7065 3d27 436f 6d70 6c45 7827 2c0a 2020  pe='ComplEx',.  
+00009b10: 2020 2020 2020 3e3e 3e20 2020 2020 2020        >>>       
+00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b30: 2020 2020 2020 2020 2020 2020 2073 6565               see
+00009b40: 643d 3029 0a20 2020 2020 2020 203e 3e3e  d=0).        >>>
+00009b50: 206d 6f64 656c 2e63 6f6d 7069 6c65 286f   model.compile(o
+00009b60: 7074 696d 697a 6572 3d27 6164 616d 272c  ptimizer='adam',
+00009b70: 206c 6f73 733d 276e 6c6c 2729 0a20 2020   loss='nll').   
+00009b80: 2020 2020 203e 3e3e 206d 6f64 656c 2e66       >>> model.f
+00009b90: 6974 2858 5b27 7472 6169 6e27 5d2c 0a20  it(X['train'],. 
+00009ba0: 2020 2020 2020 203e 3e3e 2020 2020 2020         >>>      
+00009bb0: 2020 2020 2062 6174 6368 5f73 697a 653d       batch_size=
+00009bc0: 3130 3030 302c 0a20 2020 2020 2020 203e  10000,.        >
+00009bd0: 3e3e 2020 2020 2020 2020 2020 2065 706f  >>           epo
+00009be0: 6368 733d 352c 0a20 2020 2020 2020 203e  chs=5,.        >
+00009bf0: 3e3e 2020 2020 2020 2020 2020 2076 6572  >>           ver
+00009c00: 626f 7365 3d46 616c 7365 290a 2020 2020  bose=False).    
+00009c10: 2020 2020 3e3e 3e20 7072 696e 7428 2745      >>> print('E
+00009c20: 6e74 6974 6965 733a 272c 206d 6f64 656c  ntities:', model
+00009c30: 2e67 6574 5f63 6f75 6e74 2827 6527 2929  .get_count('e'))
+00009c40: 0a20 2020 2020 2020 203e 3e3e 2070 7269  .        >>> pri
+00009c50: 6e74 2827 5265 6c61 7469 6f6e 733a 272c  nt('Relations:',
+00009c60: 206d 6f64 656c 2e67 6574 5f63 6f75 6e74   model.get_count
+00009c70: 2827 7227 2929 0a20 2020 2020 2020 2045  ('r')).        E
+00009c80: 6e74 6974 6965 733a 2031 3435 3035 0a20  ntities: 14505. 
+00009c90: 2020 2020 2020 2052 656c 6174 696f 6e73         Relations
+00009ca0: 3a20 3233 370a 2020 2020 2020 2020 2222  : 237.        ""
+00009cb0: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
+00009cc0: 2073 656c 662e 6973 5f66 6974 7465 642c   self.is_fitted,
+00009cd0: 2022 4d6f 6465 6c20 6973 206e 6f74 2066   "Model is not f
+00009ce0: 6974 206f 6e20 7468 6520 6461 7461 2079  it on the data y
+00009cf0: 6574 2122 0a20 2020 2020 2020 2069 6620  et!".        if 
+00009d00: 636f 6e63 6570 745f 7479 7065 203d 3d20  concept_type == 
+00009d10: 2265 223a 0a20 2020 2020 2020 2020 2020  "e":.           
+00009d20: 2072 6574 7572 6e20 7365 6c66 2e64 6174   return self.dat
+00009d30: 615f 696e 6465 7865 722e 6765 745f 656e  a_indexer.get_en
+00009d40: 7469 7469 6573 5f63 6f75 6e74 2829 0a20  tities_count(). 
+00009d50: 2020 2020 2020 2065 6c69 6620 636f 6e63         elif conc
+00009d60: 6570 745f 7479 7065 203d 3d20 2272 223a  ept_type == "r":
+00009d70: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00009d80: 7572 6e20 7365 6c66 2e64 6174 615f 696e  urn self.data_in
+00009d90: 6465 7865 722e 6765 745f 7265 6c61 7469  dexer.get_relati
+00009da0: 6f6e 735f 636f 756e 7428 290a 2020 2020  ons_count().    
+00009db0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00009dc0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00009dd0: 6545 7272 6f72 2822 496e 7661 6c69 6420  eError("Invalid 
+00009de0: 436f 6e63 6570 7420 5479 7065 2028 6578  Concept Type (ex
+00009df0: 7065 6374 6564 2027 6527 206f 7220 2772  pected 'e' or 'r
+00009e00: 2729 2229 0a0a 2020 2020 6465 6620 6765  ')")..    def ge
+00009e10: 745f 7472 6169 6e5f 656d 6265 6464 696e  t_train_embeddin
+00009e20: 675f 6d61 7472 6978 5f73 697a 6528 7365  g_matrix_size(se
+00009e30: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00009e40: 5265 7475 726e 7320 7468 6520 7369 7a65  Returns the size
+00009e50: 206f 6620 7468 6520 656d 6265 6464 696e   of the embeddin
+00009e60: 6720 6d61 7472 6978 2075 7365 6420 666f  g matrix used fo
+00009e70: 7220 7472 6169 6e69 6e67 2e0a 0a20 2020  r training...   
+00009e80: 2020 2020 2054 6869 7320 6d61 7920 6e6f       This may no
+00009e90: 7420 6265 2073 616d 6520 6173 2028 6e2c  t be same as (n,
+00009ea0: 206b 2920 6475 7269 6e67 2070 6172 7469   k) during parti
+00009eb0: 7469 6f6e 6564 2074 7261 696e 696e 6720  tioned training 
+00009ec0: 2877 6865 7265 2060 6e60 2069 7320 7468  (where `n` is th
+00009ed0: 6520 6e75 6d62 6572 206f 6620 7472 6970  e number of trip
+00009ee0: 6c65 7320 696e 2074 6865 0a20 2020 2020  les in the.     
+00009ef0: 2020 2077 686f 6c65 2074 7261 696e 696e     whole trainin
+00009f00: 6720 7365 7429 2e0a 2020 2020 2020 2020  g set)..        
+00009f10: 2222 220a 2020 2020 2020 2020 6173 7365  """.        asse
+00009f20: 7274 2073 656c 662e 6973 5f66 6974 7465  rt self.is_fitte
+00009f30: 642c 2022 4d6f 6465 6c20 6973 206e 6f74  d, "Model is not
+00009f40: 2066 6974 206f 6e20 7468 6520 6461 7461   fit on the data
+00009f50: 2079 6574 2122 0a20 2020 2020 2020 2072   yet!".        r
+00009f60: 6574 7572 6e20 7b0a 2020 2020 2020 2020  eturn {.        
+00009f70: 2020 2020 2265 223a 2073 656c 662e 656e      "e": self.en
+00009f80: 636f 6469 6e67 5f6c 6179 6572 2e65 6e74  coding_layer.ent
+00009f90: 5f65 6d62 2e73 6861 7065 2c0a 2020 2020  _emb.shape,.    
+00009fa0: 2020 2020 2020 2020 2272 223a 2073 656c          "r": sel
+00009fb0: 662e 656e 636f 6469 6e67 5f6c 6179 6572  f.encoding_layer
+00009fc0: 2e72 656c 5f65 6d62 2e73 6861 7065 2c0a  .rel_emb.shape,.
+00009fd0: 2020 2020 2020 2020 7d0a 0a20 2020 2064          }..    d
+00009fe0: 6566 2073 6176 6528 0a20 2020 2020 2020  ef save(.       
+00009ff0: 2073 656c 662c 0a20 2020 2020 2020 2066   self,.        f
+0000a000: 696c 6570 6174 682c 0a20 2020 2020 2020  ilepath,.       
+0000a010: 206f 7665 7277 7269 7465 3d54 7275 652c   overwrite=True,
+0000a020: 0a20 2020 2020 2020 2069 6e63 6c75 6465  .        include
+0000a030: 5f6f 7074 696d 697a 6572 3d54 7275 652c  _optimizer=True,
+0000a040: 0a20 2020 2020 2020 2073 6176 655f 666f  .        save_fo
+0000a050: 726d 6174 3d4e 6f6e 652c 0a20 2020 2020  rmat=None,.     
+0000a060: 2020 2073 6967 6e61 7475 7265 733d 4e6f     signatures=No
+0000a070: 6e65 2c0a 2020 2020 2020 2020 6f70 7469  ne,.        opti
+0000a080: 6f6e 733d 4e6f 6e65 2c0a 2020 2020 2020  ons=None,.      
+0000a090: 2020 7361 7665 5f74 7261 6365 733d 5472    save_traces=Tr
+0000a0a0: 7565 2c0a 2020 2020 293a 0a20 2020 2020  ue,.    ):.     
+0000a0b0: 2020 2022 2222 5361 7665 2074 6865 206d     """Save the m
+0000a0c0: 6f64 656c 2e22 2222 0a20 2020 2020 2020  odel.""".       
+0000a0d0: 2073 7570 6572 2853 636f 7269 6e67 4261   super(ScoringBa
+0000a0e0: 7365 6445 6d62 6564 6469 6e67 4d6f 6465  sedEmbeddingMode
+0000a0f0: 6c2c 2073 656c 6629 2e73 6176 6528 0a20  l, self).save(. 
+0000a100: 2020 2020 2020 2020 2020 2066 696c 6570             filep
+0000a110: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
+0000a120: 206f 7665 7277 7269 7465 2c0a 2020 2020   overwrite,.    
+0000a130: 2020 2020 2020 2020 696e 636c 7564 655f          include_
+0000a140: 6f70 7469 6d69 7a65 722c 0a20 2020 2020  optimizer,.     
+0000a150: 2020 2020 2020 2073 6176 655f 666f 726d         save_form
+0000a160: 6174 2c0a 2020 2020 2020 2020 2020 2020  at,.            
+0000a170: 7369 676e 6174 7572 6573 2c0a 2020 2020  signatures,.    
+0000a180: 2020 2020 2020 2020 6f70 7469 6f6e 732c          options,
+0000a190: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
+0000a1a0: 655f 7472 6163 6573 2c0a 2020 2020 2020  e_traces,.      
+0000a1b0: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+0000a1c0: 2e73 6176 655f 6d65 7461 6461 7461 2866  .save_metadata(f
+0000a1d0: 696c 6564 6972 3d66 696c 6570 6174 6829  iledir=filepath)
+0000a1e0: 0a0a 2020 2020 6465 6620 7361 7665 5f6d  ..    def save_m
+0000a1f0: 6574 6164 6174 6128 7365 6c66 2c20 6669  etadata(self, fi
+0000a200: 6c65 7061 7468 3d4e 6f6e 652c 2066 696c  lepath=None, fil
+0000a210: 6564 6972 3d4e 6f6e 6529 3a0a 2020 2020  edir=None):.    
+0000a220: 2020 2020 2222 2253 6176 6520 6d65 7461      """Save meta
+0000a230: 6461 7461 2e22 2222 0a20 2020 2020 2020  data.""".       
+0000a240: 2023 2073 746f 7265 2061 6d70 6c69 6772   # store ampligr
+0000a250: 6170 6820 7370 6563 6966 6963 206d 6574  aph specific met
+0000a260: 6164 6174 610a 2020 2020 2020 2020 6966  adata.        if
+0000a270: 2066 696c 6570 6174 6820 6973 206e 6f74   filepath is not
+0000a280: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000a290: 2020 2062 6173 655f 6469 7220 3d20 6f73     base_dir = os
+0000a2a0: 2e70 6174 682e 6469 726e 616d 6528 6669  .path.dirname(fi
+0000a2b0: 6c65 6469 7229 0a20 2020 2020 2020 2020  ledir).         
+0000a2c0: 2020 2062 6173 655f 6469 7220 3d20 222e     base_dir = ".
+0000a2d0: 2220 6966 2062 6173 655f 6469 7220 3d3d  " if base_dir ==
+0000a2e0: 2022 2220 656c 7365 2062 6173 655f 6469   "" else base_di
+0000a2f0: 720a 2020 2020 2020 2020 2020 2020 6669  r.            fi
+0000a300: 6c65 7061 7468 203d 206f 732e 7061 7468  lepath = os.path
+0000a310: 2e62 6173 656e 616d 6528 6669 6c65 7061  .basename(filepa
+0000a320: 7468 290a 0a20 2020 2020 2020 2069 6620  th)..        if 
+0000a330: 6669 6c65 6469 7220 6973 206e 6f74 204e  filedir is not N
+0000a340: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000a350: 2062 6173 655f 6469 7220 3d20 6669 6c65   base_dir = file
+0000a360: 6469 720a 2020 2020 2020 2020 2020 2020  dir.            
+0000a370: 6669 6c65 7061 7468 203d 206f 732e 7061  filepath = os.pa
+0000a380: 7468 2e62 6173 656e 616d 6528 6669 6c65  th.basename(file
+0000a390: 6469 7229 0a0a 2020 2020 2020 2020 7769  dir)..        wi
+0000a3a0: 7468 206f 7065 6e28 0a20 2020 2020 2020  th open(.       
+0000a3b0: 2020 2020 206f 732e 7061 7468 2e6a 6f69       os.path.joi
+0000a3c0: 6e28 6261 7365 5f64 6972 2c20 6669 6c65  n(base_dir, file
+0000a3d0: 7061 7468 202b 2022 5f6d 6574 6164 6174  path + "_metadat
+0000a3e0: 612e 616d 706b 6c22 292c 2022 7762 220a  a.ampkl"), "wb".
+0000a3f0: 2020 2020 2020 2020 2920 6173 2066 3a0a          ) as f:.
+0000a400: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+0000a410: 6461 7461 203d 207b 0a20 2020 2020 2020  data = {.       
+0000a420: 2020 2020 2020 2020 2022 6973 5f70 6172           "is_par
+0000a430: 7469 7469 6f6e 6564 5f74 7261 696e 696e  titioned_trainin
+0000a440: 6722 3a20 7365 6c66 2e69 735f 7061 7274  g": self.is_part
+0000a450: 6974 696f 6e65 645f 7472 6169 6e69 6e67  itioned_training
+0000a460: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a470: 2020 226d 6178 5f65 6e74 5f73 697a 6522    "max_ent_size"
+0000a480: 3a20 7365 6c66 2e6d 6178 5f65 6e74 5f73  : self.max_ent_s
+0000a490: 697a 652c 0a20 2020 2020 2020 2020 2020  ize,.           
+0000a4a0: 2020 2020 2022 6d61 785f 7265 6c5f 7369       "max_rel_si
+0000a4b0: 7a65 223a 2073 656c 662e 6d61 785f 7265  ze": self.max_re
+0000a4c0: 6c5f 7369 7a65 2c0a 2020 2020 2020 2020  l_size,.        
+0000a4d0: 2020 2020 2020 2020 2265 7461 223a 2073          "eta": s
+0000a4e0: 656c 662e 6574 612c 0a20 2020 2020 2020  elf.eta,.       
+0000a4f0: 2020 2020 2020 2020 2022 6b22 3a20 7365           "k": se
+0000a500: 6c66 2e6b 2c0a 2020 2020 2020 2020 2020  lf.k,.          
+0000a510: 2020 2020 2020 2269 735f 6669 7474 6564        "is_fitted
+0000a520: 223a 2073 656c 662e 6973 5f66 6974 7465  ": self.is_fitte
+0000a530: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+0000a540: 2020 2022 6973 5f63 616c 6962 7261 7465     "is_calibrate
+0000a550: 6422 3a20 7365 6c66 2e69 735f 6361 6c69  d": self.is_cali
+0000a560: 6272 6174 6564 2c0a 2020 2020 2020 2020  brated,.        
+0000a570: 2020 2020 2020 2020 2269 735f 6261 636b          "is_back
+0000a580: 7761 7264 223a 2073 656c 662e 6973 5f62  ward": self.is_b
+0000a590: 6163 6b77 6172 642c 0a20 2020 2020 2020  ackward,.       
+0000a5a0: 2020 2020 2020 2020 2022 6461 7461 5f73           "data_s
+0000a5b0: 6861 7065 223a 2073 656c 662e 6461 7461  hape": self.data
+0000a5c0: 5f73 6861 7065 0a20 2020 2020 2020 2020  _shape.         
+0000a5d0: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
+0000a5e0: 2020 6d65 7461 6461 7461 2e75 7064 6174    metadata.updat
+0000a5f0: 6528 7365 6c66 2e64 6174 615f 696e 6465  e(self.data_inde
+0000a600: 7865 722e 6765 745f 7570 6461 7465 5f6d  xer.get_update_m
+0000a610: 6574 6164 6174 6128 6261 7365 5f64 6972  etadata(base_dir
+0000a620: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
+0000a630: 6620 7365 6c66 2e69 735f 7061 7274 6974  f self.is_partit
+0000a640: 696f 6e65 645f 7472 6169 6e69 6e67 3a0a  ioned_training:.
+0000a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a660: 7365 6c66 2e70 6172 7469 7469 6f6e 6572  self.partitioner
+0000a670: 5f6d 6574 6164 6174 6120 3d20 280a 2020  _metadata = (.  
+0000a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a690: 2020 7365 6c66 2e64 6174 615f 6861 6e64    self.data_hand
+0000a6a0: 6c65 722e 6765 745f 7570 6461 7465 5f70  ler.get_update_p
+0000a6b0: 6172 7469 7469 6f6e 6572 5f6d 6574 6164  artitioner_metad
+0000a6c0: 6174 6128 6261 7365 5f64 6972 290a 2020  ata(base_dir).  
+0000a6d0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6f0: 6d65 7461 6461 7461 2e75 7064 6174 6528  metadata.update(
+0000a700: 7365 6c66 2e70 6172 7469 7469 6f6e 6572  self.partitioner
+0000a710: 5f6d 6574 6164 6174 6129 0a0a 2020 2020  _metadata)..    
+0000a720: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000a730: 6973 5f63 616c 6962 7261 7465 643a 0a20  is_calibrated:. 
+0000a740: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000a750: 6574 6164 6174 615b 2263 616c 6962 5f77  etadata["calib_w
+0000a760: 225d 203d 2073 656c 662e 6361 6c69 6272  "] = self.calibr
+0000a770: 6174 696f 6e5f 6c61 7965 722e 6361 6c69  ation_layer.cali
+0000a780: 625f 772e 6e75 6d70 7928 290a 2020 2020  b_w.numpy().    
+0000a790: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+0000a7a0: 6461 7461 5b22 6361 6c69 625f 6222 5d20  data["calib_b"] 
+0000a7b0: 3d20 7365 6c66 2e63 616c 6962 7261 7469  = self.calibrati
+0000a7c0: 6f6e 5f6c 6179 6572 2e63 616c 6962 5f62  on_layer.calib_b
+0000a7d0: 2e6e 756d 7079 2829 0a20 2020 2020 2020  .numpy().       
+0000a7e0: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
+0000a7f0: 615b 2270 6f73 5f73 697a 6522 5d20 3d20  a["pos_size"] = 
+0000a800: 7365 6c66 2e63 616c 6962 7261 7469 6f6e  self.calibration
+0000a810: 5f6c 6179 6572 2e70 6f73 5f73 697a 650a  _layer.pos_size.
+0000a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a830: 6d65 7461 6461 7461 5b22 6e65 675f 7369  metadata["neg_si
+0000a840: 7a65 225d 203d 2073 656c 662e 6361 6c69  ze"] = self.cali
+0000a850: 6272 6174 696f 6e5f 6c61 7965 722e 6e65  bration_layer.ne
+0000a860: 675f 7369 7a65 0a20 2020 2020 2020 2020  g_size.         
+0000a870: 2020 2020 2020 206d 6574 6164 6174 615b         metadata[
+0000a880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a890: 2020 2020 2022 706f 7369 7469 7665 5f62       "positive_b
+0000a8a0: 6173 655f 7261 7465 220a 2020 2020 2020  ase_rate".      
+0000a8b0: 2020 2020 2020 2020 2020 5d20 3d20 7365            ] = se
+0000a8c0: 6c66 2e63 616c 6962 7261 7469 6f6e 5f6c  lf.calibration_l
+0000a8d0: 6179 6572 2e70 6f73 6974 6976 655f 6261  ayer.positive_ba
+0000a8e0: 7365 5f72 6174 650a 2020 2020 2020 2020  se_rate.        
+0000a8f0: 2020 2020 7069 636b 6c65 2e64 756d 7028      pickle.dump(
+0000a900: 6d65 7461 6461 7461 2c20 6629 0a0a 2020  metadata, f)..  
+0000a910: 2020 6465 6620 7361 7665 5f77 6569 6768    def save_weigh
+0000a920: 7473 2873 656c 662c 2066 696c 6570 6174  ts(self, filepat
+0000a930: 682c 206f 7665 7277 7269 7465 3d54 7275  h, overwrite=Tru
+0000a940: 6529 3a0a 2020 2020 2020 2020 2222 2253  e):.        """S
+0000a950: 6176 6520 7468 6520 7472 6169 6e61 626c  ave the trainabl
+0000a960: 6520 7765 6967 6874 732e 0a0a 2020 2020  e weights...    
+0000a970: 2020 2020 2055 7365 2074 6869 7320 6675       Use this fu
+0000a980: 6e63 7469 6f6e 2069 6620 7468 6520 7472  nction if the tr
+0000a990: 6169 6e69 6e67 2070 726f 6365 7373 2069  aining process i
+0000a9a0: 7320 636f 6d70 6c65 7465 2061 6e64 2079  s complete and y
+0000a9b0: 6f75 2077 616e 7420 746f 0a20 2020 2020  ou want to.     
+0000a9c0: 2020 2020 7573 6520 7468 6520 6d6f 6465      use the mode
+0000a9d0: 6c20 6f6e 6c79 2066 6f72 2069 6e66 6572  l only for infer
+0000a9e0: 656e 6365 2e20 5573 6520 3a6d 6574 683a  ence. Use :meth:
+0000a9f0: 606c 6f61 645f 7765 6967 6874 7360 2074  `load_weights` t
+0000aa00: 6f20 6c6f 6164 2074 6865 206d 6f64 656c  o load the model
+0000aa10: 2077 6569 6768 7473 2062 6163 6b2e 0a0a   weights back...
+0000aa20: 2020 2020 2020 2020 202e 2e20 4e6f 7465           .. Note
+0000aa30: 203a 3a0a 2020 2020 2020 2020 2020 2020   ::.            
+0000aa40: 2049 6620 796f 7520 7761 6e74 2074 6f20   If you want to 
+0000aa50: 6265 2061 626c 6520 6f66 2063 6f6e 7469  be able of conti
+0000aa60: 6e75 696e 6720 7468 6520 7472 6169 6e69  nuing the traini
+0000aa70: 6e67 2c20 796f 7520 6361 6e20 7573 6520  ng, you can use 
+0000aa80: 7468 6520 3a6d 6574 683a 6061 6d70 6c69  the :meth:`ampli
+0000aa90: 6772 6170 682e 7574 696c 732e 7361 7665  graph.utils.save
+0000aaa0: 5f6d 6f64 656c 600a 2020 2020 2020 2020  _model`.        
+0000aab0: 2020 2020 2061 6e64 203a 6d65 7468 3a60       and :meth:`
+0000aac0: 616d 706c 6967 7261 7068 2e75 7469 6c73  ampligraph.utils
+0000aad0: 2e72 6573 746f 7265 5f6d 6f64 656c 602e  .restore_model`.
+0000aae0: 5468 6573 6520 6675 6e63 7469 6f6e 7320  These functions 
+0000aaf0: 7361 7665 2061 6e64 2072 6573 746f 7265  save and restore
+0000ab00: 2074 6865 2065 6e74 6972 6520 7374 6174   the entire stat
+0000ab10: 650a 2020 2020 2020 2020 2020 2020 206f  e.             o
+0000ab20: 6620 7468 6520 6772 6170 682c 2077 6869  f the graph, whi
+0000ab30: 6368 2061 6c6c 6f77 7320 746f 2063 6f6e  ch allows to con
+0000ab40: 7469 6e75 6520 7468 6520 7472 6169 6e69  tinue the traini
+0000ab50: 6e67 2066 726f 6d20 7768 6572 6520 6974  ng from where it
+0000ab60: 2077 6173 2073 746f 7070 6564 2e0a 0a20   was stopped... 
+0000ab70: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0000ab80: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000ab90: 2d2d 2d2d 0a20 2020 2020 2020 2066 696c  ----.        fil
+0000aba0: 6570 6174 683a 2073 7472 0a20 2020 2020  epath: str.     
+0000abb0: 2020 2020 2020 2050 6174 6820 746f 2073         Path to s
+0000abc0: 6176 6520 7468 6520 6d6f 6465 6c2e 0a20  ave the model.. 
+0000abd0: 2020 2020 2020 206f 7665 7277 7269 7465         overwrite
+0000abe0: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
+0000abf0: 2020 2046 6c61 6720 7768 6963 6820 696e     Flag which in
+0000ac00: 6469 6361 7465 7320 7768 6574 6865 7220  dicates whether 
+0000ac10: 7468 6520 6d6f 6465 6c2c 2069 6620 7072  the model, if pr
+0000ac20: 6573 656e 742c 206e 6565 6473 2074 6f20  esent, needs to 
+0000ac30: 6265 206f 7665 7277 7269 7474 656e 206f  be overwritten o
+0000ac40: 7220 6e6f 7420 2864 6566 6175 6c74 3a20  r not (default: 
+0000ac50: 6054 7275 6560 292e 0a20 2020 2020 2020  `True`)..       
+0000ac60: 2022 2222 0a20 2020 2020 2020 2023 2054   """.        # T
+0000ac70: 4f44 4f3a 2076 6572 6966 7920 6f74 6865  ODO: verify othe
+0000ac80: 7220 666f 726d 6174 730a 0a20 2020 2020  r formats..     
+0000ac90: 2020 2023 2063 616c 6c20 7468 6520 6261     # call the ba
+0000aca0: 7365 2063 6c61 7373 206d 6574 686f 6420  se class method 
+0000acb0: 746f 2073 6176 6520 7468 6520 7765 6967  to save the weig
+0000acc0: 6874 730a 2020 2020 2020 2020 6966 206e  hts.        if n
+0000acd0: 6f74 2073 656c 662e 6973 5f70 6172 7469  ot self.is_parti
+0000ace0: 7469 6f6e 6564 5f74 7261 696e 696e 673a  tioned_training:
+0000acf0: 0a20 2020 2020 2020 2020 2020 2073 7570  .            sup
+0000ad00: 6572 2853 636f 7269 6e67 4261 7365 6445  er(ScoringBasedE
+0000ad10: 6d62 6564 6469 6e67 4d6f 6465 6c2c 2073  mbeddingModel, s
+0000ad20: 656c 6629 2e73 6176 655f 7765 6967 6874  elf).save_weight
+0000ad30: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+0000ad40: 2020 2066 696c 6570 6174 682c 206f 7665     filepath, ove
+0000ad50: 7277 7269 7465 0a20 2020 2020 2020 2020  rwrite.         
+0000ad60: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+0000ad70: 662e 7361 7665 5f6d 6574 6164 6174 6128  f.save_metadata(
+0000ad80: 6669 6c65 7061 7468 290a 0a20 2020 2064  filepath)..    d
+0000ad90: 6566 2062 7569 6c64 5f66 756c 6c5f 6d6f  ef build_full_mo
+0000ada0: 6465 6c28 7365 6c66 2c20 6261 7463 685f  del(self, batch_
+0000adb0: 7369 7a65 3d31 3030 293a 0a20 2020 2020  size=100):.     
+0000adc0: 2020 2022 2222 5468 6973 206d 6574 686f     """This metho
+0000add0: 6420 6973 2063 616c 6c65 6420 7768 696c  d is called whil
+0000ade0: 6520 6c6f 6164 696e 6720 7468 6520 7765  e loading the we
+0000adf0: 6967 6874 7320 746f 2062 7569 6c64 2074  ights to build t
+0000ae00: 6865 206d 6f64 656c 2e22 2222 0a20 2020  he model.""".   
+0000ae10: 2020 2020 2073 656c 662e 6275 696c 6428       self.build(
+0000ae20: 2862 6174 6368 5f73 697a 652c 2033 2929  (batch_size, 3))
+0000ae30: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+0000ae40: 6e20 7261 6e67 6528 6c65 6e28 7365 6c66  n range(len(self
+0000ae50: 2e6c 6179 6572 7329 293a 0a20 2020 2020  .layers)):.     
+0000ae60: 2020 2020 2020 2073 656c 662e 6c61 7965         self.laye
+0000ae70: 7273 5b69 5d2e 6275 696c 6428 2862 6174  rs[i].build((bat
+0000ae80: 6368 5f73 697a 652c 2033 2929 0a20 2020  ch_size, 3)).   
+0000ae90: 2020 2020 2020 2020 2073 656c 662e 6c61           self.la
+0000aea0: 7965 7273 5b69 5d2e 6275 696c 7420 3d20  yers[i].built = 
+0000aeb0: 5472 7565 0a0a 2020 2020 6465 6620 6c6f  True..    def lo
+0000aec0: 6164 5f6d 6574 6164 6174 6128 7365 6c66  ad_metadata(self
+0000aed0: 2c20 6669 6c65 7061 7468 3d4e 6f6e 652c  , filepath=None,
+0000aee0: 2066 696c 6564 6972 3d4e 6f6e 6529 3a0a   filedir=None):.
+0000aef0: 2020 2020 2020 2020 6966 2066 696c 6564          if filed
+0000af00: 6972 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ir is not None:.
+0000af10: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+0000af20: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
+0000af30: 6f69 6e28 6669 6c65 6469 722c 206f 732e  oin(filedir, os.
+0000af40: 7061 7468 2e62 6173 656e 616d 6528 6669  path.basename(fi
+0000af50: 6c65 6469 7229 290a 0a20 2020 2020 2020  ledir))..       
+0000af60: 2077 6974 6820 6f70 656e 2866 696c 6570   with open(filep
+0000af70: 6174 6820 2b20 225f 6d65 7461 6461 7461  ath + "_metadata
+0000af80: 2e61 6d70 6b6c 222c 2022 7262 2229 2061  .ampkl", "rb") a
+0000af90: 7320 663a 0a20 2020 2020 2020 2020 2020  s f:.           
+0000afa0: 206d 6574 6164 6174 6120 3d20 7069 636b   metadata = pick
+0000afb0: 6c65 2e6c 6f61 6428 6629 0a20 2020 2020  le.load(f).     
+0000afc0: 2020 2020 2020 206d 6574 6164 6174 615b         metadata[
+0000afd0: 2272 6f6f 745f 6469 7265 6374 6f72 7922  "root_directory"
+0000afe0: 5d20 3d20 6f73 2e70 6174 682e 6469 726e  ] = os.path.dirn
+0000aff0: 616d 6528 6669 6c65 7061 7468 290a 2020  ame(filepath).  
+0000b000: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
+0000b010: 7461 5b22 726f 6f74 5f64 6972 6563 746f  ta["root_directo
+0000b020: 7279 225d 203d 2028 0a20 2020 2020 2020  ry"] = (.       
+0000b030: 2020 2020 2020 2020 2022 2e22 0a20 2020           ".".   
+0000b040: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000b050: 6d65 7461 6461 7461 5b22 726f 6f74 5f64  metadata["root_d
+0000b060: 6972 6563 746f 7279 225d 203d 3d20 2222  irectory"] == ""
+0000b070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b080: 2065 6c73 6520 6d65 7461 6461 7461 5b22   else metadata["
+0000b090: 726f 6f74 5f64 6972 6563 746f 7279 225d  root_directory"]
+0000b0a0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000b0b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b0c0: 6261 7365 5f64 6972 203d 206d 6574 6164  base_dir = metad
+0000b0d0: 6174 615b 2272 6f6f 745f 6469 7265 6374  ata["root_direct
+0000b0e0: 6f72 7922 5d0a 2020 2020 2020 2020 2020  ory"].          
+0000b0f0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0000b100: 2020 2020 2020 206d 6574 6164 6174 615b         metadata[
+0000b110: 2264 625f 6669 6c65 225d 203d 206f 732e  "db_file"] = os.
+0000b120: 7061 7468 2e62 6173 656e 616d 6528 6d65  path.basename(me
+0000b130: 7461 6461 7461 5b22 6462 5f66 696c 6522  tadata["db_file"
+0000b140: 5d29 0a20 2020 2020 2020 2020 2020 2065  ]).            e
+0000b150: 7863 6570 7420 4b65 7945 7272 6f72 3a0a  xcept KeyError:.
+0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b170: 7072 696e 7428 2253 6176 6564 206d 6f64  print("Saved mod
+0000b180: 656c 2064 6f65 7320 6e6f 7420 696e 636c  el does not incl
+0000b190: 7564 6520 6120 6462 2066 696c 652e 2053  ude a db file. S
+0000b1a0: 6b69 7070 696e 672e 2229 0a0a 2020 2020  kipping.")..    
+0000b1b0: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
+0000b1c0: 615f 696e 6465 7865 7220 3d20 4461 7461  a_indexer = Data
+0000b1d0: 496e 6465 7865 7228 5b5d 2c20 2a2a 6d65  Indexer([], **me
+0000b1e0: 7461 6461 7461 290a 2020 2020 2020 2020  tadata).        
+0000b1f0: 2020 2020 7365 6c66 2e69 735f 7061 7274      self.is_part
+0000b200: 6974 696f 6e65 645f 7472 6169 6e69 6e67  itioned_training
+0000b210: 203d 206d 6574 6164 6174 615b 2269 735f   = metadata["is_
+0000b220: 7061 7274 6974 696f 6e65 645f 7472 6169  partitioned_trai
+0000b230: 6e69 6e67 225d 0a20 2020 2020 2020 2020  ning"].         
+0000b240: 2020 2073 656c 662e 6d61 785f 656e 745f     self.max_ent_
+0000b250: 7369 7a65 203d 206d 6574 6164 6174 615b  size = metadata[
+0000b260: 226d 6178 5f65 6e74 5f73 697a 6522 5d0a  "max_ent_size"].
+0000b270: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b280: 2e6d 6178 5f72 656c 5f73 697a 6520 3d20  .max_rel_size = 
+0000b290: 6d65 7461 6461 7461 5b22 6d61 785f 7265  metadata["max_re
+0000b2a0: 6c5f 7369 7a65 225d 0a20 2020 2020 2020  l_size"].       
+0000b2b0: 2020 2020 2073 656c 662e 6973 5f66 6974       self.is_fit
+0000b2c0: 7465 6420 3d20 6d65 7461 6461 7461 5b22  ted = metadata["
+0000b2d0: 6973 5f66 6974 7465 6422 5d0a 2020 2020  is_fitted"].    
+0000b2e0: 2020 2020 2020 2020 7365 6c66 2e69 735f          self.is_
+0000b2f0: 6261 636b 7761 7264 203d 206d 6574 6164  backward = metad
+0000b300: 6174 612e 6765 7428 2269 735f 6261 636b  ata.get("is_back
+0000b310: 7761 7264 222c 2046 616c 7365 290a 2020  ward", False).  
+0000b320: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+0000b330: 6174 615f 7368 6170 6520 3d20 6d65 7461  ata_shape = meta
+0000b340: 6461 7461 2e67 6574 2827 6461 7461 5f73  data.get('data_s
+0000b350: 6861 7065 2729 0a20 2020 2020 2020 2020  hape').         
+0000b360: 2020 2069 6620 7365 6c66 2e69 735f 7061     if self.is_pa
+0000b370: 7274 6974 696f 6e65 645f 7472 6169 6e69  rtitioned_traini
+0000b380: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+0000b390: 2020 2020 7365 6c66 2e70 6172 7469 7469      self.partiti
+0000b3a0: 6f6e 6572 5f6b 203d 206d 6574 6164 6174  oner_k = metadat
+0000b3b0: 615b 2270 6172 7469 7469 6f6e 6572 5f6b  a["partitioner_k
+0000b3c0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0000b3d0: 2020 2073 656c 662e 7061 7274 6974 696f     self.partitio
+0000b3e0: 6e65 725f 6d65 7461 6461 7461 203d 207b  ner_metadata = {
+0000b3f0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+0000b400: 2020 7365 6c66 2e70 6172 7469 7469 6f6e    self.partition
+0000b410: 6572 5f6d 6574 6164 6174 615b 2265 6e74  er_metadata["ent
+0000b420: 5f6d 6170 5f66 6e61 6d65 225d 203d 206d  _map_fname"] = m
+0000b430: 6574 6164 6174 615b 0a20 2020 2020 2020  etadata[.       
+0000b440: 2020 2020 2020 2020 2020 2020 2022 656e               "en
+0000b450: 745f 6d61 705f 666e 616d 6522 0a20 2020  t_map_fname".   
+0000b460: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
+0000b470: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000b480: 656c 662e 7061 7274 6974 696f 6e65 725f  elf.partitioner_
+0000b490: 6d65 7461 6461 7461 5b22 7265 6c5f 6d61  metadata["rel_ma
+0000b4a0: 705f 666e 616d 6522 5d20 3d20 6d65 7461  p_fname"] = meta
+0000b4b0: 6461 7461 5b0a 2020 2020 2020 2020 2020  data[.          
+0000b4c0: 2020 2020 2020 2020 2020 2272 656c 5f6d            "rel_m
+0000b4d0: 6170 5f66 6e61 6d65 220a 2020 2020 2020  ap_fname".      
+0000b4e0: 2020 2020 2020 2020 2020 5d0a 0a20 2020            ]..   
+0000b4f0: 2020 2020 2020 2020 2073 656c 662e 6973           self.is
+0000b500: 5f63 616c 6962 7261 7465 6420 3d20 6d65  _calibrated = me
+0000b510: 7461 6461 7461 5b22 6973 5f63 616c 6962  tadata["is_calib
+0000b520: 7261 7465 6422 5d0a 2020 2020 2020 2020  rated"].        
+0000b530: 2020 2020 6966 2073 656c 662e 6973 5f63      if self.is_c
+0000b540: 616c 6962 7261 7465 643a 0a20 2020 2020  alibrated:.     
+0000b550: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b560: 6361 6c69 6272 6174 696f 6e5f 6c61 7965  calibration_laye
+0000b570: 7220 3d20 4361 6c69 6272 6174 696f 6e4c  r = CalibrationL
+0000b580: 6179 6572 280a 2020 2020 2020 2020 2020  ayer(.          
+0000b590: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
+0000b5a0: 7461 5b22 706f 735f 7369 7a65 225d 2c0a  ta["pos_size"],.
+0000b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5c0: 2020 2020 6d65 7461 6461 7461 5b22 6e65      metadata["ne
+0000b5d0: 675f 7369 7a65 225d 2c0a 2020 2020 2020  g_size"],.      
+0000b5e0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+0000b5f0: 7461 6461 7461 5b22 706f 7369 7469 7665  tadata["positive
+0000b600: 5f62 6173 655f 7261 7465 225d 2c0a 2020  _base_rate"],.  
+0000b610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b620: 2020 6361 6c69 625f 773d 6d65 7461 6461    calib_w=metada
+0000b630: 7461 5b22 6361 6c69 625f 7722 5d2c 0a20  ta["calib_w"],. 
+0000b640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b650: 2020 2063 616c 6962 5f62 3d6d 6574 6164     calib_b=metad
+0000b660: 6174 615b 2263 616c 6962 5f62 225d 2c0a  ata["calib_b"],.
+0000b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b680: 290a 0a20 2020 2064 6566 206c 6f61 645f  )..    def load_
+0000b690: 7765 6967 6874 7328 7365 6c66 2c20 6669  weights(self, fi
+0000b6a0: 6c65 7061 7468 293a 0a20 2020 2020 2020  lepath):.       
+0000b6b0: 2022 2222 4c6f 6164 7320 7468 6520 6d6f   """Loads the mo
+0000b6c0: 6465 6c20 7765 6967 6874 732e 0a0a 2020  del weights...  
+0000b6d0: 2020 2020 2020 2055 7365 2074 6869 7320         Use this 
+0000b6e0: 6675 6e63 7469 6f6e 2069 6620 6060 7361  function if ``sa
+0000b6f0: 7665 5f77 6569 6768 7473 6060 2077 6173  ve_weights`` was
+0000b700: 2075 7365 6420 746f 2073 6176 6520 7468   used to save th
+0000b710: 6520 6d6f 6465 6c2e 0a0a 2020 2020 2020  e model...      
+0000b720: 2020 202e 2e20 4e6f 7465 203a 3a0a 2020     .. Note ::.  
+0000b730: 2020 2020 2020 2020 2020 2049 6620 796f             If yo
+0000b740: 7520 7761 6e74 2074 6f20 636f 6e74 696e  u want to contin
+0000b750: 7565 2074 7261 696e 696e 672c 2079 6f75  ue training, you
+0000b760: 2063 616e 2075 7365 2074 6865 203a 6d65   can use the :me
+0000b770: 7468 3a60 616d 706c 6967 7261 7068 2e75  th:`ampligraph.u
+0000b780: 7469 6c73 2e73 6176 655f 6d6f 6465 6c60  tils.save_model`
+0000b790: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
+0000b7a0: 2020 3a6d 6574 683a 6061 6d70 6c69 6772    :meth:`ampligr
+0000b7b0: 6170 682e 7574 696c 732e 6c6f 6164 5f6d  aph.utils.load_m
+0000b7c0: 6f64 656c 602e 2054 6865 7365 2066 756e  odel`. These fun
+0000b7d0: 6374 696f 6e73 2073 6176 6520 7468 6520  ctions save the 
+0000b7e0: 656e 7469 7265 2073 7461 7465 206f 6620  entire state of 
+0000b7f0: 7468 6520 6772 6170 680a 2020 2020 2020  the graph.      
+0000b800: 2020 2020 2020 2077 6869 6368 2061 6c6c         which all
+0000b810: 6f77 7320 746f 2063 6f6e 7469 6e75 6520  ows to continue 
+0000b820: 7468 6520 7472 6169 6e69 6e67 2066 726f  the training fro
+0000b830: 6d20 7768 6572 6520 6974 2073 746f 7070  m where it stopp
+0000b840: 6564 2e0a 0a20 2020 2020 2020 2050 6172  ed...        Par
+0000b850: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+0000b860: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+0000b870: 2020 2066 696c 6570 6174 683a 2073 7472     filepath: str
+0000b880: 0a20 2020 2020 2020 2020 2020 2050 6174  .            Pat
+0000b890: 6820 746f 2073 6176 6520 7468 6520 6d6f  h to save the mo
+0000b8a0: 6465 6c2e 0a20 2020 2020 2020 2022 2222  del..        """
+0000b8b0: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
+0000b8c0: 6164 5f6d 6574 6164 6174 6128 6669 6c65  ad_metadata(file
+0000b8d0: 7061 7468 290a 2020 2020 2020 2020 7365  path).        se
+0000b8e0: 6c66 2e62 7569 6c64 5f66 756c 6c5f 6d6f  lf.build_full_mo
+0000b8f0: 6465 6c28 290a 2020 2020 2020 2020 6966  del().        if
+0000b900: 206e 6f74 2073 656c 662e 6973 5f70 6172   not self.is_par
+0000b910: 7469 7469 6f6e 6564 5f74 7261 696e 696e  titioned_trainin
+0000b920: 673a 0a20 2020 2020 2020 2020 2020 2073  g:.            s
+0000b930: 7570 6572 2853 636f 7269 6e67 4261 7365  uper(ScoringBase
+0000b940: 6445 6d62 6564 6469 6e67 4d6f 6465 6c2c  dEmbeddingModel,
+0000b950: 2073 656c 6629 2e6c 6f61 645f 7765 6967   self).load_weig
+0000b960: 6874 7328 6669 6c65 7061 7468 290a 0a20  hts(filepath).. 
+0000b970: 2020 2064 6566 2063 6f6d 7069 6c65 280a     def compile(.
+0000b980: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000b990: 2020 2020 2020 6f70 7469 6d69 7a65 723d        optimizer=
+0000b9a0: 2261 6461 6d22 2c0a 2020 2020 2020 2020  "adam",.        
+0000b9b0: 6c6f 7373 3d4e 6f6e 652c 0a20 2020 2020  loss=None,.     
+0000b9c0: 2020 2065 6e74 6974 795f 7265 6c61 7469     entity_relati
+0000b9d0: 6f6e 5f69 6e69 7469 616c 697a 6572 3d22  on_initializer="
+0000b9e0: 676c 6f72 6f74 5f75 6e69 666f 726d 222c  glorot_uniform",
+0000b9f0: 0a20 2020 2020 2020 2065 6e74 6974 795f  .        entity_
+0000ba00: 7265 6c61 7469 6f6e 5f72 6567 756c 6172  relation_regular
+0000ba10: 697a 6572 3d4e 6f6e 652c 0a20 2020 2020  izer=None,.     
+0000ba20: 2020 202a 2a6b 7761 7267 730a 2020 2020     **kwargs.    
+0000ba30: 293a 0a20 2020 2020 2020 2022 2222 2043  ):.        """ C
+0000ba40: 6f6d 7069 6c65 2074 6865 206d 6f64 656c  ompile the model
+0000ba50: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0000ba60: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+0000ba70: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+0000ba80: 206f 7074 696d 697a 6572 3a20 7374 7220   optimizer: str 
+0000ba90: 286e 616d 6520 6f66 206f 7074 696d 697a  (name of optimiz
+0000baa0: 6572 2920 6f72 206f 7074 696d 697a 6572  er) or optimizer
+0000bab0: 2069 6e73 7461 6e63 650a 2020 2020 2020   instance.      
+0000bac0: 2020 2020 2020 5468 6520 6f70 7469 6d69        The optimi
+0000bad0: 7a65 7220 7573 6564 2074 6f20 6d69 6e69  zer used to mini
+0000bae0: 6d69 7a65 2074 6865 206c 6f73 7320 6675  mize the loss fu
+0000baf0: 6e63 7469 6f6e 2e20 466f 7220 7072 652d  nction. For pre-
+0000bb00: 6465 6669 6e65 6420 6f70 7469 6f6e 732c  defined options,
+0000bb10: 2063 686f 6f73 6520 6265 7477 6565 6e0a   choose between.
+0000bb20: 2020 2020 2020 2020 2020 2020 6022 7367              `"sg
+0000bb30: 6422 602c 2060 2261 6461 6772 6164 2260  d"`, `"adagrad"`
+0000bb40: 2c20 6022 6164 616d 2260 2c20 6022 726d  , `"adam"`, `"rm
+0000bb50: 7370 726f 7022 602c 2065 7463 2e0a 2020  sprop"`, etc..  
+0000bb60: 2020 2020 2020 2020 2020 5365 6520 6074            See `t
+0000bb70: 662e 6b65 7261 732e 6f70 7469 6d69 7a65  f.keras.optimize
+0000bb80: 7273 203c 6874 7470 733a 2f2f 7777 772e  rs <https://www.
+0000bb90: 7465 6e73 6f72 666c 6f77 2e6f 7267 2f61  tensorflow.org/a
+0000bba0: 7069 5f64 6f63 732f 7079 7468 6f6e 2f74  pi_docs/python/t
+0000bbb0: 662f 6b65 7261 732f 6f70 7469 6d69 7a65  f/keras/optimize
+0000bbc0: 7273 3e60 5f0a 2020 2020 2020 2020 2020  rs>`_.          
+0000bbd0: 2020 666f 7220 7570 2d74 6f2d 6461 7465    for up-to-date
+0000bbe0: 2064 6574 6169 6c73 2e0a 0a20 2020 2020   details...     
+0000bbf0: 2020 2020 2020 2049 6620 6120 7374 7269         If a stri
+0000bc00: 6e67 2069 7320 7061 7373 6564 2c20 7468  ng is passed, th
+0000bc10: 656e 2074 6865 2064 6566 6175 6c74 2070  en the default p
+0000bc20: 6172 616d 6574 6572 7320 6f66 2074 6865  arameters of the
+0000bc30: 206f 7074 696d 697a 6572 2077 696c 6c20   optimizer will 
+0000bc40: 6265 2075 7365 642e 0a0a 2020 2020 2020  be used...      
+0000bc50: 2020 2020 2020 4966 2079 6f75 2077 616e        If you wan
+0000bc60: 7420 746f 2075 7365 2063 7573 746f 6d20  t to use custom 
+0000bc70: 6879 7065 7270 6172 616d 6574 6572 7320  hyperparameters 
+0000bc80: 796f 7520 6e65 6564 2074 6f20 6372 6561  you need to crea
+0000bc90: 7465 2061 6e20 696e 7374 616e 6365 206f  te an instance o
+0000bca0: 6620 7468 6520 6f70 7469 6d69 7a65 7220  f the optimizer 
+0000bcb0: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
+0000bcc0: 7061 7373 2074 6865 2069 6e73 7461 6e63  pass the instanc
+0000bcd0: 6520 746f 2074 6865 2063 6f6d 7069 6c65  e to the compile
+0000bce0: 2066 756e 6374 696f 6e20 3a3a 0a0a 2020   function ::..  
+0000bcf0: 2020 2020 2020 2020 2020 2020 2020 696d                im
+0000bd00: 706f 7274 2074 656e 736f 7266 6c6f 7720  port tensorflow 
+0000bd10: 6173 2074 660a 2020 2020 2020 2020 2020  as tf.          
+0000bd20: 2020 2020 2020 6164 616d 5f6f 7074 203d        adam_opt =
+0000bd30: 2074 662e 6b65 7261 732e 6f70 7469 6d69   tf.keras.optimi
+0000bd40: 7a65 7273 2e41 6461 6d28 6c65 6172 6e69  zers.Adam(learni
+0000bd50: 6e67 5f72 6174 653d 302e 3030 3329 0a20  ng_rate=0.003). 
+0000bd60: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000bd70: 6f64 656c 2e63 6f6d 7069 6c65 286c 6f73  odel.compile(los
+0000bd80: 733d 2770 6169 7277 6973 6527 2c20 6f70  s='pairwise', op
+0000bd90: 7469 6d3d 6164 616d 5f6f 7074 290a 0a20  tim=adam_opt).. 
+0000bda0: 2020 2020 2020 206c 6f73 733a 2073 7472         loss: str
+0000bdb0: 2028 6e61 6d65 206f 6620 6f62 6a65 6374   (name of object
+0000bdc0: 6976 6520 6675 6e63 7469 6f6e 292c 206f  ive function), o
+0000bdd0: 626a 6563 7469 7665 2066 756e 6374 696f  bjective functio
+0000bde0: 6e20 6f72 2060 616d 706c 6967 7261 7068  n or `ampligraph
+0000bdf0: 2e6c 6174 656e 745f 6665 6174 7572 6573  .latent_features
+0000be00: 2e6c 6f73 735f 6675 6e63 7469 6f6e 732e  .loss_functions.
+0000be10: 4c6f 7373 600a 0a20 2020 2020 2020 2020  Loss`..         
+0000be20: 2020 2049 6620 6120 7374 7269 6e67 2069     If a string i
+0000be30: 7320 7061 7373 6564 2c20 796f 7520 6361  s passed, you ca
+0000be40: 6e20 7573 6520 6f6e 6520 6f66 2074 6865  n use one of the
+0000be50: 2066 6f6c 6c6f 7769 6e67 206c 6f73 7365   following losse
+0000be60: 7320 7768 6963 6820 7769 6c6c 2062 6520  s which will be 
+0000be70: 7573 6564 2077 6974 6820 7468 6569 720a  used with their.
+0000be80: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+0000be90: 756c 7420 7365 7474 696e 673a 0a0a 2020  ult setting:..  
+0000bea0: 2020 2020 2020 2020 2020 2d20 6022 7061            - `"pa
+0000beb0: 6972 7769 7365 2260 3a20 2074 6865 206d  irwise"`:  the m
+0000bec0: 6f64 656c 2077 696c 6c20 7573 6520 7468  odel will use th
+0000bed0: 6520 7061 6972 7769 7365 206d 6172 6769  e pairwise margi
+0000bee0: 6e2d 6261 7365 6420 6c6f 7373 2066 756e  n-based loss fun
+0000bef0: 6374 696f 6e2e 0a20 2020 2020 2020 2020  ction..         
+0000bf00: 2020 202d 2060 226e 6c6c 2260 3a20 7468     - `"nll"`: th
+0000bf10: 6520 6d6f 6465 6c20 7769 6c6c 2075 7365  e model will use
+0000bf20: 2074 6865 206e 6567 6174 6976 6520 6c6f   the negative lo
+0000bf30: 7373 206c 696b 656c 6968 6f6f 642e 0a20  ss likelihood.. 
+0000bf40: 2020 2020 2020 2020 2020 202d 2060 2261             - `"a
+0000bf50: 6273 6f6c 7574 655f 6d61 7267 696e 2260  bsolute_margin"`
+0000bf60: 3a20 7468 6520 6d6f 6465 6c20 7769 6c6c  : the model will
+0000bf70: 2075 7365 2074 6865 2061 6273 6f6c 7574   use the absolut
+0000bf80: 6520 6d61 7267 696e 206c 696b 656c 6968  e margin likelih
+0000bf90: 6f6f 642e 0a20 2020 2020 2020 2020 2020  ood..           
+0000bfa0: 202d 2060 2273 656c 665f 6164 7665 7273   - `"self_advers
+0000bfb0: 6172 6961 6c22 603a 2074 6865 206d 6f64  arial"`: the mod
+0000bfc0: 656c 2077 696c 6c20 7573 6520 7468 6520  el will use the 
+0000bfd0: 6164 7665 7273 6172 6961 6c20 7361 6d70  adversarial samp
+0000bfe0: 6c69 6e67 206c 6f73 7320 6675 6e63 7469  ling loss functi
+0000bff0: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
+0000c000: 2d20 6022 6d75 6c74 6963 6c61 7373 5f6e  - `"multiclass_n
+0000c010: 6c6c 2260 3a20 7468 6520 6d6f 6465 6c20  ll"`: the model 
+0000c020: 7769 6c6c 2075 7365 2074 6865 206d 756c  will use the mul
+0000c030: 7469 636c 6173 7320 6e6c 6c20 6c6f 7373  ticlass nll loss
+0000c040: 2e20 3a3a 0a0a 2020 2020 2020 2020 2020  . ::..          
+0000c050: 2020 2020 2020 6d6f 6465 6c2e 636f 6d70        model.comp
+0000c060: 696c 6528 6c6f 7373 3d27 6162 736f 6c75  ile(loss='absolu
+0000c070: 7465 5f6d 6172 6769 6e27 2c20 6f70 7469  te_margin', opti
+0000c080: 6d3d 2761 6461 6d27 290a 0a20 2020 2020  m='adam')..     
+0000c090: 2020 2020 2020 2049 6620 796f 7520 7761         If you wa
+0000c0a0: 6e74 2074 6f20 6d6f 6469 6679 2074 6865  nt to modify the
+0000c0b0: 2064 6566 6175 6c74 2070 6172 616d 6574   default paramet
+0000c0c0: 6572 7320 6f66 2074 6865 206c 6f73 7320  ers of the loss 
+0000c0d0: 6675 6e63 7469 6f6e 2c20 796f 7520 6e65  function, you ne
+0000c0e0: 6564 2074 6f20 6578 706c 6963 746c 7920  ed to explictly 
+0000c0f0: 6372 6561 7465 2061 6e20 696e 7374 616e  create an instan
+0000c100: 6365 0a20 2020 2020 2020 2020 2020 206f  ce.            o
+0000c110: 6620 7468 6520 6c6f 7373 2077 6974 6820  f the loss with 
+0000c120: 7265 7175 6972 6564 2068 7970 6572 7061  required hyperpa
+0000c130: 7261 6d65 7465 7273 2061 6e64 2074 6865  rameters and the
+0000c140: 6e20 7061 7373 2074 6869 7320 696e 7374  n pass this inst
+0000c150: 616e 6365 2e20 3a3a 0a0a 2020 2020 2020  ance. ::..      
+0000c160: 2020 2020 2020 2020 2020 6672 6f6d 2061            from a
+0000c170: 6d70 6c69 6772 6170 682e 6c61 7465 6e74  mpligraph.latent
+0000c180: 5f66 6561 7475 7265 7320 696d 706f 7274  _features import
+0000c190: 2041 6273 6f6c 7574 654d 6172 6769 6e4c   AbsoluteMarginL
+0000c1a0: 6f73 730a 2020 2020 2020 2020 2020 2020  oss.            
+0000c1b0: 2020 2020 6162 5f6c 6f73 7320 3d20 4162      ab_loss = Ab
+0000c1c0: 736f 6c75 7465 4d61 7267 696e 4c6f 7373  soluteMarginLoss
+0000c1d0: 286c 6f73 735f 7061 7261 6d73 3d7b 276d  (loss_params={'m
+0000c1e0: 6172 6769 6e27 3a20 337d 290a 2020 2020  argin': 3}).    
+0000c1f0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+0000c200: 6c2e 636f 6d70 696c 6528 6c6f 7373 3d61  l.compile(loss=a
+0000c210: 625f 6c6f 7373 2c20 6f70 7469 6d3d 2761  b_loss, optim='a
+0000c220: 6461 6d27 290a 0a20 2020 2020 2020 2020  dam')..         
+0000c230: 2020 2041 6e20 6f62 6a65 6374 6976 6520     An objective 
+0000c240: 6675 6e63 7469 6f6e 2069 7320 616e 7920  function is any 
+0000c250: 6361 6c6c 6162 6c65 2077 6974 6820 7468  callable with th
+0000c260: 6520 7369 676e 6174 7572 650a 2020 2020  e signature.    
+0000c270: 2020 2020 2020 2020 6060 6c6f 7373 203d          ``loss =
+0000c280: 2066 6e28 7363 6f72 655f 7472 7565 2c20   fn(score_true, 
+0000c290: 7363 6f72 655f 636f 7272 2c20 6574 6129  score_corr, eta)
+0000c2a0: 6060 203a 3a0a 0a20 2020 2020 2020 2020  `` ::..         
+0000c2b0: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
+0000c2c0: 6120 7573 6572 2064 6566 696e 6564 206c  a user defined l
+0000c2d0: 6f73 7320 6675 6e63 7469 6f6e 2077 6974  oss function wit
+0000c2e0: 6820 7468 6520 6162 6f76 6520 7369 676e  h the above sign
+0000c2f0: 6174 7572 650a 2020 2020 2020 2020 2020  ature.          
+0000c300: 2020 2020 2020 6465 6620 7573 6572 4c6f        def userLo
+0000c310: 7373 2873 636f 7265 735f 706f 732c 2073  ss(scores_pos, s
+0000c320: 636f 7265 735f 6e65 6729 3a0a 2020 2020  cores_neg):.    
+0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c340: 2320 7573 6572 2064 6566 696e 6564 206c  # user defined l
+0000c350: 6f73 7320 2d20 7461 6b65 7320 696e 2032  oss - takes in 2
+0000c360: 2070 6172 616d 7320 616e 6420 7265 7475   params and retu
+0000c370: 726e 7320 6c6f 7373 0a20 2020 2020 2020  rns loss.       
+0000c380: 2020 2020 2020 2020 2020 2020 206e 6567               neg
+0000c390: 5f65 7870 203d 2074 662e 6578 7028 7363  _exp = tf.exp(sc
+0000c3a0: 6f72 6573 5f6e 6567 290a 2020 2020 2020  ores_neg).      
+0000c3b0: 2020 2020 2020 2020 2020 2020 2020 706f                po
+0000c3c0: 735f 6578 7020 3d20 7466 2e65 7870 2873  s_exp = tf.exp(s
+0000c3d0: 636f 7265 735f 706f 7329 0a20 2020 2020  cores_pos).     
+0000c3e0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000c3f0: 2041 7070 6c79 2073 6f66 746d 6178 2074   Apply softmax t
+0000c400: 6f20 7468 6520 7363 6f72 6573 0a20 2020  o the scores.   
+0000c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c420: 2073 636f 7265 203d 2070 6f73 5f65 7870   score = pos_exp
+0000c430: 202f 2028 7466 2e72 6564 7563 655f 7375   / (tf.reduce_su
+0000c440: 6d28 6e65 675f 6578 702c 2061 7869 733d  m(neg_exp, axis=
+0000c450: 3029 202b 2070 6f73 5f65 7870 290a 2020  0) + pos_exp).  
+0000c460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c470: 2020 6c6f 7373 203d 202d 7466 2e6d 6174    loss = -tf.mat
+0000c480: 682e 6c6f 6728 7363 6f72 6529 0a20 2020  h.log(score).   
+0000c490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4a0: 2072 6574 7572 6e20 6c6f 7373 0a20 2020   return loss.   
+0000c4b0: 2020 2020 2020 2020 2020 2020 2023 2050               # P
+0000c4c0: 6173 7320 7468 6973 206c 6f73 7320 7768  ass this loss wh
+0000c4d0: 696c 6520 636f 6d70 696c 696e 6720 7468  ile compiling th
+0000c4e0: 6520 6d6f 6465 6c0a 2020 2020 2020 2020  e model.        
+0000c4f0: 2020 2020 2020 2020 6d6f 6465 6c2e 636f          model.co
+0000c500: 6d70 696c 6528 6c6f 7373 3d75 7365 724c  mpile(loss=userL
+0000c510: 6f73 732c 206f 7074 696d 3d27 6164 616d  oss, optim='adam
+0000c520: 2729 0a0a 2020 2020 2020 2020 656e 7469  ')..        enti
+0000c530: 7479 5f72 656c 6174 696f 6e5f 696e 6974  ty_relation_init
+0000c540: 6961 6c69 7a65 723a 2073 7472 2028 6e61  ializer: str (na
+0000c550: 6d65 206f 6620 696e 6974 6961 6c69 7a65  me of initialize
+0000c560: 7220 6675 6e63 7469 6f6e 292c 2069 6e69  r function), ini
+0000c570: 7469 616c 697a 6572 2066 756e 6374 696f  tializer functio
+0000c580: 6e20 6f72 205c 0a20 2020 2020 2020 2060  n or \.        `
+0000c590: 7466 2e6b 6572 6173 2e69 6e69 7469 616c  tf.keras.initial
+0000c5a0: 697a 6572 732e 496e 6974 6961 6c69 7a65  izers.Initialize
+0000c5b0: 7260 206f 7220 6c69 7374 2e0a 0a20 2020  r` or list...   
+0000c5c0: 2020 2020 2020 2020 2049 6e69 7469 616c           Initial
+0000c5d0: 697a 6572 206f 6620 7468 6520 656e 7469  izer of the enti
+0000c5e0: 7479 2061 6e64 2072 656c 6174 696f 6e20  ty and relation 
+0000c5f0: 656d 6265 6464 696e 6773 2e20 5468 6973  embeddings. This
+0000c600: 2069 7320 6569 7468 6572 2061 2073 696e   is either a sin
+0000c610: 676c 6520 7661 6c75 6520 6f72 2061 206c  gle value or a l
+0000c620: 6973 7420 6f66 2073 697a 6520 322e 0a20  ist of size 2.. 
+0000c630: 2020 2020 2020 2020 2020 2049 6620 6120             If a 
+0000c640: 7369 6e67 6c65 2076 616c 7565 2069 7320  single value is 
+0000c650: 7061 7373 6564 2c20 7468 656e 2062 6f74  passed, then bot
+0000c660: 6820 7468 6520 656e 7469 7469 6573 2061  h the entities a
+0000c670: 6e64 2072 656c 6174 696f 6e73 2077 696c  nd relations wil
+0000c680: 6c20 6265 2069 6e69 7469 616c 697a 6564  l be initialized
+0000c690: 2062 6173 6564 206f 6e0a 2020 2020 2020   based on.      
+0000c6a0: 2020 2020 2020 7468 6520 7361 6d65 2069        the same i
+0000c6b0: 6e69 7469 616c 697a 6572 3b20 6966 2061  nitializer; if a
+0000c6c0: 206c 6973 742c 2074 6865 2066 6972 7374   list, the first
+0000c6d0: 2069 6e69 7469 616c 697a 6572 2077 696c   initializer wil
+0000c6e0: 6c20 6265 2075 7365 6420 666f 7220 656e  l be used for en
+0000c6f0: 7469 7469 6573 2061 6e64 2074 6865 2073  tities and the s
+0000c700: 6563 6f6e 640a 2020 2020 2020 2020 2020  econd.          
+0000c710: 2020 666f 7220 7265 6c61 7469 6f6e 732e    for relations.
+0000c720: 0a0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+0000c730: 2061 2073 7472 696e 6720 6973 2070 6173   a string is pas
+0000c740: 7365 642c 2074 6865 6e20 7468 6520 6465  sed, then the de
+0000c750: 6661 756c 7420 7061 7261 6d65 7465 7273  fault parameters
+0000c760: 2077 696c 6c20 6265 2075 7365 642e 2043   will be used. C
+0000c770: 686f 6f73 6520 6265 7477 6565 6e0a 2020  hoose between.  
+0000c780: 2020 2020 2020 2020 2020 6022 7261 6e64            `"rand
+0000c790: 6f6d 5f6e 6f72 6d61 6c22 602c 2060 2272  om_normal"`, `"r
+0000c7a0: 616e 646f 6d5f 756e 6966 6f72 6d22 602c  andom_uniform"`,
+0000c7b0: 2060 2267 6c6f 726f 745f 6e6f 726d 616c   `"glorot_normal
+0000c7c0: 2260 2c20 6022 6865 5f6e 6f72 6d61 6c22  "`, `"he_normal"
+0000c7d0: 602c 2065 7463 2e0a 0a20 2020 2020 2020  `, etc...       
+0000c7e0: 2020 2020 2053 6565 2060 7466 2e6b 6572       See `tf.ker
+0000c7f0: 6173 2e69 6e69 7469 616c 697a 6572 7320  as.initializers 
+0000c800: 3c68 7474 7073 3a2f 2f77 7777 2e74 656e  <https://www.ten
+0000c810: 736f 7266 6c6f 772e 6f72 672f 6170 695f  sorflow.org/api_
+0000c820: 646f 6373 2f70 7974 686f 6e2f 7466 2f6b  docs/python/tf/k
+0000c830: 6572 6173 2f69 6e69 7469 616c 697a 6572  eras/initializer
+0000c840: 733e 605f 0a20 2020 2020 2020 2020 2020  s>`_.           
+0000c850: 2066 6f72 2075 702d 746f 2d64 6174 6520   for up-to-date 
+0000c860: 6465 7461 696c 732e 203a 3a0a 0a20 2020  details. ::..   
+0000c870: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+0000c880: 656c 2e63 6f6d 7069 6c65 286c 6f73 733d  el.compile(loss=
+0000c890: 2770 6169 7277 6973 6527 2c20 6f70 7469  'pairwise', opti
+0000c8a0: 6d3d 2761 6461 6d27 2c0a 2020 2020 2020  m='adam',.      
+0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8c0: 2020 2020 2020 2020 656e 7469 7479 5f72          entity_r
+0000c8d0: 656c 6174 696f 6e5f 696e 6974 6961 6c69  elation_initiali
+0000c8e0: 7a65 723d 2772 616e 646f 6d5f 6e6f 726d  zer='random_norm
+0000c8f0: 616c 2729 0a0a 2020 2020 2020 2020 2020  al')..          
+0000c900: 2020 4966 2074 6865 2075 7365 7220 7761    If the user wa
+0000c910: 6e74 7320 746f 2075 7365 2063 7573 746f  nts to use custo
+0000c920: 6d20 6879 7065 7270 6172 616d 6574 6572  m hyperparameter
+0000c930: 732c 2074 6865 6e20 616e 2069 6e73 7461  s, then an insta
+0000c940: 6e63 6520 6f66 2074 6865 0a20 2020 2020  nce of the.     
+0000c950: 2020 2020 2020 2060 6074 662e 6b65 7261         ``tf.kera
+0000c960: 732e 696e 6974 6961 6c69 7a65 7273 2e49  s.initializers.I
+0000c970: 6e69 7469 616c 697a 6572 6060 206e 6565  nitializer`` nee
+0000c980: 6473 2074 6f20 6265 2070 6173 7365 642e  ds to be passed.
+0000c990: 203a 3a0a 0a20 2020 2020 2020 2020 2020   ::..           
+0000c9a0: 2020 2020 2069 6d70 6f72 7420 7465 6e73       import tens
+0000c9b0: 6f72 666c 6f77 2061 7320 7466 0a20 2020  orflow as tf.   
+0000c9c0: 2020 2020 2020 2020 2020 2020 2069 6e69               ini
+0000c9d0: 7420 3d20 7466 2e6b 6572 6173 2e69 6e69  t = tf.keras.ini
+0000c9e0: 7469 616c 697a 6572 732e 5261 6e64 6f6d  tializers.Random
+0000c9f0: 4e6f 726d 616c 2873 7464 6465 763d 302e  Normal(stddev=0.
+0000ca00: 3030 3030 3329 0a20 2020 2020 2020 2020  00003).         
+0000ca10: 2020 2020 2020 206d 6f64 656c 2e63 6f6d         model.com
+0000ca20: 7069 6c65 286c 6f73 733d 2770 6169 7277  pile(loss='pairw
+0000ca30: 6973 6527 2c20 6f70 7469 6d3d 2761 6461  ise', optim='ada
+0000ca40: 6d27 2c0a 2020 2020 2020 2020 2020 2020  m',.            
+0000ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca60: 2020 656e 7469 7479 5f72 656c 6174 696f    entity_relatio
+0000ca70: 6e5f 696e 6974 6961 6c69 7a65 723d 696e  n_initializer=in
+0000ca80: 6974 290a 0a20 2020 2020 2020 2020 2020  it)..           
+0000ca90: 2049 6620 7468 6520 7573 6572 2077 616e   If the user wan
+0000caa0: 7473 2074 6f20 6465 6669 6e65 2063 7573  ts to define cus
+0000cab0: 746f 6d20 696e 6974 6961 6c69 7a65 7220  tom initializer 
+0000cac0: 6974 2063 616e 2062 6520 616e 7920 6361  it can be any ca
+0000cad0: 6c6c 6162 6c65 2077 6974 6820 7468 6520  llable with the 
+0000cae0: 7369 676e 6174 7572 6520 6069 6e69 7420  signature `init 
+0000caf0: 3d20 666e 2873 6861 7065 2960 203a 3a0a  = fn(shape)` ::.
+0000cb00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cb10: 2064 6566 206d 795f 696e 6974 2873 6861   def my_init(sha
+0000cb20: 7065 293a 0a20 2020 2020 2020 2020 2020  pe):.           
+0000cb30: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000cb40: 7466 2e72 616e 646f 6d2e 6e6f 726d 616c  tf.random.normal
+0000cb50: 2873 6861 7065 290a 2020 2020 2020 2020  (shape).        
+0000cb60: 2020 2020 2020 2020 6d6f 6465 6c2e 636f          model.co
+0000cb70: 6d70 696c 6528 6c6f 7373 3d27 7061 6972  mpile(loss='pair
+0000cb80: 7769 7365 272c 206f 7074 696d 3d27 6164  wise', optim='ad
+0000cb90: 616d 272c 0a20 2020 2020 2020 2020 2020  am',.           
+0000cba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbb0: 2020 2065 6e74 6974 795f 7265 6c61 7469     entity_relati
+0000cbc0: 6f6e 5f69 6e69 7469 616c 697a 6572 3d6d  on_initializer=m
+0000cbd0: 795f 696e 6974 290a 0a20 2020 2020 2020  y_init)..       
+0000cbe0: 2065 6e74 6974 795f 7265 6c61 7469 6f6e   entity_relation
+0000cbf0: 5f72 6567 756c 6172 697a 6572 3a20 7374  _regularizer: st
+0000cc00: 7220 286e 616d 6520 6f66 2072 6567 756c  r (name of regul
+0000cc10: 6172 697a 6572 2066 756e 6374 696f 6e29  arizer function)
+0000cc20: 206f 7220 7265 6775 6c61 7269 7a65 7220   or regularizer 
+0000cc30: 6675 6e63 7469 6f6e 206f 7220 5c0a 2020  function or \.  
+0000cc40: 2020 2020 2020 6074 662e 6b65 7261 732e        `tf.keras.
+0000cc50: 7265 6775 6c61 7269 7a65 7273 2e52 6567  regularizers.Reg
+0000cc60: 756c 6172 697a 6572 6020 696e 7374 616e  ularizer` instan
+0000cc70: 6365 206f 7220 6c69 7374 0a20 2020 2020  ce or list.     
+0000cc80: 2020 2020 2020 2052 6567 756c 6172 697a         Regulariz
+0000cc90: 6572 206f 6620 656e 7469 7469 6573 2061  er of entities a
+0000cca0: 6e64 2072 656c 6174 696f 6e73 2e0a 2020  nd relations..  
+0000ccb0: 2020 2020 2020 2020 2020 4966 2061 2073            If a s
+0000ccc0: 696e 676c 6520 7661 6c75 6520 6973 2070  ingle value is p
+0000ccd0: 6173 7365 642c 2074 6865 6e20 626f 7468  assed, then both
+0000cce0: 2074 6865 2065 6e74 6974 6965 7320 616e   the entities an
+0000ccf0: 6420 7265 6c61 7469 6f6e 7320 7769 6c6c  d relations will
+0000cd00: 2062 6520 7265 6775 6c61 7269 7a65 6420   be regularized 
+0000cd10: 6261 7365 6420 6f6e 0a20 2020 2020 2020  based on.       
+0000cd20: 2020 2020 2074 6865 2073 616d 6520 7265       the same re
+0000cd30: 6775 6c61 7269 7a65 723b 2069 6620 6120  gularizer; if a 
+0000cd40: 6c69 7374 2c20 7468 6520 6669 7273 7420  list, the first 
+0000cd50: 7265 6775 6c61 7269 7a65 7220 7769 6c6c  regularizer will
+0000cd60: 2062 6520 7573 6564 2066 6f72 2065 6e74   be used for ent
+0000cd70: 6974 6965 7320 616e 6420 7365 636f 6e64  ities and second
+0000cd80: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000cd90: 2072 656c 6174 696f 6e73 2e0a 0a20 2020   relations...   
+0000cda0: 2020 2020 2020 2020 2049 6620 6120 7374           If a st
+0000cdb0: 7269 6e67 2069 7320 7061 7373 6564 2c20  ring is passed, 
+0000cdc0: 7468 656e 2074 6865 2064 6566 6175 6c74  then the default
+0000cdd0: 2070 6172 616d 6574 6572 7320 6f66 2074   parameters of t
+0000cde0: 6865 2072 6567 756c 6172 697a 6572 7320  he regularizers 
+0000cdf0: 7769 6c6c 2062 6520 7573 6564 2e20 4368  will be used. Ch
+0000ce00: 6f6f 7365 2062 6574 7765 656e 0a20 2020  oose between.   
+0000ce10: 2020 2020 2020 2020 2060 226c 3122 602c           `"l1"`,
+0000ce20: 2060 226c 3222 602c 2060 226c 315f 6c32   `"l2"`, `"l1_l2
+0000ce30: 2260 2c20 6574 632e 0a0a 2020 2020 2020  "`, etc...      
+0000ce40: 2020 2020 2020 5365 6520 6074 662e 6b65        See `tf.ke
+0000ce50: 7261 732e 7265 6775 6c61 7269 7a65 7273  ras.regularizers
+0000ce60: 203c 6874 7470 733a 2f2f 7777 772e 7465   <https://www.te
+0000ce70: 6e73 6f72 666c 6f77 2e6f 7267 2f61 7069  nsorflow.org/api
+0000ce80: 5f64 6f63 732f 7079 7468 6f6e 2f74 662f  _docs/python/tf/
+0000ce90: 6b65 7261 732f 7265 6775 6c61 7269 7a65  keras/regularize
+0000cea0: 7273 3e60 5f0a 2020 2020 2020 2020 2020  rs>`_.          
+0000ceb0: 2020 666f 7220 7570 2d74 6f2d 6461 7465    for up-to-date
+0000cec0: 2064 6574 6169 6c73 2e20 3a3a 0a0a 2020   details. ::..  
+0000ced0: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+0000cee0: 6465 6c2e 636f 6d70 696c 6528 6c6f 7373  del.compile(loss
+0000cef0: 3d27 7061 6972 7769 7365 272c 206f 7074  ='pairwise', opt
+0000cf00: 696d 3d27 6164 616d 272c 0a20 2020 2020  im='adam',.     
+0000cf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf20: 2020 2020 2020 2020 2065 6e74 6974 795f           entity_
+0000cf30: 7265 6c61 7469 6f6e 5f72 6567 756c 6172  relation_regular
+0000cf40: 697a 6572 3d27 6c32 2729 0a0a 2020 2020  izer='l2')..    
+0000cf50: 2020 2020 2020 2020 4966 2074 6865 2075          If the u
+0000cf60: 7365 7220 7761 6e74 7320 746f 2075 7365  ser wants to use
+0000cf70: 2063 7573 746f 6d20 6879 7065 7270 6172   custom hyperpar
+0000cf80: 616d 6574 6572 732c 2074 6865 6e20 616e  ameters, then an
+0000cf90: 2069 6e73 7461 6e63 6520 6f66 2074 6865   instance of the
+0000cfa0: 0a20 2020 2020 2020 2020 2020 2060 6074  .            ``t
+0000cfb0: 662e 6b65 7261 732e 7265 6775 6c61 7269  f.keras.regulari
+0000cfc0: 7a65 7273 2e52 6567 756c 6172 697a 6572  zers.Regularizer
+0000cfd0: 6060 206e 6565 6473 2074 6f20 6265 2070  `` needs to be p
+0000cfe0: 6173 7365 642e 203a 3a0a 0a20 2020 2020  assed. ::..     
+0000cff0: 2020 2020 2020 2020 2020 2069 6d70 6f72             impor
+0000d000: 7420 7465 6e73 6f72 666c 6f77 2061 7320  t tensorflow as 
+0000d010: 7466 0a20 2020 2020 2020 2020 2020 2020  tf.             
+0000d020: 2020 2072 6567 203d 2074 662e 6b65 7261     reg = tf.kera
+0000d030: 732e 7265 6775 6c61 7269 7a65 7273 2e4c  s.regularizers.L
+0000d040: 314c 3228 6c31 3d30 2e30 3031 2c20 6c32  1L2(l1=0.001, l2
+0000d050: 3d30 2e31 290a 2020 2020 2020 2020 2020  =0.1).          
+0000d060: 2020 2020 2020 6d6f 6465 6c2e 636f 6d70        model.comp
+0000d070: 696c 6528 6c6f 7373 3d27 7061 6972 7769  ile(loss='pairwi
+0000d080: 7365 272c 206f 7074 696d 3d27 6164 616d  se', optim='adam
+0000d090: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0b0: 2065 6e74 6974 795f 7265 6c61 7469 6f6e   entity_relation
+0000d0c0: 5f72 6567 756c 6172 697a 6572 3d72 6567  _regularizer=reg
+0000d0d0: 290a 0a20 2020 2020 2020 2020 2020 2049  )..            I
+0000d0e0: 6620 7468 6520 7573 6572 2077 616e 7473  f the user wants
+0000d0f0: 2074 6f20 6465 6669 6e65 2063 7573 746f   to define custo
+0000d100: 6d20 7265 6775 6c61 7269 7a65 7220 6974  m regularizer it
+0000d110: 2063 616e 2062 6520 616e 7920 6361 6c6c   can be any call
+0000d120: 6162 6c65 2077 6974 6820 7369 676e 6174  able with signat
+0000d130: 7572 650a 2020 2020 2020 2020 2020 2020  ure.            
+0000d140: 6060 7265 6720 3d20 666e 2877 6569 6768  ``reg = fn(weigh
+0000d150: 745f 6d61 7472 6978 2960 602e 203a 3a0a  t_matrix)``. ::.
+0000d160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d170: 2064 6566 206d 795f 7265 6728 7765 6967   def my_reg(weig
+0000d180: 6874 5f6d 7829 3a0a 2020 2020 2020 2020  ht_mx):.        
+0000d190: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000d1a0: 7475 726e 2030 2e30 3120 2a20 7466 2e6d  turn 0.01 * tf.m
+0000d1b0: 6174 682e 7265 6475 6365 5f73 756d 2874  ath.reduce_sum(t
+0000d1c0: 662e 6d61 7468 2e61 6273 2877 6569 6768  f.math.abs(weigh
+0000d1d0: 745f 6d78 2929 0a20 2020 2020 2020 2020  t_mx)).         
+0000d1e0: 2020 2020 2020 206d 6f64 656c 2e63 6f6d         model.com
+0000d1f0: 7069 6c65 286c 6f73 733d 2770 6169 7277  pile(loss='pairw
+0000d200: 6973 6527 2c20 6f70 7469 6d3d 2761 6461  ise', optim='ada
+0000d210: 6d27 2c0a 2020 2020 2020 2020 2020 2020  m',.            
 0000d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d240: 2020 206b 3d33 3030 2c0a 2020 2020 2020     k=300,.      
-0000d250: 2020 3e3e 3e20 2020 2020 2020 2020 2020    >>>           
-0000d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d270: 2020 2020 2020 2020 2073 636f 7269 6e67           scoring
-0000d280: 5f74 7970 653d 2743 6f6d 706c 4578 272c  _type='ComplEx',
-0000d290: 0a20 2020 2020 2020 203e 3e3e 2020 2020  .        >>>    
-0000d2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2c0: 7365 6564 3d30 290a 2020 2020 2020 2020  seed=0).        
-0000d2d0: 3e3e 3e20 6d6f 6465 6c2e 636f 6d70 696c  >>> model.compil
-0000d2e0: 6528 6f70 7469 6d69 7a65 723d 2761 6461  e(optimizer='ada
-0000d2f0: 6d27 2c20 6c6f 7373 3d27 6e6c 6c27 290a  m', loss='nll').
-0000d300: 2020 2020 2020 2020 3e3e 3e20 6d6f 6465          >>> mode
-0000d310: 6c2e 6669 7428 585b 2774 7261 696e 275d  l.fit(X['train']
-0000d320: 2c0a 2020 2020 2020 2020 3e3e 3e20 2020  ,.        >>>   
-0000d330: 2020 2020 2020 2020 6261 7463 685f 7369          batch_si
-0000d340: 7a65 3d31 3030 3030 2c0a 2020 2020 2020  ze=10000,.      
-0000d350: 2020 3e3e 3e20 2020 2020 2020 2020 2020    >>>           
-0000d360: 6570 6f63 6873 3d35 290a 2020 2020 2020  epochs=5).      
-0000d370: 2020 4570 6f63 6820 312f 350a 2020 2020    Epoch 1/5.    
-0000d380: 2020 2020 3239 2f32 3920 5b3d 3d3d 3d3d      29/29 [=====
-0000d390: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000d3a0: 3d3d 3d3d 3d3d 3d3d 3d5d 202d 2032 7320  =========] - 2s 
-0000d3b0: 3631 6d73 2f73 7465 7020 2d20 6c6f 7373  61ms/step - loss
-0000d3c0: 3a20 3637 3336 312e 3330 3437 0a20 2020  : 67361.3047.   
-0000d3d0: 2020 2020 2045 706f 6368 2032 2f35 0a20       Epoch 2/5. 
-0000d3e0: 2020 2020 2020 2032 392f 3239 205b 3d3d         29/29 [==
-0000d3f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000d400: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 5d20 2d20  ============] - 
-0000d410: 3173 2033 356d 732f 7374 6570 202d 206c  1s 35ms/step - l
-0000d420: 6f73 733a 2036 3733 3138 2e36 3039 340a  oss: 67318.6094.
-0000d430: 2020 2020 2020 2020 4570 6f63 6820 332f          Epoch 3/
-0000d440: 350a 2020 2020 2020 2020 3239 2f32 3920  5.        29/29 
-0000d450: 5b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  [===============
-0000d460: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d5d  ===============]
-0000d470: 202d 2031 7320 3334 6d73 2f73 7465 7020   - 1s 34ms/step 
-0000d480: 2d20 6c6f 7373 3a20 3637 3032 302e 3037  - loss: 67020.07
-0000d490: 3033 0a20 2020 2020 2020 2045 706f 6368  03.        Epoch
-0000d4a0: 2034 2f35 0a20 2020 2020 2020 2032 392f   4/5.        29/
-0000d4b0: 3239 205b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  29 [============
-0000d4c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000d4d0: 3d3d 5d20 2d20 3173 2033 346d 732f 7374  ==] - 1s 34ms/st
-0000d4e0: 6570 202d 206c 6f73 733a 2036 3538 3637  ep - loss: 65867
-0000d4f0: 2e33 3735 300a 2020 2020 2020 2020 4570  .3750.        Ep
-0000d500: 6f63 6820 352f 350a 2020 2020 2020 2020  och 5/5.        
-0000d510: 3239 2f32 3920 5b3d 3d3d 3d3d 3d3d 3d3d  29/29 [=========
-0000d520: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000d530: 3d3d 3d3d 3d5d 202d 2031 7320 3334 6d73  =====] - 1s 34ms
-0000d540: 2f73 7465 7020 2d20 6c6f 7373 3a20 3633  /step - loss: 63
-0000d550: 3531 372e 3930 3632 0a0a 2020 2020 2020  517.9062..      
-0000d560: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
-0000d570: 6765 7420 7468 6520 6f70 7469 6d69 7a65  get the optimize
-0000d580: 720a 2020 2020 2020 2020 7365 6c66 2e6f  r.        self.o
-0000d590: 7074 696d 697a 6572 203d 206f 7074 696d  ptimizer = optim
-0000d5a0: 697a 6572 732e 6765 7428 6f70 7469 6d69  izers.get(optimi
-0000d5b0: 7a65 7229 0a20 2020 2020 2020 2073 656c  zer).        sel
-0000d5c0: 662e 5f72 756e 5f65 6167 6572 6c79 203d  f._run_eagerly =
-0000d5d0: 206b 7761 7267 732e 706f 7028 2272 756e   kwargs.pop("run
-0000d5e0: 5f65 6167 6572 6c79 222c 204e 6f6e 6529  _eagerly", None)
-0000d5f0: 0a20 2020 2020 2020 2023 2072 6573 6574  .        # reset
-0000d600: 2074 6865 2074 7261 696e 696e 672f 6576   the training/ev
-0000d610: 616c 7561 7465 2f70 7265 6469 6374 2066  aluate/predict f
-0000d620: 756e 6374 696f 6e0a 2020 2020 2020 2020  unction.        
-0000d630: 7365 6c66 2e5f 7265 7365 745f 636f 6d70  self._reset_comp
-0000d640: 696c 655f 6361 6368 6528 290a 0a20 2020  ile_cache()..   
-0000d650: 2020 2020 2023 2067 6574 2074 6865 206c       # get the l
-0000d660: 6f73 730a 2020 2020 2020 2020 7365 6c66  oss.        self
-0000d670: 2e63 6f6d 7069 6c65 645f 6c6f 7373 203d  .compiled_loss =
-0000d680: 206c 6f73 735f 6675 6e63 7469 6f6e 732e   loss_functions.
-0000d690: 6765 7428 6c6f 7373 290a 2020 2020 2020  get(loss).      
-0000d6a0: 2020 2320 4f6e 6c79 206d 6574 7269 6320    # Only metric 
-0000d6b0: 7375 7070 6f72 7465 6420 6475 7269 6e67  supported during
-0000d6c0: 2074 6865 2074 7261 696e 696e 6720 6973   the training is
-0000d6d0: 206d 6561 6e20 4c6f 7373 0a20 2020 2020   mean Loss.     
-0000d6e0: 2020 2073 656c 662e 636f 6d70 696c 6564     self.compiled
-0000d6f0: 5f6d 6574 7269 6373 203d 2063 6f6d 7069  _metrics = compi
-0000d700: 6c65 5f75 7469 6c73 2e4d 6574 7269 6373  le_utils.Metrics
-0000d710: 436f 6e74 6169 6e65 7228 0a20 2020 2020  Container(.     
-0000d720: 2020 2020 2020 206d 6574 7269 6373 5f6d         metrics_m
-0000d730: 6f64 2e4d 6561 6e28 6e61 6d65 3d22 6c6f  od.Mean(name="lo
-0000d740: 7373 2229 2c20 4e6f 6e65 2c20 4e6f 6e65  ss"), None, None
-0000d750: 0a20 2020 2020 2020 2029 2020 2320 546f  .        )  # To
-0000d760: 7461 6c20 6c6f 7373 2e0a 0a20 2020 2020  tal loss...     
-0000d770: 2020 2023 2073 6574 2074 6865 2069 6e69     # set the ini
-0000d780: 7469 616c 697a 6572 2061 6e64 2072 6567  tializer and reg
-0000d790: 756c 6172 697a 6572 206f 6620 7468 6520  ularizer of the 
-0000d7a0: 656d 6265 6464 696e 6720 6d61 7472 6963  embedding matric
-0000d7b0: 6573 2069 6e20 7468 650a 2020 2020 2020  es in the.      
-0000d7c0: 2020 2320 656e 636f 6469 6e67 206c 6179    # encoding lay
-0000d7d0: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
-0000d7e0: 656e 636f 6469 6e67 5f6c 6179 6572 2e73  encoding_layer.s
-0000d7f0: 6574 5f69 6e69 7469 616c 697a 6572 2865  et_initializer(e
-0000d800: 6e74 6974 795f 7265 6c61 7469 6f6e 5f69  ntity_relation_i
-0000d810: 6e69 7469 616c 697a 6572 290a 2020 2020  nitializer).    
-0000d820: 2020 2020 7365 6c66 2e65 6e63 6f64 696e      self.encodin
-0000d830: 675f 6c61 7965 722e 7365 745f 7265 6775  g_layer.set_regu
-0000d840: 6c61 7269 7a65 7228 656e 7469 7479 5f72  larizer(entity_r
-0000d850: 656c 6174 696f 6e5f 7265 6775 6c61 7269  elation_regulari
-0000d860: 7a65 7229 0a20 2020 2020 2020 2073 656c  zer).        sel
-0000d870: 662e 5f69 735f 636f 6d70 696c 6564 203d  f._is_compiled =
-0000d880: 2054 7275 650a 0a20 2020 2040 7072 6f70   True..    @prop
-0000d890: 6572 7479 0a20 2020 2064 6566 206d 6574  erty.    def met
-0000d8a0: 7269 6373 2873 656c 6629 3a0a 2020 2020  rics(self):.    
-0000d8b0: 2020 2020 2222 2252 6574 7572 6e73 2061      """Returns a
-0000d8c0: 6c6c 2074 6865 206d 6574 7269 6373 2074  ll the metrics t
-0000d8d0: 6861 7420 7769 6c6c 2062 6520 636f 6d70  hat will be comp
-0000d8e0: 7574 6564 2064 7572 696e 6720 7472 6169  uted during trai
-0000d8f0: 6e69 6e67 2e22 2222 0a20 2020 2020 2020  ning.""".       
-0000d900: 206d 6574 7269 6373 203d 205b 5d0a 2020   metrics = [].  
-0000d910: 2020 2020 2020 6966 2073 656c 662e 5f69        if self._i
-0000d920: 735f 636f 6d70 696c 6564 3a0a 2020 2020  s_compiled:.    
-0000d930: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000d940: 636f 6d70 696c 6564 5f6c 6f73 7320 6973  compiled_loss is
-0000d950: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000d960: 2020 2020 2020 2020 2020 206d 6574 7269             metri
-0000d970: 6373 202b 3d20 7365 6c66 2e63 6f6d 7069  cs += self.compi
-0000d980: 6c65 645f 6c6f 7373 2e6d 6574 7269 6373  led_loss.metrics
-0000d990: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000d9a0: 6d65 7472 6963 730a 0a20 2020 2064 6566  metrics..    def
-0000d9b0: 2067 6574 5f65 6d62 5f6d 6174 7269 785f   get_emb_matrix_
-0000d9c0: 7465 7374 2873 656c 662c 2070 6172 745f  test(self, part_
-0000d9d0: 6e75 6d62 6572 3d31 2c20 6e75 6d62 6572  number=1, number
-0000d9e0: 5f6f 665f 7061 7274 733d 3129 3a0a 2020  _of_parts=1):.  
-0000d9f0: 2020 2020 2020 2222 2247 6574 2074 6865        """Get the
-0000da00: 2065 6d62 6564 6469 6e67 206d 6174 7269   embedding matri
-0000da10: 7820 6475 7269 6e67 2065 7661 6c75 6174  x during evaluat
-0000da20: 696f 6e2e 0a0a 2020 2020 2020 2020 5061  ion...        Pa
-0000da30: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-0000da40: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0000da50: 2020 2020 7061 7274 206e 756d 6265 723a      part number:
-0000da60: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
-0000da70: 2053 7065 6369 6669 6573 2077 6869 6368   Specifies which
-0000da80: 2070 6172 7420 746f 2072 6574 7572 6e20   part to return 
-0000da90: 6672 6f6d 2074 6865 2060 606e 756d 6265  from the ``numbe
-0000daa0: 725f 6f66 5f70 6172 7473 6060 2069 6e20  r_of_parts`` in 
-0000dab0: 7768 6963 6820 7468 6520 656e 7469 7265  which the entire
-0000dac0: 2065 6d62 6564 6469 6e67 206d 6174 7269   embedding matri
-0000dad0: 7820 6973 2073 706c 6974 2e0a 2020 2020  x is split..    
-0000dae0: 2020 2020 6e75 6d62 6572 5f6f 665f 7061      number_of_pa
-0000daf0: 7274 733a 2069 6e74 0a20 2020 2020 2020  rts: int.       
-0000db00: 2020 2020 2054 6f74 616c 206e 756d 6265       Total numbe
-0000db10: 7220 6f66 2070 6172 7473 2069 6e20 7768  r of parts in wh
-0000db20: 6963 6820 746f 2073 706c 6974 2074 6865  ich to split the
-0000db30: 2065 6d62 6564 6469 6e67 206d 6174 7269   embedding matri
-0000db40: 782e 0a0a 2020 2020 2020 2020 5265 7475  x...        Retu
-0000db50: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-0000db60: 2d2d 2d0a 2020 2020 2020 2020 656d 625f  ---.        emb_
-0000db70: 6d61 7472 6978 3a20 6e70 2e61 7272 6179  matrix: np.array
-0000db80: 2c20 7368 6170 6520 286e 2c6b 290a 2020  , shape (n,k).  
-0000db90: 2020 2020 2020 2020 2020 5061 7274 206f            Part o
-0000dba0: 6620 7468 6520 656d 6265 6464 696e 6720  f the embedding 
-0000dbb0: 6d61 7472 6978 2063 6f72 7265 7370 6f6e  matrix correspon
-0000dbc0: 6469 6e67 2074 6f20 6070 6172 745f 6e75  ding to `part_nu
-0000dbd0: 6d62 6572 602e 0a20 2020 2020 2020 2073  mber`..        s
-0000dbe0: 7461 7274 5f69 6e64 6578 3a20 696e 740a  tart_index: int.
-0000dbf0: 2020 2020 2020 2020 2020 2020 4f72 6967              Orig
-0000dc00: 696e 616c 2065 6e74 6974 7920 696e 6465  inal entity inde
-0000dc10: 7820 2864 6174 6120 6469 6374 2920 6f66  x (data dict) of
-0000dc20: 2074 6865 2066 6972 7374 2072 6f77 206f   the first row o
-0000dc30: 6620 7468 6520 6065 6d62 5f6d 6174 7269  f the `emb_matri
-0000dc40: 7860 2e0a 2020 2020 2020 2020 656e 645f  x`..        end_
-0000dc50: 696e 6465 783a 2069 6e74 0a20 2020 2020  index: int.     
-0000dc60: 2020 2020 2020 204f 7269 6769 6e61 6c20         Original 
-0000dc70: 656e 7469 7479 2069 6e64 6578 2028 6461  entity index (da
-0000dc80: 7461 2064 6963 7429 206f 6620 7468 6520  ta dict) of the 
-0000dc90: 6c61 7374 2072 6f77 206f 6620 7468 6520  last row of the 
-0000dca0: 6065 6d62 5f6d 6174 7269 7860 2e0a 0a20  `emb_matrix`... 
-0000dcb0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000dcc0: 2020 2069 6620 6e75 6d62 6572 5f6f 665f     if number_of_
-0000dcd0: 7061 7274 7320 3d3d 2031 3a0a 2020 2020  parts == 1:.    
-0000dce0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000dcf0: 656e 7469 7469 6573 5f73 7562 7365 742e  entities_subset.
-0000dd00: 7368 6170 655b 305d 2021 3d20 303a 0a20  shape[0] != 0:. 
-0000dd10: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0000dd20: 7574 203d 2074 662e 6e6e 2e65 6d62 6564  ut = tf.nn.embed
-0000dd30: 6469 6e67 5f6c 6f6f 6b75 7028 0a20 2020  ding_lookup(.   
-0000dd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd50: 2073 656c 662e 656e 636f 6469 6e67 5f6c   self.encoding_l
-0000dd60: 6179 6572 2e65 6e74 5f65 6d62 2c20 7365  ayer.ent_emb, se
-0000dd70: 6c66 2e65 6e74 6974 6965 735f 7375 6273  lf.entities_subs
-0000dd80: 6574 0a20 2020 2020 2020 2020 2020 2020  et.             
-0000dd90: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000dda0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000ddb0: 2020 2020 2020 206f 7574 203d 2073 656c         out = sel
-0000ddc0: 662e 656e 636f 6469 6e67 5f6c 6179 6572  f.encoding_layer
-0000ddd0: 2e65 6e74 5f65 6d62 0a20 2020 2020 2020  .ent_emb.       
-0000dde0: 2020 2020 2072 6574 7572 6e20 6f75 742c       return out,
-0000ddf0: 2030 2c20 6f75 742e 7368 6170 655b 305d   0, out.shape[0]
-0000de00: 202d 2031 0a20 2020 2020 2020 2065 6c73   - 1.        els
-0000de10: 653a 0a20 2020 2020 2020 2020 2020 2077  e:.            w
-0000de20: 6974 6820 7368 656c 7665 2e6f 7065 6e28  ith shelve.open(
-0000de30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000de40: 2073 656c 662e 7061 7274 6974 696f 6e65   self.partitione
-0000de50: 725f 6d65 7461 6461 7461 5b22 656e 745f  r_metadata["ent_
-0000de60: 6d61 705f 666e 616d 6522 5d0a 2020 2020  map_fname"].    
-0000de70: 2020 2020 2020 2020 2920 6173 2065 6e74          ) as ent
-0000de80: 5f70 6172 7469 7469 6f6e 3a0a 2020 2020  _partition:.    
-0000de90: 2020 2020 2020 2020 2020 2020 6261 7463              batc
-0000dea0: 685f 7369 7a65 203d 2069 6e74 280a 2020  h_size = int(.  
-0000deb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dec0: 2020 6e70 2e63 6569 6c28 6c65 6e28 656e    np.ceil(len(en
-0000ded0: 745f 7061 7274 6974 696f 6e2e 6b65 7973  t_partition.keys
-0000dee0: 2829 2920 2f20 6e75 6d62 6572 5f6f 665f  ()) / number_of_
-0000def0: 7061 7274 7329 0a20 2020 2020 2020 2020  parts).         
-0000df00: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000df10: 2020 2020 2020 2020 2069 6e64 6963 6573           indices
-0000df20: 203d 206e 702e 6172 616e 6765 280a 2020   = np.arange(.  
-0000df30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df40: 2020 7061 7274 5f6e 756d 6265 7220 2a20    part_number * 
-0000df50: 6261 7463 685f 7369 7a65 2c20 2870 6172  batch_size, (par
-0000df60: 745f 6e75 6d62 6572 202b 2031 2920 2a20  t_number + 1) * 
-0000df70: 6261 7463 685f 7369 7a65 0a20 2020 2020  batch_size.     
-0000df80: 2020 2020 2020 2020 2020 2029 2e61 7374             ).ast
-0000df90: 7970 6528 7374 7229 0a20 2020 2020 2020  ype(str).       
-0000dfa0: 2020 2020 2020 2020 2065 6d62 5f6d 6174           emb_mat
-0000dfb0: 7269 7820 3d20 5b5d 0a20 2020 2020 2020  rix = [].       
-0000dfc0: 2020 2020 2020 2020 2066 6f72 2069 6478           for idx
-0000dfd0: 2069 6e20 696e 6469 6365 733a 0a20 2020   in indices:.   
-0000dfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dff0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0000e000: 2020 2020 2020 2020 2020 2020 2020 656d                em
-0000e010: 625f 6d61 7472 6978 2e61 7070 656e 6428  b_matrix.append(
-0000e020: 656e 745f 7061 7274 6974 696f 6e5b 6964  ent_partition[id
-0000e030: 785d 290a 2020 2020 2020 2020 2020 2020  x]).            
-0000e040: 2020 2020 2020 2020 6578 6365 7074 204b          except K
-0000e050: 6579 4572 726f 723a 0a20 2020 2020 2020  eyError:.       
-0000e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e070: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
-0000e080: 2020 2020 2020 2072 6574 7572 6e20 6e70         return np
-0000e090: 2e61 7272 6179 2865 6d62 5f6d 6174 7269  .array(emb_matri
-0000e0a0: 7829 2c20 696e 7428 696e 6469 6365 735b  x), int(indices[
-0000e0b0: 305d 292c 2069 6e74 2869 6e64 6963 6573  0]), int(indices
-0000e0c0: 5b2d 315d 290a 0a20 2020 2064 6566 206d  [-1])..    def m
-0000e0d0: 616b 655f 7465 7374 5f66 756e 6374 696f  ake_test_functio
-0000e0e0: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
-0000e0f0: 2022 2222 5369 6d69 6c61 7220 746f 206b   """Similar to k
-0000e100: 6572 6173 206c 6962 2c20 7468 6973 2066  eras lib, this f
-0000e110: 756e 6374 696f 6e20 7265 7475 726e 7320  unction returns 
-0000e120: 7468 6520 6861 6e64 6c65 2074 6f20 7465  the handle to te
-0000e130: 7374 2073 7465 7020 6675 6e63 7469 6f6e  st step function
-0000e140: 2e0a 0a20 2020 2020 2020 2049 7420 7072  ...        It pr
-0000e150: 6f63 6573 7365 7320 6f6e 6520 6261 7463  ocesses one batc
-0000e160: 6820 6f66 2064 6174 6120 6279 2069 7465  h of data by ite
-0000e170: 7261 7469 6e67 206f 7665 7220 7468 6520  rating over the 
-0000e180: 6461 7461 7365 7420 6974 6572 6174 6f72  dataset iterator
-0000e190: 2061 6e64 2063 6f6d 7075 7465 7320 7468   and computes th
-0000e1a0: 6520 7465 7374 206d 6574 7269 6373 2e0a  e test metrics..
-0000e1b0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000e1c0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000e1d0: 0a20 2020 2020 2020 206f 7574 3a20 4675  .        out: Fu
-0000e1e0: 6e63 7469 6f6e 2068 616e 646c 650a 2020  nction handle.  
-0000e1f0: 2020 2020 2020 2020 2020 2020 4861 6e64              Hand
-0000e200: 6c65 2074 6f20 7468 6520 7465 7374 2073  le to the test s
-0000e210: 7465 7020 6675 6e63 7469 6f6e 2e0a 2020  tep function..  
-0000e220: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-0000e230: 2020 2023 2069 6620 7365 6c66 2e74 6573     # if self.tes
-0000e240: 745f 6675 6e63 7469 6f6e 2069 7320 6e6f  t_function is no
-0000e250: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000e260: 2320 2020 2072 6574 7572 6e20 7365 6c66  #    return self
-0000e270: 2e74 6573 745f 6675 6e63 7469 6f6e 0a0a  .test_function..
-0000e280: 2020 2020 2020 2020 6465 6620 7465 7374          def test
-0000e290: 5f66 756e 6374 696f 6e28 6974 6572 6174  _function(iterat
-0000e2a0: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
-0000e2b0: 2023 2074 6f74 616c 206e 756d 6265 7220   # total number 
-0000e2c0: 6f66 2070 6172 7473 2069 6e20 7768 6963  of parts in whic
-0000e2d0: 6820 746f 2073 706c 6974 2074 6865 2065  h to split the e
-0000e2e0: 6d62 6564 6469 6e67 206d 6174 7269 780a  mbedding matrix.
-0000e2f0: 2020 2020 2020 2020 2020 2020 2320 2864              # (d
-0000e300: 6566 6175 6c74 2031 2c20 692e 652e 2c20  efault 1, i.e., 
-0000e310: 7573 6520 6675 6c6c 206d 6174 7269 7820  use full matrix 
-0000e320: 6173 2069 7420 6973 290a 2020 2020 2020  as it is).      
-0000e330: 2020 2020 2020 6e75 6d62 6572 5f6f 665f        number_of_
-0000e340: 7061 7274 7320 3d20 310a 0a20 2020 2020  parts = 1..     
-0000e350: 2020 2020 2020 2023 2069 6620 6974 2069         # if it i
-0000e360: 7320 7061 7274 6974 696f 6e65 6420 7472  s partitioned tr
-0000e370: 6169 6e69 6e67 0a20 2020 2020 2020 2020  aining.         
-0000e380: 2020 2069 6620 7365 6c66 2e69 735f 7061     if self.is_pa
-0000e390: 7274 6974 696f 6e65 645f 7472 6169 6e69  rtitioned_traini
-0000e3a0: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
-0000e3b0: 2020 2020 2320 7370 6c69 7420 7468 6520      # split the 
-0000e3c0: 656d 6220 6d61 7472 6978 2062 6173 6564  emb matrix based
-0000e3d0: 206f 6e20 6e75 6d62 6572 206f 6620 6275   on number of bu
-0000e3e0: 636b 6574 730a 2020 2020 2020 2020 2020  ckets.          
-0000e3f0: 2020 2020 2020 6e75 6d62 6572 5f6f 665f        number_of_
-0000e400: 7061 7274 7320 3d20 7365 6c66 2e70 6172  parts = self.par
-0000e410: 7469 7469 6f6e 6572 5f6b 0a0a 2020 2020  titioner_k..    
-0000e420: 2020 2020 2020 2020 6461 7461 203d 206e          data = n
-0000e430: 6578 7428 6974 6572 6174 6f72 290a 2020  ext(iterator).  
-0000e440: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000e450: 662e 7573 655f 6669 6c74 6572 3a0a 2020  f.use_filter:.  
-0000e460: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000e470: 7075 7473 2c20 6669 6c74 6572 7320 3d20  puts, filters = 
-0000e480: 6461 7461 5b30 5d2c 2064 6174 615b 315d  data[0], data[1]
-0000e490: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000e4a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000e4b0: 2020 2069 6620 7365 6c66 2e64 6174 615f     if self.data_
-0000e4c0: 7368 6170 6520 3e20 333a 0a20 2020 2020  shape > 3:.     
-0000e4d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000e4e0: 6e70 7574 732c 2066 696c 7465 7273 203d  nputs, filters =
-0000e4f0: 2064 6174 615b 0a20 2020 2020 2020 2020   data[.         
-0000e500: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-0000e510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e520: 2020 2020 205d 2c20 7466 2e52 6167 6765       ], tf.Ragge
-0000e530: 6454 656e 736f 722e 6672 6f6d 5f72 6f77  dTensor.from_row
-0000e540: 5f6c 656e 6774 6873 285b 5d2c 205b 5d29  _lengths([], [])
-0000e550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e560: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000e570: 2020 2020 2020 2020 2020 2069 6e70 7574             input
-0000e580: 732c 2066 696c 7465 7273 203d 2064 6174  s, filters = dat
-0000e590: 612c 2074 662e 5261 6767 6564 5465 6e73  a, tf.RaggedTens
-0000e5a0: 6f72 2e66 726f 6d5f 726f 775f 6c65 6e67  or.from_row_leng
-0000e5b0: 7468 7328 0a20 2020 2020 2020 2020 2020  ths(.           
-0000e5c0: 2020 2020 2020 2020 2020 2020 205b 5d2c               [],
-0000e5d0: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
-0000e5e0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000e5f0: 2020 2020 2020 2023 2063 6f6d 7075 7465         # compute
-0000e600: 2074 6865 206f 7574 7075 7420 7368 6170   the output shap
-0000e610: 6520 6261 7365 6420 6f6e 2074 6865 2074  e based on the t
-0000e620: 7970 6520 6f66 2063 6f72 7275 7074 696f  ype of corruptio
-0000e630: 6e73 2074 6f20 6265 0a20 2020 2020 2020  ns to be.       
-0000e640: 2020 2020 2023 2075 7365 640a 2020 2020       # used.    
-0000e650: 2020 2020 2020 2020 6f75 7470 7574 5f73          output_s
-0000e660: 6861 7065 203d 2030 0a20 2020 2020 2020  hape = 0.       
-0000e670: 2020 2020 2069 6620 2273 2220 696e 2073       if "s" in s
-0000e680: 656c 662e 636f 7272 7570 745f 7369 6465  elf.corrupt_side
-0000e690: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e6a0: 2020 6f75 7470 7574 5f73 6861 7065 202b    output_shape +
-0000e6b0: 3d20 310a 0a20 2020 2020 2020 2020 2020  = 1..           
-0000e6c0: 2069 6620 226f 2220 696e 2073 656c 662e   if "o" in self.
-0000e6d0: 636f 7272 7570 745f 7369 6465 3a0a 2020  corrupt_side:.  
-0000e6e0: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-0000e6f0: 7470 7574 5f73 6861 7065 202b 3d20 310a  tput_shape += 1.
-0000e700: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
-0000e710: 7265 6174 6520 616e 2061 7272 6179 2074  reate an array t
-0000e720: 6f20 7374 6f72 6520 7468 6520 7261 6e6b  o store the rank
-0000e730: 7320 6261 7365 6420 6f6e 206f 7574 7075  s based on outpu
-0000e740: 7420 7368 6170 650a 2020 2020 2020 2020  t shape.        
-0000e750: 2020 2020 6f76 6572 616c 6c5f 7261 6e6b      overall_rank
-0000e760: 203d 2074 662e 7a65 726f 7328 0a20 2020   = tf.zeros(.   
-0000e770: 2020 2020 2020 2020 2020 2020 2028 6f75               (ou
-0000e780: 7470 7574 5f73 6861 7065 2c20 7466 2e73  tput_shape, tf.s
-0000e790: 6861 7065 2869 6e70 7574 7329 5b30 5d29  hape(inputs)[0])
-0000e7a0: 2c20 6474 7970 653d 6e70 2e69 6e74 3332  , dtype=np.int32
-0000e7b0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-0000e7c0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000e7d0: 656c 662e 6973 5f70 6172 7469 7469 6f6e  elf.is_partition
-0000e7e0: 6564 5f74 7261 696e 696e 673a 0a20 2020  ed_training:.   
-0000e7f0: 2020 2020 2020 2020 2020 2020 2069 6e70               inp
-0000e800: 7574 7320 3d20 7365 6c66 2e70 726f 6365  uts = self.proce
-0000e810: 7373 5f6d 6f64 656c 5f69 6e70 7574 735f  ss_model_inputs_
-0000e820: 666f 725f 7465 7374 2869 6e70 7574 7329  for_test(inputs)
-0000e830: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000e840: 7275 6e20 7468 6520 6c6f 6f70 2062 6173  run the loop bas
-0000e850: 6564 206f 6e20 6e75 6d62 6572 206f 6620  ed on number of 
-0000e860: 7061 7274 7320 696e 2077 6869 6368 2074  parts in which t
-0000e870: 6865 206f 7269 6769 6e61 6c20 656d 620a  he original emb.
-0000e880: 2020 2020 2020 2020 2020 2020 2320 6d61              # ma
-0000e890: 7472 6978 2077 6173 2067 656e 6572 6174  trix was generat
-0000e8a0: 6564 0a20 2020 2020 2020 2020 2020 2066  ed.            f
-0000e8b0: 6f72 206a 2069 6e20 7261 6e67 6528 6e75  or j in range(nu
-0000e8c0: 6d62 6572 5f6f 665f 7061 7274 7329 3a0a  mber_of_parts):.
-0000e8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8e0: 2320 6765 7420 7468 6520 656d 6265 6464  # get the embedd
-0000e8f0: 696e 6720 6d61 7472 6978 2061 6c6f 6e67  ing matrix along
-0000e900: 2077 6974 6820 656e 7469 7479 2069 6473   with entity ids
-0000e910: 206f 6620 6669 7273 7420 616e 640a 2020   of first and.  
-0000e920: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000e930: 6c61 7374 2072 6f77 206f 6620 656d 6220  last row of emb 
-0000e940: 6d61 7472 6978 0a20 2020 2020 2020 2020  matrix.         
-0000e950: 2020 2020 2020 2065 6d62 5f6d 6174 2c20         emb_mat, 
-0000e960: 7374 6172 745f 656e 745f 6964 2c20 656e  start_ent_id, en
-0000e970: 645f 656e 745f 6964 203d 2073 656c 662e  d_ent_id = self.
-0000e980: 6765 745f 656d 625f 6d61 7472 6978 5f74  get_emb_matrix_t
-0000e990: 6573 7428 0a20 2020 2020 2020 2020 2020  est(.           
-0000e9a0: 2020 2020 2020 2020 206a 2c20 6e75 6d62           j, numb
-0000e9b0: 6572 5f6f 665f 7061 7274 730a 2020 2020  er_of_parts.    
-0000e9c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000e9d0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000e9e0: 636f 6d70 7574 6520 7468 6520 7261 6e6b  compute the rank
-0000e9f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ea00: 2072 616e 6b73 203d 2073 656c 662e 5f67   ranks = self._g
-0000ea10: 6574 5f72 616e 6b73 280a 2020 2020 2020  et_ranks(.      
-0000ea20: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000ea30: 7075 7473 2c0a 2020 2020 2020 2020 2020  puts,.          
-0000ea40: 2020 2020 2020 2020 2020 656d 625f 6d61            emb_ma
-0000ea50: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-0000ea60: 2020 2020 2020 2073 7461 7274 5f65 6e74         start_ent
-0000ea70: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-0000ea80: 2020 2020 2020 2020 2065 6e64 5f65 6e74           end_ent
-0000ea90: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-0000eaa0: 2020 2020 2020 2020 2066 696c 7465 7273           filters
-0000eab0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000eac0: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
-0000ead0: 6e67 5f64 6963 742c 0a20 2020 2020 2020  ng_dict,.       
-0000eae0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000eaf0: 662e 636f 7272 7570 745f 7369 6465 2c0a  f.corrupt_side,.
-0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb10: 2020 2020 7365 6c66 2e72 616e 6b69 6e67      self.ranking
-0000eb20: 5f73 7472 6174 6567 792c 0a20 2020 2020  _strategy,.     
-0000eb30: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000eb40: 2020 2020 2020 2020 2020 2020 2023 2073               # s
-0000eb50: 746f 7265 2069 7420 696e 2074 6865 206f  tore it in the o
-0000eb60: 7574 7075 740a 2020 2020 2020 2020 2020  utput.          
-0000eb70: 2020 2020 2020 666f 7220 6920 696e 2074        for i in t
-0000eb80: 662e 7261 6e67 6528 6f75 7470 7574 5f73  f.range(output_s
-0000eb90: 6861 7065 293a 0a20 2020 2020 2020 2020  hape):.         
-0000eba0: 2020 2020 2020 2020 2020 206f 7665 7261             overa
-0000ebb0: 6c6c 5f72 616e 6b20 3d20 7466 2e74 656e  ll_rank = tf.ten
-0000ebc0: 736f 725f 7363 6174 7465 725f 6e64 5f61  sor_scatter_nd_a
-0000ebd0: 6464 280a 2020 2020 2020 2020 2020 2020  dd(.            
-0000ebe0: 2020 2020 2020 2020 2020 2020 6f76 6572              over
-0000ebf0: 616c 6c5f 7261 6e6b 2c20 5b5b 695d 5d2c  all_rank, [[i]],
-0000ec00: 205b 7261 6e6b 735b 692c 203a 5d5d 0a20   [ranks[i, :]]. 
-0000ec10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec20: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-0000ec30: 2020 6f76 6572 616c 6c5f 7261 6e6b 203d    overall_rank =
-0000ec40: 2074 662e 7472 616e 7370 6f73 6528 0a20   tf.transpose(. 
-0000ec50: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000ec60: 662e 7265 7368 6170 6528 6f76 6572 616c  f.reshape(overal
-0000ec70: 6c5f 7261 6e6b 2c20 286f 7574 7075 745f  l_rank, (output_
-0000ec80: 7368 6170 652c 202d 3129 290a 2020 2020  shape, -1)).    
-0000ec90: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000eca0: 2020 2020 2020 2320 6966 2063 6f72 7275        # if corru
-0000ecb0: 7074 696f 6e20 7479 7065 2069 7320 732b  ption type is s+
-0000ecc0: 6f20 7468 656e 2061 6464 2073 2061 6e64  o then add s and
-0000ecd0: 206f 2072 616e 6b73 2061 6e64 2072 6574   o ranks and ret
-0000ece0: 7572 6e20 7468 650a 2020 2020 2020 2020  urn the.        
-0000ecf0: 2020 2020 2320 6164 6465 6420 7261 6e6b      # added rank
-0000ed00: 730a 2020 2020 2020 2020 2020 2020 6966  s.            if
-0000ed10: 2073 656c 662e 636f 7272 7570 745f 7369   self.corrupt_si
-0000ed20: 6465 203d 3d20 2273 2b6f 223a 0a20 2020  de == "s+o":.   
-0000ed30: 2020 2020 2020 2020 2020 2020 2023 2061               # a
-0000ed40: 6464 2074 6865 2073 7562 6a65 6374 2061  dd the subject a
-0000ed50: 6e64 206f 626a 6563 7420 7261 6e6b 730a  nd object ranks.
-0000ed60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed70: 6f76 6572 616c 6c5f 7261 6e6b 203d 2074  overall_rank = t
-0000ed80: 662e 7265 6475 6365 5f73 756d 286f 7665  f.reduce_sum(ove
-0000ed90: 7261 6c6c 5f72 616e 6b2c 2031 290a 2020  rall_rank, 1).  
-0000eda0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000edb0: 7265 7475 726e 2074 6865 2061 6464 6564  return the added
-0000edc0: 2072 616e 6b73 0a20 2020 2020 2020 2020   ranks.         
-0000edd0: 2020 2020 2020 2072 6574 7572 6e20 7466         return tf
-0000ede0: 2e72 6573 6861 7065 286f 7665 7261 6c6c  .reshape(overall
-0000edf0: 5f72 616e 6b2c 2028 2d31 2c20 3129 290a  _rank, (-1, 1)).
-0000ee00: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000ee10: 7572 6e20 6f76 6572 616c 6c5f 7261 6e6b  urn overall_rank
-0000ee20: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-0000ee30: 2073 656c 662e 7275 6e5f 6561 6765 726c   self.run_eagerl
-0000ee40: 7920 616e 6420 6e6f 7420 7365 6c66 2e69  y and not self.i
-0000ee50: 735f 7061 7274 6974 696f 6e65 645f 7472  s_partitioned_tr
-0000ee60: 6169 6e69 6e67 3a0a 2020 2020 2020 2020  aining:.        
-0000ee70: 2020 2020 7465 7374 5f66 756e 6374 696f      test_functio
-0000ee80: 6e20 3d20 6465 665f 6675 6e63 7469 6f6e  n = def_function
-0000ee90: 2e66 756e 6374 696f 6e28 0a20 2020 2020  .function(.     
-0000eea0: 2020 2020 2020 2020 2020 2074 6573 745f             test_
-0000eeb0: 6675 6e63 7469 6f6e 2c20 6578 7065 7269  function, experi
-0000eec0: 6d65 6e74 616c 5f72 656c 6178 5f73 6861  mental_relax_sha
-0000eed0: 7065 733d 5472 7565 0a20 2020 2020 2020  pes=True.       
-0000eee0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000eef0: 7365 6c66 2e74 6573 745f 6675 6e63 7469  self.test_functi
-0000ef00: 6f6e 203d 2074 6573 745f 6675 6e63 7469  on = test_functi
-0000ef10: 6f6e 0a0a 2020 2020 2020 2020 7265 7475  on..        retu
-0000ef20: 726e 2073 656c 662e 7465 7374 5f66 756e  rn self.test_fun
-0000ef30: 6374 696f 6e0a 0a20 2020 2064 6566 2070  ction..    def p
-0000ef40: 726f 6365 7373 5f6d 6f64 656c 5f69 6e70  rocess_model_inp
-0000ef50: 7574 735f 666f 725f 7465 7374 2873 656c  uts_for_test(sel
-0000ef60: 662c 2074 7269 706c 6573 293a 0a20 2020  f, triples):.   
-0000ef70: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
-0000ef80: 6865 2070 726f 6365 7373 6564 2074 7269  he processed tri
-0000ef90: 706c 6573 2e0a 0a20 2020 2020 2020 2050  ples...        P
-0000efa0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-0000efb0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0000efc0: 2020 2020 2074 7269 706c 6573 3a20 6e70       triples: np
-0000efd0: 2e61 7272 6179 0a20 2020 2020 2020 2020  .array.         
-0000efe0: 2020 2054 7269 706c 6573 2074 6f20 6265     Triples to be
-0000eff0: 2070 726f 6365 7373 6564 2e0a 0a20 2020   processed...   
-0000f000: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-0000f010: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-0000f020: 2020 2020 206f 7574 5f74 7269 706c 6573       out_triples
-0000f030: 3a20 6e70 2e61 7272 6179 206f 7220 6c69  : np.array or li
-0000f040: 7374 0a20 2020 2020 2020 2020 2020 2049  st.            I
-0000f050: 6e20 7265 6775 6c61 7220 286e 6f6e 2070  n regular (non p
-0000f060: 6172 7469 7469 6f6e 6564 2920 6d6f 6465  artitioned) mode
-0000f070: 2c20 7468 6520 7472 6970 6c65 7320 6172  , the triples ar
-0000f080: 6520 7265 7475 726e 6564 2061 7320 7468  e returned as th
-0000f090: 6579 2061 7265 2067 6976 656e 2069 6e20  ey are given in 
-0000f0a0: 696e 7075 742e 0a20 2020 2020 2020 2020  input..         
-0000f0b0: 2020 2049 6e20 6361 7365 206f 6620 7061     In case of pa
-0000f0c0: 7274 6974 696f 6e69 6e67 2c20 6974 2072  rtitioning, it r
-0000f0d0: 6574 7572 6e73 2074 6865 2074 7269 706c  eturns the tripl
-0000f0e0: 6520 656d 6265 6464 696e 6773 2061 7320  e embeddings as 
-0000f0f0: 6120 6c69 7374 206f 6620 7369 7a65 2033  a list of size 3
-0000f100: 2c20 7768 6572 6520 6561 6368 2065 6c65  , where each ele
-0000f110: 6d65 6e74 0a20 2020 2020 2020 2020 2020  ment.           
-0000f120: 2069 7320 6120 6e70 2e61 7272 6179 206f   is a np.array o
-0000f130: 6620 7375 626a 6563 7473 2c20 7072 6564  f subjects, pred
-0000f140: 6963 6174 6573 2061 6e64 206f 626a 6563  icates and objec
-0000f150: 7473 2065 6d62 6564 6469 6e67 732e 0a20  ts embeddings.. 
-0000f160: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000f170: 2020 2069 6620 7365 6c66 2e69 735f 7061     if self.is_pa
-0000f180: 7274 6974 696f 6e65 645f 7472 6169 6e69  rtitioned_traini
-0000f190: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
-0000f1a0: 6e70 5f74 7269 706c 6573 203d 2074 7269  np_triples = tri
-0000f1b0: 706c 6573 2e6e 756d 7079 2829 0a20 2020  ples.numpy().   
-0000f1c0: 2020 2020 2020 2020 2073 7562 5f65 6d62           sub_emb
-0000f1d0: 5f6f 7574 203d 205b 5d0a 2020 2020 2020  _out = [].      
-0000f1e0: 2020 2020 2020 6f62 6a5f 656d 625f 6f75        obj_emb_ou
-0000f1f0: 7420 3d20 5b5d 0a20 2020 2020 2020 2020  t = [].         
-0000f200: 2020 2072 656c 5f65 6d62 5f6f 7574 203d     rel_emb_out =
-0000f210: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
-0000f220: 7769 7468 2073 6865 6c76 652e 6f70 656e  with shelve.open
-0000f230: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000f240: 2020 7365 6c66 2e70 6172 7469 7469 6f6e    self.partition
-0000f250: 6572 5f6d 6574 6164 6174 615b 2265 6e74  er_metadata["ent
-0000f260: 5f6d 6170 5f66 6e61 6d65 225d 0a20 2020  _map_fname"].   
-0000f270: 2020 2020 2020 2020 2029 2061 7320 656e           ) as en
-0000f280: 745f 656d 623a 0a20 2020 2020 2020 2020  t_emb:.         
-0000f290: 2020 2020 2020 2077 6974 6820 7368 656c         with shel
-0000f2a0: 7665 2e6f 7065 6e28 0a20 2020 2020 2020  ve.open(.       
-0000f2b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f2c0: 662e 7061 7274 6974 696f 6e65 725f 6d65  f.partitioner_me
-0000f2d0: 7461 6461 7461 5b22 7265 6c5f 6d61 705f  tadata["rel_map_
-0000f2e0: 666e 616d 6522 5d0a 2020 2020 2020 2020  fname"].        
-0000f2f0: 2020 2020 2020 2020 2920 6173 2072 656c          ) as rel
-0000f300: 5f65 6d62 3a0a 2020 2020 2020 2020 2020  _emb:.          
-0000f310: 2020 2020 2020 2020 2020 666f 7220 7472            for tr
-0000f320: 6970 6c65 2069 6e20 6e70 5f74 7269 706c  iple in np_tripl
-0000f330: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-0000f340: 2020 2020 2020 2020 2020 2020 7375 625f              sub_
-0000f350: 656d 625f 6f75 742e 6170 7065 6e64 2865  emb_out.append(e
-0000f360: 6e74 5f65 6d62 5b73 7472 2874 7269 706c  nt_emb[str(tripl
-0000f370: 655b 305d 295d 290a 2020 2020 2020 2020  e[0])]).        
-0000f380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f390: 7265 6c5f 656d 625f 6f75 742e 6170 7065  rel_emb_out.appe
-0000f3a0: 6e64 2872 656c 5f65 6d62 5b73 7472 2874  nd(rel_emb[str(t
-0000f3b0: 7269 706c 655b 315d 295d 290a 2020 2020  riple[1])]).    
-0000f3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3d0: 2020 2020 6f62 6a5f 656d 625f 6f75 742e      obj_emb_out.
-0000f3e0: 6170 7065 6e64 2865 6e74 5f65 6d62 5b73  append(ent_emb[s
-0000f3f0: 7472 2874 7269 706c 655b 325d 295d 290a  tr(triple[2])]).
-0000f400: 0a20 2020 2020 2020 2020 2020 2065 6d62  .            emb
-0000f410: 5f6f 7574 203d 205b 0a20 2020 2020 2020  _out = [.       
-0000f420: 2020 2020 2020 2020 206e 702e 6172 7261           np.arra
-0000f430: 7928 7375 625f 656d 625f 6f75 7429 2c0a  y(sub_emb_out),.
-0000f440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f450: 6e70 2e61 7272 6179 2872 656c 5f65 6d62  np.array(rel_emb
-0000f460: 5f6f 7574 292c 0a20 2020 2020 2020 2020  _out),.         
-0000f470: 2020 2020 2020 206e 702e 6172 7261 7928         np.array(
-0000f480: 6f62 6a5f 656d 625f 6f75 7429 2c0a 2020  obj_emb_out),.  
-0000f490: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-0000f4a0: 2020 2020 2020 2020 7265 7475 726e 2065          return e
-0000f4b0: 6d62 5f6f 7574 0a20 2020 2020 2020 2065  mb_out.        e
-0000f4c0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000f4d0: 2072 6574 7572 6e20 7472 6970 6c65 730a   return triples.
-0000f4e0: 0a20 2020 2064 6566 2065 7661 6c75 6174  .    def evaluat
-0000f4f0: 6528 0a20 2020 2020 2020 2073 656c 662c  e(.        self,
-0000f500: 0a20 2020 2020 2020 2078 3d4e 6f6e 652c  .        x=None,
-0000f510: 0a20 2020 2020 2020 2062 6174 6368 5f73  .        batch_s
-0000f520: 697a 653d 3332 2c0a 2020 2020 2020 2020  ize=32,.        
-0000f530: 7665 7262 6f73 653d 5472 7565 2c0a 2020  verbose=True,.  
-0000f540: 2020 2020 2020 7573 655f 6669 6c74 6572        use_filter
-0000f550: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-0000f560: 636f 7272 7570 745f 7369 6465 3d22 732c  corrupt_side="s,
-0000f570: 6f22 2c0a 2020 2020 2020 2020 656e 7469  o",.        enti
-0000f580: 7469 6573 5f73 7562 7365 743d 4e6f 6e65  ties_subset=None
-0000f590: 2c0a 2020 2020 2020 2020 7261 6e6b 696e  ,.        rankin
-0000f5a0: 675f 7374 7261 7465 6779 3d22 776f 7273  g_strategy="wors
-0000f5b0: 7422 2c0a 2020 2020 2020 2020 6361 6c6c  t",.        call
-0000f5c0: 6261 636b 733d 4e6f 6e65 2c0a 2020 2020  backs=None,.    
-0000f5d0: 2020 2020 6461 7461 7365 745f 7479 7065      dataset_type
-0000f5e0: 3d22 7465 7374 222c 0a20 2020 2029 3a0a  ="test",.    ):.
-0000f5f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000f600: 2020 2020 4576 616c 7561 7465 2074 6865      Evaluate the
-0000f610: 2069 6e70 7574 7320 6167 6169 6e73 7420   inputs against 
-0000f620: 636f 7272 7570 7469 6f6e 7320 616e 6420  corruptions and 
-0000f630: 7265 7475 726e 2072 616e 6b73 2e0a 0a20  return ranks... 
-0000f640: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-0000f650: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-0000f660: 2d2d 2d2d 0a20 2020 2020 2020 2078 3a20  ----.        x: 
-0000f670: 6e70 2e61 7272 6179 2c20 7368 6170 6520  np.array, shape 
-0000f680: 286e 2c33 2920 6f72 2073 7472 206f 7220  (n,3) or str or 
-0000f690: 4772 6170 6844 6174 614c 6f61 6465 7220  GraphDataLoader 
-0000f6a0: 6f72 2041 6273 7472 6163 7447 7261 7068  or AbstractGraph
-0000f6b0: 5061 7274 6974 696f 6e65 720a 2020 2020  Partitioner.    
-0000f6c0: 2020 2020 2020 2020 4461 7461 204f 5220          Data OR 
-0000f6d0: 4669 6c65 6e61 6d65 206f 6620 7468 6520  Filename of the 
-0000f6e0: 6461 7461 2066 696c 6520 4f52 2044 6174  data file OR Dat
-0000f6f0: 6120 4861 6e64 6c65 2074 6f20 6265 2075  a Handle to be u
-0000f700: 7365 6420 666f 7220 7472 6169 6e69 6e67  sed for training
-0000f710: 2e0a 2020 2020 2020 2020 6261 7463 685f  ..        batch_
-0000f720: 7369 7a65 3a20 696e 740a 2020 2020 2020  size: int.      
-0000f730: 2020 2020 2020 4261 7463 6820 7369 7a65        Batch size
-0000f740: 2074 6f20 7573 6520 6475 7269 6e67 2074   to use during t
-0000f750: 7261 696e 696e 672e 0a20 2020 2020 2020  raining..       
-0000f760: 2020 2020 204d 6179 2062 6520 6f76 6572       May be over
-0000f770: 7269 6464 656e 2069 6620 6060 7860 6020  ridden if ``x`` 
-0000f780: 6973 2060 4772 6170 6844 6174 614c 6f61  is `GraphDataLoa
-0000f790: 6465 7260 206f 7220 6041 6273 7472 6163  der` or `Abstrac
-0000f7a0: 7447 7261 7068 5061 7274 6974 696f 6e65  tGraphPartitione
-0000f7b0: 7260 2069 6e73 7461 6e63 650a 2020 2020  r` instance.    
-0000f7c0: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
-0000f7d0: 6c0a 2020 2020 2020 2020 2020 2020 5665  l.            Ve
-0000f7e0: 7262 6f73 6974 7920 6d6f 6465 2e0a 2020  rbosity mode..  
-0000f7f0: 2020 2020 2020 7573 655f 6669 6c74 6572        use_filter
-0000f800: 3a20 626f 6f6c 206f 7220 6469 6374 0a20  : bool or dict. 
-0000f810: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
-0000f820: 6572 2074 6f20 7573 6520 6120 6669 6c74  er to use a filt
-0000f830: 6572 206f 6620 6e6f 742e 2049 6620 6120  er of not. If a 
-0000f840: 6469 6374 696f 6e61 7279 2069 7320 7370  dictionary is sp
-0000f850: 6563 6966 6965 642c 2074 6865 2064 6174  ecified, the dat
-0000f860: 6120 696e 2074 6865 2064 6963 7420 6973  a in the dict is
-0000f870: 2063 6f6e 6361 7465 6e61 7465 640a 2020   concatenated.  
-0000f880: 2020 2020 2020 2020 2020 616e 6420 7573            and us
-0000f890: 6564 2061 7320 6669 6c74 6572 2e0a 2020  ed as filter..  
-0000f8a0: 2020 2020 2020 636f 7272 7570 745f 7369        corrupt_si
-0000f8b0: 6465 3a20 7374 720a 2020 2020 2020 2020  de: str.        
-0000f8c0: 2020 2020 5768 6963 6820 7369 6465 2074      Which side t
-0000f8d0: 6f20 636f 7272 7570 7420 6f66 2061 2074  o corrupt of a t
-0000f8e0: 7269 706c 6520 746f 2063 6f72 7275 7074  riple to corrupt
-0000f8f0: 2e20 4974 2063 616e 2062 6520 7468 6520  . It can be the 
-0000f900: 7375 626a 6563 7420 2860 6063 6f72 7275  subject (``corru
-0000f910: 7074 5f73 697a 653d 2273 2260 6029 2c0a  pt_size="s"``),.
-0000f920: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-0000f930: 6f62 6a65 6374 2028 6060 636f 7272 7570  object (``corrup
-0000f940: 745f 7369 7a65 3d22 6f22 6060 292c 2074  t_size="o"``), t
-0000f950: 6865 2073 7562 6a65 6374 2061 6e64 2074  he subject and t
-0000f960: 6865 206f 626a 6563 7420 2860 6063 6f72  he object (``cor
-0000f970: 7275 7074 5f73 697a 653d 2273 2b6f 2260  rupt_size="s+o"`
-0000f980: 6020 6f72 0a20 2020 2020 2020 2020 2020  ` or.           
-0000f990: 2060 6063 6f72 7275 7074 5f73 697a 653d   ``corrupt_size=
-0000f9a0: 2273 2c6f 2260 6029 2028 6465 6661 756c  "s,o"``) (defaul
-0000f9b0: 743a 6022 732c 6f22 6029 2e0a 2020 2020  t:`"s,o"`)..    
-0000f9c0: 2020 2020 7261 6e6b 696e 675f 7374 7261      ranking_stra
-0000f9d0: 7465 6779 3a20 7374 720a 2020 2020 2020  tegy: str.      
-0000f9e0: 2020 2020 2020 496e 6469 6361 7465 7320        Indicates 
-0000f9f0: 686f 7720 746f 2062 7265 616b 2074 6965  how to break tie
-0000fa00: 7320 7768 656e 2061 2074 6573 7420 7472  s when a test tr
-0000fa10: 6970 6c65 2067 6574 7320 7468 6520 7361  iple gets the sa
-0000fa20: 6d65 2072 616e 6b20 6f66 2061 2063 6f72  me rank of a cor
-0000fa30: 7275 7074 696f 6e2e 0a20 2020 2020 2020  ruption..       
-0000fa40: 2020 2020 2043 616e 2062 6520 6f6e 6520       Can be one 
-0000fa50: 6f66 2074 6865 2074 6872 6565 2074 7970  of the three typ
-0000fa60: 6573 3a20 6022 6265 7374 2260 2c20 6022  es: `"best"`, `"
-0000fa70: 6d69 6464 6c65 2260 2c20 6022 776f 7273  middle"`, `"wors
-0000fa80: 7422 6020 2864 6566 6175 6c74 3a20 6022  t"` (default: `"
-0000fa90: 776f 7273 7422 602c 2069 2e65 2e2c 0a20  worst"`, i.e.,. 
-0000faa0: 2020 2020 2020 2020 2020 2074 6865 2077             the w
-0000fab0: 6f72 7374 2072 616e 6b20 6973 2061 7373  orst rank is ass
-0000fac0: 6967 6e65 6420 746f 2074 6865 2074 6573  igned to the tes
-0000fad0: 7420 7472 6970 6c65 292e 0a20 2020 2020  t triple)..     
-0000fae0: 2020 2065 6e74 6974 6965 735f 7375 6273     entities_subs
-0000faf0: 6574 3a20 6c69 7374 206f 7220 6e70 2e61  et: list or np.a
-0000fb00: 7272 6179 0a20 2020 2020 2020 2020 2020  rray.           
-0000fb10: 2053 7562 7365 7420 6f66 2065 6e74 6974   Subset of entit
-0000fb20: 6965 7320 746f 2062 6520 7573 6564 2066  ies to be used f
-0000fb30: 6f72 2067 656e 6572 6174 696e 6720 636f  or generating co
-0000fb40: 7272 7570 7469 6f6e 732e 0a20 2020 2020  rruptions..     
-0000fb50: 2020 2063 616c 6c62 6163 6b73 3a20 6c69     callbacks: li
-0000fb60: 7374 206f 6620 6b65 7261 732e 6361 6c6c  st of keras.call
-0000fb70: 6261 636b 732e 4361 6c6c 6261 636b 2069  backs.Callback i
-0000fb80: 6e73 7461 6e63 6573 0a20 2020 2020 2020  nstances.       
-0000fb90: 2020 2020 204c 6973 7420 6f66 2063 616c       List of cal
-0000fba0: 6c62 6163 6b73 2074 6f20 6170 706c 7920  lbacks to apply 
-0000fbb0: 6475 7269 6e67 2065 7661 6c75 6174 696f  during evaluatio
-0000fbc0: 6e2e 0a0a 2020 2020 2020 2020 5265 7475  n...        Retu
-0000fbd0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-0000fbe0: 2d2d 2d0a 2020 2020 2020 2020 7261 6e6b  ---.        rank
-0000fbf0: 3a20 6e70 2e61 7272 6179 2c20 7368 6170  : np.array, shap
-0000fc00: 6520 286e 2c20 6e75 6d62 6572 206f 6620  e (n, number of 
-0000fc10: 636f 7272 7570 7465 6420 7369 6465 7329  corrupted sides)
-0000fc20: 0a20 2020 2020 2020 2020 2020 2052 616e  .            Ran
-0000fc30: 6b69 6e67 206f 6620 7465 7374 2074 7269  king of test tri
-0000fc40: 706c 6573 2061 6761 696e 7374 2073 7562  ples against sub
-0000fc50: 6a65 6374 2063 6f72 7275 7074 696f 6e73  ject corruptions
-0000fc60: 2061 6e64 2f6f 7220 6f62 6a65 6374 2063   and/or object c
-0000fc70: 6f72 7275 7074 696f 6e73 2e0a 0a20 2020  orruptions...   
-0000fc80: 2020 2020 2045 7861 6d70 6c65 0a20 2020       Example.   
-0000fc90: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-0000fca0: 2020 2020 203e 3e3e 2066 726f 6d20 616d       >>> from am
-0000fcb0: 706c 6967 7261 7068 2e64 6174 6173 6574  pligraph.dataset
-0000fcc0: 7320 696d 706f 7274 206c 6f61 645f 6662  s import load_fb
-0000fcd0: 3135 6b5f 3233 370a 2020 2020 2020 2020  15k_237.        
-0000fce0: 3e3e 3e20 6672 6f6d 2061 6d70 6c69 6772  >>> from ampligr
-0000fcf0: 6170 682e 6c61 7465 6e74 5f66 6561 7475  aph.latent_featu
-0000fd00: 7265 7320 696d 706f 7274 2053 636f 7269  res import Scori
-0000fd10: 6e67 4261 7365 6445 6d62 6564 6469 6e67  ngBasedEmbedding
-0000fd20: 4d6f 6465 6c0a 2020 2020 2020 2020 3e3e  Model.        >>
-0000fd30: 3e20 6672 6f6d 2061 6d70 6c69 6772 6170  > from ampligrap
-0000fd40: 682e 6576 616c 7561 7469 6f6e 2e6d 6574  h.evaluation.met
-0000fd50: 7269 6373 2069 6d70 6f72 7420 6d72 725f  rics import mrr_
-0000fd60: 7363 6f72 652c 2068 6974 735f 6174 5f6e  score, hits_at_n
-0000fd70: 5f73 636f 7265 2c20 6d72 5f73 636f 7265  _score, mr_score
-0000fd80: 0a20 2020 2020 2020 203e 3e3e 2058 203d  .        >>> X =
-0000fd90: 206c 6f61 645f 6662 3135 6b5f 3233 3728   load_fb15k_237(
-0000fda0: 290a 2020 2020 2020 2020 3e3e 3e20 6d6f  ).        >>> mo
-0000fdb0: 6465 6c20 3d20 5363 6f72 696e 6742 6173  del = ScoringBas
-0000fdc0: 6564 456d 6265 6464 696e 674d 6f64 656c  edEmbeddingModel
-0000fdd0: 2865 7461 3d35 2c0a 2020 2020 2020 2020  (eta=5,.        
-0000fde0: 3e3e 3e20 2020 2020 2020 2020 2020 2020  >>>             
-0000fdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe00: 2020 2020 2020 206b 3d33 3030 2c0a 2020         k=300,.  
-0000fe10: 2020 2020 2020 3e3e 3e20 2020 2020 2020        >>>       
-0000fe20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe30: 2020 2020 2020 2020 2020 2020 2073 636f               sco
-0000fe40: 7269 6e67 5f74 7970 653d 2743 6f6d 706c  ring_type='Compl
-0000fe50: 4578 272c 0a20 2020 2020 2020 203e 3e3e  Ex',.        >>>
-0000fe60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe80: 2020 2020 7365 6564 3d30 290a 2020 2020      seed=0).    
-0000fe90: 2020 2020 3e3e 3e20 6d6f 6465 6c2e 636f      >>> model.co
-0000fea0: 6d70 696c 6528 6f70 7469 6d69 7a65 723d  mpile(optimizer=
-0000feb0: 2761 6461 6d27 2c20 6c6f 7373 3d27 6e6c  'adam', loss='nl
-0000fec0: 6c27 290a 2020 2020 2020 2020 3e3e 3e20  l').        >>> 
-0000fed0: 6d6f 6465 6c2e 6669 7428 585b 2774 7261  model.fit(X['tra
-0000fee0: 696e 275d 2c0a 2020 2020 2020 2020 3e3e  in'],.        >>
-0000fef0: 3e20 2020 2020 2020 2020 2020 6261 7463  >           batc
-0000ff00: 685f 7369 7a65 3d31 3030 3030 2c0a 2020  h_size=10000,.  
-0000ff10: 2020 2020 2020 3e3e 3e20 2020 2020 2020        >>>       
-0000ff20: 2020 2020 6570 6f63 6873 3d35 290a 2020      epochs=5).  
-0000ff30: 2020 2020 2020 4570 6f63 6820 312f 350a        Epoch 1/5.
-0000ff40: 2020 2020 2020 2020 3239 2f32 3920 5b3d          29/29 [=
-0000ff50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000ff60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d5d 202d  =============] -
-0000ff70: 2032 7320 3731 6d73 2f73 7465 7020 2d20   2s 71ms/step - 
-0000ff80: 6c6f 7373 3a20 3637 3336 312e 3330 3437  loss: 67361.3047
-0000ff90: 0a20 2020 2020 2020 2045 706f 6368 2032  .        Epoch 2
-0000ffa0: 2f35 0a20 2020 2020 2020 2032 392f 3239  /5.        29/29
-0000ffb0: 205b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   [==============
-0000ffc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000ffd0: 5d20 2d20 3173 2033 356d 732f 7374 6570  ] - 1s 35ms/step
-0000ffe0: 202d 206c 6f73 733a 2036 3733 3138 2e36   - loss: 67318.6
-0000fff0: 3039 340a 2020 2020 2020 2020 4570 6f63  094.        Epoc
-00010000: 6820 332f 350a 2020 2020 2020 2020 3239  h 3/5.        29
-00010010: 2f32 3920 5b3d 3d3d 3d3d 3d3d 3d3d 3d3d  /29 [===========
-00010020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010030: 3d3d 3d5d 202d 2031 7320 3335 6d73 2f73  ===] - 1s 35ms/s
-00010040: 7465 7020 2d20 6c6f 7373 3a20 3637 3032  tep - loss: 6702
-00010050: 302e 3037 3033 0a20 2020 2020 2020 2045  0.0703.        E
-00010060: 706f 6368 2034 2f35 0a20 2020 2020 2020  poch 4/5.       
-00010070: 2032 392f 3239 205b 3d3d 3d3d 3d3d 3d3d   29/29 [========
-00010080: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010090: 3d3d 3d3d 3d3d 5d20 2d20 3173 2033 336d  ======] - 1s 33m
-000100a0: 732f 7374 6570 202d 206c 6f73 733a 2036  s/step - loss: 6
-000100b0: 3538 3637 2e33 3735 300a 2020 2020 2020  5867.3750.      
-000100c0: 2020 4570 6f63 6820 352f 350a 2020 2020    Epoch 5/5.    
-000100d0: 2020 2020 3239 2f32 3920 5b3d 3d3d 3d3d      29/29 [=====
-000100e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000100f0: 3d3d 3d3d 3d3d 3d3d 3d5d 202d 2031 7320  =========] - 1s 
-00010100: 3334 6d73 2f73 7465 7020 2d20 6c6f 7373  34ms/step - loss
-00010110: 3a20 3633 3531 372e 3930 3632 0a20 2020  : 63517.9062.   
-00010120: 2020 2020 203e 3e3e 2072 616e 6b73 203d       >>> ranks =
-00010130: 206d 6f64 656c 2e65 7661 6c75 6174 6528   model.evaluate(
-00010140: 585b 2774 6573 7427 5d2c 0a20 2020 2020  X['test'],.     
-00010150: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
-00010160: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-00010170: 7463 685f 7369 7a65 3d31 3030 2c0a 2020  tch_size=100,.  
-00010180: 2020 2020 2020 3e3e 3e20 2020 2020 2020        >>>       
-00010190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101a0: 2063 6f72 7275 7074 5f73 6964 653d 2773   corrupt_side='s
-000101b0: 2c6f 272c 0a20 2020 2020 2020 203e 3e3e  ,o',.        >>>
-000101c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101d0: 2020 2020 2020 2020 7573 655f 6669 6c74          use_filt
-000101e0: 6572 3d7b 2774 7261 696e 273a 2058 5b27  er={'train': X['
-000101f0: 7472 6169 6e27 5d2c 0a20 2020 2020 2020  train'],.       
-00010200: 203e 3e3e 2020 2020 2020 2020 2020 2020   >>>            
-00010210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010220: 2020 2020 2020 2020 2776 616c 6964 273a          'valid':
-00010230: 2058 5b27 7661 6c69 6427 5d2c 0a20 2020   X['valid'],.   
-00010240: 2020 2020 203e 3e3e 2020 2020 2020 2020       >>>        
-00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010260: 2020 2020 2020 2020 2020 2020 2774 6573              'tes
-00010270: 7427 3a20 585b 2774 6573 7427 5d29 0a20  t': X['test']). 
-00010280: 2020 2020 2020 203e 3e3e 206d 725f 7363         >>> mr_sc
-00010290: 6f72 6528 7261 6e6b 7329 2c20 6d72 725f  ore(ranks), mrr_
-000102a0: 7363 6f72 6528 7261 6e6b 7329 2c20 6869  score(ranks), hi
-000102b0: 7473 5f61 745f 6e5f 7363 6f72 6528 7261  ts_at_n_score(ra
-000102c0: 6e6b 732c 2031 292c 2068 6974 735f 6174  nks, 1), hits_at
-000102d0: 5f6e 5f73 636f 7265 2872 616e 6b73 2c20  _n_score(ranks, 
-000102e0: 3130 292c 206c 656e 2872 616e 6b73 290a  10), len(ranks).
-000102f0: 2020 2020 2020 2020 3238 2074 7269 706c          28 tripl
-00010300: 6573 2063 6f6e 7461 696e 696e 6720 696e  es containing in
-00010310: 7661 6c69 6420 6b65 7973 2073 6b69 7070  valid keys skipp
-00010320: 6564 210a 2020 2020 2020 2020 3920 7472  ed!.        9 tr
-00010330: 6970 6c65 7320 636f 6e74 6169 6e69 6e67  iples containing
-00010340: 2069 6e76 616c 6964 206b 6579 7320 736b   invalid keys sk
-00010350: 6970 7065 6421 0a20 2020 2020 2020 2032  ipped!.        2
-00010360: 3034 352f 3230 3435 205b 3d3d 3d3d 3d3d  045/2045 [======
-00010370: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010380: 3d3d 3d3d 3d3d 3d3d 5d20 2d20 3134 3973  ========] - 149s
-00010390: 2037 336d 732f 7374 6570 0a20 2020 2020   73ms/step.     
-000103a0: 2020 2028 3432 382e 3434 3637 3136 3839     (428.44671689
-000103b0: 3938 3932 3335 2c0a 2020 2020 2020 2020  989235,.        
-000103c0: 2030 2e32 3537 3631 3034 3130 3235 3238   0.2576104102528
-000103d0: 3233 3136 2c0a 2020 2020 2020 2020 2030  2316,.         0
-000103e0: 2e31 3839 3831 3739 3836 3130 3433 3135  .189817986104315
-000103f0: 352c 0a20 2020 2020 2020 2020 302e 3339  5,.         0.39
-00010400: 3139 3635 3934 3537 3837 3235 392c 0a20  1965945787259,. 
-00010410: 2020 2020 2020 2020 3230 3433 3829 0a20          20438). 
-00010420: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00010430: 2020 2023 2067 6574 2074 6865 2074 6573     # get the tes
-00010440: 7420 7365 7420 6861 6e64 6c65 720a 2020  t set handler.  
-00010450: 2020 2020 2020 7365 6c66 2e64 6174 615f        self.data_
-00010460: 6861 6e64 6c65 725f 7465 7374 203d 2064  handler_test = d
-00010470: 6174 615f 6164 6170 7465 722e 4461 7461  ata_adapter.Data
-00010480: 4861 6e64 6c65 7228 0a20 2020 2020 2020  Handler(.       
-00010490: 2020 2020 2078 2c0a 2020 2020 2020 2020       x,.        
-000104a0: 2020 2020 6261 7463 685f 7369 7a65 3d62      batch_size=b
-000104b0: 6174 6368 5f73 697a 652c 0a20 2020 2020  atch_size,.     
-000104c0: 2020 2020 2020 2064 6174 6173 6574 5f74         dataset_t
-000104d0: 7970 653d 6461 7461 7365 745f 7479 7065  ype=dataset_type
-000104e0: 2c0a 2020 2020 2020 2020 2020 2020 6570  ,.            ep
-000104f0: 6f63 6873 3d31 2c0a 2020 2020 2020 2020  ochs=1,.        
-00010500: 2020 2020 7573 655f 6669 6c74 6572 3d75      use_filter=u
-00010510: 7365 5f66 696c 7465 722c 0a20 2020 2020  se_filter,.     
-00010520: 2020 2020 2020 2075 7365 5f69 6e64 6578         use_index
-00010530: 6572 3d73 656c 662e 6461 7461 5f69 6e64  er=self.data_ind
-00010540: 6578 6572 2c0a 2020 2020 2020 2020 290a  exer,.        ).
-00010550: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00010560: 636f 7272 7570 745f 7369 6465 2069 6e20  corrupt_side in 
-00010570: 5b0a 2020 2020 2020 2020 2020 2020 2273  [.            "s
-00010580: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00010590: 6f22 2c0a 2020 2020 2020 2020 2020 2020  o",.            
-000105a0: 2273 2c6f 222c 0a20 2020 2020 2020 2020  "s,o",.         
-000105b0: 2020 2022 732b 6f22 2c0a 2020 2020 2020     "s+o",.      
-000105c0: 2020 5d2c 2022 496e 7661 6c69 6420 7661    ], "Invalid va
-000105d0: 6c75 6520 666f 7220 636f 7272 7570 745f  lue for corrupt_
-000105e0: 7369 6465 220a 2020 2020 2020 2020 6173  side".        as
-000105f0: 7365 7274 2072 616e 6b69 6e67 5f73 7472  sert ranking_str
-00010600: 6174 6567 7920 696e 205b 0a20 2020 2020  ategy in [.     
-00010610: 2020 2020 2020 2022 6265 7374 222c 0a20         "best",. 
-00010620: 2020 2020 2020 2020 2020 2022 6d69 6464             "midd
-00010630: 6c65 222c 0a20 2020 2020 2020 2020 2020  le",.           
-00010640: 2022 776f 7273 7422 2c0a 2020 2020 2020   "worst",.      
-00010650: 2020 5d2c 2022 496e 7661 6c69 6420 7661    ], "Invalid va
-00010660: 6c75 6520 666f 7220 7261 6e6b 696e 675f  lue for ranking_
-00010670: 7374 7261 7465 6779 220a 0a20 2020 2020  strategy"..     
-00010680: 2020 2073 656c 662e 636f 7272 7570 745f     self.corrupt_
-00010690: 7369 6465 203d 2063 6f72 7275 7074 5f73  side = corrupt_s
-000106a0: 6964 650a 2020 2020 2020 2020 7365 6c66  ide.        self
-000106b0: 2e72 616e 6b69 6e67 5f73 7472 6174 6567  .ranking_strateg
-000106c0: 7920 3d20 7261 6e6b 696e 675f 7374 7261  y = ranking_stra
-000106d0: 7465 6779 0a0a 2020 2020 2020 2020 7365  tegy..        se
-000106e0: 6c66 2e65 6e74 6974 6965 735f 7375 6273  lf.entities_subs
-000106f0: 6574 203d 2074 662e 636f 6e73 7461 6e74  et = tf.constant
-00010700: 285b 5d29 0a20 2020 2020 2020 2073 656c  ([]).        sel
-00010710: 662e 6d61 7070 696e 675f 6469 6374 203d  f.mapping_dict =
-00010720: 2074 662e 6c6f 6f6b 7570 2e65 7870 6572   tf.lookup.exper
-00010730: 696d 656e 7461 6c2e 4465 6e73 6548 6173  imental.DenseHas
-00010740: 6854 6162 6c65 280a 2020 2020 2020 2020  hTable(.        
-00010750: 2020 2020 7466 2e69 6e74 3332 2c20 7466      tf.int32, tf
-00010760: 2e69 6e74 3332 2c20 2d31 2c20 2d31 2c20  .int32, -1, -1, 
-00010770: 2d32 0a20 2020 2020 2020 2029 0a20 2020  -2.        ).   
-00010780: 2020 2020 2069 6620 656e 7469 7469 6573       if entities
-00010790: 5f73 7562 7365 7420 6973 206e 6f74 204e  _subset is not N
-000107a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000107b0: 2065 6e74 6974 6965 735f 7375 6273 6574   entities_subset
-000107c0: 203d 2073 656c 662e 6461 7461 5f69 6e64   = self.data_ind
-000107d0: 6578 6572 2e67 6574 5f69 6e64 6578 6573  exer.get_indexes
-000107e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000107f0: 2020 656e 7469 7469 6573 5f73 7562 7365    entities_subse
-00010800: 742c 2022 6522 0a20 2020 2020 2020 2020  t, "e".         
-00010810: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000d230: 2020 656e 7469 7479 5f72 656c 6174 696f    entity_relatio
+0000d240: 6e5f 7265 6775 6c61 7269 7a65 723d 6d79  n_regularizer=my
+0000d250: 5f72 6567 290a 0a20 2020 2020 2020 2045  _reg)..        E
+0000d260: 7861 6d70 6c65 0a20 2020 2020 2020 202d  xample.        -
+0000d270: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 203e  ------.        >
+0000d280: 3e3e 2066 726f 6d20 616d 706c 6967 7261  >> from ampligra
+0000d290: 7068 2e64 6174 6173 6574 7320 696d 706f  ph.datasets impo
+0000d2a0: 7274 206c 6f61 645f 6662 3135 6b5f 3233  rt load_fb15k_23
+0000d2b0: 370a 2020 2020 2020 2020 3e3e 3e20 6672  7.        >>> fr
+0000d2c0: 6f6d 2061 6d70 6c69 6772 6170 682e 6c61  om ampligraph.la
+0000d2d0: 7465 6e74 5f66 6561 7475 7265 7320 696d  tent_features im
+0000d2e0: 706f 7274 2053 636f 7269 6e67 4261 7365  port ScoringBase
+0000d2f0: 6445 6d62 6564 6469 6e67 4d6f 6465 6c0a  dEmbeddingModel.
+0000d300: 2020 2020 2020 2020 3e3e 3e20 5820 3d20          >>> X = 
+0000d310: 6c6f 6164 5f66 6231 356b 5f32 3337 2829  load_fb15k_237()
+0000d320: 0a20 2020 2020 2020 203e 3e3e 206d 6f64  .        >>> mod
+0000d330: 656c 203d 2053 636f 7269 6e67 4261 7365  el = ScoringBase
+0000d340: 6445 6d62 6564 6469 6e67 4d6f 6465 6c28  dEmbeddingModel(
+0000d350: 6574 613d 352c 0a20 2020 2020 2020 203e  eta=5,.        >
+0000d360: 3e3e 2020 2020 2020 2020 2020 2020 2020  >>              
+0000d370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d380: 2020 2020 2020 6b3d 3330 302c 0a20 2020        k=300,.   
+0000d390: 2020 2020 203e 3e3e 2020 2020 2020 2020       >>>        
+0000d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3b0: 2020 2020 2020 2020 2020 2020 7363 6f72              scor
+0000d3c0: 696e 675f 7479 7065 3d27 436f 6d70 6c45  ing_type='ComplE
+0000d3d0: 7827 2c0a 2020 2020 2020 2020 3e3e 3e20  x',.        >>> 
+0000d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d400: 2020 2073 6565 643d 3029 0a20 2020 2020     seed=0).     
+0000d410: 2020 203e 3e3e 206d 6f64 656c 2e63 6f6d     >>> model.com
+0000d420: 7069 6c65 286f 7074 696d 697a 6572 3d27  pile(optimizer='
+0000d430: 6164 616d 272c 206c 6f73 733d 276e 6c6c  adam', loss='nll
+0000d440: 2729 0a20 2020 2020 2020 203e 3e3e 206d  ').        >>> m
+0000d450: 6f64 656c 2e66 6974 2858 5b27 7472 6169  odel.fit(X['trai
+0000d460: 6e27 5d2c 0a20 2020 2020 2020 203e 3e3e  n'],.        >>>
+0000d470: 2020 2020 2020 2020 2020 2062 6174 6368             batch
+0000d480: 5f73 697a 653d 3130 3030 302c 0a20 2020  _size=10000,.   
+0000d490: 2020 2020 203e 3e3e 2020 2020 2020 2020       >>>        
+0000d4a0: 2020 2065 706f 6368 733d 3529 0a20 2020     epochs=5).   
+0000d4b0: 2020 2020 2045 706f 6368 2031 2f35 0a20       Epoch 1/5. 
+0000d4c0: 2020 2020 2020 2032 392f 3239 205b 3d3d         29/29 [==
+0000d4d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000d4e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 5d20 2d20  ============] - 
+0000d4f0: 3273 2036 316d 732f 7374 6570 202d 206c  2s 61ms/step - l
+0000d500: 6f73 733a 2036 3733 3631 2e33 3034 370a  oss: 67361.3047.
+0000d510: 2020 2020 2020 2020 4570 6f63 6820 322f          Epoch 2/
+0000d520: 350a 2020 2020 2020 2020 3239 2f32 3920  5.        29/29 
+0000d530: 5b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  [===============
+0000d540: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d5d  ===============]
+0000d550: 202d 2031 7320 3335 6d73 2f73 7465 7020   - 1s 35ms/step 
+0000d560: 2d20 6c6f 7373 3a20 3637 3331 382e 3630  - loss: 67318.60
+0000d570: 3934 0a20 2020 2020 2020 2045 706f 6368  94.        Epoch
+0000d580: 2033 2f35 0a20 2020 2020 2020 2032 392f   3/5.        29/
+0000d590: 3239 205b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  29 [============
+0000d5a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000d5b0: 3d3d 5d20 2d20 3173 2033 346d 732f 7374  ==] - 1s 34ms/st
+0000d5c0: 6570 202d 206c 6f73 733a 2036 3730 3230  ep - loss: 67020
+0000d5d0: 2e30 3730 330a 2020 2020 2020 2020 4570  .0703.        Ep
+0000d5e0: 6f63 6820 342f 350a 2020 2020 2020 2020  och 4/5.        
+0000d5f0: 3239 2f32 3920 5b3d 3d3d 3d3d 3d3d 3d3d  29/29 [=========
+0000d600: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000d610: 3d3d 3d3d 3d5d 202d 2031 7320 3334 6d73  =====] - 1s 34ms
+0000d620: 2f73 7465 7020 2d20 6c6f 7373 3a20 3635  /step - loss: 65
+0000d630: 3836 372e 3337 3530 0a20 2020 2020 2020  867.3750.       
+0000d640: 2045 706f 6368 2035 2f35 0a20 2020 2020   Epoch 5/5.     
+0000d650: 2020 2032 392f 3239 205b 3d3d 3d3d 3d3d     29/29 [======
+0000d660: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000d670: 3d3d 3d3d 3d3d 3d3d 5d20 2d20 3173 2033  ========] - 1s 3
+0000d680: 346d 732f 7374 6570 202d 206c 6f73 733a  4ms/step - loss:
+0000d690: 2036 3335 3137 2e39 3036 320a 0a20 2020   63517.9062..   
+0000d6a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000d6b0: 2023 2067 6574 2074 6865 206f 7074 696d   # get the optim
+0000d6c0: 697a 6572 0a20 2020 2020 2020 2073 656c  izer.        sel
+0000d6d0: 662e 6f70 7469 6d69 7a65 7220 3d20 6f70  f.optimizer = op
+0000d6e0: 7469 6d69 7a65 7273 2e67 6574 286f 7074  timizers.get(opt
+0000d6f0: 696d 697a 6572 290a 2020 2020 2020 2020  imizer).        
+0000d700: 7365 6c66 2e5f 7275 6e5f 6561 6765 726c  self._run_eagerl
+0000d710: 7920 3d20 6b77 6172 6773 2e70 6f70 2822  y = kwargs.pop("
+0000d720: 7275 6e5f 6561 6765 726c 7922 2c20 4e6f  run_eagerly", No
+0000d730: 6e65 290a 2020 2020 2020 2020 2320 7265  ne).        # re
+0000d740: 7365 7420 7468 6520 7472 6169 6e69 6e67  set the training
+0000d750: 2f65 7661 6c75 6174 652f 7072 6564 6963  /evaluate/predic
+0000d760: 7420 6675 6e63 7469 6f6e 0a20 2020 2020  t function.     
+0000d770: 2020 2073 656c 662e 5f72 6573 6574 5f63     self._reset_c
+0000d780: 6f6d 7069 6c65 5f63 6163 6865 2829 0a0a  ompile_cache()..
+0000d790: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
+0000d7a0: 6520 6c6f 7373 0a20 2020 2020 2020 2073  e loss.        s
+0000d7b0: 656c 662e 636f 6d70 696c 6564 5f6c 6f73  elf.compiled_los
+0000d7c0: 7320 3d20 6c6f 7373 5f66 756e 6374 696f  s = loss_functio
+0000d7d0: 6e73 2e67 6574 286c 6f73 7329 0a20 2020  ns.get(loss).   
+0000d7e0: 2020 2020 2023 204f 6e6c 7920 6d65 7472       # Only metr
+0000d7f0: 6963 2073 7570 706f 7274 6564 2064 7572  ic supported dur
+0000d800: 696e 6720 7468 6520 7472 6169 6e69 6e67  ing the training
+0000d810: 2069 7320 6d65 616e 204c 6f73 730a 2020   is mean Loss.  
+0000d820: 2020 2020 2020 7365 6c66 2e63 6f6d 7069        self.compi
+0000d830: 6c65 645f 6d65 7472 6963 7320 3d20 636f  led_metrics = co
+0000d840: 6d70 696c 655f 7574 696c 732e 4d65 7472  mpile_utils.Metr
+0000d850: 6963 7343 6f6e 7461 696e 6572 280a 2020  icsContainer(.  
+0000d860: 2020 2020 2020 2020 2020 6d65 7472 6963            metric
+0000d870: 735f 6d6f 642e 4d65 616e 286e 616d 653d  s_mod.Mean(name=
+0000d880: 226c 6f73 7322 292c 204e 6f6e 652c 204e  "loss"), None, N
+0000d890: 6f6e 650a 2020 2020 2020 2020 2920 2023  one.        )  #
+0000d8a0: 2054 6f74 616c 206c 6f73 732e 0a0a 2020   Total loss...  
+0000d8b0: 2020 2020 2020 2320 7365 7420 7468 6520        # set the 
+0000d8c0: 696e 6974 6961 6c69 7a65 7220 616e 6420  initializer and 
+0000d8d0: 7265 6775 6c61 7269 7a65 7220 6f66 2074  regularizer of t
+0000d8e0: 6865 2065 6d62 6564 6469 6e67 206d 6174  he embedding mat
+0000d8f0: 7269 6365 7320 696e 2074 6865 0a20 2020  rices in the.   
+0000d900: 2020 2020 2023 2065 6e63 6f64 696e 6720       # encoding 
+0000d910: 6c61 7965 720a 2020 2020 2020 2020 7365  layer.        se
+0000d920: 6c66 2e65 6e63 6f64 696e 675f 6c61 7965  lf.encoding_laye
+0000d930: 722e 7365 745f 696e 6974 6961 6c69 7a65  r.set_initialize
+0000d940: 7228 656e 7469 7479 5f72 656c 6174 696f  r(entity_relatio
+0000d950: 6e5f 696e 6974 6961 6c69 7a65 7229 0a20  n_initializer). 
+0000d960: 2020 2020 2020 2073 656c 662e 656e 636f         self.enco
+0000d970: 6469 6e67 5f6c 6179 6572 2e73 6574 5f72  ding_layer.set_r
+0000d980: 6567 756c 6172 697a 6572 2865 6e74 6974  egularizer(entit
+0000d990: 795f 7265 6c61 7469 6f6e 5f72 6567 756c  y_relation_regul
+0000d9a0: 6172 697a 6572 290a 2020 2020 2020 2020  arizer).        
+0000d9b0: 7365 6c66 2e5f 6973 5f63 6f6d 7069 6c65  self._is_compile
+0000d9c0: 6420 3d20 5472 7565 0a0a 2020 2020 4070  d = True..    @p
+0000d9d0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000d9e0: 6d65 7472 6963 7328 7365 6c66 293a 0a20  metrics(self):. 
+0000d9f0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+0000da00: 7320 616c 6c20 7468 6520 6d65 7472 6963  s all the metric
+0000da10: 7320 7468 6174 2077 696c 6c20 6265 2063  s that will be c
+0000da20: 6f6d 7075 7465 6420 6475 7269 6e67 2074  omputed during t
+0000da30: 7261 696e 696e 672e 2222 220a 2020 2020  raining.""".    
+0000da40: 2020 2020 6d65 7472 6963 7320 3d20 5b5d      metrics = []
+0000da50: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000da60: 2e5f 6973 5f63 6f6d 7069 6c65 643a 0a20  ._is_compiled:. 
+0000da70: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000da80: 6c66 2e63 6f6d 7069 6c65 645f 6c6f 7373  lf.compiled_loss
+0000da90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000daa0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+0000dab0: 7472 6963 7320 2b3d 2073 656c 662e 636f  trics += self.co
+0000dac0: 6d70 696c 6564 5f6c 6f73 732e 6d65 7472  mpiled_loss.metr
+0000dad0: 6963 730a 2020 2020 2020 2020 7265 7475  ics.        retu
+0000dae0: 726e 206d 6574 7269 6373 0a0a 2020 2020  rn metrics..    
+0000daf0: 6465 6620 6765 745f 656d 625f 6d61 7472  def get_emb_matr
+0000db00: 6978 5f74 6573 7428 7365 6c66 2c20 7061  ix_test(self, pa
+0000db10: 7274 5f6e 756d 6265 723d 312c 206e 756d  rt_number=1, num
+0000db20: 6265 725f 6f66 5f70 6172 7473 3d31 293a  ber_of_parts=1):
+0000db30: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
+0000db40: 7468 6520 656d 6265 6464 696e 6720 6d61  the embedding ma
+0000db50: 7472 6978 2064 7572 696e 6720 6576 616c  trix during eval
+0000db60: 7561 7469 6f6e 2e0a 0a20 2020 2020 2020  uation...       
+0000db70: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+0000db80: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0000db90: 2020 2020 2020 2070 6172 7420 6e75 6d62         part numb
+0000dba0: 6572 3a20 696e 740a 2020 2020 2020 2020  er: int.        
+0000dbb0: 2020 2020 5370 6563 6966 6965 7320 7768      Specifies wh
+0000dbc0: 6963 6820 7061 7274 2074 6f20 7265 7475  ich part to retu
+0000dbd0: 726e 2066 726f 6d20 7468 6520 6060 6e75  rn from the ``nu
+0000dbe0: 6d62 6572 5f6f 665f 7061 7274 7360 6020  mber_of_parts`` 
+0000dbf0: 696e 2077 6869 6368 2074 6865 2065 6e74  in which the ent
+0000dc00: 6972 6520 656d 6265 6464 696e 6720 6d61  ire embedding ma
+0000dc10: 7472 6978 2069 7320 7370 6c69 742e 0a20  trix is split.. 
+0000dc20: 2020 2020 2020 206e 756d 6265 725f 6f66         number_of
+0000dc30: 5f70 6172 7473 3a20 696e 740a 2020 2020  _parts: int.    
+0000dc40: 2020 2020 2020 2020 546f 7461 6c20 6e75          Total nu
+0000dc50: 6d62 6572 206f 6620 7061 7274 7320 696e  mber of parts in
+0000dc60: 2077 6869 6368 2074 6f20 7370 6c69 7420   which to split 
+0000dc70: 7468 6520 656d 6265 6464 696e 6720 6d61  the embedding ma
+0000dc80: 7472 6978 2e0a 0a20 2020 2020 2020 2052  trix...        R
+0000dc90: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+0000dca0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2065  ------.        e
+0000dcb0: 6d62 5f6d 6174 7269 783a 206e 702e 6172  mb_matrix: np.ar
+0000dcc0: 7261 792c 2073 6861 7065 2028 6e2c 6b29  ray, shape (n,k)
+0000dcd0: 0a20 2020 2020 2020 2020 2020 2050 6172  .            Par
+0000dce0: 7420 6f66 2074 6865 2065 6d62 6564 6469  t of the embeddi
+0000dcf0: 6e67 206d 6174 7269 7820 636f 7272 6573  ng matrix corres
+0000dd00: 706f 6e64 696e 6720 746f 2060 7061 7274  ponding to `part
+0000dd10: 5f6e 756d 6265 7260 2e0a 2020 2020 2020  _number`..      
+0000dd20: 2020 7374 6172 745f 696e 6465 783a 2069    start_index: i
+0000dd30: 6e74 0a20 2020 2020 2020 2020 2020 204f  nt.            O
+0000dd40: 7269 6769 6e61 6c20 656e 7469 7479 2069  riginal entity i
+0000dd50: 6e64 6578 2028 6461 7461 2064 6963 7429  ndex (data dict)
+0000dd60: 206f 6620 7468 6520 6669 7273 7420 726f   of the first ro
+0000dd70: 7720 6f66 2074 6865 2060 656d 625f 6d61  w of the `emb_ma
+0000dd80: 7472 6978 602e 0a20 2020 2020 2020 2065  trix`..        e
+0000dd90: 6e64 5f69 6e64 6578 3a20 696e 740a 2020  nd_index: int.  
+0000dda0: 2020 2020 2020 2020 2020 4f72 6967 696e            Origin
+0000ddb0: 616c 2065 6e74 6974 7920 696e 6465 7820  al entity index 
+0000ddc0: 2864 6174 6120 6469 6374 2920 6f66 2074  (data dict) of t
+0000ddd0: 6865 206c 6173 7420 726f 7720 6f66 2074  he last row of t
+0000dde0: 6865 2060 656d 625f 6d61 7472 6978 602e  he `emb_matrix`.
+0000ddf0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000de00: 2020 2020 2020 6966 206e 756d 6265 725f        if number_
+0000de10: 6f66 5f70 6172 7473 203d 3d20 313a 0a20  of_parts == 1:. 
+0000de20: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000de30: 6c66 2e65 6e74 6974 6965 735f 7375 6273  lf.entities_subs
+0000de40: 6574 2e73 6861 7065 5b30 5d20 213d 2030  et.shape[0] != 0
+0000de50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000de60: 2020 6f75 7420 3d20 7466 2e6e 6e2e 656d    out = tf.nn.em
+0000de70: 6265 6464 696e 675f 6c6f 6f6b 7570 280a  bedding_lookup(.
+0000de80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de90: 2020 2020 7365 6c66 2e65 6e63 6f64 696e      self.encodin
+0000dea0: 675f 6c61 7965 722e 656e 745f 656d 622c  g_layer.ent_emb,
+0000deb0: 2073 656c 662e 656e 7469 7469 6573 5f73   self.entities_s
+0000dec0: 7562 7365 740a 2020 2020 2020 2020 2020  ubset.          
+0000ded0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000dee0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000def0: 2020 2020 2020 2020 2020 6f75 7420 3d20            out = 
+0000df00: 7365 6c66 2e65 6e63 6f64 696e 675f 6c61  self.encoding_la
+0000df10: 7965 722e 656e 745f 656d 620a 2020 2020  yer.ent_emb.    
+0000df20: 2020 2020 2020 2020 7265 7475 726e 206f          return o
+0000df30: 7574 2c20 302c 206f 7574 2e73 6861 7065  ut, 0, out.shape
+0000df40: 5b30 5d20 2d20 310a 2020 2020 2020 2020  [0] - 1.        
+0000df50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000df60: 2020 7769 7468 2073 6865 6c76 652e 6f70    with shelve.op
+0000df70: 656e 280a 2020 2020 2020 2020 2020 2020  en(.            
+0000df80: 2020 2020 7365 6c66 2e70 6172 7469 7469      self.partiti
+0000df90: 6f6e 6572 5f6d 6574 6164 6174 615b 2265  oner_metadata["e
+0000dfa0: 6e74 5f6d 6170 5f66 6e61 6d65 225d 0a20  nt_map_fname"]. 
+0000dfb0: 2020 2020 2020 2020 2020 2029 2061 7320             ) as 
+0000dfc0: 656e 745f 7061 7274 6974 696f 6e3a 0a20  ent_partition:. 
+0000dfd0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0000dfe0: 6174 6368 5f73 697a 6520 3d20 696e 7428  atch_size = int(
+0000dff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e000: 2020 2020 206e 702e 6365 696c 286c 656e       np.ceil(len
+0000e010: 2865 6e74 5f70 6172 7469 7469 6f6e 2e6b  (ent_partition.k
+0000e020: 6579 7328 2929 202f 206e 756d 6265 725f  eys()) / number_
+0000e030: 6f66 5f70 6172 7473 290a 2020 2020 2020  of_parts).      
+0000e040: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000e050: 2020 2020 2020 2020 2020 2020 696e 6469              indi
+0000e060: 6365 7320 3d20 6e70 2e61 7261 6e67 6528  ces = np.arange(
+0000e070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e080: 2020 2020 2070 6172 745f 6e75 6d62 6572       part_number
+0000e090: 202a 2062 6174 6368 5f73 697a 652c 2028   * batch_size, (
+0000e0a0: 7061 7274 5f6e 756d 6265 7220 2b20 3129  part_number + 1)
+0000e0b0: 202a 2062 6174 6368 5f73 697a 650a 2020   * batch_size.  
+0000e0c0: 2020 2020 2020 2020 2020 2020 2020 292e                ).
+0000e0d0: 6173 7479 7065 2873 7472 290a 2020 2020  astype(str).    
+0000e0e0: 2020 2020 2020 2020 2020 2020 656d 625f              emb_
+0000e0f0: 6d61 7472 6978 203d 205b 5d0a 2020 2020  matrix = [].    
+0000e100: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000e110: 6964 7820 696e 2069 6e64 6963 6573 3a0a  idx in indices:.
+0000e120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e130: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e150: 2065 6d62 5f6d 6174 7269 782e 6170 7065   emb_matrix.appe
+0000e160: 6e64 2865 6e74 5f70 6172 7469 7469 6f6e  nd(ent_partition
+0000e170: 5b69 6478 5d29 0a20 2020 2020 2020 2020  [idx]).         
+0000e180: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+0000e190: 7420 4b65 7945 7272 6f72 3a0a 2020 2020  t KeyError:.    
+0000e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1b0: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+0000e1c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000e1d0: 206e 702e 6172 7261 7928 656d 625f 6d61   np.array(emb_ma
+0000e1e0: 7472 6978 292c 2069 6e74 2869 6e64 6963  trix), int(indic
+0000e1f0: 6573 5b30 5d29 2c20 696e 7428 696e 6469  es[0]), int(indi
+0000e200: 6365 735b 2d31 5d29 0a0a 2020 2020 6465  ces[-1])..    de
+0000e210: 6620 6d61 6b65 5f74 6573 745f 6675 6e63  f make_test_func
+0000e220: 7469 6f6e 2873 656c 6629 3a0a 2020 2020  tion(self):.    
+0000e230: 2020 2020 2222 2253 696d 696c 6172 2074      """Similar t
+0000e240: 6f20 6b65 7261 7320 6c69 622c 2074 6869  o keras lib, thi
+0000e250: 7320 6675 6e63 7469 6f6e 2072 6574 7572  s function retur
+0000e260: 6e73 2074 6865 2068 616e 646c 6520 746f  ns the handle to
+0000e270: 2074 6573 7420 7374 6570 2066 756e 6374   test step funct
+0000e280: 696f 6e2e 0a0a 2020 2020 2020 2020 4974  ion...        It
+0000e290: 2070 726f 6365 7373 6573 206f 6e65 2062   processes one b
+0000e2a0: 6174 6368 206f 6620 6461 7461 2062 7920  atch of data by 
+0000e2b0: 6974 6572 6174 696e 6720 6f76 6572 2074  iterating over t
+0000e2c0: 6865 2064 6174 6173 6574 2069 7465 7261  he dataset itera
+0000e2d0: 746f 7220 616e 6420 636f 6d70 7574 6573  tor and computes
+0000e2e0: 2074 6865 2074 6573 7420 6d65 7472 6963   the test metric
+0000e2f0: 732e 0a0a 2020 2020 2020 2020 5265 7475  s...        Retu
+0000e300: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+0000e310: 2d2d 2d0a 2020 2020 2020 2020 6f75 743a  ---.        out:
+0000e320: 2046 756e 6374 696f 6e20 6861 6e64 6c65   Function handle
+0000e330: 0a20 2020 2020 2020 2020 2020 2020 2048  .              H
+0000e340: 616e 646c 6520 746f 2074 6865 2074 6573  andle to the tes
+0000e350: 7420 7374 6570 2066 756e 6374 696f 6e2e  t step function.
+0000e360: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+0000e370: 2020 2020 2020 2320 6966 2073 656c 662e        # if self.
+0000e380: 7465 7374 5f66 756e 6374 696f 6e20 6973  test_function is
+0000e390: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000e3a0: 2020 2023 2020 2020 7265 7475 726e 2073     #    return s
+0000e3b0: 656c 662e 7465 7374 5f66 756e 6374 696f  elf.test_functio
+0000e3c0: 6e0a 0a20 2020 2020 2020 2064 6566 2074  n..        def t
+0000e3d0: 6573 745f 6675 6e63 7469 6f6e 2869 7465  est_function(ite
+0000e3e0: 7261 746f 7229 3a0a 2020 2020 2020 2020  rator):.        
+0000e3f0: 2020 2020 2320 746f 7461 6c20 6e75 6d62      # total numb
+0000e400: 6572 206f 6620 7061 7274 7320 696e 2077  er of parts in w
+0000e410: 6869 6368 2074 6f20 7370 6c69 7420 7468  hich to split th
+0000e420: 6520 656d 6265 6464 696e 6720 6d61 7472  e embedding matr
+0000e430: 6978 0a20 2020 2020 2020 2020 2020 2023  ix.            #
+0000e440: 2028 6465 6661 756c 7420 312c 2069 2e65   (default 1, i.e
+0000e450: 2e2c 2075 7365 2066 756c 6c20 6d61 7472  ., use full matr
+0000e460: 6978 2061 7320 6974 2069 7329 0a20 2020  ix as it is).   
+0000e470: 2020 2020 2020 2020 206e 756d 6265 725f           number_
+0000e480: 6f66 5f70 6172 7473 203d 2031 0a0a 2020  of_parts = 1..  
+0000e490: 2020 2020 2020 2020 2020 2320 6966 2069            # if i
+0000e4a0: 7420 6973 2070 6172 7469 7469 6f6e 6564  t is partitioned
+0000e4b0: 2074 7261 696e 696e 670a 2020 2020 2020   training.      
+0000e4c0: 2020 2020 2020 6966 2073 656c 662e 6973        if self.is
+0000e4d0: 5f70 6172 7469 7469 6f6e 6564 5f74 7261  _partitioned_tra
+0000e4e0: 696e 696e 673a 0a20 2020 2020 2020 2020  ining:.         
+0000e4f0: 2020 2020 2020 2023 2073 706c 6974 2074         # split t
+0000e500: 6865 2065 6d62 206d 6174 7269 7820 6261  he emb matrix ba
+0000e510: 7365 6420 6f6e 206e 756d 6265 7220 6f66  sed on number of
+0000e520: 2062 7563 6b65 7473 0a20 2020 2020 2020   buckets.       
+0000e530: 2020 2020 2020 2020 206e 756d 6265 725f           number_
+0000e540: 6f66 5f70 6172 7473 203d 2073 656c 662e  of_parts = self.
+0000e550: 7061 7274 6974 696f 6e65 725f 6b0a 0a20  partitioner_k.. 
+0000e560: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+0000e570: 3d20 6e65 7874 2869 7465 7261 746f 7229  = next(iterator)
+0000e580: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000e590: 7365 6c66 2e75 7365 5f66 696c 7465 723a  self.use_filter:
+0000e5a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e5b0: 2069 6e70 7574 732c 2066 696c 7465 7273   inputs, filters
+0000e5c0: 203d 2064 6174 615b 305d 2c20 6461 7461   = data[0], data
+0000e5d0: 5b31 5d0a 2020 2020 2020 2020 2020 2020  [1].            
+0000e5e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000e5f0: 2020 2020 2020 6966 2073 656c 662e 6461        if self.da
+0000e600: 7461 5f73 6861 7065 203e 2033 3a0a 2020  ta_shape > 3:.  
+0000e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e620: 2020 696e 7075 7473 2c20 6669 6c74 6572    inputs, filter
+0000e630: 7320 3d20 6461 7461 5b0a 2020 2020 2020  s = data[.      
+0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e650: 2020 300a 2020 2020 2020 2020 2020 2020    0.            
+0000e660: 2020 2020 2020 2020 5d2c 2074 662e 5261          ], tf.Ra
+0000e670: 6767 6564 5465 6e73 6f72 2e66 726f 6d5f  ggedTensor.from_
+0000e680: 726f 775f 6c65 6e67 7468 7328 5b5d 2c20  row_lengths([], 
+0000e690: 5b5d 290a 2020 2020 2020 2020 2020 2020  []).            
+0000e6a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000e6b0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000e6c0: 7075 7473 2c20 6669 6c74 6572 7320 3d20  puts, filters = 
+0000e6d0: 6461 7461 2c20 7466 2e52 6167 6765 6454  data, tf.RaggedT
+0000e6e0: 656e 736f 722e 6672 6f6d 5f72 6f77 5f6c  ensor.from_row_l
+0000e6f0: 656e 6774 6873 280a 2020 2020 2020 2020  engths(.        
+0000e700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e710: 5b5d 2c20 5b5d 0a20 2020 2020 2020 2020  [], [].         
+0000e720: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0000e730: 2020 2020 2020 2020 2020 2320 636f 6d70            # comp
+0000e740: 7574 6520 7468 6520 6f75 7470 7574 2073  ute the output s
+0000e750: 6861 7065 2062 6173 6564 206f 6e20 7468  hape based on th
+0000e760: 6520 7479 7065 206f 6620 636f 7272 7570  e type of corrup
+0000e770: 7469 6f6e 7320 746f 2062 650a 2020 2020  tions to be.    
+0000e780: 2020 2020 2020 2020 2320 7573 6564 0a20          # used. 
+0000e790: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+0000e7a0: 745f 7368 6170 6520 3d20 300a 2020 2020  t_shape = 0.    
+0000e7b0: 2020 2020 2020 2020 6966 2022 7322 2069          if "s" i
+0000e7c0: 6e20 7365 6c66 2e63 6f72 7275 7074 5f73  n self.corrupt_s
+0000e7d0: 6964 653a 0a20 2020 2020 2020 2020 2020  ide:.           
+0000e7e0: 2020 2020 206f 7574 7075 745f 7368 6170       output_shap
+0000e7f0: 6520 2b3d 2031 0a0a 2020 2020 2020 2020  e += 1..        
+0000e800: 2020 2020 6966 2022 6f22 2069 6e20 7365      if "o" in se
+0000e810: 6c66 2e63 6f72 7275 7074 5f73 6964 653a  lf.corrupt_side:
+0000e820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e830: 206f 7574 7075 745f 7368 6170 6520 2b3d   output_shape +=
+0000e840: 2031 0a0a 2020 2020 2020 2020 2020 2020   1..            
+0000e850: 2320 6372 6561 7465 2061 6e20 6172 7261  # create an arra
+0000e860: 7920 746f 2073 746f 7265 2074 6865 2072  y to store the r
+0000e870: 616e 6b73 2062 6173 6564 206f 6e20 6f75  anks based on ou
+0000e880: 7470 7574 2073 6861 7065 0a20 2020 2020  tput shape.     
+0000e890: 2020 2020 2020 206f 7665 7261 6c6c 5f72         overall_r
+0000e8a0: 616e 6b20 3d20 7466 2e7a 6572 6f73 280a  ank = tf.zeros(.
+0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8c0: 286f 7574 7075 745f 7368 6170 652c 2074  (output_shape, t
+0000e8d0: 662e 7368 6170 6528 696e 7075 7473 295b  f.shape(inputs)[
+0000e8e0: 305d 292c 2064 7479 7065 3d6e 702e 696e  0]), dtype=np.in
+0000e8f0: 7433 320a 2020 2020 2020 2020 2020 2020  t32.            
+0000e900: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+0000e910: 6620 7365 6c66 2e69 735f 7061 7274 6974  f self.is_partit
+0000e920: 696f 6e65 645f 7472 6169 6e69 6e67 3a0a  ioned_training:.
+0000e930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e940: 696e 7075 7473 203d 2073 656c 662e 7072  inputs = self.pr
+0000e950: 6f63 6573 735f 6d6f 6465 6c5f 696e 7075  ocess_model_inpu
+0000e960: 7473 5f66 6f72 5f74 6573 7428 696e 7075  ts_for_test(inpu
+0000e970: 7473 290a 0a20 2020 2020 2020 2020 2020  ts)..           
+0000e980: 2023 2072 756e 2074 6865 206c 6f6f 7020   # run the loop 
+0000e990: 6261 7365 6420 6f6e 206e 756d 6265 7220  based on number 
+0000e9a0: 6f66 2070 6172 7473 2069 6e20 7768 6963  of parts in whic
+0000e9b0: 6820 7468 6520 6f72 6967 696e 616c 2065  h the original e
+0000e9c0: 6d62 0a20 2020 2020 2020 2020 2020 2023  mb.            #
+0000e9d0: 206d 6174 7269 7820 7761 7320 6765 6e65   matrix was gene
+0000e9e0: 7261 7465 640a 2020 2020 2020 2020 2020  rated.          
+0000e9f0: 2020 666f 7220 6a20 696e 2072 616e 6765    for j in range
+0000ea00: 286e 756d 6265 725f 6f66 5f70 6172 7473  (number_of_parts
+0000ea10: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000ea20: 2020 2023 2067 6574 2074 6865 2065 6d62     # get the emb
+0000ea30: 6564 6469 6e67 206d 6174 7269 7820 616c  edding matrix al
+0000ea40: 6f6e 6720 7769 7468 2065 6e74 6974 7920  ong with entity 
+0000ea50: 6964 7320 6f66 2066 6972 7374 2061 6e64  ids of first and
+0000ea60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ea70: 2023 206c 6173 7420 726f 7720 6f66 2065   # last row of e
+0000ea80: 6d62 206d 6174 7269 780a 2020 2020 2020  mb matrix.      
+0000ea90: 2020 2020 2020 2020 2020 656d 625f 6d61            emb_ma
+0000eaa0: 742c 2073 7461 7274 5f65 6e74 5f69 642c  t, start_ent_id,
+0000eab0: 2065 6e64 5f65 6e74 5f69 6420 3d20 7365   end_ent_id = se
+0000eac0: 6c66 2e67 6574 5f65 6d62 5f6d 6174 7269  lf.get_emb_matri
+0000ead0: 785f 7465 7374 280a 2020 2020 2020 2020  x_test(.        
+0000eae0: 2020 2020 2020 2020 2020 2020 6a2c 206e              j, n
+0000eaf0: 756d 6265 725f 6f66 5f70 6172 7473 0a20  umber_of_parts. 
+0000eb00: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000eb10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eb20: 2023 2063 6f6d 7075 7465 2074 6865 2072   # compute the r
+0000eb30: 616e 6b0a 2020 2020 2020 2020 2020 2020  ank.            
+0000eb40: 2020 2020 7261 6e6b 7320 3d20 7365 6c66      ranks = self
+0000eb50: 2e5f 6765 745f 7261 6e6b 7328 0a20 2020  ._get_ranks(.   
+0000eb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb70: 2069 6e70 7574 732c 0a20 2020 2020 2020   inputs,.       
+0000eb80: 2020 2020 2020 2020 2020 2020 2065 6d62               emb
+0000eb90: 5f6d 6174 2c0a 2020 2020 2020 2020 2020  _mat,.          
+0000eba0: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+0000ebb0: 656e 745f 6964 2c0a 2020 2020 2020 2020  ent_id,.        
+0000ebc0: 2020 2020 2020 2020 2020 2020 656e 645f              end_
+0000ebd0: 656e 745f 6964 2c0a 2020 2020 2020 2020  ent_id,.        
+0000ebe0: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
+0000ebf0: 6572 732c 0a20 2020 2020 2020 2020 2020  ers,.           
+0000ec00: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+0000ec10: 7070 696e 675f 6469 6374 2c0a 2020 2020  pping_dict,.    
+0000ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec30: 7365 6c66 2e63 6f72 7275 7074 5f73 6964  self.corrupt_sid
+0000ec40: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000ec50: 2020 2020 2020 2073 656c 662e 7261 6e6b         self.rank
+0000ec60: 696e 675f 7374 7261 7465 6779 2c0a 2020  ing_strategy,.  
+0000ec70: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000ec80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec90: 2320 7374 6f72 6520 6974 2069 6e20 7468  # store it in th
+0000eca0: 6520 6f75 7470 7574 0a20 2020 2020 2020  e output.       
+0000ecb0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+0000ecc0: 6e20 7466 2e72 616e 6765 286f 7574 7075  n tf.range(outpu
+0000ecd0: 745f 7368 6170 6529 3a0a 2020 2020 2020  t_shape):.      
+0000ece0: 2020 2020 2020 2020 2020 2020 2020 6f76                ov
+0000ecf0: 6572 616c 6c5f 7261 6e6b 203d 2074 662e  erall_rank = tf.
+0000ed00: 7465 6e73 6f72 5f73 6361 7474 6572 5f6e  tensor_scatter_n
+0000ed10: 645f 6164 6428 0a20 2020 2020 2020 2020  d_add(.         
+0000ed20: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000ed30: 7665 7261 6c6c 5f72 616e 6b2c 205b 5b69  verall_rank, [[i
+0000ed40: 5d5d 2c20 5b72 616e 6b73 5b69 2c20 3a5d  ]], [ranks[i, :]
+0000ed50: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000ed60: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000ed70: 2020 2020 206f 7665 7261 6c6c 5f72 616e       overall_ran
+0000ed80: 6b20 3d20 7466 2e74 7261 6e73 706f 7365  k = tf.transpose
+0000ed90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000eda0: 2020 7466 2e72 6573 6861 7065 286f 7665    tf.reshape(ove
+0000edb0: 7261 6c6c 5f72 616e 6b2c 2028 6f75 7470  rall_rank, (outp
+0000edc0: 7574 5f73 6861 7065 2c20 2d31 2929 0a20  ut_shape, -1)). 
+0000edd0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000ede0: 2020 2020 2020 2020 2023 2069 6620 636f           # if co
+0000edf0: 7272 7570 7469 6f6e 2074 7970 6520 6973  rruption type is
+0000ee00: 2073 2b6f 2074 6865 6e20 6164 6420 7320   s+o then add s 
+0000ee10: 616e 6420 6f20 7261 6e6b 7320 616e 6420  and o ranks and 
+0000ee20: 7265 7475 726e 2074 6865 0a20 2020 2020  return the.     
+0000ee30: 2020 2020 2020 2023 2061 6464 6564 2072         # added r
+0000ee40: 616e 6b73 0a20 2020 2020 2020 2020 2020  anks.           
+0000ee50: 2069 6620 7365 6c66 2e63 6f72 7275 7074   if self.corrupt
+0000ee60: 5f73 6964 6520 3d3d 2022 732b 6f22 3a0a  _side == "s+o":.
+0000ee70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee80: 2320 6164 6420 7468 6520 7375 626a 6563  # add the subjec
+0000ee90: 7420 616e 6420 6f62 6a65 6374 2072 616e  t and object ran
+0000eea0: 6b73 0a20 2020 2020 2020 2020 2020 2020  ks.             
+0000eeb0: 2020 206f 7665 7261 6c6c 5f72 616e 6b20     overall_rank 
+0000eec0: 3d20 7466 2e72 6564 7563 655f 7375 6d28  = tf.reduce_sum(
+0000eed0: 6f76 6572 616c 6c5f 7261 6e6b 2c20 3129  overall_rank, 1)
+0000eee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eef0: 2023 2072 6574 7572 6e20 7468 6520 6164   # return the ad
+0000ef00: 6465 6420 7261 6e6b 730a 2020 2020 2020  ded ranks.      
+0000ef10: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000ef20: 2074 662e 7265 7368 6170 6528 6f76 6572   tf.reshape(over
+0000ef30: 616c 6c5f 7261 6e6b 2c20 282d 312c 2031  all_rank, (-1, 1
+0000ef40: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+0000ef50: 7265 7475 726e 206f 7665 7261 6c6c 5f72  return overall_r
+0000ef60: 616e 6b0a 0a20 2020 2020 2020 2069 6620  ank..        if 
+0000ef70: 6e6f 7420 7365 6c66 2e72 756e 5f65 6167  not self.run_eag
+0000ef80: 6572 6c79 2061 6e64 206e 6f74 2073 656c  erly and not sel
+0000ef90: 662e 6973 5f70 6172 7469 7469 6f6e 6564  f.is_partitioned
+0000efa0: 5f74 7261 696e 696e 673a 0a20 2020 2020  _training:.     
+0000efb0: 2020 2020 2020 2074 6573 745f 6675 6e63         test_func
+0000efc0: 7469 6f6e 203d 2064 6566 5f66 756e 6374  tion = def_funct
+0000efd0: 696f 6e2e 6675 6e63 7469 6f6e 280a 2020  ion.function(.  
+0000efe0: 2020 2020 2020 2020 2020 2020 2020 7465                te
+0000eff0: 7374 5f66 756e 6374 696f 6e2c 2065 7870  st_function, exp
+0000f000: 6572 696d 656e 7461 6c5f 7265 6c61 785f  erimental_relax_
+0000f010: 7368 6170 6573 3d54 7275 650a 2020 2020  shapes=True.    
+0000f020: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000f030: 2020 2073 656c 662e 7465 7374 5f66 756e     self.test_fun
+0000f040: 6374 696f 6e20 3d20 7465 7374 5f66 756e  ction = test_fun
+0000f050: 6374 696f 6e0a 0a20 2020 2020 2020 2072  ction..        r
+0000f060: 6574 7572 6e20 7365 6c66 2e74 6573 745f  eturn self.test_
+0000f070: 6675 6e63 7469 6f6e 0a0a 2020 2020 6465  function..    de
+0000f080: 6620 7072 6f63 6573 735f 6d6f 6465 6c5f  f process_model_
+0000f090: 696e 7075 7473 5f66 6f72 5f74 6573 7428  inputs_for_test(
+0000f0a0: 7365 6c66 2c20 7472 6970 6c65 7329 3a0a  self, triples):.
+0000f0b0: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+0000f0c0: 6e20 7468 6520 7072 6f63 6573 7365 6420  n the processed 
+0000f0d0: 7472 6970 6c65 732e 0a0a 2020 2020 2020  triples...      
+0000f0e0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+0000f0f0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+0000f100: 2020 2020 2020 2020 7472 6970 6c65 733a          triples:
+0000f110: 206e 702e 6172 7261 790a 2020 2020 2020   np.array.      
+0000f120: 2020 2020 2020 5472 6970 6c65 7320 746f        Triples to
+0000f130: 2062 6520 7072 6f63 6573 7365 642e 0a0a   be processed...
+0000f140: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+0000f150: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+0000f160: 2020 2020 2020 2020 6f75 745f 7472 6970          out_trip
+0000f170: 6c65 733a 206e 702e 6172 7261 7920 6f72  les: np.array or
+0000f180: 206c 6973 740a 2020 2020 2020 2020 2020   list.          
+0000f190: 2020 496e 2072 6567 756c 6172 2028 6e6f    In regular (no
+0000f1a0: 6e20 7061 7274 6974 696f 6e65 6429 206d  n partitioned) m
+0000f1b0: 6f64 652c 2074 6865 2074 7269 706c 6573  ode, the triples
+0000f1c0: 2061 7265 2072 6574 7572 6e65 6420 6173   are returned as
+0000f1d0: 2074 6865 7920 6172 6520 6769 7665 6e20   they are given 
+0000f1e0: 696e 2069 6e70 7574 2e0a 2020 2020 2020  in input..      
+0000f1f0: 2020 2020 2020 496e 2063 6173 6520 6f66        In case of
+0000f200: 2070 6172 7469 7469 6f6e 696e 672c 2069   partitioning, i
+0000f210: 7420 7265 7475 726e 7320 7468 6520 7472  t returns the tr
+0000f220: 6970 6c65 2065 6d62 6564 6469 6e67 7320  iple embeddings 
+0000f230: 6173 2061 206c 6973 7420 6f66 2073 697a  as a list of siz
+0000f240: 6520 332c 2077 6865 7265 2065 6163 6820  e 3, where each 
+0000f250: 656c 656d 656e 740a 2020 2020 2020 2020  element.        
+0000f260: 2020 2020 6973 2061 206e 702e 6172 7261      is a np.arra
+0000f270: 7920 6f66 2073 7562 6a65 6374 732c 2070  y of subjects, p
+0000f280: 7265 6469 6361 7465 7320 616e 6420 6f62  redicates and ob
+0000f290: 6a65 6374 7320 656d 6265 6464 696e 6773  jects embeddings
+0000f2a0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000f2b0: 2020 2020 2020 6966 2073 656c 662e 6973        if self.is
+0000f2c0: 5f70 6172 7469 7469 6f6e 6564 5f74 7261  _partitioned_tra
+0000f2d0: 696e 696e 673a 0a20 2020 2020 2020 2020  ining:.         
+0000f2e0: 2020 206e 705f 7472 6970 6c65 7320 3d20     np_triples = 
+0000f2f0: 7472 6970 6c65 732e 6e75 6d70 7928 290a  triples.numpy().
+0000f300: 2020 2020 2020 2020 2020 2020 7375 625f              sub_
+0000f310: 656d 625f 6f75 7420 3d20 5b5d 0a20 2020  emb_out = [].   
+0000f320: 2020 2020 2020 2020 206f 626a 5f65 6d62           obj_emb
+0000f330: 5f6f 7574 203d 205b 5d0a 2020 2020 2020  _out = [].      
+0000f340: 2020 2020 2020 7265 6c5f 656d 625f 6f75        rel_emb_ou
+0000f350: 7420 3d20 5b5d 0a20 2020 2020 2020 2020  t = [].         
+0000f360: 2020 2077 6974 6820 7368 656c 7665 2e6f     with shelve.o
+0000f370: 7065 6e28 0a20 2020 2020 2020 2020 2020  pen(.           
+0000f380: 2020 2020 2073 656c 662e 7061 7274 6974       self.partit
+0000f390: 696f 6e65 725f 6d65 7461 6461 7461 5b22  ioner_metadata["
+0000f3a0: 656e 745f 6d61 705f 666e 616d 6522 5d0a  ent_map_fname"].
+0000f3b0: 2020 2020 2020 2020 2020 2020 2920 6173              ) as
+0000f3c0: 2065 6e74 5f65 6d62 3a0a 2020 2020 2020   ent_emb:.      
+0000f3d0: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+0000f3e0: 6865 6c76 652e 6f70 656e 280a 2020 2020  helve.open(.    
+0000f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f400: 7365 6c66 2e70 6172 7469 7469 6f6e 6572  self.partitioner
+0000f410: 5f6d 6574 6164 6174 615b 2272 656c 5f6d  _metadata["rel_m
+0000f420: 6170 5f66 6e61 6d65 225d 0a20 2020 2020  ap_fname"].     
+0000f430: 2020 2020 2020 2020 2020 2029 2061 7320             ) as 
+0000f440: 7265 6c5f 656d 623a 0a20 2020 2020 2020  rel_emb:.       
+0000f450: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000f460: 2074 7269 706c 6520 696e 206e 705f 7472   triple in np_tr
+0000f470: 6970 6c65 733a 0a20 2020 2020 2020 2020  iples:.         
+0000f480: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f490: 7562 5f65 6d62 5f6f 7574 2e61 7070 656e  ub_emb_out.appen
+0000f4a0: 6428 656e 745f 656d 625b 7374 7228 7472  d(ent_emb[str(tr
+0000f4b0: 6970 6c65 5b30 5d29 5d29 0a20 2020 2020  iple[0])]).     
+0000f4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4d0: 2020 2072 656c 5f65 6d62 5f6f 7574 2e61     rel_emb_out.a
+0000f4e0: 7070 656e 6428 7265 6c5f 656d 625b 7374  ppend(rel_emb[st
+0000f4f0: 7228 7472 6970 6c65 5b31 5d29 5d29 0a20  r(triple[1])]). 
+0000f500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f510: 2020 2020 2020 206f 626a 5f65 6d62 5f6f         obj_emb_o
+0000f520: 7574 2e61 7070 656e 6428 656e 745f 656d  ut.append(ent_em
+0000f530: 625b 7374 7228 7472 6970 6c65 5b32 5d29  b[str(triple[2])
+0000f540: 5d29 0a0a 2020 2020 2020 2020 2020 2020  ])..            
+0000f550: 656d 625f 6f75 7420 3d20 5b0a 2020 2020  emb_out = [.    
+0000f560: 2020 2020 2020 2020 2020 2020 6e70 2e61              np.a
+0000f570: 7272 6179 2873 7562 5f65 6d62 5f6f 7574  rray(sub_emb_out
+0000f580: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000f590: 2020 206e 702e 6172 7261 7928 7265 6c5f     np.array(rel_
+0000f5a0: 656d 625f 6f75 7429 2c0a 2020 2020 2020  emb_out),.      
+0000f5b0: 2020 2020 2020 2020 2020 6e70 2e61 7272            np.arr
+0000f5c0: 6179 286f 626a 5f65 6d62 5f6f 7574 292c  ay(obj_emb_out),
+0000f5d0: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
+0000f5e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000f5f0: 6e20 656d 625f 6f75 740a 2020 2020 2020  n emb_out.      
+0000f600: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000f610: 2020 2020 7265 7475 726e 2074 7269 706c      return tripl
+0000f620: 6573 0a0a 2020 2020 6465 6620 6576 616c  es..    def eval
+0000f630: 7561 7465 280a 2020 2020 2020 2020 7365  uate(.        se
+0000f640: 6c66 2c0a 2020 2020 2020 2020 783d 4e6f  lf,.        x=No
+0000f650: 6e65 2c0a 2020 2020 2020 2020 6261 7463  ne,.        batc
+0000f660: 685f 7369 7a65 3d33 322c 0a20 2020 2020  h_size=32,.     
+0000f670: 2020 2076 6572 626f 7365 3d54 7275 652c     verbose=True,
+0000f680: 0a20 2020 2020 2020 2075 7365 5f66 696c  .        use_fil
+0000f690: 7465 723d 4661 6c73 652c 0a20 2020 2020  ter=False,.     
+0000f6a0: 2020 2063 6f72 7275 7074 5f73 6964 653d     corrupt_side=
+0000f6b0: 2273 2c6f 222c 0a20 2020 2020 2020 2065  "s,o",.        e
+0000f6c0: 6e74 6974 6965 735f 7375 6273 6574 3d4e  ntities_subset=N
+0000f6d0: 6f6e 652c 0a20 2020 2020 2020 2072 616e  one,.        ran
+0000f6e0: 6b69 6e67 5f73 7472 6174 6567 793d 2277  king_strategy="w
+0000f6f0: 6f72 7374 222c 0a20 2020 2020 2020 2063  orst",.        c
+0000f700: 616c 6c62 6163 6b73 3d4e 6f6e 652c 0a20  allbacks=None,. 
+0000f710: 2020 2020 2020 2064 6174 6173 6574 5f74         dataset_t
+0000f720: 7970 653d 2274 6573 7422 2c0a 2020 2020  ype="test",.    
+0000f730: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000f740: 2020 2020 2020 2045 7661 6c75 6174 6520         Evaluate 
+0000f750: 7468 6520 696e 7075 7473 2061 6761 696e  the inputs again
+0000f760: 7374 2063 6f72 7275 7074 696f 6e73 2061  st corruptions a
+0000f770: 6e64 2072 6574 7572 6e20 7261 6e6b 732e  nd return ranks.
+0000f780: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+0000f790: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+0000f7a0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000f7b0: 783a 206e 702e 6172 7261 792c 2073 6861  x: np.array, sha
+0000f7c0: 7065 2028 6e2c 3329 206f 7220 7374 7220  pe (n,3) or str 
+0000f7d0: 6f72 2047 7261 7068 4461 7461 4c6f 6164  or GraphDataLoad
+0000f7e0: 6572 206f 7220 4162 7374 7261 6374 4772  er or AbstractGr
+0000f7f0: 6170 6850 6172 7469 7469 6f6e 6572 0a20  aphPartitioner. 
+0000f800: 2020 2020 2020 2020 2020 2044 6174 6120             Data 
+0000f810: 4f52 2046 696c 656e 616d 6520 6f66 2074  OR Filename of t
+0000f820: 6865 2064 6174 6120 6669 6c65 204f 5220  he data file OR 
+0000f830: 4461 7461 2048 616e 646c 6520 746f 2062  Data Handle to b
+0000f840: 6520 7573 6564 2066 6f72 2074 7261 696e  e used for train
+0000f850: 696e 672e 0a20 2020 2020 2020 2062 6174  ing..        bat
+0000f860: 6368 5f73 697a 653a 2069 6e74 0a20 2020  ch_size: int.   
+0000f870: 2020 2020 2020 2020 2042 6174 6368 2073           Batch s
+0000f880: 697a 6520 746f 2075 7365 2064 7572 696e  ize to use durin
+0000f890: 6720 7472 6169 6e69 6e67 2e0a 2020 2020  g training..    
+0000f8a0: 2020 2020 2020 2020 4d61 7920 6265 206f          May be o
+0000f8b0: 7665 7272 6964 6465 6e20 6966 2060 6078  verridden if ``x
+0000f8c0: 6060 2069 7320 6047 7261 7068 4461 7461  `` is `GraphData
+0000f8d0: 4c6f 6164 6572 6020 6f72 2060 4162 7374  Loader` or `Abst
+0000f8e0: 7261 6374 4772 6170 6850 6172 7469 7469  ractGraphPartiti
+0000f8f0: 6f6e 6572 6020 696e 7374 616e 6365 0a20  oner` instance. 
+0000f900: 2020 2020 2020 2076 6572 626f 7365 3a20         verbose: 
+0000f910: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
+0000f920: 2056 6572 626f 7369 7479 206d 6f64 652e   Verbosity mode.
+0000f930: 0a20 2020 2020 2020 2075 7365 5f66 696c  .        use_fil
+0000f940: 7465 723a 2062 6f6f 6c20 6f72 2064 6963  ter: bool or dic
+0000f950: 740a 2020 2020 2020 2020 2020 2020 5768  t.            Wh
+0000f960: 6574 6865 7220 746f 2075 7365 2061 2066  ether to use a f
+0000f970: 696c 7465 7220 6f66 206e 6f74 2e20 4966  ilter of not. If
+0000f980: 2061 2064 6963 7469 6f6e 6172 7920 6973   a dictionary is
+0000f990: 2073 7065 6369 6669 6564 2c20 7468 6520   specified, the 
+0000f9a0: 6461 7461 2069 6e20 7468 6520 6469 6374  data in the dict
+0000f9b0: 2069 7320 636f 6e63 6174 656e 6174 6564   is concatenated
+0000f9c0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0000f9d0: 2075 7365 6420 6173 2066 696c 7465 722e   used as filter.
+0000f9e0: 0a20 2020 2020 2020 2063 6f72 7275 7074  .        corrupt
+0000f9f0: 5f73 6964 653a 2073 7472 0a20 2020 2020  _side: str.     
+0000fa00: 2020 2020 2020 2057 6869 6368 2073 6964         Which sid
+0000fa10: 6520 746f 2063 6f72 7275 7074 206f 6620  e to corrupt of 
+0000fa20: 6120 7472 6970 6c65 2074 6f20 636f 7272  a triple to corr
+0000fa30: 7570 742e 2049 7420 6361 6e20 6265 2074  upt. It can be t
+0000fa40: 6865 2073 7562 6a65 6374 2028 6060 636f  he subject (``co
+0000fa50: 7272 7570 745f 7369 7a65 3d22 7322 6060  rrupt_size="s"``
+0000fa60: 292c 0a20 2020 2020 2020 2020 2020 2074  ),.            t
+0000fa70: 6865 206f 626a 6563 7420 2860 6063 6f72  he object (``cor
+0000fa80: 7275 7074 5f73 697a 653d 226f 2260 6029  rupt_size="o"``)
+0000fa90: 2c20 7468 6520 7375 626a 6563 7420 616e  , the subject an
+0000faa0: 6420 7468 6520 6f62 6a65 6374 2028 6060  d the object (``
+0000fab0: 636f 7272 7570 745f 7369 7a65 3d22 732b  corrupt_size="s+
+0000fac0: 6f22 6060 206f 720a 2020 2020 2020 2020  o"`` or.        
+0000fad0: 2020 2020 6060 636f 7272 7570 745f 7369      ``corrupt_si
+0000fae0: 7a65 3d22 732c 6f22 6060 2920 2864 6566  ze="s,o"``) (def
+0000faf0: 6175 6c74 3a60 2273 2c6f 2260 292e 0a20  ault:`"s,o"`).. 
+0000fb00: 2020 2020 2020 2072 616e 6b69 6e67 5f73         ranking_s
+0000fb10: 7472 6174 6567 793a 2073 7472 0a20 2020  trategy: str.   
+0000fb20: 2020 2020 2020 2020 2049 6e64 6963 6174           Indicat
+0000fb30: 6573 2068 6f77 2074 6f20 6272 6561 6b20  es how to break 
+0000fb40: 7469 6573 2077 6865 6e20 6120 7465 7374  ties when a test
+0000fb50: 2074 7269 706c 6520 6765 7473 2074 6865   triple gets the
+0000fb60: 2073 616d 6520 7261 6e6b 206f 6620 6120   same rank of a 
+0000fb70: 636f 7272 7570 7469 6f6e 2e0a 2020 2020  corruption..    
+0000fb80: 2020 2020 2020 2020 4361 6e20 6265 206f          Can be o
+0000fb90: 6e65 206f 6620 7468 6520 7468 7265 6520  ne of the three 
+0000fba0: 7479 7065 733a 2060 2262 6573 7422 602c  types: `"best"`,
+0000fbb0: 2060 226d 6964 646c 6522 602c 2060 2277   `"middle"`, `"w
+0000fbc0: 6f72 7374 2260 2028 6465 6661 756c 743a  orst"` (default:
+0000fbd0: 2060 2277 6f72 7374 2260 2c20 692e 652e   `"worst"`, i.e.
+0000fbe0: 2c0a 2020 2020 2020 2020 2020 2020 7468  ,.            th
+0000fbf0: 6520 776f 7273 7420 7261 6e6b 2069 7320  e worst rank is 
+0000fc00: 6173 7369 676e 6564 2074 6f20 7468 6520  assigned to the 
+0000fc10: 7465 7374 2074 7269 706c 6529 2e0a 2020  test triple)..  
+0000fc20: 2020 2020 2020 656e 7469 7469 6573 5f73        entities_s
+0000fc30: 7562 7365 743a 206c 6973 7420 6f72 206e  ubset: list or n
+0000fc40: 702e 6172 7261 790a 2020 2020 2020 2020  p.array.        
+0000fc50: 2020 2020 5375 6273 6574 206f 6620 656e      Subset of en
+0000fc60: 7469 7469 6573 2074 6f20 6265 2075 7365  tities to be use
+0000fc70: 6420 666f 7220 6765 6e65 7261 7469 6e67  d for generating
+0000fc80: 2063 6f72 7275 7074 696f 6e73 2e0a 2020   corruptions..  
+0000fc90: 2020 2020 2020 6361 6c6c 6261 636b 733a        callbacks:
+0000fca0: 206c 6973 7420 6f66 206b 6572 6173 2e63   list of keras.c
+0000fcb0: 616c 6c62 6163 6b73 2e43 616c 6c62 6163  allbacks.Callbac
+0000fcc0: 6b20 696e 7374 616e 6365 730a 2020 2020  k instances.    
+0000fcd0: 2020 2020 2020 2020 4c69 7374 206f 6620          List of 
+0000fce0: 6361 6c6c 6261 636b 7320 746f 2061 7070  callbacks to app
+0000fcf0: 6c79 2064 7572 696e 6720 6576 616c 7561  ly during evalua
+0000fd00: 7469 6f6e 2e0a 0a20 2020 2020 2020 2052  tion...        R
+0000fd10: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+0000fd20: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2072  ------.        r
+0000fd30: 616e 6b3a 206e 702e 6172 7261 792c 2073  ank: np.array, s
+0000fd40: 6861 7065 2028 6e2c 206e 756d 6265 7220  hape (n, number 
+0000fd50: 6f66 2063 6f72 7275 7074 6564 2073 6964  of corrupted sid
+0000fd60: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
+0000fd70: 5261 6e6b 696e 6720 6f66 2074 6573 7420  Ranking of test 
+0000fd80: 7472 6970 6c65 7320 6167 6169 6e73 7420  triples against 
+0000fd90: 7375 626a 6563 7420 636f 7272 7570 7469  subject corrupti
+0000fda0: 6f6e 7320 616e 642f 6f72 206f 626a 6563  ons and/or objec
+0000fdb0: 7420 636f 7272 7570 7469 6f6e 732e 0a0a  t corruptions...
+0000fdc0: 2020 2020 2020 2020 4578 616d 706c 650a          Example.
+0000fdd0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+0000fde0: 2020 2020 2020 2020 3e3e 3e20 6672 6f6d          >>> from
+0000fdf0: 2061 6d70 6c69 6772 6170 682e 6461 7461   ampligraph.data
+0000fe00: 7365 7473 2069 6d70 6f72 7420 6c6f 6164  sets import load
+0000fe10: 5f66 6231 356b 5f32 3337 0a20 2020 2020  _fb15k_237.     
+0000fe20: 2020 203e 3e3e 2066 726f 6d20 616d 706c     >>> from ampl
+0000fe30: 6967 7261 7068 2e6c 6174 656e 745f 6665  igraph.latent_fe
+0000fe40: 6174 7572 6573 2069 6d70 6f72 7420 5363  atures import Sc
+0000fe50: 6f72 696e 6742 6173 6564 456d 6265 6464  oringBasedEmbedd
+0000fe60: 696e 674d 6f64 656c 0a20 2020 2020 2020  ingModel.       
+0000fe70: 203e 3e3e 2066 726f 6d20 616d 706c 6967   >>> from amplig
+0000fe80: 7261 7068 2e65 7661 6c75 6174 696f 6e2e  raph.evaluation.
+0000fe90: 6d65 7472 6963 7320 696d 706f 7274 206d  metrics import m
+0000fea0: 7272 5f73 636f 7265 2c20 6869 7473 5f61  rr_score, hits_a
+0000feb0: 745f 6e5f 7363 6f72 652c 206d 725f 7363  t_n_score, mr_sc
+0000fec0: 6f72 650a 2020 2020 2020 2020 3e3e 3e20  ore.        >>> 
+0000fed0: 5820 3d20 6c6f 6164 5f66 6231 356b 5f32  X = load_fb15k_2
+0000fee0: 3337 2829 0a20 2020 2020 2020 203e 3e3e  37().        >>>
+0000fef0: 206d 6f64 656c 203d 2053 636f 7269 6e67   model = Scoring
+0000ff00: 4261 7365 6445 6d62 6564 6469 6e67 4d6f  BasedEmbeddingMo
+0000ff10: 6465 6c28 6574 613d 352c 0a20 2020 2020  del(eta=5,.     
+0000ff20: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
+0000ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff40: 2020 2020 2020 2020 2020 6b3d 3330 302c            k=300,
+0000ff50: 0a20 2020 2020 2020 203e 3e3e 2020 2020  .        >>>    
+0000ff60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff80: 7363 6f72 696e 675f 7479 7065 3d27 436f  scoring_type='Co
+0000ff90: 6d70 6c45 7827 2c0a 2020 2020 2020 2020  mplEx',.        
+0000ffa0: 3e3e 3e20 2020 2020 2020 2020 2020 2020  >>>             
+0000ffb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffc0: 2020 2020 2020 2073 6565 643d 3029 0a20         seed=0). 
+0000ffd0: 2020 2020 2020 203e 3e3e 206d 6f64 656c         >>> model
+0000ffe0: 2e63 6f6d 7069 6c65 286f 7074 696d 697a  .compile(optimiz
+0000fff0: 6572 3d27 6164 616d 272c 206c 6f73 733d  er='adam', loss=
+00010000: 276e 6c6c 2729 0a20 2020 2020 2020 203e  'nll').        >
+00010010: 3e3e 206d 6f64 656c 2e66 6974 2858 5b27  >> model.fit(X['
+00010020: 7472 6169 6e27 5d2c 0a20 2020 2020 2020  train'],.       
+00010030: 203e 3e3e 2020 2020 2020 2020 2020 2062   >>>           b
+00010040: 6174 6368 5f73 697a 653d 3130 3030 302c  atch_size=10000,
+00010050: 0a20 2020 2020 2020 203e 3e3e 2020 2020  .        >>>    
+00010060: 2020 2020 2020 2065 706f 6368 733d 3529         epochs=5)
+00010070: 0a20 2020 2020 2020 2045 706f 6368 2031  .        Epoch 1
+00010080: 2f35 0a20 2020 2020 2020 2032 392f 3239  /5.        29/29
+00010090: 205b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   [==============
+000100a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000100b0: 5d20 2d20 3273 2037 316d 732f 7374 6570  ] - 2s 71ms/step
+000100c0: 202d 206c 6f73 733a 2036 3733 3631 2e33   - loss: 67361.3
+000100d0: 3034 370a 2020 2020 2020 2020 4570 6f63  047.        Epoc
+000100e0: 6820 322f 350a 2020 2020 2020 2020 3239  h 2/5.        29
+000100f0: 2f32 3920 5b3d 3d3d 3d3d 3d3d 3d3d 3d3d  /29 [===========
+00010100: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010110: 3d3d 3d5d 202d 2031 7320 3335 6d73 2f73  ===] - 1s 35ms/s
+00010120: 7465 7020 2d20 6c6f 7373 3a20 3637 3331  tep - loss: 6731
+00010130: 382e 3630 3934 0a20 2020 2020 2020 2045  8.6094.        E
+00010140: 706f 6368 2033 2f35 0a20 2020 2020 2020  poch 3/5.       
+00010150: 2032 392f 3239 205b 3d3d 3d3d 3d3d 3d3d   29/29 [========
+00010160: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010170: 3d3d 3d3d 3d3d 5d20 2d20 3173 2033 356d  ======] - 1s 35m
+00010180: 732f 7374 6570 202d 206c 6f73 733a 2036  s/step - loss: 6
+00010190: 3730 3230 2e30 3730 330a 2020 2020 2020  7020.0703.      
+000101a0: 2020 4570 6f63 6820 342f 350a 2020 2020    Epoch 4/5.    
+000101b0: 2020 2020 3239 2f32 3920 5b3d 3d3d 3d3d      29/29 [=====
+000101c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000101d0: 3d3d 3d3d 3d3d 3d3d 3d5d 202d 2031 7320  =========] - 1s 
+000101e0: 3333 6d73 2f73 7465 7020 2d20 6c6f 7373  33ms/step - loss
+000101f0: 3a20 3635 3836 372e 3337 3530 0a20 2020  : 65867.3750.   
+00010200: 2020 2020 2045 706f 6368 2035 2f35 0a20       Epoch 5/5. 
+00010210: 2020 2020 2020 2032 392f 3239 205b 3d3d         29/29 [==
+00010220: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010230: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 5d20 2d20  ============] - 
+00010240: 3173 2033 346d 732f 7374 6570 202d 206c  1s 34ms/step - l
+00010250: 6f73 733a 2036 3335 3137 2e39 3036 320a  oss: 63517.9062.
+00010260: 2020 2020 2020 2020 3e3e 3e20 7261 6e6b          >>> rank
+00010270: 7320 3d20 6d6f 6465 6c2e 6576 616c 7561  s = model.evalua
+00010280: 7465 2858 5b27 7465 7374 275d 2c0a 2020  te(X['test'],.  
+00010290: 2020 2020 2020 3e3e 3e20 2020 2020 2020        >>>       
+000102a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102b0: 2062 6174 6368 5f73 697a 653d 3130 302c   batch_size=100,
+000102c0: 0a20 2020 2020 2020 203e 3e3e 2020 2020  .        >>>    
+000102d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102e0: 2020 2020 636f 7272 7570 745f 7369 6465      corrupt_side
+000102f0: 3d27 732c 6f27 2c0a 2020 2020 2020 2020  ='s,o',.        
+00010300: 3e3e 3e20 2020 2020 2020 2020 2020 2020  >>>             
+00010310: 2020 2020 2020 2020 2020 2075 7365 5f66             use_f
+00010320: 696c 7465 723d 7b27 7472 6169 6e27 3a20  ilter={'train': 
+00010330: 585b 2774 7261 696e 275d 2c0a 2020 2020  X['train'],.    
+00010340: 2020 2020 3e3e 3e20 2020 2020 2020 2020      >>>         
+00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010360: 2020 2020 2020 2020 2020 2027 7661 6c69             'vali
+00010370: 6427 3a20 585b 2776 616c 6964 275d 2c0a  d': X['valid'],.
+00010380: 2020 2020 2020 2020 3e3e 3e20 2020 2020          >>>     
+00010390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103a0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000103b0: 7465 7374 273a 2058 5b27 7465 7374 275d  test': X['test']
+000103c0: 290a 2020 2020 2020 2020 3e3e 3e20 6d72  ).        >>> mr
+000103d0: 5f73 636f 7265 2872 616e 6b73 292c 206d  _score(ranks), m
+000103e0: 7272 5f73 636f 7265 2872 616e 6b73 292c  rr_score(ranks),
+000103f0: 2068 6974 735f 6174 5f6e 5f73 636f 7265   hits_at_n_score
+00010400: 2872 616e 6b73 2c20 3129 2c20 6869 7473  (ranks, 1), hits
+00010410: 5f61 745f 6e5f 7363 6f72 6528 7261 6e6b  _at_n_score(rank
+00010420: 732c 2031 3029 2c20 6c65 6e28 7261 6e6b  s, 10), len(rank
+00010430: 7329 0a20 2020 2020 2020 2032 3820 7472  s).        28 tr
+00010440: 6970 6c65 7320 636f 6e74 6169 6e69 6e67  iples containing
+00010450: 2069 6e76 616c 6964 206b 6579 7320 736b   invalid keys sk
+00010460: 6970 7065 6421 0a20 2020 2020 2020 2039  ipped!.        9
+00010470: 2074 7269 706c 6573 2063 6f6e 7461 696e   triples contain
+00010480: 696e 6720 696e 7661 6c69 6420 6b65 7973  ing invalid keys
+00010490: 2073 6b69 7070 6564 210a 2020 2020 2020   skipped!.      
+000104a0: 2020 3230 3435 2f32 3034 3520 5b3d 3d3d    2045/2045 [===
+000104b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000104c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d5d 202d 2031  ===========] - 1
+000104d0: 3439 7320 3733 6d73 2f73 7465 700a 2020  49s 73ms/step.  
+000104e0: 2020 2020 2020 2834 3238 2e34 3436 3731        (428.44671
+000104f0: 3638 3939 3839 3233 352c 0a20 2020 2020  689989235,.     
+00010500: 2020 2020 302e 3235 3736 3130 3431 3032      0.2576104102
+00010510: 3532 3832 3331 362c 0a20 2020 2020 2020  5282316,.       
+00010520: 2020 302e 3138 3938 3137 3938 3631 3034    0.189817986104
+00010530: 3331 3535 2c0a 2020 2020 2020 2020 2030  3155,.         0
+00010540: 2e33 3931 3936 3539 3435 3738 3732 3539  .391965945787259
+00010550: 2c0a 2020 2020 2020 2020 2032 3034 3338  ,.         20438
+00010560: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
+00010570: 2020 2020 2020 2320 6765 7420 7468 6520        # get the 
+00010580: 7465 7374 2073 6574 2068 616e 646c 6572  test set handler
+00010590: 0a20 2020 2020 2020 2073 656c 662e 6461  .        self.da
+000105a0: 7461 5f68 616e 646c 6572 5f74 6573 7420  ta_handler_test 
+000105b0: 3d20 6461 7461 5f61 6461 7074 6572 2e44  = data_adapter.D
+000105c0: 6174 6148 616e 646c 6572 280a 2020 2020  ataHandler(.    
+000105d0: 2020 2020 2020 2020 782c 0a20 2020 2020          x,.     
+000105e0: 2020 2020 2020 2062 6174 6368 5f73 697a         batch_siz
+000105f0: 653d 6261 7463 685f 7369 7a65 2c0a 2020  e=batch_size,.  
+00010600: 2020 2020 2020 2020 2020 6461 7461 7365            datase
+00010610: 745f 7479 7065 3d64 6174 6173 6574 5f74  t_type=dataset_t
+00010620: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
+00010630: 2065 706f 6368 733d 312c 0a20 2020 2020   epochs=1,.     
+00010640: 2020 2020 2020 2075 7365 5f66 696c 7465         use_filte
+00010650: 723d 7573 655f 6669 6c74 6572 2c0a 2020  r=use_filter,.  
+00010660: 2020 2020 2020 2020 2020 7573 655f 696e            use_in
+00010670: 6465 7865 723d 7365 6c66 2e64 6174 615f  dexer=self.data_
+00010680: 696e 6465 7865 722c 0a20 2020 2020 2020  indexer,.       
+00010690: 2029 0a0a 2020 2020 2020 2020 6173 7365   )..        asse
+000106a0: 7274 2063 6f72 7275 7074 5f73 6964 6520  rt corrupt_side 
+000106b0: 696e 205b 0a20 2020 2020 2020 2020 2020  in [.           
+000106c0: 2022 7322 2c0a 2020 2020 2020 2020 2020   "s",.          
+000106d0: 2020 226f 222c 0a20 2020 2020 2020 2020    "o",.         
+000106e0: 2020 2022 732c 6f22 2c0a 2020 2020 2020     "s,o",.      
+000106f0: 2020 2020 2020 2273 2b6f 222c 0a20 2020        "s+o",.   
+00010700: 2020 2020 205d 2c20 2249 6e76 616c 6964       ], "Invalid
+00010710: 2076 616c 7565 2066 6f72 2063 6f72 7275   value for corru
+00010720: 7074 5f73 6964 6522 0a20 2020 2020 2020  pt_side".       
+00010730: 2061 7373 6572 7420 7261 6e6b 696e 675f   assert ranking_
+00010740: 7374 7261 7465 6779 2069 6e20 5b0a 2020  strategy in [.  
+00010750: 2020 2020 2020 2020 2020 2262 6573 7422            "best"
+00010760: 2c0a 2020 2020 2020 2020 2020 2020 226d  ,.            "m
+00010770: 6964 646c 6522 2c0a 2020 2020 2020 2020  iddle",.        
+00010780: 2020 2020 2277 6f72 7374 222c 0a20 2020      "worst",.   
+00010790: 2020 2020 205d 2c20 2249 6e76 616c 6964       ], "Invalid
+000107a0: 2076 616c 7565 2066 6f72 2072 616e 6b69   value for ranki
+000107b0: 6e67 5f73 7472 6174 6567 7922 0a0a 2020  ng_strategy"..  
+000107c0: 2020 2020 2020 7365 6c66 2e63 6f72 7275        self.corru
+000107d0: 7074 5f73 6964 6520 3d20 636f 7272 7570  pt_side = corrup
+000107e0: 745f 7369 6465 0a20 2020 2020 2020 2073  t_side.        s
+000107f0: 656c 662e 7261 6e6b 696e 675f 7374 7261  elf.ranking_stra
+00010800: 7465 6779 203d 2072 616e 6b69 6e67 5f73  tegy = ranking_s
+00010810: 7472 6174 6567 790a 0a20 2020 2020 2020  trategy..       
 00010820: 2073 656c 662e 656e 7469 7469 6573 5f73   self.entities_s
 00010830: 7562 7365 7420 3d20 7466 2e63 6f6e 7374  ubset = tf.const
-00010840: 616e 7428 656e 7469 7469 6573 5f73 7562  ant(entities_sub
-00010850: 7365 742c 2064 7479 7065 3d74 662e 696e  set, dtype=tf.in
-00010860: 7433 3229 0a20 2020 2020 2020 2020 2020  t32).           
-00010870: 2073 656c 662e 6d61 7070 696e 675f 6469   self.mapping_di
-00010880: 6374 2e69 6e73 6572 7428 0a20 2020 2020  ct.insert(.     
-00010890: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000108a0: 656e 7469 7469 6573 5f73 7562 7365 742c  entities_subset,
-000108b0: 2074 662e 7261 6e67 6528 7365 6c66 2e65   tf.range(self.e
-000108c0: 6e74 6974 6965 735f 7375 6273 6574 2e73  ntities_subset.s
-000108d0: 6861 7065 5b30 5d29 0a20 2020 2020 2020  hape[0]).       
-000108e0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-000108f0: 2320 666c 6167 2074 6f20 696e 6469 6361  # flag to indica
-00010900: 7465 2069 6620 7765 2061 7265 2075 7369  te if we are usi
-00010910: 6e67 2066 696c 7465 7220 6f72 206e 6f74  ng filter or not
-00010920: 0a20 2020 2020 2020 2073 656c 662e 7573  .        self.us
-00010930: 655f 6669 6c74 6572 203d 2028 0a20 2020  e_filter = (.   
-00010940: 2020 2020 2020 2020 2073 656c 662e 6461           self.da
-00010950: 7461 5f68 616e 646c 6572 5f74 6573 742e  ta_handler_test.
-00010960: 5f70 6172 656e 745f 6164 6170 7465 722e  _parent_adapter.
-00010970: 6261 636b 656e 642e 7573 655f 6669 6c74  backend.use_filt
-00010980: 6572 0a20 2020 2020 2020 2020 2020 206f  er.            o
-00010990: 7220 6973 696e 7374 616e 6365 280a 2020  r isinstance(.  
-000109a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000109b0: 6c66 2e64 6174 615f 6861 6e64 6c65 725f  lf.data_handler_
-000109c0: 7465 7374 2e5f 7061 7265 6e74 5f61 6461  test._parent_ada
-000109d0: 7074 6572 2e62 6163 6b65 6e64 2e75 7365  pter.backend.use
-000109e0: 5f66 696c 7465 722c 2064 6963 740a 2020  _filter, dict.  
-000109f0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00010a00: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-00010a10: 2043 6f6e 7461 696e 6572 2074 6861 7420   Container that 
-00010a20: 636f 6e66 6967 7572 6573 2061 6e64 2063  configures and c
-00010a30: 616c 6c73 2060 7466 2e6b 6572 6173 2e43  alls `tf.keras.C
-00010a40: 616c 6c62 6163 6b60 732e 0a20 2020 2020  allback`s..     
-00010a50: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-00010a60: 616e 6365 2863 616c 6c62 6163 6b73 2c20  ance(callbacks, 
-00010a70: 6361 6c6c 6261 636b 735f 6d6f 6475 6c65  callbacks_module
-00010a80: 2e43 616c 6c62 6163 6b4c 6973 7429 3a0a  .CallbackList):.
-00010a90: 2020 2020 2020 2020 2020 2020 6361 6c6c              call
-00010aa0: 6261 636b 7320 3d20 6361 6c6c 6261 636b  backs = callback
-00010ab0: 735f 6d6f 6475 6c65 2e43 616c 6c62 6163  s_module.Callbac
-00010ac0: 6b4c 6973 7428 0a20 2020 2020 2020 2020  kList(.         
-00010ad0: 2020 2020 2020 2063 616c 6c62 6163 6b73         callbacks
-00010ae0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010af0: 2020 6164 645f 6869 7374 6f72 793d 5472    add_history=Tr
-00010b00: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00010b10: 2020 2020 6164 645f 7072 6f67 6261 723d      add_progbar=
-00010b20: 7665 7262 6f73 6520 213d 2030 2c0a 2020  verbose != 0,.  
-00010b30: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
-00010b40: 6465 6c3d 7365 6c66 2c0a 2020 2020 2020  del=self,.      
-00010b50: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
-00010b60: 653d 7665 7262 6f73 652c 0a20 2020 2020  e=verbose,.     
-00010b70: 2020 2020 2020 2020 2020 2065 706f 6368             epoch
-00010b80: 733d 312c 0a20 2020 2020 2020 2020 2020  s=1,.           
-00010b90: 2020 2020 2073 7465 7073 3d73 656c 662e       steps=self.
-00010ba0: 6461 7461 5f68 616e 646c 6572 5f74 6573  data_handler_tes
-00010bb0: 742e 696e 6665 7272 6564 5f73 7465 7073  t.inferred_steps
-00010bc0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00010bd0: 0a20 2020 2020 2020 2074 6573 745f 6675  .        test_fu
-00010be0: 6e63 7469 6f6e 203d 2073 656c 662e 6d61  nction = self.ma
-00010bf0: 6b65 5f74 6573 745f 6675 6e63 7469 6f6e  ke_test_function
-00010c00: 2829 0a0a 2020 2020 2020 2020 2320 6265  ()..        # be
-00010c10: 666f 7265 2074 6573 7420 6265 6769 6e73  fore test begins
-00010c20: 2063 616c 6c20 7468 6973 2063 616c 6c62   call this callb
-00010c30: 6163 6b20 6675 6e63 7469 6f6e 0a20 2020  ack function.   
-00010c40: 2020 2020 2063 616c 6c62 6163 6b73 2e6f       callbacks.o
-00010c50: 6e5f 7465 7374 5f62 6567 696e 2829 0a0a  n_test_begin()..
-00010c60: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00010c70: 5f72 616e 6b73 203d 205b 5d0a 0a20 2020  _ranks = []..   
-00010c80: 2020 2020 2023 2065 6e75 6d65 7261 7465       # enumerate
-00010c90: 206f 7665 7220 7468 6520 6461 7461 0a20   over the data. 
-00010ca0: 2020 2020 2020 2066 6f72 205f 2c20 6974         for _, it
-00010cb0: 6572 6174 6f72 2069 6e20 7365 6c66 2e64  erator in self.d
-00010cc0: 6174 615f 6861 6e64 6c65 725f 7465 7374  ata_handler_test
-00010cd0: 2e65 6e75 6d65 7261 7465 5f65 706f 6368  .enumerate_epoch
-00010ce0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00010cf0: 2023 2068 616e 646c 6520 7468 6520 7374   # handle the st
-00010d00: 6f70 2069 7465 7261 7469 6f6e 206f 6620  op iteration of 
-00010d10: 6461 7461 2069 7465 7261 746f 7220 696e  data iterator in
-00010d20: 2074 6869 7320 7363 6f70 650a 2020 2020   this scope.    
-00010d30: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00010d40: 662e 6461 7461 5f68 616e 646c 6572 5f74  f.data_handler_t
-00010d50: 6573 742e 6361 7463 685f 7374 6f70 5f69  est.catch_stop_i
-00010d60: 7465 7261 7469 6f6e 2829 3a0a 2020 2020  teration():.    
-00010d70: 2020 2020 2020 2020 2020 2020 2320 6974              # it
-00010d80: 6572 6174 6520 6f76 6572 2074 6865 2064  erate over the d
-00010d90: 6174 6173 6574 0a20 2020 2020 2020 2020  ataset.         
-00010da0: 2020 2020 2020 2066 6f72 2073 7465 7020         for step 
-00010db0: 696e 2073 656c 662e 6461 7461 5f68 616e  in self.data_han
-00010dc0: 646c 6572 5f74 6573 742e 7374 6570 7328  dler_test.steps(
-00010dd0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00010de0: 2020 2020 2020 2023 2062 6566 6f72 6520         # before 
-00010df0: 6120 6261 7463 6820 6973 2070 726f 6365  a batch is proce
-00010e00: 7373 6564 2063 616c 6c20 7468 6973 2063  ssed call this c
-00010e10: 616c 6c62 6163 6b20 6675 6e63 7469 6f6e  allback function
-00010e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010e30: 2020 2020 2063 616c 6c62 6163 6b73 2e6f       callbacks.o
-00010e40: 6e5f 7465 7374 5f62 6174 6368 5f62 6567  n_test_batch_beg
-00010e50: 696e 2873 7465 7029 0a0a 2020 2020 2020  in(step)..      
-00010e60: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00010e70: 7072 6f63 6573 7320 7468 6973 2062 6174  process this bat
-00010e80: 6368 0a20 2020 2020 2020 2020 2020 2020  ch.             
-00010e90: 2020 2020 2020 206f 7665 7261 6c6c 5f72         overall_r
-00010ea0: 616e 6b20 3d20 7465 7374 5f66 756e 6374  ank = test_funct
-00010eb0: 696f 6e28 6974 6572 6174 6f72 290a 2020  ion(iterator).  
-00010ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ed0: 2020 2320 696e 6372 656d 656e 7420 7468    # increment th
-00010ee0: 6520 7261 6e6b 2062 7920 3120 2872 616e  e rank by 1 (ran
-00010ef0: 6b73 2072 6574 7572 6e65 6420 6172 6520  ks returned are 
-00010f00: 6672 6f6d 2028 3020 2d0a 2020 2020 2020  from (0 -.      
-00010f10: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00010f20: 6e2d 3129 2073 6f20 696e 6372 656d 656e  n-1) so incremen
-00010f30: 7420 6279 2031 0a20 2020 2020 2020 2020  t by 1.         
-00010f40: 2020 2020 2020 2020 2020 206f 7665 7261             overa
-00010f50: 6c6c 5f72 616e 6b20 2b3d 2031 0a20 2020  ll_rank += 1.   
-00010f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f70: 2023 2073 6176 6520 7468 6520 7261 6e6b   # save the rank
-00010f80: 7320 6f66 2074 6865 2062 6174 6368 2074  s of the batch t
-00010f90: 7269 706c 6573 0a20 2020 2020 2020 2020  riples.         
-00010fa0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010fb0: 616c 6c5f 7261 6e6b 732e 6170 7065 6e64  all_ranks.append
-00010fc0: 286f 7665 7261 6c6c 5f72 616e 6b29 0a20  (overall_rank). 
-00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fe0: 2020 2023 2061 6674 6572 2061 2062 6174     # after a bat
-00010ff0: 6368 2069 7320 7072 6f63 6573 7365 6420  ch is processed 
-00011000: 6361 6c6c 2074 6869 7320 6361 6c6c 6261  call this callba
-00011010: 636b 2066 756e 6374 696f 6e0a 2020 2020  ck function.    
-00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011030: 6361 6c6c 6261 636b 732e 6f6e 5f74 6573  callbacks.on_tes
-00011040: 745f 6261 7463 685f 656e 6428 7374 6570  t_batch_end(step
-00011050: 290a 2020 2020 2020 2020 2320 6f6e 2074  ).        # on t
-00011060: 6573 7420 656e 6420 6361 6c6c 2074 6869  est end call thi
-00011070: 7320 6d65 7468 6f64 0a20 2020 2020 2020  s method.       
-00011080: 2063 616c 6c62 6163 6b73 2e6f 6e5f 7465   callbacks.on_te
-00011090: 7374 5f65 6e64 2829 0a20 2020 2020 2020  st_end().       
-000110a0: 2023 2072 6574 7572 6e20 7261 6e6b 730a   # return ranks.
-000110b0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
-000110c0: 702e 636f 6e63 6174 656e 6174 6528 7365  p.concatenate(se
-000110d0: 6c66 2e61 6c6c 5f72 616e 6b73 290a 0a20  lf.all_ranks).. 
-000110e0: 2020 2064 6566 2070 7265 6469 6374 5f73     def predict_s
-000110f0: 7465 7028 7365 6c66 2c20 696e 7075 7473  tep(self, inputs
-00011100: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
-00011110: 7475 726e 7320 7468 6520 6f75 7470 7574  turns the output
-00011120: 206f 6620 7072 6564 6963 7420 7374 6570   of predict step
-00011130: 206f 6e20 6120 6261 7463 6820 6f66 2064   on a batch of d
-00011140: 6174 612e 2222 220a 2020 2020 2020 2020  ata.""".        
-00011150: 6966 2073 656c 662e 6461 7461 5f73 6861  if self.data_sha
-00011160: 7065 203e 2033 2061 6e64 2069 7369 6e73  pe > 3 and isins
-00011170: 7461 6e63 6528 696e 7075 7473 2c20 7475  tance(inputs, tu
-00011180: 706c 6529 3a0a 2020 2020 2020 2020 2020  ple):.          
-00011190: 2020 696e 7075 7473 203d 2069 6e70 7574    inputs = input
-000111a0: 735b 305d 0a20 2020 2020 2020 2073 636f  s[0].        sco
-000111b0: 7265 5f70 6f73 203d 2073 656c 6628 696e  re_pos = self(in
-000111c0: 7075 7473 2c20 4661 6c73 6529 0a20 2020  puts, False).   
-000111d0: 2020 2020 2072 6574 7572 6e20 7363 6f72       return scor
-000111e0: 655f 706f 730a 0a20 2020 2064 6566 2070  e_pos..    def p
-000111f0: 7265 6469 6374 5f73 7465 705f 7061 7274  redict_step_part
-00011200: 6974 696f 6e69 6e67 2873 656c 662c 2069  itioning(self, i
-00011210: 6e70 7574 7329 3a0a 2020 2020 2020 2020  nputs):.        
-00011220: 2222 2252 6574 7572 6e73 2074 6865 206f  """Returns the o
-00011230: 7574 7075 7420 6f66 2070 7265 6469 6374  utput of predict
-00011240: 2073 7465 7020 6f6e 2061 2062 6174 6368   step on a batch
-00011250: 206f 6620 6461 7461 2e22 2222 0a20 2020   of data.""".   
-00011260: 2020 2020 2073 636f 7265 5f70 6f73 203d       score_pos =
-00011270: 2073 656c 662e 7363 6f72 696e 675f 6c61   self.scoring_la
-00011280: 7965 7228 696e 7075 7473 290a 2020 2020  yer(inputs).    
-00011290: 2020 2020 7265 7475 726e 2073 636f 7265      return score
-000112a0: 5f70 6f73 0a0a 2020 2020 6465 6620 6d61  _pos..    def ma
-000112b0: 6b65 5f70 7265 6469 6374 5f66 756e 6374  ke_predict_funct
-000112c0: 696f 6e28 7365 6c66 293a 0a20 2020 2020  ion(self):.     
-000112d0: 2020 2022 2222 5369 6d69 6c61 7220 746f     """Similar to
-000112e0: 206b 6572 6173 206c 6962 2c20 7468 6973   keras lib, this
-000112f0: 2066 756e 6374 696f 6e20 7265 7475 726e   function return
-00011300: 7320 7468 6520 6861 6e64 6c65 2074 6f20  s the handle to 
-00011310: 7468 6520 7072 6564 6963 7420 7374 6570  the predict step
-00011320: 2066 756e 6374 696f 6e2e 0a0a 2020 2020   function...    
-00011330: 2020 2020 4974 2070 726f 6365 7373 6573      It processes
-00011340: 206f 6e65 2062 6174 6368 206f 6620 6461   one batch of da
-00011350: 7461 2062 7920 6974 6572 6174 696e 6720  ta by iterating 
-00011360: 6f76 6572 2074 6865 2064 6174 6173 6574  over the dataset
-00011370: 2069 7465 7261 746f 7220 616e 6420 636f   iterator and co
-00011380: 6d70 7574 6573 2074 6865 2070 7265 6469  mputes the predi
-00011390: 6374 696f 6e20 6f75 7470 7574 732e 0a0a  ction outputs...
-000113a0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-000113b0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-000113c0: 2020 2020 2020 2020 6f75 743a 2046 756e          out: Fun
-000113d0: 6374 696f 6e20 6861 6e64 6c65 0a20 2020  ction handle.   
-000113e0: 2020 2020 2020 2020 2020 2048 616e 646c             Handl
-000113f0: 6520 746f 2074 6865 2070 7265 6469 6374  e to the predict
-00011400: 2066 756e 6374 696f 6e2e 0a20 2020 2020   function..     
-00011410: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00011420: 6620 7365 6c66 2e70 7265 6469 6374 5f66  f self.predict_f
-00011430: 756e 6374 696f 6e20 6973 206e 6f74 204e  unction is not N
-00011440: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00011450: 2072 6574 7572 6e20 7365 6c66 2e70 7265   return self.pre
-00011460: 6469 6374 5f66 756e 6374 696f 6e0a 0a20  dict_function.. 
-00011470: 2020 2020 2020 2064 6566 2070 7265 6469         def predi
-00011480: 6374 5f66 756e 6374 696f 6e28 6974 6572  ct_function(iter
-00011490: 6174 6f72 293a 0a20 2020 2020 2020 2020  ator):.         
-000114a0: 2020 2069 6e70 7574 7320 3d20 6e65 7874     inputs = next
-000114b0: 2869 7465 7261 746f 7229 0a20 2020 2020  (iterator).     
-000114c0: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
-000114d0: 735f 7061 7274 6974 696f 6e65 645f 7472  s_partitioned_tr
-000114e0: 6169 6e69 6e67 3a0a 2020 2020 2020 2020  aining:.        
-000114f0: 2020 2020 2020 2020 696e 7075 7473 203d          inputs =
-00011500: 2073 656c 662e 7072 6f63 6573 735f 6d6f   self.process_mo
-00011510: 6465 6c5f 696e 7075 7473 5f66 6f72 5f74  del_inputs_for_t
-00011520: 6573 7428 696e 7075 7473 290a 2020 2020  est(inputs).    
-00011530: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-00011540: 7574 7320 3d20 7365 6c66 2e70 7265 6469  uts = self.predi
-00011550: 6374 5f73 7465 705f 7061 7274 6974 696f  ct_step_partitio
-00011560: 6e69 6e67 2869 6e70 7574 7329 0a20 2020  ning(inputs).   
-00011570: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00011580: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00011590: 7574 7075 7473 203d 2073 656c 662e 7072  utputs = self.pr
-000115a0: 6564 6963 745f 7374 6570 2869 6e70 7574  edict_step(input
-000115b0: 7329 0a20 2020 2020 2020 2020 2020 2072  s).            r
-000115c0: 6574 7572 6e20 6f75 7470 7574 730a 0a20  eturn outputs.. 
-000115d0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-000115e0: 6c66 2e72 756e 5f65 6167 6572 6c79 2061  lf.run_eagerly a
-000115f0: 6e64 206e 6f74 2073 656c 662e 6973 5f70  nd not self.is_p
-00011600: 6172 7469 7469 6f6e 6564 5f74 7261 696e  artitioned_train
-00011610: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
-00011620: 2070 7265 6469 6374 5f66 756e 6374 696f   predict_functio
-00011630: 6e20 3d20 6465 665f 6675 6e63 7469 6f6e  n = def_function
-00011640: 2e66 756e 6374 696f 6e28 0a20 2020 2020  .function(.     
-00011650: 2020 2020 2020 2020 2020 2070 7265 6469             predi
-00011660: 6374 5f66 756e 6374 696f 6e2c 2065 7870  ct_function, exp
-00011670: 6572 696d 656e 7461 6c5f 7265 6c61 785f  erimental_relax_
-00011680: 7368 6170 6573 3d54 7275 650a 2020 2020  shapes=True.    
-00011690: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-000116a0: 2020 2073 656c 662e 7072 6564 6963 745f     self.predict_
-000116b0: 6675 6e63 7469 6f6e 203d 2070 7265 6469  function = predi
-000116c0: 6374 5f66 756e 6374 696f 6e0a 2020 2020  ct_function.    
-000116d0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000116e0: 7072 6564 6963 745f 6675 6e63 7469 6f6e  predict_function
-000116f0: 0a0a 2020 2020 6465 6620 7072 6564 6963  ..    def predic
-00011700: 7428 7365 6c66 2c20 782c 2062 6174 6368  t(self, x, batch
-00011710: 5f73 697a 653d 3332 2c20 7665 7262 6f73  _size=32, verbos
-00011720: 653d 302c 2063 616c 6c62 6163 6b73 3d4e  e=0, callbacks=N
-00011730: 6f6e 6529 3a0a 2020 2020 2020 2020 2222  one):.        ""
-00011740: 220a 2020 2020 2020 2020 436f 6d70 7574  ".        Comput
-00011750: 6520 7363 6f72 6573 206f 6620 7468 6520  e scores of the 
-00011760: 696e 7075 7420 7472 6970 6c65 732e 0a0a  input triples...
-00011770: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00011780: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-00011790: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2078  ------.        x
-000117a0: 3a20 6e70 2e61 7272 6179 2c20 7368 6170  : np.array, shap
-000117b0: 6520 286e 2c20 3329 206f 7220 7374 7220  e (n, 3) or str 
-000117c0: 6f72 2047 7261 7068 4461 7461 4c6f 6164  or GraphDataLoad
-000117d0: 6572 206f 7220 4162 7374 7261 6374 4772  er or AbstractGr
-000117e0: 6170 6850 6172 7469 7469 6f6e 6572 0a20  aphPartitioner. 
-000117f0: 2020 2020 2020 2020 2020 2044 6174 6120             Data 
-00011800: 4f52 2046 696c 656e 616d 6520 6f66 2074  OR Filename of t
-00011810: 6865 2064 6174 6120 6669 6c65 204f 5220  he data file OR 
-00011820: 4461 7461 2048 616e 646c 6520 746f 2062  Data Handle to b
-00011830: 6520 7573 6564 2066 6f72 2074 7261 696e  e used for train
-00011840: 696e 672e 0a20 2020 2020 2020 2062 6174  ing..        bat
-00011850: 6368 5f73 697a 653a 2069 6e74 0a20 2020  ch_size: int.   
-00011860: 2020 2020 2020 2020 2042 6174 6368 2073           Batch s
-00011870: 697a 6520 746f 2075 7365 2064 7572 696e  ize to use durin
-00011880: 6720 7472 6169 6e69 6e67 2e0a 2020 2020  g training..    
-00011890: 2020 2020 2020 2020 4d61 7920 6265 206f          May be o
-000118a0: 7665 7272 6964 6465 6e20 6966 2060 6078  verridden if ``x
-000118b0: 6060 2069 7320 6047 7261 7068 4461 7461  `` is `GraphData
-000118c0: 4c6f 6164 6572 6020 6f72 2060 4162 7374  Loader` or `Abst
-000118d0: 7261 6374 4772 6170 6850 6172 7469 7469  ractGraphPartiti
-000118e0: 6f6e 6572 6020 696e 7374 616e 6365 0a20  oner` instance. 
-000118f0: 2020 2020 2020 2076 6572 626f 7365 3a20         verbose: 
-00011900: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
-00011910: 2056 6572 626f 7369 7479 206d 6f64 652e   Verbosity mode.
-00011920: 0a20 2020 2020 2020 2063 616c 6c62 6163  .        callbac
-00011930: 6b73 3a20 6c69 7374 206f 6620 6b65 7261  ks: list of kera
-00011940: 732e 6361 6c6c 6261 636b 732e 4361 6c6c  s.callbacks.Call
-00011950: 6261 636b 2069 6e73 7461 6e63 6573 0a20  back instances. 
-00011960: 2020 2020 2020 2020 2020 204c 6973 7420             List 
-00011970: 6f66 2063 616c 6c62 6163 6b73 2074 6f20  of callbacks to 
-00011980: 6170 706c 7920 6475 7269 6e67 2065 7661  apply during eva
-00011990: 6c75 6174 696f 6e2e 0a0a 2020 2020 2020  luation...      
-000119a0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-000119b0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-000119c0: 2020 7363 6f72 6573 3a20 6e70 2e61 7272    scores: np.arr
-000119d0: 6179 2c20 7368 6170 6520 286e 2c20 290a  ay, shape (n, ).
-000119e0: 2020 2020 2020 2020 2020 2020 5363 6f72              Scor
-000119f0: 6520 6f66 2074 6865 2069 6e70 7574 2074  e of the input t
-00011a00: 7269 706c 6573 2e0a 0a20 2020 2020 2020  riples...       
-00011a10: 2045 7861 6d70 6c65 0a20 2020 2020 2020   Example.       
-00011a20: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00011a30: 203e 3e3e 2066 726f 6d20 616d 706c 6967   >>> from amplig
-00011a40: 7261 7068 2e6c 6174 656e 745f 6665 6174  raph.latent_feat
-00011a50: 7572 6573 2069 6d70 6f72 7420 5363 6f72  ures import Scor
-00011a60: 696e 6742 6173 6564 456d 6265 6464 696e  ingBasedEmbeddin
-00011a70: 674d 6f64 656c 0a20 2020 2020 2020 203e  gModel.        >
-00011a80: 3e3e 2069 6d70 6f72 7420 6e75 6d70 7920  >> import numpy 
-00011a90: 6173 206e 700a 2020 2020 2020 2020 3e3e  as np.        >>
-00011aa0: 3e20 6672 6f6d 2061 6d70 6c69 6772 6170  > from ampligrap
-00011ab0: 682e 6461 7461 7365 7473 2069 6d70 6f72  h.datasets impor
-00011ac0: 7420 6c6f 6164 5f66 6231 356b 5f32 3337  t load_fb15k_237
-00011ad0: 0a20 2020 2020 2020 203e 3e3e 2058 203d  .        >>> X =
-00011ae0: 206c 6f61 645f 6662 3135 6b5f 3233 3728   load_fb15k_237(
-00011af0: 290a 2020 2020 2020 2020 3e3e 3e20 6d6f  ).        >>> mo
-00011b00: 6465 6c20 3d20 5363 6f72 696e 6742 6173  del = ScoringBas
-00011b10: 6564 456d 6265 6464 696e 674d 6f64 656c  edEmbeddingModel
-00011b20: 2865 7461 3d35 2c0a 2020 2020 2020 2020  (eta=5,.        
-00011b30: 3e3e 3e20 2020 2020 2020 2020 2020 2020  >>>             
-00011b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b50: 2020 2020 2020 206b 3d33 3030 2c0a 2020         k=300,.  
-00011b60: 2020 2020 2020 3e3e 3e20 2020 2020 2020        >>>       
-00011b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b80: 2020 2020 2020 2020 2020 2020 2073 636f               sco
-00011b90: 7269 6e67 5f74 7970 653d 2743 6f6d 706c  ring_type='Compl
-00011ba0: 4578 272c 0a20 2020 2020 2020 203e 3e3e  Ex',.        >>>
-00011bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011bd0: 2020 2020 7365 6564 3d30 290a 2020 2020      seed=0).    
-00011be0: 2020 2020 3e3e 3e20 6d6f 6465 6c2e 636f      >>> model.co
-00011bf0: 6d70 696c 6528 6f70 7469 6d69 7a65 723d  mpile(optimizer=
-00011c00: 2761 6461 6d27 2c20 6c6f 7373 3d27 6e6c  'adam', loss='nl
-00011c10: 6c27 290a 2020 2020 2020 2020 3e3e 3e20  l').        >>> 
-00011c20: 6d6f 6465 6c2e 6669 7428 585b 2774 7261  model.fit(X['tra
-00011c30: 696e 275d 2c0a 2020 2020 2020 2020 3e3e  in'],.        >>
-00011c40: 3e20 2020 2020 2020 2020 2020 6261 7463  >           batc
-00011c50: 685f 7369 7a65 3d31 3030 3030 2c0a 2020  h_size=10000,.  
-00011c60: 2020 2020 2020 3e3e 3e20 2020 2020 2020        >>>       
-00011c70: 2020 2020 6570 6f63 6873 3d35 290a 2020      epochs=5).  
-00011c80: 2020 2020 2020 4570 6f63 6820 312f 350a        Epoch 1/5.
-00011c90: 2020 2020 2020 2020 3239 2f32 3920 5b3d          29/29 [=
-00011ca0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00011cb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d5d 202d  =============] -
-00011cc0: 2037 7320 3232 386d 732f 7374 6570 202d   7s 228ms/step -
-00011cd0: 206c 6f73 733a 2036 3733 3631 2e32 3733   loss: 67361.273
-00011ce0: 340a 2020 2020 2020 2020 4570 6f63 6820  4.        Epoch 
-00011cf0: 322f 350a 2020 2020 2020 2020 3239 2f32  2/5.        29/2
-00011d00: 3920 5b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  9 [=============
-00011d10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00011d20: 3d5d 202d 2035 7320 3138 346d 732f 7374  =] - 5s 184ms/st
-00011d30: 6570 202d 206c 6f73 733a 2036 3733 3138  ep - loss: 67318
-00011d40: 2e38 3230 330a 2020 2020 2020 2020 4570  .8203.        Ep
-00011d50: 6f63 6820 332f 350a 2020 2020 2020 2020  och 3/5.        
-00011d60: 3239 2f32 3920 5b3d 3d3d 3d3d 3d3d 3d3d  29/29 [=========
-00011d70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00011d80: 3d3d 3d3d 3d5d 202d 2035 7320 3138 376d  =====] - 5s 187m
-00011d90: 732f 7374 6570 202d 206c 6f73 733a 2036  s/step - loss: 6
-00011da0: 3730 3231 2e31 3634 310a 2020 2020 2020  7021.1641.      
-00011db0: 2020 4570 6f63 6820 342f 350a 2020 2020    Epoch 4/5.    
-00011dc0: 2020 2020 3239 2f32 3920 5b3d 3d3d 3d3d      29/29 [=====
-00011dd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00011de0: 3d3d 3d3d 3d3d 3d3d 3d5d 202d 2035 7320  =========] - 5s 
-00011df0: 3138 386d 732f 7374 6570 202d 206c 6f73  188ms/step - los
-00011e00: 733a 2036 3538 3635 2e35 3534 370a 2020  s: 65865.5547.  
-00011e10: 2020 2020 2020 4570 6f63 6820 352f 350a        Epoch 5/5.
-00011e20: 2020 2020 2020 2020 3239 2f32 3920 5b3d          29/29 [=
-00011e30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00011e40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d5d 202d  =============] -
-00011e50: 2035 7320 3138 386d 732f 7374 6570 202d   5s 188ms/step -
-00011e60: 206c 6f73 733a 2036 3335 3130 2e32 3737   loss: 63510.277
-00011e70: 330a 0a20 2020 2020 2020 203e 3e3e 2070  3..        >>> p
-00011e80: 7265 6420 3d20 6d6f 6465 6c2e 7072 6564  red = model.pred
-00011e90: 6963 7428 585b 2774 6573 7427 5d2c 0a20  ict(X['test'],. 
-00011ea0: 2020 2020 2020 203e 3e3e 2020 2020 2020         >>>      
-00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ec0: 6261 7463 685f 7369 7a65 3d31 3030 290a  batch_size=100).
-00011ed0: 2020 2020 2020 2020 3e3e 3e20 7072 696e          >>> prin
-00011ee0: 7428 6e70 2e73 6f72 7428 7072 6564 2929  t(np.sort(pred))
-00011ef0: 0a20 2020 2020 2020 205b 2d31 2e30 3836  .        [-1.086
-00011f00: 3831 3638 2020 2d30 2e34 3635 3832 3439  8168  -0.4658249
-00011f10: 3620 2d30 2e34 3437 3135 3836 3320 2e2e  6 -0.44715863 ..
-00011f20: 2e20 2033 2e32 3438 3432 3734 2020 2033  .  3.2484274   3
-00011f30: 2e33 3134 3737 3132 2020 332e 3332 3620  .3147712  3.326 
-00011f40: 2020 2020 5d0a 0a20 2020 2020 2020 2022      ]..        "
-00011f50: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
-00011f60: 2e64 6174 615f 6861 6e64 6c65 725f 7465  .data_handler_te
-00011f70: 7374 203d 2064 6174 615f 6164 6170 7465  st = data_adapte
-00011f80: 722e 4461 7461 4861 6e64 6c65 7228 0a20  r.DataHandler(. 
-00011f90: 2020 2020 2020 2020 2020 2078 2c0a 2020             x,.  
-00011fa0: 2020 2020 2020 2020 2020 6261 7463 685f            batch_
-00011fb0: 7369 7a65 3d62 6174 6368 5f73 697a 652c  size=batch_size,
-00011fc0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00011fd0: 6173 6574 5f74 7970 653d 2274 6573 7422  aset_type="test"
-00011fe0: 2c0a 2020 2020 2020 2020 2020 2020 6570  ,.            ep
-00011ff0: 6f63 6873 3d31 2c0a 2020 2020 2020 2020  ochs=1,.        
-00012000: 2020 2020 7573 655f 6669 6c74 6572 3d46      use_filter=F
-00012010: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-00012020: 2020 7573 655f 696e 6465 7865 723d 7365    use_indexer=se
-00012030: 6c66 2e64 6174 615f 696e 6465 7865 722c  lf.data_indexer,
-00012040: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00012050: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-00012060: 7461 6e63 6528 6361 6c6c 6261 636b 732c  tance(callbacks,
-00012070: 2063 616c 6c62 6163 6b73 5f6d 6f64 756c   callbacks_modul
-00012080: 652e 4361 6c6c 6261 636b 4c69 7374 293a  e.CallbackList):
-00012090: 0a20 2020 2020 2020 2020 2020 2063 616c  .            cal
-000120a0: 6c62 6163 6b73 203d 2063 616c 6c62 6163  lbacks = callbac
-000120b0: 6b73 5f6d 6f64 756c 652e 4361 6c6c 6261  ks_module.Callba
-000120c0: 636b 4c69 7374 280a 2020 2020 2020 2020  ckList(.        
-000120d0: 2020 2020 2020 2020 6361 6c6c 6261 636b          callback
-000120e0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-000120f0: 2020 2061 6464 5f68 6973 746f 7279 3d54     add_history=T
-00012100: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00012110: 2020 2020 2061 6464 5f70 726f 6762 6172       add_progbar
-00012120: 3d76 6572 626f 7365 2021 3d20 302c 0a20  =verbose != 0,. 
-00012130: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00012140: 6f64 656c 3d73 656c 662c 0a20 2020 2020  odel=self,.     
-00012150: 2020 2020 2020 2020 2020 2076 6572 626f             verbo
-00012160: 7365 3d76 6572 626f 7365 2c0a 2020 2020  se=verbose,.    
-00012170: 2020 2020 2020 2020 2020 2020 6570 6f63              epoc
-00012180: 6873 3d31 2c0a 2020 2020 2020 2020 2020  hs=1,.          
-00012190: 2020 2020 2020 7374 6570 733d 7365 6c66        steps=self
-000121a0: 2e64 6174 615f 6861 6e64 6c65 725f 7465  .data_handler_te
-000121b0: 7374 2e69 6e66 6572 7265 645f 7374 6570  st.inferred_step
-000121c0: 732c 0a20 2020 2020 2020 2020 2020 2029  s,.            )
-000121d0: 0a0a 2020 2020 2020 2020 7072 6564 6963  ..        predic
-000121e0: 745f 6675 6e63 7469 6f6e 203d 2073 656c  t_function = sel
-000121f0: 662e 6d61 6b65 5f70 7265 6469 6374 5f66  f.make_predict_f
-00012200: 756e 6374 696f 6e28 290a 2020 2020 2020  unction().      
-00012210: 2020 6361 6c6c 6261 636b 732e 6f6e 5f70    callbacks.on_p
-00012220: 7265 6469 6374 5f62 6567 696e 2829 0a20  redict_begin(). 
-00012230: 2020 2020 2020 206f 7574 7075 7473 203d         outputs =
-00012240: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
-00012250: 5f2c 2069 7465 7261 746f 7220 696e 2073  _, iterator in s
-00012260: 656c 662e 6461 7461 5f68 616e 646c 6572  elf.data_handler
-00012270: 5f74 6573 742e 656e 756d 6572 6174 655f  _test.enumerate_
-00012280: 6570 6f63 6873 2829 3a0a 2020 2020 2020  epochs():.      
-00012290: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-000122a0: 6461 7461 5f68 616e 646c 6572 5f74 6573  data_handler_tes
-000122b0: 742e 6361 7463 685f 7374 6f70 5f69 7465  t.catch_stop_ite
-000122c0: 7261 7469 6f6e 2829 3a0a 2020 2020 2020  ration():.      
-000122d0: 2020 2020 2020 2020 2020 666f 7220 7374            for st
-000122e0: 6570 2069 6e20 7365 6c66 2e64 6174 615f  ep in self.data_
-000122f0: 6861 6e64 6c65 725f 7465 7374 2e73 7465  handler_test.ste
-00012300: 7073 2829 3a0a 2020 2020 2020 2020 2020  ps():.          
-00012310: 2020 2020 2020 2020 2020 6361 6c6c 6261            callba
-00012320: 636b 732e 6f6e 5f70 7265 6469 6374 5f62  cks.on_predict_b
-00012330: 6174 6368 5f62 6567 696e 2873 7465 7029  atch_begin(step)
-00012340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012350: 2020 2020 2062 6174 6368 5f6f 7574 7075       batch_outpu
-00012360: 7473 203d 2070 7265 6469 6374 5f66 756e  ts = predict_fun
-00012370: 6374 696f 6e28 6974 6572 6174 6f72 290a  ction(iterator).
-00012380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012390: 2020 2020 6f75 7470 7574 732e 6170 7065      outputs.appe
-000123a0: 6e64 2862 6174 6368 5f6f 7574 7075 7473  nd(batch_outputs
-000123b0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-000123c0: 2020 2020 2020 2063 616c 6c62 6163 6b73         callbacks
-000123d0: 2e6f 6e5f 7072 6564 6963 745f 6261 7463  .on_predict_batc
-000123e0: 685f 656e 6428 0a20 2020 2020 2020 2020  h_end(.         
-000123f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012400: 7465 702c 207b 226f 7574 7075 7473 223a  tep, {"outputs":
-00012410: 2062 6174 6368 5f6f 7574 7075 7473 7d0a   batch_outputs}.
-00012420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012430: 2020 2020 290a 2020 2020 2020 2020 6361      ).        ca
-00012440: 6c6c 6261 636b 732e 6f6e 5f70 7265 6469  llbacks.on_predi
-00012450: 6374 5f65 6e64 2829 0a20 2020 2020 2020  ct_end().       
-00012460: 2072 6574 7572 6e20 6e70 2e63 6f6e 6361   return np.conca
-00012470: 7465 6e61 7465 286f 7574 7075 7473 290a  tenate(outputs).
-00012480: 0a20 2020 2064 6566 206d 616b 655f 6361  .    def make_ca
-00012490: 6c69 6272 6174 655f 6675 6e63 7469 6f6e  librate_function
-000124a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000124b0: 2222 2253 696d 696c 6172 2074 6f20 6b65  """Similar to ke
-000124c0: 7261 7320 6c69 622c 2074 6869 7320 6675  ras lib, this fu
-000124d0: 6e63 7469 6f6e 2072 6574 7572 6e73 2074  nction returns t
-000124e0: 6865 2068 616e 646c 6520 746f 2074 6865  he handle to the
-000124f0: 2063 616c 6962 7261 7465 2073 7465 7020   calibrate step 
-00012500: 6675 6e63 7469 6f6e 2e0a 0a20 2020 2020  function...     
-00012510: 2020 2049 7420 7072 6f63 6573 7365 7320     It processes 
-00012520: 6f6e 6520 6261 7463 6820 6f66 2064 6174  one batch of dat
-00012530: 6120 6279 2069 7465 7261 7469 6e67 206f  a by iterating o
-00012540: 7665 7220 7468 6520 6461 7461 7365 7420  ver the dataset 
-00012550: 6974 6572 6174 6f72 2061 6e64 2063 6f6d  iterator and com
-00012560: 7075 7465 7320 7468 6520 6361 6c69 6272  putes the calibr
-00012570: 6174 696f 6e0a 2020 2020 2020 2020 6f66  ation.        of
-00012580: 2070 7265 6469 6374 696f 6e73 2e0a 0a20   predictions... 
-00012590: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-000125a0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-000125b0: 2020 2020 2020 206f 7574 3a20 4675 6e63         out: Func
-000125c0: 7469 6f6e 2068 616e 646c 650a 2020 2020  tion handle.    
-000125d0: 2020 2020 2020 2020 2020 4861 6e64 6c65            Handle
-000125e0: 2074 6f20 7468 6520 6361 6c69 6272 6174   to the calibrat
-000125f0: 696f 6e20 6675 6e63 7469 6f6e 2e0a 2020  ion function..  
-00012600: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00012610: 2020 2064 6566 2063 616c 6962 7261 7465     def calibrate
-00012620: 5f77 6974 685f 636f 7272 7570 7469 6f6e  _with_corruption
-00012630: 2869 7465 7261 746f 7229 3a0a 2020 2020  (iterator):.    
-00012640: 2020 2020 2020 2020 696e 7075 7473 203d          inputs =
-00012650: 206e 6578 7428 6974 6572 6174 6f72 290a   next(iterator).
-00012660: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00012670: 656c 662e 6461 7461 5f73 6861 7065 203e  elf.data_shape >
-00012680: 2033 2061 6e64 2069 7369 6e73 7461 6e63   3 and isinstanc
-00012690: 6528 696e 7075 7473 2c20 7475 706c 6529  e(inputs, tuple)
-000126a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000126b0: 2020 696e 7075 7473 203d 2069 6e70 7574    inputs = input
-000126c0: 735b 305d 0a20 2020 2020 2020 2020 2020  s[0].           
-000126d0: 2069 6620 7365 6c66 2e69 735f 7061 7274   if self.is_part
-000126e0: 6974 696f 6e65 645f 7472 6169 6e69 6e67  itioned_training
-000126f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012700: 2020 696e 705f 656d 6220 3d20 7365 6c66    inp_emb = self
-00012710: 2e70 726f 6365 7373 5f6d 6f64 656c 5f69  .process_model_i
-00012720: 6e70 7574 735f 666f 725f 7465 7374 2869  nputs_for_test(i
-00012730: 6e70 7574 7329 0a20 2020 2020 2020 2020  nputs).         
-00012740: 2020 2020 2020 2069 6e70 5f73 636f 7265         inp_score
-00012750: 203d 2073 656c 662e 7363 6f72 696e 675f   = self.scoring_
-00012760: 6c61 7965 7228 696e 705f 656d 6229 0a0a  layer(inp_emb)..
-00012770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012780: 636f 7272 7570 7469 6f6e 7320 3d20 7365  corruptions = se
-00012790: 6c66 2e63 6f72 7275 7074 696f 6e5f 6c61  lf.corruption_la
-000127a0: 7965 7228 696e 7075 7473 2c20 7365 6c66  yer(inputs, self
-000127b0: 2e6e 756d 5f65 6e74 732c 2031 290a 2020  .num_ents, 1).  
-000127c0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000127d0: 7272 5f65 6d62 203d 2073 656c 662e 656e  rr_emb = self.en
-000127e0: 636f 6469 6e67 5f6c 6179 6572 2863 6f72  coding_layer(cor
-000127f0: 7275 7074 696f 6e73 290a 2020 2020 2020  ruptions).      
-00012800: 2020 2020 2020 2020 2020 636f 7272 5f73            corr_s
-00012810: 636f 7265 203d 2073 656c 662e 7363 6f72  core = self.scor
-00012820: 696e 675f 6c61 7965 7228 636f 7272 5f65  ing_layer(corr_e
-00012830: 6d62 290a 2020 2020 2020 2020 2020 2020  mb).            
-00012840: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00012850: 2020 2020 2020 696e 705f 656d 6220 3d20        inp_emb = 
-00012860: 7365 6c66 2e65 6e63 6f64 696e 675f 6c61  self.encoding_la
-00012870: 7965 7228 696e 7075 7473 290a 2020 2020  yer(inputs).    
-00012880: 2020 2020 2020 2020 2020 2020 696e 705f              inp_
-00012890: 7363 6f72 6520 3d20 7365 6c66 2e73 636f  score = self.sco
-000128a0: 7269 6e67 5f6c 6179 6572 2869 6e70 5f65  ring_layer(inp_e
-000128b0: 6d62 290a 0a20 2020 2020 2020 2020 2020  mb)..           
-000128c0: 2020 2020 2063 6f72 7275 7074 696f 6e73       corruptions
-000128d0: 203d 2073 656c 662e 636f 7272 7570 7469   = self.corrupti
-000128e0: 6f6e 5f6c 6179 6572 2869 6e70 7574 732c  on_layer(inputs,
-000128f0: 2073 656c 662e 6e75 6d5f 656e 7473 2c20   self.num_ents, 
-00012900: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
-00012910: 2020 2063 6f72 725f 656d 6220 3d20 7365     corr_emb = se
-00012920: 6c66 2e65 6e63 6f64 696e 675f 6c61 7965  lf.encoding_laye
-00012930: 7228 636f 7272 7570 7469 6f6e 7329 0a20  r(corruptions). 
-00012940: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012950: 6f72 725f 7363 6f72 6520 3d20 7365 6c66  orr_score = self
-00012960: 2e73 636f 7269 6e67 5f6c 6179 6572 2863  .scoring_layer(c
-00012970: 6f72 725f 656d 6229 0a20 2020 2020 2020  orr_emb).       
-00012980: 2020 2020 2072 6574 7572 6e20 696e 705f       return inp_
-00012990: 7363 6f72 652c 2063 6f72 725f 7363 6f72  score, corr_scor
-000129a0: 650a 0a20 2020 2020 2020 2064 6566 2063  e..        def c
-000129b0: 616c 6962 7261 7465 5f77 6974 685f 6e65  alibrate_with_ne
-000129c0: 6761 7469 7665 7328 6974 6572 6174 6f72  gatives(iterator
-000129d0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-000129e0: 6e70 7574 7320 3d20 6e65 7874 2869 7465  nputs = next(ite
-000129f0: 7261 746f 7229 0a20 2020 2020 2020 2020  rator).         
-00012a00: 2020 2069 6620 7365 6c66 2e64 6174 615f     if self.data_
-00012a10: 7368 6170 6520 3e20 3320 616e 6420 6973  shape > 3 and is
-00012a20: 696e 7374 616e 6365 2869 6e70 7574 732c  instance(inputs,
-00012a30: 2074 7570 6c65 293a 0a20 2020 2020 2020   tuple):.       
-00012a40: 2020 2020 2020 2020 2069 6e70 7574 7320           inputs 
-00012a50: 3d20 696e 7075 7473 5b30 5d0a 2020 2020  = inputs[0].    
-00012a60: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00012a70: 6973 5f70 6172 7469 7469 6f6e 6564 5f74  is_partitioned_t
-00012a80: 7261 696e 696e 673a 0a20 2020 2020 2020  raining:.       
-00012a90: 2020 2020 2020 2020 2069 6e70 5f65 6d62           inp_emb
-00012aa0: 203d 2073 656c 662e 7072 6f63 6573 735f   = self.process_
-00012ab0: 6d6f 6465 6c5f 696e 7075 7473 5f66 6f72  model_inputs_for
-00012ac0: 5f74 6573 7428 696e 7075 7473 290a 2020  _test(inputs).  
-00012ad0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00012ae0: 705f 7363 6f72 6520 3d20 7365 6c66 2e73  p_score = self.s
-00012af0: 636f 7269 6e67 5f6c 6179 6572 2869 6e70  coring_layer(inp
-00012b00: 5f65 6d62 290a 2020 2020 2020 2020 2020  _emb).          
-00012b10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00012b20: 2020 2020 2020 2020 696e 705f 656d 6220          inp_emb 
-00012b30: 3d20 7365 6c66 2e65 6e63 6f64 696e 675f  = self.encoding_
-00012b40: 6c61 7965 7228 696e 7075 7473 290a 2020  layer(inputs).  
-00012b50: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00012b60: 705f 7363 6f72 6520 3d20 7365 6c66 2e73  p_score = self.s
-00012b70: 636f 7269 6e67 5f6c 6179 6572 2869 6e70  coring_layer(inp
-00012b80: 5f65 6d62 290a 2020 2020 2020 2020 2020  _emb).          
-00012b90: 2020 7265 7475 726e 2069 6e70 5f73 636f    return inp_sco
-00012ba0: 7265 0a0a 2020 2020 2020 2020 6966 2073  re..        if s
-00012bb0: 656c 662e 6973 5f63 616c 6962 7261 7465  elf.is_calibrate
-00012bc0: 5f77 6974 685f 636f 7272 7570 7469 6f6e  _with_corruption
-00012bd0: 3a0a 2020 2020 2020 2020 2020 2020 6361  :.            ca
-00012be0: 6c69 6272 6174 655f 666e 203d 2063 616c  librate_fn = cal
-00012bf0: 6962 7261 7465 5f77 6974 685f 636f 7272  ibrate_with_corr
-00012c00: 7570 7469 6f6e 0a20 2020 2020 2020 2065  uption.        e
-00012c10: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00012c20: 2063 616c 6962 7261 7465 5f66 6e20 3d20   calibrate_fn = 
-00012c30: 6361 6c69 6272 6174 655f 7769 7468 5f6e  calibrate_with_n
-00012c40: 6567 6174 6976 6573 0a0a 2020 2020 2020  egatives..      
-00012c50: 2020 6966 206e 6f74 2073 656c 662e 7275    if not self.ru
-00012c60: 6e5f 6561 6765 726c 7920 616e 6420 6e6f  n_eagerly and no
-00012c70: 7420 7365 6c66 2e69 735f 7061 7274 6974  t self.is_partit
-00012c80: 696f 6e65 645f 7472 6169 6e69 6e67 3a0a  ioned_training:.
-00012c90: 2020 2020 2020 2020 2020 2020 6361 6c69              cali
-00012ca0: 6272 6174 655f 666e 203d 2064 6566 5f66  brate_fn = def_f
-00012cb0: 756e 6374 696f 6e2e 6675 6e63 7469 6f6e  unction.function
-00012cc0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00012cd0: 2020 6361 6c69 6272 6174 655f 666e 2c20    calibrate_fn, 
-00012ce0: 6578 7065 7269 6d65 6e74 616c 5f72 656c  experimental_rel
-00012cf0: 6178 5f73 6861 7065 733d 5472 7565 0a20  ax_shapes=True. 
-00012d00: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00012d10: 2020 2020 2020 7265 7475 726e 2063 616c        return cal
-00012d20: 6962 7261 7465 5f66 6e0a 0a20 2020 2064  ibrate_fn..    d
-00012d30: 6566 2063 616c 6962 7261 7465 280a 2020  ef calibrate(.  
-00012d40: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00012d50: 2020 2020 585f 706f 732c 0a20 2020 2020      X_pos,.     
-00012d60: 2020 2058 5f6e 6567 3d4e 6f6e 652c 0a20     X_neg=None,. 
-00012d70: 2020 2020 2020 2070 6f73 6974 6976 655f         positive_
-00012d80: 6261 7365 5f72 6174 653d 4e6f 6e65 2c0a  base_rate=None,.
-00012d90: 2020 2020 2020 2020 6261 7463 685f 7369          batch_si
-00012da0: 7a65 3d33 322c 0a20 2020 2020 2020 2065  ze=32,.        e
-00012db0: 706f 6368 733d 3530 2c0a 2020 2020 2020  pochs=50,.      
-00012dc0: 2020 7665 7262 6f73 653d 302c 0a20 2020    verbose=0,.   
-00012dd0: 2029 3a0a 2020 2020 2020 2020 2222 2243   ):.        """C
-00012de0: 616c 6962 7261 7465 2070 7265 6469 6374  alibrate predict
-00012df0: 696f 6e73 2e0a 0a20 2020 2020 2020 2054  ions...        T
-00012e00: 6865 206d 6574 686f 6420 696d 706c 656d  he method implem
-00012e10: 656e 7473 2074 6865 2068 6575 7269 7374  ents the heurist
-00012e20: 6963 7320 6465 7363 7269 6265 6420 696e  ics described in
-00012e30: 203a 6369 7465 3a60 6361 6c69 6272 6174   :cite:`calibrat
-00012e40: 696f 6e60 2c0a 2020 2020 2020 2020 7573  ion`,.        us
-00012e50: 696e 6720 506c 6174 7420 7363 616c 696e  ing Platt scalin
-00012e60: 6720 3a63 6974 653a 6070 6c61 7474 3139  g :cite:`platt19
-00012e70: 3939 7072 6f62 6162 696c 6973 7469 6360  99probabilistic`
-00012e80: 2e0a 0a20 2020 2020 2020 2054 6865 2063  ...        The c
-00012e90: 616c 6962 7261 7465 6420 7072 6564 6963  alibrated predic
-00012ea0: 7469 6f6e 7320 6361 6e20 6265 206f 6274  tions can be obt
-00012eb0: 6169 6e65 6420 7769 7468 203a 6d65 7468  ained with :meth
-00012ec0: 3a60 7072 6564 6963 745f 7072 6f62 6160  :`predict_proba`
-00012ed0: 0a20 2020 2020 2020 2061 6674 6572 2063  .        after c
-00012ee0: 616c 6962 7261 7469 6f6e 2069 7320 646f  alibration is do
-00012ef0: 6e65 2e0a 0a20 2020 2020 2020 2049 6465  ne...        Ide
-00012f00: 616c 6c79 2c20 6361 6c69 6272 6174 696f  ally, calibratio
-00012f10: 6e20 7368 6f75 6c64 2062 6520 7065 7266  n should be perf
-00012f20: 6f72 6d65 6420 6f6e 2061 2076 616c 6964  ormed on a valid
-00012f30: 6174 696f 6e20 7365 7420 7468 6174 2077  ation set that w
-00012f40: 6173 206e 6f74 2075 7365 6420 746f 2074  as not used to t
-00012f50: 7261 696e 2074 6865 2065 6d62 6564 6469  rain the embeddi
-00012f60: 6e67 732e 0a0a 2020 2020 2020 2020 5468  ngs...        Th
-00012f70: 6572 6520 6172 6520 7477 6f20 6d6f 6465  ere are two mode
-00012f80: 7320 6f66 206f 7065 7261 7469 6f6e 2c20  s of operation, 
-00012f90: 6465 7065 6e64 696e 6720 6f6e 2074 6865  depending on the
-00012fa0: 2061 7661 696c 6162 696c 6974 7920 6f66   availability of
-00012fb0: 206e 6567 6174 6976 6520 7472 6970 6c65   negative triple
-00012fc0: 733a 0a0a 2020 2020 2020 2020 232e 2042  s:..        #. B
-00012fd0: 6f74 6820 706f 7369 7469 7665 2061 6e64  oth positive and
-00012fe0: 206e 6567 6174 6976 6520 7472 6970 6c65   negative triple
-00012ff0: 7320 6172 6520 7072 6f76 6964 6564 2076  s are provided v
-00013000: 6961 2060 6058 5f70 6f73 6060 2061 6e64  ia ``X_pos`` and
-00013010: 2060 6058 5f6e 6567 6060 2072 6573 7065   ``X_neg`` respe
-00013020: 6374 6976 656c 792e 205c 0a20 2020 2020  ctively. \.     
-00013030: 2020 2054 6865 206f 7074 696d 697a 6174     The optimizat
-00013040: 696f 6e20 6973 2064 6f6e 6520 7573 696e  ion is done usin
-00013050: 6720 6120 7365 636f 6e64 2d6f 7264 6572  g a second-order
-00013060: 206d 6574 686f 6420 286c 696d 6974 6564   method (limited
-00013070: 2d6d 656d 6f72 7920 4246 4753 292c 205c  -memory BFGS), \
-00013080: 0a20 2020 2020 2020 2074 6865 7265 666f  .        therefo
-00013090: 7265 206e 6f20 6879 7065 7270 6172 616d  re no hyperparam
-000130a0: 6574 6572 206e 6565 6473 2074 6f20 6265  eter needs to be
-000130b0: 2073 7065 6369 6669 6564 2e0a 0a20 2020   specified...   
-000130c0: 2020 2020 2023 2e20 4f6e 6c79 2070 6f73       #. Only pos
-000130d0: 6974 6976 6520 7472 6970 6c65 7320 6172  itive triples ar
-000130e0: 6520 7072 6f76 6964 6564 2c20 616e 6420  e provided, and 
-000130f0: 7468 6520 6e65 6761 7469 7665 2074 7269  the negative tri
-00013100: 706c 6573 2061 7265 2067 656e 6572 6174  ples are generat
-00013110: 6564 2062 7920 636f 7272 7570 7469 6f6e  ed by corruption
-00013120: 732c 205c 0a20 2020 2020 2020 206a 7573  s, \.        jus
-00013130: 7420 6c69 6b65 2069 7420 6973 2064 6f6e  t like it is don
-00013140: 6520 696e 2074 7261 696e 696e 6720 6f72  e in training or
-00013150: 2065 7661 6c75 6174 696f 6e2e 2054 6865   evaluation. The
-00013160: 206f 7074 696d 697a 6174 696f 6e20 6973   optimization is
-00013170: 2064 6f6e 6520 7573 696e 6720 6120 6669   done using a fi
-00013180: 7273 742d 6f72 6465 7220 6d65 7468 6f64  rst-order method
-00013190: 2028 4144 414d 292c 205c 0a20 2020 2020   (ADAM), \.     
-000131a0: 2020 2074 6865 7265 666f 7265 2060 6062     therefore ``b
-000131b0: 6174 6368 6573 5f63 6f75 6e74 6060 2061  atches_count`` a
-000131c0: 6e64 2060 6065 706f 6368 7360 6020 6d75  nd ``epochs`` mu
-000131d0: 7374 2062 6520 7370 6563 6966 6965 642e  st be specified.
-000131e0: 0a0a 0a20 2020 2020 2020 2043 616c 6962  ...        Calib
-000131f0: 7261 7469 6f6e 2069 7320 6869 6768 6c79  ration is highly
-00013200: 2064 6570 656e 6465 6e74 206f 6e20 7468   dependent on th
-00013210: 6520 6261 7365 2072 6174 6520 6f66 2070  e base rate of p
-00013220: 6f73 6974 6976 6520 7472 6970 6c65 732e  ositive triples.
-00013230: 0a20 2020 2020 2020 2054 6865 7265 666f  .        Therefo
-00013240: 7265 2c20 666f 7220 6d6f 6465 2028 3229  re, for mode (2)
-00013250: 206f 6620 6f70 6572 6174 696f 6e2c 2074   of operation, t
-00013260: 6865 2075 7365 7220 6973 2072 6571 7569  he user is requi
-00013270: 7265 6420 746f 2070 726f 7669 6465 2074  red to provide t
-00013280: 6865 2060 6070 6f73 6974 6976 655f 6261  he ``positive_ba
-00013290: 7365 5f72 6174 6560 6020 6172 6775 6d65  se_rate`` argume
-000132a0: 6e74 2e0a 2020 2020 2020 2020 466f 7220  nt..        For 
-000132b0: 6d6f 6465 2028 3129 2c20 7468 6174 2063  mode (1), that c
-000132c0: 616e 2062 6520 696e 6665 7272 6564 2061  an be inferred a
-000132d0: 7574 6f6d 6174 6963 616c 6c79 2062 7920  utomatically by 
-000132e0: 7468 6520 7265 6c61 7469 7665 2073 697a  the relative siz
-000132f0: 6573 206f 6620 7468 6520 706f 7369 7469  es of the positi
-00013300: 7665 2061 6e64 206e 6567 6174 6976 6520  ve and negative 
-00013310: 7365 7473 2c0a 2020 2020 2020 2020 6275  sets,.        bu
-00013320: 7420 7468 6520 7573 6572 2063 616e 206f  t the user can o
-00013330: 7665 7272 6964 6520 7468 6973 2062 6568  verride this beh
-00013340: 6176 696f 7572 2062 7920 7072 6f76 6964  aviour by provid
-00013350: 696e 6720 6120 7661 6c75 6520 746f 2060  ing a value to `
-00013360: 6070 6f73 6974 6976 655f 6261 7365 5f72  `positive_base_r
-00013370: 6174 6560 602e 0a0a 2020 2020 2020 2020  ate``...        
-00013380: 4465 6669 6e69 6e67 2074 6865 2070 6f73  Defining the pos
-00013390: 6974 6976 6520 6261 7365 2072 6174 6520  itive base rate 
-000133a0: 6973 2074 6865 2062 6967 6765 7374 2063  is the biggest c
-000133b0: 6861 6c6c 656e 6765 2077 6865 6e20 6361  hallenge when ca
-000133c0: 6c69 6272 6174 696e 6720 7769 7468 6f75  librating withou
-000133d0: 7420 6e65 6761 7469 7665 732e 2054 6861  t negatives. Tha
-000133e0: 7420 6465 7065 6e64 7320 6f6e 0a20 2020  t depends on.   
-000133f0: 2020 2020 2074 6865 2075 7365 7220 6368       the user ch
-00013400: 6f69 6365 206f 6620 7472 6970 6c65 7320  oice of triples 
-00013410: 746f 2062 6520 6576 616c 7561 7465 6420  to be evaluated 
-00013420: 6475 7269 6e67 2074 6573 7420 7469 6d65  during test time
-00013430: 2e0a 2020 2020 2020 2020 4c65 7427 7320  ..        Let's 
-00013440: 7461 6b65 2074 6865 2057 4e31 3120 6461  take the WN11 da
-00013450: 7461 7365 7420 6173 2061 6e20 6578 616d  taset as an exam
-00013460: 706c 653a 2069 7420 6861 7320 6172 6f75  ple: it has arou
-00013470: 6e64 2035 3025 2070 6f73 6974 6976 6573  nd 50% positives
-00013480: 2074 7269 706c 6573 206f 6e20 626f 7468   triples on both
-00013490: 2074 6865 2076 616c 6964 6174 696f 6e20   the validation 
-000134a0: 7365 740a 2020 2020 2020 2020 616e 6420  set.        and 
-000134b0: 7465 7374 2073 6574 2c20 736f 2074 6865  test set, so the
-000134c0: 2070 6f73 6974 6976 6520 6261 7365 2072   positive base r
-000134d0: 6174 6520 666f 6c6c 6f77 7320 746f 2062  ate follows to b
-000134e0: 6520 3530 252e 2048 6f77 6576 6572 2c20  e 50%. However, 
-000134f0: 7368 6f75 6c64 2074 6865 2075 7365 7220  should the user 
-00013500: 7265 7361 6d70 6c65 2069 7420 746f 2068  resample it to h
-00013510: 6176 650a 2020 2020 2020 2020 3735 2520  ave.        75% 
-00013520: 706f 7369 7469 7665 7320 616e 6420 3235  positives and 25
-00013530: 2520 6e65 6761 7469 7665 732c 2074 6865  % negatives, the
-00013540: 2070 7265 7669 6f75 7320 6361 6c69 6272   previous calibr
-00013550: 6174 696f 6e20 776f 756c 6420 6265 2064  ation would be d
-00013560: 6567 7261 6465 642e 2054 6865 2075 7365  egraded. The use
-00013570: 7220 6d75 7374 2072 6563 616c 6962 7261  r must recalibra
-00013580: 7465 0a20 2020 2020 2020 2074 6865 206d  te.        the m
-00013590: 6f64 656c 2077 6974 6820 6120 3735 2520  odel with a 75% 
-000135a0: 706f 7369 7469 7665 2062 6173 6520 7261  positive base ra
-000135b0: 7465 2e20 5468 6572 6566 6f72 652c 2074  te. Therefore, t
-000135c0: 6869 7320 7061 7261 6d65 7465 7220 6465  his parameter de
-000135d0: 7065 6e64 7320 6f6e 2068 6f77 2074 6865  pends on how the
-000135e0: 2075 7365 7220 6861 6e64 6c65 7320 7468   user handles th
-000135f0: 650a 2020 2020 2020 2020 6461 7461 7365  e.        datase
-00013600: 7420 616e 6420 6361 6e6e 6f74 2062 6520  t and cannot be 
-00013610: 6465 7465 726d 696e 6564 2061 7574 6f6d  determined autom
-00013620: 6174 6963 616c 6c79 206f 7220 6120 7072  atically or a pr
-00013630: 696f 7269 2e0a 0a20 2020 2020 2020 202e  iori...        .
-00013640: 2e20 4e6f 7465 203a 3a0a 2020 2020 2020  . Note ::.      
-00013650: 2020 2020 2020 3a63 6974 653a 6063 616c        :cite:`cal
-00013660: 6962 7261 7469 6f6e 6020 6063 616c 6962  ibration` `calib
-00013670: 7261 7469 6f6e 2065 7870 6572 696d 656e  ration experimen
-00013680: 7473 2061 7661 696c 6162 6c65 2068 6572  ts available her
-00013690: 650a 2020 2020 2020 2020 2020 2020 3c68  e.            <h
-000136a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000136b0: 6d2f 4163 6365 6e74 7572 652f 416d 706c  m/Accenture/Ampl
-000136c0: 6947 7261 7068 2f74 7265 652f 7061 7065  iGraph/tree/pape
-000136d0: 722f 4943 4c52 2d32 302f 6578 7065 7269  r/ICLR-20/experi
-000136e0: 6d65 6e74 732f 4943 4c52 2d32 303e 605f  ments/ICLR-20>`_
-000136f0: 2e0a 0a0a 2020 2020 2020 2020 5061 7261  ....        Para
-00013700: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00013710: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00013720: 2020 585f 706f 7320 3a20 6e70 2e61 7272    X_pos : np.arr
-00013730: 6179 2c20 7368 6170 6520 286e 2c33 2920  ay, shape (n,3) 
-00013740: 6f72 2073 7472 206f 7220 4772 6170 6844  or str or GraphD
-00013750: 6174 614c 6f61 6465 7220 6f72 2041 6273  ataLoader or Abs
-00013760: 7472 6163 7447 7261 7068 5061 7274 6974  tractGraphPartit
-00013770: 696f 6e65 720a 2020 2020 2020 2020 2020  ioner.          
-00013780: 2020 4461 7461 204f 5220 4669 6c65 6e61    Data OR Filena
-00013790: 6d65 206f 6620 7468 6520 6461 7461 2066  me of the data f
-000137a0: 696c 6520 4f52 2044 6174 6120 4861 6e64  ile OR Data Hand
-000137b0: 6c65 2074 6f20 6265 2075 7365 6420 6173  le to be used as
-000137c0: 2070 6f73 6974 6976 6520 7472 6970 6c65   positive triple
-000137d0: 732e 0a20 2020 2020 2020 2058 5f6e 6567  s..        X_neg
-000137e0: 203a 206e 702e 6172 7261 792c 2073 6861   : np.array, sha
-000137f0: 7065 2028 6e2c 3329 206f 7220 7374 7220  pe (n,3) or str 
-00013800: 6f72 2047 7261 7068 4461 7461 4c6f 6164  or GraphDataLoad
-00013810: 6572 206f 7220 4162 7374 7261 6374 4772  er or AbstractGr
-00013820: 6170 6850 6172 7469 7469 6f6e 6572 0a20  aphPartitioner. 
-00013830: 2020 2020 2020 2020 2020 2044 6174 6120             Data 
-00013840: 4f52 2046 696c 656e 616d 6520 6f66 2074  OR Filename of t
-00013850: 6865 2064 6174 6120 6669 6c65 204f 5220  he data file OR 
-00013860: 4461 7461 2048 616e 646c 6520 746f 2062  Data Handle to b
-00013870: 6520 7573 6564 2061 7320 6e65 6761 7469  e used as negati
-00013880: 7665 2074 7269 706c 6573 2e0a 0a20 2020  ve triples...   
-00013890: 2020 2020 2020 2020 2049 6620 604e 6f6e           If `Non
-000138a0: 6560 2c20 7468 6520 6e65 6761 7469 7665  e`, the negative
-000138b0: 2074 7269 706c 6573 2061 7265 2067 656e   triples are gen
-000138c0: 6572 6174 6564 2076 6961 2063 6f72 7275  erated via corru
-000138d0: 7074 696f 6e73 0a20 2020 2020 2020 2020  ptions.         
-000138e0: 2020 2061 6e64 2074 6865 2075 7365 7220     and the user 
-000138f0: 6d75 7374 2070 726f 7669 6465 2061 2070  must provide a p
-00013900: 6f73 6974 6976 6520 6261 7365 2072 6174  ositive base rat
-00013910: 6520 696e 7374 6561 642e 0a0a 2020 2020  e instead...    
-00013920: 2020 2020 706f 7369 7469 7665 5f62 6173      positive_bas
-00013930: 655f 7261 7465 3a20 666c 6f61 740a 2020  e_rate: float.  
-00013940: 2020 2020 2020 2020 2020 4261 7365 2072            Base r
-00013950: 6174 6520 6f66 2070 6f73 6974 6976 6520  ate of positive 
-00013960: 7374 6174 656d 656e 7473 2e0a 0a20 2020  statements...   
-00013970: 2020 2020 2020 2020 2046 6f72 2065 7861           For exa
-00013980: 6d70 6c65 2c20 6966 2077 6520 6173 7375  mple, if we assu
-00013990: 6d65 2074 6865 7265 2069 7320 616e 2065  me there is an e
-000139a0: 7665 6e20 6368 616e 6365 2066 6f72 2061  ven chance for a
-000139b0: 6e79 2071 7565 7279 2074 6f20 6265 2074  ny query to be t
-000139c0: 7275 652c 2074 6865 2062 6173 6520 7261  rue, the base ra
-000139d0: 7465 2077 6f75 6c64 2062 6520 3530 252e  te would be 50%.
-000139e0: 0a0a 2020 2020 2020 2020 2020 2020 4966  ..            If
-000139f0: 2060 6058 5f6e 6567 6060 2069 7320 7072   ``X_neg`` is pr
-00013a00: 6f76 6964 6564 2061 6e64 2060 6070 6f73  ovided and ``pos
-00013a10: 6974 6976 655f 6261 7365 5f72 6174 653d  itive_base_rate=
-00013a20: 4e6f 6e65 6060 2c20 7468 6520 7265 6c61  None``, the rela
-00013a30: 7469 7665 2073 697a 6573 206f 6620 6060  tive sizes of ``
-00013a40: 585f 706f 7360 6020 616e 6420 6060 585f  X_pos`` and ``X_
-00013a50: 6e65 6760 600a 2020 2020 2020 2020 2020  neg``.          
-00013a60: 2020 7769 6c6c 2062 6520 7573 6564 2074    will be used t
-00013a70: 6f20 6465 7465 726d 696e 6520 7468 6520  o determine the 
-00013a80: 6261 7365 2072 6174 652e 2053 6179 2077  base rate. Say w
-00013a90: 6520 6861 7665 2035 3020 706f 7369 7469  e have 50 positi
-00013aa0: 7665 2074 7269 706c 6573 2061 6e64 2032  ve triples and 2
-00013ab0: 3030 206e 6567 6174 6976 650a 2020 2020  00 negative.    
-00013ac0: 2020 2020 2020 2020 7472 6970 6c65 732c          triples,
-00013ad0: 2074 6865 2070 6f73 6974 6976 6520 6261   the positive ba
-00013ae0: 7365 2072 6174 6520 7769 6c6c 2062 6520  se rate will be 
-00013af0: 6173 7375 6d65 6420 746f 2062 6520 3a6d  assumed to be :m
-00013b00: 6174 683a 605c 5c66 7261 637b 3530 7d7b  ath:`\\frac{50}{
-00013b10: 2835 302b 3230 3029 7d20 3d20 5c5c 6672  (50+200)} = \\fr
-00013b20: 6163 7b31 7d7b 357d 203d 2030 2e32 602e  ac{1}{5} = 0.2`.
-00013b30: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00013b40: 6973 2076 616c 7565 206d 7573 7420 6265  is value must be
-00013b50: 203a 6d61 7468 3a60 5c5c 696e 205b 302c   :math:`\\in [0,
-00013b60: 315d 602e 0a20 2020 2020 2020 2062 6174  1]`..        bat
-00013b70: 6368 6573 5f73 697a 653a 2069 6e74 0a20  ches_size: int. 
-00013b80: 2020 2020 2020 2020 2020 2042 6174 6368             Batch
-00013b90: 2073 697a 6520 666f 7220 706f 7369 7469   size for positi
-00013ba0: 7665 732e 0a20 2020 2020 2020 2065 706f  ves..        epo
-00013bb0: 6368 733a 2069 6e74 0a20 2020 2020 2020  chs: int.       
-00013bc0: 2020 2020 204e 756d 6265 7220 6f66 2065       Number of e
-00013bd0: 706f 6368 7320 7573 6564 2074 6f20 7472  pochs used to tr
-00013be0: 6169 6e20 7468 6520 506c 6174 7420 7363  ain the Platt sc
-00013bf0: 616c 696e 6720 6d6f 6465 6c2e 0a20 2020  aling model..   
-00013c00: 2020 2020 2020 2020 204f 6e6c 7920 6170           Only ap
-00013c10: 706c 6965 7320 7768 656e 2060 6058 5f6e  plies when ``X_n
-00013c20: 6567 3d4e 6f6e 6560 602e 0a20 2020 2020  eg=None``..     
-00013c30: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
-00013c40: 0a20 2020 2020 2020 2020 2020 2056 6572  .            Ver
-00013c50: 626f 7369 7479 2028 6465 6661 756c 743a  bosity (default:
-00013c60: 2060 4661 6c73 6560 292e 0a0a 2020 2020   `False`)...    
-00013c70: 2020 2020 4578 616d 706c 650a 2020 2020      Example.    
-00013c80: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00013c90: 2020 2020 3e3e 3e20 6672 6f6d 2061 6d70      >>> from amp
-00013ca0: 6c69 6772 6170 682e 6461 7461 7365 7473  ligraph.datasets
-00013cb0: 2069 6d70 6f72 7420 6c6f 6164 5f66 6231   import load_fb1
-00013cc0: 356b 5f32 3337 0a20 2020 2020 2020 203e  5k_237.        >
-00013cd0: 3e3e 2066 726f 6d20 616d 706c 6967 7261  >> from ampligra
-00013ce0: 7068 2e6c 6174 656e 745f 6665 6174 7572  ph.latent_featur
-00013cf0: 6573 2069 6d70 6f72 7420 5363 6f72 696e  es import Scorin
-00013d00: 6742 6173 6564 456d 6265 6464 696e 674d  gBasedEmbeddingM
-00013d10: 6f64 656c 0a20 2020 2020 2020 203e 3e3e  odel.        >>>
-00013d20: 2069 6d70 6f72 7420 6e75 6d70 7920 6173   import numpy as
-00013d30: 206e 700a 2020 2020 2020 2020 3e3e 3e20   np.        >>> 
-00013d40: 6461 7461 7365 7420 3d20 6c6f 6164 5f66  dataset = load_f
-00013d50: 6231 356b 5f32 3337 2829 0a20 2020 2020  b15k_237().     
-00013d60: 2020 203e 3e3e 206d 6f64 656c 203d 2053     >>> model = S
-00013d70: 636f 7269 6e67 4261 7365 6445 6d62 6564  coringBasedEmbed
-00013d80: 6469 6e67 4d6f 6465 6c28 6574 613d 352c  dingModel(eta=5,
-00013d90: 0a20 2020 2020 2020 203e 3e3e 2020 2020  .        >>>    
-00013da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013dc0: 6b3d 3330 302c 0a20 2020 2020 2020 203e  k=300,.        >
-00013dd0: 3e3e 2020 2020 2020 2020 2020 2020 2020  >>              
-00013de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013df0: 2020 2020 2020 7363 6f72 696e 675f 7479        scoring_ty
-00013e00: 7065 3d27 436f 6d70 6c45 7827 290a 2020  pe='ComplEx').  
-00013e10: 2020 2020 2020 3e3e 3e20 6d6f 6465 6c2e        >>> model.
-00013e20: 636f 6d70 696c 6528 6f70 7469 6d69 7a65  compile(optimize
-00013e30: 723d 2761 6461 6d27 2c20 6c6f 7373 3d27  r='adam', loss='
-00013e40: 6e6c 6c27 290a 2020 2020 2020 2020 3e3e  nll').        >>
-00013e50: 3e20 6d6f 6465 6c2e 6669 7428 6461 7461  > model.fit(data
-00013e60: 7365 745b 2774 7261 696e 275d 2c0a 2020  set['train'],.  
-00013e70: 2020 2020 2020 3e3e 3e20 2020 2020 2020        >>>       
-00013e80: 2020 2020 6261 7463 685f 7369 7a65 3d31      batch_size=1
-00013e90: 3030 3030 2c0a 2020 2020 2020 2020 3e3e  0000,.        >>
-00013ea0: 3e20 2020 2020 2020 2020 2020 6570 6f63  >           epoc
-00013eb0: 6873 3d35 290a 2020 2020 2020 2020 3e3e  hs=5).        >>
-00013ec0: 3e20 7072 696e 7428 2752 6177 2073 636f  > print('Raw sco
-00013ed0: 7265 7320 2873 6f72 7465 6429 3a27 2c20  res (sorted):', 
-00013ee0: 6e70 2e73 6f72 7428 6d6f 6465 6c2e 7072  np.sort(model.pr
-00013ef0: 6564 6963 7428 6461 7461 7365 745b 2774  edict(dataset['t
-00013f00: 6573 7427 5d29 2929 0a20 2020 2020 2020  est']))).       
-00013f10: 203e 3e3e 2070 7269 6e74 2827 496e 6469   >>> print('Indi
-00013f20: 6365 7320 6f62 7461 696e 6564 2062 7920  ces obtained by 
-00013f30: 736f 7274 696e 6720 2873 636f 7265 7329  sorting (scores)
-00013f40: 3a27 2c20 6e70 2e61 7267 736f 7274 286d  :', np.argsort(m
-00013f50: 6f64 656c 2e70 7265 6469 6374 2864 6174  odel.predict(dat
-00013f60: 6173 6574 5b27 7465 7374 275d 2929 290a  aset['test']))).
-00013f70: 2020 2020 2020 2020 5261 7720 7363 6f72          Raw scor
-00013f80: 6573 2028 736f 7274 6564 293a 205b 2d31  es (sorted): [-1
-00013f90: 2e30 3638 3937 3738 2020 202d 302e 3432  .0689778   -0.42
-00013fa0: 3038 3230 3132 2020 2d30 2e33 3938 3837  082012  -0.39887
-00013fb0: 3838 3720 2e2e 2e20 2033 2e32 3631 3833  887 ...  3.26183
-00013fc0: 3820 2033 2e32 3735 3537 3733 2020 332e  8  3.2755773  3.
-00013fd0: 3237 3638 3335 3420 5d0a 2020 2020 2020  2768354 ].      
-00013fe0: 2020 496e 6469 6365 7320 6f62 7461 696e    Indices obtain
-00013ff0: 6564 2062 7920 736f 7274 696e 6720 2873  ed by sorting (s
-00014000: 636f 7265 7329 3a20 5b20 3338 3334 2031  cores): [ 3834 1
-00014010: 3836 3334 2020 3430 3636 202e 2e2e 2020  8634  4066 ...  
-00014020: 3632 3337 2031 3336 3333 2031 3039 3631  6237 13633 10961
-00014030: 5d0a 2020 2020 2020 2020 3e3e 3e20 6d6f  ].        >>> mo
-00014040: 6465 6c2e 6361 6c69 6272 6174 6528 6461  del.calibrate(da
-00014050: 7461 7365 745b 2774 6573 7427 5d2c 0a20  taset['test'],. 
-00014060: 2020 2020 2020 203e 3e3e 2020 2020 2020         >>>      
-00014070: 2020 2020 2020 2020 2020 2062 6174 6368             batch
-00014080: 5f73 697a 653d 3130 3030 302c 0a20 2020  _size=10000,.   
-00014090: 2020 2020 203e 3e3e 2020 2020 2020 2020       >>>        
-000140a0: 2020 2020 2020 2020 2070 6f73 6974 6976           positiv
-000140b0: 655f 6261 7365 5f72 6174 653d 302e 392c  e_base_rate=0.9,
-000140c0: 0a20 2020 2020 2020 203e 3e3e 2020 2020  .        >>>    
-000140d0: 2020 2020 2020 2020 2020 2020 2065 706f               epo
-000140e0: 6368 733d 3130 3029 0a20 2020 2020 2020  chs=100).       
-000140f0: 203e 3e3e 2070 7269 6e74 2827 4361 6c69   >>> print('Cali
-00014100: 6272 6174 6564 2073 636f 7265 7320 2873  brated scores (s
-00014110: 6f72 7465 6429 3a27 2c20 6e70 2e73 6f72  orted):', np.sor
-00014120: 7428 6d6f 6465 6c2e 7072 6564 6963 745f  t(model.predict_
-00014130: 7072 6f62 6128 6461 7461 7365 745b 2774  proba(dataset['t
-00014140: 6573 7427 5d29 2929 0a20 2020 2020 2020  est']))).       
-00014150: 203e 3e3e 2070 7269 6e74 2827 496e 6469   >>> print('Indi
-00014160: 6365 7320 6f62 7461 696e 6564 2062 7920  ces obtained by 
-00014170: 736f 7274 696e 6720 2843 616c 6962 7261  sorting (Calibra
-00014180: 7465 6429 3a27 2c20 6e70 2e61 7267 736f  ted):', np.argso
-00014190: 7274 286d 6f64 656c 2e70 7265 6469 6374  rt(model.predict
-000141a0: 5f70 726f 6261 2864 6174 6173 6574 5b27  _proba(dataset['
-000141b0: 7465 7374 275d 2929 290a 2020 2020 2020  test']))).      
-000141c0: 2020 4361 6c69 6272 6174 6564 2073 636f    Calibrated sco
-000141d0: 7265 7320 2873 6f72 7465 6429 3a20 5b30  res (sorted): [0
-000141e0: 2e34 3935 3437 3938 3220 302e 3533 3936  .49547982 0.5396
-000141f0: 3939 3620 2030 2e35 3431 3138 3935 3520  996  0.54118955 
-00014200: 2e2e 2e20 302e 3736 3234 3234 3520 2030  ... 0.7624245  0
-00014210: 2e37 3633 3130 3434 2020 302e 3736 3331  .7631044  0.7631
-00014220: 3636 3535 5d0a 2020 2020 2020 2020 496e  6655].        In
-00014230: 6469 6365 7320 6f62 7461 696e 6564 2062  dices obtained b
-00014240: 7920 736f 7274 696e 6720 2843 616c 6962  y sorting (Calib
-00014250: 7261 7465 6429 3a20 5b20 3338 3334 2031  rated): [ 3834 1
-00014260: 3836 3334 2020 3430 3636 202e 2e2e 2020  8634  4066 ...  
-00014270: 3632 3337 2031 3336 3333 2031 3039 3631  6237 13633 10961
-00014280: 5d0a 0a20 2020 2020 2020 2022 2222 0a20  ]..        """. 
-00014290: 2020 2020 2020 2073 656c 662e 6973 5f63         self.is_c
-000142a0: 616c 6962 7261 7465 6420 3d20 4661 6c73  alibrated = Fals
-000142b0: 650a 2020 2020 2020 2020 6461 7461 5f68  e.        data_h
-000142c0: 616e 646c 6572 5f63 616c 6962 7261 7465  andler_calibrate
-000142d0: 5f70 6f73 203d 2064 6174 615f 6164 6170  _pos = data_adap
-000142e0: 7465 722e 4461 7461 4861 6e64 6c65 7228  ter.DataHandler(
-000142f0: 0a20 2020 2020 2020 2020 2020 2058 5f70  .            X_p
-00014300: 6f73 2c0a 2020 2020 2020 2020 2020 2020  os,.            
-00014310: 6261 7463 685f 7369 7a65 3d62 6174 6368  batch_size=batch
-00014320: 5f73 697a 652c 0a20 2020 2020 2020 2020  _size,.         
-00014330: 2020 2064 6174 6173 6574 5f74 7970 653d     dataset_type=
-00014340: 2274 6573 7422 2c0a 2020 2020 2020 2020  "test",.        
-00014350: 2020 2020 6570 6f63 6873 3d65 706f 6368      epochs=epoch
-00014360: 732c 0a20 2020 2020 2020 2020 2020 2075  s,.            u
-00014370: 7365 5f66 696c 7465 723d 4661 6c73 652c  se_filter=False,
-00014380: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
-00014390: 5f69 6e64 6578 6572 3d73 656c 662e 6461  _indexer=self.da
-000143a0: 7461 5f69 6e64 6578 6572 2c0a 2020 2020  ta_indexer,.    
-000143b0: 2020 2020 290a 0a20 2020 2020 2020 2070      )..        p
-000143c0: 6f73 5f73 697a 6520 3d20 6461 7461 5f68  os_size = data_h
-000143d0: 616e 646c 6572 5f63 616c 6962 7261 7465  andler_calibrate
-000143e0: 5f70 6f73 2e5f 7061 7265 6e74 5f61 6461  _pos._parent_ada
-000143f0: 7074 6572 2e67 6574 5f64 6174 615f 7369  pter.get_data_si
-00014400: 7a65 2829 0a20 2020 2020 2020 206e 6567  ze().        neg
-00014410: 5f73 697a 6520 3d20 706f 735f 7369 7a65  _size = pos_size
-00014420: 0a0a 2020 2020 2020 2020 6966 2058 5f6e  ..        if X_n
-00014430: 6567 2069 7320 4e6f 6e65 3a0a 2020 2020  eg is None:.    
-00014440: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
-00014450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014460: 2070 6f73 6974 6976 655f 6261 7365 5f72   positive_base_r
-00014470: 6174 6520 6973 206e 6f74 204e 6f6e 650a  ate is not None.
-00014480: 2020 2020 2020 2020 2020 2020 292c 2022              ), "
-00014490: 506c 6561 7365 2070 726f 7669 6465 2074  Please provide t
-000144a0: 6865 206e 6567 6174 6976 6573 206f 7220  he negatives or 
-000144b0: 706f 7369 7469 7665 2062 6173 6520 7261  positive base ra
-000144c0: 7465 2122 0a20 2020 2020 2020 2020 2020  te!".           
-000144d0: 2073 656c 662e 6973 5f63 616c 6962 7261   self.is_calibra
-000144e0: 7465 5f77 6974 685f 636f 7272 7570 7469  te_with_corrupti
-000144f0: 6f6e 203d 2054 7275 650a 2020 2020 2020  on = True.      
-00014500: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00014510: 2020 2020 7365 6c66 2e69 735f 6361 6c69      self.is_cali
-00014520: 6272 6174 655f 7769 7468 5f63 6f72 7275  brate_with_corru
-00014530: 7074 696f 6e20 3d20 4661 6c73 650a 0a20  ption = False.. 
-00014540: 2020 2020 2020 2020 2020 2070 6f73 5f62             pos_b
-00014550: 6174 6368 5f63 6f75 6e74 203d 2069 6e74  atch_count = int
-00014560: 286e 702e 6365 696c 2870 6f73 5f73 697a  (np.ceil(pos_siz
-00014570: 6520 2f20 6261 7463 685f 7369 7a65 2929  e / batch_size))
-00014580: 0a0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-00014590: 7461 5f68 616e 646c 6572 5f63 616c 6962  ta_handler_calib
-000145a0: 7261 7465 5f6e 6567 203d 2064 6174 615f  rate_neg = data_
-000145b0: 6164 6170 7465 722e 4461 7461 4861 6e64  adapter.DataHand
-000145c0: 6c65 7228 0a20 2020 2020 2020 2020 2020  ler(.           
-000145d0: 2020 2020 2058 5f6e 6567 2c0a 2020 2020       X_neg,.    
-000145e0: 2020 2020 2020 2020 2020 2020 6261 7463              batc
-000145f0: 685f 7369 7a65 3d62 6174 6368 5f73 697a  h_size=batch_siz
-00014600: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00014610: 2020 2064 6174 6173 6574 5f74 7970 653d     dataset_type=
-00014620: 2274 6573 7422 2c0a 2020 2020 2020 2020  "test",.        
-00014630: 2020 2020 2020 2020 6570 6f63 6873 3d65          epochs=e
-00014640: 706f 6368 732c 0a20 2020 2020 2020 2020  pochs,.         
-00014650: 2020 2020 2020 2075 7365 5f66 696c 7465         use_filte
-00014660: 723d 4661 6c73 652c 0a20 2020 2020 2020  r=False,.       
-00014670: 2020 2020 2020 2020 2075 7365 5f69 6e64           use_ind
-00014680: 6578 6572 3d73 656c 662e 6461 7461 5f69  exer=self.data_i
-00014690: 6e64 6578 6572 2c0a 2020 2020 2020 2020  ndexer,.        
-000146a0: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-000146b0: 2020 206e 6567 5f73 697a 6520 3d20 280a     neg_size = (.
-000146c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146d0: 6461 7461 5f68 616e 646c 6572 5f63 616c  data_handler_cal
-000146e0: 6962 7261 7465 5f6e 6567 2e5f 7061 7265  ibrate_neg._pare
-000146f0: 6e74 5f61 6461 7074 6572 2e67 6574 5f64  nt_adapter.get_d
-00014700: 6174 615f 7369 7a65 2829 0a20 2020 2020  ata_size().     
-00014710: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00014720: 2020 2020 206e 6567 5f62 6174 6368 5f63       neg_batch_c
-00014730: 6f75 6e74 203d 2069 6e74 286e 702e 6365  ount = int(np.ce
-00014740: 696c 286e 6567 5f73 697a 6520 2f20 6261  il(neg_size / ba
-00014750: 7463 685f 7369 7a65 2929 0a0a 2020 2020  tch_size))..    
-00014760: 2020 2020 2020 2020 6966 2070 6f73 5f62          if pos_b
-00014770: 6174 6368 5f63 6f75 6e74 2021 3d20 6e65  atch_count != ne
-00014780: 675f 6261 7463 685f 636f 756e 743a 0a20  g_batch_count:. 
-00014790: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-000147a0: 6174 6368 5f73 697a 655f 6e65 6720 3d20  atch_size_neg = 
-000147b0: 696e 7428 6e70 2e63 6569 6c28 6e65 675f  int(np.ceil(neg_
-000147c0: 7369 7a65 202f 2070 6f73 5f62 6174 6368  size / pos_batch
-000147d0: 5f63 6f75 6e74 2929 0a20 2020 2020 2020  _count)).       
-000147e0: 2020 2020 2020 2020 2064 6174 615f 6861           data_ha
-000147f0: 6e64 6c65 725f 6361 6c69 6272 6174 655f  ndler_calibrate_
-00014800: 6e65 6720 3d20 6461 7461 5f61 6461 7074  neg = data_adapt
-00014810: 6572 2e44 6174 6148 616e 646c 6572 280a  er.DataHandler(.
-00014820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014830: 2020 2020 585f 6e65 672c 0a20 2020 2020      X_neg,.     
-00014840: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00014850: 6174 6368 5f73 697a 653d 6261 7463 685f  atch_size=batch_
-00014860: 7369 7a65 5f6e 6567 2c0a 2020 2020 2020  size_neg,.      
-00014870: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00014880: 7461 7365 745f 7479 7065 3d22 7465 7374  taset_type="test
-00014890: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000148a0: 2020 2020 2020 2065 706f 6368 733d 6570         epochs=ep
-000148b0: 6f63 6873 2c0a 2020 2020 2020 2020 2020  ochs,.          
-000148c0: 2020 2020 2020 2020 2020 7573 655f 6669            use_fi
-000148d0: 6c74 6572 3d46 616c 7365 2c0a 2020 2020  lter=False,.    
-000148e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148f0: 7573 655f 696e 6465 7865 723d 7365 6c66  use_indexer=self
-00014900: 2e64 6174 615f 696e 6465 7865 722c 0a20  .data_indexer,. 
-00014910: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00014920: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00014930: 2070 6f73 6974 6976 655f 6261 7365 5f72   positive_base_r
-00014940: 6174 6520 6973 204e 6f6e 653a 0a20 2020  ate is None:.   
-00014950: 2020 2020 2020 2020 2020 2020 2070 6f73               pos
-00014960: 6974 6976 655f 6261 7365 5f72 6174 6520  itive_base_rate 
-00014970: 3d20 706f 735f 7369 7a65 202f 2028 706f  = pos_size / (po
-00014980: 735f 7369 7a65 202b 206e 6567 5f73 697a  s_size + neg_siz
-00014990: 6529 0a0a 2020 2020 2020 2020 6966 2070  e)..        if p
-000149a0: 6f73 6974 6976 655f 6261 7365 5f72 6174  ositive_base_rat
-000149b0: 6520 6973 206e 6f74 204e 6f6e 6520 616e  e is not None an
-000149c0: 6420 280a 2020 2020 2020 2020 2020 2020  d (.            
-000149d0: 706f 7369 7469 7665 5f62 6173 655f 7261  positive_base_ra
-000149e0: 7465 203c 3d20 3020 6f72 2070 6f73 6974  te <= 0 or posit
-000149f0: 6976 655f 6261 7365 5f72 6174 6520 3e3d  ive_base_rate >=
-00014a00: 2031 0a20 2020 2020 2020 2029 3a0a 2020   1.        ):.  
-00014a10: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00014a20: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-00014a30: 2020 2020 2020 2020 2020 2020 2270 6f73              "pos
-00014a40: 6974 6976 655f 6261 7365 5f72 6174 6520  itive_base_rate 
-00014a50: 6d75 7374 2062 6520 6120 7661 6c75 6520  must be a value 
-00014a60: 6265 7477 6565 6e20 3020 616e 6420 312e  between 0 and 1.
-00014a70: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-00014a80: 0a20 2020 2020 2020 2073 656c 662e 6361  .        self.ca
-00014a90: 6c69 6272 6174 696f 6e5f 6c61 7965 7220  libration_layer 
-00014aa0: 3d20 4361 6c69 6272 6174 696f 6e4c 6179  = CalibrationLay
-00014ab0: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-00014ac0: 706f 735f 7369 7a65 2c20 6e65 675f 7369  pos_size, neg_si
-00014ad0: 7a65 2c20 706f 7369 7469 7665 5f62 6173  ze, positive_bas
-00014ae0: 655f 7261 7465 0a20 2020 2020 2020 2029  e_rate.        )
-00014af0: 0a20 2020 2020 2020 2063 616c 6962 7261  .        calibra
-00014b00: 7465 5f66 756e 6374 696f 6e20 3d20 7365  te_function = se
-00014b10: 6c66 2e6d 616b 655f 6361 6c69 6272 6174  lf.make_calibrat
-00014b20: 655f 6675 6e63 7469 6f6e 2829 0a0a 2020  e_function()..  
-00014b30: 2020 2020 2020 6f70 7469 6d69 7a65 7220        optimizer 
-00014b40: 3d20 7466 2e6b 6572 6173 2e6f 7074 696d  = tf.keras.optim
-00014b50: 697a 6572 732e 4164 616d 2829 0a0a 2020  izers.Adam()..  
-00014b60: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00014b70: 662e 6973 5f63 616c 6962 7261 7465 5f77  f.is_calibrate_w
-00014b80: 6974 685f 636f 7272 7570 7469 6f6e 3a0a  ith_corruption:.
-00014b90: 2020 2020 2020 2020 2020 2020 6e65 6761              nega
-00014ba0: 7469 7665 5f69 7465 7261 746f 7220 3d20  tive_iterator = 
-00014bb0: 6974 6572 280a 2020 2020 2020 2020 2020  iter(.          
-00014bc0: 2020 2020 2020 6461 7461 5f68 616e 646c        data_handl
-00014bd0: 6572 5f63 616c 6962 7261 7465 5f6e 6567  er_calibrate_neg
-00014be0: 2e65 6e75 6d65 7261 7465 5f65 706f 6368  .enumerate_epoch
-00014bf0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-00014c00: 290a 0a20 2020 2020 2020 2066 6f72 205f  )..        for _
-00014c10: 2c20 6974 6572 6174 6f72 2069 6e20 6461  , iterator in da
-00014c20: 7461 5f68 616e 646c 6572 5f63 616c 6962  ta_handler_calib
-00014c30: 7261 7465 5f70 6f73 2e65 6e75 6d65 7261  rate_pos.enumera
-00014c40: 7465 5f65 706f 6368 7328 5472 7565 293a  te_epochs(True):
-00014c50: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00014c60: 6e6f 7420 7365 6c66 2e69 735f 6361 6c69  not self.is_cali
-00014c70: 6272 6174 655f 7769 7468 5f63 6f72 7275  brate_with_corru
-00014c80: 7074 696f 6e3a 0a20 2020 2020 2020 2020  ption:.         
-00014c90: 2020 2020 2020 205f 2c20 6e65 675f 6861         _, neg_ha
-00014ca0: 6e64 6c65 203d 206e 6578 7428 6e65 6761  ndle = next(nega
-00014cb0: 7469 7665 5f69 7465 7261 746f 7229 0a0a  tive_iterator)..
-00014cc0: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00014cd0: 2064 6174 615f 6861 6e64 6c65 725f 6361   data_handler_ca
-00014ce0: 6c69 6272 6174 655f 706f 732e 6361 7463  librate_pos.catc
-00014cf0: 685f 7374 6f70 5f69 7465 7261 7469 6f6e  h_stop_iteration
-00014d00: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00014d10: 2020 2020 666f 7220 7374 6570 2069 6e20      for step in 
-00014d20: 6461 7461 5f68 616e 646c 6572 5f63 616c  data_handler_cal
-00014d30: 6962 7261 7465 5f70 6f73 2e73 7465 7073  ibrate_pos.steps
-00014d40: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00014d50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00014d60: 6973 5f63 616c 6962 7261 7465 5f77 6974  is_calibrate_wit
-00014d70: 685f 636f 7272 7570 7469 6f6e 3a0a 2020  h_corruption:.  
-00014d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d90: 2020 2020 2020 7363 6f72 6573 5f70 6f73        scores_pos
-00014da0: 2c20 7363 6f72 6573 5f6e 6567 203d 2063  , scores_neg = c
-00014db0: 616c 6962 7261 7465 5f66 756e 6374 696f  alibrate_functio
-00014dc0: 6e28 6974 6572 6174 6f72 290a 0a20 2020  n(iterator)..   
-00014dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014de0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00014df0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014e00: 636f 7265 735f 706f 7320 3d20 6361 6c69  cores_pos = cali
-00014e10: 6272 6174 655f 6675 6e63 7469 6f6e 2869  brate_function(i
-00014e20: 7465 7261 746f 7229 0a20 2020 2020 2020  terator).       
-00014e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e40: 2077 6974 6820 6461 7461 5f68 616e 646c   with data_handl
-00014e50: 6572 5f63 616c 6962 7261 7465 5f6e 6567  er_calibrate_neg
-00014e60: 2e63 6174 6368 5f73 746f 705f 6974 6572  .catch_stop_iter
-00014e70: 6174 696f 6e28 293a 0a20 2020 2020 2020  ation():.       
-00014e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e90: 2020 2020 2073 636f 7265 735f 6e65 6720       scores_neg 
-00014ea0: 3d20 6361 6c69 6272 6174 655f 6675 6e63  = calibrate_func
-00014eb0: 7469 6f6e 286e 6567 5f68 616e 646c 6529  tion(neg_handle)
-00014ec0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014ed0: 2020 2020 2020 7769 7468 2074 662e 4772        with tf.Gr
-00014ee0: 6164 6965 6e74 5461 7065 2829 2061 7320  adientTape() as 
-00014ef0: 7461 7065 3a0a 2020 2020 2020 2020 2020  tape:.          
-00014f00: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-00014f10: 7420 3d20 7365 6c66 2e63 616c 6962 7261  t = self.calibra
-00014f20: 7469 6f6e 5f6c 6179 6572 2873 636f 7265  tion_layer(score
-00014f30: 735f 706f 732c 2073 636f 7265 735f 6e65  s_pos, scores_ne
-00014f40: 672c 2031 290a 0a20 2020 2020 2020 2020  g, 1)..         
-00014f50: 2020 2020 2020 2020 2020 2067 7261 6469             gradi
-00014f60: 656e 7473 203d 2074 6170 652e 6772 6164  ents = tape.grad
-00014f70: 6965 6e74 280a 2020 2020 2020 2020 2020  ient(.          
-00014f80: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-00014f90: 742c 2073 656c 662e 6361 6c69 6272 6174  t, self.calibrat
-00014fa0: 696f 6e5f 6c61 7965 722e 5f74 7261 696e  ion_layer._train
-00014fb0: 6162 6c65 5f77 6569 6768 7473 0a20 2020  able_weights.   
+00010840: 616e 7428 5b5d 290a 2020 2020 2020 2020  ant([]).        
+00010850: 7365 6c66 2e6d 6170 7069 6e67 5f64 6963  self.mapping_dic
+00010860: 7420 3d20 7466 2e6c 6f6f 6b75 702e 6578  t = tf.lookup.ex
+00010870: 7065 7269 6d65 6e74 616c 2e44 656e 7365  perimental.Dense
+00010880: 4861 7368 5461 626c 6528 0a20 2020 2020  HashTable(.     
+00010890: 2020 2020 2020 2074 662e 696e 7433 322c         tf.int32,
+000108a0: 2074 662e 696e 7433 322c 202d 312c 202d   tf.int32, -1, -
+000108b0: 312c 202d 320a 2020 2020 2020 2020 290a  1, -2.        ).
+000108c0: 2020 2020 2020 2020 6966 2065 6e74 6974          if entit
+000108d0: 6965 735f 7375 6273 6574 2069 7320 6e6f  ies_subset is no
+000108e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000108f0: 2020 2020 656e 7469 7469 6573 5f73 7562      entities_sub
+00010900: 7365 7420 3d20 7365 6c66 2e64 6174 615f  set = self.data_
+00010910: 696e 6465 7865 722e 6765 745f 696e 6465  indexer.get_inde
+00010920: 7865 7328 0a20 2020 2020 2020 2020 2020  xes(.           
+00010930: 2020 2020 2065 6e74 6974 6965 735f 7375       entities_su
+00010940: 6273 6574 2c20 2265 220a 2020 2020 2020  bset, "e".      
+00010950: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00010960: 2020 2020 7365 6c66 2e65 6e74 6974 6965      self.entitie
+00010970: 735f 7375 6273 6574 203d 2074 662e 636f  s_subset = tf.co
+00010980: 6e73 7461 6e74 2865 6e74 6974 6965 735f  nstant(entities_
+00010990: 7375 6273 6574 2c20 6474 7970 653d 7466  subset, dtype=tf
+000109a0: 2e69 6e74 3332 290a 2020 2020 2020 2020  .int32).        
+000109b0: 2020 2020 7365 6c66 2e6d 6170 7069 6e67      self.mapping
+000109c0: 5f64 6963 742e 696e 7365 7274 280a 2020  _dict.insert(.  
+000109d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000109e0: 6c66 2e65 6e74 6974 6965 735f 7375 6273  lf.entities_subs
+000109f0: 6574 2c20 7466 2e72 616e 6765 2873 656c  et, tf.range(sel
+00010a00: 662e 656e 7469 7469 6573 5f73 7562 7365  f.entities_subse
+00010a10: 742e 7368 6170 655b 305d 290a 2020 2020  t.shape[0]).    
+00010a20: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00010a30: 2020 2023 2066 6c61 6720 746f 2069 6e64     # flag to ind
+00010a40: 6963 6174 6520 6966 2077 6520 6172 6520  icate if we are 
+00010a50: 7573 696e 6720 6669 6c74 6572 206f 7220  using filter or 
+00010a60: 6e6f 740a 2020 2020 2020 2020 7365 6c66  not.        self
+00010a70: 2e75 7365 5f66 696c 7465 7220 3d20 280a  .use_filter = (.
+00010a80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010a90: 2e64 6174 615f 6861 6e64 6c65 725f 7465  .data_handler_te
+00010aa0: 7374 2e5f 7061 7265 6e74 5f61 6461 7074  st._parent_adapt
+00010ab0: 6572 2e62 6163 6b65 6e64 2e75 7365 5f66  er.backend.use_f
+00010ac0: 696c 7465 720a 2020 2020 2020 2020 2020  ilter.          
+00010ad0: 2020 6f72 2069 7369 6e73 7461 6e63 6528    or isinstance(
+00010ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010af0: 2073 656c 662e 6461 7461 5f68 616e 646c   self.data_handl
+00010b00: 6572 5f74 6573 742e 5f70 6172 656e 745f  er_test._parent_
+00010b10: 6164 6170 7465 722e 6261 636b 656e 642e  adapter.backend.
+00010b20: 7573 655f 6669 6c74 6572 2c20 6469 6374  use_filter, dict
+00010b30: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00010b40: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00010b50: 2020 2320 436f 6e74 6169 6e65 7220 7468    # Container th
+00010b60: 6174 2063 6f6e 6669 6775 7265 7320 616e  at configures an
+00010b70: 6420 6361 6c6c 7320 6074 662e 6b65 7261  d calls `tf.kera
+00010b80: 732e 4361 6c6c 6261 636b 6073 2e0a 2020  s.Callback`s..  
+00010b90: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+00010ba0: 6e73 7461 6e63 6528 6361 6c6c 6261 636b  nstance(callback
+00010bb0: 732c 2063 616c 6c62 6163 6b73 5f6d 6f64  s, callbacks_mod
+00010bc0: 756c 652e 4361 6c6c 6261 636b 4c69 7374  ule.CallbackList
+00010bd0: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+00010be0: 616c 6c62 6163 6b73 203d 2063 616c 6c62  allbacks = callb
+00010bf0: 6163 6b73 5f6d 6f64 756c 652e 4361 6c6c  acks_module.Call
+00010c00: 6261 636b 4c69 7374 280a 2020 2020 2020  backList(.      
+00010c10: 2020 2020 2020 2020 2020 6361 6c6c 6261            callba
+00010c20: 636b 732c 0a20 2020 2020 2020 2020 2020  cks,.           
+00010c30: 2020 2020 2061 6464 5f68 6973 746f 7279       add_history
+00010c40: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00010c50: 2020 2020 2020 2061 6464 5f70 726f 6762         add_progb
+00010c60: 6172 3d76 6572 626f 7365 2021 3d20 302c  ar=verbose != 0,
+00010c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010c80: 206d 6f64 656c 3d73 656c 662c 0a20 2020   model=self,.   
+00010c90: 2020 2020 2020 2020 2020 2020 2076 6572               ver
+00010ca0: 626f 7365 3d76 6572 626f 7365 2c0a 2020  bose=verbose,.  
+00010cb0: 2020 2020 2020 2020 2020 2020 2020 6570                ep
+00010cc0: 6f63 6873 3d31 2c0a 2020 2020 2020 2020  ochs=1,.        
+00010cd0: 2020 2020 2020 2020 7374 6570 733d 7365          steps=se
+00010ce0: 6c66 2e64 6174 615f 6861 6e64 6c65 725f  lf.data_handler_
+00010cf0: 7465 7374 2e69 6e66 6572 7265 645f 7374  test.inferred_st
+00010d00: 6570 732c 0a20 2020 2020 2020 2020 2020  eps,.           
+00010d10: 2029 0a0a 2020 2020 2020 2020 7465 7374   )..        test
+00010d20: 5f66 756e 6374 696f 6e20 3d20 7365 6c66  _function = self
+00010d30: 2e6d 616b 655f 7465 7374 5f66 756e 6374  .make_test_funct
+00010d40: 696f 6e28 290a 0a20 2020 2020 2020 2023  ion()..        #
+00010d50: 2062 6566 6f72 6520 7465 7374 2062 6567   before test beg
+00010d60: 696e 7320 6361 6c6c 2074 6869 7320 6361  ins call this ca
+00010d70: 6c6c 6261 636b 2066 756e 6374 696f 6e0a  llback function.
+00010d80: 2020 2020 2020 2020 6361 6c6c 6261 636b          callback
+00010d90: 732e 6f6e 5f74 6573 745f 6265 6769 6e28  s.on_test_begin(
+00010da0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00010db0: 616c 6c5f 7261 6e6b 7320 3d20 5b5d 0a0a  all_ranks = []..
+00010dc0: 2020 2020 2020 2020 2320 656e 756d 6572          # enumer
+00010dd0: 6174 6520 6f76 6572 2074 6865 2064 6174  ate over the dat
+00010de0: 610a 2020 2020 2020 2020 666f 7220 5f2c  a.        for _,
+00010df0: 2069 7465 7261 746f 7220 696e 2073 656c   iterator in sel
+00010e00: 662e 6461 7461 5f68 616e 646c 6572 5f74  f.data_handler_t
+00010e10: 6573 742e 656e 756d 6572 6174 655f 6570  est.enumerate_ep
+00010e20: 6f63 6873 2829 3a0a 2020 2020 2020 2020  ochs():.        
+00010e30: 2020 2020 2320 6861 6e64 6c65 2074 6865      # handle the
+00010e40: 2073 746f 7020 6974 6572 6174 696f 6e20   stop iteration 
+00010e50: 6f66 2064 6174 6120 6974 6572 6174 6f72  of data iterator
+00010e60: 2069 6e20 7468 6973 2073 636f 7065 0a20   in this scope. 
+00010e70: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00010e80: 7365 6c66 2e64 6174 615f 6861 6e64 6c65  self.data_handle
+00010e90: 725f 7465 7374 2e63 6174 6368 5f73 746f  r_test.catch_sto
+00010ea0: 705f 6974 6572 6174 696f 6e28 293a 0a20  p_iteration():. 
+00010eb0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00010ec0: 2069 7465 7261 7465 206f 7665 7220 7468   iterate over th
+00010ed0: 6520 6461 7461 7365 740a 2020 2020 2020  e dataset.      
+00010ee0: 2020 2020 2020 2020 2020 666f 7220 7374            for st
+00010ef0: 6570 2069 6e20 7365 6c66 2e64 6174 615f  ep in self.data_
+00010f00: 6861 6e64 6c65 725f 7465 7374 2e73 7465  handler_test.ste
+00010f10: 7073 2829 3a0a 2020 2020 2020 2020 2020  ps():.          
+00010f20: 2020 2020 2020 2020 2020 2320 6265 666f            # befo
+00010f30: 7265 2061 2062 6174 6368 2069 7320 7072  re a batch is pr
+00010f40: 6f63 6573 7365 6420 6361 6c6c 2074 6869  ocessed call thi
+00010f50: 7320 6361 6c6c 6261 636b 2066 756e 6374  s callback funct
+00010f60: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+00010f70: 2020 2020 2020 2020 6361 6c6c 6261 636b          callback
+00010f80: 732e 6f6e 5f74 6573 745f 6261 7463 685f  s.on_test_batch_
+00010f90: 6265 6769 6e28 7374 6570 290a 0a20 2020  begin(step)..   
+00010fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fb0: 2023 2070 726f 6365 7373 2074 6869 7320   # process this 
+00010fc0: 6261 7463 680a 2020 2020 2020 2020 2020  batch.          
+00010fd0: 2020 2020 2020 2020 2020 6f76 6572 616c            overal
+00010fe0: 6c5f 7261 6e6b 203d 2074 6573 745f 6675  l_rank = test_fu
+00010ff0: 6e63 7469 6f6e 2869 7465 7261 746f 7229  nction(iterator)
+00011000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011010: 2020 2020 2023 2069 6e63 7265 6d65 6e74       # increment
+00011020: 2074 6865 2072 616e 6b20 6279 2031 2028   the rank by 1 (
+00011030: 7261 6e6b 7320 7265 7475 726e 6564 2061  ranks returned a
+00011040: 7265 2066 726f 6d20 2830 202d 0a20 2020  re from (0 -.   
+00011050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011060: 2023 206e 2d31 2920 736f 2069 6e63 7265   # n-1) so incre
+00011070: 6d65 6e74 2062 7920 310a 2020 2020 2020  ment by 1.      
+00011080: 2020 2020 2020 2020 2020 2020 2020 6f76                ov
+00011090: 6572 616c 6c5f 7261 6e6b 202b 3d20 310a  erall_rank += 1.
+000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110b0: 2020 2020 2320 7361 7665 2074 6865 2072      # save the r
+000110c0: 616e 6b73 206f 6620 7468 6520 6261 7463  anks of the batc
+000110d0: 6820 7472 6970 6c65 730a 2020 2020 2020  h triples.      
+000110e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000110f0: 6c66 2e61 6c6c 5f72 616e 6b73 2e61 7070  lf.all_ranks.app
+00011100: 656e 6428 6f76 6572 616c 6c5f 7261 6e6b  end(overall_rank
+00011110: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011120: 2020 2020 2020 2320 6166 7465 7220 6120        # after a 
+00011130: 6261 7463 6820 6973 2070 726f 6365 7373  batch is process
+00011140: 6564 2063 616c 6c20 7468 6973 2063 616c  ed call this cal
+00011150: 6c62 6163 6b20 6675 6e63 7469 6f6e 0a20  lback function. 
+00011160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011170: 2020 2063 616c 6c62 6163 6b73 2e6f 6e5f     callbacks.on_
+00011180: 7465 7374 5f62 6174 6368 5f65 6e64 2873  test_batch_end(s
+00011190: 7465 7029 0a20 2020 2020 2020 2023 206f  tep).        # o
+000111a0: 6e20 7465 7374 2065 6e64 2063 616c 6c20  n test end call 
+000111b0: 7468 6973 206d 6574 686f 640a 2020 2020  this method.    
+000111c0: 2020 2020 6361 6c6c 6261 636b 732e 6f6e      callbacks.on
+000111d0: 5f74 6573 745f 656e 6428 290a 2020 2020  _test_end().    
+000111e0: 2020 2020 2320 7265 7475 726e 2072 616e      # return ran
+000111f0: 6b73 0a20 2020 2020 2020 2072 6574 7572  ks.        retur
+00011200: 6e20 6e70 2e63 6f6e 6361 7465 6e61 7465  n np.concatenate
+00011210: 2873 656c 662e 616c 6c5f 7261 6e6b 7329  (self.all_ranks)
+00011220: 0a0a 2020 2020 6465 6620 7072 6564 6963  ..    def predic
+00011230: 745f 7374 6570 2873 656c 662c 2069 6e70  t_step(self, inp
+00011240: 7574 7329 3a0a 2020 2020 2020 2020 2222  uts):.        ""
+00011250: 2252 6574 7572 6e73 2074 6865 206f 7574  "Returns the out
+00011260: 7075 7420 6f66 2070 7265 6469 6374 2073  put of predict s
+00011270: 7465 7020 6f6e 2061 2062 6174 6368 206f  tep on a batch o
+00011280: 6620 6461 7461 2e22 2222 0a20 2020 2020  f data.""".     
+00011290: 2020 2069 6620 7365 6c66 2e64 6174 615f     if self.data_
+000112a0: 7368 6170 6520 3e20 3320 616e 6420 6973  shape > 3 and is
+000112b0: 696e 7374 616e 6365 2869 6e70 7574 732c  instance(inputs,
+000112c0: 2074 7570 6c65 293a 0a20 2020 2020 2020   tuple):.       
+000112d0: 2020 2020 2069 6e70 7574 7320 3d20 696e       inputs = in
+000112e0: 7075 7473 5b30 5d0a 2020 2020 2020 2020  puts[0].        
+000112f0: 7363 6f72 655f 706f 7320 3d20 7365 6c66  score_pos = self
+00011300: 2869 6e70 7574 732c 2046 616c 7365 290a  (inputs, False).
+00011310: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00011320: 636f 7265 5f70 6f73 0a0a 2020 2020 6465  core_pos..    de
+00011330: 6620 7072 6564 6963 745f 7374 6570 5f70  f predict_step_p
+00011340: 6172 7469 7469 6f6e 696e 6728 7365 6c66  artitioning(self
+00011350: 2c20 696e 7075 7473 293a 0a20 2020 2020  , inputs):.     
+00011360: 2020 2022 2222 5265 7475 726e 7320 7468     """Returns th
+00011370: 6520 6f75 7470 7574 206f 6620 7072 6564  e output of pred
+00011380: 6963 7420 7374 6570 206f 6e20 6120 6261  ict step on a ba
+00011390: 7463 6820 6f66 2064 6174 612e 2222 220a  tch of data.""".
+000113a0: 2020 2020 2020 2020 7363 6f72 655f 706f          score_po
+000113b0: 7320 3d20 7365 6c66 2e73 636f 7269 6e67  s = self.scoring
+000113c0: 5f6c 6179 6572 2869 6e70 7574 7329 0a20  _layer(inputs). 
+000113d0: 2020 2020 2020 2072 6574 7572 6e20 7363         return sc
+000113e0: 6f72 655f 706f 730a 0a20 2020 2064 6566  ore_pos..    def
+000113f0: 206d 616b 655f 7072 6564 6963 745f 6675   make_predict_fu
+00011400: 6e63 7469 6f6e 2873 656c 6629 3a0a 2020  nction(self):.  
+00011410: 2020 2020 2020 2222 2253 696d 696c 6172        """Similar
+00011420: 2074 6f20 6b65 7261 7320 6c69 622c 2074   to keras lib, t
+00011430: 6869 7320 6675 6e63 7469 6f6e 2072 6574  his function ret
+00011440: 7572 6e73 2074 6865 2068 616e 646c 6520  urns the handle 
+00011450: 746f 2074 6865 2070 7265 6469 6374 2073  to the predict s
+00011460: 7465 7020 6675 6e63 7469 6f6e 2e0a 0a20  tep function... 
+00011470: 2020 2020 2020 2049 7420 7072 6f63 6573         It proces
+00011480: 7365 7320 6f6e 6520 6261 7463 6820 6f66  ses one batch of
+00011490: 2064 6174 6120 6279 2069 7465 7261 7469   data by iterati
+000114a0: 6e67 206f 7665 7220 7468 6520 6461 7461  ng over the data
+000114b0: 7365 7420 6974 6572 6174 6f72 2061 6e64  set iterator and
+000114c0: 2063 6f6d 7075 7465 7320 7468 6520 7072   computes the pr
+000114d0: 6564 6963 7469 6f6e 206f 7574 7075 7473  ediction outputs
+000114e0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+000114f0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+00011500: 2d2d 0a20 2020 2020 2020 206f 7574 3a20  --.        out: 
+00011510: 4675 6e63 7469 6f6e 2068 616e 646c 650a  Function handle.
+00011520: 2020 2020 2020 2020 2020 2020 2020 4861                Ha
+00011530: 6e64 6c65 2074 6f20 7468 6520 7072 6564  ndle to the pred
+00011540: 6963 7420 6675 6e63 7469 6f6e 2e0a 2020  ict function..  
+00011550: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00011560: 2020 6966 2073 656c 662e 7072 6564 6963    if self.predic
+00011570: 745f 6675 6e63 7469 6f6e 2069 7320 6e6f  t_function is no
+00011580: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00011590: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000115a0: 7072 6564 6963 745f 6675 6e63 7469 6f6e  predict_function
+000115b0: 0a0a 2020 2020 2020 2020 6465 6620 7072  ..        def pr
+000115c0: 6564 6963 745f 6675 6e63 7469 6f6e 2869  edict_function(i
+000115d0: 7465 7261 746f 7229 3a0a 2020 2020 2020  terator):.      
+000115e0: 2020 2020 2020 696e 7075 7473 203d 206e        inputs = n
+000115f0: 6578 7428 6974 6572 6174 6f72 290a 2020  ext(iterator).  
+00011600: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00011610: 662e 6973 5f70 6172 7469 7469 6f6e 6564  f.is_partitioned
+00011620: 5f74 7261 696e 696e 673a 0a20 2020 2020  _training:.     
+00011630: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+00011640: 7320 3d20 7365 6c66 2e70 726f 6365 7373  s = self.process
+00011650: 5f6d 6f64 656c 5f69 6e70 7574 735f 666f  _model_inputs_fo
+00011660: 725f 7465 7374 2869 6e70 7574 7329 0a20  r_test(inputs). 
+00011670: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00011680: 7574 7075 7473 203d 2073 656c 662e 7072  utputs = self.pr
+00011690: 6564 6963 745f 7374 6570 5f70 6172 7469  edict_step_parti
+000116a0: 7469 6f6e 696e 6728 696e 7075 7473 290a  tioning(inputs).
+000116b0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000116c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000116d0: 2020 6f75 7470 7574 7320 3d20 7365 6c66    outputs = self
+000116e0: 2e70 7265 6469 6374 5f73 7465 7028 696e  .predict_step(in
+000116f0: 7075 7473 290a 2020 2020 2020 2020 2020  puts).          
+00011700: 2020 7265 7475 726e 206f 7574 7075 7473    return outputs
+00011710: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00011720: 2073 656c 662e 7275 6e5f 6561 6765 726c   self.run_eagerl
+00011730: 7920 616e 6420 6e6f 7420 7365 6c66 2e69  y and not self.i
+00011740: 735f 7061 7274 6974 696f 6e65 645f 7472  s_partitioned_tr
+00011750: 6169 6e69 6e67 3a0a 2020 2020 2020 2020  aining:.        
+00011760: 2020 2020 7072 6564 6963 745f 6675 6e63      predict_func
+00011770: 7469 6f6e 203d 2064 6566 5f66 756e 6374  tion = def_funct
+00011780: 696f 6e2e 6675 6e63 7469 6f6e 280a 2020  ion.function(.  
+00011790: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+000117a0: 6564 6963 745f 6675 6e63 7469 6f6e 2c20  edict_function, 
+000117b0: 6578 7065 7269 6d65 6e74 616c 5f72 656c  experimental_rel
+000117c0: 6178 5f73 6861 7065 733d 5472 7565 0a20  ax_shapes=True. 
+000117d0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+000117e0: 2020 2020 2020 7365 6c66 2e70 7265 6469        self.predi
+000117f0: 6374 5f66 756e 6374 696f 6e20 3d20 7072  ct_function = pr
+00011800: 6564 6963 745f 6675 6e63 7469 6f6e 0a20  edict_function. 
+00011810: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00011820: 6c66 2e70 7265 6469 6374 5f66 756e 6374  lf.predict_funct
+00011830: 696f 6e0a 0a20 2020 2064 6566 2070 7265  ion..    def pre
+00011840: 6469 6374 2873 656c 662c 2078 2c20 6261  dict(self, x, ba
+00011850: 7463 685f 7369 7a65 3d33 322c 2076 6572  tch_size=32, ver
+00011860: 626f 7365 3d30 2c20 6361 6c6c 6261 636b  bose=0, callback
+00011870: 733d 4e6f 6e65 293a 0a20 2020 2020 2020  s=None):.       
+00011880: 2022 2222 0a20 2020 2020 2020 2043 6f6d   """.        Com
+00011890: 7075 7465 2073 636f 7265 7320 6f66 2074  pute scores of t
+000118a0: 6865 2069 6e70 7574 2074 7269 706c 6573  he input triples
+000118b0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+000118c0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+000118d0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+000118e0: 2020 783a 206e 702e 6172 7261 792c 2073    x: np.array, s
+000118f0: 6861 7065 2028 6e2c 2033 2920 6f72 2073  hape (n, 3) or s
+00011900: 7472 206f 7220 4772 6170 6844 6174 614c  tr or GraphDataL
+00011910: 6f61 6465 7220 6f72 2041 6273 7472 6163  oader or Abstrac
+00011920: 7447 7261 7068 5061 7274 6974 696f 6e65  tGraphPartitione
+00011930: 720a 2020 2020 2020 2020 2020 2020 4461  r.            Da
+00011940: 7461 204f 5220 4669 6c65 6e61 6d65 206f  ta OR Filename o
+00011950: 6620 7468 6520 6461 7461 2066 696c 6520  f the data file 
+00011960: 4f52 2044 6174 6120 4861 6e64 6c65 2074  OR Data Handle t
+00011970: 6f20 6265 2075 7365 6420 666f 7220 7472  o be used for tr
+00011980: 6169 6e69 6e67 2e0a 2020 2020 2020 2020  aining..        
+00011990: 6261 7463 685f 7369 7a65 3a20 696e 740a  batch_size: int.
+000119a0: 2020 2020 2020 2020 2020 2020 4261 7463              Batc
+000119b0: 6820 7369 7a65 2074 6f20 7573 6520 6475  h size to use du
+000119c0: 7269 6e67 2074 7261 696e 696e 672e 0a20  ring training.. 
+000119d0: 2020 2020 2020 2020 2020 204d 6179 2062             May b
+000119e0: 6520 6f76 6572 7269 6464 656e 2069 6620  e overridden if 
+000119f0: 6060 7860 6020 6973 2060 4772 6170 6844  ``x`` is `GraphD
+00011a00: 6174 614c 6f61 6465 7260 206f 7220 6041  ataLoader` or `A
+00011a10: 6273 7472 6163 7447 7261 7068 5061 7274  bstractGraphPart
+00011a20: 6974 696f 6e65 7260 2069 6e73 7461 6e63  itioner` instanc
+00011a30: 650a 2020 2020 2020 2020 7665 7262 6f73  e.        verbos
+00011a40: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+00011a50: 2020 2020 5665 7262 6f73 6974 7920 6d6f      Verbosity mo
+00011a60: 6465 2e0a 2020 2020 2020 2020 6361 6c6c  de..        call
+00011a70: 6261 636b 733a 206c 6973 7420 6f66 206b  backs: list of k
+00011a80: 6572 6173 2e63 616c 6c62 6163 6b73 2e43  eras.callbacks.C
+00011a90: 616c 6c62 6163 6b20 696e 7374 616e 6365  allback instance
+00011aa0: 730a 2020 2020 2020 2020 2020 2020 4c69  s.            Li
+00011ab0: 7374 206f 6620 6361 6c6c 6261 636b 7320  st of callbacks 
+00011ac0: 746f 2061 7070 6c79 2064 7572 696e 6720  to apply during 
+00011ad0: 6576 616c 7561 7469 6f6e 2e0a 0a20 2020  evaluation...   
+00011ae0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00011af0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00011b00: 2020 2020 2073 636f 7265 733a 206e 702e       scores: np.
+00011b10: 6172 7261 792c 2073 6861 7065 2028 6e2c  array, shape (n,
+00011b20: 2029 0a20 2020 2020 2020 2020 2020 2053   ).            S
+00011b30: 636f 7265 206f 6620 7468 6520 696e 7075  core of the inpu
+00011b40: 7420 7472 6970 6c65 732e 0a0a 2020 2020  t triples...    
+00011b50: 2020 2020 4578 616d 706c 650a 2020 2020      Example.    
+00011b60: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00011b70: 2020 2020 3e3e 3e20 6672 6f6d 2061 6d70      >>> from amp
+00011b80: 6c69 6772 6170 682e 6c61 7465 6e74 5f66  ligraph.latent_f
+00011b90: 6561 7475 7265 7320 696d 706f 7274 2053  eatures import S
+00011ba0: 636f 7269 6e67 4261 7365 6445 6d62 6564  coringBasedEmbed
+00011bb0: 6469 6e67 4d6f 6465 6c0a 2020 2020 2020  dingModel.      
+00011bc0: 2020 3e3e 3e20 696d 706f 7274 206e 756d    >>> import num
+00011bd0: 7079 2061 7320 6e70 0a20 2020 2020 2020  py as np.       
+00011be0: 203e 3e3e 2066 726f 6d20 616d 706c 6967   >>> from amplig
+00011bf0: 7261 7068 2e64 6174 6173 6574 7320 696d  raph.datasets im
+00011c00: 706f 7274 206c 6f61 645f 6662 3135 6b5f  port load_fb15k_
+00011c10: 3233 370a 2020 2020 2020 2020 3e3e 3e20  237.        >>> 
+00011c20: 5820 3d20 6c6f 6164 5f66 6231 356b 5f32  X = load_fb15k_2
+00011c30: 3337 2829 0a20 2020 2020 2020 203e 3e3e  37().        >>>
+00011c40: 206d 6f64 656c 203d 2053 636f 7269 6e67   model = Scoring
+00011c50: 4261 7365 6445 6d62 6564 6469 6e67 4d6f  BasedEmbeddingMo
+00011c60: 6465 6c28 6574 613d 352c 0a20 2020 2020  del(eta=5,.     
+00011c70: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
+00011c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c90: 2020 2020 2020 2020 2020 6b3d 3330 302c            k=300,
+00011ca0: 0a20 2020 2020 2020 203e 3e3e 2020 2020  .        >>>    
+00011cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cd0: 7363 6f72 696e 675f 7479 7065 3d27 436f  scoring_type='Co
+00011ce0: 6d70 6c45 7827 2c0a 2020 2020 2020 2020  mplEx',.        
+00011cf0: 3e3e 3e20 2020 2020 2020 2020 2020 2020  >>>             
+00011d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d10: 2020 2020 2020 2073 6565 643d 3029 0a20         seed=0). 
+00011d20: 2020 2020 2020 203e 3e3e 206d 6f64 656c         >>> model
+00011d30: 2e63 6f6d 7069 6c65 286f 7074 696d 697a  .compile(optimiz
+00011d40: 6572 3d27 6164 616d 272c 206c 6f73 733d  er='adam', loss=
+00011d50: 276e 6c6c 2729 0a20 2020 2020 2020 203e  'nll').        >
+00011d60: 3e3e 206d 6f64 656c 2e66 6974 2858 5b27  >> model.fit(X['
+00011d70: 7472 6169 6e27 5d2c 0a20 2020 2020 2020  train'],.       
+00011d80: 203e 3e3e 2020 2020 2020 2020 2020 2062   >>>           b
+00011d90: 6174 6368 5f73 697a 653d 3130 3030 302c  atch_size=10000,
+00011da0: 0a20 2020 2020 2020 203e 3e3e 2020 2020  .        >>>    
+00011db0: 2020 2020 2020 2065 706f 6368 733d 3529         epochs=5)
+00011dc0: 0a20 2020 2020 2020 2045 706f 6368 2031  .        Epoch 1
+00011dd0: 2f35 0a20 2020 2020 2020 2032 392f 3239  /5.        29/29
+00011de0: 205b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   [==============
+00011df0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00011e00: 5d20 2d20 3773 2032 3238 6d73 2f73 7465  ] - 7s 228ms/ste
+00011e10: 7020 2d20 6c6f 7373 3a20 3637 3336 312e  p - loss: 67361.
+00011e20: 3237 3334 0a20 2020 2020 2020 2045 706f  2734.        Epo
+00011e30: 6368 2032 2f35 0a20 2020 2020 2020 2032  ch 2/5.        2
+00011e40: 392f 3239 205b 3d3d 3d3d 3d3d 3d3d 3d3d  9/29 [==========
+00011e50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00011e60: 3d3d 3d3d 5d20 2d20 3573 2031 3834 6d73  ====] - 5s 184ms
+00011e70: 2f73 7465 7020 2d20 6c6f 7373 3a20 3637  /step - loss: 67
+00011e80: 3331 382e 3832 3033 0a20 2020 2020 2020  318.8203.       
+00011e90: 2045 706f 6368 2033 2f35 0a20 2020 2020   Epoch 3/5.     
+00011ea0: 2020 2032 392f 3239 205b 3d3d 3d3d 3d3d     29/29 [======
+00011eb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00011ec0: 3d3d 3d3d 3d3d 3d3d 5d20 2d20 3573 2031  ========] - 5s 1
+00011ed0: 3837 6d73 2f73 7465 7020 2d20 6c6f 7373  87ms/step - loss
+00011ee0: 3a20 3637 3032 312e 3136 3431 0a20 2020  : 67021.1641.   
+00011ef0: 2020 2020 2045 706f 6368 2034 2f35 0a20       Epoch 4/5. 
+00011f00: 2020 2020 2020 2032 392f 3239 205b 3d3d         29/29 [==
+00011f10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00011f20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 5d20 2d20  ============] - 
+00011f30: 3573 2031 3838 6d73 2f73 7465 7020 2d20  5s 188ms/step - 
+00011f40: 6c6f 7373 3a20 3635 3836 352e 3535 3437  loss: 65865.5547
+00011f50: 0a20 2020 2020 2020 2045 706f 6368 2035  .        Epoch 5
+00011f60: 2f35 0a20 2020 2020 2020 2032 392f 3239  /5.        29/29
+00011f70: 205b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   [==============
+00011f80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00011f90: 5d20 2d20 3573 2031 3838 6d73 2f73 7465  ] - 5s 188ms/ste
+00011fa0: 7020 2d20 6c6f 7373 3a20 3633 3531 302e  p - loss: 63510.
+00011fb0: 3237 3733 0a0a 2020 2020 2020 2020 3e3e  2773..        >>
+00011fc0: 3e20 7072 6564 203d 206d 6f64 656c 2e70  > pred = model.p
+00011fd0: 7265 6469 6374 2858 5b27 7465 7374 275d  redict(X['test']
+00011fe0: 2c0a 2020 2020 2020 2020 3e3e 3e20 2020  ,.        >>>   
+00011ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012000: 2020 2062 6174 6368 5f73 697a 653d 3130     batch_size=10
+00012010: 3029 0a20 2020 2020 2020 203e 3e3e 2070  0).        >>> p
+00012020: 7269 6e74 286e 702e 736f 7274 2870 7265  rint(np.sort(pre
+00012030: 6429 290a 2020 2020 2020 2020 5b2d 312e  d)).        [-1.
+00012040: 3038 3638 3136 3820 202d 302e 3436 3538  0868168  -0.4658
+00012050: 3234 3936 202d 302e 3434 3731 3538 3633  2496 -0.44715863
+00012060: 202e 2e2e 2020 332e 3234 3834 3237 3420   ...  3.2484274 
+00012070: 2020 332e 3331 3437 3731 3220 2033 2e33    3.3147712  3.3
+00012080: 3236 2020 2020 205d 0a0a 2020 2020 2020  26     ]..      
+00012090: 2020 2222 220a 0a20 2020 2020 2020 2073    """..        s
+000120a0: 656c 662e 6461 7461 5f68 616e 646c 6572  elf.data_handler
+000120b0: 5f74 6573 7420 3d20 6461 7461 5f61 6461  _test = data_ada
+000120c0: 7074 6572 2e44 6174 6148 616e 646c 6572  pter.DataHandler
+000120d0: 280a 2020 2020 2020 2020 2020 2020 782c  (.            x,
+000120e0: 0a20 2020 2020 2020 2020 2020 2062 6174  .            bat
+000120f0: 6368 5f73 697a 653d 6261 7463 685f 7369  ch_size=batch_si
+00012100: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
+00012110: 6461 7461 7365 745f 7479 7065 3d22 7465  dataset_type="te
+00012120: 7374 222c 0a20 2020 2020 2020 2020 2020  st",.           
+00012130: 2065 706f 6368 733d 312c 0a20 2020 2020   epochs=1,.     
+00012140: 2020 2020 2020 2075 7365 5f66 696c 7465         use_filte
+00012150: 723d 4661 6c73 652c 0a20 2020 2020 2020  r=False,.       
+00012160: 2020 2020 2075 7365 5f69 6e64 6578 6572       use_indexer
+00012170: 3d73 656c 662e 6461 7461 5f69 6e64 6578  =self.data_index
+00012180: 6572 2c0a 2020 2020 2020 2020 290a 0a20  er,.        ).. 
+00012190: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+000121a0: 696e 7374 616e 6365 2863 616c 6c62 6163  instance(callbac
+000121b0: 6b73 2c20 6361 6c6c 6261 636b 735f 6d6f  ks, callbacks_mo
+000121c0: 6475 6c65 2e43 616c 6c62 6163 6b4c 6973  dule.CallbackLis
+000121d0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+000121e0: 6361 6c6c 6261 636b 7320 3d20 6361 6c6c  callbacks = call
+000121f0: 6261 636b 735f 6d6f 6475 6c65 2e43 616c  backs_module.Cal
+00012200: 6c62 6163 6b4c 6973 7428 0a20 2020 2020  lbackList(.     
+00012210: 2020 2020 2020 2020 2020 2063 616c 6c62             callb
+00012220: 6163 6b73 2c0a 2020 2020 2020 2020 2020  acks,.          
+00012230: 2020 2020 2020 6164 645f 6869 7374 6f72        add_histor
+00012240: 793d 5472 7565 2c0a 2020 2020 2020 2020  y=True,.        
+00012250: 2020 2020 2020 2020 6164 645f 7072 6f67          add_prog
+00012260: 6261 723d 7665 7262 6f73 6520 213d 2030  bar=verbose != 0
+00012270: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012280: 2020 6d6f 6465 6c3d 7365 6c66 2c0a 2020    model=self,.  
+00012290: 2020 2020 2020 2020 2020 2020 2020 7665                ve
+000122a0: 7262 6f73 653d 7665 7262 6f73 652c 0a20  rbose=verbose,. 
+000122b0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000122c0: 706f 6368 733d 312c 0a20 2020 2020 2020  pochs=1,.       
+000122d0: 2020 2020 2020 2020 2073 7465 7073 3d73           steps=s
+000122e0: 656c 662e 6461 7461 5f68 616e 646c 6572  elf.data_handler
+000122f0: 5f74 6573 742e 696e 6665 7272 6564 5f73  _test.inferred_s
+00012300: 7465 7073 2c0a 2020 2020 2020 2020 2020  teps,.          
+00012310: 2020 290a 0a20 2020 2020 2020 2070 7265    )..        pre
+00012320: 6469 6374 5f66 756e 6374 696f 6e20 3d20  dict_function = 
+00012330: 7365 6c66 2e6d 616b 655f 7072 6564 6963  self.make_predic
+00012340: 745f 6675 6e63 7469 6f6e 2829 0a20 2020  t_function().   
+00012350: 2020 2020 2063 616c 6c62 6163 6b73 2e6f       callbacks.o
+00012360: 6e5f 7072 6564 6963 745f 6265 6769 6e28  n_predict_begin(
+00012370: 290a 2020 2020 2020 2020 6f75 7470 7574  ).        output
+00012380: 7320 3d20 5b5d 0a20 2020 2020 2020 2066  s = [].        f
+00012390: 6f72 205f 2c20 6974 6572 6174 6f72 2069  or _, iterator i
+000123a0: 6e20 7365 6c66 2e64 6174 615f 6861 6e64  n self.data_hand
+000123b0: 6c65 725f 7465 7374 2e65 6e75 6d65 7261  ler_test.enumera
+000123c0: 7465 5f65 706f 6368 7328 293a 0a20 2020  te_epochs():.   
+000123d0: 2020 2020 2020 2020 2077 6974 6820 7365           with se
+000123e0: 6c66 2e64 6174 615f 6861 6e64 6c65 725f  lf.data_handler_
+000123f0: 7465 7374 2e63 6174 6368 5f73 746f 705f  test.catch_stop_
+00012400: 6974 6572 6174 696f 6e28 293a 0a20 2020  iteration():.   
+00012410: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00012420: 2073 7465 7020 696e 2073 656c 662e 6461   step in self.da
+00012430: 7461 5f68 616e 646c 6572 5f74 6573 742e  ta_handler_test.
+00012440: 7374 6570 7328 293a 0a20 2020 2020 2020  steps():.       
+00012450: 2020 2020 2020 2020 2020 2020 2063 616c               cal
+00012460: 6c62 6163 6b73 2e6f 6e5f 7072 6564 6963  lbacks.on_predic
+00012470: 745f 6261 7463 685f 6265 6769 6e28 7374  t_batch_begin(st
+00012480: 6570 290a 2020 2020 2020 2020 2020 2020  ep).            
+00012490: 2020 2020 2020 2020 6261 7463 685f 6f75          batch_ou
+000124a0: 7470 7574 7320 3d20 7072 6564 6963 745f  tputs = predict_
+000124b0: 6675 6e63 7469 6f6e 2869 7465 7261 746f  function(iterato
+000124c0: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
+000124d0: 2020 2020 2020 206f 7574 7075 7473 2e61         outputs.a
+000124e0: 7070 656e 6428 6261 7463 685f 6f75 7470  ppend(batch_outp
+000124f0: 7574 7329 0a0a 2020 2020 2020 2020 2020  uts)..          
+00012500: 2020 2020 2020 2020 2020 6361 6c6c 6261            callba
+00012510: 636b 732e 6f6e 5f70 7265 6469 6374 5f62  cks.on_predict_b
+00012520: 6174 6368 5f65 6e64 280a 2020 2020 2020  atch_end(.      
+00012530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012540: 2020 7374 6570 2c20 7b22 6f75 7470 7574    step, {"output
+00012550: 7322 3a20 6261 7463 685f 6f75 7470 7574  s": batch_output
+00012560: 737d 0a20 2020 2020 2020 2020 2020 2020  s}.             
+00012570: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00012580: 2063 616c 6c62 6163 6b73 2e6f 6e5f 7072   callbacks.on_pr
+00012590: 6564 6963 745f 656e 6428 290a 2020 2020  edict_end().    
+000125a0: 2020 2020 7265 7475 726e 206e 702e 636f      return np.co
+000125b0: 6e63 6174 656e 6174 6528 6f75 7470 7574  ncatenate(output
+000125c0: 7329 0a0a 2020 2020 6465 6620 6d61 6b65  s)..    def make
+000125d0: 5f63 616c 6962 7261 7465 5f66 756e 6374  _calibrate_funct
+000125e0: 696f 6e28 7365 6c66 293a 0a20 2020 2020  ion(self):.     
+000125f0: 2020 2022 2222 5369 6d69 6c61 7220 746f     """Similar to
+00012600: 206b 6572 6173 206c 6962 2c20 7468 6973   keras lib, this
+00012610: 2066 756e 6374 696f 6e20 7265 7475 726e   function return
+00012620: 7320 7468 6520 6861 6e64 6c65 2074 6f20  s the handle to 
+00012630: 7468 6520 6361 6c69 6272 6174 6520 7374  the calibrate st
+00012640: 6570 2066 756e 6374 696f 6e2e 0a0a 2020  ep function...  
+00012650: 2020 2020 2020 4974 2070 726f 6365 7373        It process
+00012660: 6573 206f 6e65 2062 6174 6368 206f 6620  es one batch of 
+00012670: 6461 7461 2062 7920 6974 6572 6174 696e  data by iteratin
+00012680: 6720 6f76 6572 2074 6865 2064 6174 6173  g over the datas
+00012690: 6574 2069 7465 7261 746f 7220 616e 6420  et iterator and 
+000126a0: 636f 6d70 7574 6573 2074 6865 2063 616c  computes the cal
+000126b0: 6962 7261 7469 6f6e 0a20 2020 2020 2020  ibration.       
+000126c0: 206f 6620 7072 6564 6963 7469 6f6e 732e   of predictions.
+000126d0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+000126e0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+000126f0: 2d0a 2020 2020 2020 2020 6f75 743a 2046  -.        out: F
+00012700: 756e 6374 696f 6e20 6861 6e64 6c65 0a20  unction handle. 
+00012710: 2020 2020 2020 2020 2020 2020 2048 616e               Han
+00012720: 646c 6520 746f 2074 6865 2063 616c 6962  dle to the calib
+00012730: 7261 7469 6f6e 2066 756e 6374 696f 6e2e  ration function.
+00012740: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00012750: 2020 2020 2020 6465 6620 6361 6c69 6272        def calibr
+00012760: 6174 655f 7769 7468 5f63 6f72 7275 7074  ate_with_corrupt
+00012770: 696f 6e28 6974 6572 6174 6f72 293a 0a20  ion(iterator):. 
+00012780: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+00012790: 7320 3d20 6e65 7874 2869 7465 7261 746f  s = next(iterato
+000127a0: 7229 0a20 2020 2020 2020 2020 2020 2069  r).            i
+000127b0: 6620 7365 6c66 2e64 6174 615f 7368 6170  f self.data_shap
+000127c0: 6520 3e20 3320 616e 6420 6973 696e 7374  e > 3 and isinst
+000127d0: 616e 6365 2869 6e70 7574 732c 2074 7570  ance(inputs, tup
+000127e0: 6c65 293a 0a20 2020 2020 2020 2020 2020  le):.           
+000127f0: 2020 2020 2069 6e70 7574 7320 3d20 696e       inputs = in
+00012800: 7075 7473 5b30 5d0a 2020 2020 2020 2020  puts[0].        
+00012810: 2020 2020 6966 2073 656c 662e 6973 5f70      if self.is_p
+00012820: 6172 7469 7469 6f6e 6564 5f74 7261 696e  artitioned_train
+00012830: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
+00012840: 2020 2020 2069 6e70 5f65 6d62 203d 2073       inp_emb = s
+00012850: 656c 662e 7072 6f63 6573 735f 6d6f 6465  elf.process_mode
+00012860: 6c5f 696e 7075 7473 5f66 6f72 5f74 6573  l_inputs_for_tes
+00012870: 7428 696e 7075 7473 290a 2020 2020 2020  t(inputs).      
+00012880: 2020 2020 2020 2020 2020 696e 705f 7363            inp_sc
+00012890: 6f72 6520 3d20 7365 6c66 2e73 636f 7269  ore = self.scori
+000128a0: 6e67 5f6c 6179 6572 2869 6e70 5f65 6d62  ng_layer(inp_emb
+000128b0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+000128c0: 2020 2063 6f72 7275 7074 696f 6e73 203d     corruptions =
+000128d0: 2073 656c 662e 636f 7272 7570 7469 6f6e   self.corruption
+000128e0: 5f6c 6179 6572 2869 6e70 7574 732c 2073  _layer(inputs, s
+000128f0: 656c 662e 6e75 6d5f 656e 7473 2c20 3129  elf.num_ents, 1)
+00012900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012910: 2063 6f72 725f 656d 6220 3d20 7365 6c66   corr_emb = self
+00012920: 2e65 6e63 6f64 696e 675f 6c61 7965 7228  .encoding_layer(
+00012930: 636f 7272 7570 7469 6f6e 7329 0a20 2020  corruptions).   
+00012940: 2020 2020 2020 2020 2020 2020 2063 6f72               cor
+00012950: 725f 7363 6f72 6520 3d20 7365 6c66 2e73  r_score = self.s
+00012960: 636f 7269 6e67 5f6c 6179 6572 2863 6f72  coring_layer(cor
+00012970: 725f 656d 6229 0a20 2020 2020 2020 2020  r_emb).         
+00012980: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00012990: 2020 2020 2020 2020 2069 6e70 5f65 6d62           inp_emb
+000129a0: 203d 2073 656c 662e 656e 636f 6469 6e67   = self.encoding
+000129b0: 5f6c 6179 6572 2869 6e70 7574 7329 0a20  _layer(inputs). 
+000129c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000129d0: 6e70 5f73 636f 7265 203d 2073 656c 662e  np_score = self.
+000129e0: 7363 6f72 696e 675f 6c61 7965 7228 696e  scoring_layer(in
+000129f0: 705f 656d 6229 0a0a 2020 2020 2020 2020  p_emb)..        
+00012a00: 2020 2020 2020 2020 636f 7272 7570 7469          corrupti
+00012a10: 6f6e 7320 3d20 7365 6c66 2e63 6f72 7275  ons = self.corru
+00012a20: 7074 696f 6e5f 6c61 7965 7228 696e 7075  ption_layer(inpu
+00012a30: 7473 2c20 7365 6c66 2e6e 756d 5f65 6e74  ts, self.num_ent
+00012a40: 732c 2031 290a 2020 2020 2020 2020 2020  s, 1).          
+00012a50: 2020 2020 2020 636f 7272 5f65 6d62 203d        corr_emb =
+00012a60: 2073 656c 662e 656e 636f 6469 6e67 5f6c   self.encoding_l
+00012a70: 6179 6572 2863 6f72 7275 7074 696f 6e73  ayer(corruptions
+00012a80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012a90: 2020 636f 7272 5f73 636f 7265 203d 2073    corr_score = s
+00012aa0: 656c 662e 7363 6f72 696e 675f 6c61 7965  elf.scoring_laye
+00012ab0: 7228 636f 7272 5f65 6d62 290a 2020 2020  r(corr_emb).    
+00012ac0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+00012ad0: 6e70 5f73 636f 7265 2c20 636f 7272 5f73  np_score, corr_s
+00012ae0: 636f 7265 0a0a 2020 2020 2020 2020 6465  core..        de
+00012af0: 6620 6361 6c69 6272 6174 655f 7769 7468  f calibrate_with
+00012b00: 5f6e 6567 6174 6976 6573 2869 7465 7261  _negatives(itera
+00012b10: 746f 7229 3a0a 2020 2020 2020 2020 2020  tor):.          
+00012b20: 2020 696e 7075 7473 203d 206e 6578 7428    inputs = next(
+00012b30: 6974 6572 6174 6f72 290a 2020 2020 2020  iterator).      
+00012b40: 2020 2020 2020 6966 2073 656c 662e 6461        if self.da
+00012b50: 7461 5f73 6861 7065 203e 2033 2061 6e64  ta_shape > 3 and
+00012b60: 2069 7369 6e73 7461 6e63 6528 696e 7075   isinstance(inpu
+00012b70: 7473 2c20 7475 706c 6529 3a0a 2020 2020  ts, tuple):.    
+00012b80: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
+00012b90: 7473 203d 2069 6e70 7574 735b 305d 0a20  ts = inputs[0]. 
+00012ba0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00012bb0: 6c66 2e69 735f 7061 7274 6974 696f 6e65  lf.is_partitione
+00012bc0: 645f 7472 6169 6e69 6e67 3a0a 2020 2020  d_training:.    
+00012bd0: 2020 2020 2020 2020 2020 2020 696e 705f              inp_
+00012be0: 656d 6220 3d20 7365 6c66 2e70 726f 6365  emb = self.proce
+00012bf0: 7373 5f6d 6f64 656c 5f69 6e70 7574 735f  ss_model_inputs_
+00012c00: 666f 725f 7465 7374 2869 6e70 7574 7329  for_test(inputs)
+00012c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012c20: 2069 6e70 5f73 636f 7265 203d 2073 656c   inp_score = sel
+00012c30: 662e 7363 6f72 696e 675f 6c61 7965 7228  f.scoring_layer(
+00012c40: 696e 705f 656d 6229 0a20 2020 2020 2020  inp_emb).       
+00012c50: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00012c60: 2020 2020 2020 2020 2020 2069 6e70 5f65             inp_e
+00012c70: 6d62 203d 2073 656c 662e 656e 636f 6469  mb = self.encodi
+00012c80: 6e67 5f6c 6179 6572 2869 6e70 7574 7329  ng_layer(inputs)
+00012c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ca0: 2069 6e70 5f73 636f 7265 203d 2073 656c   inp_score = sel
+00012cb0: 662e 7363 6f72 696e 675f 6c61 7965 7228  f.scoring_layer(
+00012cc0: 696e 705f 656d 6229 0a20 2020 2020 2020  inp_emb).       
+00012cd0: 2020 2020 2072 6574 7572 6e20 696e 705f       return inp_
+00012ce0: 7363 6f72 650a 0a20 2020 2020 2020 2069  score..        i
+00012cf0: 6620 7365 6c66 2e69 735f 6361 6c69 6272  f self.is_calibr
+00012d00: 6174 655f 7769 7468 5f63 6f72 7275 7074  ate_with_corrupt
+00012d10: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+00012d20: 2063 616c 6962 7261 7465 5f66 6e20 3d20   calibrate_fn = 
+00012d30: 6361 6c69 6272 6174 655f 7769 7468 5f63  calibrate_with_c
+00012d40: 6f72 7275 7074 696f 6e0a 2020 2020 2020  orruption.      
+00012d50: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00012d60: 2020 2020 6361 6c69 6272 6174 655f 666e      calibrate_fn
+00012d70: 203d 2063 616c 6962 7261 7465 5f77 6974   = calibrate_wit
+00012d80: 685f 6e65 6761 7469 7665 730a 0a20 2020  h_negatives..   
+00012d90: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00012da0: 2e72 756e 5f65 6167 6572 6c79 2061 6e64  .run_eagerly and
+00012db0: 206e 6f74 2073 656c 662e 6973 5f70 6172   not self.is_par
+00012dc0: 7469 7469 6f6e 6564 5f74 7261 696e 696e  titioned_trainin
+00012dd0: 673a 0a20 2020 2020 2020 2020 2020 2063  g:.            c
+00012de0: 616c 6962 7261 7465 5f66 6e20 3d20 6465  alibrate_fn = de
+00012df0: 665f 6675 6e63 7469 6f6e 2e66 756e 6374  f_function.funct
+00012e00: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+00012e10: 2020 2020 2063 616c 6962 7261 7465 5f66       calibrate_f
+00012e20: 6e2c 2065 7870 6572 696d 656e 7461 6c5f  n, experimental_
+00012e30: 7265 6c61 785f 7368 6170 6573 3d54 7275  relax_shapes=Tru
+00012e40: 650a 2020 2020 2020 2020 2020 2020 290a  e.            ).
+00012e50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00012e60: 6361 6c69 6272 6174 655f 666e 0a0a 2020  calibrate_fn..  
+00012e70: 2020 6465 6620 6361 6c69 6272 6174 6528    def calibrate(
+00012e80: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00012e90: 2020 2020 2020 2058 5f70 6f73 2c0a 2020         X_pos,.  
+00012ea0: 2020 2020 2020 585f 6e65 673d 4e6f 6e65        X_neg=None
+00012eb0: 2c0a 2020 2020 2020 2020 706f 7369 7469  ,.        positi
+00012ec0: 7665 5f62 6173 655f 7261 7465 3d4e 6f6e  ve_base_rate=Non
+00012ed0: 652c 0a20 2020 2020 2020 2062 6174 6368  e,.        batch
+00012ee0: 5f73 697a 653d 3332 2c0a 2020 2020 2020  _size=32,.      
+00012ef0: 2020 6570 6f63 6873 3d35 302c 0a20 2020    epochs=50,.   
+00012f00: 2020 2020 2076 6572 626f 7365 3d30 2c0a       verbose=0,.
+00012f10: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
+00012f20: 2222 4361 6c69 6272 6174 6520 7072 6564  ""Calibrate pred
+00012f30: 6963 7469 6f6e 732e 0a0a 2020 2020 2020  ictions...      
+00012f40: 2020 5468 6520 6d65 7468 6f64 2069 6d70    The method imp
+00012f50: 6c65 6d65 6e74 7320 7468 6520 6865 7572  lements the heur
+00012f60: 6973 7469 6373 2064 6573 6372 6962 6564  istics described
+00012f70: 2069 6e20 3a63 6974 653a 6063 616c 6962   in :cite:`calib
+00012f80: 7261 7469 6f6e 602c 0a20 2020 2020 2020  ration`,.       
+00012f90: 2075 7369 6e67 2050 6c61 7474 2073 6361   using Platt sca
+00012fa0: 6c69 6e67 203a 6369 7465 3a60 706c 6174  ling :cite:`plat
+00012fb0: 7431 3939 3970 726f 6261 6269 6c69 7374  t1999probabilist
+00012fc0: 6963 602e 0a0a 2020 2020 2020 2020 5468  ic`...        Th
+00012fd0: 6520 6361 6c69 6272 6174 6564 2070 7265  e calibrated pre
+00012fe0: 6469 6374 696f 6e73 2063 616e 2062 6520  dictions can be 
+00012ff0: 6f62 7461 696e 6564 2077 6974 6820 3a6d  obtained with :m
+00013000: 6574 683a 6070 7265 6469 6374 5f70 726f  eth:`predict_pro
+00013010: 6261 600a 2020 2020 2020 2020 6166 7465  ba`.        afte
+00013020: 7220 6361 6c69 6272 6174 696f 6e20 6973  r calibration is
+00013030: 2064 6f6e 652e 0a0a 2020 2020 2020 2020   done...        
+00013040: 4964 6561 6c6c 792c 2063 616c 6962 7261  Ideally, calibra
+00013050: 7469 6f6e 2073 686f 756c 6420 6265 2070  tion should be p
+00013060: 6572 666f 726d 6564 206f 6e20 6120 7661  erformed on a va
+00013070: 6c69 6461 7469 6f6e 2073 6574 2074 6861  lidation set tha
+00013080: 7420 7761 7320 6e6f 7420 7573 6564 2074  t was not used t
+00013090: 6f20 7472 6169 6e20 7468 6520 656d 6265  o train the embe
+000130a0: 6464 696e 6773 2e0a 0a20 2020 2020 2020  ddings...       
+000130b0: 2054 6865 7265 2061 7265 2074 776f 206d   There are two m
+000130c0: 6f64 6573 206f 6620 6f70 6572 6174 696f  odes of operatio
+000130d0: 6e2c 2064 6570 656e 6469 6e67 206f 6e20  n, depending on 
+000130e0: 7468 6520 6176 6169 6c61 6269 6c69 7479  the availability
+000130f0: 206f 6620 6e65 6761 7469 7665 2074 7269   of negative tri
+00013100: 706c 6573 3a0a 0a20 2020 2020 2020 2023  ples:..        #
+00013110: 2e20 426f 7468 2070 6f73 6974 6976 6520  . Both positive 
+00013120: 616e 6420 6e65 6761 7469 7665 2074 7269  and negative tri
+00013130: 706c 6573 2061 7265 2070 726f 7669 6465  ples are provide
+00013140: 6420 7669 6120 6060 585f 706f 7360 6020  d via ``X_pos`` 
+00013150: 616e 6420 6060 585f 6e65 6760 6020 7265  and ``X_neg`` re
+00013160: 7370 6563 7469 7665 6c79 2e20 5c0a 2020  spectively. \.  
+00013170: 2020 2020 2020 5468 6520 6f70 7469 6d69        The optimi
+00013180: 7a61 7469 6f6e 2069 7320 646f 6e65 2075  zation is done u
+00013190: 7369 6e67 2061 2073 6563 6f6e 642d 6f72  sing a second-or
+000131a0: 6465 7220 6d65 7468 6f64 2028 6c69 6d69  der method (limi
+000131b0: 7465 642d 6d65 6d6f 7279 2042 4647 5329  ted-memory BFGS)
+000131c0: 2c20 5c0a 2020 2020 2020 2020 7468 6572  , \.        ther
+000131d0: 6566 6f72 6520 6e6f 2068 7970 6572 7061  efore no hyperpa
+000131e0: 7261 6d65 7465 7220 6e65 6564 7320 746f  rameter needs to
+000131f0: 2062 6520 7370 6563 6966 6965 642e 0a0a   be specified...
+00013200: 2020 2020 2020 2020 232e 204f 6e6c 7920          #. Only 
+00013210: 706f 7369 7469 7665 2074 7269 706c 6573  positive triples
+00013220: 2061 7265 2070 726f 7669 6465 642c 2061   are provided, a
+00013230: 6e64 2074 6865 206e 6567 6174 6976 6520  nd the negative 
+00013240: 7472 6970 6c65 7320 6172 6520 6765 6e65  triples are gene
+00013250: 7261 7465 6420 6279 2063 6f72 7275 7074  rated by corrupt
+00013260: 696f 6e73 2c20 5c0a 2020 2020 2020 2020  ions, \.        
+00013270: 6a75 7374 206c 696b 6520 6974 2069 7320  just like it is 
+00013280: 646f 6e65 2069 6e20 7472 6169 6e69 6e67  done in training
+00013290: 206f 7220 6576 616c 7561 7469 6f6e 2e20   or evaluation. 
+000132a0: 5468 6520 6f70 7469 6d69 7a61 7469 6f6e  The optimization
+000132b0: 2069 7320 646f 6e65 2075 7369 6e67 2061   is done using a
+000132c0: 2066 6972 7374 2d6f 7264 6572 206d 6574   first-order met
+000132d0: 686f 6420 2841 4441 4d29 2c20 5c0a 2020  hod (ADAM), \.  
+000132e0: 2020 2020 2020 7468 6572 6566 6f72 6520        therefore 
+000132f0: 6060 6261 7463 6865 735f 636f 756e 7460  ``batches_count`
+00013300: 6020 616e 6420 6060 6570 6f63 6873 6060  ` and ``epochs``
+00013310: 206d 7573 7420 6265 2073 7065 6369 6669   must be specifi
+00013320: 6564 2e0a 0a0a 2020 2020 2020 2020 4361  ed....        Ca
+00013330: 6c69 6272 6174 696f 6e20 6973 2068 6967  libration is hig
+00013340: 686c 7920 6465 7065 6e64 656e 7420 6f6e  hly dependent on
+00013350: 2074 6865 2062 6173 6520 7261 7465 206f   the base rate o
+00013360: 6620 706f 7369 7469 7665 2074 7269 706c  f positive tripl
+00013370: 6573 2e0a 2020 2020 2020 2020 5468 6572  es..        Ther
+00013380: 6566 6f72 652c 2066 6f72 206d 6f64 6520  efore, for mode 
+00013390: 2832 2920 6f66 206f 7065 7261 7469 6f6e  (2) of operation
+000133a0: 2c20 7468 6520 7573 6572 2069 7320 7265  , the user is re
+000133b0: 7175 6972 6564 2074 6f20 7072 6f76 6964  quired to provid
+000133c0: 6520 7468 6520 6060 706f 7369 7469 7665  e the ``positive
+000133d0: 5f62 6173 655f 7261 7465 6060 2061 7267  _base_rate`` arg
+000133e0: 756d 656e 742e 0a20 2020 2020 2020 2046  ument..        F
+000133f0: 6f72 206d 6f64 6520 2831 292c 2074 6861  or mode (1), tha
+00013400: 7420 6361 6e20 6265 2069 6e66 6572 7265  t can be inferre
+00013410: 6420 6175 746f 6d61 7469 6361 6c6c 7920  d automatically 
+00013420: 6279 2074 6865 2072 656c 6174 6976 6520  by the relative 
+00013430: 7369 7a65 7320 6f66 2074 6865 2070 6f73  sizes of the pos
+00013440: 6974 6976 6520 616e 6420 6e65 6761 7469  itive and negati
+00013450: 7665 2073 6574 732c 0a20 2020 2020 2020  ve sets,.       
+00013460: 2062 7574 2074 6865 2075 7365 7220 6361   but the user ca
+00013470: 6e20 6f76 6572 7269 6465 2074 6869 7320  n override this 
+00013480: 6265 6861 7669 6f75 7220 6279 2070 726f  behaviour by pro
+00013490: 7669 6469 6e67 2061 2076 616c 7565 2074  viding a value t
+000134a0: 6f20 6060 706f 7369 7469 7665 5f62 6173  o ``positive_bas
+000134b0: 655f 7261 7465 6060 2e0a 0a20 2020 2020  e_rate``...     
+000134c0: 2020 2044 6566 696e 696e 6720 7468 6520     Defining the 
+000134d0: 706f 7369 7469 7665 2062 6173 6520 7261  positive base ra
+000134e0: 7465 2069 7320 7468 6520 6269 6767 6573  te is the bigges
+000134f0: 7420 6368 616c 6c65 6e67 6520 7768 656e  t challenge when
+00013500: 2063 616c 6962 7261 7469 6e67 2077 6974   calibrating wit
+00013510: 686f 7574 206e 6567 6174 6976 6573 2e20  hout negatives. 
+00013520: 5468 6174 2064 6570 656e 6473 206f 6e0a  That depends on.
+00013530: 2020 2020 2020 2020 7468 6520 7573 6572          the user
+00013540: 2063 686f 6963 6520 6f66 2074 7269 706c   choice of tripl
+00013550: 6573 2074 6f20 6265 2065 7661 6c75 6174  es to be evaluat
+00013560: 6564 2064 7572 696e 6720 7465 7374 2074  ed during test t
+00013570: 696d 652e 0a20 2020 2020 2020 204c 6574  ime..        Let
+00013580: 2773 2074 616b 6520 7468 6520 574e 3131  's take the WN11
+00013590: 2064 6174 6173 6574 2061 7320 616e 2065   dataset as an e
+000135a0: 7861 6d70 6c65 3a20 6974 2068 6173 2061  xample: it has a
+000135b0: 726f 756e 6420 3530 2520 706f 7369 7469  round 50% positi
+000135c0: 7665 7320 7472 6970 6c65 7320 6f6e 2062  ves triples on b
+000135d0: 6f74 6820 7468 6520 7661 6c69 6461 7469  oth the validati
+000135e0: 6f6e 2073 6574 0a20 2020 2020 2020 2061  on set.        a
+000135f0: 6e64 2074 6573 7420 7365 742c 2073 6f20  nd test set, so 
+00013600: 7468 6520 706f 7369 7469 7665 2062 6173  the positive bas
+00013610: 6520 7261 7465 2066 6f6c 6c6f 7773 2074  e rate follows t
+00013620: 6f20 6265 2035 3025 2e20 486f 7765 7665  o be 50%. Howeve
+00013630: 722c 2073 686f 756c 6420 7468 6520 7573  r, should the us
+00013640: 6572 2072 6573 616d 706c 6520 6974 2074  er resample it t
+00013650: 6f20 6861 7665 0a20 2020 2020 2020 2037  o have.        7
+00013660: 3525 2070 6f73 6974 6976 6573 2061 6e64  5% positives and
+00013670: 2032 3525 206e 6567 6174 6976 6573 2c20   25% negatives, 
+00013680: 7468 6520 7072 6576 696f 7573 2063 616c  the previous cal
+00013690: 6962 7261 7469 6f6e 2077 6f75 6c64 2062  ibration would b
+000136a0: 6520 6465 6772 6164 6564 2e20 5468 6520  e degraded. The 
+000136b0: 7573 6572 206d 7573 7420 7265 6361 6c69  user must recali
+000136c0: 6272 6174 650a 2020 2020 2020 2020 7468  brate.        th
+000136d0: 6520 6d6f 6465 6c20 7769 7468 2061 2037  e model with a 7
+000136e0: 3525 2070 6f73 6974 6976 6520 6261 7365  5% positive base
+000136f0: 2072 6174 652e 2054 6865 7265 666f 7265   rate. Therefore
+00013700: 2c20 7468 6973 2070 6172 616d 6574 6572  , this parameter
+00013710: 2064 6570 656e 6473 206f 6e20 686f 7720   depends on how 
+00013720: 7468 6520 7573 6572 2068 616e 646c 6573  the user handles
+00013730: 2074 6865 0a20 2020 2020 2020 2064 6174   the.        dat
+00013740: 6173 6574 2061 6e64 2063 616e 6e6f 7420  aset and cannot 
+00013750: 6265 2064 6574 6572 6d69 6e65 6420 6175  be determined au
+00013760: 746f 6d61 7469 6361 6c6c 7920 6f72 2061  tomatically or a
+00013770: 2070 7269 6f72 692e 0a0a 2020 2020 2020   priori...      
+00013780: 2020 2e2e 204e 6f74 6520 3a3a 0a20 2020    .. Note ::.   
+00013790: 2020 2020 2020 2020 203a 6369 7465 3a60           :cite:`
+000137a0: 6361 6c69 6272 6174 696f 6e60 2060 6361  calibration` `ca
+000137b0: 6c69 6272 6174 696f 6e20 6578 7065 7269  libration experi
+000137c0: 6d65 6e74 7320 6176 6169 6c61 626c 6520  ments available 
+000137d0: 6865 7265 0a20 2020 2020 2020 2020 2020  here.           
+000137e0: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
+000137f0: 2e63 6f6d 2f41 6363 656e 7475 7265 2f41  .com/Accenture/A
+00013800: 6d70 6c69 4772 6170 682f 7472 6565 2f70  mpliGraph/tree/p
+00013810: 6170 6572 2f49 434c 522d 3230 2f65 7870  aper/ICLR-20/exp
+00013820: 6572 696d 656e 7473 2f49 434c 522d 3230  eriments/ICLR-20
+00013830: 3e60 5f2e 0a0a 0a20 2020 2020 2020 2050  >`_....        P
+00013840: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00013850: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00013860: 2020 2020 2058 5f70 6f73 203a 206e 702e       X_pos : np.
+00013870: 6172 7261 792c 2073 6861 7065 2028 6e2c  array, shape (n,
+00013880: 3329 206f 7220 7374 7220 6f72 2047 7261  3) or str or Gra
+00013890: 7068 4461 7461 4c6f 6164 6572 206f 7220  phDataLoader or 
+000138a0: 4162 7374 7261 6374 4772 6170 6850 6172  AbstractGraphPar
+000138b0: 7469 7469 6f6e 6572 0a20 2020 2020 2020  titioner.       
+000138c0: 2020 2020 2044 6174 6120 4f52 2046 696c       Data OR Fil
+000138d0: 656e 616d 6520 6f66 2074 6865 2064 6174  ename of the dat
+000138e0: 6120 6669 6c65 204f 5220 4461 7461 2048  a file OR Data H
+000138f0: 616e 646c 6520 746f 2062 6520 7573 6564  andle to be used
+00013900: 2061 7320 706f 7369 7469 7665 2074 7269   as positive tri
+00013910: 706c 6573 2e0a 2020 2020 2020 2020 585f  ples..        X_
+00013920: 6e65 6720 3a20 6e70 2e61 7272 6179 2c20  neg : np.array, 
+00013930: 7368 6170 6520 286e 2c33 2920 6f72 2073  shape (n,3) or s
+00013940: 7472 206f 7220 4772 6170 6844 6174 614c  tr or GraphDataL
+00013950: 6f61 6465 7220 6f72 2041 6273 7472 6163  oader or Abstrac
+00013960: 7447 7261 7068 5061 7274 6974 696f 6e65  tGraphPartitione
+00013970: 720a 2020 2020 2020 2020 2020 2020 4461  r.            Da
+00013980: 7461 204f 5220 4669 6c65 6e61 6d65 206f  ta OR Filename o
+00013990: 6620 7468 6520 6461 7461 2066 696c 6520  f the data file 
+000139a0: 4f52 2044 6174 6120 4861 6e64 6c65 2074  OR Data Handle t
+000139b0: 6f20 6265 2075 7365 6420 6173 206e 6567  o be used as neg
+000139c0: 6174 6976 6520 7472 6970 6c65 732e 0a0a  ative triples...
+000139d0: 2020 2020 2020 2020 2020 2020 4966 2060              If `
+000139e0: 4e6f 6e65 602c 2074 6865 206e 6567 6174  None`, the negat
+000139f0: 6976 6520 7472 6970 6c65 7320 6172 6520  ive triples are 
+00013a00: 6765 6e65 7261 7465 6420 7669 6120 636f  generated via co
+00013a10: 7272 7570 7469 6f6e 730a 2020 2020 2020  rruptions.      
+00013a20: 2020 2020 2020 616e 6420 7468 6520 7573        and the us
+00013a30: 6572 206d 7573 7420 7072 6f76 6964 6520  er must provide 
+00013a40: 6120 706f 7369 7469 7665 2062 6173 6520  a positive base 
+00013a50: 7261 7465 2069 6e73 7465 6164 2e0a 0a20  rate instead... 
+00013a60: 2020 2020 2020 2070 6f73 6974 6976 655f         positive_
+00013a70: 6261 7365 5f72 6174 653a 2066 6c6f 6174  base_rate: float
+00013a80: 0a20 2020 2020 2020 2020 2020 2042 6173  .            Bas
+00013a90: 6520 7261 7465 206f 6620 706f 7369 7469  e rate of positi
+00013aa0: 7665 2073 7461 7465 6d65 6e74 732e 0a0a  ve statements...
+00013ab0: 2020 2020 2020 2020 2020 2020 466f 7220              For 
+00013ac0: 6578 616d 706c 652c 2069 6620 7765 2061  example, if we a
+00013ad0: 7373 756d 6520 7468 6572 6520 6973 2061  ssume there is a
+00013ae0: 6e20 6576 656e 2063 6861 6e63 6520 666f  n even chance fo
+00013af0: 7220 616e 7920 7175 6572 7920 746f 2062  r any query to b
+00013b00: 6520 7472 7565 2c20 7468 6520 6261 7365  e true, the base
+00013b10: 2072 6174 6520 776f 756c 6420 6265 2035   rate would be 5
+00013b20: 3025 2e0a 0a20 2020 2020 2020 2020 2020  0%...           
+00013b30: 2049 6620 6060 585f 6e65 6760 6020 6973   If ``X_neg`` is
+00013b40: 2070 726f 7669 6465 6420 616e 6420 6060   provided and ``
+00013b50: 706f 7369 7469 7665 5f62 6173 655f 7261  positive_base_ra
+00013b60: 7465 3d4e 6f6e 6560 602c 2074 6865 2072  te=None``, the r
+00013b70: 656c 6174 6976 6520 7369 7a65 7320 6f66  elative sizes of
+00013b80: 2060 6058 5f70 6f73 6060 2061 6e64 2060   ``X_pos`` and `
+00013b90: 6058 5f6e 6567 6060 0a20 2020 2020 2020  `X_neg``.       
+00013ba0: 2020 2020 2077 696c 6c20 6265 2075 7365       will be use
+00013bb0: 6420 746f 2064 6574 6572 6d69 6e65 2074  d to determine t
+00013bc0: 6865 2062 6173 6520 7261 7465 2e20 5361  he base rate. Sa
+00013bd0: 7920 7765 2068 6176 6520 3530 2070 6f73  y we have 50 pos
+00013be0: 6974 6976 6520 7472 6970 6c65 7320 616e  itive triples an
+00013bf0: 6420 3230 3020 6e65 6761 7469 7665 0a20  d 200 negative. 
+00013c00: 2020 2020 2020 2020 2020 2074 7269 706c             tripl
+00013c10: 6573 2c20 7468 6520 706f 7369 7469 7665  es, the positive
+00013c20: 2062 6173 6520 7261 7465 2077 696c 6c20   base rate will 
+00013c30: 6265 2061 7373 756d 6564 2074 6f20 6265  be assumed to be
+00013c40: 203a 6d61 7468 3a60 5c5c 6672 6163 7b35   :math:`\\frac{5
+00013c50: 307d 7b28 3530 2b32 3030 297d 203d 205c  0}{(50+200)} = \
+00013c60: 5c66 7261 637b 317d 7b35 7d20 3d20 302e  \frac{1}{5} = 0.
+00013c70: 3260 2e0a 0a20 2020 2020 2020 2020 2020  2`...           
+00013c80: 2054 6869 7320 7661 6c75 6520 6d75 7374   This value must
+00013c90: 2062 6520 3a6d 6174 683a 605c 5c69 6e20   be :math:`\\in 
+00013ca0: 5b30 2c31 5d60 2e0a 2020 2020 2020 2020  [0,1]`..        
+00013cb0: 6261 7463 6865 735f 7369 7a65 3a20 696e  batches_size: in
+00013cc0: 740a 2020 2020 2020 2020 2020 2020 4261  t.            Ba
+00013cd0: 7463 6820 7369 7a65 2066 6f72 2070 6f73  tch size for pos
+00013ce0: 6974 6976 6573 2e0a 2020 2020 2020 2020  itives..        
+00013cf0: 6570 6f63 6873 3a20 696e 740a 2020 2020  epochs: int.    
+00013d00: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
+00013d10: 6620 6570 6f63 6873 2075 7365 6420 746f  f epochs used to
+00013d20: 2074 7261 696e 2074 6865 2050 6c61 7474   train the Platt
+00013d30: 2073 6361 6c69 6e67 206d 6f64 656c 2e0a   scaling model..
+00013d40: 2020 2020 2020 2020 2020 2020 4f6e 6c79              Only
+00013d50: 2061 7070 6c69 6573 2077 6865 6e20 6060   applies when ``
+00013d60: 585f 6e65 673d 4e6f 6e65 6060 2e0a 2020  X_neg=None``..  
+00013d70: 2020 2020 2020 7665 7262 6f73 653a 2062        verbose: b
+00013d80: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
+00013d90: 5665 7262 6f73 6974 7920 2864 6566 6175  Verbosity (defau
+00013da0: 6c74 3a20 6046 616c 7365 6029 2e0a 0a20  lt: `False`)... 
+00013db0: 2020 2020 2020 2045 7861 6d70 6c65 0a20         Example. 
+00013dc0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00013dd0: 2020 2020 2020 203e 3e3e 2066 726f 6d20         >>> from 
+00013de0: 616d 706c 6967 7261 7068 2e64 6174 6173  ampligraph.datas
+00013df0: 6574 7320 696d 706f 7274 206c 6f61 645f  ets import load_
+00013e00: 6662 3135 6b5f 3233 370a 2020 2020 2020  fb15k_237.      
+00013e10: 2020 3e3e 3e20 6672 6f6d 2061 6d70 6c69    >>> from ampli
+00013e20: 6772 6170 682e 6c61 7465 6e74 5f66 6561  graph.latent_fea
+00013e30: 7475 7265 7320 696d 706f 7274 2053 636f  tures import Sco
+00013e40: 7269 6e67 4261 7365 6445 6d62 6564 6469  ringBasedEmbeddi
+00013e50: 6e67 4d6f 6465 6c0a 2020 2020 2020 2020  ngModel.        
+00013e60: 3e3e 3e20 696d 706f 7274 206e 756d 7079  >>> import numpy
+00013e70: 2061 7320 6e70 0a20 2020 2020 2020 203e   as np.        >
+00013e80: 3e3e 2064 6174 6173 6574 203d 206c 6f61  >> dataset = loa
+00013e90: 645f 6662 3135 6b5f 3233 3728 290a 2020  d_fb15k_237().  
+00013ea0: 2020 2020 2020 3e3e 3e20 6d6f 6465 6c20        >>> model 
+00013eb0: 3d20 5363 6f72 696e 6742 6173 6564 456d  = ScoringBasedEm
+00013ec0: 6265 6464 696e 674d 6f64 656c 2865 7461  beddingModel(eta
+00013ed0: 3d35 2c0a 2020 2020 2020 2020 3e3e 3e20  =5,.        >>> 
+00013ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f00: 2020 206b 3d33 3030 2c0a 2020 2020 2020     k=300,.      
+00013f10: 2020 3e3e 3e20 2020 2020 2020 2020 2020    >>>           
+00013f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f30: 2020 2020 2020 2020 2073 636f 7269 6e67           scoring
+00013f40: 5f74 7970 653d 2743 6f6d 706c 4578 2729  _type='ComplEx')
+00013f50: 0a20 2020 2020 2020 203e 3e3e 206d 6f64  .        >>> mod
+00013f60: 656c 2e63 6f6d 7069 6c65 286f 7074 696d  el.compile(optim
+00013f70: 697a 6572 3d27 6164 616d 272c 206c 6f73  izer='adam', los
+00013f80: 733d 276e 6c6c 2729 0a20 2020 2020 2020  s='nll').       
+00013f90: 203e 3e3e 206d 6f64 656c 2e66 6974 2864   >>> model.fit(d
+00013fa0: 6174 6173 6574 5b27 7472 6169 6e27 5d2c  ataset['train'],
+00013fb0: 0a20 2020 2020 2020 203e 3e3e 2020 2020  .        >>>    
+00013fc0: 2020 2020 2020 2062 6174 6368 5f73 697a         batch_siz
+00013fd0: 653d 3130 3030 302c 0a20 2020 2020 2020  e=10000,.       
+00013fe0: 203e 3e3e 2020 2020 2020 2020 2020 2065   >>>           e
+00013ff0: 706f 6368 733d 3529 0a20 2020 2020 2020  pochs=5).       
+00014000: 203e 3e3e 2070 7269 6e74 2827 5261 7720   >>> print('Raw 
+00014010: 7363 6f72 6573 2028 736f 7274 6564 293a  scores (sorted):
+00014020: 272c 206e 702e 736f 7274 286d 6f64 656c  ', np.sort(model
+00014030: 2e70 7265 6469 6374 2864 6174 6173 6574  .predict(dataset
+00014040: 5b27 7465 7374 275d 2929 290a 2020 2020  ['test']))).    
+00014050: 2020 2020 3e3e 3e20 7072 696e 7428 2749      >>> print('I
+00014060: 6e64 6963 6573 206f 6274 6169 6e65 6420  ndices obtained 
+00014070: 6279 2073 6f72 7469 6e67 2028 7363 6f72  by sorting (scor
+00014080: 6573 293a 272c 206e 702e 6172 6773 6f72  es):', np.argsor
+00014090: 7428 6d6f 6465 6c2e 7072 6564 6963 7428  t(model.predict(
+000140a0: 6461 7461 7365 745b 2774 6573 7427 5d29  dataset['test'])
+000140b0: 2929 0a20 2020 2020 2020 2052 6177 2073  )).        Raw s
+000140c0: 636f 7265 7320 2873 6f72 7465 6429 3a20  cores (sorted): 
+000140d0: 5b2d 312e 3036 3839 3737 3820 2020 2d30  [-1.0689778   -0
+000140e0: 2e34 3230 3832 3031 3220 202d 302e 3339  .42082012  -0.39
+000140f0: 3838 3738 3837 202e 2e2e 2020 332e 3236  887887 ...  3.26
+00014100: 3138 3338 2020 332e 3237 3535 3737 3320  1838  3.2755773 
+00014110: 2033 2e32 3736 3833 3534 205d 0a20 2020   3.2768354 ].   
+00014120: 2020 2020 2049 6e64 6963 6573 206f 6274       Indices obt
+00014130: 6169 6e65 6420 6279 2073 6f72 7469 6e67  ained by sorting
+00014140: 2028 7363 6f72 6573 293a 205b 2033 3833   (scores): [ 383
+00014150: 3420 3138 3633 3420 2034 3036 3620 2e2e  4 18634  4066 ..
+00014160: 2e20 2036 3233 3720 3133 3633 3320 3130  .  6237 13633 10
+00014170: 3936 315d 0a20 2020 2020 2020 203e 3e3e  961].        >>>
+00014180: 206d 6f64 656c 2e63 616c 6962 7261 7465   model.calibrate
+00014190: 2864 6174 6173 6574 5b27 7465 7374 275d  (dataset['test']
+000141a0: 2c0a 2020 2020 2020 2020 3e3e 3e20 2020  ,.        >>>   
+000141b0: 2020 2020 2020 2020 2020 2020 2020 6261                ba
+000141c0: 7463 685f 7369 7a65 3d31 3030 3030 2c0a  tch_size=10000,.
+000141d0: 2020 2020 2020 2020 3e3e 3e20 2020 2020          >>>     
+000141e0: 2020 2020 2020 2020 2020 2020 706f 7369              posi
+000141f0: 7469 7665 5f62 6173 655f 7261 7465 3d30  tive_base_rate=0
+00014200: 2e39 2c0a 2020 2020 2020 2020 3e3e 3e20  .9,.        >>> 
+00014210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014220: 6570 6f63 6873 3d31 3030 290a 2020 2020  epochs=100).    
+00014230: 2020 2020 3e3e 3e20 7072 696e 7428 2743      >>> print('C
+00014240: 616c 6962 7261 7465 6420 7363 6f72 6573  alibrated scores
+00014250: 2028 736f 7274 6564 293a 272c 206e 702e   (sorted):', np.
+00014260: 736f 7274 286d 6f64 656c 2e70 7265 6469  sort(model.predi
+00014270: 6374 5f70 726f 6261 2864 6174 6173 6574  ct_proba(dataset
+00014280: 5b27 7465 7374 275d 2929 290a 2020 2020  ['test']))).    
+00014290: 2020 2020 3e3e 3e20 7072 696e 7428 2749      >>> print('I
+000142a0: 6e64 6963 6573 206f 6274 6169 6e65 6420  ndices obtained 
+000142b0: 6279 2073 6f72 7469 6e67 2028 4361 6c69  by sorting (Cali
+000142c0: 6272 6174 6564 293a 272c 206e 702e 6172  brated):', np.ar
+000142d0: 6773 6f72 7428 6d6f 6465 6c2e 7072 6564  gsort(model.pred
+000142e0: 6963 745f 7072 6f62 6128 6461 7461 7365  ict_proba(datase
+000142f0: 745b 2774 6573 7427 5d29 2929 0a20 2020  t['test']))).   
+00014300: 2020 2020 2043 616c 6962 7261 7465 6420       Calibrated 
+00014310: 7363 6f72 6573 2028 736f 7274 6564 293a  scores (sorted):
+00014320: 205b 302e 3439 3534 3739 3832 2030 2e35   [0.49547982 0.5
+00014330: 3339 3639 3936 2020 302e 3534 3131 3839  396996  0.541189
+00014340: 3535 202e 2e2e 2030 2e37 3632 3432 3435  55 ... 0.7624245
+00014350: 2020 302e 3736 3331 3034 3420 2030 2e37    0.7631044  0.7
+00014360: 3633 3136 3635 355d 0a20 2020 2020 2020  6316655].       
+00014370: 2049 6e64 6963 6573 206f 6274 6169 6e65   Indices obtaine
+00014380: 6420 6279 2073 6f72 7469 6e67 2028 4361  d by sorting (Ca
+00014390: 6c69 6272 6174 6564 293a 205b 2033 3833  librated): [ 383
+000143a0: 3420 3138 3633 3420 2034 3036 3620 2e2e  4 18634  4066 ..
+000143b0: 2e20 2036 3233 3720 3133 3633 3320 3130  .  6237 13633 10
+000143c0: 3936 315d 0a0a 2020 2020 2020 2020 2222  961]..        ""
+000143d0: 220a 2020 2020 2020 2020 7365 6c66 2e69  ".        self.i
+000143e0: 735f 6361 6c69 6272 6174 6564 203d 2046  s_calibrated = F
+000143f0: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
+00014400: 615f 6861 6e64 6c65 725f 6361 6c69 6272  a_handler_calibr
+00014410: 6174 655f 706f 7320 3d20 6461 7461 5f61  ate_pos = data_a
+00014420: 6461 7074 6572 2e44 6174 6148 616e 646c  dapter.DataHandl
+00014430: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
+00014440: 585f 706f 732c 0a20 2020 2020 2020 2020  X_pos,.         
+00014450: 2020 2062 6174 6368 5f73 697a 653d 6261     batch_size=ba
+00014460: 7463 685f 7369 7a65 2c0a 2020 2020 2020  tch_size,.      
+00014470: 2020 2020 2020 6461 7461 7365 745f 7479        dataset_ty
+00014480: 7065 3d22 7465 7374 222c 0a20 2020 2020  pe="test",.     
+00014490: 2020 2020 2020 2065 706f 6368 733d 6570         epochs=ep
+000144a0: 6f63 6873 2c0a 2020 2020 2020 2020 2020  ochs,.          
+000144b0: 2020 7573 655f 6669 6c74 6572 3d46 616c    use_filter=Fal
+000144c0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+000144d0: 7573 655f 696e 6465 7865 723d 7365 6c66  use_indexer=self
+000144e0: 2e64 6174 615f 696e 6465 7865 722c 0a20  .data_indexer,. 
+000144f0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00014500: 2020 706f 735f 7369 7a65 203d 2064 6174    pos_size = dat
+00014510: 615f 6861 6e64 6c65 725f 6361 6c69 6272  a_handler_calibr
+00014520: 6174 655f 706f 732e 5f70 6172 656e 745f  ate_pos._parent_
+00014530: 6164 6170 7465 722e 6765 745f 6461 7461  adapter.get_data
+00014540: 5f73 697a 6528 290a 2020 2020 2020 2020  _size().        
+00014550: 6e65 675f 7369 7a65 203d 2070 6f73 5f73  neg_size = pos_s
+00014560: 697a 650a 0a20 2020 2020 2020 2069 6620  ize..        if 
+00014570: 585f 6e65 6720 6973 204e 6f6e 653a 0a20  X_neg is None:. 
+00014580: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00014590: 7420 280a 2020 2020 2020 2020 2020 2020  t (.            
+000145a0: 2020 2020 706f 7369 7469 7665 5f62 6173      positive_bas
+000145b0: 655f 7261 7465 2069 7320 6e6f 7420 4e6f  e_rate is not No
+000145c0: 6e65 0a20 2020 2020 2020 2020 2020 2029  ne.            )
+000145d0: 2c20 2250 6c65 6173 6520 7072 6f76 6964  , "Please provid
+000145e0: 6520 7468 6520 6e65 6761 7469 7665 7320  e the negatives 
+000145f0: 6f72 2070 6f73 6974 6976 6520 6261 7365  or positive base
+00014600: 2072 6174 6521 220a 2020 2020 2020 2020   rate!".        
+00014610: 2020 2020 7365 6c66 2e69 735f 6361 6c69      self.is_cali
+00014620: 6272 6174 655f 7769 7468 5f63 6f72 7275  brate_with_corru
+00014630: 7074 696f 6e20 3d20 5472 7565 0a20 2020  ption = True.   
+00014640: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00014650: 2020 2020 2020 2073 656c 662e 6973 5f63         self.is_c
+00014660: 616c 6962 7261 7465 5f77 6974 685f 636f  alibrate_with_co
+00014670: 7272 7570 7469 6f6e 203d 2046 616c 7365  rruption = False
+00014680: 0a0a 2020 2020 2020 2020 2020 2020 706f  ..            po
+00014690: 735f 6261 7463 685f 636f 756e 7420 3d20  s_batch_count = 
+000146a0: 696e 7428 6e70 2e63 6569 6c28 706f 735f  int(np.ceil(pos_
+000146b0: 7369 7a65 202f 2062 6174 6368 5f73 697a  size / batch_siz
+000146c0: 6529 290a 0a20 2020 2020 2020 2020 2020  e))..           
+000146d0: 2064 6174 615f 6861 6e64 6c65 725f 6361   data_handler_ca
+000146e0: 6c69 6272 6174 655f 6e65 6720 3d20 6461  librate_neg = da
+000146f0: 7461 5f61 6461 7074 6572 2e44 6174 6148  ta_adapter.DataH
+00014700: 616e 646c 6572 280a 2020 2020 2020 2020  andler(.        
+00014710: 2020 2020 2020 2020 585f 6e65 672c 0a20          X_neg,. 
+00014720: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00014730: 6174 6368 5f73 697a 653d 6261 7463 685f  atch_size=batch_
+00014740: 7369 7a65 2c0a 2020 2020 2020 2020 2020  size,.          
+00014750: 2020 2020 2020 6461 7461 7365 745f 7479        dataset_ty
+00014760: 7065 3d22 7465 7374 222c 0a20 2020 2020  pe="test",.     
+00014770: 2020 2020 2020 2020 2020 2065 706f 6368             epoch
+00014780: 733d 6570 6f63 6873 2c0a 2020 2020 2020  s=epochs,.      
+00014790: 2020 2020 2020 2020 2020 7573 655f 6669            use_fi
+000147a0: 6c74 6572 3d46 616c 7365 2c0a 2020 2020  lter=False,.    
+000147b0: 2020 2020 2020 2020 2020 2020 7573 655f              use_
+000147c0: 696e 6465 7865 723d 7365 6c66 2e64 6174  indexer=self.dat
+000147d0: 615f 696e 6465 7865 722c 0a20 2020 2020  a_indexer,.     
+000147e0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+000147f0: 2020 2020 2020 6e65 675f 7369 7a65 203d        neg_size =
+00014800: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00014810: 2020 2064 6174 615f 6861 6e64 6c65 725f     data_handler_
+00014820: 6361 6c69 6272 6174 655f 6e65 672e 5f70  calibrate_neg._p
+00014830: 6172 656e 745f 6164 6170 7465 722e 6765  arent_adapter.ge
+00014840: 745f 6461 7461 5f73 697a 6528 290a 2020  t_data_size().  
+00014850: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00014860: 2020 2020 2020 2020 6e65 675f 6261 7463          neg_batc
+00014870: 685f 636f 756e 7420 3d20 696e 7428 6e70  h_count = int(np
+00014880: 2e63 6569 6c28 6e65 675f 7369 7a65 202f  .ceil(neg_size /
+00014890: 2062 6174 6368 5f73 697a 6529 290a 0a20   batch_size)).. 
+000148a0: 2020 2020 2020 2020 2020 2069 6620 706f             if po
+000148b0: 735f 6261 7463 685f 636f 756e 7420 213d  s_batch_count !=
+000148c0: 206e 6567 5f62 6174 6368 5f63 6f75 6e74   neg_batch_count
+000148d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000148e0: 2020 6261 7463 685f 7369 7a65 5f6e 6567    batch_size_neg
+000148f0: 203d 2069 6e74 286e 702e 6365 696c 286e   = int(np.ceil(n
+00014900: 6567 5f73 697a 6520 2f20 706f 735f 6261  eg_size / pos_ba
+00014910: 7463 685f 636f 756e 7429 290a 2020 2020  tch_count)).    
+00014920: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00014930: 5f68 616e 646c 6572 5f63 616c 6962 7261  _handler_calibra
+00014940: 7465 5f6e 6567 203d 2064 6174 615f 6164  te_neg = data_ad
+00014950: 6170 7465 722e 4461 7461 4861 6e64 6c65  apter.DataHandle
+00014960: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00014970: 2020 2020 2020 2058 5f6e 6567 2c0a 2020         X_neg,.  
+00014980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014990: 2020 6261 7463 685f 7369 7a65 3d62 6174    batch_size=bat
+000149a0: 6368 5f73 697a 655f 6e65 672c 0a20 2020  ch_size_neg,.   
+000149b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149c0: 2064 6174 6173 6574 5f74 7970 653d 2274   dataset_type="t
+000149d0: 6573 7422 2c0a 2020 2020 2020 2020 2020  est",.          
+000149e0: 2020 2020 2020 2020 2020 6570 6f63 6873            epochs
+000149f0: 3d65 706f 6368 732c 0a20 2020 2020 2020  =epochs,.       
+00014a00: 2020 2020 2020 2020 2020 2020 2075 7365               use
+00014a10: 5f66 696c 7465 723d 4661 6c73 652c 0a20  _filter=False,. 
+00014a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a30: 2020 2075 7365 5f69 6e64 6578 6572 3d73     use_indexer=s
+00014a40: 656c 662e 6461 7461 5f69 6e64 6578 6572  elf.data_indexer
+00014a50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014a60: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+00014a70: 2069 6620 706f 7369 7469 7665 5f62 6173   if positive_bas
+00014a80: 655f 7261 7465 2069 7320 4e6f 6e65 3a0a  e_rate is None:.
+00014a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014aa0: 706f 7369 7469 7665 5f62 6173 655f 7261  positive_base_ra
+00014ab0: 7465 203d 2070 6f73 5f73 697a 6520 2f20  te = pos_size / 
+00014ac0: 2870 6f73 5f73 697a 6520 2b20 6e65 675f  (pos_size + neg_
+00014ad0: 7369 7a65 290a 0a20 2020 2020 2020 2069  size)..        i
+00014ae0: 6620 706f 7369 7469 7665 5f62 6173 655f  f positive_base_
+00014af0: 7261 7465 2069 7320 6e6f 7420 4e6f 6e65  rate is not None
+00014b00: 2061 6e64 2028 0a20 2020 2020 2020 2020   and (.         
+00014b10: 2020 2070 6f73 6974 6976 655f 6261 7365     positive_base
+00014b20: 5f72 6174 6520 3c3d 2030 206f 7220 706f  _rate <= 0 or po
+00014b30: 7369 7469 7665 5f62 6173 655f 7261 7465  sitive_base_rate
+00014b40: 203e 3d20 310a 2020 2020 2020 2020 293a   >= 1.        ):
+00014b50: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00014b60: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+00014b70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00014b80: 706f 7369 7469 7665 5f62 6173 655f 7261  positive_base_ra
+00014b90: 7465 206d 7573 7420 6265 2061 2076 616c  te must be a val
+00014ba0: 7565 2062 6574 7765 656e 2030 2061 6e64  ue between 0 and
+00014bb0: 2031 2e22 0a20 2020 2020 2020 2020 2020   1.".           
+00014bc0: 2029 0a0a 2020 2020 2020 2020 7365 6c66   )..        self
+00014bd0: 2e63 616c 6962 7261 7469 6f6e 5f6c 6179  .calibration_lay
+00014be0: 6572 203d 2043 616c 6962 7261 7469 6f6e  er = Calibration
+00014bf0: 4c61 7965 7228 0a20 2020 2020 2020 2020  Layer(.         
+00014c00: 2020 2070 6f73 5f73 697a 652c 206e 6567     pos_size, neg
+00014c10: 5f73 697a 652c 2070 6f73 6974 6976 655f  _size, positive_
+00014c20: 6261 7365 5f72 6174 650a 2020 2020 2020  base_rate.      
+00014c30: 2020 290a 2020 2020 2020 2020 6361 6c69    ).        cali
+00014c40: 6272 6174 655f 6675 6e63 7469 6f6e 203d  brate_function =
+00014c50: 2073 656c 662e 6d61 6b65 5f63 616c 6962   self.make_calib
+00014c60: 7261 7465 5f66 756e 6374 696f 6e28 290a  rate_function().
+00014c70: 0a20 2020 2020 2020 206f 7074 696d 697a  .        optimiz
+00014c80: 6572 203d 2074 662e 6b65 7261 732e 6f70  er = tf.keras.op
+00014c90: 7469 6d69 7a65 7273 2e41 6461 6d28 290a  timizers.Adam().
+00014ca0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00014cb0: 7365 6c66 2e69 735f 6361 6c69 6272 6174  self.is_calibrat
+00014cc0: 655f 7769 7468 5f63 6f72 7275 7074 696f  e_with_corruptio
+00014cd0: 6e3a 0a20 2020 2020 2020 2020 2020 206e  n:.            n
+00014ce0: 6567 6174 6976 655f 6974 6572 6174 6f72  egative_iterator
+00014cf0: 203d 2069 7465 7228 0a20 2020 2020 2020   = iter(.       
+00014d00: 2020 2020 2020 2020 2064 6174 615f 6861           data_ha
+00014d10: 6e64 6c65 725f 6361 6c69 6272 6174 655f  ndler_calibrate_
+00014d20: 6e65 672e 656e 756d 6572 6174 655f 6570  neg.enumerate_ep
+00014d30: 6f63 6873 2829 0a20 2020 2020 2020 2020  ochs().         
+00014d40: 2020 2029 0a0a 2020 2020 2020 2020 666f     )..        fo
+00014d50: 7220 5f2c 2069 7465 7261 746f 7220 696e  r _, iterator in
+00014d60: 2064 6174 615f 6861 6e64 6c65 725f 6361   data_handler_ca
+00014d70: 6c69 6272 6174 655f 706f 732e 656e 756d  librate_pos.enum
+00014d80: 6572 6174 655f 6570 6f63 6873 2854 7275  erate_epochs(Tru
+00014d90: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00014da0: 6966 206e 6f74 2073 656c 662e 6973 5f63  if not self.is_c
+00014db0: 616c 6962 7261 7465 5f77 6974 685f 636f  alibrate_with_co
+00014dc0: 7272 7570 7469 6f6e 3a0a 2020 2020 2020  rruption:.      
+00014dd0: 2020 2020 2020 2020 2020 5f2c 206e 6567            _, neg
+00014de0: 5f68 616e 646c 6520 3d20 6e65 7874 286e  _handle = next(n
+00014df0: 6567 6174 6976 655f 6974 6572 6174 6f72  egative_iterator
+00014e00: 290a 0a20 2020 2020 2020 2020 2020 2077  )..            w
+00014e10: 6974 6820 6461 7461 5f68 616e 646c 6572  ith data_handler
+00014e20: 5f63 616c 6962 7261 7465 5f70 6f73 2e63  _calibrate_pos.c
+00014e30: 6174 6368 5f73 746f 705f 6974 6572 6174  atch_stop_iterat
+00014e40: 696f 6e28 293a 0a20 2020 2020 2020 2020  ion():.         
+00014e50: 2020 2020 2020 2066 6f72 2073 7465 7020         for step 
+00014e60: 696e 2064 6174 615f 6861 6e64 6c65 725f  in data_handler_
+00014e70: 6361 6c69 6272 6174 655f 706f 732e 7374  calibrate_pos.st
+00014e80: 6570 7328 293a 0a20 2020 2020 2020 2020  eps():.         
+00014e90: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00014ea0: 6c66 2e69 735f 6361 6c69 6272 6174 655f  lf.is_calibrate_
+00014eb0: 7769 7468 5f63 6f72 7275 7074 696f 6e3a  with_corruption:
+00014ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014ed0: 2020 2020 2020 2020 2073 636f 7265 735f           scores_
+00014ee0: 706f 732c 2073 636f 7265 735f 6e65 6720  pos, scores_neg 
+00014ef0: 3d20 6361 6c69 6272 6174 655f 6675 6e63  = calibrate_func
+00014f00: 7469 6f6e 2869 7465 7261 746f 7229 0a0a  tion(iterator)..
+00014f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f20: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00014f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f40: 2020 7363 6f72 6573 5f70 6f73 203d 2063    scores_pos = c
+00014f50: 616c 6962 7261 7465 5f66 756e 6374 696f  alibrate_functio
+00014f60: 6e28 6974 6572 6174 6f72 290a 2020 2020  n(iterator).    
+00014f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f80: 2020 2020 7769 7468 2064 6174 615f 6861      with data_ha
+00014f90: 6e64 6c65 725f 6361 6c69 6272 6174 655f  ndler_calibrate_
+00014fa0: 6e65 672e 6361 7463 685f 7374 6f70 5f69  neg.catch_stop_i
+00014fb0: 7465 7261 7469 6f6e 2829 3a0a 2020 2020  teration():.    
 00014fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fd0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00014fe0: 2020 2020 2020 2023 2075 7064 6174 6520         # update 
-00014ff0: 7468 6520 7472 6169 6e61 626c 6520 7061  the trainable pa
-00015000: 7261 6d73 0a20 2020 2020 2020 2020 2020  rams.           
-00015010: 2020 2020 2020 2020 206f 7074 696d 697a           optimiz
-00015020: 6572 2e61 7070 6c79 5f67 7261 6469 656e  er.apply_gradien
-00015030: 7473 280a 2020 2020 2020 2020 2020 2020  ts(.            
-00015040: 2020 2020 2020 2020 2020 2020 7a69 7028              zip(
-00015050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015060: 2020 2020 2020 2020 2020 2020 2067 7261               gra
-00015070: 6469 656e 7473 2c0a 2020 2020 2020 2020  dients,.        
-00015080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015090: 2020 2020 7365 6c66 2e63 616c 6962 7261      self.calibra
-000150a0: 7469 6f6e 5f6c 6179 6572 2e5f 7472 6169  tion_layer._trai
-000150b0: 6e61 626c 655f 7765 6967 6874 732c 0a20  nable_weights,. 
+00014fd0: 2020 2020 2020 2020 7363 6f72 6573 5f6e          scores_n
+00014fe0: 6567 203d 2063 616c 6962 7261 7465 5f66  eg = calibrate_f
+00014ff0: 756e 6374 696f 6e28 6e65 675f 6861 6e64  unction(neg_hand
+00015000: 6c65 290a 0a20 2020 2020 2020 2020 2020  le)..           
+00015010: 2020 2020 2020 2020 2077 6974 6820 7466           with tf
+00015020: 2e47 7261 6469 656e 7454 6170 6528 2920  .GradientTape() 
+00015030: 6173 2074 6170 653a 0a20 2020 2020 2020  as tape:.       
+00015040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015050: 206f 7574 203d 2073 656c 662e 6361 6c69   out = self.cali
+00015060: 6272 6174 696f 6e5f 6c61 7965 7228 7363  bration_layer(sc
+00015070: 6f72 6573 5f70 6f73 2c20 7363 6f72 6573  ores_pos, scores
+00015080: 5f6e 6567 2c20 3129 0a0a 2020 2020 2020  _neg, 1)..      
+00015090: 2020 2020 2020 2020 2020 2020 2020 6772                gr
+000150a0: 6164 6965 6e74 7320 3d20 7461 7065 2e67  adients = tape.g
+000150b0: 7261 6469 656e 7428 0a20 2020 2020 2020  radient(.       
 000150c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000150e0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-000150f0: 2020 2020 2020 2073 656c 662e 6973 5f63         self.is_c
-00015100: 616c 6962 7261 7465 6420 3d20 5472 7565  alibrated = True
-00015110: 0a0a 2020 2020 6465 6620 7072 6564 6963  ..    def predic
-00015120: 745f 7072 6f62 6128 7365 6c66 2c20 782c  t_proba(self, x,
-00015130: 2062 6174 6368 5f73 697a 653d 3332 2c20   batch_size=32, 
-00015140: 7665 7262 6f73 653d 302c 2063 616c 6c62  verbose=0, callb
-00015150: 6163 6b73 3d4e 6f6e 6529 3a0a 2020 2020  acks=None):.    
-00015160: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00015170: 436f 6d70 7574 6520 6361 6c69 6272 6174  Compute calibrat
-00015180: 6564 2073 636f 7265 7320 283a 6d61 7468  ed scores (:math
-00015190: 3a60 3020 e289 a420 7363 6f72 6520 e289  :`0 ... score ..
-000151a0: a420 3160 2920 666f 7220 7468 6520 696e  . 1`) for the in
-000151b0: 7075 7420 7472 6970 6c65 732e 0a0a 2020  put triples...  
-000151c0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-000151d0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000151e0: 2d2d 2d0a 2020 2020 2020 2020 783a 206e  ---.        x: n
-000151f0: 702e 6172 7261 792c 2073 6861 7065 2028  p.array, shape (
-00015200: 6e2c 3329 206f 7220 7374 7220 6f72 2047  n,3) or str or G
-00015210: 7261 7068 4461 7461 4c6f 6164 6572 206f  raphDataLoader o
-00015220: 7220 4162 7374 7261 6374 4772 6170 6850  r AbstractGraphP
-00015230: 6172 7469 7469 6f6e 6572 0a20 2020 2020  artitioner.     
-00015240: 2020 2020 2020 2044 6174 6120 4f52 2046         Data OR F
-00015250: 696c 656e 616d 6520 6f66 2074 6865 2064  ilename of the d
-00015260: 6174 6120 6669 6c65 204f 5220 4461 7461  ata file OR Data
-00015270: 2048 616e 646c 6520 746f 2062 6520 7573   Handle to be us
-00015280: 6564 2066 6f72 2074 7261 696e 696e 672e  ed for training.
-00015290: 0a20 2020 2020 2020 2062 6174 6368 5f73  .        batch_s
-000152a0: 697a 653a 2069 6e74 0a20 2020 2020 2020  ize: int.       
-000152b0: 2020 2020 2042 6174 6368 2073 697a 6520       Batch size 
-000152c0: 746f 2075 7365 2064 7572 696e 6720 7472  to use during tr
-000152d0: 6169 6e69 6e67 2e0a 2020 2020 2020 2020  aining..        
-000152e0: 2020 2020 4d61 7920 6265 206f 7665 7272      May be overr
-000152f0: 6964 6465 6e20 6966 2060 6078 6060 2069  idden if ``x`` i
-00015300: 7320 6047 7261 7068 4461 7461 4c6f 6164  s `GraphDataLoad
-00015310: 6572 6020 6f72 2060 4162 7374 7261 6374  er` or `Abstract
-00015320: 4772 6170 6850 6172 7469 7469 6f6e 6572  GraphPartitioner
-00015330: 6020 696e 7374 616e 6365 2e0a 2020 2020  ` instance..    
-00015340: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
-00015350: 6c0a 2020 2020 2020 2020 2020 2020 5665  l.            Ve
-00015360: 7262 6f73 6974 7920 6d6f 6465 2028 6465  rbosity mode (de
-00015370: 6661 756c 743a 2060 4661 6c73 6560 292e  fault: `False`).
-00015380: 0a20 2020 2020 2020 2063 616c 6c62 6163  .        callbac
-00015390: 6b73 3a20 6c69 7374 206f 6620 6b65 7261  ks: list of kera
-000153a0: 732e 6361 6c6c 6261 636b 732e 4361 6c6c  s.callbacks.Call
-000153b0: 6261 636b 2069 6e73 7461 6e63 6573 0a20  back instances. 
-000153c0: 2020 2020 2020 2020 2020 204c 6973 7420             List 
-000153d0: 6f66 2063 616c 6c62 6163 6b73 2074 6f20  of callbacks to 
-000153e0: 6170 706c 7920 6475 7269 6e67 2065 7661  apply during eva
-000153f0: 6c75 6174 696f 6e2e 0a0a 2020 2020 2020  luation...      
-00015400: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-00015410: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00015420: 2020 7363 6f72 6573 3a20 6e70 2e61 7272    scores: np.arr
-00015430: 6179 2c20 7368 6170 6520 286e 2c20 290a  ay, shape (n, ).
-00015440: 2020 2020 2020 2020 2020 2020 4361 6c69              Cali
-00015450: 6272 6174 6564 2073 636f 7265 7320 666f  brated scores fo
-00015460: 7220 7468 6520 696e 7075 7420 7472 6970  r the input trip
-00015470: 6c65 732e 0a0a 2020 2020 2020 2020 4578  les...        Ex
-00015480: 616d 706c 650a 2020 2020 2020 2020 2d2d  ample.        --
-00015490: 2d2d 2d2d 2d0a 2020 2020 2020 2020 3e3e  -----.        >>
-000154a0: 3e20 6672 6f6d 2061 6d70 6c69 6772 6170  > from ampligrap
-000154b0: 682e 6461 7461 7365 7473 2069 6d70 6f72  h.datasets impor
-000154c0: 7420 6c6f 6164 5f66 6231 356b 5f32 3337  t load_fb15k_237
-000154d0: 0a20 2020 2020 2020 203e 3e3e 2066 726f  .        >>> fro
-000154e0: 6d20 616d 706c 6967 7261 7068 2e6c 6174  m ampligraph.lat
-000154f0: 656e 745f 6665 6174 7572 6573 2069 6d70  ent_features imp
-00015500: 6f72 7420 5363 6f72 696e 6742 6173 6564  ort ScoringBased
-00015510: 456d 6265 6464 696e 674d 6f64 656c 0a20  EmbeddingModel. 
-00015520: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
-00015530: 7420 6e75 6d70 7920 6173 206e 700a 2020  t numpy as np.  
-00015540: 2020 2020 2020 3e3e 3e20 6461 7461 7365        >>> datase
-00015550: 7420 3d20 6c6f 6164 5f66 6231 356b 5f32  t = load_fb15k_2
-00015560: 3337 2829 0a20 2020 2020 2020 203e 3e3e  37().        >>>
-00015570: 206d 6f64 656c 203d 2053 636f 7269 6e67   model = Scoring
-00015580: 4261 7365 6445 6d62 6564 6469 6e67 4d6f  BasedEmbeddingMo
-00015590: 6465 6c28 6574 613d 352c 0a20 2020 2020  del(eta=5,.     
-000155a0: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
-000155b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155c0: 2020 2020 2020 2020 2020 6b3d 3330 302c            k=300,
-000155d0: 0a20 2020 2020 2020 203e 3e3e 2020 2020  .        >>>    
-000155e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015600: 7363 6f72 696e 675f 7479 7065 3d27 436f  scoring_type='Co
-00015610: 6d70 6c45 7827 290a 2020 2020 2020 2020  mplEx').        
-00015620: 3e3e 3e20 6d6f 6465 6c2e 636f 6d70 696c  >>> model.compil
-00015630: 6528 6f70 7469 6d69 7a65 723d 2761 6461  e(optimizer='ada
-00015640: 6d27 2c20 6c6f 7373 3d27 6e6c 6c27 290a  m', loss='nll').
-00015650: 2020 2020 2020 2020 3e3e 3e20 6d6f 6465          >>> mode
-00015660: 6c2e 6669 7428 6461 7461 7365 745b 2774  l.fit(dataset['t
-00015670: 7261 696e 275d 2c0a 2020 2020 2020 2020  rain'],.        
-00015680: 3e3e 3e20 2020 2020 2020 2020 2020 6261  >>>           ba
-00015690: 7463 685f 7369 7a65 3d31 3030 3030 2c0a  tch_size=10000,.
-000156a0: 2020 2020 2020 2020 3e3e 3e20 2020 2020          >>>     
-000156b0: 2020 2020 2020 6570 6f63 6873 3d35 290a        epochs=5).
-000156c0: 2020 2020 2020 2020 3e3e 3e20 7072 696e          >>> prin
-000156d0: 7428 2752 6177 2073 636f 7265 7320 2873  t('Raw scores (s
-000156e0: 6f72 7465 6429 3a27 2c20 6e70 2e73 6f72  orted):', np.sor
-000156f0: 7428 6d6f 6465 6c2e 7072 6564 6963 7428  t(model.predict(
-00015700: 6461 7461 7365 745b 2774 6573 7427 5d29  dataset['test'])
-00015710: 2929 0a20 2020 2020 2020 203e 3e3e 2070  )).        >>> p
-00015720: 7269 6e74 2827 496e 6469 6365 7320 6f62  rint('Indices ob
-00015730: 7461 696e 6564 2062 7920 736f 7274 696e  tained by sortin
-00015740: 6720 2873 636f 7265 7329 3a27 2c20 6e70  g (scores):', np
-00015750: 2e61 7267 736f 7274 286d 6f64 656c 2e70  .argsort(model.p
-00015760: 7265 6469 6374 2864 6174 6173 6574 5b27  redict(dataset['
-00015770: 7465 7374 275d 2929 290a 2020 2020 2020  test']))).      
-00015780: 2020 5261 7720 7363 6f72 6573 2028 736f    Raw scores (so
-00015790: 7274 6564 293a 205b 2d31 2e30 3338 3436  rted): [-1.03846
-000157a0: 3133 2020 2d30 2e34 3637 3532 3630 3820  13  -0.46752608 
-000157b0: 2d30 2e34 3531 3439 3837 3520 2e2e 2e20  -0.45149875 ... 
-000157c0: 2033 2e32 3839 3738 3434 2020 332e 3330   3.2897844  3.30
-000157d0: 3334 3331 3520 2033 2e33 3238 3036 3335  34315  3.3280635
-000157e0: 205d 0a20 2020 2020 2020 2049 6e64 6963   ].        Indic
-000157f0: 6573 206f 6274 6169 6e65 6420 6279 2073  es obtained by s
-00015800: 6f72 7469 6e67 2028 7363 6f72 6573 293a  orting (scores):
-00015810: 205b 2033 3833 3420 3138 3633 3420 2034   [ 3834 18634  4
-00015820: 3036 3620 2e2e 2e20 2031 3335 3520 3133  066 ...  1355 13
-00015830: 3633 3320 3130 3936 315d 0a20 2020 2020  633 10961].     
-00015840: 2020 203e 3e3e 206d 6f64 656c 2e63 616c     >>> model.cal
-00015850: 6962 7261 7465 2864 6174 6173 6574 5b27  ibrate(dataset['
-00015860: 7465 7374 275d 2c0a 2020 2020 2020 2020  test'],.        
-00015870: 3e3e 3e20 2020 2020 2020 2020 2020 2020  >>>             
-00015880: 2020 2020 6261 7463 685f 7369 7a65 3d31      batch_size=1
-00015890: 3030 3030 2c0a 2020 2020 2020 2020 3e3e  0000,.        >>
-000158a0: 3e20 2020 2020 2020 2020 2020 2020 2020  >               
-000158b0: 2020 706f 7369 7469 7665 5f62 6173 655f    positive_base_
-000158c0: 7261 7465 3d30 2e39 2c0a 2020 2020 2020  rate=0.9,.      
-000158d0: 2020 3e3e 3e20 2020 2020 2020 2020 2020    >>>           
-000158e0: 2020 2020 2020 6570 6f63 6873 3d31 3030        epochs=100
-000158f0: 290a 2020 2020 2020 2020 3e3e 3e20 7072  ).        >>> pr
-00015900: 696e 7428 2743 616c 6962 7261 7465 6420  int('Calibrated 
-00015910: 7363 6f72 6573 2028 736f 7274 6564 293a  scores (sorted):
-00015920: 272c 206e 702e 736f 7274 286d 6f64 656c  ', np.sort(model
-00015930: 2e70 7265 6469 6374 5f70 726f 6261 2864  .predict_proba(d
-00015940: 6174 6173 6574 5b27 7465 7374 275d 2929  ataset['test']))
-00015950: 290a 2020 2020 2020 2020 3e3e 3e20 7072  ).        >>> pr
-00015960: 696e 7428 2749 6e64 6963 6573 206f 6274  int('Indices obt
-00015970: 6169 6e65 6420 6279 2073 6f72 7469 6e67  ained by sorting
-00015980: 2028 4361 6c69 6272 6174 6564 293a 272c   (Calibrated):',
-00015990: 206e 702e 6172 6773 6f72 7428 6d6f 6465   np.argsort(mode
-000159a0: 6c2e 7072 6564 6963 745f 7072 6f62 6128  l.predict_proba(
-000159b0: 6461 7461 7365 745b 2774 6573 7427 5d29  dataset['test'])
-000159c0: 2929 0a20 2020 2020 2020 2043 616c 6962  )).        Calib
-000159d0: 7261 7465 6420 7363 6f72 6573 2028 736f  rated scores (so
-000159e0: 7274 6564 293a 205b 302e 3535 3533 3732  rted): [0.555372
-000159f0: 3520 2030 2e35 3535 3631 3038 2020 302e  5  0.5556108  0.
-00015a00: 3535 3638 3431 3520 202e 2e2e 2030 2e36  5568415  ... 0.6
-00015a10: 3231 3130 3131 2020 302e 3632 3338 3232  211011  0.623822
-00015a20: 3333 2030 2e36 3239 3735 3835 205d 0a20  33 0.6297585 ]. 
-00015a30: 2020 2020 2020 2049 6e64 6963 6573 206f         Indices o
-00015a40: 6274 6169 6e65 6420 6279 2073 6f72 7469  btained by sorti
-00015a50: 6e67 2028 4361 6c69 6272 6174 6564 293a  ng (Calibrated):
-00015a60: 205b 3134 3537 3320 3131 3537 3720 2034   [14573 11577  4
-00015a70: 3430 3420 2e2e 2e20 3137 3831 3720 3137  404 ... 17817 17
-00015a80: 3831 3620 2020 3733 335d 0a20 2020 2020  816   733].     
-00015a90: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00015aa0: 6620 6e6f 7420 7365 6c66 2e69 735f 6361  f not self.is_ca
-00015ab0: 6c69 6272 6174 6564 3a0a 2020 2020 2020  librated:.      
-00015ac0: 2020 2020 2020 6d73 6720 3d20 224d 6f64        msg = "Mod
-00015ad0: 656c 2068 6173 206e 6f74 2062 6565 6e20  el has not been 
-00015ae0: 6361 6c69 6272 6174 6564 2e20 5c0a 2020  calibrated. \.  
-00015af0: 2020 2020 2020 2020 2020 506c 6561 7365            Please
-00015b00: 2063 616c 6c20 606d 6f64 656c 2e63 616c   call `model.cal
-00015b10: 6962 7261 7465 282e 2e2e 2960 2062 6566  ibrate(...)` bef
-00015b20: 6f72 6520 7072 6564 6963 7469 6e67 2070  ore predicting p
-00015b30: 726f 6261 6269 6c69 7469 6573 2e22 0a0a  robabilities."..
-00015b40: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00015b50: 6520 5275 6e74 696d 6545 7272 6f72 286d  e RuntimeError(m
-00015b60: 7367 290a 0a20 2020 2020 2020 2073 656c  sg)..        sel
-00015b70: 662e 6461 7461 5f68 616e 646c 6572 5f74  f.data_handler_t
-00015b80: 6573 7420 3d20 6461 7461 5f61 6461 7074  est = data_adapt
-00015b90: 6572 2e44 6174 6148 616e 646c 6572 280a  er.DataHandler(.
-00015ba0: 2020 2020 2020 2020 2020 2020 782c 0a20              x,. 
-00015bb0: 2020 2020 2020 2020 2020 2062 6174 6368             batch
-00015bc0: 5f73 697a 653d 6261 7463 685f 7369 7a65  _size=batch_size
-00015bd0: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
-00015be0: 7461 7365 745f 7479 7065 3d22 7465 7374  taset_type="test
-00015bf0: 222c 0a20 2020 2020 2020 2020 2020 2065  ",.            e
-00015c00: 706f 6368 733d 312c 0a20 2020 2020 2020  pochs=1,.       
-00015c10: 2020 2020 2075 7365 5f66 696c 7465 723d       use_filter=
-00015c20: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-00015c30: 2020 2075 7365 5f69 6e64 6578 6572 3d73     use_indexer=s
-00015c40: 656c 662e 6461 7461 5f69 6e64 6578 6572  elf.data_indexer
-00015c50: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00015c60: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
-00015c70: 7374 616e 6365 2863 616c 6c62 6163 6b73  stance(callbacks
-00015c80: 2c20 6361 6c6c 6261 636b 735f 6d6f 6475  , callbacks_modu
-00015c90: 6c65 2e43 616c 6c62 6163 6b4c 6973 7429  le.CallbackList)
-00015ca0: 3a0a 2020 2020 2020 2020 2020 2020 6361  :.            ca
-00015cb0: 6c6c 6261 636b 7320 3d20 6361 6c6c 6261  llbacks = callba
-00015cc0: 636b 735f 6d6f 6475 6c65 2e43 616c 6c62  cks_module.Callb
-00015cd0: 6163 6b4c 6973 7428 0a20 2020 2020 2020  ackList(.       
-00015ce0: 2020 2020 2020 2020 2063 616c 6c62 6163           callbac
-00015cf0: 6b73 2c0a 2020 2020 2020 2020 2020 2020  ks,.            
-00015d00: 2020 2020 6164 645f 6869 7374 6f72 793d      add_history=
-00015d10: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00015d20: 2020 2020 2020 6164 645f 7072 6f67 6261        add_progba
-00015d30: 723d 7665 7262 6f73 6520 213d 2030 2c0a  r=verbose != 0,.
-00015d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d50: 6d6f 6465 6c3d 7365 6c66 2c0a 2020 2020  model=self,.    
-00015d60: 2020 2020 2020 2020 2020 2020 7665 7262              verb
-00015d70: 6f73 653d 7665 7262 6f73 652c 0a20 2020  ose=verbose,.   
-00015d80: 2020 2020 2020 2020 2020 2020 2065 706f               epo
-00015d90: 6368 733d 312c 0a20 2020 2020 2020 2020  chs=1,.         
-00015da0: 2020 2020 2020 2073 7465 7073 3d73 656c         steps=sel
-00015db0: 662e 6461 7461 5f68 616e 646c 6572 5f74  f.data_handler_t
-00015dc0: 6573 742e 696e 6665 7272 6564 5f73 7465  est.inferred_ste
-00015dd0: 7073 2c0a 2020 2020 2020 2020 2020 2020  ps,.            
-00015de0: 290a 0a20 2020 2020 2020 2070 7265 6469  )..        predi
-00015df0: 6374 5f66 756e 6374 696f 6e20 3d20 7365  ct_function = se
-00015e00: 6c66 2e6d 616b 655f 7072 6564 6963 745f  lf.make_predict_
-00015e10: 6675 6e63 7469 6f6e 2829 0a20 2020 2020  function().     
-00015e20: 2020 2063 616c 6c62 6163 6b73 2e6f 6e5f     callbacks.on_
-00015e30: 7072 6564 6963 745f 6265 6769 6e28 290a  predict_begin().
-00015e40: 2020 2020 2020 2020 6f75 7470 7574 7320          outputs 
-00015e50: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
-00015e60: 205f 2c20 6974 6572 6174 6f72 2069 6e20   _, iterator in 
-00015e70: 7365 6c66 2e64 6174 615f 6861 6e64 6c65  self.data_handle
-00015e80: 725f 7465 7374 2e65 6e75 6d65 7261 7465  r_test.enumerate
-00015e90: 5f65 706f 6368 7328 293a 0a20 2020 2020  _epochs():.     
-00015ea0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00015eb0: 2e64 6174 615f 6861 6e64 6c65 725f 7465  .data_handler_te
-00015ec0: 7374 2e63 6174 6368 5f73 746f 705f 6974  st.catch_stop_it
-00015ed0: 6572 6174 696f 6e28 293a 0a20 2020 2020  eration():.     
-00015ee0: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-00015ef0: 7465 7020 696e 2073 656c 662e 6461 7461  tep in self.data
-00015f00: 5f68 616e 646c 6572 5f74 6573 742e 7374  _handler_test.st
-00015f10: 6570 7328 293a 0a20 2020 2020 2020 2020  eps():.         
-00015f20: 2020 2020 2020 2020 2020 2063 616c 6c62             callb
-00015f30: 6163 6b73 2e6f 6e5f 7072 6564 6963 745f  acks.on_predict_
-00015f40: 6261 7463 685f 6265 6769 6e28 7374 6570  batch_begin(step
-00015f50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00015f60: 2020 2020 2020 6261 7463 685f 6f75 7470        batch_outp
-00015f70: 7574 7320 3d20 7072 6564 6963 745f 6675  uts = predict_fu
-00015f80: 6e63 7469 6f6e 2869 7465 7261 746f 7229  nction(iterator)
-00015f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015fa0: 2020 2020 2070 726f 6261 7320 3d20 7365       probas = se
-00015fb0: 6c66 2e63 616c 6962 7261 7469 6f6e 5f6c  lf.calibration_l
-00015fc0: 6179 6572 2862 6174 6368 5f6f 7574 7075  ayer(batch_outpu
-00015fd0: 7473 2c20 7472 6169 6e69 6e67 3d30 290a  ts, training=0).
-00015fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ff0: 2020 2020 6f75 7470 7574 732e 6170 7065      outputs.appe
-00016000: 6e64 2870 726f 6261 7329 0a0a 2020 2020  nd(probas)..    
-00016010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016020: 6361 6c6c 6261 636b 732e 6f6e 5f70 7265  callbacks.on_pre
-00016030: 6469 6374 5f62 6174 6368 5f65 6e64 280a  dict_batch_end(.
-00016040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016050: 2020 2020 2020 2020 7374 6570 2c20 7b22          step, {"
-00016060: 6f75 7470 7574 7322 3a20 6261 7463 685f  outputs": batch_
-00016070: 6f75 7470 7574 737d 0a20 2020 2020 2020  outputs}.       
-00016080: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00016090: 2020 2020 2020 2063 616c 6c62 6163 6b73         callbacks
-000160a0: 2e6f 6e5f 7072 6564 6963 745f 656e 6428  .on_predict_end(
-000160b0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000160c0: 206e 702e 636f 6e63 6174 656e 6174 6528   np.concatenate(
-000160d0: 6f75 7470 7574 7329 0a0a 2020 2020 6465  outputs)..    de
-000160e0: 6620 6765 745f 656d 6265 6464 696e 6773  f get_embeddings
-000160f0: 2873 656c 662c 2065 6e74 6974 6965 732c  (self, entities,
-00016100: 2065 6d62 6564 6469 6e67 5f74 7970 653d   embedding_type=
-00016110: 2265 2229 3a0a 2020 2020 2020 2020 2222  "e"):.        ""
-00016120: 2247 6574 2074 6865 2065 6d62 6564 6469  "Get the embeddi
-00016130: 6e67 7320 6f66 2065 6e74 6974 6965 7320  ngs of entities 
-00016140: 6f72 2072 656c 6174 696f 6e73 2e0a 0a20  or relations... 
-00016150: 2020 2020 2020 202e 2e20 4e6f 7465 203a         .. Note :
-00016160: 3a0a 0a20 2020 2020 2020 2020 2020 2055  :..            U
-00016170: 7365 203a 6d65 7468 3a60 616d 706c 6967  se :meth:`amplig
-00016180: 7261 7068 2e75 7469 6c73 2e63 7265 6174  raph.utils.creat
-00016190: 655f 7465 6e73 6f72 626f 6172 645f 7669  e_tensorboard_vi
-000161a0: 7375 616c 697a 6174 696f 6e73 6020 746f  sualizations` to
-000161b0: 2076 6973 7561 6c69 7a65 2074 6865 2065   visualize the e
-000161c0: 6d62 6564 6469 6e67 7320 7769 7468 2054  mbeddings with T
-000161d0: 656e 736f 7242 6f61 7264 2e0a 0a20 2020  ensorBoard...   
-000161e0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-000161f0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00016200: 2d2d 0a20 2020 2020 2020 2065 6e74 6974  --.        entit
-00016210: 6965 7320 3a20 6172 7261 792d 6c69 6b65  ies : array-like
-00016220: 2c20 7368 6170 653d 286e 290a 2020 2020  , shape=(n).    
-00016230: 2020 2020 2020 2020 5468 6520 656e 7469          The enti
-00016240: 7469 6573 2028 6f72 2072 656c 6174 696f  ties (or relatio
-00016250: 6e73 2920 6f66 2069 6e74 6572 6573 742e  ns) of interest.
-00016260: 2045 6c65 6d65 6e74 206f 6620 7468 6520   Element of the 
-00016270: 7665 6374 6f72 206d 7573 7420 6265 2074  vector must be t
-00016280: 6865 206f 7269 6769 6e61 6c20 7374 7269  he original stri
-00016290: 6e67 206c 6974 6572 616c 732c 2061 6e64  ng literals, and
-000162a0: 0a20 2020 2020 2020 2020 2020 206e 6f74  .            not
-000162b0: 2069 6e74 6572 6e61 6c20 4944 732e 0a20   internal IDs.. 
-000162c0: 2020 2020 2020 2065 6d62 6564 6469 6e67         embedding
-000162d0: 5f74 7970 6520 3a20 7374 720a 2020 2020  _type : str.    
-000162e0: 2020 2020 2020 2020 4966 2060 2765 2760          If `'e'`
-000162f0: 2069 7320 7061 7373 6564 2c20 6060 656e   is passed, ``en
-00016300: 7469 7469 6573 6060 2061 7267 756d 656e  tities`` argumen
-00016310: 7420 7769 6c6c 2062 6520 636f 6e73 6964  t will be consid
-00016320: 6572 6564 2061 7320 6120 6c69 7374 206f  ered as a list o
-00016330: 6620 6b6e 6f77 6c65 6467 6520 6772 6170  f knowledge grap
-00016340: 6820 656e 7469 7469 6573 0a20 2020 2020  h entities.     
-00016350: 2020 2020 2020 2028 692e 652e 2c20 6e6f         (i.e., no
-00016360: 6465 7329 2e20 4966 2073 6574 2074 6f20  des). If set to 
-00016370: 6027 7227 602c 2060 6065 6e74 6974 6965  `'r'`, ``entitie
-00016380: 7360 6020 7769 6c6c 2062 6520 7472 6561  s`` will be trea
-00016390: 7465 6420 6173 2072 656c 6174 696f 6e73  ted as relations
-000163a0: 2069 6e73 7465 6164 2e0a 2020 2020 2020   instead..      
-000163b0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-000163c0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-000163d0: 2020 656d 6265 6464 696e 6773 203a 206e    embeddings : n
-000163e0: 6461 7272 6179 2c20 7368 6170 6520 286e  darray, shape (n
-000163f0: 2c20 6b29 0a20 2020 2020 2020 2020 2020  , k).           
-00016400: 2041 6e20 6172 7261 7920 6f66 2060 6b60   An array of `k`
-00016410: 2d64 696d 656e 7369 6f6e 616c 2065 6d62  -dimensional emb
-00016420: 6564 6469 6e67 732e 0a0a 2020 2020 2020  eddings...      
-00016430: 2020 4578 616d 706c 650a 2020 2020 2020    Example.      
-00016440: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00016450: 2020 3e3e 3e20 6672 6f6d 2061 6d70 6c69    >>> from ampli
-00016460: 6772 6170 682e 6c61 7465 6e74 5f66 6561  graph.latent_fea
-00016470: 7475 7265 7320 696d 706f 7274 2053 636f  tures import Sco
-00016480: 7269 6e67 4261 7365 6445 6d62 6564 6469  ringBasedEmbeddi
-00016490: 6e67 4d6f 6465 6c0a 2020 2020 2020 2020  ngModel.        
-000164a0: 3e3e 3e20 6672 6f6d 2061 6d70 6c69 6772  >>> from ampligr
-000164b0: 6170 682e 6461 7461 7365 7473 2069 6d70  aph.datasets imp
-000164c0: 6f72 7420 6c6f 6164 5f66 6231 356b 5f32  ort load_fb15k_2
-000164d0: 3337 0a20 2020 2020 2020 203e 3e3e 2058  37.        >>> X
-000164e0: 203d 206c 6f61 645f 6662 3135 6b5f 3233   = load_fb15k_23
-000164f0: 3728 290a 2020 2020 2020 2020 3e3e 3e20  7().        >>> 
-00016500: 6d6f 6465 6c20 3d20 5363 6f72 696e 6742  model = ScoringB
-00016510: 6173 6564 456d 6265 6464 696e 674d 6f64  asedEmbeddingMod
-00016520: 656c 2865 7461 3d35 2c0a 2020 2020 2020  el(eta=5,.      
-00016530: 2020 3e3e 3e20 2020 2020 2020 2020 2020    >>>           
-00016540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016550: 2020 2020 2020 2020 206b 3d33 3030 2c0a           k=300,.
-00016560: 2020 2020 2020 2020 3e3e 3e20 2020 2020          >>>     
-00016570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016580: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016590: 636f 7269 6e67 5f74 7970 653d 2743 6f6d  coring_type='Com
-000165a0: 706c 4578 272c 0a20 2020 2020 2020 203e  plEx',.        >
-000165b0: 3e3e 2020 2020 2020 2020 2020 2020 2020  >>              
-000165c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000165d0: 2020 2020 2020 7365 6564 3d30 290a 2020        seed=0).  
-000165e0: 2020 2020 2020 3e3e 3e20 6d6f 6465 6c2e        >>> model.
-000165f0: 636f 6d70 696c 6528 6f70 7469 6d69 7a65  compile(optimize
-00016600: 723d 2761 6461 6d27 2c20 6c6f 7373 3d27  r='adam', loss='
-00016610: 6e6c 6c27 290a 2020 2020 2020 2020 3e3e  nll').        >>
-00016620: 3e20 6d6f 6465 6c2e 6669 7428 585b 2774  > model.fit(X['t
-00016630: 7261 696e 275d 2c0a 2020 2020 2020 2020  rain'],.        
-00016640: 3e3e 3e20 2020 2020 2020 2020 2020 6261  >>>           ba
-00016650: 7463 685f 7369 7a65 3d31 3030 3030 2c0a  tch_size=10000,.
-00016660: 2020 2020 2020 2020 3e3e 3e20 2020 2020          >>>     
-00016670: 2020 2020 2020 6570 6f63 6873 3d35 2c0a        epochs=5,.
-00016680: 2020 2020 2020 2020 3e3e 3e20 2020 2020          >>>     
-00016690: 2020 2020 2020 7665 7262 6f73 653d 4661        verbose=Fa
-000166a0: 6c73 6529 0a20 2020 2020 2020 203e 3e3e  lse).        >>>
-000166b0: 206d 6f64 656c 2e67 6574 5f65 6d62 6564   model.get_embed
-000166c0: 6469 6e67 7328 5b27 2f6d 2f30 3237 726e  dings(['/m/027rn
-000166d0: 272c 2027 2f6d 2f30 3676 3873 3027 5d2c  ', '/m/06v8s0'],
-000166e0: 2027 6527 290a 2020 2020 2020 2020 6172   'e').        ar
-000166f0: 7261 7928 5b5b 2030 2e30 3434 3832 3439  ray([[ 0.0448249
-00016700: 3620 2030 2e31 3139 3733 3930 3720 2030  6  0.11973907  0
-00016710: 2e30 3131 3137 3733 3320 2e2e 2e20 2d30  .01117733 ... -0
-00016720: 2e31 3333 3931 3932 3220 2030 2e31 3131  .13391922  0.111
-00016730: 3033 3535 3320 202d 302e 3038 3133 3238  03553  -0.081328
-00016740: 3631 5d0a 2020 2020 2020 2020 205b 2d30  61].         [-0
-00016750: 2e31 3031 3538 3338 3120 2030 2e30 3831  .10158381  0.081
-00016760: 3038 3630 3520 2d30 2e30 3736 3038 3637  08605 -0.0760867
-00016770: 3620 2e2e 2e20 2030 2e30 3539 3134 3037  6 ...  0.0591407
-00016780: 2020 302e 3032 3739 3134 3236 2020 302e    0.02791426  0.
-00016790: 3037 3535 3930 3136 5d5d 2c20 6474 7970  07559016]], dtyp
-000167a0: 653d 666c 6f61 7433 3229 0a20 2020 2020  e=float32).     
-000167b0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-000167c0: 6966 2065 6d62 6564 6469 6e67 5f74 7970  if embedding_typ
-000167d0: 6520 3d3d 2022 6522 3a0a 2020 2020 2020  e == "e":.      
-000167e0: 2020 2020 2020 6c6f 6f6b 7570 5f63 6f6e        lookup_con
-000167f0: 6365 7074 203d 2073 656c 662e 6461 7461  cept = self.data
-00016800: 5f69 6e64 6578 6572 2e67 6574 5f69 6e64  _indexer.get_ind
-00016810: 6578 6573 2865 6e74 6974 6965 732c 2022  exes(entities, "
-00016820: 6522 290a 2020 2020 2020 2020 2020 2020  e").            
-00016830: 6966 2073 656c 662e 6973 5f70 6172 7469  if self.is_parti
-00016840: 7469 6f6e 6564 5f74 7261 696e 696e 673a  tioned_training:
-00016850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016860: 2065 6d62 5f6f 7574 203d 205b 5d0a 2020   emb_out = [].  
-00016870: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00016880: 7468 2073 6865 6c76 652e 6f70 656e 280a  th shelve.open(.
-00016890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168a0: 2020 2020 7365 6c66 2e70 6172 7469 7469      self.partiti
-000168b0: 6f6e 6572 5f6d 6574 6164 6174 615b 2265  oner_metadata["e
-000168c0: 6e74 5f6d 6170 5f66 6e61 6d65 225d 0a20  nt_map_fname"]. 
-000168d0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000168e0: 2061 7320 656e 745f 656d 623a 0a20 2020   as ent_emb:.   
-000168f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016900: 2066 6f72 2065 6e74 5f69 6420 696e 206c   for ent_id in l
-00016910: 6f6f 6b75 705f 636f 6e63 6570 743a 0a20  ookup_concept:. 
-00016920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016930: 2020 2020 2020 2065 6d62 5f6f 7574 2e61         emb_out.a
-00016940: 7070 656e 6428 656e 745f 656d 625b 7374  ppend(ent_emb[st
-00016950: 7228 656e 745f 6964 295d 290a 2020 2020  r(ent_id)]).    
-00016960: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00016970: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00016980: 7475 726e 2074 662e 6e6e 2e65 6d62 6564  turn tf.nn.embed
-00016990: 6469 6e67 5f6c 6f6f 6b75 7028 0a20 2020  ding_lookup(.   
-000169a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169b0: 2073 656c 662e 656e 636f 6469 6e67 5f6c   self.encoding_l
-000169c0: 6179 6572 2e65 6e74 5f65 6d62 2c20 6c6f  ayer.ent_emb, lo
-000169d0: 6f6b 7570 5f63 6f6e 6365 7074 0a20 2020  okup_concept.   
-000169e0: 2020 2020 2020 2020 2020 2020 2029 2e6e               ).n
-000169f0: 756d 7079 2829 0a20 2020 2020 2020 2065  umpy().        e
-00016a00: 6c69 6620 656d 6265 6464 696e 675f 7479  lif embedding_ty
-00016a10: 7065 203d 3d20 2272 223a 0a20 2020 2020  pe == "r":.     
-00016a20: 2020 2020 2020 206c 6f6f 6b75 705f 636f         lookup_co
-00016a30: 6e63 6570 7420 3d20 7365 6c66 2e64 6174  ncept = self.dat
-00016a40: 615f 696e 6465 7865 722e 6765 745f 696e  a_indexer.get_in
-00016a50: 6465 7865 7328 656e 7469 7469 6573 2c20  dexes(entities, 
-00016a60: 2272 2229 0a20 2020 2020 2020 2020 2020  "r").           
-00016a70: 2069 6620 7365 6c66 2e69 735f 7061 7274   if self.is_part
-00016a80: 6974 696f 6e65 645f 7472 6169 6e69 6e67  itioned_training
-00016a90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00016aa0: 2020 656d 625f 6f75 7420 3d20 5b5d 0a20    emb_out = []. 
-00016ab0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00016ac0: 6974 6820 7368 656c 7665 2e6f 7065 6e28  ith shelve.open(
-00016ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016ae0: 2020 2020 2073 656c 662e 7061 7274 6974       self.partit
-00016af0: 696f 6e65 725f 6d65 7461 6461 7461 5b22  ioner_metadata["
-00016b00: 7265 6c5f 6d61 705f 666e 616d 6522 5d0a  rel_map_fname"].
-00016b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b20: 2920 6173 2072 656c 5f65 6d62 3a0a 2020  ) as rel_emb:.  
-00016b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b40: 2020 666f 7220 7265 6c5f 6964 2069 6e20    for rel_id in 
-00016b50: 6c6f 6f6b 7570 5f63 6f6e 6365 7074 3a0a  lookup_concept:.
-00016b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b70: 2020 2020 2020 2020 656d 625f 6f75 742e          emb_out.
-00016b80: 6170 7065 6e64 2872 656c 5f65 6d62 5b73  append(rel_emb[s
-00016b90: 7472 2872 656c 5f69 6429 5d29 0a20 2020  tr(rel_id)]).   
-00016ba0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00016bb0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00016bc0: 6574 7572 6e20 7466 2e6e 6e2e 656d 6265  eturn tf.nn.embe
-00016bd0: 6464 696e 675f 6c6f 6f6b 7570 280a 2020  dding_lookup(.  
-00016be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bf0: 2020 7365 6c66 2e65 6e63 6f64 696e 675f    self.encoding_
-00016c00: 6c61 7965 722e 7265 6c5f 656d 622c 206c  layer.rel_emb, l
-00016c10: 6f6f 6b75 705f 636f 6e63 6570 740a 2020  ookup_concept.  
-00016c20: 2020 2020 2020 2020 2020 2020 2020 292e                ).
-00016c30: 6e75 6d70 7928 290a 2020 2020 2020 2020  numpy().        
-00016c40: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00016c50: 2020 6d73 6720 3d20 2249 6e76 616c 6964    msg = "Invalid
-00016c60: 2065 6e74 6974 7920 7479 7065 3a20 7b7d   entity type: {}
-00016c70: 222e 666f 726d 6174 2865 6d62 6564 6469  ".format(embeddi
-00016c80: 6e67 5f74 7970 6529 0a20 2020 2020 2020  ng_type).       
-00016c90: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00016ca0: 4572 726f 7228 6d73 6729 0a              Error(msg).
+000150d0: 206f 7574 2c20 7365 6c66 2e63 616c 6962   out, self.calib
+000150e0: 7261 7469 6f6e 5f6c 6179 6572 2e5f 7472  ration_layer._tr
+000150f0: 6169 6e61 626c 655f 7765 6967 6874 730a  ainable_weights.
+00015100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015110: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00015120: 2020 2020 2020 2020 2020 2320 7570 6461            # upda
+00015130: 7465 2074 6865 2074 7261 696e 6162 6c65  te the trainable
+00015140: 2070 6172 616d 730a 2020 2020 2020 2020   params.        
+00015150: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
+00015160: 6d69 7a65 722e 6170 706c 795f 6772 6164  mizer.apply_grad
+00015170: 6965 6e74 7328 0a20 2020 2020 2020 2020  ients(.         
+00015180: 2020 2020 2020 2020 2020 2020 2020 207a                 z
+00015190: 6970 280a 2020 2020 2020 2020 2020 2020  ip(.            
+000151a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151b0: 6772 6164 6965 6e74 732c 0a20 2020 2020  gradients,.     
+000151c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151d0: 2020 2020 2020 2073 656c 662e 6361 6c69         self.cali
+000151e0: 6272 6174 696f 6e5f 6c61 7965 722e 5f74  bration_layer._t
+000151f0: 7261 696e 6162 6c65 5f77 6569 6768 7473  rainable_weights
+00015200: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00015210: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00015220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015230: 290a 2020 2020 2020 2020 7365 6c66 2e69  ).        self.i
+00015240: 735f 6361 6c69 6272 6174 6564 203d 2054  s_calibrated = T
+00015250: 7275 650a 0a20 2020 2064 6566 2070 7265  rue..    def pre
+00015260: 6469 6374 5f70 726f 6261 2873 656c 662c  dict_proba(self,
+00015270: 2078 2c20 6261 7463 685f 7369 7a65 3d33   x, batch_size=3
+00015280: 322c 2076 6572 626f 7365 3d30 2c20 6361  2, verbose=0, ca
+00015290: 6c6c 6261 636b 733d 4e6f 6e65 293a 0a20  llbacks=None):. 
+000152a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000152b0: 2020 2043 6f6d 7075 7465 2063 616c 6962     Compute calib
+000152c0: 7261 7465 6420 7363 6f72 6573 2028 3a6d  rated scores (:m
+000152d0: 6174 683a 6030 20e2 89a4 2073 636f 7265  ath:`0 ... score
+000152e0: 20e2 89a4 2031 6029 2066 6f72 2074 6865   ... 1`) for the
+000152f0: 2069 6e70 7574 2074 7269 706c 6573 2e0a   input triples..
+00015300: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00015310: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00015320: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2078  ------.        x
+00015330: 3a20 6e70 2e61 7272 6179 2c20 7368 6170  : np.array, shap
+00015340: 6520 286e 2c33 2920 6f72 2073 7472 206f  e (n,3) or str o
+00015350: 7220 4772 6170 6844 6174 614c 6f61 6465  r GraphDataLoade
+00015360: 7220 6f72 2041 6273 7472 6163 7447 7261  r or AbstractGra
+00015370: 7068 5061 7274 6974 696f 6e65 720a 2020  phPartitioner.  
+00015380: 2020 2020 2020 2020 2020 4461 7461 204f            Data O
+00015390: 5220 4669 6c65 6e61 6d65 206f 6620 7468  R Filename of th
+000153a0: 6520 6461 7461 2066 696c 6520 4f52 2044  e data file OR D
+000153b0: 6174 6120 4861 6e64 6c65 2074 6f20 6265  ata Handle to be
+000153c0: 2075 7365 6420 666f 7220 7472 6169 6e69   used for traini
+000153d0: 6e67 2e0a 2020 2020 2020 2020 6261 7463  ng..        batc
+000153e0: 685f 7369 7a65 3a20 696e 740a 2020 2020  h_size: int.    
+000153f0: 2020 2020 2020 2020 4261 7463 6820 7369          Batch si
+00015400: 7a65 2074 6f20 7573 6520 6475 7269 6e67  ze to use during
+00015410: 2074 7261 696e 696e 672e 0a20 2020 2020   training..     
+00015420: 2020 2020 2020 204d 6179 2062 6520 6f76         May be ov
+00015430: 6572 7269 6464 656e 2069 6620 6060 7860  erridden if ``x`
+00015440: 6020 6973 2060 4772 6170 6844 6174 614c  ` is `GraphDataL
+00015450: 6f61 6465 7260 206f 7220 6041 6273 7472  oader` or `Abstr
+00015460: 6163 7447 7261 7068 5061 7274 6974 696f  actGraphPartitio
+00015470: 6e65 7260 2069 6e73 7461 6e63 652e 0a20  ner` instance.. 
+00015480: 2020 2020 2020 2076 6572 626f 7365 3a20         verbose: 
+00015490: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
+000154a0: 2056 6572 626f 7369 7479 206d 6f64 6520   Verbosity mode 
+000154b0: 2864 6566 6175 6c74 3a20 6046 616c 7365  (default: `False
+000154c0: 6029 2e0a 2020 2020 2020 2020 6361 6c6c  `)..        call
+000154d0: 6261 636b 733a 206c 6973 7420 6f66 206b  backs: list of k
+000154e0: 6572 6173 2e63 616c 6c62 6163 6b73 2e43  eras.callbacks.C
+000154f0: 616c 6c62 6163 6b20 696e 7374 616e 6365  allback instance
+00015500: 730a 2020 2020 2020 2020 2020 2020 4c69  s.            Li
+00015510: 7374 206f 6620 6361 6c6c 6261 636b 7320  st of callbacks 
+00015520: 746f 2061 7070 6c79 2064 7572 696e 6720  to apply during 
+00015530: 6576 616c 7561 7469 6f6e 2e0a 0a20 2020  evaluation...   
+00015540: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00015550: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00015560: 2020 2020 2073 636f 7265 733a 206e 702e       scores: np.
+00015570: 6172 7261 792c 2073 6861 7065 2028 6e2c  array, shape (n,
+00015580: 2029 0a20 2020 2020 2020 2020 2020 2043   ).            C
+00015590: 616c 6962 7261 7465 6420 7363 6f72 6573  alibrated scores
+000155a0: 2066 6f72 2074 6865 2069 6e70 7574 2074   for the input t
+000155b0: 7269 706c 6573 2e0a 0a20 2020 2020 2020  riples...       
+000155c0: 2045 7861 6d70 6c65 0a20 2020 2020 2020   Example.       
+000155d0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+000155e0: 203e 3e3e 2066 726f 6d20 616d 706c 6967   >>> from amplig
+000155f0: 7261 7068 2e64 6174 6173 6574 7320 696d  raph.datasets im
+00015600: 706f 7274 206c 6f61 645f 6662 3135 6b5f  port load_fb15k_
+00015610: 3233 370a 2020 2020 2020 2020 3e3e 3e20  237.        >>> 
+00015620: 6672 6f6d 2061 6d70 6c69 6772 6170 682e  from ampligraph.
+00015630: 6c61 7465 6e74 5f66 6561 7475 7265 7320  latent_features 
+00015640: 696d 706f 7274 2053 636f 7269 6e67 4261  import ScoringBa
+00015650: 7365 6445 6d62 6564 6469 6e67 4d6f 6465  sedEmbeddingMode
+00015660: 6c0a 2020 2020 2020 2020 3e3e 3e20 696d  l.        >>> im
+00015670: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
+00015680: 0a20 2020 2020 2020 203e 3e3e 2064 6174  .        >>> dat
+00015690: 6173 6574 203d 206c 6f61 645f 6662 3135  aset = load_fb15
+000156a0: 6b5f 3233 3728 290a 2020 2020 2020 2020  k_237().        
+000156b0: 3e3e 3e20 6d6f 6465 6c20 3d20 5363 6f72  >>> model = Scor
+000156c0: 696e 6742 6173 6564 456d 6265 6464 696e  ingBasedEmbeddin
+000156d0: 674d 6f64 656c 2865 7461 3d35 2c0a 2020  gModel(eta=5,.  
+000156e0: 2020 2020 2020 3e3e 3e20 2020 2020 2020        >>>       
+000156f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015700: 2020 2020 2020 2020 2020 2020 206b 3d33               k=3
+00015710: 3030 2c0a 2020 2020 2020 2020 3e3e 3e20  00,.        >>> 
+00015720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015740: 2020 2073 636f 7269 6e67 5f74 7970 653d     scoring_type=
+00015750: 2743 6f6d 706c 4578 2729 0a20 2020 2020  'ComplEx').     
+00015760: 2020 203e 3e3e 206d 6f64 656c 2e63 6f6d     >>> model.com
+00015770: 7069 6c65 286f 7074 696d 697a 6572 3d27  pile(optimizer='
+00015780: 6164 616d 272c 206c 6f73 733d 276e 6c6c  adam', loss='nll
+00015790: 2729 0a20 2020 2020 2020 203e 3e3e 206d  ').        >>> m
+000157a0: 6f64 656c 2e66 6974 2864 6174 6173 6574  odel.fit(dataset
+000157b0: 5b27 7472 6169 6e27 5d2c 0a20 2020 2020  ['train'],.     
+000157c0: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
+000157d0: 2062 6174 6368 5f73 697a 653d 3130 3030   batch_size=1000
+000157e0: 302c 0a20 2020 2020 2020 203e 3e3e 2020  0,.        >>>  
+000157f0: 2020 2020 2020 2020 2065 706f 6368 733d           epochs=
+00015800: 3529 0a20 2020 2020 2020 203e 3e3e 2070  5).        >>> p
+00015810: 7269 6e74 2827 5261 7720 7363 6f72 6573  rint('Raw scores
+00015820: 2028 736f 7274 6564 293a 272c 206e 702e   (sorted):', np.
+00015830: 736f 7274 286d 6f64 656c 2e70 7265 6469  sort(model.predi
+00015840: 6374 2864 6174 6173 6574 5b27 7465 7374  ct(dataset['test
+00015850: 275d 2929 290a 2020 2020 2020 2020 3e3e  ']))).        >>
+00015860: 3e20 7072 696e 7428 2749 6e64 6963 6573  > print('Indices
+00015870: 206f 6274 6169 6e65 6420 6279 2073 6f72   obtained by sor
+00015880: 7469 6e67 2028 7363 6f72 6573 293a 272c  ting (scores):',
+00015890: 206e 702e 6172 6773 6f72 7428 6d6f 6465   np.argsort(mode
+000158a0: 6c2e 7072 6564 6963 7428 6461 7461 7365  l.predict(datase
+000158b0: 745b 2774 6573 7427 5d29 2929 0a20 2020  t['test']))).   
+000158c0: 2020 2020 2052 6177 2073 636f 7265 7320       Raw scores 
+000158d0: 2873 6f72 7465 6429 3a20 5b2d 312e 3033  (sorted): [-1.03
+000158e0: 3834 3631 3320 202d 302e 3436 3735 3236  84613  -0.467526
+000158f0: 3038 202d 302e 3435 3134 3938 3735 202e  08 -0.45149875 .
+00015900: 2e2e 2020 332e 3238 3937 3834 3420 2033  ..  3.2897844  3
+00015910: 2e33 3033 3433 3135 2020 332e 3332 3830  .3034315  3.3280
+00015920: 3633 3520 5d0a 2020 2020 2020 2020 496e  635 ].        In
+00015930: 6469 6365 7320 6f62 7461 696e 6564 2062  dices obtained b
+00015940: 7920 736f 7274 696e 6720 2873 636f 7265  y sorting (score
+00015950: 7329 3a20 5b20 3338 3334 2031 3836 3334  s): [ 3834 18634
+00015960: 2020 3430 3636 202e 2e2e 2020 3133 3535    4066 ...  1355
+00015970: 2031 3336 3333 2031 3039 3631 5d0a 2020   13633 10961].  
+00015980: 2020 2020 2020 3e3e 3e20 6d6f 6465 6c2e        >>> model.
+00015990: 6361 6c69 6272 6174 6528 6461 7461 7365  calibrate(datase
+000159a0: 745b 2774 6573 7427 5d2c 0a20 2020 2020  t['test'],.     
+000159b0: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
+000159c0: 2020 2020 2020 2062 6174 6368 5f73 697a         batch_siz
+000159d0: 653d 3130 3030 302c 0a20 2020 2020 2020  e=10000,.       
+000159e0: 203e 3e3e 2020 2020 2020 2020 2020 2020   >>>            
+000159f0: 2020 2020 2070 6f73 6974 6976 655f 6261       positive_ba
+00015a00: 7365 5f72 6174 653d 302e 392c 0a20 2020  se_rate=0.9,.   
+00015a10: 2020 2020 203e 3e3e 2020 2020 2020 2020       >>>        
+00015a20: 2020 2020 2020 2020 2065 706f 6368 733d           epochs=
+00015a30: 3130 3029 0a20 2020 2020 2020 203e 3e3e  100).        >>>
+00015a40: 2070 7269 6e74 2827 4361 6c69 6272 6174   print('Calibrat
+00015a50: 6564 2073 636f 7265 7320 2873 6f72 7465  ed scores (sorte
+00015a60: 6429 3a27 2c20 6e70 2e73 6f72 7428 6d6f  d):', np.sort(mo
+00015a70: 6465 6c2e 7072 6564 6963 745f 7072 6f62  del.predict_prob
+00015a80: 6128 6461 7461 7365 745b 2774 6573 7427  a(dataset['test'
+00015a90: 5d29 2929 0a20 2020 2020 2020 203e 3e3e  ]))).        >>>
+00015aa0: 2070 7269 6e74 2827 496e 6469 6365 7320   print('Indices 
+00015ab0: 6f62 7461 696e 6564 2062 7920 736f 7274  obtained by sort
+00015ac0: 696e 6720 2843 616c 6962 7261 7465 6429  ing (Calibrated)
+00015ad0: 3a27 2c20 6e70 2e61 7267 736f 7274 286d  :', np.argsort(m
+00015ae0: 6f64 656c 2e70 7265 6469 6374 5f70 726f  odel.predict_pro
+00015af0: 6261 2864 6174 6173 6574 5b27 7465 7374  ba(dataset['test
+00015b00: 275d 2929 290a 2020 2020 2020 2020 4361  ']))).        Ca
+00015b10: 6c69 6272 6174 6564 2073 636f 7265 7320  librated scores 
+00015b20: 2873 6f72 7465 6429 3a20 5b30 2e35 3535  (sorted): [0.555
+00015b30: 3337 3235 2020 302e 3535 3536 3130 3820  3725  0.5556108 
+00015b40: 2030 2e35 3536 3834 3135 2020 2e2e 2e20   0.5568415  ... 
+00015b50: 302e 3632 3131 3031 3120 2030 2e36 3233  0.6211011  0.623
+00015b60: 3832 3233 3320 302e 3632 3937 3538 3520  82233 0.6297585 
+00015b70: 5d0a 2020 2020 2020 2020 496e 6469 6365  ].        Indice
+00015b80: 7320 6f62 7461 696e 6564 2062 7920 736f  s obtained by so
+00015b90: 7274 696e 6720 2843 616c 6962 7261 7465  rting (Calibrate
+00015ba0: 6429 3a20 5b31 3435 3733 2031 3135 3737  d): [14573 11577
+00015bb0: 2020 3434 3034 202e 2e2e 2031 3738 3137    4404 ... 17817
+00015bc0: 2031 3738 3136 2020 2037 3333 5d0a 2020   17816   733].  
+00015bd0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00015be0: 2020 6966 206e 6f74 2073 656c 662e 6973    if not self.is
+00015bf0: 5f63 616c 6962 7261 7465 643a 0a20 2020  _calibrated:.   
+00015c00: 2020 2020 2020 2020 206d 7367 203d 2022           msg = "
+00015c10: 4d6f 6465 6c20 6861 7320 6e6f 7420 6265  Model has not be
+00015c20: 656e 2063 616c 6962 7261 7465 642e 205c  en calibrated. \
+00015c30: 0a20 2020 2020 2020 2020 2020 2050 6c65  .            Ple
+00015c40: 6173 6520 6361 6c6c 2060 6d6f 6465 6c2e  ase call `model.
+00015c50: 6361 6c69 6272 6174 6528 2e2e 2e29 6020  calibrate(...)` 
+00015c60: 6265 666f 7265 2070 7265 6469 6374 696e  before predictin
+00015c70: 6720 7072 6f62 6162 696c 6974 6965 732e  g probabilities.
+00015c80: 220a 0a20 2020 2020 2020 2020 2020 2072  "..            r
+00015c90: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
+00015ca0: 7228 6d73 6729 0a0a 2020 2020 2020 2020  r(msg)..        
+00015cb0: 7365 6c66 2e64 6174 615f 6861 6e64 6c65  self.data_handle
+00015cc0: 725f 7465 7374 203d 2064 6174 615f 6164  r_test = data_ad
+00015cd0: 6170 7465 722e 4461 7461 4861 6e64 6c65  apter.DataHandle
+00015ce0: 7228 0a20 2020 2020 2020 2020 2020 2078  r(.            x
+00015cf0: 2c0a 2020 2020 2020 2020 2020 2020 6261  ,.            ba
+00015d00: 7463 685f 7369 7a65 3d62 6174 6368 5f73  tch_size=batch_s
+00015d10: 697a 652c 0a20 2020 2020 2020 2020 2020  ize,.           
+00015d20: 2064 6174 6173 6574 5f74 7970 653d 2274   dataset_type="t
+00015d30: 6573 7422 2c0a 2020 2020 2020 2020 2020  est",.          
+00015d40: 2020 6570 6f63 6873 3d31 2c0a 2020 2020    epochs=1,.    
+00015d50: 2020 2020 2020 2020 7573 655f 6669 6c74          use_filt
+00015d60: 6572 3d46 616c 7365 2c0a 2020 2020 2020  er=False,.      
+00015d70: 2020 2020 2020 7573 655f 696e 6465 7865        use_indexe
+00015d80: 723d 7365 6c66 2e64 6174 615f 696e 6465  r=self.data_inde
+00015d90: 7865 722c 0a20 2020 2020 2020 2029 0a0a  xer,.        )..
+00015da0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+00015db0: 7369 6e73 7461 6e63 6528 6361 6c6c 6261  sinstance(callba
+00015dc0: 636b 732c 2063 616c 6c62 6163 6b73 5f6d  cks, callbacks_m
+00015dd0: 6f64 756c 652e 4361 6c6c 6261 636b 4c69  odule.CallbackLi
+00015de0: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
+00015df0: 2063 616c 6c62 6163 6b73 203d 2063 616c   callbacks = cal
+00015e00: 6c62 6163 6b73 5f6d 6f64 756c 652e 4361  lbacks_module.Ca
+00015e10: 6c6c 6261 636b 4c69 7374 280a 2020 2020  llbackList(.    
+00015e20: 2020 2020 2020 2020 2020 2020 6361 6c6c              call
+00015e30: 6261 636b 732c 0a20 2020 2020 2020 2020  backs,.         
+00015e40: 2020 2020 2020 2061 6464 5f68 6973 746f         add_histo
+00015e50: 7279 3d54 7275 652c 0a20 2020 2020 2020  ry=True,.       
+00015e60: 2020 2020 2020 2020 2061 6464 5f70 726f           add_pro
+00015e70: 6762 6172 3d76 6572 626f 7365 2021 3d20  gbar=verbose != 
+00015e80: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+00015e90: 2020 206d 6f64 656c 3d73 656c 662c 0a20     model=self,. 
+00015ea0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00015eb0: 6572 626f 7365 3d76 6572 626f 7365 2c0a  erbose=verbose,.
+00015ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ed0: 6570 6f63 6873 3d31 2c0a 2020 2020 2020  epochs=1,.      
+00015ee0: 2020 2020 2020 2020 2020 7374 6570 733d            steps=
+00015ef0: 7365 6c66 2e64 6174 615f 6861 6e64 6c65  self.data_handle
+00015f00: 725f 7465 7374 2e69 6e66 6572 7265 645f  r_test.inferred_
+00015f10: 7374 6570 732c 0a20 2020 2020 2020 2020  steps,.         
+00015f20: 2020 2029 0a0a 2020 2020 2020 2020 7072     )..        pr
+00015f30: 6564 6963 745f 6675 6e63 7469 6f6e 203d  edict_function =
+00015f40: 2073 656c 662e 6d61 6b65 5f70 7265 6469   self.make_predi
+00015f50: 6374 5f66 756e 6374 696f 6e28 290a 2020  ct_function().  
+00015f60: 2020 2020 2020 6361 6c6c 6261 636b 732e        callbacks.
+00015f70: 6f6e 5f70 7265 6469 6374 5f62 6567 696e  on_predict_begin
+00015f80: 2829 0a20 2020 2020 2020 206f 7574 7075  ().        outpu
+00015f90: 7473 203d 205b 5d0a 2020 2020 2020 2020  ts = [].        
+00015fa0: 666f 7220 5f2c 2069 7465 7261 746f 7220  for _, iterator 
+00015fb0: 696e 2073 656c 662e 6461 7461 5f68 616e  in self.data_han
+00015fc0: 646c 6572 5f74 6573 742e 656e 756d 6572  dler_test.enumer
+00015fd0: 6174 655f 6570 6f63 6873 2829 3a0a 2020  ate_epochs():.  
+00015fe0: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+00015ff0: 656c 662e 6461 7461 5f68 616e 646c 6572  elf.data_handler
+00016000: 5f74 6573 742e 6361 7463 685f 7374 6f70  _test.catch_stop
+00016010: 5f69 7465 7261 7469 6f6e 2829 3a0a 2020  _iteration():.  
+00016020: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00016030: 7220 7374 6570 2069 6e20 7365 6c66 2e64  r step in self.d
+00016040: 6174 615f 6861 6e64 6c65 725f 7465 7374  ata_handler_test
+00016050: 2e73 7465 7073 2829 3a0a 2020 2020 2020  .steps():.      
+00016060: 2020 2020 2020 2020 2020 2020 2020 6361                ca
+00016070: 6c6c 6261 636b 732e 6f6e 5f70 7265 6469  llbacks.on_predi
+00016080: 6374 5f62 6174 6368 5f62 6567 696e 2873  ct_batch_begin(s
+00016090: 7465 7029 0a20 2020 2020 2020 2020 2020  tep).           
+000160a0: 2020 2020 2020 2020 2062 6174 6368 5f6f           batch_o
+000160b0: 7574 7075 7473 203d 2070 7265 6469 6374  utputs = predict
+000160c0: 5f66 756e 6374 696f 6e28 6974 6572 6174  _function(iterat
+000160d0: 6f72 290a 2020 2020 2020 2020 2020 2020  or).            
+000160e0: 2020 2020 2020 2020 7072 6f62 6173 203d          probas =
+000160f0: 2073 656c 662e 6361 6c69 6272 6174 696f   self.calibratio
+00016100: 6e5f 6c61 7965 7228 6261 7463 685f 6f75  n_layer(batch_ou
+00016110: 7470 7574 732c 2074 7261 696e 696e 673d  tputs, training=
+00016120: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
+00016130: 2020 2020 2020 206f 7574 7075 7473 2e61         outputs.a
+00016140: 7070 656e 6428 7072 6f62 6173 290a 0a20  ppend(probas).. 
+00016150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016160: 2020 2063 616c 6c62 6163 6b73 2e6f 6e5f     callbacks.on_
+00016170: 7072 6564 6963 745f 6261 7463 685f 656e  predict_batch_en
+00016180: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
+00016190: 2020 2020 2020 2020 2020 2073 7465 702c             step,
+000161a0: 207b 226f 7574 7075 7473 223a 2062 6174   {"outputs": bat
+000161b0: 6368 5f6f 7574 7075 7473 7d0a 2020 2020  ch_outputs}.    
+000161c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161d0: 290a 2020 2020 2020 2020 6361 6c6c 6261  ).        callba
+000161e0: 636b 732e 6f6e 5f70 7265 6469 6374 5f65  cks.on_predict_e
+000161f0: 6e64 2829 0a20 2020 2020 2020 2072 6574  nd().        ret
+00016200: 7572 6e20 6e70 2e63 6f6e 6361 7465 6e61  urn np.concatena
+00016210: 7465 286f 7574 7075 7473 290a 0a20 2020  te(outputs)..   
+00016220: 2064 6566 2067 6574 5f65 6d62 6564 6469   def get_embeddi
+00016230: 6e67 7328 7365 6c66 2c20 656e 7469 7469  ngs(self, entiti
+00016240: 6573 2c20 656d 6265 6464 696e 675f 7479  es, embedding_ty
+00016250: 7065 3d22 6522 293a 0a20 2020 2020 2020  pe="e"):.       
+00016260: 2022 2222 4765 7420 7468 6520 656d 6265   """Get the embe
+00016270: 6464 696e 6773 206f 6620 656e 7469 7469  ddings of entiti
+00016280: 6573 206f 7220 7265 6c61 7469 6f6e 732e  es or relations.
+00016290: 0a0a 2020 2020 2020 2020 2e2e 204e 6f74  ..        .. Not
+000162a0: 6520 3a3a 0a0a 2020 2020 2020 2020 2020  e ::..          
+000162b0: 2020 5573 6520 3a6d 6574 683a 6061 6d70    Use :meth:`amp
+000162c0: 6c69 6772 6170 682e 7574 696c 732e 6372  ligraph.utils.cr
+000162d0: 6561 7465 5f74 656e 736f 7262 6f61 7264  eate_tensorboard
+000162e0: 5f76 6973 7561 6c69 7a61 7469 6f6e 7360  _visualizations`
+000162f0: 2074 6f20 7669 7375 616c 697a 6520 7468   to visualize th
+00016300: 6520 656d 6265 6464 696e 6773 2077 6974  e embeddings wit
+00016310: 6820 5465 6e73 6f72 426f 6172 642e 0a0a  h TensorBoard...
+00016320: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00016330: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00016340: 2d2d 2d2d 2d0a 2020 2020 2020 2020 656e  -----.        en
+00016350: 7469 7469 6573 203a 2061 7272 6179 2d6c  tities : array-l
+00016360: 696b 652c 2073 6861 7065 3d28 6e29 0a20  ike, shape=(n). 
+00016370: 2020 2020 2020 2020 2020 2054 6865 2065             The e
+00016380: 6e74 6974 6965 7320 286f 7220 7265 6c61  ntities (or rela
+00016390: 7469 6f6e 7329 206f 6620 696e 7465 7265  tions) of intere
+000163a0: 7374 2e20 456c 656d 656e 7420 6f66 2074  st. Element of t
+000163b0: 6865 2076 6563 746f 7220 6d75 7374 2062  he vector must b
+000163c0: 6520 7468 6520 6f72 6967 696e 616c 2073  e the original s
+000163d0: 7472 696e 6720 6c69 7465 7261 6c73 2c20  tring literals, 
+000163e0: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
+000163f0: 6e6f 7420 696e 7465 726e 616c 2049 4473  not internal IDs
+00016400: 2e0a 2020 2020 2020 2020 656d 6265 6464  ..        embedd
+00016410: 696e 675f 7479 7065 203a 2073 7472 0a20  ing_type : str. 
+00016420: 2020 2020 2020 2020 2020 2049 6620 6027             If `'
+00016430: 6527 6020 6973 2070 6173 7365 642c 2060  e'` is passed, `
+00016440: 6065 6e74 6974 6965 7360 6020 6172 6775  `entities`` argu
+00016450: 6d65 6e74 2077 696c 6c20 6265 2063 6f6e  ment will be con
+00016460: 7369 6465 7265 6420 6173 2061 206c 6973  sidered as a lis
+00016470: 7420 6f66 206b 6e6f 776c 6564 6765 2067  t of knowledge g
+00016480: 7261 7068 2065 6e74 6974 6965 730a 2020  raph entities.  
+00016490: 2020 2020 2020 2020 2020 2869 2e65 2e2c            (i.e.,
+000164a0: 206e 6f64 6573 292e 2049 6620 7365 7420   nodes). If set 
+000164b0: 746f 2060 2772 2760 2c20 6060 656e 7469  to `'r'`, ``enti
+000164c0: 7469 6573 6060 2077 696c 6c20 6265 2074  ties`` will be t
+000164d0: 7265 6174 6564 2061 7320 7265 6c61 7469  reated as relati
+000164e0: 6f6e 7320 696e 7374 6561 642e 0a20 2020  ons instead..   
+000164f0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00016500: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00016510: 2020 2020 2065 6d62 6564 6469 6e67 7320       embeddings 
+00016520: 3a20 6e64 6172 7261 792c 2073 6861 7065  : ndarray, shape
+00016530: 2028 6e2c 206b 290a 2020 2020 2020 2020   (n, k).        
+00016540: 2020 2020 416e 2061 7272 6179 206f 6620      An array of 
+00016550: 606b 602d 6469 6d65 6e73 696f 6e61 6c20  `k`-dimensional 
+00016560: 656d 6265 6464 696e 6773 2e0a 0a20 2020  embeddings...   
+00016570: 2020 2020 2045 7861 6d70 6c65 0a20 2020       Example.   
+00016580: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00016590: 2020 2020 203e 3e3e 2066 726f 6d20 616d       >>> from am
+000165a0: 706c 6967 7261 7068 2e6c 6174 656e 745f  pligraph.latent_
+000165b0: 6665 6174 7572 6573 2069 6d70 6f72 7420  features import 
+000165c0: 5363 6f72 696e 6742 6173 6564 456d 6265  ScoringBasedEmbe
+000165d0: 6464 696e 674d 6f64 656c 0a20 2020 2020  ddingModel.     
+000165e0: 2020 203e 3e3e 2066 726f 6d20 616d 706c     >>> from ampl
+000165f0: 6967 7261 7068 2e64 6174 6173 6574 7320  igraph.datasets 
+00016600: 696d 706f 7274 206c 6f61 645f 6662 3135  import load_fb15
+00016610: 6b5f 3233 370a 2020 2020 2020 2020 3e3e  k_237.        >>
+00016620: 3e20 5820 3d20 6c6f 6164 5f66 6231 356b  > X = load_fb15k
+00016630: 5f32 3337 2829 0a20 2020 2020 2020 203e  _237().        >
+00016640: 3e3e 206d 6f64 656c 203d 2053 636f 7269  >> model = Scori
+00016650: 6e67 4261 7365 6445 6d62 6564 6469 6e67  ngBasedEmbedding
+00016660: 4d6f 6465 6c28 6574 613d 352c 0a20 2020  Model(eta=5,.   
+00016670: 2020 2020 203e 3e3e 2020 2020 2020 2020       >>>        
+00016680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016690: 2020 2020 2020 2020 2020 2020 6b3d 3330              k=30
+000166a0: 302c 0a20 2020 2020 2020 203e 3e3e 2020  0,.        >>>  
+000166b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166d0: 2020 7363 6f72 696e 675f 7479 7065 3d27    scoring_type='
+000166e0: 436f 6d70 6c45 7827 2c0a 2020 2020 2020  ComplEx',.      
+000166f0: 2020 3e3e 3e20 2020 2020 2020 2020 2020    >>>           
+00016700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016710: 2020 2020 2020 2020 2073 6565 643d 3029           seed=0)
+00016720: 0a20 2020 2020 2020 203e 3e3e 206d 6f64  .        >>> mod
+00016730: 656c 2e63 6f6d 7069 6c65 286f 7074 696d  el.compile(optim
+00016740: 697a 6572 3d27 6164 616d 272c 206c 6f73  izer='adam', los
+00016750: 733d 276e 6c6c 2729 0a20 2020 2020 2020  s='nll').       
+00016760: 203e 3e3e 206d 6f64 656c 2e66 6974 2858   >>> model.fit(X
+00016770: 5b27 7472 6169 6e27 5d2c 0a20 2020 2020  ['train'],.     
+00016780: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
+00016790: 2062 6174 6368 5f73 697a 653d 3130 3030   batch_size=1000
+000167a0: 302c 0a20 2020 2020 2020 203e 3e3e 2020  0,.        >>>  
+000167b0: 2020 2020 2020 2020 2065 706f 6368 733d           epochs=
+000167c0: 352c 0a20 2020 2020 2020 203e 3e3e 2020  5,.        >>>  
+000167d0: 2020 2020 2020 2020 2076 6572 626f 7365           verbose
+000167e0: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+000167f0: 3e3e 3e20 6d6f 6465 6c2e 6765 745f 656d  >>> model.get_em
+00016800: 6265 6464 696e 6773 285b 272f 6d2f 3032  beddings(['/m/02
+00016810: 3772 6e27 2c20 272f 6d2f 3036 7638 7330  7rn', '/m/06v8s0
+00016820: 275d 2c20 2765 2729 0a20 2020 2020 2020  '], 'e').       
+00016830: 2061 7272 6179 285b 5b20 302e 3034 3438   array([[ 0.0448
+00016840: 3234 3936 2020 302e 3131 3937 3339 3037  2496  0.11973907
+00016850: 2020 302e 3031 3131 3737 3333 202e 2e2e    0.01117733 ...
+00016860: 202d 302e 3133 3339 3139 3232 2020 302e   -0.13391922  0.
+00016870: 3131 3130 3335 3533 2020 2d30 2e30 3831  11103553  -0.081
+00016880: 3332 3836 315d 0a20 2020 2020 2020 2020  32861].         
+00016890: 5b2d 302e 3130 3135 3833 3831 2020 302e  [-0.10158381  0.
+000168a0: 3038 3130 3836 3035 202d 302e 3037 3630  08108605 -0.0760
+000168b0: 3836 3736 202e 2e2e 2020 302e 3035 3931  8676 ...  0.0591
+000168c0: 3430 3720 2030 2e30 3237 3931 3432 3620  407  0.02791426 
+000168d0: 2030 2e30 3735 3539 3031 365d 5d2c 2064   0.07559016]], d
+000168e0: 7479 7065 3d66 6c6f 6174 3332 290a 2020  type=float32).  
+000168f0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00016900: 2020 2069 6620 656d 6265 6464 696e 675f     if embedding_
+00016910: 7479 7065 203d 3d20 2265 223a 0a20 2020  type == "e":.   
+00016920: 2020 2020 2020 2020 206c 6f6f 6b75 705f           lookup_
+00016930: 636f 6e63 6570 7420 3d20 7365 6c66 2e64  concept = self.d
+00016940: 6174 615f 696e 6465 7865 722e 6765 745f  ata_indexer.get_
+00016950: 696e 6465 7865 7328 656e 7469 7469 6573  indexes(entities
+00016960: 2c20 2265 2229 0a20 2020 2020 2020 2020  , "e").         
+00016970: 2020 2069 6620 7365 6c66 2e69 735f 7061     if self.is_pa
+00016980: 7274 6974 696f 6e65 645f 7472 6169 6e69  rtitioned_traini
+00016990: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+000169a0: 2020 2020 656d 625f 6f75 7420 3d20 5b5d      emb_out = []
+000169b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000169c0: 2077 6974 6820 7368 656c 7665 2e6f 7065   with shelve.ope
+000169d0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+000169e0: 2020 2020 2020 2073 656c 662e 7061 7274         self.part
+000169f0: 6974 696f 6e65 725f 6d65 7461 6461 7461  itioner_metadata
+00016a00: 5b22 656e 745f 6d61 705f 666e 616d 6522  ["ent_map_fname"
+00016a10: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00016a20: 2020 2920 6173 2065 6e74 5f65 6d62 3a0a    ) as ent_emb:.
+00016a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a40: 2020 2020 666f 7220 656e 745f 6964 2069      for ent_id i
+00016a50: 6e20 6c6f 6f6b 7570 5f63 6f6e 6365 7074  n lookup_concept
+00016a60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016a70: 2020 2020 2020 2020 2020 656d 625f 6f75            emb_ou
+00016a80: 742e 6170 7065 6e64 2865 6e74 5f65 6d62  t.append(ent_emb
+00016a90: 5b73 7472 2865 6e74 5f69 6429 5d29 0a20  [str(ent_id)]). 
+00016aa0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00016ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016ac0: 2072 6574 7572 6e20 7466 2e6e 6e2e 656d   return tf.nn.em
+00016ad0: 6265 6464 696e 675f 6c6f 6f6b 7570 280a  bedding_lookup(.
+00016ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016af0: 2020 2020 7365 6c66 2e65 6e63 6f64 696e      self.encodin
+00016b00: 675f 6c61 7965 722e 656e 745f 656d 622c  g_layer.ent_emb,
+00016b10: 206c 6f6f 6b75 705f 636f 6e63 6570 740a   lookup_concept.
+00016b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b30: 292e 6e75 6d70 7928 290a 2020 2020 2020  ).numpy().      
+00016b40: 2020 656c 6966 2065 6d62 6564 6469 6e67    elif embedding
+00016b50: 5f74 7970 6520 3d3d 2022 7222 3a0a 2020  _type == "r":.  
+00016b60: 2020 2020 2020 2020 2020 6c6f 6f6b 7570            lookup
+00016b70: 5f63 6f6e 6365 7074 203d 2073 656c 662e  _concept = self.
+00016b80: 6461 7461 5f69 6e64 6578 6572 2e67 6574  data_indexer.get
+00016b90: 5f69 6e64 6578 6573 2865 6e74 6974 6965  _indexes(entitie
+00016ba0: 732c 2022 7222 290a 2020 2020 2020 2020  s, "r").        
+00016bb0: 2020 2020 6966 2073 656c 662e 6973 5f70      if self.is_p
+00016bc0: 6172 7469 7469 6f6e 6564 5f74 7261 696e  artitioned_train
+00016bd0: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
+00016be0: 2020 2020 2065 6d62 5f6f 7574 203d 205b       emb_out = [
+00016bf0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00016c00: 2020 7769 7468 2073 6865 6c76 652e 6f70    with shelve.op
+00016c10: 656e 280a 2020 2020 2020 2020 2020 2020  en(.            
+00016c20: 2020 2020 2020 2020 7365 6c66 2e70 6172          self.par
+00016c30: 7469 7469 6f6e 6572 5f6d 6574 6164 6174  titioner_metadat
+00016c40: 615b 2272 656c 5f6d 6170 5f66 6e61 6d65  a["rel_map_fname
+00016c50: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00016c60: 2020 2029 2061 7320 7265 6c5f 656d 623a     ) as rel_emb:
+00016c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016c80: 2020 2020 2066 6f72 2072 656c 5f69 6420       for rel_id 
+00016c90: 696e 206c 6f6f 6b75 705f 636f 6e63 6570  in lookup_concep
+00016ca0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00016cb0: 2020 2020 2020 2020 2020 2065 6d62 5f6f             emb_o
+00016cc0: 7574 2e61 7070 656e 6428 7265 6c5f 656d  ut.append(rel_em
+00016cd0: 625b 7374 7228 7265 6c5f 6964 295d 290a  b[str(rel_id)]).
+00016ce0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00016cf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016d00: 2020 7265 7475 726e 2074 662e 6e6e 2e65    return tf.nn.e
+00016d10: 6d62 6564 6469 6e67 5f6c 6f6f 6b75 7028  mbedding_lookup(
+00016d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016d30: 2020 2020 2073 656c 662e 656e 636f 6469       self.encodi
+00016d40: 6e67 5f6c 6179 6572 2e72 656c 5f65 6d62  ng_layer.rel_emb
+00016d50: 2c20 6c6f 6f6b 7570 5f63 6f6e 6365 7074  , lookup_concept
+00016d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016d70: 2029 2e6e 756d 7079 2829 0a20 2020 2020   ).numpy().     
+00016d80: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00016d90: 2020 2020 206d 7367 203d 2022 496e 7661       msg = "Inva
+00016da0: 6c69 6420 656e 7469 7479 2074 7970 653a  lid entity type:
+00016db0: 207b 7d22 2e66 6f72 6d61 7428 656d 6265   {}".format(embe
+00016dc0: 6464 696e 675f 7479 7065 290a 2020 2020  dding_type).    
+00016dd0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00016de0: 6c75 6545 7272 6f72 286d 7367 290a       lueError(msg).
```

## ampligraph/utils/model_utils.py

```diff
@@ -22,15 +22,15 @@
 
 DEFAULT_MODEL_NAMES = "{0}.model.pkl"
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
-def save_model(model, model_name_path=None):
+def save_model(model, model_name_path=None, protocol=pickle.HIGHEST_PROTOCOL):
     """Save a trained model to disk.
 
     Example
     -------
     >>> import numpy as np
     >>> from ampligraph.latent_features import ComplEx
     >>> from ampligraph.utils import save_model
@@ -57,17 +57,14 @@
         The model must be an instance of TransE, DistMult, ComplEx, or HolE.
     model_name_path: str
         The name of the model to be saved.
         If not specified, a default name with current datetime is selected and the model is saved
         to the working directory.
 
     """
-    model.data_shape = tf.Variable(
-        model.data_shape, trainable=False
-    )  # Redefine the attribute for saving it
     if model_name_path is None:
         model_name_path = "{0}".format(strftime("%Y_%m_%d-%H_%M_%S", gmtime()))
     if os.path.exists(model_name_path):
         print(
             "The path {} already exists. This save operation will overwrite the model \
                 at the specified path.".format(
                 model_name_path
```

## tests/ampligraph/datasets/test_datasets.py

```diff
@@ -4,14 +4,15 @@
 # A copy of the Licence is available in LICENCE, or at:
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 from ampligraph.datasets import load_wn18, load_fb15k, load_fb15k_237, load_yago3_10, load_wn18rr, load_wn11, \
     load_fb13
 from ampligraph.datasets.datasets import _clean_data
+import os
 import numpy as np
 import pytest
 
 
 def test_clean_data():
     X = {
         'train': np.array([['a', 'b', 'c'], ['d', 'e', 'f'], ['g', 'h', 'i'], ['j', 'k', 'l']]),
```

## Comparing `ampligraph-2.0.0.dist-info/LICENSE` & `ampligraph-2.0.1.dist-info/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2019 The AmpliGraph Authors
+   Copyright 2019-2020 The AmpliGraph Authors
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

## Comparing `ampligraph-2.0.0.dist-info/METADATA` & `ampligraph-2.0.1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: ampligraph
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Python library for relational learning on knowledge graphs.
 Home-page: https://github.com/Accenture/AmpliGraph/
 Author: Accenture Dublin Labs
 Author-email: about@ampligraph.org
 License: Apache 2.0
 License-File: LICENSE
 Requires-Dist: numpy (>=1.14.3)
 Requires-Dist: pytest (>=3.5.1)
 Requires-Dist: scikit-learn (>=0.19.1)
-Requires-Dist: deap (>=1.2.2)
-Requires-Dist: joblib (>=0.11)
 Requires-Dist: tqdm (>=4.23.4)
 Requires-Dist: pandas (>=0.23.1)
 Requires-Dist: sphinx (==5.0.2)
 Requires-Dist: myst-parser (==0.18.0)
 Requires-Dist: docutils (<0.18)
 Requires-Dist: sphinx-rtd-theme (==1.0.0)
 Requires-Dist: sphinxcontrib-bibtex (==2.4.2)
 Requires-Dist: beautifultable (>=0.7.0)
 Requires-Dist: pyyaml (>=3.13)
 Requires-Dist: rdflib (>=4.2.2)
-Requires-Dist: scipy (>=1.10.0)
+Requires-Dist: scipy (==1.10.0)
 Requires-Dist: networkx (>=2.3)
 Requires-Dist: flake8 (>=3.7.7)
 Requires-Dist: setuptools (>=36)
 Requires-Dist: matplotlib (>=3.7)
 Requires-Dist: docopt (==0.6.2)
 Requires-Dist: schema (==0.7.5)
```

## Comparing `ampligraph-2.0.0.dist-info/RECORD` & `ampligraph-2.0.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,57 @@
-ampligraph/__init__.py,sha256=II_5gwtek4NUxbg3gX2LLQGYcA681nkbXiLfqKpudlk,679
+ampligraph/__init__.py,sha256=xYeKv-uynYGG9rSxGCYhTk3L14eGWSPikp0BrHYioeU,679
 ampligraph/logger.conf,sha256=-LrMUFmCdzKL8qPDUe4OXKnZ7AfAzKi8Oam6dqFHgWk,506
 ampligraph/compat/__init__.py,sha256=F53YefkssfYI2NnNigeHghboIsvtdTETaqUmO5LLDxw,473
 ampligraph/compat/evaluate.py,sha256=_HmOp2tE1JgtKIcrbiVtbCfcaQz6s9dpKxSYeqhoBVc,7534
 ampligraph/compat/models.py,sha256=rOyf1A0_LRLBMMnJ2KZ1uZGh0AnZCuf-0ETZwcu6aag,29377
 ampligraph/datasets/__init__.py,sha256=IjIIfhilIIQjZJIJn9sUl-7Ln_SRsAPtkpVVqLH2h18,1533
 ampligraph/datasets/data_adapter.py,sha256=x3d-9AMWhOIp-HEeOeG25h1RypZzPtjRQVbR9VEtflI,4961
-ampligraph/datasets/data_indexer.py,sha256=DS5YdbieFXp2XV8p9xMitWUjpMIpmENt_SEiD7i6pTU,64485
-ampligraph/datasets/datasets.py,sha256=fnWchJGOqpfysnz60Iw1gRzRb_xB2i5czjg6XzZhUPg,74774
-ampligraph/datasets/graph_data_loader.py,sha256=nES3i0UpvhsyCTJ-gWmLTfpLKHKRIgtmqXjH9ZMh2w4,35488
+ampligraph/datasets/data_indexer.py,sha256=J3Al2Znxg62MdfaVjBvHXsGjynFdBO2g_RCHFVPmrdc,64717
+ampligraph/datasets/datasets.py,sha256=68AAAAFu0dZeFS0ZKAKcWJ_ae5vEc5eATtEI-ch_vQo,74882
+ampligraph/datasets/graph_data_loader.py,sha256=zg1-9pAGM2NhCvhLV9uj95VhIpgtBmdcBMzsoB-_Zg8,35727
 ampligraph/datasets/graph_partitioner.py,sha256=0N1TL_-vYT9xk12Ua22zdRKqf_CByG4d21yosSIlRsY,32263
 ampligraph/datasets/partitioned_data_manager.py,sha256=4N3DnsXVOHbM9J5oZAcaCc36hRfQZFY9CUnj8IOelOc,38764
 ampligraph/datasets/partitioning_reporter.py,sha256=gsHzVp9LgkxTVKjnMDclLtU4G5xx3SuWR4Ce5F4ZMfo,15810
 ampligraph/datasets/source_identifier.py,sha256=tVHFF1ZL7j9z3nR2I2I8wPu0_HWELu4KxnK2IZ3RNSI,5677
 ampligraph/datasets/sqlite_adapter.py,sha256=9xsp42zkXUEl8JHBnvOI2bpWRcadPEC4Zmvio13wOy8,34921
-ampligraph/discovery/__init__.py,sha256=ftnrLDv8F-RbDoGql95zgDRBTk1GMvEd5z44Fqo3i2c,1057
-ampligraph/discovery/discovery.py,sha256=2m7vIKrOTUUdsaxFvYHegSxv88EyZnGQIYCwSEiM9n0,45346
+ampligraph/discovery/__init__.py,sha256=eW7zUoAU-may741tEaI94WKkBVCjcAaEVUuYYp-0ER4,1112
+ampligraph/discovery/discovery.py,sha256=6d-MCM8lLziBxlEwfYdHHEEtSWopewZ6hJjkiVu1r-I,49019
 ampligraph/evaluation/__init__.py,sha256=0Spsm9clSeX-Xq4yf3EPOE1RkqTH7YcQOe8NaUk-ggA,848
-ampligraph/evaluation/metrics.py,sha256=ZaJ9AX9av5QjhIZ2KgMbeWj11pQc1x2SHqCtDG-InrA,7823
-ampligraph/evaluation/protocol.py,sha256=Xum9oeM_vU-uHqA6hTh8k24Y3avUfs8ZUDr8n5ef2Bs,31224
+ampligraph/evaluation/metrics.py,sha256=IKPz3JMDqri5ds6Jwf3ISnvb1qRPDngPEy3lMiiSXVk,7883
+ampligraph/evaluation/protocol.py,sha256=oMQcNkCKUvNXKUeiHEHXUlQU4rMRVp5p-W1W2gr-0O4,31276
 ampligraph/latent_features/__init__.py,sha256=t6PWTeb_1nI-hk2hil1vlCJ6h9DskBGzUyTSiF5p-0w,1172
 ampligraph/latent_features/loss_functions.py,sha256=UPf06nfyOiHfkj7iXgOSbMBOC2EWmiK9NDPSQwxffJM,24974
 ampligraph/latent_features/optimizers.py,sha256=ZSlwdSN-d9hMP2_V86XL-OQVpmJx0blni9ocpiHfJnM,7263
 ampligraph/latent_features/regularizers.py,sha256=FmlOPDDLRdN2uSfqM8eW1Zqm9gfwfcr_Ital7DJ4NBo,2295
 ampligraph/latent_features/layers/__init__.py,sha256=sog31Ous7e8qXkT2dkhn_ReREgj4qwW8TH1SoEq0_rs,315
 ampligraph/latent_features/layers/calibration/__init__.py,sha256=C48DyoxgokyqKZzdbit4PMUwfY9basTEh7W2tlHeihE,313
-ampligraph/latent_features/layers/calibration/calibrate.py,sha256=1GkbHtoWK2DYez3ItuPWAbGcWT1cQRz7W8aghmpx9Ls,4151
+ampligraph/latent_features/layers/calibration/calibrate.py,sha256=OeMN-nuE9Suoeqen3YLCy5bdU9Ha1EMN8vr5ySxxEs0,4064
 ampligraph/latent_features/layers/corruption_generation/CorruptionGenerationLayerTrain.py,sha256=QfYg32H9RUcFGJgQHsdtH0jnfIsVOxPDAaotLUmsumk,3474
 ampligraph/latent_features/layers/corruption_generation/__init__.py,sha256=KuFDFYuZ_bWfAr7lMi7ZIKDaShut2MQ7rOLmF9Da0VQ,362
-ampligraph/latent_features/layers/encoding/EmbeddingLookupLayer.py,sha256=dS2LOKIQuCUrFisrkNBbIHyfRZSV-zC2tpzBGxJsQ_4,12594
+ampligraph/latent_features/layers/encoding/EmbeddingLookupLayer.py,sha256=PGczQcvigWyhRI2Spfj5sH71hFAECDD3VGHxwZInbx4,13633
 ampligraph/latent_features/layers/encoding/__init__.py,sha256=a8KOkIAOJOmnUWK1DUJbF0Zx_O0shXNt1Qw6gZldTNQ,332
 ampligraph/latent_features/layers/scoring/AbstractScoringLayer.py,sha256=tN_pC25kZlmZDpKL_GwXMTbtIj52Wc0fu8Ip1OS-qYk,16689
 ampligraph/latent_features/layers/scoring/ComplEx.py,sha256=BdPfj5fF9bfrRgmcX7plvPujsWuBTI4BtcJB3_I6Jnw,5339
 ampligraph/latent_features/layers/scoring/DistMult.py,sha256=lurGiPnzbmBCOC8BE3OZdzsUi5uUd0Iz523ZbqaslIA,3413
 ampligraph/latent_features/layers/scoring/HolE.py,sha256=bm2RCq2UCO9JWK7iZn9zqkaZkGZL17TTK25f8tLAL00,2784
 ampligraph/latent_features/layers/scoring/Random.py,sha256=Pz-TSaolkf9t8Fl0tpFA3gllR5w8ZQGA0oKqwG8yIus,2510
+ampligraph/latent_features/layers/scoring/RotatE.py,sha256=X1pKNwhwD9hktmKFv7qZqKx1qbs-IgOsbXozMRa13vE,6275
 ampligraph/latent_features/layers/scoring/TransE.py,sha256=oI97Oi3ByRZj7s9BLkhH4BCmLK1BHWuDfBnLsE8kOzc,3969
 ampligraph/latent_features/layers/scoring/__init__.py,sha256=nNwkG_RKWLKQs_sBn-uE6j7bJS2LTsm1FaUnHNzyqbk,441
-ampligraph/latent_features/models/ScoringBasedEmbeddingModel.py,sha256=ywCazCnStY7ptxdYIxV-WZIh4Ia1gh_fpF92Zj7sWjc,93355
+ampligraph/latent_features/models/NodePiece.py,sha256=BytGieyoJVWsb47lphYhdEreL6pB3t0UaXKvbRlptsA,99848
+ampligraph/latent_features/models/ScoringBasedEmbeddingModel.py,sha256=nvNOt1XQ7EjCmgGSNQMbN9sCdhFVOlGCywgLKdNW1bE,93678
 ampligraph/latent_features/models/__init__.py,sha256=wqUWMuow3cpb5ROK0px8c17UgPWMFqM6aNz65OQBWHM,350
 ampligraph/utils/__init__.py,sha256=PbMD-CI3LTS0a9ZMawD0PrxGvgoDZdda1ZwEmtkhkVA,703
-ampligraph/utils/model_utils.py,sha256=-TqxBffrxLljGKVqDVdkVLBlif8g107L-FCmG2y07Xg,15606
+ampligraph/utils/model_utils.py,sha256=Qq-ozuQNq7BkXytK2Ylsmt0pdEfJph9kogRCXMYckBU,15516
 ampligraph/utils/profiling.py,sha256=perb51Qp1rAY19tv4z3cMS-XtMx1ef9e3iebSqE5qLc,2841
 ampligraph/utils/tags.py,sha256=8E24eh8gLdw5sZT2s4240oq51kZhG0jMbdo48ghSGIg,2298
 tests/ampligraph/__init__.py,sha256=exjjGWt9bngN2x1McryHhW5tWpuKM45CdTjQ-zRo4aI,241
 tests/ampligraph/datasets/__init__.py,sha256=exjjGWt9bngN2x1McryHhW5tWpuKM45CdTjQ-zRo4aI,241
 tests/ampligraph/datasets/test_data_indexer.py,sha256=XNvtN4p4MgVCA2Y64vt5ybDLRJ0BjqDST-jq5HouM8U,2935
-tests/ampligraph/datasets/test_datasets.py,sha256=Wq8qtBBFiJvwtXwuJZq1cGdZHNa48x9kLwBEFJjWClg,7161
+tests/ampligraph/datasets/test_datasets.py,sha256=YmCoJgAqLSeMiD5EqpxmDzEF1honc6ERbKENYFmxiQs,7171
 tests/ampligraph/datasets/test_graph_data_loader.py,sha256=syX02Nj6LYxSRQaxhCTjN0YwOoE7EXJH0QJ37BC-L1s,4585
 tests/ampligraph/datasets/test_graph_partitioner.py,sha256=WFIQ0XKTv7_tXOXBlxZ1JmJ_gZ9wUFI76cDQsSD412Q,8582
 tests/ampligraph/datasets/test_partitioning_reporter.py,sha256=wZJG_RIV2orGjM5g2HYhwPQ-QTsBU4eBu0q-AETmBZs,4936
 tests/ampligraph/datasets/test_source_identifier.py,sha256=dCjP0YEperjeP2P0ImJCFF51W2IUXEr313OQTVNxN_k,2430
 tests/ampligraph/datasets/test_sqlite_adapter.py,sha256=dgxvWlB3Zx6F0t60fqT0cLvN-VeftEezRsiBP8Da4DY,1368
 tests/ampligraph/discovery/__init__.py,sha256=uw4c8xBEZOZ-peF1WUqXttae3CWVbQYyFn4lty_Zn_M,240
 tests/ampligraph/discovery/test_discovery.py,sha256=iFN63HbtkcgvBbJD6zOr2LeCwuULOVaVTaPEYRHhBTE,12382
@@ -58,12 +60,12 @@
 tests/ampligraph/latent_features/__init__.py,sha256=uw4c8xBEZOZ-peF1WUqXttae3CWVbQYyFn4lty_Zn_M,240
 tests/ampligraph/latent_features/test_initializers.py,sha256=UsYHwad_najmFCpDBRCDasXm3FX83n3MgTqIEfNyZHE,2121
 tests/ampligraph/latent_features/test_loss_functions.py,sha256=zal98tvy5nakEhoH0ddUIc1-pMyqfGWtmGfE_x25M7g,8632
 tests/ampligraph/latent_features/test_optimizers.py,sha256=zYc_hG6Zyrj_qbUgO-VoS9PgGnDsDVLV2RKRyOZP5yM,3198
 tests/ampligraph/latent_features/test_regularizer.py,sha256=_pCudEOmv7cQpMmkqcSNzgme-yC4-WWRyVfIDaXtMqk,1519
 tests/ampligraph/utils/__init__.py,sha256=eKUcwG9jGh2USSGEUVAnmUv00N_rSP8q8mouM9xwBTw,242
 tests/ampligraph/utils/test_profiling.py,sha256=E8kaQUrB-q1f3Oi6Z6DnDKnzx5U8F62-9sFOAgbb4LI,1257
-ampligraph-2.0.0.dist-info/LICENSE,sha256=c5Az_pipHa_NltQlJladYGXsZOTz8tky6jLA_NAmgJA,11351
-ampligraph-2.0.0.dist-info/METADATA,sha256=lyxCPkj7HypVj0TSH1Mo7VTc6vRAXbTEGFqJkDiqzfs,1033
-ampligraph-2.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-ampligraph-2.0.0.dist-info/top_level.txt,sha256=qp3q59ucJOin6yD2C9JlRtCDMv47pZKNUIrKbwTPCl8,17
-ampligraph-2.0.0.dist-info/RECORD,,
+ampligraph-2.0.1.dist-info/LICENSE,sha256=F95KC9ZpaGJjPAzKl25_LIFsL6YFgwJdG3NYZhFKoso,11356
+ampligraph-2.0.1.dist-info/METADATA,sha256=uJ1xl8g4QDr4SU_VWCBmHLixXysK-YKLkWP9kQRZif4,972
+ampligraph-2.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+ampligraph-2.0.1.dist-info/top_level.txt,sha256=qp3q59ucJOin6yD2C9JlRtCDMv47pZKNUIrKbwTPCl8,17
+ampligraph-2.0.1.dist-info/RECORD,,
```


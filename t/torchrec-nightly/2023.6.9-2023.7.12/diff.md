# Comparing `tmp/torchrec_nightly-2023.6.9-py39-none-any.whl.zip` & `tmp/torchrec_nightly-2023.7.12-3.9-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,145 +1,197 @@
-Zip file size: 353905 bytes, number of entries: 143
--rw-r--r--  2.0 unx      811 b- defN 23-Jun-09 11:18 torchrec/__init__.py
--rw-r--r--  2.0 unx     1638 b- defN 23-Jun-09 11:18 torchrec/streamable.py
--rw-r--r--  2.0 unx      854 b- defN 23-Jun-09 11:18 torchrec/types.py
--rw-r--r--  2.0 unx     1153 b- defN 23-Jun-09 11:18 torchrec/datasets/__init__.py
--rw-r--r--  2.0 unx    41469 b- defN 23-Jun-09 11:18 torchrec/datasets/criteo.py
--rw-r--r--  2.0 unx     4548 b- defN 23-Jun-09 11:18 torchrec/datasets/movielens.py
--rw-r--r--  2.0 unx     6539 b- defN 23-Jun-09 11:18 torchrec/datasets/random.py
--rw-r--r--  2.0 unx    10909 b- defN 23-Jun-09 11:18 torchrec/datasets/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 11:18 torchrec/datasets/scripts/__init__.py
--rw-r--r--  2.0 unx     2448 b- defN 23-Jun-09 11:18 torchrec/datasets/scripts/contiguous_preproc_criteo.py
--rw-r--r--  2.0 unx     2847 b- defN 23-Jun-09 11:18 torchrec/datasets/scripts/npy_preproc_criteo.py
--rw-r--r--  2.0 unx     3077 b- defN 23-Jun-09 11:18 torchrec/datasets/scripts/shuffle_preproc_criteo.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 11:18 torchrec/datasets/test_utils/__init__.py
--rw-r--r--  2.0 unx     5308 b- defN 23-Jun-09 11:18 torchrec/datasets/test_utils/criteo_test_utils.py
--rw-r--r--  2.0 unx     1912 b- defN 23-Jun-09 11:18 torchrec/distributed/__init__.py
--rw-r--r--  2.0 unx    37411 b- defN 23-Jun-09 11:18 torchrec/distributed/batched_embedding_kernel.py
--rw-r--r--  2.0 unx     2069 b- defN 23-Jun-09 11:18 torchrec/distributed/collective_utils.py
--rw-r--r--  2.0 unx     4988 b- defN 23-Jun-09 11:18 torchrec/distributed/comm.py
--rw-r--r--  2.0 unx    55918 b- defN 23-Jun-09 11:18 torchrec/distributed/comm_ops.py
--rw-r--r--  2.0 unx    35580 b- defN 23-Jun-09 11:18 torchrec/distributed/dist_data.py
--rw-r--r--  2.0 unx    32013 b- defN 23-Jun-09 11:18 torchrec/distributed/embedding.py
--rw-r--r--  2.0 unx     4947 b- defN 23-Jun-09 11:18 torchrec/distributed/embedding_kernel.py
--rw-r--r--  2.0 unx    29176 b- defN 23-Jun-09 11:18 torchrec/distributed/embedding_lookup.py
--rw-r--r--  2.0 unx    20599 b- defN 23-Jun-09 11:18 torchrec/distributed/embedding_sharding.py
--rw-r--r--  2.0 unx    37089 b- defN 23-Jun-09 11:18 torchrec/distributed/embedding_tower_sharding.py
--rw-r--r--  2.0 unx    15030 b- defN 23-Jun-09 11:18 torchrec/distributed/embedding_types.py
--rw-r--r--  2.0 unx    35218 b- defN 23-Jun-09 11:18 torchrec/distributed/embeddingbag.py
--rw-r--r--  2.0 unx     7373 b- defN 23-Jun-09 11:18 torchrec/distributed/fbgemm_qcomm_codec.py
--rw-r--r--  2.0 unx     6137 b- defN 23-Jun-09 11:18 torchrec/distributed/fp_embeddingbag.py
--rw-r--r--  2.0 unx     5243 b- defN 23-Jun-09 11:18 torchrec/distributed/fused_embedding.py
--rw-r--r--  2.0 unx     5110 b- defN 23-Jun-09 11:18 torchrec/distributed/fused_embeddingbag.py
--rw-r--r--  2.0 unx     2271 b- defN 23-Jun-09 11:18 torchrec/distributed/fused_params.py
--rw-r--r--  2.0 unx     3807 b- defN 23-Jun-09 11:18 torchrec/distributed/grouped_position_weighted.py
--rw-r--r--  2.0 unx    19786 b- defN 23-Jun-09 11:18 torchrec/distributed/model_parallel.py
--rw-r--r--  2.0 unx    14686 b- defN 23-Jun-09 11:18 torchrec/distributed/quant_embedding.py
--rw-r--r--  2.0 unx    14976 b- defN 23-Jun-09 11:18 torchrec/distributed/quant_embedding_kernel.py
--rw-r--r--  2.0 unx    11770 b- defN 23-Jun-09 11:18 torchrec/distributed/quant_embeddingbag.py
--rw-r--r--  2.0 unx     9261 b- defN 23-Jun-09 11:18 torchrec/distributed/shard.py
--rw-r--r--  2.0 unx    19411 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding_plan.py
--rw-r--r--  2.0 unx    36724 b- defN 23-Jun-09 11:18 torchrec/distributed/train_pipeline.py
--rw-r--r--  2.0 unx    24927 b- defN 23-Jun-09 11:18 torchrec/distributed/types.py
--rw-r--r--  2.0 unx    11873 b- defN 23-Jun-09 11:18 torchrec/distributed/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 11:18 torchrec/distributed/composable/__init__.py
--rw-r--r--  2.0 unx     3207 b- defN 23-Jun-09 11:18 torchrec/distributed/composable/table_batched_embedding_slice.py
--rw-r--r--  2.0 unx     1025 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/__init__.py
--rw-r--r--  2.0 unx     3135 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/constants.py
--rw-r--r--  2.0 unx    10318 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/enumerators.py
--rw-r--r--  2.0 unx    12642 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/partitioners.py
--rw-r--r--  2.0 unx      835 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/perf_models.py
--rw-r--r--  2.0 unx    13288 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/planners.py
--rw-r--r--  2.0 unx    11236 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/proposers.py
--rw-r--r--  2.0 unx    40395 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/shard_estimators.py
--rw-r--r--  2.0 unx    23617 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/stats.py
--rw-r--r--  2.0 unx     9125 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/storage_reservations.py
--rw-r--r--  2.0 unx    13899 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/types.py
--rw-r--r--  2.0 unx     1119 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/__init__.py
--rw-r--r--  2.0 unx     2539 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/cw_sequence_sharding.py
--rw-r--r--  2.0 unx     9519 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/cw_sharding.py
--rw-r--r--  2.0 unx     2802 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/dp_sequence_sharding.py
--rw-r--r--  2.0 unx     7681 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/dp_sharding.py
--rw-r--r--  2.0 unx     5041 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/rw_sequence_sharding.py
--rw-r--r--  2.0 unx    12850 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/rw_sharding.py
--rw-r--r--  2.0 unx     3114 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/sequence_sharding.py
--rw-r--r--  2.0 unx     7692 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/tw_sequence_sharding.py
--rw-r--r--  2.0 unx    16315 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/tw_sharding.py
--rw-r--r--  2.0 unx     1284 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/twcw_sharding.py
--rw-r--r--  2.0 unx    19898 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/twrw_sharding.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 11:18 torchrec/distributed/test_utils/__init__.py
--rw-r--r--  2.0 unx    10453 b- defN 23-Jun-09 11:18 torchrec/distributed/test_utils/infer_utils.py
--rw-r--r--  2.0 unx     4868 b- defN 23-Jun-09 11:18 torchrec/distributed/test_utils/multi_process.py
--rw-r--r--  2.0 unx    34246 b- defN 23-Jun-09 11:18 torchrec/distributed/test_utils/test_model.py
--rw-r--r--  2.0 unx    11193 b- defN 23-Jun-09 11:18 torchrec/distributed/test_utils/test_model_parallel.py
--rw-r--r--  2.0 unx    25308 b- defN 23-Jun-09 11:18 torchrec/distributed/test_utils/test_model_parallel_base.py
--rw-r--r--  2.0 unx    15367 b- defN 23-Jun-09 11:18 torchrec/distributed/test_utils/test_sharding.py
--rw-r--r--  2.0 unx      422 b- defN 23-Jun-09 11:18 torchrec/fx/__init__.py
--rw-r--r--  2.0 unx     6477 b- defN 23-Jun-09 11:18 torchrec/fx/tracer.py
--rw-r--r--  2.0 unx     4401 b- defN 23-Jun-09 11:18 torchrec/fx/utils.py
--rw-r--r--  2.0 unx     1223 b- defN 23-Jun-09 11:18 torchrec/inference/__init__.py
--rw-r--r--  2.0 unx     3614 b- defN 23-Jun-09 11:18 torchrec/inference/client.py
--rw-r--r--  2.0 unx     3957 b- defN 23-Jun-09 11:18 torchrec/inference/model_packager.py
--rw-r--r--  2.0 unx     8068 b- defN 23-Jun-09 11:18 torchrec/inference/modules.py
--rw-r--r--  2.0 unx     3797 b- defN 23-Jun-09 11:18 torchrec/inference/state_dict_transform.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 11:18 torchrec/metrics/__init__.py
--rw-r--r--  2.0 unx     4168 b- defN 23-Jun-09 11:18 torchrec/metrics/accuracy.py
--rw-r--r--  2.0 unx    12549 b- defN 23-Jun-09 11:18 torchrec/metrics/auc.py
--rw-r--r--  2.0 unx     3703 b- defN 23-Jun-09 11:18 torchrec/metrics/calibration.py
--rw-r--r--  2.0 unx     3465 b- defN 23-Jun-09 11:18 torchrec/metrics/ctr.py
--rw-r--r--  2.0 unx     3836 b- defN 23-Jun-09 11:18 torchrec/metrics/mae.py
--rw-r--r--  2.0 unx    17909 b- defN 23-Jun-09 11:18 torchrec/metrics/metric_module.py
--rw-r--r--  2.0 unx     6778 b- defN 23-Jun-09 11:18 torchrec/metrics/metrics_config.py
--rw-r--r--  2.0 unx     3695 b- defN 23-Jun-09 11:18 torchrec/metrics/metrics_namespace.py
--rw-r--r--  2.0 unx     3904 b- defN 23-Jun-09 11:18 torchrec/metrics/model_utils.py
--rw-r--r--  2.0 unx     4631 b- defN 23-Jun-09 11:18 torchrec/metrics/mse.py
--rw-r--r--  2.0 unx     5605 b- defN 23-Jun-09 11:18 torchrec/metrics/multiclass_recall.py
--rw-r--r--  2.0 unx     6811 b- defN 23-Jun-09 11:18 torchrec/metrics/ne.py
--rw-r--r--  2.0 unx    33554 b- defN 23-Jun-09 11:18 torchrec/metrics/rec_metric.py
--rw-r--r--  2.0 unx    10490 b- defN 23-Jun-09 11:18 torchrec/metrics/recall_session.py
--rw-r--r--  2.0 unx     6057 b- defN 23-Jun-09 11:18 torchrec/metrics/throughput.py
--rw-r--r--  2.0 unx    11160 b- defN 23-Jun-09 11:18 torchrec/metrics/tower_qps.py
--rw-r--r--  2.0 unx     2867 b- defN 23-Jun-09 11:18 torchrec/metrics/weighted_avg.py
--rw-r--r--  2.0 unx    16441 b- defN 23-Jun-09 11:18 torchrec/metrics/test_utils/__init__.py
--rw-r--r--  2.0 unx      913 b- defN 23-Jun-09 11:18 torchrec/models/__init__.py
--rw-r--r--  2.0 unx    11410 b- defN 23-Jun-09 11:18 torchrec/models/deepfm.py
--rw-r--r--  2.0 unx    30000 b- defN 23-Jun-09 11:18 torchrec/models/dlrm.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 11:18 torchrec/models/experimental/__init__.py
--rw-r--r--  2.0 unx     9825 b- defN 23-Jun-09 11:18 torchrec/models/experimental/test_transformerdlrm.py
--rw-r--r--  2.0 unx     7434 b- defN 23-Jun-09 11:18 torchrec/models/experimental/transformerdlrm.py
--rw-r--r--  2.0 unx     1179 b- defN 23-Jun-09 11:18 torchrec/modules/__init__.py
--rw-r--r--  2.0 unx     1456 b- defN 23-Jun-09 11:18 torchrec/modules/activation.py
--rw-r--r--  2.0 unx    15163 b- defN 23-Jun-09 11:18 torchrec/modules/crossnet.py
--rw-r--r--  2.0 unx     8415 b- defN 23-Jun-09 11:18 torchrec/modules/deepfm.py
--rw-r--r--  2.0 unx     5537 b- defN 23-Jun-09 11:18 torchrec/modules/embedding_configs.py
--rw-r--r--  2.0 unx    14021 b- defN 23-Jun-09 11:18 torchrec/modules/embedding_modules.py
--rw-r--r--  2.0 unx     4858 b- defN 23-Jun-09 11:18 torchrec/modules/embedding_tower.py
--rw-r--r--  2.0 unx    12360 b- defN 23-Jun-09 11:18 torchrec/modules/feature_processor.py
--rw-r--r--  2.0 unx     4830 b- defN 23-Jun-09 11:18 torchrec/modules/feature_processor_.py
--rw-r--r--  2.0 unx     4403 b- defN 23-Jun-09 11:18 torchrec/modules/fp_embedding_modules.py
--rw-r--r--  2.0 unx    31453 b- defN 23-Jun-09 11:18 torchrec/modules/fused_embedding_modules.py
--rw-r--r--  2.0 unx    10894 b- defN 23-Jun-09 11:18 torchrec/modules/lazy_extension.py
--rw-r--r--  2.0 unx     6309 b- defN 23-Jun-09 11:18 torchrec/modules/mlp.py
--rw-r--r--  2.0 unx     4022 b- defN 23-Jun-09 11:18 torchrec/modules/utils.py
--rw-r--r--  2.0 unx     1639 b- defN 23-Jun-09 11:18 torchrec/optim/__init__.py
--rw-r--r--  2.0 unx     2012 b- defN 23-Jun-09 11:18 torchrec/optim/apply_optimizer_in_backward.py
--rw-r--r--  2.0 unx     1569 b- defN 23-Jun-09 11:18 torchrec/optim/clipping.py
--rw-r--r--  2.0 unx     1353 b- defN 23-Jun-09 11:18 torchrec/optim/fused.py
--rw-r--r--  2.0 unx    16069 b- defN 23-Jun-09 11:18 torchrec/optim/keyed.py
--rw-r--r--  2.0 unx     4420 b- defN 23-Jun-09 11:18 torchrec/optim/optimizers.py
--rw-r--r--  2.0 unx     7405 b- defN 23-Jun-09 11:18 torchrec/optim/rowwise_adagrad.py
--rw-r--r--  2.0 unx     4865 b- defN 23-Jun-09 11:18 torchrec/optim/warmup.py
--rw-r--r--  2.0 unx      560 b- defN 23-Jun-09 11:18 torchrec/optim/test_utils/__init__.py
--rw-r--r--  2.0 unx     1140 b- defN 23-Jun-09 11:18 torchrec/quant/__init__.py
--rw-r--r--  2.0 unx    25656 b- defN 23-Jun-09 11:18 torchrec/quant/embedding_modules.py
--rw-r--r--  2.0 unx     4296 b- defN 23-Jun-09 11:18 torchrec/quant/utils.py
--rw-r--r--  2.0 unx     1163 b- defN 23-Jun-09 11:18 torchrec/sparse/__init__.py
--rw-r--r--  2.0 unx    55583 b- defN 23-Jun-09 11:18 torchrec/sparse/jagged_tensor.py
--rw-r--r--  2.0 unx     1430 b- defN 23-Jun-09 11:18 torchrec/sparse/test_utils/__init__.py
--rw-r--r--  2.0 unx     5661 b- defN 23-Jun-09 11:18 torchrec/test_utils/__init__.py
--rw-r--r--  2.0 unx     1530 b- defN 23-Jun-09 11:22 torchrec_nightly-2023.6.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     5011 b- defN 23-Jun-09 11:22 torchrec_nightly-2023.6.9.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-09 11:22 torchrec_nightly-2023.6.9.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-09 11:22 torchrec_nightly-2023.6.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    13347 b- defN 23-Jun-09 11:22 torchrec_nightly-2023.6.9.dist-info/RECORD
-143 files, 1449792 bytes uncompressed, 332551 bytes compressed:  77.1%
+Zip file size: 458309 bytes, number of entries: 195
+-rw-rw-r--  2.0 unx      811 b- defN 22-Jun-26 17:35 torchrec/__init__.py
+-rw-rw-r--  2.0 unx     1638 b- defN 22-Dec-08 16:16 torchrec/streamable.py
+-rw-rw-r--  2.0 unx      854 b- defN 22-Nov-19 20:09 torchrec/types.py
+-rw-rw-r--  2.0 unx     1153 b- defN 22-Jun-26 17:35 torchrec/datasets/__init__.py
+-rw-rw-r--  2.0 unx    41469 b- defN 23-Mar-14 04:25 torchrec/datasets/criteo.py
+-rw-rw-r--  2.0 unx     4548 b- defN 22-Jun-26 17:35 torchrec/datasets/movielens.py
+-rw-rw-r--  2.0 unx     6539 b- defN 23-Mar-14 04:25 torchrec/datasets/random.py
+-rw-rw-r--  2.0 unx    10909 b- defN 22-Jun-26 17:35 torchrec/datasets/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-May-12 04:55 torchrec/datasets/scripts/__init__.py
+-rw-rw-r--  2.0 unx     2448 b- defN 22-Oct-05 20:41 torchrec/datasets/scripts/contiguous_preproc_criteo.py
+-rw-rw-r--  2.0 unx     2847 b- defN 23-Mar-14 04:25 torchrec/datasets/scripts/npy_preproc_criteo.py
+-rw-rw-r--  2.0 unx     3077 b- defN 22-Oct-05 20:41 torchrec/datasets/scripts/shuffle_preproc_criteo.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Jun-26 17:35 torchrec/datasets/test_utils/__init__.py
+-rw-rw-r--  2.0 unx     5308 b- defN 22-Oct-05 20:41 torchrec/datasets/test_utils/criteo_test_utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-May-12 04:55 torchrec/datasets/tests/__init__.py
+-rw-rw-r--  2.0 unx    22047 b- defN 22-Dec-08 16:16 torchrec/datasets/tests/test_criteo.py
+-rw-rw-r--  2.0 unx     4659 b- defN 22-Jun-26 17:35 torchrec/datasets/tests/test_movielens.py
+-rw-rw-r--  2.0 unx     3925 b- defN 22-Jun-26 17:35 torchrec/datasets/tests/test_random.py
+-rw-rw-r--  2.0 unx     5684 b- defN 22-Jun-26 17:35 torchrec/datasets/tests/test_utils.py
+-rw-rw-r--  2.0 unx     1912 b- defN 22-Jun-26 17:35 torchrec/distributed/__init__.py
+-rw-rw-r--  2.0 unx    37307 b- defN 23-Jul-12 13:50 torchrec/distributed/batched_embedding_kernel.py
+-rw-rw-r--  2.0 unx     2069 b- defN 22-Nov-19 20:09 torchrec/distributed/collective_utils.py
+-rw-rw-r--  2.0 unx     4988 b- defN 23-Jul-12 13:50 torchrec/distributed/comm.py
+-rw-rw-r--  2.0 unx    55918 b- defN 23-Jul-12 13:50 torchrec/distributed/comm_ops.py
+-rw-rw-r--  2.0 unx    36506 b- defN 23-Jul-12 13:50 torchrec/distributed/dist_data.py
+-rw-rw-r--  2.0 unx    32295 b- defN 23-Jul-12 13:50 torchrec/distributed/embedding.py
+-rw-rw-r--  2.0 unx     4947 b- defN 23-Jul-12 13:50 torchrec/distributed/embedding_kernel.py
+-rw-rw-r--  2.0 unx    29185 b- defN 23-Jul-12 13:50 torchrec/distributed/embedding_lookup.py
+-rw-rw-r--  2.0 unx    20950 b- defN 23-Jul-12 13:50 torchrec/distributed/embedding_sharding.py
+-rw-rw-r--  2.0 unx    36853 b- defN 23-Jul-12 13:50 torchrec/distributed/embedding_tower_sharding.py
+-rw-rw-r--  2.0 unx    15030 b- defN 23-Jul-12 13:50 torchrec/distributed/embedding_types.py
+-rw-rw-r--  2.0 unx    37214 b- defN 23-Jul-12 13:50 torchrec/distributed/embeddingbag.py
+-rw-rw-r--  2.0 unx     7373 b- defN 23-Apr-27 17:01 torchrec/distributed/fbgemm_qcomm_codec.py
+-rw-rw-r--  2.0 unx     6137 b- defN 23-Jul-12 13:50 torchrec/distributed/fp_embeddingbag.py
+-rw-rw-r--  2.0 unx     5243 b- defN 23-Jul-12 13:50 torchrec/distributed/fused_embedding.py
+-rw-rw-r--  2.0 unx     5080 b- defN 23-Jul-12 13:50 torchrec/distributed/fused_embeddingbag.py
+-rw-rw-r--  2.0 unx     2271 b- defN 23-Jul-12 13:50 torchrec/distributed/fused_params.py
+-rw-rw-r--  2.0 unx     3807 b- defN 22-Dec-08 16:16 torchrec/distributed/grouped_position_weighted.py
+-rw-rw-r--  2.0 unx    19750 b- defN 23-Jul-12 13:50 torchrec/distributed/model_parallel.py
+-rw-rw-r--  2.0 unx    20748 b- defN 23-Jul-12 13:50 torchrec/distributed/quant_embedding.py
+-rw-rw-r--  2.0 unx    15112 b- defN 23-Jul-12 13:50 torchrec/distributed/quant_embedding_kernel.py
+-rw-rw-r--  2.0 unx    12621 b- defN 23-Jul-12 13:50 torchrec/distributed/quant_embeddingbag.py
+-rw-rw-r--  2.0 unx    13928 b- defN 23-Jul-12 13:50 torchrec/distributed/quant_state.py
+-rw-rw-r--  2.0 unx     9261 b- defN 23-Jul-12 13:50 torchrec/distributed/shard.py
+-rw-rw-r--  2.0 unx    19646 b- defN 23-Jul-12 13:50 torchrec/distributed/sharding_plan.py
+-rw-rw-r--  2.0 unx    39755 b- defN 23-Jul-12 13:50 torchrec/distributed/train_pipeline.py
+-rw-rw-r--  2.0 unx    27865 b- defN 23-Jul-12 13:50 torchrec/distributed/types.py
+-rw-rw-r--  2.0 unx    15470 b- defN 23-Jul-12 13:50 torchrec/distributed/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jan-25 20:15 torchrec/distributed/composable/__init__.py
+-rw-rw-r--  2.0 unx     3207 b- defN 23-Feb-01 01:07 torchrec/distributed/composable/table_batched_embedding_slice.py
+-rw-rw-r--  2.0 unx     1025 b- defN 22-Jun-26 17:35 torchrec/distributed/planner/__init__.py
+-rw-rw-r--  2.0 unx     3135 b- defN 23-Mar-14 04:25 torchrec/distributed/planner/constants.py
+-rw-rw-r--  2.0 unx    11430 b- defN 23-Jul-12 13:50 torchrec/distributed/planner/enumerators.py
+-rw-rw-r--  2.0 unx    11739 b- defN 22-Oct-10 22:25 torchrec/distributed/planner/parallelized_planners.py
+-rw-rw-r--  2.0 unx    12642 b- defN 23-Jul-12 13:50 torchrec/distributed/planner/partitioners.py
+-rw-rw-r--  2.0 unx      835 b- defN 23-Jul-12 13:50 torchrec/distributed/planner/perf_models.py
+-rw-rw-r--  2.0 unx    13530 b- defN 23-Jul-12 13:50 torchrec/distributed/planner/planners.py
+-rw-rw-r--  2.0 unx    11236 b- defN 23-Jul-12 13:50 torchrec/distributed/planner/proposers.py
+-rw-rw-r--  2.0 unx    41291 b- defN 23-Jul-12 13:50 torchrec/distributed/planner/shard_estimators.py
+-rw-rw-r--  2.0 unx    23791 b- defN 23-Jul-12 13:50 torchrec/distributed/planner/stats.py
+-rw-rw-r--  2.0 unx     9643 b- defN 23-Jul-12 13:50 torchrec/distributed/planner/storage_reservations.py
+-rw-rw-r--  2.0 unx    14582 b- defN 23-Jul-12 13:50 torchrec/distributed/planner/types.py
+-rw-rw-r--  2.0 unx     1119 b- defN 22-Oct-26 23:15 torchrec/distributed/planner/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Jun-26 17:35 torchrec/distributed/sharding/__init__.py
+-rw-rw-r--  2.0 unx     2479 b- defN 23-Jul-12 13:50 torchrec/distributed/sharding/cw_sequence_sharding.py
+-rw-rw-r--  2.0 unx    12945 b- defN 23-Jul-12 13:50 torchrec/distributed/sharding/cw_sharding.py
+-rw-rw-r--  2.0 unx     2802 b- defN 23-Jan-25 20:15 torchrec/distributed/sharding/dp_sequence_sharding.py
+-rw-rw-r--  2.0 unx     7681 b- defN 23-Jul-12 13:50 torchrec/distributed/sharding/dp_sharding.py
+-rw-rw-r--  2.0 unx     7640 b- defN 23-Jul-12 13:50 torchrec/distributed/sharding/rw_sequence_sharding.py
+-rw-rw-r--  2.0 unx    17911 b- defN 23-Jul-12 13:50 torchrec/distributed/sharding/rw_sharding.py
+-rw-rw-r--  2.0 unx     3627 b- defN 23-Jul-12 13:50 torchrec/distributed/sharding/sequence_sharding.py
+-rw-rw-r--  2.0 unx     7632 b- defN 23-Jul-12 13:50 torchrec/distributed/sharding/tw_sequence_sharding.py
+-rw-rw-r--  2.0 unx    16097 b- defN 23-Jul-12 13:50 torchrec/distributed/sharding/tw_sharding.py
+-rw-rw-r--  2.0 unx     1284 b- defN 22-Jul-28 18:28 torchrec/distributed/sharding/twcw_sharding.py
+-rw-rw-r--  2.0 unx    19871 b- defN 23-Jul-12 13:50 torchrec/distributed/sharding/twrw_sharding.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Jun-26 17:35 torchrec/distributed/test_utils/__init__.py
+-rw-rw-r--  2.0 unx    11237 b- defN 23-Jul-12 13:50 torchrec/distributed/test_utils/infer_utils.py
+-rw-rw-r--  2.0 unx     4868 b- defN 23-Mar-14 04:25 torchrec/distributed/test_utils/multi_process.py
+-rw-rw-r--  2.0 unx    34091 b- defN 23-Jul-12 13:50 torchrec/distributed/test_utils/test_model.py
+-rw-rw-r--  2.0 unx    11197 b- defN 23-Jul-12 13:50 torchrec/distributed/test_utils/test_model_parallel.py
+-rw-rw-r--  2.0 unx    25310 b- defN 23-Jul-12 13:50 torchrec/distributed/test_utils/test_model_parallel_base.py
+-rw-rw-r--  2.0 unx    15367 b- defN 23-Mar-14 04:25 torchrec/distributed/test_utils/test_sharding.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Jun-26 17:35 torchrec/distributed/tests/__init__.py
+-rw-rw-r--  2.0 unx     4747 b- defN 22-Jun-26 17:35 torchrec/distributed/tests/collective_utils_test.py
+-rw-rw-r--  2.0 unx    16544 b- defN 22-Nov-19 20:09 torchrec/distributed/tests/test_apply_optim_per_param.py
+-rw-rw-r--  2.0 unx     1122 b- defN 22-Jun-26 17:35 torchrec/distributed/tests/test_awaitable.py
+-rw-rw-r--  2.0 unx     6614 b- defN 22-Jun-26 17:35 torchrec/distributed/tests/test_comm.py
+-rw-rw-r--  2.0 unx    33737 b- defN 22-Dec-08 16:16 torchrec/distributed/tests/test_dist_data.py
+-rw-rw-r--  2.0 unx     2801 b- defN 22-Nov-19 20:09 torchrec/distributed/tests/test_fbgemm_qcomm_codec.py
+-rw-rw-r--  2.0 unx     7157 b- defN 22-Dec-08 16:16 torchrec/distributed/tests/test_fused_embedding_bag_collection.py
+-rw-rw-r--  2.0 unx     7477 b- defN 22-Jul-28 18:28 torchrec/distributed/tests/test_fused_embedding_collection.py
+-rw-rw-r--  2.0 unx    10230 b- defN 22-Jun-26 17:35 torchrec/distributed/tests/test_fused_optim.py
+-rw-rw-r--  2.0 unx     7993 b- defN 22-Jun-26 17:35 torchrec/distributed/tests/test_lazy_awaitable.py
+-rw-rw-r--  2.0 unx      667 b- defN 22-Dec-08 16:16 torchrec/distributed/tests/test_model_parallel_gloo.py
+-rw-rw-r--  2.0 unx    11105 b- defN 22-Dec-08 16:16 torchrec/distributed/tests/test_model_parallel_hierarchical.py
+-rw-rw-r--  2.0 unx      667 b- defN 22-Dec-08 16:16 torchrec/distributed/tests/test_model_parallel_nccl.py
+-rw-rw-r--  2.0 unx     9363 b- defN 22-Nov-19 20:09 torchrec/distributed/tests/test_qcomms_embedding_modules.py
+-rw-rw-r--  2.0 unx    22396 b- defN 22-Nov-19 20:09 torchrec/distributed/tests/test_quant_model_parallel.py
+-rw-rw-r--  2.0 unx     5835 b- defN 22-Oct-26 23:15 torchrec/distributed/tests/test_quant_sequence_model_parallel.py
+-rw-rw-r--  2.0 unx     6409 b- defN 22-Jun-26 17:35 torchrec/distributed/tests/test_quantize.py
+-rw-rw-r--  2.0 unx    11072 b- defN 22-Dec-08 16:16 torchrec/distributed/tests/test_sequence_model.py
+-rw-rw-r--  2.0 unx    11060 b- defN 22-Dec-08 16:16 torchrec/distributed/tests/test_sequence_model_parallel.py
+-rw-rw-r--  2.0 unx     4396 b- defN 22-Oct-19 18:30 torchrec/distributed/tests/test_sequence_model_parallel_hierarchical.py
+-rw-rw-r--  2.0 unx    22707 b- defN 22-Dec-08 16:16 torchrec/distributed/tests/test_sharding_plan.py
+-rw-rw-r--  2.0 unx    12988 b- defN 22-Dec-08 16:16 torchrec/distributed/tests/test_train_pipeline.py
+-rw-rw-r--  2.0 unx    13178 b- defN 22-Oct-05 20:41 torchrec/distributed/tests/test_utils.py
+-rw-rw-r--  2.0 unx      422 b- defN 22-Jun-26 17:35 torchrec/fx/__init__.py
+-rw-rw-r--  2.0 unx     6451 b- defN 23-Jul-12 13:50 torchrec/fx/tracer.py
+-rw-rw-r--  2.0 unx     4524 b- defN 23-Jul-12 13:50 torchrec/fx/utils.py
+-rw-rw-r--  2.0 unx     1223 b- defN 22-Jun-26 17:35 torchrec/inference/__init__.py
+-rw-rw-r--  2.0 unx     3614 b- defN 22-Jun-26 17:35 torchrec/inference/client.py
+-rw-rw-r--  2.0 unx     3957 b- defN 23-Jan-25 20:15 torchrec/inference/model_packager.py
+-rw-rw-r--  2.0 unx     8068 b- defN 23-Jul-12 13:50 torchrec/inference/modules.py
+-rw-rw-r--  2.0 unx     3797 b- defN 22-Nov-19 20:09 torchrec/inference/state_dict_transform.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Jun-26 17:35 torchrec/metrics/__init__.py
+-rw-rw-r--  2.0 unx     4168 b- defN 23-Jul-12 13:50 torchrec/metrics/accuracy.py
+-rw-rw-r--  2.0 unx    12549 b- defN 23-Jul-12 13:50 torchrec/metrics/auc.py
+-rw-rw-r--  2.0 unx     3703 b- defN 23-Jan-25 20:15 torchrec/metrics/calibration.py
+-rw-rw-r--  2.0 unx     3465 b- defN 23-Jan-25 20:15 torchrec/metrics/ctr.py
+-rw-rw-r--  2.0 unx     3836 b- defN 22-Dec-08 16:16 torchrec/metrics/mae.py
+-rw-rw-r--  2.0 unx    17909 b- defN 23-Jul-12 13:50 torchrec/metrics/metric_module.py
+-rw-rw-r--  2.0 unx     6796 b- defN 23-Jul-12 13:50 torchrec/metrics/metrics_config.py
+-rw-rw-r--  2.0 unx     3731 b- defN 23-Jul-12 13:50 torchrec/metrics/metrics_namespace.py
+-rw-rw-r--  2.0 unx     3904 b- defN 23-Mar-14 04:25 torchrec/metrics/model_utils.py
+-rw-rw-r--  2.0 unx     4631 b- defN 23-Jan-25 20:15 torchrec/metrics/mse.py
+-rw-rw-r--  2.0 unx     5605 b- defN 22-Dec-08 16:16 torchrec/metrics/multiclass_recall.py
+-rw-rw-r--  2.0 unx     6811 b- defN 23-Mar-14 04:25 torchrec/metrics/ne.py
+-rw-rw-r--  2.0 unx    33554 b- defN 23-Jul-12 13:50 torchrec/metrics/rec_metric.py
+-rw-rw-r--  2.0 unx    10490 b- defN 23-Apr-27 17:01 torchrec/metrics/recall_session.py
+-rw-rw-r--  2.0 unx     6057 b- defN 22-Nov-19 20:09 torchrec/metrics/throughput.py
+-rw-rw-r--  2.0 unx    11160 b- defN 23-Jul-12 13:50 torchrec/metrics/tower_qps.py
+-rw-rw-r--  2.0 unx     2867 b- defN 23-Mar-14 04:25 torchrec/metrics/weighted_avg.py
+-rw-rw-r--  2.0 unx    16441 b- defN 23-Mar-14 04:25 torchrec/metrics/test_utils/__init__.py
+-rw-rw-r--  2.0 unx      913 b- defN 22-Jun-26 17:35 torchrec/models/__init__.py
+-rw-rw-r--  2.0 unx    11410 b- defN 23-Apr-27 17:01 torchrec/models/deepfm.py
+-rw-rw-r--  2.0 unx    29965 b- defN 23-Jul-12 13:50 torchrec/models/dlrm.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Dec-08 16:16 torchrec/models/experimental/__init__.py
+-rw-rw-r--  2.0 unx     9825 b- defN 23-Jul-12 13:50 torchrec/models/experimental/test_transformerdlrm.py
+-rw-rw-r--  2.0 unx     7434 b- defN 22-Dec-08 16:16 torchrec/models/experimental/transformerdlrm.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Jun-26 17:35 torchrec/models/tests/__init__.py
+-rw-rw-r--  2.0 unx     5892 b- defN 22-Oct-05 20:41 torchrec/models/tests/test_deepfm.py
+-rw-rw-r--  2.0 unx    34899 b- defN 22-Oct-05 20:41 torchrec/models/tests/test_dlrm.py
+-rw-rw-r--  2.0 unx     1179 b- defN 22-Jun-26 17:35 torchrec/modules/__init__.py
+-rw-rw-r--  2.0 unx     1456 b- defN 22-Jun-26 17:35 torchrec/modules/activation.py
+-rw-rw-r--  2.0 unx    14636 b- defN 23-Jul-12 13:50 torchrec/modules/crossnet.py
+-rw-rw-r--  2.0 unx     8415 b- defN 22-Jun-26 17:35 torchrec/modules/deepfm.py
+-rw-rw-r--  2.0 unx     6468 b- defN 23-Jul-12 13:50 torchrec/modules/embedding_configs.py
+-rw-rw-r--  2.0 unx    14021 b- defN 23-Jul-12 13:50 torchrec/modules/embedding_modules.py
+-rw-rw-r--  2.0 unx     4858 b- defN 22-Jun-27 21:00 torchrec/modules/embedding_tower.py
+-rw-rw-r--  2.0 unx    12360 b- defN 23-Apr-27 17:01 torchrec/modules/feature_processor.py
+-rw-rw-r--  2.0 unx     4832 b- defN 23-Jul-12 13:50 torchrec/modules/feature_processor_.py
+-rw-rw-r--  2.0 unx     4403 b- defN 23-Jul-12 13:50 torchrec/modules/fp_embedding_modules.py
+-rw-rw-r--  2.0 unx    31545 b- defN 23-Jul-12 13:50 torchrec/modules/fused_embedding_modules.py
+-rw-rw-r--  2.0 unx    10541 b- defN 23-Jul-12 13:50 torchrec/modules/lazy_extension.py
+-rw-rw-r--  2.0 unx     6309 b- defN 22-Jun-26 17:35 torchrec/modules/mlp.py
+-rw-rw-r--  2.0 unx     3897 b- defN 23-Jul-12 13:50 torchrec/modules/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-May-12 04:55 torchrec/modules/tests/__init__.py
+-rw-rw-r--  2.0 unx      855 b- defN 22-Jun-26 17:35 torchrec/modules/tests/test_activation.py
+-rw-rw-r--  2.0 unx     1145 b- defN 22-Jun-26 17:35 torchrec/modules/tests/test_code_quality.py
+-rw-rw-r--  2.0 unx     5328 b- defN 22-Jun-26 17:35 torchrec/modules/tests/test_crossnet.py
+-rw-rw-r--  2.0 unx     5095 b- defN 22-Jun-26 17:35 torchrec/modules/tests/test_deepfm.py
+-rw-rw-r--  2.0 unx    10958 b- defN 22-Jun-27 21:00 torchrec/modules/tests/test_embedding_modules.py
+-rw-rw-r--  2.0 unx     3476 b- defN 22-Jun-29 03:57 torchrec/modules/tests/test_feature_processor.py
+-rw-rw-r--  2.0 unx    36277 b- defN 22-Jul-28 18:28 torchrec/modules/tests/test_fused_embedding_modules.py
+-rw-rw-r--  2.0 unx    11158 b- defN 22-Jun-26 17:35 torchrec/modules/tests/test_lazy_extension.py
+-rw-rw-r--  2.0 unx     3325 b- defN 22-Jun-26 17:35 torchrec/modules/tests/test_mlp.py
+-rw-rw-r--  2.0 unx     1639 b- defN 22-Oct-19 18:30 torchrec/optim/__init__.py
+-rw-rw-r--  2.0 unx     2012 b- defN 23-Mar-14 04:25 torchrec/optim/apply_optimizer_in_backward.py
+-rw-rw-r--  2.0 unx     1569 b- defN 22-Jun-26 17:35 torchrec/optim/clipping.py
+-rw-rw-r--  2.0 unx     1353 b- defN 23-Jan-25 20:15 torchrec/optim/fused.py
+-rw-rw-r--  2.0 unx    16069 b- defN 23-Mar-14 04:25 torchrec/optim/keyed.py
+-rw-rw-r--  2.0 unx     4420 b- defN 23-Jan-25 20:15 torchrec/optim/optimizers.py
+-rw-rw-r--  2.0 unx     7405 b- defN 23-Apr-27 17:01 torchrec/optim/rowwise_adagrad.py
+-rw-rw-r--  2.0 unx     4865 b- defN 22-Oct-05 20:41 torchrec/optim/warmup.py
+-rw-rw-r--  2.0 unx      560 b- defN 22-Jun-26 17:35 torchrec/optim/test_utils/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Jun-26 17:35 torchrec/optim/tests/__init__.py
+-rw-rw-r--  2.0 unx     3377 b- defN 22-Oct-19 18:30 torchrec/optim/tests/test_apply_optimizer_in_backward.py
+-rw-rw-r--  2.0 unx     8255 b- defN 22-Jun-26 17:35 torchrec/optim/tests/test_clipping.py
+-rw-rw-r--  2.0 unx    12347 b- defN 22-Jun-26 17:35 torchrec/optim/tests/test_keyed.py
+-rw-rw-r--  2.0 unx     1973 b- defN 22-Jun-26 17:35 torchrec/optim/tests/test_rowwise_adagrad.py
+-rw-rw-r--  2.0 unx     2486 b- defN 22-Jun-26 17:35 torchrec/optim/tests/test_warmup.py
+-rw-rw-r--  2.0 unx     1140 b- defN 22-Jun-26 17:35 torchrec/quant/__init__.py
+-rw-rw-r--  2.0 unx    26618 b- defN 23-Jul-12 13:50 torchrec/quant/embedding_modules.py
+-rw-rw-r--  2.0 unx     4292 b- defN 23-Jul-12 13:50 torchrec/quant/utils.py
+-rw-rw-r--  2.0 unx     1163 b- defN 22-Jun-26 17:35 torchrec/sparse/__init__.py
+-rw-rw-r--  2.0 unx    56945 b- defN 23-Jul-12 14:03 torchrec/sparse/jagged_tensor.py
+-rw-rw-r--  2.0 unx     1430 b- defN 22-Jun-26 17:35 torchrec/sparse/test_utils/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-May-12 04:55 torchrec/sparse/tests/__init__.py
+-rw-rw-r--  2.0 unx    53408 b- defN 22-Dec-08 16:16 torchrec/sparse/tests/test_jagged_tensor.py
+-rw-rw-r--  2.0 unx     5661 b- defN 23-Jan-25 20:15 torchrec/test_utils/__init__.py
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Jul-12 14:36 torchrec_nightly-2023.7.12.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5012 b- defN 23-Jul-12 14:36 torchrec_nightly-2023.7.12.dist-info/METADATA
+-rw-rw-r--  2.0 unx      106 b- defN 23-Jul-12 14:36 torchrec_nightly-2023.7.12.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jul-12 14:36 torchrec_nightly-2023.7.12.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    18685 b- defN 23-Jul-12 14:36 torchrec_nightly-2023.7.12.dist-info/RECORD
+195 files, 1985603 bytes uncompressed, 428255 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -36,14 +36,29 @@
 
 Filename: torchrec/datasets/test_utils/__init__.py
 Comment: 
 
 Filename: torchrec/datasets/test_utils/criteo_test_utils.py
 Comment: 
 
+Filename: torchrec/datasets/tests/__init__.py
+Comment: 
+
+Filename: torchrec/datasets/tests/test_criteo.py
+Comment: 
+
+Filename: torchrec/datasets/tests/test_movielens.py
+Comment: 
+
+Filename: torchrec/datasets/tests/test_random.py
+Comment: 
+
+Filename: torchrec/datasets/tests/test_utils.py
+Comment: 
+
 Filename: torchrec/distributed/__init__.py
 Comment: 
 
 Filename: torchrec/distributed/batched_embedding_kernel.py
 Comment: 
 
 Filename: torchrec/distributed/collective_utils.py
@@ -105,14 +120,17 @@
 
 Filename: torchrec/distributed/quant_embedding_kernel.py
 Comment: 
 
 Filename: torchrec/distributed/quant_embeddingbag.py
 Comment: 
 
+Filename: torchrec/distributed/quant_state.py
+Comment: 
+
 Filename: torchrec/distributed/shard.py
 Comment: 
 
 Filename: torchrec/distributed/sharding_plan.py
 Comment: 
 
 Filename: torchrec/distributed/train_pipeline.py
@@ -135,14 +153,17 @@
 
 Filename: torchrec/distributed/planner/constants.py
 Comment: 
 
 Filename: torchrec/distributed/planner/enumerators.py
 Comment: 
 
+Filename: torchrec/distributed/planner/parallelized_planners.py
+Comment: 
+
 Filename: torchrec/distributed/planner/partitioners.py
 Comment: 
 
 Filename: torchrec/distributed/planner/perf_models.py
 Comment: 
 
 Filename: torchrec/distributed/planner/planners.py
@@ -219,14 +240,86 @@
 
 Filename: torchrec/distributed/test_utils/test_model_parallel_base.py
 Comment: 
 
 Filename: torchrec/distributed/test_utils/test_sharding.py
 Comment: 
 
+Filename: torchrec/distributed/tests/__init__.py
+Comment: 
+
+Filename: torchrec/distributed/tests/collective_utils_test.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_apply_optim_per_param.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_awaitable.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_comm.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_dist_data.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_fbgemm_qcomm_codec.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_fused_embedding_bag_collection.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_fused_embedding_collection.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_fused_optim.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_lazy_awaitable.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_model_parallel_gloo.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_model_parallel_hierarchical.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_model_parallel_nccl.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_qcomms_embedding_modules.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_quant_model_parallel.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_quant_sequence_model_parallel.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_quantize.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_sequence_model.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_sequence_model_parallel.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_sequence_model_parallel_hierarchical.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_sharding_plan.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_train_pipeline.py
+Comment: 
+
+Filename: torchrec/distributed/tests/test_utils.py
+Comment: 
+
 Filename: torchrec/fx/__init__.py
 Comment: 
 
 Filename: torchrec/fx/tracer.py
 Comment: 
 
 Filename: torchrec/fx/utils.py
@@ -318,14 +411,23 @@
 
 Filename: torchrec/models/experimental/test_transformerdlrm.py
 Comment: 
 
 Filename: torchrec/models/experimental/transformerdlrm.py
 Comment: 
 
+Filename: torchrec/models/tests/__init__.py
+Comment: 
+
+Filename: torchrec/models/tests/test_deepfm.py
+Comment: 
+
+Filename: torchrec/models/tests/test_dlrm.py
+Comment: 
+
 Filename: torchrec/modules/__init__.py
 Comment: 
 
 Filename: torchrec/modules/activation.py
 Comment: 
 
 Filename: torchrec/modules/crossnet.py
@@ -360,14 +462,44 @@
 
 Filename: torchrec/modules/mlp.py
 Comment: 
 
 Filename: torchrec/modules/utils.py
 Comment: 
 
+Filename: torchrec/modules/tests/__init__.py
+Comment: 
+
+Filename: torchrec/modules/tests/test_activation.py
+Comment: 
+
+Filename: torchrec/modules/tests/test_code_quality.py
+Comment: 
+
+Filename: torchrec/modules/tests/test_crossnet.py
+Comment: 
+
+Filename: torchrec/modules/tests/test_deepfm.py
+Comment: 
+
+Filename: torchrec/modules/tests/test_embedding_modules.py
+Comment: 
+
+Filename: torchrec/modules/tests/test_feature_processor.py
+Comment: 
+
+Filename: torchrec/modules/tests/test_fused_embedding_modules.py
+Comment: 
+
+Filename: torchrec/modules/tests/test_lazy_extension.py
+Comment: 
+
+Filename: torchrec/modules/tests/test_mlp.py
+Comment: 
+
 Filename: torchrec/optim/__init__.py
 Comment: 
 
 Filename: torchrec/optim/apply_optimizer_in_backward.py
 Comment: 
 
 Filename: torchrec/optim/clipping.py
@@ -387,14 +519,32 @@
 
 Filename: torchrec/optim/warmup.py
 Comment: 
 
 Filename: torchrec/optim/test_utils/__init__.py
 Comment: 
 
+Filename: torchrec/optim/tests/__init__.py
+Comment: 
+
+Filename: torchrec/optim/tests/test_apply_optimizer_in_backward.py
+Comment: 
+
+Filename: torchrec/optim/tests/test_clipping.py
+Comment: 
+
+Filename: torchrec/optim/tests/test_keyed.py
+Comment: 
+
+Filename: torchrec/optim/tests/test_rowwise_adagrad.py
+Comment: 
+
+Filename: torchrec/optim/tests/test_warmup.py
+Comment: 
+
 Filename: torchrec/quant/__init__.py
 Comment: 
 
 Filename: torchrec/quant/embedding_modules.py
 Comment: 
 
 Filename: torchrec/quant/utils.py
@@ -405,26 +555,32 @@
 
 Filename: torchrec/sparse/jagged_tensor.py
 Comment: 
 
 Filename: torchrec/sparse/test_utils/__init__.py
 Comment: 
 
+Filename: torchrec/sparse/tests/__init__.py
+Comment: 
+
+Filename: torchrec/sparse/tests/test_jagged_tensor.py
+Comment: 
+
 Filename: torchrec/test_utils/__init__.py
 Comment: 
 
-Filename: torchrec_nightly-2023.6.9.dist-info/LICENSE
+Filename: torchrec_nightly-2023.7.12.dist-info/LICENSE
 Comment: 
 
-Filename: torchrec_nightly-2023.6.9.dist-info/METADATA
+Filename: torchrec_nightly-2023.7.12.dist-info/METADATA
 Comment: 
 
-Filename: torchrec_nightly-2023.6.9.dist-info/WHEEL
+Filename: torchrec_nightly-2023.7.12.dist-info/WHEEL
 Comment: 
 
-Filename: torchrec_nightly-2023.6.9.dist-info/top_level.txt
+Filename: torchrec_nightly-2023.7.12.dist-info/top_level.txt
 Comment: 
 
-Filename: torchrec_nightly-2023.6.9.dist-info/RECORD
+Filename: torchrec_nightly-2023.7.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torchrec/distributed/batched_embedding_kernel.py

```diff
@@ -379,25 +379,21 @@
     for t_idx, (rows, dim, location, _) in enumerate(emb_module.embedding_specs):
         table_name = config.embedding_tables[t_idx].name
         if table_name not in table_name_to_count:
             continue
         table_count = table_name_to_count.pop(table_name)
         if emb_module.weights_precision == SparseType.INT8:
             dim += emb_module.int8_emb_row_dim_offset
-        # pyre-ignore[29]
         offset = emb_module.weights_physical_offsets[t_idx]
         weights: torch.Tensor
         if location == EmbeddingLocation.DEVICE.value:
-            # pyre-ignore
             weights = emb_module.weights_dev
         elif location == EmbeddingLocation.HOST.value:
-            # pyre-ignore
             weights = emb_module.weights_host
         else:
-            # pyre-ignore
             weights = emb_module.weights_uvm
         weight = TableBatchedEmbeddingSlice(
             data=weights,
             start_offset=offset,
             end_offset=offset + table_count * rows * dim,
             num_embeddings=-1,
             embedding_dim=dim,
```

## torchrec/distributed/dist_data.py

```diff
@@ -373,23 +373,22 @@
     tensors asynchronously.
 
     Args:
         pg (dist.ProcessGroup): ProcessGroup for AlltoAll communication.
         splits (List[int]): List of len(pg.size()) which indicates how many features to
             send to each pg.rank(). It is assumed the `KeyedJaggedTensor` is ordered by
             destination rank. Same for all ranks.
-        device (Optional[torch.device]): device on which buffers will be allocated.
         stagger (int): stagger value to apply to recat tensor, see `_get_recat` function
             for more detail.
 
     Example::
 
         keys=['A','B','C']
         splits=[2,1]
-        kjtA2A = KJTAllToAll(pg, splits, device)
+        kjtA2A = KJTAllToAll(pg, splits)
         awaitable = kjtA2A(rank0_input)
 
         # where:
         # rank0_input is KeyedJaggedTensor holding
 
         #         0           1           2
         # 'A'    [A.V0]       None        [A.V1, A.V2]
@@ -417,15 +416,14 @@
         # 'C'     [C.V0]      [C.V1]      None        [C.V2]      [C.V3]      None
     """
 
     def __init__(
         self,
         pg: dist.ProcessGroup,
         splits: List[int],
-        device: Optional[torch.device] = None,
         stagger: int = 1,
     ) -> None:
         super().__init__()
         assert len(splits) == pg.size()
         self._pg: dist.ProcessGroup = pg
         self._splits = splits
         self._splits_cumsum: List[int] = [0] + list(itertools.accumulate(splits))
@@ -443,15 +441,14 @@
         Args:
             input (KeyedJaggedTensor): `KeyedJaggedTensor` of values to distribute.
 
         Returns:
             Awaitable[KJTAllToAllTensorsAwaitable]: awaitable of a `KJTAllToAllTensorsAwaitable`.
         """
 
-        device = input.values().device
         with torch.no_grad():
             assert len(input.keys()) == sum(self._splits)
             rank = dist.get_rank(self._pg)
             local_keys = input.keys()[
                 self._splits_cumsum[rank] : self._splits_cumsum[rank + 1]
             ]
 
@@ -459,15 +456,15 @@
                 pg=self._pg,
                 input=input,
                 splits=self._splits,
                 labels=input.dist_labels(),
                 tensor_splits=input.dist_splits(self._splits),
                 input_tensors=input.dist_tensors(),
                 keys=local_keys,
-                device=device,
+                device=input.device(),
                 stagger=self._stagger,
             )
 
 
 class KJTOneToAll(nn.Module):
     """
     Redistributes `KeyedJaggedTensor` to all devices.
@@ -488,15 +485,15 @@
         world_size: int,
         device: Optional[torch.device] = None,
     ) -> None:
         super().__init__()
         self._splits = splits
         self._world_size = world_size
         self._device_type = (
-            "cuda" if device is None or device.type == "cuda" else "meta"
+            "meta" if device is not None and device.type == "meta" else "cuda"
         )
         assert self._world_size == len(splits)
 
     def forward(self, kjt: KeyedJaggedTensor) -> KJTList:
         """
         Splits features first and then sends the slices to the corresponding devices.
 
@@ -649,14 +646,56 @@
         return pooled_embedding_awaitable
 
     @property
     def callbacks(self) -> List[Callable[[torch.Tensor], torch.Tensor]]:
         return self._callbacks
 
 
+class EmbeddingsAllToOneReduce(nn.Module):
+    """
+    Merges the pooled/sequence embedding tensor on each device into single tensor.
+
+    Args:
+        device (torch.device): device on which buffer will be allocated.
+        world_size (int): number of devices in the topology.
+        cat_dim (int): which dimension you would like to concatenate on.
+            For pooled embedding it is 1; for sequence embedding it is 0.
+    """
+
+    def __init__(
+        self,
+        device: torch.device,
+        world_size: int,
+        cat_dim: int,
+    ) -> None:
+        super().__init__()
+        self._device = device
+        self._world_size = world_size
+        self._cat_dim = cat_dim
+
+    def forward(
+        self,
+        tensors: List[torch.Tensor],
+    ) -> torch.Tensor:
+        """
+        Performs AlltoOne operation with Reduce on pooled/sequence embeddings tensors.
+
+        Args:
+            tensors (List[torch.Tensor]): list of embedding tensors.
+
+        Returns:
+            Awaitable[torch.Tensor]: awaitable of the reduced embeddings.
+        """
+        assert len(tensors) == self._world_size
+        return torch.ops.fbgemm.sum_reduce_to_one(
+            tensors,
+            self._device,
+        )
+
+
 class EmbeddingsAllToOne(nn.Module):
     """
     Merges the pooled/sequence embedding tensor on each device into single tensor.
 
     Args:
         device (torch.device): device on which buffer will be allocated.
         world_size (int): number of devices in the topology.
@@ -865,23 +904,21 @@
         self,
         tensor_awaitable: Awaitable[torch.Tensor],
         unbucketize_permute_tensor: Optional[torch.Tensor],
         embedding_dim: int,
     ) -> None:
         super().__init__()
         self._tensor_awaitable = tensor_awaitable
-        self._unbucketize_permute_tensor = unbucketize_permute_tensor
-        self._embedding_dim = embedding_dim
 
-        if self._unbucketize_permute_tensor is not None:
+        if unbucketize_permute_tensor is not None:
             self.callbacks.append(
                 lambda ret: torch.index_select(
-                    ret.view(-1, self._embedding_dim),
+                    ret.view(-1, embedding_dim),
                     0,
-                    self._unbucketize_permute_tensor,
+                    unbucketize_permute_tensor,
                 )
             )
 
     def _wait_impl(self) -> torch.Tensor:
         """
         Syncs sequence embeddings after collective operation.
```

## torchrec/distributed/embedding.py

```diff
@@ -48,15 +48,17 @@
     ParameterSharding,
     QuantizedCommCodecs,
     ShardedTensor,
     ShardingEnv,
     ShardMetadata,
 )
 from torchrec.distributed.utils import (
+    add_params_from_parameter_sharding,
     append_prefix,
+    convert_to_fbgemm_types,
     filter_state_dict,
     merge_fused_params,
     optimizer_type_to_emb_opt_type,
 )
 from torchrec.modules.embedding_configs import (
     EmbeddingConfig,
     EmbeddingTableConfig,
@@ -163,15 +165,20 @@
 
         optimizer_class = optimizer_classes[0]
         optimizer_params = optimizer_params[0]
         if optimizer_class:
             optimizer_params["optimizer"] = optimizer_type_to_emb_opt_type(
                 optimizer_class
             )
-        fused_params = merge_fused_params(fused_params, optimizer_params)
+
+        per_table_fused_params = merge_fused_params(fused_params, optimizer_params)
+        per_table_fused_params = add_params_from_parameter_sharding(
+            per_table_fused_params, parameter_sharding
+        )
+        per_table_fused_params = convert_to_fbgemm_types(per_table_fused_params)
 
         sharding_type_to_sharding_infos[parameter_sharding.sharding_type].append(
             (
                 EmbeddingShardingInfo(
                     embedding_config=EmbeddingTableConfig(
                         num_embeddings=config.num_embeddings,
                         embedding_dim=config.embedding_dim,
@@ -183,15 +190,15 @@
                         has_feature_processor=False,
                         embedding_names=embedding_names,
                         weight_init_max=config.weight_init_max,
                         weight_init_min=config.weight_init_min,
                     ),
                     param_sharding=parameter_sharding,
                     param=param,
-                    fused_params=fused_params,
+                    fused_params=per_table_fused_params,
                 )
             )
         )
     return sharding_type_to_sharding_infos
 
 
 def _construct_jagged_tensors(
@@ -428,17 +435,20 @@
                 local_shards = state_dict[key].local_shards()
                 # If no local shards, create an empty tensor
                 if len(local_shards) == 0:
                     state_dict[key] = torch.empty(0)
                 else:
                     dim = state_dict[key].metadata().shards_metadata[0].shard_sizes[1]
                     # CW multiple shards are merged
-                    state_dict[key] = torch.cat(
-                        [shard.tensor.view(-1) for shard in local_shards], dim=0
-                    ).view(-1, dim)
+                    if len(local_shards) > 1:
+                        state_dict[key] = torch.cat(
+                            [s.tensor.view(-1) for s in local_shards], dim=0
+                        ).view(-1, dim)
+                    else:
+                        state_dict[key] = local_shards[0].tensor.view(-1, dim)
             else:
                 local_shards = []
                 for shard in model_shards:
                     # Extract shard size and offsets for splicing
                     shard_sizes = shard.metadata.shard_sizes
                     shard_offsets = shard.metadata.shard_offsets
 
@@ -499,16 +509,14 @@
                     table_name = key[: -len(".weight")]
                     self._model_parallel_name_to_local_shards[table_name].extend(
                         v.local_shards()
                     )
             for (
                 table_name,
                 tbe_slice,
-                # pyre-fixme[16]: Item `Tensor` of `Union[Tensor, Module]` has no
-                #  attribute `named_parameters_by_table`.
             ) in lookup.named_parameters_by_table():
                 self.embeddings[table_name].register_parameter("weight", tbe_slice)
         for (
             table_name,
             local_shards,
         ) in self._model_parallel_name_to_local_shards.items():
             # for shards that don't exist on this rank, register with empty tensor
@@ -656,15 +664,14 @@
         if self._has_uninitialized_input_dist:
             self._create_input_dist(input_feature_names=features.keys())
             self._has_uninitialized_input_dist = False
         with torch.no_grad():
             if self._features_order:
                 features = features.permute(
                     self._features_order,
-                    # pyre-ignore [6]
                     self._features_order_tensor,
                 )
             features_by_shards = features.split(
                 self._feature_splits,
             )
             awaitables = []
             for input_dist, features in zip(self._input_dists, features_by_shards):
```

## torchrec/distributed/embedding_lookup.py

```diff
@@ -754,15 +754,15 @@
         device: Optional[torch.device] = None,
     ) -> None:
         super().__init__()
         self._embedding_lookups_per_rank: List[
             MetaInferGroupedPooledEmbeddingsLookup
         ] = []
 
-        device_type = "cuda" if device is None or device.type == "cuda" else "meta"
+        device_type = "meta" if device is not None and device.type == "meta" else "cuda"
         for rank in range(world_size):
             self._embedding_lookups_per_rank.append(
                 # TODO add position weighted module support
                 MetaInferGroupedPooledEmbeddingsLookup(
                     grouped_configs=grouped_configs_per_rank[rank],
                     # syntax for torchscript
                     device=torch.device(type=device_type, index=rank),
@@ -787,16 +787,15 @@
         world_size: int,
         fused_params: Optional[Dict[str, Any]] = None,
         device: Optional[torch.device] = None,
     ) -> None:
         super().__init__()
         self._embedding_lookups_per_rank: List[MetaInferGroupedEmbeddingsLookup] = []
 
-        device_type = "cuda" if device is None or device.type == "cuda" else "meta"
-
+        device_type = "meta" if device is not None and device.type == "meta" else "cuda"
         for rank in range(world_size):
             self._embedding_lookups_per_rank.append(
                 MetaInferGroupedEmbeddingsLookup(
                     grouped_configs=grouped_configs_per_rank[rank],
                     # syntax for torchscript
                     device=torch.device(type=device_type, index=rank),
                     fused_params=fused_params,
```

## torchrec/distributed/embedding_sharding.py

```diff
@@ -27,22 +27,33 @@
 )
 from torchrec.distributed.types import (
     Awaitable,
     ParameterSharding,
     QuantizedCommCodecs,
     ShardMetadata,
 )
+from torchrec.fx.utils import assert_fx_safe
 from torchrec.modules.embedding_configs import (
     DataType,
     EmbeddingTableConfig,
     PoolingType,
 )
 from torchrec.sparse.jagged_tensor import KeyedJaggedTensor
 from torchrec.streamable import Multistreamable
 
+torch.fx.wrap("len")
+
+
+# torch.Tensor.to can not be fx symbolic traced as it does not go through __torch_dispatch__ => fx.wrap it
+@torch.fx.wrap
+def _fx_wrap_tensor_to_device_dtype(
+    t: torch.Tensor, tensor_device_dtype: torch.Tensor
+) -> torch.Tensor:
+    return t.to(device=tensor_device_dtype.device, dtype=tensor_device_dtype.dtype)
+
 
 def bucketize_kjt_before_all2all(
     kjt: KeyedJaggedTensor,
     num_buckets: int,
     block_sizes: torch.Tensor,
     output_permute: bool = False,
     bucketize_pos: bool = False,
@@ -63,20 +74,19 @@
             not.
 
     Returns:
         Tuple[KeyedJaggedTensor, Optional[torch.Tensor]]: the bucketized `KeyedJaggedTensor` and the optional permute mapping from the unbucketized values to bucketized value.
     """
 
     num_features = len(kjt.keys())
-    assert (
-        block_sizes.numel() == num_features
-    ), f"Expecting block sizes for {num_features} features, but {block_sizes.numel()} received."
-
-    # kernel expects them to be same type, cast to avoid type mismatch
-    block_sizes_new_type = block_sizes.type(kjt.values().type())
+    assert_fx_safe(
+        block_sizes.numel() == num_features,
+        f"Expecting block sizes for {num_features} features, but {block_sizes.numel()} received.",
+    )
+    block_sizes_new_type = _fx_wrap_tensor_to_device_dtype(block_sizes, kjt.values())
     (
         bucketized_lengths,
         bucketized_indices,
         bucketized_weights,
         pos,
         unbucketize_permute,
     ) = torch.ops.fbgemm.block_bucketize_sparse_features(
```

## torchrec/distributed/embedding_tower_sharding.py

```diff
@@ -173,16 +173,14 @@
                 device_ids=[self._device],
                 process_group=self._intra_pg,
                 gradient_as_bucket_view=True,
                 broadcast_buffers=False,
             )
 
         # Setup output dists for quantized comms
-        # pyre-fixme[8]: Attribute has type `ModuleList`; used as `Union[Module,
-        #  Tensor]`.
         self._output_dists: nn.ModuleList = (
             self.embedding._output_dists if self.embedding else nn.ModuleList()
         )
 
     def _create_input_dist(
         self,
         kjt_feature_names: List[str],
@@ -222,22 +220,20 @@
             for node in range(node_count)
         ]
         self._cross_dist = KJTAllToAll(
             # pyre-fixme[6]: For 1st param expected `ProcessGroup` but got
             #  `Optional[ProcessGroup]`.
             self._cross_pg,
             kjt_features_per_node,
-            self._device,
         )
         self._weighted_cross_dist = KJTAllToAll(
             # pyre-fixme[6]: For 1st param expected `ProcessGroup` but got
             #  `Optional[ProcessGroup]`.
             self._cross_pg,
             wkjt_features_per_node,
-            self._device,
         )
 
     # pyre-ignore[14]
     def input_dist(
         self,
         ctx: NullShardedModuleContext,
         features: KeyedJaggedTensor,
@@ -377,15 +373,14 @@
                 destination, prefix + "interaction.", keep_vars
             )
         return destination
 
     @property
     def fused_optimizer(self) -> KeyedOptimizer:
         if self.embedding:
-            # pyre-ignore [7]
             return self.embedding.fused_optimizer
         else:
             return CombinedOptimizer([])
 
     def named_parameters(
         self, prefix: str = "", recurse: bool = True, remove_duplicate: bool = True
     ) -> Iterator[Tuple[str, nn.Parameter]]:
@@ -618,22 +613,20 @@
             )
 
         self._cross_dist = KJTAllToAll(
             # pyre-fixme[6]: For 1st param expected `ProcessGroup` but got
             #  `Optional[ProcessGroup]`.
             self._cross_pg,
             self._kjt_num_features_per_pt,
-            self._device,
         )
         self._weighted_cross_dist = KJTAllToAll(
             # pyre-fixme[6]: For 1st param expected `ProcessGroup` but got
             #  `Optional[ProcessGroup]`.
             self._cross_pg,
             self._wkjt_num_features_per_pt,
-            self._device,
         )
 
     # pyre-ignore [14]
     def input_dist(
         self,
         ctx: EmbeddingTowerCollectionContext,
         kjt_features: Optional[KeyedJaggedTensor] = None,
```

## torchrec/distributed/embeddingbag.py

```diff
@@ -46,23 +46,26 @@
 from torchrec.distributed.sharding.twcw_sharding import TwCwPooledEmbeddingSharding
 from torchrec.distributed.sharding.twrw_sharding import TwRwPooledEmbeddingSharding
 from torchrec.distributed.types import (
     Awaitable,
     EmbeddingModuleShardingPlan,
     EnumerableShardingSpec,
     LazyAwaitable,
+    LazyGetItemMixin,
     NullShardedModuleContext,
     ParameterSharding,
     QuantizedCommCodecs,
     ShardedTensor,
     ShardingEnv,
     ShardingType,
 )
 from torchrec.distributed.utils import (
+    add_params_from_parameter_sharding,
     append_prefix,
+    convert_to_fbgemm_types,
     merge_fused_params,
     optimizer_type_to_emb_opt_type,
 )
 from torchrec.modules.embedding_configs import (
     EmbeddingBagConfig,
     EmbeddingTableConfig,
     PoolingType,
@@ -228,15 +231,20 @@
 
         optimizer_class = optimizer_classes[0]
         optimizer_params = optimizer_params[0]
         if optimizer_class:
             optimizer_params["optimizer"] = optimizer_type_to_emb_opt_type(
                 optimizer_class
             )
-        fused_params = merge_fused_params(fused_params, optimizer_params)
+
+        per_table_fused_params = merge_fused_params(fused_params, optimizer_params)
+        per_table_fused_params = add_params_from_parameter_sharding(
+            per_table_fused_params, parameter_sharding
+        )
+        per_table_fused_params = convert_to_fbgemm_types(per_table_fused_params)
 
         sharding_type_to_sharding_infos[parameter_sharding.sharding_type].append(
             EmbeddingShardingInfo(
                 embedding_config=EmbeddingTableConfig(
                     num_embeddings=config.num_embeddings,
                     embedding_dim=config.embedding_dim,
                     name=config.name,
@@ -247,15 +255,15 @@
                     has_feature_processor=False,
                     embedding_names=embedding_names,
                     weight_init_max=config.weight_init_max,
                     weight_init_min=config.weight_init_min,
                 ),
                 param_sharding=parameter_sharding,
                 param=param,
-                fused_params=fused_params,
+                fused_params=per_table_fused_params,
             )
         )
     return sharding_type_to_sharding_infos
 
 
 def _check_need_pos(module: EmbeddingBagCollectionInterface) -> bool:
     for config in module.embedding_bag_configs():
@@ -278,15 +286,17 @@
         keys=embedding_names,
         length_per_key=embedding_dims,
         values=cat_embeddings,
         key_dim=1,
     )
 
 
-class EmbeddingBagCollectionAwaitable(LazyAwaitable[KeyedTensor]):
+class EmbeddingBagCollectionAwaitable(
+    LazyGetItemMixin[str, Tensor], LazyAwaitable[KeyedTensor]
+):
     def __init__(
         self,
         awaitables: List[Awaitable[torch.Tensor]],
         embedding_dims: List[int],
         embedding_names: List[str],
     ) -> None:
         super().__init__()
@@ -396,27 +406,26 @@
         self._features_order: List[int] = []
         # to support the FP16 hook
         self._create_output_dist()
 
         # forward pass flow control
         self._has_uninitialized_input_dist: bool = True
         self._has_features_permute: bool = True
-
         # Get all fused optimizers and combine them.
         optims = []
         for lookup in self._lookups:
-            for _, module in lookup.named_modules():
-                if isinstance(module, FusedOptimizerModule):
+            for _, tbe_module in lookup.named_modules():
+                if isinstance(tbe_module, FusedOptimizerModule):
                     # modify param keys to match EmbeddingBagCollection
                     params: Mapping[str, Union[torch.Tensor, ShardedTensor]] = {}
-                    for param_key, weight in module.fused_optimizer.params.items():
-                        # pyre-fixme[16]: `Mapping` has no attribute `__setitem__`.
+                    for param_key, weight in tbe_module.fused_optimizer.params.items():
+                        # pyre-fixme[16]: `Mapping` has no attribute `__setitem__`
                         params["embedding_bags." + param_key] = weight
-                    module.fused_optimizer.params = params
-                    optims.append(("", module.fused_optimizer))
+                    tbe_module.fused_optimizer.params = params
+                    optims.append(("", tbe_module.fused_optimizer))
         self._optim: CombinedOptimizer = CombinedOptimizer(optims)
 
         for index, (sharding, lookup) in enumerate(
             zip(
                 self._sharding_type_to_sharding.values(),
                 self._lookups,
             )
@@ -431,36 +440,78 @@
                     process_group=env.process_group,
                     gradient_as_bucket_view=True,
                     broadcast_buffers=True,
                     static_graph=True,
                 )
         self._initialize_torch_state()
 
+        # TODO[zainhuda]: support module device coming from CPU
+        if module.device not in [
+            torch.device("meta"),
+            torch.device("cpu"),
+            "meta",
+            "cpu",
+        ]:
+            self.load_state_dict(module.state_dict(), strict=False)
+
     @staticmethod
     def _pre_load_state_dict_hook(
         self: "ShardedEmbeddingBagCollection",
         state_dict: Dict[str, Any],
         prefix: str,
         *args: Any,
     ) -> None:
         """
         Modify the destination state_dict for model parallel
         to transform from ShardedTensors into tensors
         """
-        for table_name in self._model_parallel_name_to_local_shards.keys():
+        for (
+            table_name,
+            model_shards,
+        ) in self._model_parallel_name_to_local_shards.items():
             key = f"{prefix}embedding_bags.{table_name}.weight"
-            local_shards = state_dict[key].local_shards()
-            if len(local_shards) == 0:
-                state_dict[key] = torch.empty(0)
+
+            # If state_dict[key] is already a ShardedTensor, use its local shards
+            if isinstance(state_dict[key], ShardedTensor):
+                local_shards = state_dict[key].local_shards()
+                if len(local_shards) == 0:
+                    state_dict[key] = torch.empty(0)
+                else:
+                    dim = state_dict[key].metadata().shards_metadata[0].shard_sizes[1]
+                    # CW multiple shards are merged
+                    if len(local_shards) > 1:
+                        state_dict[key] = torch.cat(
+                            [s.tensor.view(-1) for s in local_shards], dim=0
+                        ).view(-1, dim)
+                    else:
+                        state_dict[key] = local_shards[0].tensor.view(-1, dim)
+            elif isinstance(state_dict[key], torch.Tensor):
+                local_shards = []
+                for shard in model_shards:
+                    # Extract shard size and offsets for splicing
+                    shard_sizes = shard.metadata.shard_sizes
+                    shard_offsets = shard.metadata.shard_offsets
+
+                    # Prepare tensor by splicing and placing on appropriate device
+                    spliced_tensor = state_dict[key][
+                        shard_offsets[0] : shard_offsets[0] + shard_sizes[0],
+                        shard_offsets[1] : shard_offsets[1] + shard_sizes[1],
+                    ]
+
+                    # Append spliced tensor into local shards
+                    local_shards.append(spliced_tensor)
+                state_dict[key] = (
+                    torch.empty(0)
+                    if not local_shards
+                    else torch.cat(local_shards, dim=0)
+                )
             else:
-                dim = state_dict[key].metadata().shards_metadata[0].shard_sizes[1]
-                # CW multiple shards are merged
-                state_dict[key] = torch.cat(
-                    [s.tensor.view(-1) for s in local_shards], dim=0
-                ).view(-1, dim)
+                raise RuntimeError(
+                    f"Unexpected state_dict key type {type(state_dict[key])} found for {key}"
+                )
 
     def _initialize_torch_state(self) -> None:  # noqa
         """
         This provides consistency between this class and the EmbeddingBagCollection's
         nn.Module API calls (state_dict, named_modules, etc)
         """
         self.embedding_bags: nn.ModuleDict = nn.ModuleDict()
@@ -499,16 +550,14 @@
                     table_name = key[: -len(".weight")]
                     self._model_parallel_name_to_local_shards[table_name].extend(
                         v.local_shards()
                     )
             for (
                 table_name,
                 tbe_slice,
-                # pyre-fixme[16]: Item `Tensor` of `Union[Tensor, Module]` has no
-                #  attribute `named_parameters_by_table`.
             ) in lookup.named_parameters_by_table():
                 self.embedding_bags[table_name].register_parameter("weight", tbe_slice)
         for (
             table_name,
             local_shards,
         ) in self._model_parallel_name_to_local_shards.items():
             # for shards that don't exist on this rank, register with empty tensor
@@ -605,15 +654,14 @@
         if self._has_uninitialized_input_dist:
             self._create_input_dist(features.keys())
             self._has_uninitialized_input_dist = False
         with torch.no_grad():
             if self._has_features_permute:
                 features = features.permute(
                     self._features_order,
-                    # pyre-ignore [6]
                     self._features_order_tensor,
                 )
             features_by_shards = features.split(
                 self._feature_splits,
             )
             awaitables = []
             for input_dist, features_by_shard in zip(
```

## torchrec/distributed/fused_embeddingbag.py

```diff
@@ -71,15 +71,14 @@
                     module=lookup,
                     device_ids=[device],
                     process_group=env.process_group,
                     gradient_as_bucket_view=True,
                     broadcast_buffers=False,
                     static_graph=True,
                 )
-                # pyre-ignore
                 self._lookups[index]._register_fused_optim(
                     optimizer_type, **optimizer_kwargs
                 )
                 # TODO - We need a way to get this optimizer back (and add to optims) so it
                 # can be checkpointed.
                 # We need to ensure that a checkpoint from DDP and a checkpoint from a
                 # model parallel version are compatible.
```

## torchrec/distributed/model_parallel.py

```diff
@@ -228,15 +228,14 @@
             )
             pg = self._env.process_group
             if pg is not None:
                 plan = planner.collective_plan(module, sharders, pg)
             else:
                 plan = planner.plan(module, sharders)
         self._plan: ShardingPlan = plan
-
         self._dmp_wrapped_module: nn.Module = self._init_dmp(module)
         self._optim: CombinedOptimizer = self._init_optim(self._dmp_wrapped_module)
 
         if init_parameters:
             self._init_parameters(self.module)
 
         if init_data_parallel:
@@ -367,15 +366,14 @@
                     has_meta_param = True
             for name, buffer in module._buffers.items():
                 if isinstance(buffer, torch.Tensor) and buffer.device.type == "meta":
                     module._buffers[name] = torch.zeros_like(buffer, device=self.device)
 
             # Init parameters if at least one parameter is over 'meta' device.
             if has_meta_param and hasattr(module, "reset_parameters"):
-                # pyre-ignore [29]
                 module.reset_parameters()
 
         module.apply(init_parameters)
 
     def sparse_grad_parameter_names(
         self, destination: Optional[List[str]] = None, prefix: str = ""
     ) -> List[str]:
```

## torchrec/distributed/quant_embedding.py

```diff
@@ -21,22 +21,28 @@
 from torchrec.distributed.embedding_sharding import EmbeddingSharding
 from torchrec.distributed.embedding_types import (
     BaseQuantEmbeddingSharder,
     FeatureShardingMixIn,
     GroupedEmbeddingConfig,
     KJTList,
     ListOfKJTList,
-    ShardedEmbeddingModule,
     ShardingType,
 )
 from torchrec.distributed.fused_params import (
     FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS,
+    FUSED_PARAM_REGISTER_TBE_BOOL,
     get_tbes_to_register_from_iterable,
+    is_fused_param_quant_state_dict_split_scale_bias,
     is_fused_param_register_tbe,
 )
+from torchrec.distributed.quant_state import ShardedQuantEmbeddingModuleState
+from torchrec.distributed.sharding.rw_sequence_sharding import (
+    InferRwSequenceEmbeddingSharding,
+)
+from torchrec.distributed.sharding.rw_sharding import InferRwSparseFeaturesDist
 from torchrec.distributed.sharding.sequence_sharding import InferSequenceShardingContext
 from torchrec.distributed.sharding.tw_sequence_sharding import (
     InferTwSequenceEmbeddingSharding,
 )
 from torchrec.distributed.types import ParameterSharding, ShardingEnv
 from torchrec.modules.embedding_configs import (
     data_type_to_sparse_type,
@@ -77,75 +83,158 @@
     InferSequenceShardingContext,
     KJTList,
     List[torch.Tensor],
     List[torch.Tensor],
 ]:
     if sharding_type == ShardingType.TABLE_WISE.value:
         return InferTwSequenceEmbeddingSharding(sharding_infos, env, device)
+    elif sharding_type == ShardingType.ROW_WISE.value:
+        return InferRwSequenceEmbeddingSharding(sharding_infos, env, device)
     else:
         raise ValueError(f"Sharding type not supported {sharding_type}")
 
 
-def _construct_jagged_tensors(
-    embeddings: torch.Tensor,
-    features: KeyedJaggedTensor,
-    need_indices: bool = False,
+@torch.fx.wrap
+def _fx_unwrap_optional_tensor(optional: Optional[torch.Tensor]) -> torch.Tensor:
+    assert optional is not None, "Expected optional to be non-None Tensor"
+    return optional
+
+
+def _construct_jagged_tensors_tw(
+    embeddings: List[torch.Tensor],
+    features: KJTList,
+    need_indices: bool,
+) -> Dict[str, JaggedTensor]:
+    ret: Dict[str, JaggedTensor] = {}
+    for i in range(len(embeddings)):
+        embeddings_i: torch.Tensor = embeddings[i]
+        features_i: KeyedJaggedTensor = features[i]
+
+        lengths = features_i.lengths().view(-1, features_i.stride())
+        values = features_i.values()
+        length_per_key = features_i.length_per_key()
+
+        embeddings_list = torch.split(embeddings_i, length_per_key, dim=0)
+        stride = features_i.stride()
+        lengths_tuple = torch.unbind(lengths.view(-1, stride), dim=0)
+        if need_indices:
+            values_list = torch.split(values, length_per_key)
+            for i, key in enumerate(features_i.keys()):
+                ret[key] = JaggedTensor(
+                    lengths=lengths_tuple[i],
+                    values=embeddings_list[i],
+                    weights=values_list[i],
+                )
+        else:
+            for i, key in enumerate(features_i.keys()):
+                ret[key] = JaggedTensor(
+                    lengths=lengths_tuple[i],
+                    values=embeddings_list[i],
+                    weights=None,
+                )
+    return ret
+
+
+def _construct_jagged_tensors_rw(
+    embeddings: List[torch.Tensor],
+    features_before_input_dist: KeyedJaggedTensor,
+    need_indices: bool,
+    unbucketize_tensor: torch.Tensor,
 ) -> Dict[str, JaggedTensor]:
-    # ignore cw consideration for inference now.
     ret: Dict[str, JaggedTensor] = {}
-    lengths = features.lengths().view(-1, features.stride())
-    values = features.values()
-    length_per_key = features.length_per_key()
-
-    embeddings_list = torch.split(embeddings, length_per_key, dim=0)
-    stride = features.stride()
-    lengths_tuple = torch.unbind(lengths.view(-1, stride), dim=0)
+    unbucketized_embs = torch.concat(embeddings, dim=0).index_select(
+        0, unbucketize_tensor
+    )
+    embs_split_per_key = unbucketized_embs.split(
+        features_before_input_dist.length_per_key(), dim=0
+    )
+    stride = features_before_input_dist.stride()
+    lengths_list = torch.unbind(
+        features_before_input_dist.lengths().view(-1, stride), dim=0
+    )
+    values_list: List[torch.Tensor] = []
     if need_indices:
-        values_list = torch.split(values, length_per_key)
-        for i, key in enumerate(features.keys()):
-            ret[key] = JaggedTensor(
-                lengths=lengths_tuple[i],
-                values=embeddings_list[i],
-                weights=values_list[i],
-            )
-    else:
-        for i, key in enumerate(features.keys()):
-            ret[key] = JaggedTensor(
-                lengths=lengths_tuple[i],
-                values=embeddings_list[i],
-                weights=None,
-            )
+        # pyre-ignore
+        values_list = torch.split(
+            features_before_input_dist.values(),
+            features_before_input_dist.length_per_key(),
+        )
+    for i, key in enumerate(features_before_input_dist.keys()):
+        ret[key] = JaggedTensor(
+            values=embs_split_per_key[i],
+            lengths=lengths_list[i],
+            weights=values_list[i] if need_indices else None,
+        )
     return ret
 
 
+def _construct_jagged_tensors(
+    embeddings: List[torch.Tensor],
+    features: KJTList,
+    embedding_names_per_rank: List[List[str]],
+    features_before_input_dist: KeyedJaggedTensor,
+    need_indices: bool,
+    unbucketize_tensor: Optional[torch.Tensor],
+    features_to_permute_indices: Dict[str, torch.Tensor],
+) -> Dict[str, JaggedTensor]:
+    if unbucketize_tensor is not None:
+        # RW sharding
+        return _construct_jagged_tensors_rw(
+            embeddings,
+            features_before_input_dist,
+            need_indices,
+            unbucketize_tensor,
+        )
+
+    return _construct_jagged_tensors_tw(embeddings, features, need_indices)
+
+
 @torch.fx.wrap
 def output_jt_dict(
     emb_per_sharding: List[List[torch.Tensor]],
     features_per_sharding: List[KJTList],
+    embedding_names_per_rank_per_sharding: List[List[List[str]]],
     need_indices: bool,
+    features_before_input_dist_per_sharding: List[KeyedJaggedTensor],
+    features_to_permute_indices: Dict[str, torch.Tensor],
+    unbucketize_tensors: List[torch.Tensor],
+    unbucketize_tensor_idxs_per_sharding: List[int],
 ) -> Dict[str, JaggedTensor]:
     jt_dict: Dict[str, JaggedTensor] = {}
-    for emb_sharding, f_sharding in zip(
+    for (
+        emb_sharding,
+        features_sharding,
+        embedding_names_per_rank,
+        unbucketize_tensor_idx,
+        features_before_input_dist,
+    ) in zip(
         emb_per_sharding,
         features_per_sharding,
+        embedding_names_per_rank_per_sharding,
+        unbucketize_tensor_idxs_per_sharding,
+        features_before_input_dist_per_sharding,
     ):
-        # Can not use zip here as Iterator of KJTList is not supported by jit
-        for i in range(len(emb_sharding)):
-            jt_dict.update(
-                _construct_jagged_tensors(
-                    embeddings=emb_sharding[i],
-                    features=f_sharding[i],
-                    need_indices=need_indices,
-                )
+        jt_dict.update(
+            _construct_jagged_tensors(
+                embeddings=emb_sharding,
+                features=features_sharding,
+                embedding_names_per_rank=embedding_names_per_rank,
+                features_before_input_dist=features_before_input_dist,
+                need_indices=need_indices,
+                unbucketize_tensor=unbucketize_tensors[unbucketize_tensor_idx]
+                if unbucketize_tensor_idx != -1
+                else None,
+                features_to_permute_indices=features_to_permute_indices,
             )
+        )
     return jt_dict
 
 
 class ShardedQuantEmbeddingCollection(
-    ShardedEmbeddingModule[
+    ShardedQuantEmbeddingModuleState[
         ListOfKJTList,
         List[List[torch.Tensor]],
         Dict[str, JaggedTensor],
         EmbeddingCollectionContext,
     ],
 ):
     """
@@ -177,14 +266,24 @@
             ],
         ] = {
             sharding_type: create_infer_embedding_sharding(
                 sharding_type, embedding_confings, env
             )
             for sharding_type, embedding_confings in sharding_type_to_sharding_infos.items()
         }
+        self._embedding_dim: int = module.embedding_dim()
+        self._local_embedding_dim: int = self._embedding_dim
+        self._embedding_names_per_sharding: List[List[str]] = []
+        self._embedding_names_per_rank_per_sharding: List[List[List[str]]] = []
+        for sharding in self._sharding_type_to_sharding.values():
+            self._embedding_names_per_sharding.append(sharding.embedding_names())
+            self._embedding_names_per_rank_per_sharding.append(
+                sharding.embedding_names_per_rank()
+            )
+        self._features_to_permute_indices: Dict[str, torch.Tensor] = {}
 
         self._device = device
         self._input_dists: List[nn.Module] = []
         self._lookups: List[nn.Module] = []
         self._create_lookups(fused_params, device)
         self._output_dists: List[nn.Module] = []
 
@@ -195,53 +294,58 @@
         self._has_uninitialized_output_dist: bool = True
 
         self._embedding_dim: int = module.embedding_dim()
         self._need_indices: bool = module.need_indices()
 
         self._fused_params = fused_params
 
-        # This provides consistency between this class and the EmbeddingBagCollection's
-        # nn.Module API calls (state_dict, named_modules, etc)
-        # Currently, Sharded Quant EC only uses TW sharding, and returns non-sharded tensors as part of state dict
-        # TODO - revisit if we state_dict can be represented as sharded tensor
-        self.embeddings: nn.ModuleDict = nn.ModuleDict()
-        for table in self._embedding_configs:
-            self.embeddings[table.name] = torch.nn.Module()
-
-        for _sharding_type, lookup in zip(
-            self._sharding_type_to_sharding.keys(), self._lookups
-        ):
-            lookup_state_dict = lookup.state_dict()
-            for key in lookup_state_dict:
-                if key.endswith(".weight"):
-                    table_name = key[: -len(".weight")]
-                    # Register as buffer because this is an inference model, and can potentially use uint8 types.
-                    self.embeddings[table_name].register_buffer(
-                        "weight", lookup_state_dict[key]
-                    )
-                elif key.endswith(".weight_qscale"):
-                    table_name = key[: -len(".weight_qscale")]
-                    self.embeddings[table_name].register_buffer(
-                        "weight_qscale", lookup_state_dict[key]
-                    )
-                elif key.endswith(".weight_qbias"):
-                    table_name = key[: -len(".weight_qbias")]
-                    self.embeddings[table_name].register_buffer(
-                        "weight_qbias", lookup_state_dict[key]
-                    )
-                else:
-                    continue
+        tbes: Dict[
+            IntNBitTableBatchedEmbeddingBagsCodegen, GroupedEmbeddingConfig
+        ] = get_tbes_to_register_from_iterable(self._lookups)
 
         # Optional registration of TBEs for model post processing utilities
         if is_fused_param_register_tbe(fused_params):
-            tbes: Dict[
-                IntNBitTableBatchedEmbeddingBagsCodegen, GroupedEmbeddingConfig
-            ] = get_tbes_to_register_from_iterable(self._lookups)
             self.tbes: torch.nn.ModuleList = torch.nn.ModuleList(tbes.keys())
 
+        quant_state_dict_split_scale_bias = (
+            is_fused_param_quant_state_dict_split_scale_bias(fused_params)
+        )
+
+        if quant_state_dict_split_scale_bias:
+            self._initialize_torch_state(
+                tbes=tbes,
+                table_name_to_parameter_sharding=table_name_to_parameter_sharding,
+                tables_weights_prefix="embeddings",
+            )
+        else:
+            table_wise_sharded_only: bool = all(
+                [
+                    sharding_type == ShardingType.TABLE_WISE.value
+                    for sharding_type in self._sharding_type_to_sharding.keys()
+                ]
+            )
+            assert (
+                table_wise_sharded_only
+            ), "ROW_WISE,COLUMN_WISE shardings can be used only in 'quant_state_dict_split_scale_bias' mode, specify fused_params[FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS]=True to __init__ argument"
+
+            self.embeddings: nn.ModuleDict = nn.ModuleDict()
+            for table in self._embedding_configs:
+                self.embeddings[table.name] = torch.nn.Module()
+
+            for _sharding_type, lookup in zip(
+                self._sharding_type_to_sharding.keys(), self._lookups
+            ):
+                lookup_state_dict = lookup.state_dict()
+                for key in lookup_state_dict:
+                    if key.endswith(".weight"):
+                        table_name = key[: -len(".weight")]
+                        self.embeddings[table_name].register_buffer(
+                            "weight", lookup_state_dict[key]
+                        )
+
     def _create_input_dist(
         self,
         input_feature_names: List[str],
         device: torch.device,
         input_dist_device: Optional[torch.device] = None,
     ) -> None:
         feature_names: List[str] = []
@@ -296,65 +400,96 @@
                 device=features.device(),
                 input_dist_device=self._device,
             )
             self._has_uninitialized_input_dist = False
         if self._has_uninitialized_output_dist:
             self._create_output_dist(features.device())
             self._has_uninitialized_output_dist = False
+        ret: List[KJTList] = []
         with torch.no_grad():
             features_by_sharding = []
             if self._features_order:
                 features = features.permute(
                     self._features_order,
-                    # pyre-ignore [6]
                     self._features_order_tensor,
                 )
             features_by_sharding = features.split(
                 self._feature_splits,
             )
 
-            return ListOfKJTList(
-                [
-                    self._input_dists[i].forward(features_by_sharding[i])
-                    for i in range(len(self._input_dists))
-                ]
-            )
+            for i in range(len(self._input_dists)):
+                input_dist = self._input_dists[i]
+                input_dist_result = input_dist.forward(features_by_sharding[i])
+                ret.append(input_dist_result)
+                ctx.sharding_contexts.append(
+                    InferSequenceShardingContext(
+                        features=input_dist_result,
+                        features_before_input_dist=features,
+                        unbucketize_permute_tensor=input_dist.unbucketize_permute_tensor
+                        if isinstance(input_dist, InferRwSparseFeaturesDist)
+                        else None,
+                    )
+                )
+        return ListOfKJTList(ret)
 
     def compute(
         self, ctx: EmbeddingCollectionContext, dist_input: ListOfKJTList
     ) -> List[List[torch.Tensor]]:
         ret: List[List[torch.Tensor]] = []
+
         for lookup, features in zip(
             self._lookups,
             dist_input,
         ):
-            ctx.sharding_contexts.append(InferSequenceShardingContext(features))
             ret.append(
                 [o.view(-1, self._embedding_dim) for o in lookup.forward(features)]
             )
         return ret
 
     # pyre-ignore
     def output_dist(
         self, ctx: EmbeddingCollectionContext, output: List[List[torch.Tensor]]
     ) -> Dict[str, JaggedTensor]:
         emb_per_sharding: List[List[torch.Tensor]] = []
-        features_per_sharding: List[List[KeyedJaggedTensor]] = []
-        for odist, embeddings, sharding_ctx in zip(
+        features_before_input_dist_per_sharding: List[KeyedJaggedTensor] = []
+        features_per_sharding: List[KJTList] = []
+        unbucketize_tensor_idxs_per_sharding: List[int] = []
+        unbucketize_tensors: List[torch.Tensor] = []
+        for sharding_output_dist, embeddings, sharding_ctx in zip(
             self._output_dists,
             output,
             ctx.sharding_contexts,
         ):
-            emb_per_sharding.append(odist.forward(embeddings, sharding_ctx))
-            # pyre-fixme[6]: For 1st argument expected `List[KeyedJaggedTensor]` but
-            #  got `Optional[KJTList]`.
+            sharding_output_dist_res: List[torch.Tensor] = sharding_output_dist.forward(
+                embeddings, sharding_ctx
+            )
+            emb_per_sharding.append(sharding_output_dist_res)
             features_per_sharding.append(sharding_ctx.features)
-
+            if sharding_ctx.unbucketize_permute_tensor is None:
+                unbucketize_tensor_idxs_per_sharding.append(-1)
+            else:
+                unbucketize_tensors.append(
+                    _fx_unwrap_optional_tensor(sharding_ctx.unbucketize_permute_tensor)
+                )
+                unbucketize_tensor_idxs_per_sharding.append(
+                    len(unbucketize_tensors) - 1
+                )
+            features_before_input_dist_per_sharding.append(
+                # pyre-ignore
+                sharding_ctx.features_before_input_dist
+            )
         return output_jt_dict(
-            emb_per_sharding, features_per_sharding, self._need_indices
+            emb_per_sharding=emb_per_sharding,
+            features_per_sharding=features_per_sharding,
+            embedding_names_per_rank_per_sharding=self._embedding_names_per_rank_per_sharding,
+            need_indices=self._need_indices,
+            features_before_input_dist_per_sharding=features_before_input_dist_per_sharding,
+            unbucketize_tensor_idxs_per_sharding=unbucketize_tensor_idxs_per_sharding,
+            unbucketize_tensors=unbucketize_tensors,
+            features_to_permute_indices=self._features_to_permute_indices,
         )
 
     # pyre-ignore
     def compute_and_output_dist(
         self, ctx: EmbeddingCollectionContext, input: ListOfKJTList
     ) -> Dict[str, JaggedTensor]:
         return self.output_dist(ctx, self.compute(ctx, input))
@@ -394,15 +529,26 @@
         env: ShardingEnv,
         device: Optional[torch.device] = None,
     ) -> ShardedQuantEmbeddingCollection:
         fused_params = self.fused_params if self.fused_params else {}
         fused_params["output_dtype"] = data_type_to_sparse_type(
             dtype_to_data_type(module.output_dtype())
         )
-        fused_params[FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS] = getattr(
-            module, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, False
+        if FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS not in fused_params:
+            fused_params[FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS] = getattr(
+                module, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, False
+            )
+        if FUSED_PARAM_REGISTER_TBE_BOOL not in fused_params:
+            fused_params[FUSED_PARAM_REGISTER_TBE_BOOL] = getattr(
+                module, FUSED_PARAM_REGISTER_TBE_BOOL, False
+            )
+        return ShardedQuantEmbeddingCollection(
+            module=module,
+            table_name_to_parameter_sharding=params,
+            env=env,
+            fused_params=fused_params,
+            device=device,
         )
-        return ShardedQuantEmbeddingCollection(module, params, env, fused_params)
 
     @property
     def module_type(self) -> Type[QuantEmbeddingCollection]:
         return QuantEmbeddingCollection
```

## torchrec/distributed/quant_embedding_kernel.py

```diff
@@ -110,14 +110,21 @@
         quant_weight = quantized_weights[:, :-4]
         scale_shift = quantized_weights[:, -4:]
 
         quant_weight_list.append((quant_weight, scale_shift))
     return quant_weight_list
 
 
+@torch.fx.wrap
+def _unwrap_kjt(
+    features: KeyedJaggedTensor,
+) -> Tuple[torch.Tensor, torch.Tensor, Optional[torch.Tensor]]:
+    return features.values().int(), features.offsets().int(), features.weights_or_none()
+
+
 class QuantBatchedEmbeddingBag(
     BaseBatchedEmbeddingBag[
         Tuple[torch.Tensor, Optional[torch.Tensor], Optional[torch.Tensor]]
     ],
     TBEToRegisterMixIn,
 ):
     def __init__(
@@ -178,29 +185,30 @@
 
     def get_tbes_to_register(
         self,
     ) -> Dict[IntNBitTableBatchedEmbeddingBagsCodegen, GroupedEmbeddingConfig]:
         return {self._emb_module: self._config}
 
     def forward(self, features: KeyedJaggedTensor) -> torch.Tensor:
+        indices, offsets, per_sample_weights = _unwrap_kjt(features)
         # Conditional call of .forward function for FX:
         # emb_module() can go through FX only if emb_module is registered in named_modules (FX node call_module)
         # emb_module.forward() does not require registering emb_module in named_modules (FX node call_function)
         # For some post processing that requires TBE emb_module copied in fx.GraphModule we need to be call_module, as it will copies this module inside fx.GraphModule unchanged.
         if self._emb_module_registered:
             return self.emb_module(
-                indices=features.values().int(),
-                offsets=features.offsets().int(),
-                per_sample_weights=features.weights_or_none(),
+                indices=indices,
+                offsets=offsets,
+                per_sample_weights=per_sample_weights,
             )
         else:
             return self.emb_module.forward(
-                indices=features.values().int(),
-                offsets=features.offsets().int(),
-                per_sample_weights=features.weights_or_none(),
+                indices=indices,
+                offsets=offsets,
+                per_sample_weights=per_sample_weights,
             )
 
     def named_buffers(
         self, prefix: str = "", recurse: bool = True, remove_duplicate: bool = True
     ) -> Iterator[Tuple[str, torch.Tensor]]:
         assert (
             remove_duplicate
@@ -234,15 +242,14 @@
 
     @classmethod
     def from_float(cls, module: BaseEmbedding) -> "QuantBatchedEmbeddingBag":
         assert hasattr(
             module, "qconfig"
         ), "BaseEmbedding input float module must have qconfig defined"
 
-        # pyre-ignore [16]
         data_type = dtype_to_data_type(module.qconfig.weight().dtype)
         sparse_type = data_type_to_sparse_type(data_type)
 
         # TODO Can we simplify this with state_dict = module.state_dict()?
         state_dict = (
             dict(module.named_split_embedding_weights())
             if isinstance(module, BatchedDenseEmbeddingBag)
@@ -333,23 +340,24 @@
                 split_scale_bias_mode=2
                 if self._quant_state_dict_split_scale_bias
                 else 0
             )
         ]
 
     def forward(self, features: KeyedJaggedTensor) -> torch.Tensor:
+        values, offsets, _ = _unwrap_kjt(features)
         if self._emb_module_registered:
             return self.emb_module(
-                indices=features.values().int(),
-                offsets=features.offsets().int(),
+                indices=values,
+                offsets=offsets,
             )
         else:
             return self.emb_module.forward(
-                indices=features.values().int(),
-                offsets=features.offsets().int(),
+                indices=values,
+                offsets=offsets,
             )
 
     def named_buffers(
         self, prefix: str = "", recurse: bool = True, remove_duplicate: bool = True
     ) -> Iterator[Tuple[str, torch.Tensor]]:
         for config, (weight, weight_qscale, weight_qbias) in zip(
             self._config.embedding_tables,
@@ -368,15 +376,14 @@
 
     @classmethod
     def from_float(cls, module: BaseEmbedding) -> "QuantBatchedEmbedding":
         assert hasattr(
             module, "qconfig"
         ), "BaseEmbedding input float module must have qconfig defined"
 
-        # pyre-ignore [16]
         data_type = dtype_to_data_type(module.qconfig.weight().dtype)
         sparse_type = data_type_to_sparse_type(data_type)
 
         # TODO Can we simplify this with state_dict = module.state_dict()?
         state_dict = (
             dict(module.named_split_embedding_weights())
             if isinstance(module, BatchedDenseEmbedding)
```

## torchrec/distributed/quant_embeddingbag.py

```diff
@@ -18,25 +18,29 @@
 )
 from torchrec.distributed.embedding_types import (
     BaseQuantEmbeddingSharder,
     FeatureShardingMixIn,
     GroupedEmbeddingConfig,
     KJTList,
     ListOfKJTList,
-    ShardedEmbeddingModule,
 )
 from torchrec.distributed.embeddingbag import (
     construct_output_kt,
     create_sharding_infos_by_sharding,
 )
 from torchrec.distributed.fused_params import (
     FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS,
+    FUSED_PARAM_REGISTER_TBE_BOOL,
     get_tbes_to_register_from_iterable,
+    is_fused_param_quant_state_dict_split_scale_bias,
     is_fused_param_register_tbe,
 )
+from torchrec.distributed.quant_state import ShardedQuantEmbeddingModuleState
+from torchrec.distributed.sharding.cw_sharding import InferCwPooledEmbeddingSharding
+from torchrec.distributed.sharding.rw_sharding import InferRwPooledEmbeddingSharding
 from torchrec.distributed.sharding.tw_sharding import InferTwEmbeddingSharding
 from torchrec.distributed.types import (
     NullShardedModuleContext,
     NullShardingContext,
     ParameterSharding,
     ShardingEnv,
     ShardingType,
@@ -59,20 +63,26 @@
 def create_infer_embedding_bag_sharding(
     sharding_type: str,
     sharding_infos: List[EmbeddingShardingInfo],
     env: ShardingEnv,
 ) -> EmbeddingSharding[NullShardingContext, KJTList, List[torch.Tensor], torch.Tensor]:
     if sharding_type == ShardingType.TABLE_WISE.value:
         return InferTwEmbeddingSharding(sharding_infos, env, device=None)
+    elif sharding_type == ShardingType.ROW_WISE.value:
+        return InferRwPooledEmbeddingSharding(sharding_infos, env, device=None)
+    elif sharding_type == ShardingType.COLUMN_WISE.value:
+        return InferCwPooledEmbeddingSharding(
+            sharding_infos, env, device=None, permute_embeddings=True
+        )
     else:
         raise ValueError(f"Sharding type not supported {sharding_type}")
 
 
 class ShardedQuantEmbeddingBagCollection(
-    ShardedEmbeddingModule[
+    ShardedQuantEmbeddingModuleState[
         ListOfKJTList,
         List[List[torch.Tensor]],
         KeyedTensor,
         NullShardedModuleContext,
     ],
 ):
     """
@@ -121,54 +131,58 @@
         self._features_order: List[int] = []
 
         # forward pass flow control
         self._has_uninitialized_input_dist: bool = True
         self._has_uninitialized_output_dist: bool = True
         self._has_features_permute: bool = True
 
-        # This provides consistency between this class and the EmbeddingBagCollection's
-        # nn.Module API calls (state_dict, named_modules, etc)
-        # Currently, Sharded Quant EBC only uses TW sharding, and returns non-sharded tensors as part of state dict
-        # TODO - revisit if we state_dict can be represented as sharded tensor
-        self.embedding_bags: nn.ModuleDict = nn.ModuleDict()
-        for table in self._embedding_bag_configs:
-            self.embedding_bags[table.name] = torch.nn.Module()
-
-        for _sharding_type, lookup in zip(
-            self._sharding_type_to_sharding.keys(), self._lookups
-        ):
-            lookup_state_dict = lookup.state_dict()
-            for key in lookup_state_dict:
-                if key.endswith(".weight"):
-                    table_name = key[: -len(".weight")]
-                    # Register as buffer because this is an inference model, and can potentially use uint8 types.
-                    self.embedding_bags[table_name].register_buffer(
-                        "weight", lookup_state_dict[key]
-                    )
-                elif key.endswith("weight_qscale"):
-                    table_name = key[: -len(".weight_qscale")]
-                    self.embedding_bags[table_name].register_buffer(
-                        "weight_qscale", lookup_state_dict[key]
-                    )
-                elif key.endswith("weight_qbias"):
-                    table_name = key[: -len(".weight_qbias")]
-                    self.embedding_bags[table_name].register_buffer(
-                        "weight_qbias", lookup_state_dict[key]
-                    )
-                else:
-                    continue
+        tbes: Dict[
+            IntNBitTableBatchedEmbeddingBagsCodegen, GroupedEmbeddingConfig
+        ] = get_tbes_to_register_from_iterable(self._lookups)
 
         # Optional registration of TBEs for model post processing utilities
         if is_fused_param_register_tbe(fused_params):
-            tbes: Dict[
-                IntNBitTableBatchedEmbeddingBagsCodegen, GroupedEmbeddingConfig
-            ] = get_tbes_to_register_from_iterable(self._lookups)
-
             self.tbes: torch.nn.ModuleList = torch.nn.ModuleList(tbes.keys())
 
+        quant_state_dict_split_scale_bias = (
+            is_fused_param_quant_state_dict_split_scale_bias(fused_params)
+        )
+
+        if quant_state_dict_split_scale_bias:
+            self._initialize_torch_state(
+                tbes=tbes,
+                table_name_to_parameter_sharding=table_name_to_parameter_sharding,
+                tables_weights_prefix="embedding_bags",
+            )
+        else:
+            table_wise_sharded_only: bool = all(
+                [
+                    sharding_type == ShardingType.TABLE_WISE.value
+                    for sharding_type in self._sharding_type_to_sharding.keys()
+                ]
+            )
+            assert (
+                table_wise_sharded_only
+            ), "ROW_WISE,COLUMN_WISE shardings can be used only in 'quant_state_dict_split_scale_bias' mode, specify fused_params[FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS]=True to __init__ argument"
+
+            self.embedding_bags: nn.ModuleDict = nn.ModuleDict()
+            for table in self._embedding_bag_configs:
+                self.embedding_bags[table.name] = torch.nn.Module()
+
+            for _sharding_type, lookup in zip(
+                self._sharding_type_to_sharding.keys(), self._lookups
+            ):
+                lookup_state_dict = lookup.state_dict()
+                for key in lookup_state_dict:
+                    if key.endswith(".weight"):
+                        table_name = key[: -len(".weight")]
+                        self.embedding_bags[table_name].register_buffer(
+                            "weight", lookup_state_dict[key]
+                        )
+
     def _create_input_dist(
         self,
         input_feature_names: List[str],
         features_device: torch.device,
         input_dist_device: Optional[torch.device] = None,
     ) -> None:
         feature_names: List[str] = []
@@ -226,15 +240,14 @@
         if self._has_uninitialized_output_dist:
             self._create_output_dist(features.device())
             self._has_uninitialized_output_dist = False
         with torch.no_grad():
             if self._has_features_permute:
                 features = features.permute(
                     self._features_order,
-                    # pyre-ignore [6]
                     self._features_order_tensor,
                 )
             features_by_shards = features.split(self._feature_splits)
             return ListOfKJTList(
                 [
                     self._input_dists[i].forward(features_by_shards[i])
                     for i in range(len(self._input_dists))
@@ -300,15 +313,23 @@
         env: ShardingEnv,
         device: Optional[torch.device] = None,
     ) -> ShardedQuantEmbeddingBagCollection:
         fused_params = self.fused_params if self.fused_params else {}
         fused_params["output_dtype"] = data_type_to_sparse_type(
             dtype_to_data_type(module.output_dtype())
         )
-        fused_params[FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS] = getattr(
-            module, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, False
+        if FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS not in fused_params:
+            fused_params[FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS] = getattr(
+                module, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, False
+            )
+        if FUSED_PARAM_REGISTER_TBE_BOOL not in fused_params:
+            fused_params[FUSED_PARAM_REGISTER_TBE_BOOL] = getattr(
+                module, FUSED_PARAM_REGISTER_TBE_BOOL, False
+            )
+
+        return ShardedQuantEmbeddingBagCollection(
+            module, params, env, fused_params, device=device
         )
-        return ShardedQuantEmbeddingBagCollection(module, params, env, fused_params)
 
     @property
     def module_type(self) -> Type[QuantEmbeddingBagCollection]:
         return QuantEmbeddingBagCollection
```

## torchrec/distributed/sharding_plan.py

```diff
@@ -4,14 +4,15 @@
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 #!/usr/bin/env python3
 
 import math
+import warnings
 from typing import Callable, cast, Dict, List, Optional, Tuple, Type
 
 import torch
 from torch import distributed as dist, nn
 from torchrec.distributed.comm import get_local_size
 from torchrec.distributed.embedding import EmbeddingCollectionSharder
 from torchrec.distributed.embedding_types import EmbeddingComputeKernel
@@ -147,19 +148,25 @@
     columns: int,
     rows: int,
     col_wise_shard_dim: Optional[int] = None,
 ) -> Tuple[List[List[int]], List[List[int]]]:
     block_size: int = min(
         col_wise_shard_dim if col_wise_shard_dim else MIN_CW_DIM, columns
     )
-    num_col_wise_shards, residual = divmod(columns, block_size)
 
-    shard_sizes: List[List[int]] = [[rows, block_size]] * (num_col_wise_shards - 1)
-    shard_sizes.append([rows, block_size + residual])
+    if columns % block_size != 0:
+        warnings.warn(
+            f"Dim of {columns} cannot be evenly divided with column wise shard dim {col_wise_shard_dim}, overriding block_size to embedding_dim={columns}",
+            UserWarning,
+        )
+        block_size = columns
 
+    num_col_wise_shards, _residual = divmod(columns, block_size)
+
+    shard_sizes: List[List[int]] = [[rows, block_size]] * num_col_wise_shards
     shard_offsets: List[List[int]] = [
         [0, block_size * rank] for rank in range(num_col_wise_shards)
     ]
     return shard_sizes, shard_offsets
 
 
 def _get_parameter_size_offsets(
```

## torchrec/distributed/train_pipeline.py

```diff
@@ -7,14 +7,15 @@
 
 """
 NOTE: Due to an internal packaging issue, `train_pipeline.py` must be compatible with
 older versions of TorchRec. Importing new modules from other files may break model
 publishing flows.
 """
 import abc
+import copy
 import itertools
 import logging
 from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import (
     Any,
     cast,
@@ -598,14 +599,18 @@
             continue
         while True:
             if not isinstance(arg, torch.fx.Node):
                 break
             child_node = arg
 
             if child_node.op == "placeholder":
+                if hasattr(child_node, "ph_key"):
+                    # pyre-ignore[16]
+                    arg_info.input_attrs.insert(0, child_node.ph_key)
+                    arg_info.is_getitems.insert(0, False)
                 num_found += 1
                 break
             # skip this fp node
             elif (
                 feature_processor_arguments is not None
                 and child_node in feature_processor_arguments
             ):
@@ -656,60 +661,96 @@
     for name, arg_info_list in zip(node.kwargs, kwargs_arg_info_list):
         arg_info_list.name = name
 
     arg_info_list = pos_arg_info_list + kwargs_arg_info_list
     return arg_info_list, num_found
 
 
-def _get_unsharded_module_names_helper(
+def _get_leaf_module_names_helper(
     model: torch.nn.Module,
     path: str,
-    unsharded_module_names: Set[str],
+    leaf_module_names: Set[str],
 ) -> bool:
     sharded_children = set()
     for name, child in model.named_children():
         curr_path = path + name
         if isinstance(child, ShardedModule):
             sharded_children.add(name)
         else:
-            child_sharded = _get_unsharded_module_names_helper(
+            child_sharded = _get_leaf_module_names_helper(
                 child,
                 curr_path + ".",
-                unsharded_module_names,
+                leaf_module_names,
             )
             if child_sharded:
                 sharded_children.add(name)
 
     if len(sharded_children) > 0:
-        for name, _ in model.named_children():
-            if name not in sharded_children:
-                unsharded_module_names.add(path + name)
-
+        for name, child in model.named_children():
+            if name in sharded_children:
+                continue
+            # assume module is leaf node unless annotated otherwise
+            if not getattr(child, "_is_pytorch_fx_traceable", False):
+                leaf_module_names.add(path + name)
     return len(sharded_children) > 0
 
 
-def _get_unsharded_module_names(model: torch.nn.Module) -> List[str]:
+def _get_leaf_module_names(model: torch.nn.Module) -> List[str]:
     """
-    Returns a list of top level modules do not contain any sharded sub modules.
+    Returns a list of top level modules to be used as leaf modules for FX tracing.
+    This is a shallow FX trace that only goes the minimum depth required to pipeline
+    the model unless child modules are explicitly tagged as `_is_pytorch_fx_traceable`.
     """
 
-    unsharded_module_names: Set[str] = set()
-    _get_unsharded_module_names_helper(
+    leaf_module_names: Set[str] = set()
+    _get_leaf_module_names_helper(
         model,
         "",
-        unsharded_module_names,
+        leaf_module_names,
     )
-    return list(unsharded_module_names)
+    return list(leaf_module_names)
+
+
+def _jit_modules(module: torch.nn.Module, path: str, optional: bool = True) -> bool:
+    sharded_children = set()
+    for name, child in module.named_children():
+        curr_path = path + name
+        if isinstance(child, ShardedModule):
+            sharded_children.add(name)
+        else:
+            child_sharded = _jit_modules(child, curr_path + ".", optional)
+            if child_sharded:
+                sharded_children.add(name)
+
+    if len(sharded_children) > 0:
+        for name, child in module.named_children():
+            if name not in sharded_children:
+                try:
+                    jit_child = torch.jit.script(child)
+                    setattr(module, name, jit_child)
+                    logger.info(f"jit.script applied to {path + name}.")
+                except Exception as error:
+                    if not optional:
+                        raise
+                    else:
+                        logger.info(
+                            f"Warning: failed to jit.script {path + name}: {error}."
+                        )
+
+    return len(sharded_children) > 0
 
 
 def _rewrite_model(  # noqa C901
     model: torch.nn.Module,
     context: TrainPipelineContext,
     dist_stream: Optional[torch.cuda.streams.Stream],
-) -> List[ShardedModule]:
+    batch: Optional[In] = None,
+    apply_jit: bool = False,
+) -> Tuple[List[ShardedModule], torch.nn.Module]:
+    input_model = model
     # Get underlying nn.Module
     if isinstance(model, DistributedModelParallel):
         model = model.module
 
     # Collect feature processors.
     for _, m in model.named_modules():
         if isinstance(m, BaseGroupedFeatureProcessor):
@@ -723,44 +764,67 @@
     for name, m in model.named_modules():
         if isinstance(m, ShardedModule):
             sharded_modules[name] = m
         if isinstance(m, BaseGroupedFeatureProcessor):
             fp_modules[name] = m
 
     # Trace a model.
-    tracer = Tracer(leaf_modules=_get_unsharded_module_names(model))
-    graph = tracer.trace(model)
+    concrete_args = (
+        # pyre-ignore[16]
+        {"inputs": copy.copy(batch).to_proxy()}
+        if batch and hasattr(batch, "to_proxy")
+        else {}
+    )
+    tracer = Tracer(leaf_modules=_get_leaf_module_names(model))
+    graph = tracer.trace(model, concrete_args=concrete_args)
 
     feature_processor_nodes = []
-    # find the fp node
+    # Find the fp node
     for node in graph.nodes:
         if node.op == "call_module" and node.target in fp_modules:
             feature_processor_nodes.append(node)
+
     # Select sharded modules, which are top-level in the forward call graph,
-    # i.e. which don't have input transformations, i.e.
-    # rely only on 'builtins.getattr'.
-    ret = []
+    # i.e. don't have input transformations, i.e. rely only on 'builtins.getattr'.
+    pipelined_forwards = []
     for node in graph.nodes:
         if node.op == "call_module" and node.target in sharded_modules:
             total_num_args = len(node.args) + len(node.kwargs)
             if total_num_args == 0:
                 continue
             arg_info_list, num_found = _get_node_args(node, feature_processor_nodes)
+            if hasattr(model, "_fx_trace_sparse_arg_info"):
+                # the model already provide the arg info, use that to avoid the graph
+                # input already flattened so cannot extract that information
+                # pyre-ignore
+                arg_info_list: List[ArgInfo] = model._fx_trace_sparse_arg_info
+                assert num_found == len(
+                    arg_info_list
+                ), "the number of args doesn't match the fx trace arg info provided in the model"
+
             if num_found == total_num_args:
                 logger.info(f"Module '{node.target}'' will be pipelined")
                 child = sharded_modules[node.target]
                 child.forward = PipelinedForward(
                     node.target,
                     arg_info_list,
                     child,
                     context,
                     dist_stream,
                 )
-                ret.append(child)
-    return ret
+                pipelined_forwards.append(child)
+
+    # JIT script unsharded modules if applicable.
+    if apply_jit:
+        graph_model = torch.fx.GraphModule(model, graph)
+        _jit_modules(graph_model, "")
+        if isinstance(input_model, DistributedModelParallel):
+            input_model.module = graph_model
+
+    return pipelined_forwards, input_model
 
 
 def _override_input_dist_forwards(pipelined_modules: List[ShardedModule]) -> None:
     """
     Overrides each input dist forward to support fusing the splits collective.
     NOTE: this can only be called after the input dists are initialized.
     """
@@ -804,27 +868,30 @@
     Args:
         model (torch.nn.Module): model to pipeline.
         optimizer (torch.optim.Optimizer): optimizer to use.
         device (torch.device): device where device transfer, sparse data dist, and
             forward/backward pass will happen.
         execute_all_batches (bool): executes remaining batches in pipeline after
             exhausting dataloader iterator.
+        apply_jit (bool): apply torch.jit.script to non-pipelined (unsharded) modules.
     """
 
     def __init__(
         self,
         model: torch.nn.Module,
         optimizer: torch.optim.Optimizer,
         device: torch.device,
         execute_all_batches: bool = True,
+        apply_jit: bool = False,
     ) -> None:
         self._model = model
         self._optimizer = optimizer
         self._device = device
         self._execute_all_batches = execute_all_batches
+        self._apply_jit = apply_jit
         # use two data streams to support two concurrent batches
         if device.type == "cuda":
             self._memcpy_stream: Optional[
                 torch.cuda.streams.Stream
             ] = torch.cuda.Stream(priority=-1)
             self._data_dist_stream: Optional[
                 torch.cuda.streams.Stream
@@ -896,16 +963,20 @@
         """
         Retrieves the pipelined modules after overriding their forwards, initializes the
         modules' input dists, and overrides the input dist forwards to support fusing
         the splits collective in the input dist.
         """
         if self._pipelined_modules:
             return
-        self._pipelined_modules = _rewrite_model(
-            self._model, self._context, self._data_dist_stream
+        self._pipelined_modules, self._model = _rewrite_model(
+            model=self._model,
+            context=self._context,
+            dist_stream=self._data_dist_stream,
+            batch=self._batch_i,
+            apply_jit=self._apply_jit,
         )
         # initializes input dist, so we can override input dist forwards
         self._start_sparse_data_dist(self._batch_i)
         _override_input_dist_forwards(self._pipelined_modules)
 
     def _copy_batch_to_gpu(self, dataloader_iter: Iterator[In]) -> Optional[In]:
         """
```

## torchrec/distributed/types.py

```diff
@@ -51,14 +51,55 @@
     ShardingSpec,
     ShardMetadata,
 )
 from torch.nn.modules.module import _addindent
 from torchrec.streamable import Multistreamable
 
 
+@unique
+class BoundsCheckMode(Enum):
+    # Raise an exception (CPU) or device-side assert (CUDA)
+    FATAL = 0
+    # Log the first out-of-bounds instance per kernel, and set to zero.
+    WARNING = 1
+    # Set to zero.
+    IGNORE = 2
+    # No bounds checks.
+    NONE = 3
+
+
+@unique
+class CacheAlgorithm(Enum):
+    LRU = 0
+    LFU = 1
+
+
+# moved DataType here to avoid circular import
+# TODO: organize types and dependencies
+@unique
+class DataType(Enum):
+    """
+    Our fusion implementation supports only certain types of data
+    so it makes sense to retrict in a non-fused version as well.
+    """
+
+    FP32 = "FP32"
+    FP16 = "FP16"
+    BF16 = "BF16"
+    INT64 = "INT64"
+    INT32 = "INT32"
+    INT8 = "INT8"
+    UINT8 = "UINT8"
+    INT4 = "INT4"
+    INT2 = "INT2"
+
+    def __str__(self) -> str:
+        return self.value
+
+
 class ShardingType(Enum):
     """
     Well-known sharding types, used by inter-module optimizations.
     """
 
     # Replicated on all ranks
     DATA_PARALLEL = "data_parallel"
@@ -297,16 +338,17 @@
         if isinstance(obj, LazyAwaitable):
             if obj._result is None:
                 obj._result = obj.wait()
             return obj._result
         else:
             return obj
 
+    @classmethod
     # pyre-ignore [2, 3]
-    def __torch_function__(self, func, types, args=(), kwargs=None):
+    def __torch_function__(cls, func, types, args=(), kwargs=None):
         """
         The LazyAwaitable type has a `__torch_function__` implementation.
         This means when this type is seens as an argument to a PyTorch
         function in a position where it expects a W, the PyTorch's
         dispatcher will call into this function for special handling
 
         Our `__torch_function__` implementation goes through all of the
@@ -346,14 +388,56 @@
         super().__init__()
         self._obj = obj
 
     def _wait_impl(self) -> W:
         return self._obj
 
 
+KT = TypeVar("KT")
+VT_co = TypeVar("VT_co")
+ParentW = TypeVar("ParentW")
+
+
+class LazyGetItemMixin(Generic[KT, VT_co]):
+    """Augments the base LazyAwaitable with a lazy __getitem__ method.
+
+    Instead of triggering a wait() on a __getitem__ call, KeyedLazyAwaitable
+    will return another awaitable. This can achieve better
+    communication/computation overlap by deferring the wait() until the
+    tensor data is actually needed.
+
+    This is intended for Awaitables that model keyed collections, like
+    dictionaries or EmbeddingBagCollectionAwaitable.
+
+    NOTE: if using this mixin, please include it before LazyAwaitable in the
+    inheritance list, so that Python MRO can properly select this __getitem__
+    implementation.
+    """
+
+    def __getitem__(self, key: KT) -> LazyAwaitable[VT_co]:
+        return GetItemLazyAwaitable(self, key)
+
+
+class GetItemLazyAwaitable(LazyAwaitable[W], Generic[W, ParentW, KT]):
+    """The LazyAwaitable returned from a __getitem__ call on `LazyGetItemMixin`.
+
+    When the actual value of this awaitable is requested, wait on the parent and
+    then call __getitem__ on the result.
+    """
+
+    def __init__(self, parent: LazyAwaitable[ParentW], key: KT) -> None:
+        super().__init__()
+        self._parent = parent
+        self._key = key
+
+    def _wait_impl(self) -> W:
+        kt = LazyAwaitable._wait_async(self._parent)
+        return kt[self._key]
+
+
 # install magic methods
 for orig_method_name in torch.fx.graph.magic_methods:
     as_magic = f"__{orig_method_name}__"
 
     def scope(method):
         def impl(*args, **kwargs):
             lhs = args[0]
@@ -395,37 +479,53 @@
 
 
 class ModuleShardingPlan:
     pass
 
 
 @dataclass
+class CacheParams:
+    algorithm: Optional[CacheAlgorithm] = None
+    load_factor: Optional[float] = None
+    reserved_memory: Optional[float] = None
+    precision: Optional[DataType] = None
+
+
+@dataclass
 class ParameterSharding:
     """
         Describes the sharding of the parameter.
 
         sharding_type (str): how this parameter is sharded. See ShardingType for well-known
             types.
         compute_kernel (str): compute kernel to be used by this parameter.
         ranks (Optional[List[int]]): rank of each shard.
         sharding_spec (Optional[ShardingSpec]): list of ShardMetadata for each shard.
+        cache_params (Optional[CacheParams]): cache params for embedding lookup.
+        enforce_hbm (Optional[bool]): whether to use HBM.
+        stochastic_rounding (Optional[bool]): whether to use stochastic rounding.
+        bounds_check_mode (Optional[BoundsCheckMode]): bounds check mode.
 
     NOTE:
       ShardingType.TABLE_WISE - rank where this embedding is placed
       ShardingType.COLUMN_WISE - rank where the embedding shards are placed, seen as
       individual tables
       ShardingType.TABLE_ROW_WISE  - first rank when this embedding is placed
       ShardingType.ROW_WISE, ShardingType.DATA_PARALLEL - unused
 
     """
 
     sharding_type: str
     compute_kernel: str
     ranks: Optional[List[int]] = None
     sharding_spec: Optional[ShardingSpec] = None
+    cache_params: Optional[CacheParams] = None
+    enforce_hbm: Optional[bool] = None
+    stochastic_rounding: Optional[bool] = None
+    bounds_check_mode: Optional[BoundsCheckMode] = None
 
 
 class EmbeddingModuleShardingPlan(ModuleShardingPlan, Dict[str, ParameterSharding]):
     """
     Map of ParameterSharding per parameter (usually a table). This describes the sharding plan for a torchrec module (e.g. `EmbeddingBagCollection`)
     """
```

## torchrec/distributed/utils.py

```diff
@@ -2,26 +2,40 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import copy
+import logging
 
 from collections import OrderedDict
 from typing import Any, Dict, List, Optional, Set, Type, TypeVar, Union
 
 import torch
 from fbgemm_gpu.split_embedding_configs import EmbOptimType
 from torch import nn
 from torchrec import optim as trec_optim
-from torchrec.distributed.types import ShardedModule
+from torchrec.distributed.embedding_types import EmbeddingComputeKernel
+from torchrec.distributed.types import (
+    BoundsCheckMode,
+    CacheAlgorithm,
+    DataType,
+    ParameterSharding,
+    ShardedModule,
+    ShardingType,
+)
+from torchrec.modules.embedding_configs import (
+    data_type_to_sparse_type,
+    to_fbgemm_bounds_check_mode,
+    to_fbgemm_cache_algorithm,
+)
 from torchrec.types import CopyMixIn
 
-
+logger: logging.Logger = logging.getLogger(__name__)
 _T = TypeVar("_T")
 
 
 """
 torch.package safe functions from pyre_extensions. However, pyre_extensions is
 not safe to use in code that will be torch.packaged, as it requires sys for
 version checks
@@ -330,14 +344,95 @@
         param_fused_params["learning_rate"] = param_fused_params.pop("lr")
 
     _fused_params = copy.deepcopy(fused_params)
     _fused_params.update(param_fused_params)
     return _fused_params
 
 
+def add_params_from_parameter_sharding(
+    fused_params: Optional[Dict[str, Any]],
+    parameter_sharding: ParameterSharding,
+) -> Dict[str, Any]:
+    """
+    Extract params from parameter sharding and then add them to fused_params.
+
+    Params from parameter sharding will override the ones in fused_params if they
+    exist already.
+
+    Args:
+        fused_params (Optional[Dict[str, Any]]): the existing fused_params
+        parameter_sharding (ParameterSharding): the parameter sharding to use
+
+    Returns:
+        [Dict[str, Any]]: the fused_params dictionary with params from parameter
+        sharding added.
+
+    """
+    if fused_params is None:
+        fused_params = {}
+
+    # update fused_params using params from parameter_sharding
+    # this will take precidence over the fused_params provided from sharders
+    if parameter_sharding.cache_params is not None:
+        cache_params = parameter_sharding.cache_params
+        if cache_params.algorithm is not None:
+            fused_params["cache_algorithm"] = cache_params.algorithm
+        if cache_params.load_factor is not None:
+            fused_params["cache_load_factor"] = cache_params.load_factor
+        if cache_params.reserved_memory is not None:
+            fused_params["cache_reserved_memory"] = cache_params.reserved_memory
+        if cache_params.precision is not None:
+            fused_params["cache_precision"] = cache_params.precision
+
+    if parameter_sharding.enforce_hbm is not None:
+        fused_params["enforce_hbm"] = parameter_sharding.enforce_hbm
+
+    if parameter_sharding.stochastic_rounding is not None:
+        fused_params["stochastic_rounding"] = parameter_sharding.stochastic_rounding
+
+    if parameter_sharding.bounds_check_mode is not None:
+        fused_params["bounds_check_mode"] = parameter_sharding.bounds_check_mode
+
+    # print warning if sharding_type is data_parallel or kernel is dense
+    if parameter_sharding.sharding_type == ShardingType.DATA_PARALLEL.value:
+        logger.warning(
+            f"Sharding Type is {parameter_sharding.sharding_type}, "
+            "caching params will be ignored"
+        )
+    elif parameter_sharding.compute_kernel == EmbeddingComputeKernel.DENSE.value:
+        logger.warning(
+            f"Compute Kernel is {parameter_sharding.compute_kernel}, "
+            "caching params will be ignored"
+        )
+
+    return fused_params
+
+
+def convert_to_fbgemm_types(fused_params: Dict[str, Any]) -> Dict[str, Any]:
+    if "cache_precision" in fused_params:
+        if isinstance(fused_params["cache_precision"], DataType):
+            fused_params["cache_precision"] = data_type_to_sparse_type(
+                fused_params["cache_precision"]
+            )
+
+    if "cache_algorithm" in fused_params:
+        if isinstance(fused_params["cache_algorithm"], CacheAlgorithm):
+            fused_params["cache_algorithm"] = to_fbgemm_cache_algorithm(
+                fused_params["cache_algorithm"]
+            )
+
+    if "bounds_check_mode" in fused_params:
+        if isinstance(fused_params["bounds_check_mode"], BoundsCheckMode):
+            fused_params["bounds_check_mode"] = to_fbgemm_bounds_check_mode(
+                fused_params["bounds_check_mode"]
+            )
+
+    return fused_params
+
+
 def init_parameters(module: nn.Module, device: torch.device) -> None:
     @torch.no_grad()
     def init_parameters(module: nn.Module) -> None:
         # Allocate parameters and buffers if over 'meta' device.
         has_meta_param = False
         for name, param in module._parameters.items():
             if isinstance(param, torch.Tensor) and param.device.type == "meta":
@@ -348,11 +443,10 @@
                 has_meta_param = True
         for name, buffer in module._buffers.items():
             if isinstance(buffer, torch.Tensor) and buffer.device.type == "meta":
                 module._buffers[name] = torch.empty_like(buffer, device=device)
 
         # Init parameters if at least one parameter is over 'meta' device.
         if has_meta_param and hasattr(module, "reset_parameters"):
-            # pyre-ignore [29]
             module.reset_parameters()
 
     module.apply(init_parameters)
```

## torchrec/distributed/planner/enumerators.py

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import logging
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 from torch import nn
 from torchrec.distributed.embedding_types import EmbeddingComputeKernel
 from torchrec.distributed.planner.constants import POOLING_FACTOR
 from torchrec.distributed.planner.shard_estimators import (
     EmbeddingPerfEstimator,
     EmbeddingStorageEstimator,
@@ -22,15 +22,20 @@
     Shard,
     ShardEstimator,
     ShardingOption,
     Topology,
 )
 from torchrec.distributed.planner.utils import sharder_name
 from torchrec.distributed.sharding_plan import calculate_shard_sizes_and_offsets
-from torchrec.distributed.types import ModuleSharder, ShardingType
+from torchrec.distributed.types import (
+    BoundsCheckMode,
+    CacheParams,
+    ModuleSharder,
+    ShardingType,
+)
 from torchrec.modules.embedding_tower import EmbeddingTower, EmbeddingTowerCollection
 
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class EmbeddingEnumerator(Enumerator):
@@ -99,32 +104,30 @@
                     if child_path != "":
                         named_modules_queue.append((child_path + "." + n, m))
                     else:
                         named_modules_queue.append((n, m))
                 continue
 
             for name, param in sharder.shardable_parameters(child_module).items():
+                (
+                    input_lengths,
+                    col_wise_shard_dim,
+                    cache_params,
+                    enforce_hbm,
+                    stochastic_rounding,
+                    bounds_check_mode,
+                ) = _extract_constraints_for_param(self._constraints, name)
+
                 for sharding_type in self._filter_sharding_types(
                     name, sharder.sharding_types(self._compute_device)
                 ):
                     for compute_kernel in self._filter_compute_kernels(
                         name,
                         sharder.compute_kernels(sharding_type, self._compute_device),
                     ):
-
-                        input_lengths = (
-                            self._constraints[name].pooling_factors
-                            if self._constraints and self._constraints.get(name)
-                            else [POOLING_FACTOR]
-                        )
-                        col_wise_shard_dim = (
-                            self._constraints[name].min_partition
-                            if self._constraints and self._constraints.get(name)
-                            else None
-                        )
                         (
                             shard_sizes,
                             shard_offsets,
                         ) = calculate_shard_sizes_and_offsets(
                             tensor=param,
                             world_size=self._world_size,
                             local_world_size=self._local_world_size,
@@ -147,14 +150,18 @@
                                 compute_kernel=compute_kernel,
                                 sharding_type=sharding_type,
                                 partition_by=get_partition_by_type(sharding_type),
                                 shards=[
                                     Shard(size=size, offset=offset)
                                     for size, offset in zip(shard_sizes, shard_offsets)
                                 ],
+                                cache_params=cache_params,
+                                enforce_hbm=enforce_hbm,
+                                stochastic_rounding=stochastic_rounding,
+                                bounds_check_mode=bounds_check_mode,
                                 dependency=dependency,
                             )
                         )
                 if not sharding_options:
                     raise RuntimeError(
                         "No available sharding type and compute kernel combination "
                         f"after applying user provided constraints for {name}"
@@ -208,14 +215,49 @@
         if not filtered_compute_kernels:
             logger.warn(
                 f"No available compute kernels after applying user provided constraints for {name}"
             )
         return filtered_compute_kernels
 
 
+def _extract_constraints_for_param(
+    constraints: Optional[Dict[str, ParameterConstraints]], name: str
+) -> Tuple[
+    List[float],
+    Optional[int],
+    Optional[CacheParams],
+    Optional[bool],
+    Optional[bool],
+    Optional[BoundsCheckMode],
+]:
+    input_lengths = [POOLING_FACTOR]
+    col_wise_shard_dim = None
+    cache_params = None
+    enforce_hbm = None
+    stochastic_rounding = None
+    bounds_check_mode = None
+
+    if constraints and constraints.get(name):
+        input_lengths = constraints[name].pooling_factors
+        col_wise_shard_dim = constraints[name].min_partition
+        cache_params = constraints[name].cache_params
+        enforce_hbm = constraints[name].enforce_hbm
+        stochastic_rounding = constraints[name].stochastic_rounding
+        bounds_check_mode = constraints[name].bounds_check_mode
+
+    return (
+        input_lengths,
+        col_wise_shard_dim,
+        cache_params,
+        enforce_hbm,
+        stochastic_rounding,
+        bounds_check_mode,
+    )
+
+
 def get_partition_by_type(sharding_type: str) -> str:
     """
     Gets corresponding partition by type for provided sharding type.
 
     Args:
         sharding_type (str): sharding type string.
```

## torchrec/distributed/planner/planners.py

```diff
@@ -90,14 +90,18 @@
                     )
                     for shard in shards
                 ]
             ),
             sharding_type=sharding_type,
             compute_kernel=sharding_option.compute_kernel,
             ranks=[cast(int, shard.rank) for shard in shards],
+            cache_params=sharding_option.cache_params,
+            enforce_hbm=sharding_option.enforce_hbm,
+            stochastic_rounding=sharding_option.stochastic_rounding,
+            bounds_check_mode=sharding_option.bounds_check_mode,
         )
         plan[sharding_option.path] = module_plan
     return ShardingPlan(plan)
 
 
 class EmbeddingShardingPlanner(ShardingPlanner):
     """
```

## torchrec/distributed/planner/shard_estimators.py

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+import logging
 import math
 from typing import cast, Dict, List, Optional, Tuple, Type
 
 import torch
 import torchrec.optim as trec_optim
 from torch import nn
 from torchrec.distributed.embedding_types import EmbeddingComputeKernel
@@ -34,14 +35,16 @@
     Topology,
 )
 from torchrec.distributed.planner.utils import prod, sharder_name
 from torchrec.distributed.types import CommOp, ModuleSharder, ShardingType
 
 from torchrec.modules.embedding_modules import EmbeddingBagCollectionInterface
 
+logger: logging.Logger = logging.getLogger(__name__)
+
 
 class EmbeddingPerfEstimator(ShardEstimator):
     """
     Embedding Wall Time Perf Estimator
     """
 
     def __init__(
@@ -62,19 +65,32 @@
         if not sharder_map:
             assert not sharding_options, "sharder_map not provided for sharding_options"
             return
 
         for sharding_option in sharding_options:
             sharder_key = sharder_name(type(sharding_option.module[1]))
             sharder = sharder_map[sharder_key]
+
             caching_ratio = (
-                sharder.fused_params.get("cache_load_factor")  # pyre-ignore[16]
-                if hasattr(sharder, "fused_params") and sharder.fused_params
+                self._constraints[  # pyre-ignore[16]
+                    sharding_option.name
+                ].cache_params.load_factor
+                if self._constraints
+                and self._constraints.get(sharding_option.name)
+                and self._constraints[sharding_option.name].cache_params
                 else None
             )
+            # TODO: remove after deprecating fused_params in sharder
+            if caching_ratio is None:
+                caching_ratio = (
+                    sharder.fused_params.get("cache_load_factor")  # pyre-ignore[16]
+                    if hasattr(sharder, "fused_params") and sharder.fused_params
+                    else None
+                )
+
             num_poolings = (
                 cast(List[float], self._constraints[sharding_option.name].num_poolings)
                 if self._constraints
                 and self._constraints.get(sharding_option.name)
                 and self._constraints[sharding_option.name].num_poolings
                 else [1.0] * sharding_option.num_inputs
             )
@@ -91,29 +107,43 @@
                 == len(num_poolings)
                 == len(batch_sizes)
             ), "Provided `pooling_factors`, `num_poolings`, and `batch_sizes` constraints must match."
 
             module = sharding_option.module[1]
 
             # TODO remove this hack once feature processor is disaggregated
-            has_feature_processor = (
-                True if getattr(module, "feature_processor", None) else False
-            )
+            has_feature_processor = False
+            if (
+                hasattr(module, "_feature_processor")
+                and hasattr(module._feature_processor, "feature_processor_modules")
+                and isinstance(
+                    module._feature_processor.feature_processor_modules,
+                    nn.ModuleDict,
+                )
+                and sharding_option.name
+                in module._feature_processor.feature_processor_modules.keys()
+            ):
+                has_feature_processor = True
+                logger.info(f"Table {sharding_option.name} has feature processor.")
 
             if isinstance(module, EmbeddingBagCollectionInterface):
                 is_weighted = module.is_weighted()
             elif (
                 self._constraints
                 and self._constraints.get(sharding_option.name)
                 and self._constraints[sharding_option.name].is_weighted
             ):
                 is_weighted = self._constraints[sharding_option.name].is_weighted
             else:
                 is_weighted = False
 
+            # TODO remove this once migrate away from PEA
+            is_weighted = is_weighted or has_feature_processor
+            sharding_option.is_weighted = is_weighted
+
             table_data_type_size = sharding_option.tensor.element_size()
             (
                 fwd_a2a_comm_data_type_size,
                 bwd_a2a_comm_data_type_size,
                 fwd_sr_comm_data_type_size,
                 bwd_sr_comm_data_type_size,
             ) = _extract_comm_data_type_size(sharder, sharding_option)
@@ -137,15 +167,14 @@
                 hbm_mem_bw=self._topology.hbm_mem_bw,
                 ddr_mem_bw=self._topology.ddr_mem_bw,
                 intra_host_bw=self._topology.intra_host_bw,
                 inter_host_bw=self._topology.inter_host_bw,
                 is_pooled=sharding_option.is_pooled,
                 is_weighted=is_weighted,
                 is_inference=self._is_inference,
-                has_feature_processor=has_feature_processor,
                 caching_ratio=caching_ratio,
             )
 
             for shard, perf in zip(sharding_option.shards, shard_perfs):
                 shard.perf = perf
 
 
@@ -167,15 +196,14 @@
     num_poolings: List[float],
     hbm_mem_bw: float,
     ddr_mem_bw: float,
     intra_host_bw: float,
     inter_host_bw: float,
     is_pooled: bool,
     is_weighted: bool = False,
-    has_feature_processor: bool = False,
     caching_ratio: Optional[float] = None,
     is_inference: bool = False,
 ) -> List[Perf]:
     """
     Attempts to model perfs as a function of relative wall times.
 
     Args:
@@ -202,15 +230,14 @@
         intra_host_bw (float): the bandwidth within a single host like multiple threads.
         inter_host_bw (float): the bandwidth between two hosts like multiple machines.
         is_pooled (bool): True if embedding output is pooled (ie. `EmbeddingBag`), False
             if unpooled/sequential (ie. `Embedding`).
         is_weighted (bool = False): if the module is an EBC and is weighted, typically
             signifying an id score list feature.
         is_inference (bool = False): if planning for inference.
-        has_feature_processor (bool = False): if the module has a feature processor.
         caching_ratio (Optional[float] = None): cache ratio to determine the bandwidth
             of device.
 
     Returns:
         List[float]: the list of perf for each shard.
     """
 
@@ -242,15 +269,14 @@
                 num_poolings=num_poolings,
                 device_bw=device_bw,
                 inter_host_bw=inter_host_bw,
                 intra_host_bw=intra_host_bw,
                 is_pooled=is_pooled,
                 is_weighted=is_weighted,
                 is_inference=is_inference,
-                has_feature_processor=has_feature_processor,
             )
         elif sharding_type == ShardingType.ROW_WISE.value:
             shard_perf = _get_rw_sharding_perf(
                 batch_sizes=batch_sizes,
                 world_size=world_size,
                 local_world_size=local_world_size,
                 input_lengths=input_lengths,
@@ -263,15 +289,14 @@
                 bwd_sr_comm_data_type_size=bwd_sr_comm_data_type_size,
                 num_poolings=num_poolings,
                 device_bw=device_bw,
                 inter_host_bw=inter_host_bw,
                 intra_host_bw=intra_host_bw,
                 is_pooled=is_pooled,
                 is_weighted=is_weighted,
-                has_feature_processor=has_feature_processor,
             )
         elif sharding_type == ShardingType.TABLE_ROW_WISE.value:
             shard_perf = _get_twrw_sharding_perf(
                 batch_sizes=batch_sizes,
                 world_size=world_size,
                 local_world_size=local_world_size,
                 input_lengths=input_lengths,
@@ -284,15 +309,14 @@
                 bwd_sr_comm_data_type_size=bwd_sr_comm_data_type_size,
                 num_poolings=num_poolings,
                 device_bw=device_bw,
                 inter_host_bw=inter_host_bw,
                 intra_host_bw=intra_host_bw,
                 is_pooled=is_pooled,
                 is_weighted=is_weighted,
-                has_feature_processor=has_feature_processor,
             )
         elif sharding_type == ShardingType.DATA_PARALLEL.value:
             shard_perf = _get_dp_sharding_perf(
                 batch_sizes=batch_sizes,
                 world_size=world_size,
                 local_world_size=local_world_size,
                 input_lengths=input_lengths,
@@ -301,15 +325,14 @@
                 input_data_type_size=input_data_type_size,
                 table_data_type_size=table_data_type_size,
                 num_poolings=num_poolings,
                 device_bw=device_bw,
                 inter_host_bw=inter_host_bw,
                 is_pooled=is_pooled,
                 is_weighted=is_weighted,
-                has_feature_processor=has_feature_processor,
             )
         else:
             raise ValueError(
                 f"Unrecognized or unsupported sharding type provided: {sharding_type}"
             )
         shard_perfs.append(shard_perf)
 
@@ -329,27 +352,26 @@
     num_poolings: List[float],
     device_bw: float,
     inter_host_bw: float,
     intra_host_bw: float,
     is_pooled: bool,
     is_weighted: bool = False,
     is_inference: bool = False,
-    has_feature_processor: bool = False,
 ) -> Perf:
     batch_inputs = sum(
         [x * y * z for x, y, z in zip(input_lengths, num_poolings, batch_sizes)]
     )
     batch_outputs = (
         sum([x * y for x, y in zip(num_poolings, batch_sizes)])
         if is_pooled
         else batch_inputs
     )
 
     input_read_size = math.ceil(batch_inputs * world_size * input_data_type_size)
-    if is_weighted or has_feature_processor:
+    if is_weighted:
         input_read_size *= 2
 
     # minimum embedding dim is set to 32 due to kernel usage
     embedding_lookup_size = (
         batch_inputs * world_size * max(emb_dim, 32) * table_data_type_size
     )
 
@@ -381,17 +403,15 @@
         return Perf(
             fwd_compute=fwd_compute, fwd_comms=fwd_comms, bwd_compute=0, bwd_comms=0
         )
 
     bwd_comms = bwd_output_write_size / comms_bw
 
     bwd_grad_indice_weights_kernel = (
-        fwd_compute * WEIGHTED_KERNEL_MULTIPLIER
-        if is_weighted or has_feature_processor
-        else 0
+        fwd_compute * WEIGHTED_KERNEL_MULTIPLIER if is_weighted else 0
     )
 
     # includes fused optimizers
     bwd_compute = fwd_compute * BWD_COMPUTE_MULTIPLIER
 
     # in order of model parallel execution, starting with:
     # BWD DP -> BWD MP ... FWD MP -> FWD DP
@@ -417,28 +437,27 @@
     bwd_sr_comm_data_type_size: float,
     num_poolings: List[float],
     device_bw: float,
     inter_host_bw: float,
     intra_host_bw: float,
     is_pooled: bool,
     is_weighted: bool = False,
-    has_feature_processor: bool = False,
 ) -> Perf:
     batch_inputs = (
         sum([x * y * z for x, y, z in zip(input_lengths, num_poolings, batch_sizes)])
         / world_size
     )
     batch_outputs = (
         sum([x * y for x, y in zip(num_poolings, batch_sizes)])
         if is_pooled
         else batch_inputs
     )
 
     input_read_size = math.ceil(batch_inputs * world_size * input_data_type_size)
-    if is_weighted or has_feature_processor:
+    if is_weighted:
         input_read_size *= 2
 
     embedding_lookup_size = batch_inputs * world_size * emb_dim * table_data_type_size
 
     fwd_output_write_size = (
         batch_outputs * world_size * emb_dim * fwd_sr_comm_data_type_size
         if is_pooled
@@ -458,17 +477,15 @@
     ) / device_bw
 
     bwd_comms = bwd_output_write_size / comms_bw
 
     bwd_batched_copy = bwd_output_write_size * BATCHED_COPY_PERF_FACTOR / device_bw
 
     bwd_grad_indice_weights_kernel = (
-        fwd_compute * WEIGHTED_KERNEL_MULTIPLIER
-        if is_weighted or has_feature_processor
-        else 0
+        fwd_compute * WEIGHTED_KERNEL_MULTIPLIER if is_weighted else 0
     )
 
     bwd_compute = fwd_compute * BWD_COMPUTE_MULTIPLIER
 
     return Perf(
         fwd_compute=fwd_compute,
         fwd_comms=fwd_comms,
@@ -491,28 +508,27 @@
     bwd_sr_comm_data_type_size: float,
     num_poolings: List[float],
     device_bw: float,
     inter_host_bw: float,
     intra_host_bw: float,
     is_pooled: bool,
     is_weighted: bool = False,
-    has_feature_processor: bool = False,
 ) -> Perf:
     batch_inputs = (
         sum([x * y * z for x, y, z in zip(input_lengths, num_poolings, batch_sizes)])
         / local_world_size
     )
     batch_outputs = (
         sum([x * y for x, y in zip(num_poolings, batch_sizes)])
         if is_pooled
         else batch_inputs
     )
 
     input_read_size = math.ceil(batch_inputs * world_size * input_data_type_size)
-    if is_weighted or has_feature_processor:
+    if is_weighted:
         input_read_size *= 2
 
     embedding_lookup_size = batch_inputs * world_size * emb_dim * table_data_type_size
 
     fwd_output_write_size = (
         batch_outputs * world_size * emb_dim * fwd_sr_comm_data_type_size
     )
@@ -537,17 +553,15 @@
     fwd_compute = (
         input_read_size + embedding_lookup_size + fwd_output_write_size
     ) / device_bw
 
     bwd_comms = bwd_output_write_size / intra_host_bw
 
     bwd_grad_indice_weights_kernel = (
-        fwd_compute * WEIGHTED_KERNEL_MULTIPLIER
-        if is_weighted or has_feature_processor
-        else 0
+        fwd_compute * WEIGHTED_KERNEL_MULTIPLIER if is_weighted else 0
     )
 
     bwd_batched_copy = bwd_output_write_size * BATCHED_COPY_PERF_FACTOR / device_bw
 
     bwd_compute = fwd_compute * BWD_COMPUTE_MULTIPLIER
 
     return Perf(
@@ -568,27 +582,26 @@
     input_data_type_size: float,
     table_data_type_size: float,
     num_poolings: List[float],
     device_bw: float,
     inter_host_bw: float,
     is_pooled: bool,
     is_weighted: bool = False,
-    has_feature_processor: bool = False,
 ) -> Perf:
     batch_inputs = sum(
         [x * y * z for x, y, z in zip(input_lengths, num_poolings, batch_sizes)]
     )
     batch_outputs = (
         sum([x * y for x, y in zip(num_poolings, batch_sizes)])
         if is_pooled
         else batch_inputs
     )
 
     input_read_size = math.ceil(batch_inputs * input_data_type_size)
-    if is_weighted or has_feature_processor:
+    if is_weighted:
         input_read_size *= 2
 
     embedding_lookup_size = batch_inputs * emb_dim * table_data_type_size
 
     output_write_size = batch_outputs * emb_dim * table_data_type_size
     table_size = grad_num_elem * table_data_type_size
 
@@ -611,17 +624,15 @@
 
     # SGD + Fill + BUnary
     optimizer_kernels = table_size * DP_ELEMENTWISE_KERNELS_PERF_FACTOR / device_bw
 
     bwd_compute = fwd_compute * BWD_COMPUTE_MULTIPLIER
 
     bwd_grad_indice_weights_kernel = (
-        fwd_compute * WEIGHTED_KERNEL_MULTIPLIER
-        if is_weighted or has_feature_processor
-        else 0
+        fwd_compute * WEIGHTED_KERNEL_MULTIPLIER if is_weighted else 0
     )
 
     return Perf(
         fwd_compute=fwd_compute,
         fwd_comms=0,
         bwd_compute=bwd_compute + bwd_grad_indice_weights_kernel,
         bwd_comms=all_reduce + optimizer_kernels,
@@ -707,19 +718,32 @@
         if not sharder_map:
             assert not sharding_options, "sharder_map not provided for sharding_options"
             return
 
         for sharding_option in sharding_options:
             sharder_key = sharder_name(type(sharding_option.module[1]))
             sharder = sharder_map[sharder_key]
+
             caching_ratio = (
-                sharder.fused_params.get("cache_load_factor")  # pyre-ignore[16]
-                if hasattr(sharder, "fused_params") and sharder.fused_params
+                self._constraints[  # pyre-ignore[16]
+                    sharding_option.name
+                ].cache_params.load_factor
+                if self._constraints
+                and self._constraints.get(sharding_option.name)
+                and self._constraints[sharding_option.name].cache_params
                 else None
             )
+            # TODO: remove after deprecating fused_params in sharder
+            if caching_ratio is None:
+                caching_ratio = (
+                    sharder.fused_params.get("cache_load_factor")  # pyre-ignore[16]
+                    if hasattr(sharder, "fused_params") and sharder.fused_params
+                    else None
+                )
+
             num_poolings = (
                 cast(List[float], self._constraints[sharding_option.name].num_poolings)
                 if self._constraints
                 and self._constraints.get(sharding_option.name)
                 and self._constraints[sharding_option.name].num_poolings
                 else [1.0] * sharding_option.num_inputs
             )
```

## torchrec/distributed/planner/stats.py

```diff
@@ -231,28 +231,30 @@
                     "FQN",
                     "Sharding",
                     "Compute Kernel",
                     "Perf (ms)",
                     "Pooling Factor",
                     "Num Poolings",
                     "Output",
+                    "Weighing",
                     "Features",
                     "Emb Dim",
                     "Hash Size",
                     "Ranks",
                 ],
                 [
                     "-----",
                     "----------",
                     "----------------",
                     "-----------",
                     "----------------",
                     "--------------",
                     "--------",
                     "----------",
+                    "----------",
                     "---------",
                     "-----------",
                     "-------",
                 ],
             ]
             feat_batch_sizes = [
                 constraints[so.name].batch_sizes
@@ -279,26 +281,28 @@
                     if constraints
                     and constraints.get(so.name)
                     and constraints[so.name].num_poolings
                     else [NUM_POOLINGS] * len(so.input_lengths)
                 )
                 num_poolings = str(round(sum(num_poolings), 3))
                 output = "pooled" if so.is_pooled else "sequence"
+                weighing = "weighted" if so.is_weighted else "unweighted"
                 num_features = len(so.input_lengths)
                 embedding_dim = so.tensor.shape[1]
                 hash_size = so.tensor.shape[0]
                 param_table.append(
                     [
                         so.fqn,
                         _get_sharding_type_abbr(so.sharding_type),
                         so.compute_kernel,
                         shard_perfs,
                         pooling_factor,
                         num_poolings,
                         output,
+                        weighing,
                         num_features,
                         embedding_dim,
                         hash_size,
                         ",".join(ranks),
                     ]
                 )
                 if include_batch_sizes:
```

## torchrec/distributed/planner/storage_reservations.py

```diff
@@ -231,27 +231,33 @@
         return reserved_topology
 
 
 class InferenceStorageReservation(StorageReservation):
     """
     Reserves storage for model to be sharded for inference. The storage reservation
     is comprised of dense tensor storage, KJT storage, and an extra percentage of total
-    storage.
+    storage. Note that when estimating for storage, dense modules are assumed to be on
+    GPUs and replicated across ranks. If this is not the case, please override the
+    estimates with dense_tensor_estimate.
 
     Args:
         percentage (float): extra storage percentage to reserve that acts as a margin of
             error beyond storage calculation.
+        dense_tensor_estimate (Optional[int]): storage estimate for dense tensors, use
+            default heuristic estimate if not provided.
     """
 
     def __init__(
         self,
         percentage: float,
+        dense_tensor_estimate: Optional[int] = None,
     ) -> None:
         assert percentage >= 0 and percentage <= 1
         self._percentage: float = percentage
+        self._dense_tensor_estimate = dense_tensor_estimate
 
         self._dense_storage: Optional[Storage] = None
         self._kjt_storage: Optional[Storage] = None
 
     def reserve(
         self,
         topology: Topology,
@@ -269,14 +275,15 @@
         _reserve_storage_percentage(reserved_topology, self._percentage)
 
         self._dense_storage = _reserve_dense_storage(
             topology=reserved_topology,
             module=module,
             shardable_modules=shardable_modules,
             multiplier=1,
+            dense_tensor_estimate=self._dense_tensor_estimate,
         )
 
         self._kjt_storage = _reserve_kjt_storage(
             topology=reserved_topology,
             batch_size=batch_size,
             input_lengths=input_lengths,
             input_data_type_size=BIGINT_DTYPE,
```

## torchrec/distributed/planner/types.py

```diff
@@ -19,15 +19,20 @@
     DDR_CAP,
     DDR_MEM_BW,
     HBM_CAP,
     HBM_MEM_BW,
     INTRA_NODE_BANDWIDTH,
     POOLING_FACTOR,
 )
-from torchrec.distributed.types import ModuleSharder, ShardingPlan
+from torchrec.distributed.types import (
+    BoundsCheckMode,
+    CacheParams,
+    ModuleSharder,
+    ShardingPlan,
+)
 from torchrec.modules.embedding_modules import EmbeddingCollectionInterface
 
 # ---- Perf ---- #
 
 
 @dataclass(repr=True, eq=True)
 class Perf:
@@ -240,29 +245,38 @@
         module: Tuple[str, nn.Module],
         input_lengths: List[float],
         batch_size: int,
         sharding_type: str,
         partition_by: str,
         compute_kernel: str,
         shards: List[Shard],
+        cache_params: Optional[CacheParams] = None,
+        enforce_hbm: Optional[bool] = None,
+        stochastic_rounding: Optional[bool] = None,
+        bounds_check_mode: Optional[BoundsCheckMode] = None,
         dependency: Optional[str] = None,
     ) -> None:
         self.name = name
         self._tensor = tensor
         self._module = module
         self.input_lengths = input_lengths
         self.batch_size = batch_size
         self.sharding_type = sharding_type
         self.partition_by = partition_by
         self.compute_kernel = compute_kernel
         # relevant to planner output, must be populated if sharding option
         # part of final solution
         self.shards = shards
+        self.cache_params = cache_params
+        self.enforce_hbm = enforce_hbm
+        self.stochastic_rounding = stochastic_rounding
+        self.bounds_check_mode = bounds_check_mode
         self.dependency = dependency
         self._is_pooled: Optional[bool] = None
+        self.is_weighted: Optional[bool] = None
 
     @property
     def tensor(self) -> torch.Tensor:
         return self._tensor
 
     @property
     def module(self) -> Tuple[str, nn.Module]:
@@ -358,14 +372,18 @@
     min_partition: Optional[int] = None  # CW sharding
     pooling_factors: List[float] = field(
         default_factory=lambda: [POOLING_FACTOR]
     )  # average number of embedding lookups required per sample
     num_poolings: Optional[List[float]] = None  # number of poolings per sample in batch
     batch_sizes: Optional[List[int]] = None  # batch size per input feature
     is_weighted: bool = False
+    cache_params: Optional[CacheParams] = None
+    enforce_hbm: Optional[bool] = None
+    stochastic_rounding: Optional[bool] = None
+    bounds_check_mode: Optional[BoundsCheckMode] = None
 
 
 class PlannerErrorType(Enum):
     """
     Classify PlannerError based on the following cases.
     """
```

## torchrec/distributed/sharding/cw_sequence_sharding.py

```diff
@@ -36,15 +36,14 @@
         self,
         device: Optional[torch.device] = None,
     ) -> BaseSparseFeaturesDist[KeyedJaggedTensor]:
         assert self._pg is not None
         return TwSparseFeaturesDist(
             self._pg,
             self.features_per_rank(),
-            device if device is not None else self._device,
         )
 
     def create_lookup(
         self,
         device: Optional[torch.device] = None,
         fused_params: Optional[Dict[str, Any]] = None,
         feature_processor: Optional[BaseGroupedFeatureProcessor] = None,
```

## torchrec/distributed/sharding/cw_sharding.py

```diff
@@ -8,33 +8,42 @@
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, TypeVar
 
 import torch
 import torch.distributed as dist  # noqa
 from fbgemm_gpu.permute_pooled_embedding_modules_split import (
     PermutePooledEmbeddingsSplit,
 )
-from torchrec.distributed.embedding_lookup import GroupedPooledEmbeddingsLookup
+from torchrec.distributed.dist_data import EmbeddingsAllToOne
+from torchrec.distributed.embedding_lookup import (
+    GroupedPooledEmbeddingsLookup,
+    InferGroupedPooledEmbeddingsLookup,
+)
 from torchrec.distributed.embedding_sharding import (
     BaseEmbeddingDist,
     BaseEmbeddingLookup,
     BaseSparseFeaturesDist,
     EmbeddingShardingContext,
     EmbeddingShardingInfo,
 )
 from torchrec.distributed.embedding_types import (
     BaseGroupedFeatureProcessor,
     EmbeddingComputeKernel,
+    KJTList,
     ShardedEmbeddingTable,
 )
 from torchrec.distributed.sharding.tw_sharding import (
     BaseTwEmbeddingSharding,
+    InferTwSparseFeaturesDist,
     TwPooledEmbeddingDist,
     TwSparseFeaturesDist,
 )
 from torchrec.distributed.types import (
+    Awaitable,
+    NoWait,
+    NullShardingContext,
     QuantizedCommCodecs,
     ShardedTensorMetadata,
     ShardingEnv,
     ShardMetadata,
 )
 from torchrec.sparse.jagged_tensor import KeyedJaggedTensor
 from torchrec.streamable import Multistreamable
@@ -128,16 +137,15 @@
         self._combined_embedding_names: List[str] = combined_embedding_names
         self._combined_embedding_dims: List[int] = combined_embedding_dims
 
     def _shard(
         self,
         sharding_infos: List[EmbeddingShardingInfo],
     ) -> List[List[ShardedEmbeddingTable]]:
-        # pyre-fixme[16]: `Optional` has no attribute `size`.
-        world_size = self._pg.size()
+        world_size: int = self._env.world_size
         tables_per_rank: List[List[ShardedEmbeddingTable]] = [
             [] for i in range(world_size)
         ]
         for info in sharding_infos:
             # pyre-fixme [16]
             shards: List[ShardMetadata] = info.param_sharding.sharding_spec.shards
 
@@ -209,15 +217,14 @@
         self,
         device: Optional[torch.device] = None,
     ) -> BaseSparseFeaturesDist[KeyedJaggedTensor]:
         assert self._pg is not None
         return TwSparseFeaturesDist(
             self._pg,
             self.features_per_rank(),
-            device if device is not None else self._device,
         )
 
     def create_lookup(
         self,
         device: Optional[torch.device] = None,
         fused_params: Optional[Dict[str, Any]] = None,
         feature_processor: Optional[BaseGroupedFeatureProcessor] = None,
@@ -249,7 +256,114 @@
         return TwPooledEmbeddingDist(
             self._pg,
             self._dim_sum_per_rank(),
             device,
             callbacks,
             qcomm_codecs_registry=self.qcomm_codecs_registry,
         )
+
+
+class InferCwPooledEmbeddingSharding(
+    BaseCwEmbeddingSharding[
+        NullShardingContext, KJTList, List[torch.Tensor], torch.Tensor
+    ]
+):
+    def create_input_dist(
+        self, device: Optional[torch.device] = None
+    ) -> BaseSparseFeaturesDist[KJTList]:
+        return InferTwSparseFeaturesDist(
+            self.features_per_rank(),
+            self._world_size,
+            device if device is not None else self._device,
+        )
+
+    def create_lookup(
+        self,
+        device: Optional[torch.device] = None,
+        fused_params: Optional[Dict[str, Any]] = None,
+        feature_processor: Optional[BaseGroupedFeatureProcessor] = None,
+    ) -> BaseEmbeddingLookup[KJTList, List[torch.Tensor]]:
+        return InferGroupedPooledEmbeddingsLookup(
+            grouped_configs_per_rank=self._grouped_embedding_configs_per_rank,
+            world_size=self._world_size,
+            fused_params=fused_params,
+            device=device if device is not None else self._device,
+        )
+
+    def create_output_dist(
+        self,
+        device: Optional[torch.device] = None,
+    ) -> BaseEmbeddingDist[NullShardingContext, List[torch.Tensor], torch.Tensor]:
+        device = device if device is not None else self._device
+        assert device is not None
+
+        dist_out = InferCwPooledEmbeddingDist(
+            device,
+            self._world_size,
+        )
+
+        if self._permute_embeddings and self._embedding_order != list(
+            range(len(self._embedding_order))
+        ):
+            return InferCwPooledEmbeddingDistWithPermute(
+                device, self._world_size, self._embedding_dims, self._embedding_order
+            )
+
+        return dist_out
+
+
+class InferCwPooledEmbeddingDist(
+    BaseEmbeddingDist[NullShardingContext, List[torch.Tensor], torch.Tensor]
+):
+    def __init__(
+        self,
+        device: torch.device,
+        world_size: int,
+    ) -> None:
+        super().__init__()
+        self._dist: EmbeddingsAllToOne = EmbeddingsAllToOne(
+            device=device, world_size=world_size, cat_dim=1
+        )
+
+    def forward(
+        self,
+        local_embs: List[torch.Tensor],
+        sharding_ctx: Optional[NullShardingContext] = None,
+    ) -> torch.Tensor:
+        return self._dist.forward(
+            local_embs,
+        )
+
+
+@torch.fx.wrap
+def _fx_wrap_permute(
+    permute_module: PermutePooledEmbeddingsSplit, input: torch.Tensor
+) -> torch.Tensor:
+    return permute_module.forward(input)
+
+
+class InferCwPooledEmbeddingDistWithPermute(
+    BaseEmbeddingDist[NullShardingContext, List[torch.Tensor], torch.Tensor]
+):
+    def __init__(
+        self,
+        device: torch.device,
+        world_size: int,
+        embedding_dims: List[int],
+        permute: List[int],
+    ) -> None:
+        super().__init__()
+        self._dist: EmbeddingsAllToOne = EmbeddingsAllToOne(
+            device=device, world_size=world_size, cat_dim=1
+        )
+        self._permute: PermutePooledEmbeddingsSplit = PermutePooledEmbeddingsSplit(
+            embs_dims=embedding_dims,
+            permute=permute,
+            device=device,
+        )
+
+    def forward(
+        self,
+        local_embs: List[torch.Tensor],
+        sharding_ctx: Optional[NullShardingContext] = None,
+    ) -> torch.Tensor:
+        return self._permute.forward(self._dist.forward(local_embs))
```

## torchrec/distributed/sharding/rw_sequence_sharding.py

```diff
@@ -1,31 +1,41 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 import torch
 import torch.distributed as dist
-from torchrec.distributed.dist_data import SequenceEmbeddingsAllToAll
-from torchrec.distributed.embedding_lookup import GroupedEmbeddingsLookup
+from torchrec.distributed.dist_data import (
+    SeqEmbeddingsAllToOne,
+    SequenceEmbeddingsAllToAll,
+)
+from torchrec.distributed.embedding_lookup import (
+    GroupedEmbeddingsLookup,
+    InferGroupedEmbeddingsLookup,
+)
 from torchrec.distributed.embedding_sharding import (
     BaseEmbeddingDist,
     BaseEmbeddingLookup,
     BaseSparseFeaturesDist,
 )
-from torchrec.distributed.embedding_types import BaseGroupedFeatureProcessor
+from torchrec.distributed.embedding_types import BaseGroupedFeatureProcessor, KJTList
 from torchrec.distributed.sharding.rw_sharding import (
     BaseRwEmbeddingSharding,
+    InferRwSparseFeaturesDist,
     RwSparseFeaturesDist,
 )
-from torchrec.distributed.sharding.sequence_sharding import SequenceShardingContext
+from torchrec.distributed.sharding.sequence_sharding import (
+    InferSequenceShardingContext,
+    SequenceShardingContext,
+)
 from torchrec.distributed.types import Awaitable, CommOp, QuantizedCommCodecs
 from torchrec.sparse.jagged_tensor import KeyedJaggedTensor
 
 
 class RwSequenceEmbeddingDist(
     BaseEmbeddingDist[SequenceShardingContext, torch.Tensor, torch.Tensor]
 ):
@@ -133,7 +143,79 @@
             # pyre-fixme[6]: For 1st param expected `ProcessGroup` but got
             #  `Optional[ProcessGroup]`.
             self._pg,
             self._get_num_features(),
             device if device is not None else self._device,
             qcomm_codecs_registry=self.qcomm_codecs_registry,
         )
+
+
+class InferRwSequenceEmbeddingDist(
+    BaseEmbeddingDist[
+        InferSequenceShardingContext, List[torch.Tensor], List[torch.Tensor]
+    ]
+):
+    def __init__(
+        self,
+        device: torch.device,
+        world_size: int,
+    ) -> None:
+        super().__init__()
+        self._dist: SeqEmbeddingsAllToOne = SeqEmbeddingsAllToOne(device, world_size)
+
+    def forward(
+        self,
+        local_embs: List[torch.Tensor],
+        sharding_ctx: Optional[InferSequenceShardingContext] = None,
+    ) -> List[torch.Tensor]:
+        return self._dist.forward(local_embs)
+
+
+class InferRwSequenceEmbeddingSharding(
+    BaseRwEmbeddingSharding[
+        InferSequenceShardingContext, KJTList, List[torch.Tensor], List[torch.Tensor]
+    ]
+):
+    """
+    Shards sequence (unpooled) row-wise, i.e.. a given embedding table is evenly
+    distributed by rows and table slices are placed on all ranks for inference.
+    """
+
+    def create_input_dist(
+        self,
+        device: Optional[torch.device] = None,
+    ) -> BaseSparseFeaturesDist[KJTList]:
+        num_features = self._get_num_features()
+        feature_hash_sizes = self._get_feature_hash_sizes()
+        return InferRwSparseFeaturesDist(
+            world_size=self._world_size,
+            num_features=num_features,
+            feature_hash_sizes=feature_hash_sizes,
+            device=device if device is not None else self._device,
+            is_sequence=True,
+            has_feature_processor=self._has_feature_processor,
+            need_pos=False,
+        )
+
+    def create_lookup(
+        self,
+        device: Optional[torch.device] = None,
+        fused_params: Optional[Dict[str, Any]] = None,
+        feature_processor: Optional[BaseGroupedFeatureProcessor] = None,
+    ) -> BaseEmbeddingLookup[KJTList, List[torch.Tensor]]:
+        return InferGroupedEmbeddingsLookup(
+            grouped_configs_per_rank=self._grouped_embedding_configs_per_rank,
+            world_size=self._world_size,
+            fused_params=fused_params,
+            device=device if device is not None else self._device,
+        )
+
+    def create_output_dist(
+        self,
+        device: Optional[torch.device] = None,
+    ) -> BaseEmbeddingDist[
+        InferSequenceShardingContext, List[torch.Tensor], List[torch.Tensor]
+    ]:
+        return InferRwSequenceEmbeddingDist(
+            device if device is not None else self._device,
+            self._world_size,
+        )
```

## torchrec/distributed/sharding/rw_sharding.py

```diff
@@ -5,40 +5,51 @@
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Any, Dict, List, Optional, TypeVar
 
 import torch
 import torch.distributed as dist
-from torchrec.distributed.dist_data import KJTAllToAll, PooledEmbeddingsReduceScatter
-from torchrec.distributed.embedding_lookup import GroupedPooledEmbeddingsLookup
+from torchrec.distributed.dist_data import (
+    EmbeddingsAllToOneReduce,
+    KJTAllToAll,
+    KJTOneToAll,
+    PooledEmbeddingsReduceScatter,
+)
+from torchrec.distributed.embedding_lookup import (
+    GroupedPooledEmbeddingsLookup,
+    InferGroupedPooledEmbeddingsLookup,
+)
 from torchrec.distributed.embedding_sharding import (
     BaseEmbeddingDist,
     BaseEmbeddingLookup,
     BaseSparseFeaturesDist,
     bucketize_kjt_before_all2all,
     EmbeddingSharding,
     EmbeddingShardingContext,
     EmbeddingShardingInfo,
     group_tables,
 )
 from torchrec.distributed.embedding_types import (
     BaseGroupedFeatureProcessor,
     EmbeddingComputeKernel,
     GroupedEmbeddingConfig,
+    KJTList,
     ShardedEmbeddingTable,
 )
 from torchrec.distributed.types import (
     Awaitable,
     CommOp,
+    NullShardingContext,
     QuantizedCommCodecs,
     ShardedTensorMetadata,
     ShardingEnv,
     ShardMetadata,
 )
+from torchrec.fx.utils import assert_fx_safe
 from torchrec.sparse.jagged_tensor import KeyedJaggedTensor
 from torchrec.streamable import Multistreamable
 
 
 C = TypeVar("C", bound=Multistreamable)
 F = TypeVar("F", bound=Multistreamable)
 T = TypeVar("T")
@@ -64,15 +75,15 @@
 
         self._env = env
         self._pg: Optional[dist.ProcessGroup] = self._env.process_group
         self._world_size: int = self._env.world_size
         self._rank: int = self._env.rank
         if device is None:
             device = torch.device("cpu")
-        self._device = device
+        self._device: torch.device = device
         sharded_tables_per_rank = self._shard(sharding_infos)
         self._need_pos = need_pos
         self._grouped_embedding_configs_per_rank: List[
             List[GroupedEmbeddingConfig]
         ] = []
         self._grouped_embedding_configs_per_rank = group_tables(sharded_tables_per_rank)
         self._grouped_embedding_configs: List[
@@ -141,15 +152,21 @@
     def embedding_names(self) -> List[str]:
         embedding_names = []
         for grouped_config in self._grouped_embedding_configs:
             embedding_names.extend(grouped_config.embedding_names())
         return embedding_names
 
     def embedding_names_per_rank(self) -> List[List[str]]:
-        raise NotImplementedError
+        embedding_names = []
+        for grouped_embedding_configs in self._grouped_embedding_configs_per_rank:
+            embedding_names_per_rank = []
+            for grouped_config in grouped_embedding_configs:
+                embedding_names_per_rank.extend(grouped_config.embedding_names())
+            embedding_names.append(embedding_names_per_rank)
+        return embedding_names
 
     def embedding_shard_metadata(self) -> List[Optional[ShardMetadata]]:
         embedding_shard_metadata = []
         for grouped_config in self._grouped_embedding_configs:
             embedding_shard_metadata.extend(grouped_config.embedding_shard_metadata())
         return embedding_shard_metadata
 
@@ -213,16 +230,15 @@
                 feature_block_sizes,
                 device=device,
                 dtype=torch.int32,
             ),
         )
         self._dist = KJTAllToAll(
             pg=pg,
-            splits=self._world_size * [self._num_features],
-            device=device,
+            splits=[self._num_features] * self._world_size,
         )
         self._is_sequence = is_sequence
         self._has_feature_processor = has_feature_processor
         self._need_pos = need_pos
         self.unbucketize_permute_tensor: Optional[torch.Tensor] = None
 
     def forward(
@@ -301,14 +317,57 @@
 
         if sharding_ctx is None:
             return self._dist(local_embs)
         else:
             return self._dist(local_embs, input_splits=sharding_ctx.batch_size_per_rank)
 
 
+class InferRwPooledEmbeddingDist(
+    BaseEmbeddingDist[NullShardingContext, List[torch.Tensor], torch.Tensor]
+):
+    """
+    Redistributes sequence embedding tensor in RW fashion with an AlltoOne operation.
+
+    Args:
+        device (torch.device): device on which the tensors will be communicated to.
+        world_size (int): number of devices in the topology.
+    """
+
+    def __init__(
+        self,
+        device: torch.device,
+        world_size: int,
+    ) -> None:
+        super().__init__()
+        self._dist: EmbeddingsAllToOneReduce = EmbeddingsAllToOneReduce(
+            device=device,
+            world_size=world_size,
+            cat_dim=1,
+        )
+
+    def forward(
+        self,
+        local_embs: List[torch.Tensor],
+        sharding_ctx: Optional[NullShardingContext] = None,
+    ) -> torch.Tensor:
+        """
+        Performs AlltoOne operation on sequence embeddings tensor.
+
+        Args:
+            local_embs (torch.Tensor): tensor of values to distribute.
+
+        Returns:
+            Awaitable[torch.Tensor]: awaitable of sequence embeddings.
+        """
+
+        return self._dist.forward(
+            local_embs,
+        )
+
+
 class RwPooledEmbeddingSharding(
     BaseRwEmbeddingSharding[
         EmbeddingShardingContext, KeyedJaggedTensor, torch.Tensor, torch.Tensor
     ]
 ):
     """
     Shards embedding bags row-wise, i.e.. a given embedding table is evenly distributed
@@ -352,7 +411,104 @@
     ) -> BaseEmbeddingDist[EmbeddingShardingContext, torch.Tensor, torch.Tensor]:
         return RwPooledEmbeddingDist(
             # pyre-fixme[6]: For 1st param expected `ProcessGroup` but got
             #  `Optional[ProcessGroup]`.
             self._pg,
             qcomm_codecs_registry=self.qcomm_codecs_registry,
         )
+
+
+class InferRwSparseFeaturesDist(BaseSparseFeaturesDist[KJTList]):
+    def __init__(
+        self,
+        world_size: int,
+        num_features: int,
+        feature_hash_sizes: List[int],
+        device: Optional[torch.device] = None,
+        is_sequence: bool = False,
+        has_feature_processor: bool = False,
+        need_pos: bool = False,
+    ) -> None:
+        super().__init__()
+        self._world_size: int = world_size
+        self._num_features = num_features
+        feature_block_sizes = [
+            (hash_size + self._world_size - 1) // self._world_size
+            for hash_size in feature_hash_sizes
+        ]
+        self.register_buffer(
+            "_feature_block_sizes_tensor",
+            torch.tensor(
+                feature_block_sizes,
+                device=device,
+                dtype=torch.int32,
+            ),
+        )
+        self._dist = KJTOneToAll(
+            splits=self._world_size * [self._num_features],
+            world_size=world_size,
+            device=device,
+        )
+        self._is_sequence = is_sequence
+        self._has_feature_processor = has_feature_processor
+        self._need_pos = need_pos
+        self.unbucketize_permute_tensor: Optional[torch.Tensor] = None
+
+    def forward(
+        self,
+        sparse_features: KeyedJaggedTensor,
+    ) -> KJTList:
+        (
+            bucketized_features,
+            self.unbucketize_permute_tensor,
+        ) = bucketize_kjt_before_all2all(
+            sparse_features,
+            num_buckets=self._world_size,
+            block_sizes=self._feature_block_sizes_tensor,
+            output_permute=self._is_sequence,
+            bucketize_pos=self._has_feature_processor
+            if sparse_features.weights_or_none() is None
+            else self._need_pos,
+        )
+        return self._dist.forward(bucketized_features)
+
+
+class InferRwPooledEmbeddingSharding(
+    BaseRwEmbeddingSharding[
+        NullShardingContext, KJTList, List[torch.Tensor], torch.Tensor
+    ]
+):
+    def create_input_dist(
+        self,
+        device: Optional[torch.device] = None,
+    ) -> BaseSparseFeaturesDist[KJTList]:
+        num_features = self._get_num_features()
+        feature_hash_sizes = self._get_feature_hash_sizes()
+        return InferRwSparseFeaturesDist(
+            world_size=self._world_size,
+            num_features=num_features,
+            feature_hash_sizes=feature_hash_sizes,
+            device=device if device is not None else self._device,
+        )
+
+    def create_lookup(
+        self,
+        device: Optional[torch.device] = None,
+        fused_params: Optional[Dict[str, Any]] = None,
+        feature_processor: Optional[BaseGroupedFeatureProcessor] = None,
+    ) -> BaseEmbeddingLookup[KJTList, List[torch.Tensor]]:
+        return InferGroupedPooledEmbeddingsLookup(
+            grouped_configs_per_rank=self._grouped_embedding_configs_per_rank,
+            world_size=self._world_size,
+            fused_params=fused_params,
+            device=device if device is not None else self._device,
+        )
+
+    def create_output_dist(
+        self,
+        device: Optional[torch.device] = None,
+    ) -> BaseEmbeddingDist[NullShardingContext, List[torch.Tensor], torch.Tensor]:
+        assert device is not None
+        return InferRwPooledEmbeddingDist(
+            device=device,
+            world_size=self._world_size,
+        )
```

## torchrec/distributed/sharding/sequence_sharding.py

```diff
@@ -56,18 +56,24 @@
 
 @dataclass
 class InferSequenceShardingContext(Multistreamable):
     """
     Stores inference context and reuses it in sequence embedding output_dist or result return.
 
     Attributes:
-        features (Optional[List[KeyedJaggedTensor]]): stores the original
-            shards of KJT after input dist.
+        features KJTList: stores the shards of KJT after input dist.
+        features_before_input_dist KJT: stores the original input KJT (before input dist).
+        unbucketize_permute_tensor Optional[torch.Tensor]: stores unbucketize tensor, only for RowWise sharding.
     """
 
-    features: Optional[KJTList] = None
+    features: KJTList
+    features_before_input_dist: Optional[KeyedJaggedTensor] = None
+    unbucketize_permute_tensor: Optional[torch.Tensor] = None
 
     def record_stream(self, stream: torch.cuda.streams.Stream) -> None:
-        if self.features is not None:
-            # pyre-ignore [16]
-            for feature in self.features:
-                feature.record_stream(stream)
+        for feature in self.features:
+            feature.record_stream(stream)
+        if self.features_before_input_dist is not None:
+            self.features_before_input_dist.record_stream(stream)
+        if self.unbucketize_permute_tensor is not None:
+            # pyre-fixme[6]: For 1st param expected `Stream` but got `Stream`.
+            self.unbucketize_permute_tensor.record_stream(stream)
```

## torchrec/distributed/sharding/tw_sequence_sharding.py

```diff
@@ -112,15 +112,14 @@
         device: Optional[torch.device] = None,
     ) -> BaseSparseFeaturesDist[KeyedJaggedTensor]:
         return TwSparseFeaturesDist(
             # pyre-fixme[6]: For 1st param expected `ProcessGroup` but got
             #  `Optional[ProcessGroup]`.
             self._pg,
             self.features_per_rank(),
-            device if device is not None else self._device,
         )
 
     def create_lookup(
         self,
         device: Optional[torch.device] = None,
         fused_params: Optional[Dict[str, Any]] = None,
         feature_processor: Optional[BaseGroupedFeatureProcessor] = None,
```

## torchrec/distributed/sharding/tw_sharding.py

```diff
@@ -206,28 +206,25 @@
     """
     Redistributes sparse features with an AlltoAll collective operation for table wise
     sharding.
 
     Args:
         pg (dist.ProcessGroup): ProcessGroup for AlltoAll communication.
         features_per_rank (List[int]): number of features to send to each rank.
-        device (Optional[torch.device]): device on which buffers will be allocated.
     """
 
     def __init__(
         self,
         pg: dist.ProcessGroup,
         features_per_rank: List[int],
-        device: Optional[torch.device] = None,
     ) -> None:
         super().__init__()
         self._dist = KJTAllToAll(
             pg=pg,
             splits=features_per_rank,
-            device=device,
         )
 
     def forward(
         self,
         sparse_features: KeyedJaggedTensor,
     ) -> Awaitable[Awaitable[KeyedJaggedTensor]]:
         """
@@ -316,15 +313,14 @@
         self,
         device: Optional[torch.device] = None,
     ) -> BaseSparseFeaturesDist[KeyedJaggedTensor]:
         assert self._pg is not None
         return TwSparseFeaturesDist(
             self._pg,
             self.features_per_rank(),
-            device if device is not None else self._device,
         )
 
     def create_lookup(
         self,
         device: Optional[torch.device] = None,
         fused_params: Optional[Dict[str, Any]] = None,
         feature_processor: Optional[BaseGroupedFeatureProcessor] = None,
```

## torchrec/distributed/sharding/twrw_sharding.py

```diff
@@ -302,15 +302,14 @@
                 device=device,
                 dtype=torch.int32,
             ),
         )
         self._dist = KJTAllToAll(
             pg=pg,
             splits=features_per_rank,
-            device=device,
             stagger=self._num_cross_nodes,
         )
         self._has_feature_processor = has_feature_processor
         self._need_pos = need_pos
 
     def forward(
         self,
```

## torchrec/distributed/test_utils/infer_utils.py

```diff
@@ -11,15 +11,18 @@
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import torch
 import torchrec
 from torch import quantization as quant
 from torchrec import EmbeddingCollection, EmbeddingConfig, KeyedJaggedTensor
 from torchrec.distributed.embedding_types import ModuleSharder
-from torchrec.distributed.fused_params import FUSED_PARAM_REGISTER_TBE_BOOL
+from torchrec.distributed.fused_params import (
+    FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS,
+    FUSED_PARAM_REGISTER_TBE_BOOL,
+)
 from torchrec.distributed.planner import EmbeddingShardingPlanner, Topology
 from torchrec.distributed.quant_embedding import (
     QuantEmbeddingCollectionSharder,
     ShardedQuantEmbeddingCollection,
 )
 from torchrec.distributed.quant_embeddingbag import (
     QuantEmbeddingBagCollection,
@@ -34,14 +37,16 @@
     data_type_to_sparse_type,
     dtype_to_data_type,
     EmbeddingBagConfig,
 )
 from torchrec.modules.embedding_modules import EmbeddingBagCollection
 from torchrec.quant.embedding_modules import (
     EmbeddingCollection as QuantEmbeddingCollection,
+    MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS,
+    MODULE_ATTR_REGISTER_TBES_BOOL,
     quant_prep_enable_quant_state_dict_split_scale_bias_for_types,
     quant_prep_enable_register_tbes,
 )
 
 
 @dataclass
 class TestModelInfo:
@@ -204,31 +209,38 @@
         env: ShardingEnv,
         device: Optional[torch.device] = None,
     ) -> ShardedQuantEmbeddingBagCollection:
         fused_params = self.fused_params if self.fused_params else {}
         fused_params["output_dtype"] = data_type_to_sparse_type(
             dtype_to_data_type(module.output_dtype())
         )
-        fused_params[FUSED_PARAM_REGISTER_TBE_BOOL] = True
+        fused_params[FUSED_PARAM_REGISTER_TBE_BOOL] = getattr(
+            module, MODULE_ATTR_REGISTER_TBES_BOOL, False
+        )
+        fused_params[FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS] = getattr(
+            module, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, False
+        )
         return ShardedQuantEmbeddingBagCollection(
             module=module,
             table_name_to_parameter_sharding=params,
             env=env,
             fused_params=fused_params,
             device=device,
         )
 
 
 class TestQuantECSharder(QuantEmbeddingCollectionSharder):
     def __init__(
         self,
         sharding_type: str,
         kernel_type: str,
+        fused_params: Optional[Dict[str, Any]] = None,
+        shardable_params: Optional[List[str]] = None,
     ) -> None:
-        super().__init__()
+        super().__init__(fused_params=fused_params, shardable_params=shardable_params)
         self._sharding_type = sharding_type
         self._kernel_type = kernel_type
 
     def sharding_types(self, compute_device_type: str) -> List[str]:
         return [self._sharding_type]
 
     def compute_kernels(
@@ -243,15 +255,20 @@
         env: ShardingEnv,
         device: Optional[torch.device] = None,
     ) -> ShardedQuantEmbeddingCollection:
         fused_params = self.fused_params if self.fused_params else {}
         fused_params["output_dtype"] = data_type_to_sparse_type(
             dtype_to_data_type(module.output_dtype())
         )
-        fused_params[FUSED_PARAM_REGISTER_TBE_BOOL] = True
+        fused_params[FUSED_PARAM_REGISTER_TBE_BOOL] = getattr(
+            module, MODULE_ATTR_REGISTER_TBES_BOOL, False
+        )
+        fused_params[FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS] = getattr(
+            module, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, False
+        )
         return ShardedQuantEmbeddingCollection(
             module, params, env, fused_params, device
         )
 
 
 class KJTInputWrapper(torch.nn.Module):
     def __init__(
```

## torchrec/distributed/test_utils/test_model.py

```diff
@@ -275,18 +275,18 @@
         super().__init__()
         if device is None:
             device = torch.device("cpu")
         self.linear: nn.modules.Linear = nn.Linear(
             in_features=num_float_features, out_features=8, device=device
         )
 
-        self.dummy_param = torch.nn.Parameter(torch.empty(2, device=device))
+        self.dummy_param = torch.nn.Parameter(torch.zeros(2, device=device))
         self.register_buffer(
             "dummy_buffer",
-            torch.nn.Parameter(torch.empty(1, device=device)),
+            torch.nn.Parameter(torch.zeros(1, device=device)),
         )
 
     def forward(self, dense_input: torch.Tensor) -> torch.Tensor:
         return self.linear(dense_input)
 
 
 class TestOverArch(nn.Module):
@@ -708,17 +708,15 @@
         )
         self.sparse_arch_feature_names: List[str] = (
             tables[1].feature_names + weighted_tables[0].feature_names
         )
 
         self.over = nn.Linear(
             in_features=8
-            # pyre-ignore [16]
             + self.tower_0.interaction.linear.out_features
-            # pyre-ignore [16]
             + self.tower_1.interaction.linear.out_features
             + tables[1].embedding_dim * len(tables[1].feature_names)
             + weighted_tables[0].embedding_dim * len(weighted_tables[0].feature_names),
             out_features=16,
             device=dense_device,
         )
 
@@ -802,19 +800,16 @@
                 is_weighted=True,
             ),
             interaction_module=TestTowerInteraction(tables=[weighted_tables[0]]),
         )
         self.tower_arch = EmbeddingTowerCollection(towers=[tower_0, tower_1, tower_2])
         self.over = nn.Linear(
             in_features=8
-            # pyre-ignore [16]
             + tower_0.interaction.linear.out_features
-            # pyre-ignore [16]
             + tower_1.interaction.linear.out_features
-            # pyre-ignore [16]
             + tower_2.interaction.linear.out_features,
             out_features=16,
             device=dense_device,
         )
 
     def forward(
         self,
```

## torchrec/distributed/test_utils/test_model_parallel.py

```diff
@@ -107,15 +107,15 @@
         torch.cuda.device_count() <= 1,
         "Not enough GPUs, this test requires at least two GPUs",
     )
     # pyre-fixme[56]
     @given(
         sharder_type=st.sampled_from(
             [
-                SharderType.EMBEDDING_BAG.value,
+                # SharderType.EMBEDDING_BAG.value,
                 SharderType.EMBEDDING_BAG_COLLECTION.value,
             ]
         ),
         qcomms_config=st.sampled_from(
             [
                 None,
                 QCommsConfig(
@@ -169,15 +169,15 @@
             variable_batch_size=variable_batch_size,
         )
 
     # pyre-fixme[56]
     @given(
         sharder_type=st.sampled_from(
             [
-                SharderType.EMBEDDING_BAG.value,
+                # SharderType.EMBEDDING_BAG.value,
                 SharderType.EMBEDDING_BAG_COLLECTION.value,
             ]
         ),
         apply_optimizer_in_backward_config=st.sampled_from([None]),
         # TODO - need to enable optimizer overlapped behavior for data_parallel tables
     )
     @settings(verbosity=Verbosity.verbose, max_examples=3, deadline=None)
```

## torchrec/distributed/test_utils/test_model_parallel_base.py

```diff
@@ -506,15 +506,15 @@
             self.assertTrue(torch.equal(src, dst))
 
     # pyre-ignore[56]
     @given(
         sharders=st.sampled_from(
             [
                 [EmbeddingBagCollectionSharder()],
-                [EmbeddingBagSharder()],
+                # [EmbeddingBagSharder()],
             ]
         ),
     )
     @settings(verbosity=Verbosity.verbose, max_examples=2, deadline=None)
     def test_load_state_dict_prefix(
         self, sharders: List[ModuleSharder[nn.Module]]
     ) -> None:
```

## torchrec/fx/tracer.py

```diff
@@ -127,15 +127,14 @@
     def path_of_module(self, mod: torch.nn.Module) -> str:
         """
         Allows trace-ability of non registered modules. This is typically used for Table Batched Embeddings
         made to look like nn.EmbeddingBags
         """
 
         if hasattr(mod, "_fx_path"):
-            # pyre-ignore
             return mod._fx_path
         else:
             return super().path_of_module(mod)
 
 
 def symbolic_trace(
     # pyre-ignore[24]
```

## torchrec/fx/utils.py

```diff
@@ -13,15 +13,14 @@
 from torch.fx._symbolic_trace import is_fx_tracing
 
 # Not importing DistributedModelParallel here to avoid circular dependencies as DMP depends on torchrec.fx.tracer
 # def dmp_fx_trace_forward(dmp: DistributedModelParallel)
 
 # pyre-ignore
 def fake_range():
-    # pyre-ignore
     return torch._C._jit_tree_views.SourceRangeFactory("", None, 0, 0).make_raw_range(
         0, 1
     )
 
 
 # pyre-ignore
 def dmp_fx_trace_forward(  # noqa: C901
@@ -139,7 +138,13 @@
     # bool() syntax for pyre
     return bool(
         node.op == "call_function"
         and node.target == _fx_marker
         and isinstance(node.args[0], str)
         and node.args[0] == marker_name
     )
+
+
+@torch.jit.ignore
+def assert_fx_safe(condition: bool, message: str) -> None:
+    if not is_fx_tracing():
+        assert condition, message
```

## torchrec/metrics/metrics_config.py

```diff
@@ -25,14 +25,15 @@
     MSE = "mse"
     MAE = "mae"
     MULTICLASS_RECALL = "multiclass_recall"
     RECALL_SESSION_LEVEL = "recall_session_level"
     WEIGHTED_AVG = "weighted_avg"
     TOWER_QPS = "tower_qps"
     ACCURACY = "accuracy"
+    NDCG = "ndcg"
 
 
 @dataclass(unsafe_hash=True, eq=True)
 class SessionMetricDef:
     # hyperparameters required for session level metrics
     # session_var_name: name of session tensor in the model_out
     # top_threshold: predictiones ranked in top "top_threshold" are considered as positive
```

## torchrec/metrics/metrics_namespace.py

```diff
@@ -49,14 +49,15 @@
     AUC = "auc"
     GROUPED_AUC = "grouped_auc"
     RECALL_SESSION_LEVEL = "recall_session_level"
     MULTICLASS_RECALL = "multiclass_recall"
     WEIGHTED_AVG = "weighted_avg"
     TOWER_QPS = "qps"
     ACCURACY = "accuracy"
+    NDCG = "ndcg"
 
 
 class MetricNamespaceBase(StrValueMixin, Enum):
     pass
 
 
 class MetricNamespace(MetricNamespaceBase):
@@ -76,14 +77,15 @@
 
     MULTICLASS_RECALL = "multiclass_recall"
 
     WEIGHTED_AVG = "weighted_avg"
     RECALL_SESSION_LEVEL = "recall_session_level"
 
     TOWER_QPS = "qps"
+    NDCG = "ndcg"
 
 
 class MetricPrefix(StrValueMixin, Enum):
     DEFAULT = ""
     LIFETIME = "lifetime_"
     WINDOW = "window_"
```

## torchrec/models/dlrm.py

```diff
@@ -94,22 +94,20 @@
 
         Returns:
             torch.Tensor: tensor of shape B X F X D.
         """
 
         sparse_features: KeyedTensor = self.embedding_bag_collection(features)
 
-        B: int = features.stride()
-
         sparse: Dict[str, torch.Tensor] = sparse_features.to_dict()
         sparse_values: List[torch.Tensor] = []
         for name in self.sparse_feature_names:
             sparse_values.append(sparse[name])
 
-        return torch.cat(sparse_values, dim=1).reshape(B, self.F, self.D)
+        return torch.cat(sparse_values, dim=1).reshape(-1, self.F, self.D)
 
     @property
     def sparse_feature_names(self) -> List[str]:
         return self._sparse_feature_names
 
 
 class DenseArch(nn.Module):
```

## torchrec/modules/crossnet.py

```diff
@@ -77,17 +77,15 @@
         Returns:
             torch.Tensor: tensor with shape [batch_size, in_features].
         """
         x_0 = input.unsqueeze(2)  # (B, N, 1)
         x_l = x_0
 
         for layer in range(self._num_layers):
-            # pyre-ignore[29]: `Union[torch.Tensor, torch.nn.Module]` is not a function.
             xl_w = torch.matmul(self.kernels[layer], x_l)  # (B, N, 1)
-            # pyre-ignore[29]: `Union[torch.Tensor, torch.nn.Module]` is not a function.
             x_l = x_0 * (xl_w + self.bias[layer]) + x_l  # (B, N, 1)
 
         return torch.squeeze(x_l, dim=2)
 
 
 class LowRankCrossNet(torch.nn.Module):
     r"""
@@ -246,20 +244,17 @@
 
         x_0 = input.unsqueeze(2)  # (B, N, 1)
         x_l = x_0
 
         for layer in range(self._num_layers):
             xl_w = torch.tensordot(
                 x_l,
-                # pyre-ignore[29]: `Union[torch.Tensor, torch.nn.Module]` is not a
-                #  function.
                 self.kernels[layer],
                 dims=([1], [0]),
             )  # (B, 1, 1)
-            # pyre-ignore[29]: `Union[torch.Tensor, torch.nn.Module]` is not a function.
             x_l = torch.matmul(x_0, xl_w) + self.bias[layer] + x_l  # (B, N, 1)
 
         return torch.squeeze(x_l, dim=2)  # (B, N)
 
 
 class LowRankMixtureCrossNet(torch.nn.Module):
     r"""
@@ -402,29 +397,25 @@
                     gating.append(self.gates[i](x_l.squeeze(2)))
                 gating = torch.stack(gating, 1)  # (B, K, 1)
 
             # set up experts
             experts = []
             for i in range(self._num_experts):
                 expert = torch.matmul(
-                    # pyre-ignore[29]
                     self.V_kernels[layer][i],
                     x_l,
                 )  # (B, r, 1)
                 expert = torch.matmul(
-                    # pyre-ignore[29]
                     self.C_kernels[layer][i],
                     self._activation(expert),
                 )  # (B, r, 1)
                 expert = torch.matmul(
-                    # pyre-ignore[29]
                     self.U_kernels[layer][i],
                     self._activation(expert),
                 )  # (B, N, 1)
-                # pyre-ignore[29]
                 expert = x_0 * (expert + self.bias[layer])  # (B, N, 1)
                 experts.append(expert.squeeze(2))  # (B, N)
             experts = torch.stack(experts, 2)  # (B, N, K)
 
             if self._num_experts > 1:
                 # MOE update
                 moe = torch.matmul(
```

## torchrec/modules/embedding_configs.py

```diff
@@ -9,59 +9,71 @@
 from enum import Enum, unique
 from functools import partial
 from math import sqrt
 from typing import Callable, Dict, List, Optional
 
 import torch
 from fbgemm_gpu.split_embedding_configs import SparseType
-from fbgemm_gpu.split_table_batched_embeddings_ops_training import PoolingMode
+from fbgemm_gpu.split_table_batched_embeddings_ops_training import (
+    BoundsCheckMode as FbgemmBoundsCheckMode,
+    CacheAlgorithm as FbgemmCacheAlgorithm,
+    PoolingMode,
+)
+from torchrec.distributed.types import BoundsCheckMode, CacheAlgorithm, DataType
 
 
 @unique
 class PoolingType(Enum):
     SUM = "SUM"
     MEAN = "MEAN"
     NONE = "NONE"
 
 
-@unique
-class DataType(Enum):
-    """
-    Our fusion implementation supports only certain types of data
-    so it makes sense to retrict in a non-fused version as well.
-    """
-
-    FP32 = "FP32"
-    FP16 = "FP16"
-    INT64 = "INT64"
-    INT32 = "INT32"
-    INT8 = "INT8"
-    UINT8 = "UINT8"
-    INT4 = "INT4"
-    INT2 = "INT2"
-
-    def __str__(self) -> str:
-        return self.value
-
-
 DATA_TYPE_NUM_BITS: Dict[DataType, int] = {
     DataType.FP32: 32,
     DataType.FP16: 16,
+    DataType.BF16: 16,
     DataType.INT8: 8,
     DataType.UINT8: 8,
     DataType.INT4: 4,
     DataType.INT2: 2,
 }
 
 
+def to_fbgemm_bounds_check_mode(
+    bounds_check_mode: BoundsCheckMode,
+) -> FbgemmBoundsCheckMode:
+    if bounds_check_mode == BoundsCheckMode.FATAL:
+        return FbgemmBoundsCheckMode.FATAL
+    elif bounds_check_mode == BoundsCheckMode.WARNING:
+        return FbgemmBoundsCheckMode.WARNING
+    elif bounds_check_mode == BoundsCheckMode.IGNORE:
+        return FbgemmBoundsCheckMode.IGNORE
+    elif bounds_check_mode == BoundsCheckMode.NONE:
+        return FbgemmBoundsCheckMode.NONE
+    else:
+        raise Exception(f"Invalid bounds check mode {bounds_check_mode}")
+
+
+def to_fbgemm_cache_algorithm(cache_algorithm: CacheAlgorithm) -> FbgemmCacheAlgorithm:
+    if cache_algorithm == CacheAlgorithm.LRU:
+        return FbgemmCacheAlgorithm.LRU
+    elif cache_algorithm == CacheAlgorithm.LFU:
+        return FbgemmCacheAlgorithm.LFU
+    else:
+        raise Exception(f"Invalid cache algorithm {cache_algorithm}")
+
+
 def dtype_to_data_type(dtype: torch.dtype) -> DataType:
     if dtype == torch.float:
         return DataType.FP32
     elif dtype == torch.float16 or dtype == torch.half:
         return DataType.FP16
+    elif dtype == torch.bfloat16:
+        return DataType.BF16
     elif dtype in {torch.int, torch.int32}:
         return DataType.INT32
     elif dtype in {torch.long, torch.int64}:
         return DataType.INT64
     elif dtype in {torch.quint8, torch.qint8, torch.int8}:
         return DataType.INT8
     elif dtype == torch.uint8:
@@ -95,14 +107,16 @@
 
 
 def data_type_to_sparse_type(data_type: DataType) -> SparseType:
     if data_type == DataType.FP32:
         return SparseType.FP32
     elif data_type == DataType.FP16:
         return SparseType.FP16
+    elif data_type == DataType.BF16:
+        return SparseType.BF16
     elif data_type == DataType.INT8 or data_type == DataType.UINT8:
         return SparseType.INT8
     elif data_type == DataType.INT4:
         return SparseType.INT4
     elif data_type == DataType.INT2:
         return SparseType.INT2
     else:
@@ -110,14 +124,16 @@
 
 
 def data_type_to_dtype(data_type: DataType) -> torch.dtype:
     if data_type == DataType.FP32:
         return torch.float32
     elif data_type == DataType.FP16:
         return torch.float16
+    elif data_type == DataType.BF16:
+        return torch.bfloat16
     elif data_type == DataType.INT64:
         return torch.int64
     elif data_type == DataType.INT32:
         return torch.int32
     elif data_type == DataType.INT8:
         return torch.int8
     elif data_type == DataType.UINT8:
```

## torchrec/modules/feature_processor_.py

```diff
@@ -150,24 +150,24 @@
         cat_seq = torch.ops.fbgemm.offsets_range(
             features.offsets().long(), torch.numel(features.values())
         )
 
         seqs = torch.split(cat_seq, features.length_per_key())
         weights_list = []
         for key, seq in zip(features.keys(), seqs):
-            if key in self.max_feature_lengths:
+            if key in self.position_weights:
                 weights_list.append(
                     torch.gather(self.position_weights[key], dim=0, index=seq)
                 )
             else:
                 weights_list.append(
-                    self._dummy_weights[: self.max_feature_lengths[key]]
+                    torch.ones(seq.shape[0], device=features.values().device)
                 )
-        weights = torch.cat(weights_list)
 
+        weights = torch.cat(weights_list)
         return KeyedJaggedTensor(
             keys=features.keys(),
             values=features.values(),
             weights=weights,
             lengths=features.lengths(),
             offsets=features.offsets(),
             stride=features.stride(),
```

## torchrec/modules/fused_embedding_modules.py

```diff
@@ -350,14 +350,17 @@
         device: Optional[torch.device] = None,
         location: Optional[EmbeddingLocation] = None,
     ) -> None:
         super().__init__()
 
         self._optimizer_type = optimizer_type
         self._optimizer_kwargs = optimizer_kwargs
+        self._device: torch.device = (
+            device if device is not None else torch.device("cpu")
+        )
 
         emb_optim_and_kwargs = convert_optimizer_type_and_kwargs(
             optimizer_type, optimizer_kwargs
         )
         if emb_optim_and_kwargs is None:
             raise ValueError(
                 f"Cannot fuse optimizer_type={optimizer_type} with kwargs {optimizer_kwargs}"
@@ -434,15 +437,15 @@
         # nn.Module API calls (state_dict, named_modules, etc)
         self.embedding_bags: nn.ModuleDict = nn.ModuleDict()
         for (_key, tables), emb_module in zip(
             self._key_to_tables.items(), self._emb_modules
         ):
             for embedding_config, weight in zip(
                 tables,
-                emb_module.split_embedding_weights(),  # pyre-fixme[29]: `Union[nn.modules.module.Module,
+                emb_module.split_embedding_weights(),
                 #  torch._tensor.Tensor]` is not a function.
             ):
                 self.embedding_bags[embedding_config.name] = torch.nn.Module()
                 self.embedding_bags[embedding_config.name].register_parameter(
                     "weight", torch.nn.Parameter(weight)
                 )
 
@@ -496,14 +499,18 @@
             values=embeddings,
             length_per_key=self._length_per_key,
         )
 
     def _get_name(self) -> str:
         return "FusedEmbeddingBagCollection"
 
+    @property
+    def device(self) -> torch.device:
+        return self._device
+
     def embedding_bag_configs(self) -> List[EmbeddingBagConfig]:
         return self._embedding_bag_configs
 
     def is_weighted(self) -> bool:
         return self._is_weighted
 
     def optimizer_type(self) -> Type[torch.optim.Optimizer]:
@@ -682,15 +689,15 @@
         # nn.Module API calls (state_dict, named_modules, etc)
         self.embeddings: nn.ModuleDict = nn.ModuleDict()
         for (_key, tables), emb_module in zip(
             self._key_to_tables.items(), self._emb_modules
         ):
             for embedding_config, weight in zip(
                 tables,
-                emb_module.split_embedding_weights(),  # pyre-fixme[29]: `Union[nn.modules.module.Module,
+                emb_module.split_embedding_weights(),
                 #  torch._tensor.Tensor]` is not a function.
             ):
                 self.embeddings[embedding_config.name] = torch.nn.Module()
                 self.embeddings[embedding_config.name].register_parameter(
                     "weight", torch.nn.Parameter(weight)
                 )
```

## torchrec/modules/lazy_extension.py

```diff
@@ -24,22 +24,17 @@
     # pyre-ignore[2]
     input: Any,
     # pyre-ignore[2]
     output: Any,
 ) -> None:
     _functions_to_lazy_apply = getattr(module, "_functions_to_lazy_apply", None)
     if _functions_to_lazy_apply is not None:
-        # pyre-fixme[29]:
-        #  `Union[BoundMethod[typing.Callable(torch.Tensor.__iter__)[[Named(self,
-        #  torch.Tensor)], typing.Iterator[typing.Any]], torch.Tensor], torch.Tensor,
-        #  torch.nn.modules.module.Module]` is not a function.
         for fn in _functions_to_lazy_apply:
             module.apply(fn)
         delattr(module, "_functions_to_lazy_apply")
-    # pyre-ignore[16]
     module._lazy_apply_hook.remove()
     delattr(module, "_lazy_apply_hook")
 
 
 def lazy_apply(
     module: torch.nn.Module, fn: Callable[[torch.nn.Module], None]
 ) -> torch.nn.Module:
@@ -79,22 +74,19 @@
         seq = torch.nn.Sequential(torch.nn.LazyLinear(2), torch.nn.LazyLinear(2))
         lazy_apply(seq, init_weights)  # doesn't run `init_weights` immediately
         input = torch.randn(2, 10)
         seq(input)  # runs `init_weights` only once, right after first forward pass
     """
 
     if not hasattr(module, "_functions_to_lazy_apply"):
-        # pyre-ignore[16]
         module._functions_to_lazy_apply = []
     if not hasattr(module, "_lazy_apply_hook"):
-        # pyre-ignore[16]
         module._lazy_apply_hook = module.register_forward_hook(
             _apply_functions_after_first_forward
         )
-    # pyre-ignore[16]
     module._functions_to_lazy_apply.append(fn)
     return module
 
 
 class _LazyExtensionProtocol(_LazyProtocol):
     # pyre-ignore[2,3]
     def _call_impl(self, *input, **kwargs):
```

## torchrec/modules/utils.py

```diff
@@ -106,12 +106,9 @@
         == sizes[0]
     ), f"the counts of modules ({len(modules)}) do not match with the required counts {sizes}"
     if len(sizes) == 1:
         return torch.nn.ModuleList(modules)
     else:
         # recursively create nested list
         return torch.nn.ModuleList(
-            # pyre-fixme[6]: Expected `Iterable[torch.nn.Module]` for 1st param but
-            #  got `Module`.
-            convert_list_of_modules_to_modulelist(m, sizes[1:])
-            for m in modules
+            convert_list_of_modules_to_modulelist(m, sizes[1:]) for m in modules
         )
```

## torchrec/quant/embedding_modules.py

```diff
@@ -53,14 +53,18 @@
 
 MODULE_ATTR_REGISTER_TBES_BOOL: str = "__register_tbes_in_named_modules"
 
 MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS: str = (
     "__quant_state_dict_split_scale_bias"
 )
 
+MODULE_ATTR_ROW_ALIGNMENT_INT: str = "__register_row_alignment_in_named_modules"
+
+DEFAULT_ROW_ALIGNMENT = 16
+
 
 def for_each_module_of_type_do(
     module: nn.Module,
     module_types: List[Type[torch.nn.Module]],
     op: Callable[[torch.nn.Module], None],
 ) -> None:
     for m in module.modules():
@@ -71,33 +75,41 @@
 def quant_prep_enable_quant_state_dict_split_scale_bias(module: nn.Module) -> None:
     setattr(module, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, True)
 
 
 def quant_prep_enable_quant_state_dict_split_scale_bias_for_types(
     module: nn.Module, module_types: List[Type[torch.nn.Module]]
 ) -> None:
-
     for_each_module_of_type_do(
         module,
         module_types,
         lambda m: setattr(m, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, True),
     )
 
 
 def quant_prep_enable_register_tbes(
     module: nn.Module, module_types: List[Type[torch.nn.Module]]
 ) -> None:
-
     for_each_module_of_type_do(
         module,
         module_types,
         lambda m: setattr(m, MODULE_ATTR_REGISTER_TBES_BOOL, True),
     )
 
 
+def quant_prep_customize_row_alignment(
+    module: nn.Module, module_types: List[Type[torch.nn.Module]], row_alignment: int
+) -> None:
+    for_each_module_of_type_do(
+        module,
+        module_types,
+        lambda m: setattr(m, MODULE_ATTR_ROW_ALIGNMENT_INT, row_alignment),
+    )
+
+
 def quantize_state_dict(
     module: nn.Module,
     table_name_to_quantized_weights: Dict[str, Tuple[Tensor, Tensor]],
     data_type: DataType,
 ) -> torch.device:
     device = torch.device("cpu")
     for key, tensor in module.state_dict().items():
@@ -224,14 +236,15 @@
         device: torch.device,
         output_dtype: torch.dtype = torch.float,
         table_name_to_quantized_weights: Optional[
             Dict[str, Tuple[Tensor, Tensor]]
         ] = None,
         register_tbes: bool = False,
         quant_state_dict_split_scale_bias: bool = False,
+        row_alignment: int = DEFAULT_ROW_ALIGNMENT,
     ) -> None:
         super().__init__()
         self._is_weighted = is_weighted
         self._embedding_bag_configs: List[EmbeddingBagConfig] = tables
         self._key_to_tables: Dict[
             Tuple[PoolingType, DataType], List[EmbeddingBagConfig]
         ] = defaultdict(list)
@@ -240,14 +253,15 @@
         # Their states will be modified via self.embedding_bags
         self._emb_modules: List[nn.Module] = []
         self._output_dtype = output_dtype
         self._device: torch.device = device
         self._table_name_to_quantized_weights: Optional[
             Dict[str, Tuple[Tensor, Tensor]]
         ] = None
+        self.row_alignment = row_alignment
 
         table_names = set()
         for table in self._embedding_bag_configs:
             if table.name in table_names:
                 raise ValueError(f"Duplicate table name {table.name}")
             table_names.add(table.name)
             self._length_per_key.extend(
@@ -288,15 +302,15 @@
 
             emb_module = IntNBitTableBatchedEmbeddingBagsCodegen(
                 embedding_specs=embedding_specs,
                 pooling_mode=pooling_type_to_pooling_mode(pooling),
                 weight_lists=weight_lists,
                 device=device,
                 output_dtype=data_type_to_sparse_type(dtype_to_data_type(output_dtype)),
-                row_alignment=16,
+                row_alignment=row_alignment,
                 feature_table_map=feature_table_map,
             )
             if device != torch.device("meta") and weight_lists is None:
                 emb_module.initialize_weights()
             self._emb_modules.append(emb_module)
 
         self._embedding_names: List[str] = list(
@@ -307,15 +321,15 @@
         # nn.Module API calls (state_dict, named_modules, etc)
         self.embedding_bags: nn.ModuleDict = nn.ModuleDict()
         for (_key, tables), emb_module in zip(
             self._key_to_tables.items(), self._emb_modules
         ):
             for embedding_config, (weight, qscale, qbias) in zip(
                 tables,
-                emb_module.split_embedding_weights_with_scale_bias(  # pyre-ignore[29]
+                emb_module.split_embedding_weights_with_scale_bias(
                     split_scale_bias_mode=2 if quant_state_dict_split_scale_bias else 0
                 ),
             ):
                 self.embedding_bags[embedding_config.name] = torch.nn.Module()
                 # register as a buffer so it's exposed in state_dict.
                 # TODO: register as param instead of buffer
                 # however, since this is only needed for inference, we do not need to expose it as part of parameters.
@@ -332,14 +346,15 @@
                     )
 
         setattr(
             self,
             MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS,
             quant_state_dict_split_scale_bias,
         )
+        setattr(self, MODULE_ATTR_REGISTER_TBES_BOOL, register_tbes)
         self.register_tbes = register_tbes
         if register_tbes:
             self.tbes: torch.nn.ModuleList = torch.nn.ModuleList(self._emb_modules)
 
     def forward(
         self,
         features: KeyedJaggedTensor,
@@ -411,33 +426,34 @@
     def from_float(
         cls, module: OriginalEmbeddingBagCollection
     ) -> "EmbeddingBagCollection":
         assert hasattr(
             module, "qconfig"
         ), "EmbeddingBagCollection input float module must have qconfig defined"
 
-        # pyre-ignore [16]
         data_type = dtype_to_data_type(module.qconfig.weight().dtype)
         embedding_bag_configs = copy.deepcopy(module.embedding_bag_configs())
         for config in embedding_bag_configs:
             config.data_type = data_type
 
         table_name_to_quantized_weights: Dict[str, Tuple[Tensor, Tensor]] = {}
         device = quantize_state_dict(module, table_name_to_quantized_weights, data_type)
         return cls(
             embedding_bag_configs,
             module.is_weighted(),
             device=device,
-            # pyre-ignore [16]
             output_dtype=module.qconfig.activation().dtype,
             table_name_to_quantized_weights=table_name_to_quantized_weights,
             register_tbes=getattr(module, MODULE_ATTR_REGISTER_TBES_BOOL, False),
             quant_state_dict_split_scale_bias=getattr(
                 module, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, False
             ),
+            row_alignment=getattr(
+                module, MODULE_ATTR_ROW_ALIGNMENT_INT, DEFAULT_ROW_ALIGNMENT
+            ),
         )
 
     def embedding_bag_configs(
         self,
     ) -> List[EmbeddingBagConfig]:
         return self._embedding_bag_configs
 
@@ -514,24 +530,26 @@
         need_indices: bool = False,
         output_dtype: torch.dtype = torch.float,
         table_name_to_quantized_weights: Optional[
             Dict[str, Tuple[Tensor, Tensor]]
         ] = None,
         register_tbes: bool = False,
         quant_state_dict_split_scale_bias: bool = False,
+        row_alignment: int = DEFAULT_ROW_ALIGNMENT,
     ) -> None:
         super().__init__()
         self._emb_modules: List[IntNBitTableBatchedEmbeddingBagsCodegen] = []
         self.embeddings: nn.ModuleDict = nn.ModuleDict()
 
         self._embedding_configs = tables
         self._embedding_dim: int = -1
         self._need_indices: bool = need_indices
         self._output_dtype = output_dtype
         self._device = device
+        self.row_alignment = row_alignment
 
         table_names = set()
         for config in tables:
             if config.name in table_names:
                 raise ValueError(f"Duplicate table name {config.name}")
             table_names.add(config.name)
             self._embedding_dim = (
@@ -547,28 +565,28 @@
             if table_name_to_quantized_weights:
                 none_throws(weight_lists).append(
                     table_name_to_quantized_weights[config.name]
                 )
             emb_module = IntNBitTableBatchedEmbeddingBagsCodegen(
                 embedding_specs=[
                     (
-                        "",
+                        config.name,
                         config.num_embeddings,
                         config.embedding_dim,
                         data_type_to_sparse_type(config.data_type),
                         EmbeddingLocation.HOST
                         if device.type == "cpu"
                         else EmbeddingLocation.DEVICE,
                     )
                 ],
                 pooling_mode=PoolingMode.NONE,
                 weight_lists=weight_lists,
                 device=device,
                 output_dtype=data_type_to_sparse_type(dtype_to_data_type(output_dtype)),
-                row_alignment=16,
+                row_alignment=row_alignment,
             )
             if device != torch.device("meta") and weight_lists is None:
                 emb_module.initialize_weights()
 
             self._emb_modules.append(emb_module)
             self.embeddings[config.name] = torch.nn.Module()
             # register as a buffer so it's exposed in state_dict.
@@ -594,14 +612,15 @@
             tables
         )
         setattr(
             self,
             MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS,
             quant_state_dict_split_scale_bias,
         )
+        setattr(self, MODULE_ATTR_REGISTER_TBES_BOOL, register_tbes)
         self.register_tbes = register_tbes
         if register_tbes:
             self.tbes: torch.nn.ModuleList = torch.nn.ModuleList(self._emb_modules)
 
     def forward(
         self,
         features: KeyedJaggedTensor,
@@ -642,33 +661,34 @@
 
     @classmethod
     def from_float(cls, module: OriginalEmbeddingCollection) -> "EmbeddingCollection":
         assert hasattr(
             module, "qconfig"
         ), "EmbeddingCollection input float module must have qconfig defined"
 
-        # pyre-ignore [16]
         data_type = dtype_to_data_type(module.qconfig.weight().dtype)
         tables = copy.deepcopy(module.embedding_configs())
         for config in tables:
             config.data_type = data_type
 
         table_name_to_quantized_weights: Dict[str, Tuple[Tensor, Tensor]] = {}
         device = quantize_state_dict(module, table_name_to_quantized_weights, data_type)
-
         return cls(
             tables,
             device=device,
             need_indices=module.need_indices(),
-            # pyre-ignore
             output_dtype=module.qconfig.activation().dtype,
             table_name_to_quantized_weights=table_name_to_quantized_weights,
+            register_tbes=getattr(module, MODULE_ATTR_REGISTER_TBES_BOOL, False),
             quant_state_dict_split_scale_bias=getattr(
                 module, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, False
             ),
+            row_alignment=getattr(
+                module, MODULE_ATTR_ROW_ALIGNMENT_INT, DEFAULT_ROW_ALIGNMENT
+            ),
         )
 
     def _get_name(self) -> str:
         return "QuantizedEmbeddingCollection"
 
     def need_indices(self) -> bool:
         return self._need_indices
```

## torchrec/quant/utils.py

```diff
@@ -29,25 +29,22 @@
         for emb_configs, emb_module in zip(
             quant_ebc._key_to_tables, quant_ebc._emb_modules
         ):
             table_names = []
             for config in emb_configs:
                 table_names.append(config.name)
             joined_table_names = ",".join(table_names)
-            # pyre-fixme[16]: `Module` has no attribute `_fx_path`.
             emb_module._fx_path = f"emb_module.{joined_table_names}"
     elif isinstance(quant_ebc, ShardedQuantEmbeddingBagCollection):
         for i, (emb_module, emb_dist_module) in enumerate(
             zip(quant_ebc._lookups, quant_ebc._output_dists)
         ):
             embedding_fx_path = f"embedding_lookup.sharding_{i}"
             emb_module._fx_path = embedding_fx_path
             emb_dist_module._fx_path = f"embedding_dist.{i}"
-            # pyre-fixme[6]: For 1st argument expected `Iterable[Variable[_T]]` but
-            #  got `Union[Module, Tensor]`.
             for rank, rank_module in enumerate(emb_module._embedding_lookups_per_rank):
                 rank_fx_path = f"{embedding_fx_path}.rank_{rank}"
                 rank_module._fx_path = rank_fx_path
                 for group, group_module in enumerate(rank_module._emb_modules):
                     group_module._fx_path = f"{rank_fx_path}.group_{group}"
                     group_module._emb_module._fx_path = (
                         f"{rank_fx_path}.group_{group}.tbe"
@@ -84,24 +81,28 @@
         and module.device.type == "meta"
     ):
         qebc_cpu = QuantEmbeddingBagCollection(
             tables=module.embedding_bag_configs(),
             is_weighted=module.is_weighted(),
             device=torch.device("cpu"),
             output_dtype=module.output_dtype(),
+            register_tbes=module.register_tbes,
+            row_alignment=module.row_alignment,
         )
         setattr(root_module, name, qebc_cpu)
     elif (
         name is not None
         and isinstance(module, QuantEmbeddingCollection)
         and module.device.type == "meta"
     ):
         qec_cpu = QuantEmbeddingCollection(
             tables=module.embedding_configs(),
             device=torch.device("cpu"),
             need_indices=module.need_indices(),
             output_dtype=module.output_dtype(),
+            register_tbes=module.register_tbes,
+            row_alignment=module.row_alignment,
         )
         setattr(root_module, name, qec_cpu)
     else:
         for name, submodule in module.named_children():
             _meta_to_cpu_placement(submodule, module, name)
```

## torchrec/sparse/jagged_tensor.py

```diff
@@ -207,20 +207,30 @@
             _assert_tensor_has_no_elements_or_has_integers(offsets, "offsets")
         if lengths is not None:
             _assert_tensor_has_no_elements_or_has_integers(lengths, "lengths")
         self._lengths: Optional[torch.Tensor] = lengths
         self._offsets: Optional[torch.Tensor] = offsets
 
     @staticmethod
-    def empty(is_weighted: bool = False) -> "JaggedTensor":
-        weights = torch.tensor([]) if is_weighted else None
+    def empty(
+        is_weighted: bool = False,
+        device: Optional[torch.device] = None,
+        values_dtype: Optional[torch.dtype] = None,
+        weights_dtype: Optional[torch.dtype] = None,
+        lengths_dtype: torch.dtype = torch.int32,
+    ) -> "JaggedTensor":
+        weights = (
+            torch.tensor([], dtype=weights_dtype, device=device)
+            if is_weighted
+            else None
+        )
         return JaggedTensor(
-            values=torch.tensor([]),
-            offsets=torch.tensor([]),
-            lengths=torch.tensor([]),
+            values=torch.tensor([], dtype=values_dtype, device=device),
+            offsets=torch.tensor([], dtype=lengths_dtype, device=device),
+            lengths=torch.tensor([], dtype=lengths_dtype, device=device),
             weights=weights,
         )
 
     @staticmethod
     def from_dense_lengths(
         values: torch.Tensor,
         lengths: torch.Tensor,
@@ -933,25 +943,29 @@
             lengths=torch.cat(length_list, dim=0),
             stride=stride,
             length_per_key=length_per_key if has_length_per_key else None,
         )
 
     @staticmethod
     def empty(
-        is_weighted: bool = False, device: Optional[torch.device] = None
+        is_weighted: bool = False,
+        device: Optional[torch.device] = None,
+        values_dtype: Optional[torch.dtype] = None,
+        weights_dtype: Optional[torch.dtype] = None,
+        lengths_dtype: torch.dtype = torch.int32,
     ) -> "KeyedJaggedTensor":
         weights = None
         if is_weighted is True:
-            weights = torch.tensor([], device=device) if device else torch.tensor([])
+            weights = torch.tensor([], dtype=weights_dtype, device=device)
 
         return KeyedJaggedTensor(
             keys=[],
-            values=torch.tensor([], device=device) if device else torch.tensor([]),
+            values=torch.tensor([], dtype=values_dtype, device=device),
             weights=weights,
-            lengths=torch.tensor([], device=device) if device else torch.tensor([]),
+            lengths=torch.tensor([], dtype=lengths_dtype, device=device),
             stride=0,
         )
 
     @staticmethod
     def empty_like(kjt: "KeyedJaggedTensor") -> "KeyedJaggedTensor":
         return KeyedJaggedTensor(
             keys=[],
@@ -1134,29 +1148,36 @@
                         length_per_key=self._length_per_key,
                         offset_per_key=self._offset_per_key,
                         index_per_key=self._index_per_key,
                         jt_dict=self._jt_dict,
                     )
                 )
             elif segment == 0:
+                empty_int_list: List[int] = torch.jit.annotate(List[int], [])
                 split_list.append(
                     KeyedJaggedTensor(
                         keys=keys,
                         values=torch.tensor(
-                            [], device=self.device(), dtype=self._values.dtype
+                            empty_int_list,
+                            device=self.device(),
+                            dtype=self._values.dtype,
                         ),
                         weights=None
                         if self.weights_or_none() is None
                         else torch.tensor(
-                            [],
+                            empty_int_list,
                             device=self.device(),
                             dtype=self.weights().dtype,
                         ),
-                        lengths=torch.tensor([], device=self.device(), dtype=torch.int),
-                        offsets=torch.tensor([], device=self.device(), dtype=torch.int),
+                        lengths=torch.tensor(
+                            empty_int_list, device=self.device(), dtype=torch.int
+                        ),
+                        offsets=torch.tensor(
+                            empty_int_list, device=self.device(), dtype=torch.int
+                        ),
                         stride=self._stride,
                         length_per_key=None,
                         offset_per_key=None,
                         index_per_key=None,
                         jt_dict=None,
                     )
                 )
@@ -1198,25 +1219,35 @@
         permuted_length_per_key: List[int] = []
         permuted_lengths_sum = 0
         for index in indices:
             key = self._keys[index]
             permuted_keys.append(key)
             permuted_lengths_sum += length_per_key[index]
             permuted_length_per_key.append(length_per_key[index])
-        (
-            permuted_lengths,
-            permuted_values,
-            permuted_weights,
-        ) = torch.ops.fbgemm.permute_2D_sparse_data(
-            indices_tensor,
-            self.lengths().view(len(self._keys), -1),
-            self.values(),
-            self.weights_or_none(),
-            permuted_lengths_sum,
-        )
+
+            
+            try:
+                (
+                    permuted_lengths,
+                    permuted_values,
+                    permuted_weights,
+                ) = torch.ops.fbgemm.permute_2D_sparse_data(
+                    indices_tensor,
+                    self.lengths().view(len(self._keys), -1),
+                    self.values(),
+                    self.weights_or_none(),
+                    permuted_lengths_sum,
+                )
+            except Exception as e:
+                if torch.cuda.current_device() == 0:
+                    print("indices_tensor", indices_tensor)
+                    print("self.lengths().view(len(self._keys), -1)", self.lengths().view(len(self._keys), -1))
+                    print("self.values()", self.values())
+                    print("permuted_lengths_sum", permuted_lengths_sum)
+                raise e
 
         kjt = KeyedJaggedTensor(
             keys=permuted_keys,
             values=permuted_values,
             weights=permuted_weights,
             lengths=permuted_lengths.view(-1),
             offsets=None,
```

## Comparing `torchrec_nightly-2023.6.9.dist-info/LICENSE` & `torchrec_nightly-2023.7.12.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torchrec_nightly-2023.6.9.dist-info/METADATA` & `torchrec_nightly-2023.7.12.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchrec-nightly
-Version: 2023.6.9
+Version: 2023.7.12
 Summary: Pytorch domain library for recommendation systems
 Home-page: https://github.com/pytorch/torchrec
 Author: TorchRec Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: pytorch,recommendation systems,sharding
 Classifier: Development Status :: 4 - Beta
```

## Comparing `torchrec_nightly-2023.6.9.dist-info/RECORD` & `torchrec_nightly-2023.7.12.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -8,136 +8,188 @@
 torchrec/datasets/utils.py,sha256=eQDJJCkEl60pmgc7z1yjKcl-OrNQImflhhmohI-CuL0,10909
 torchrec/datasets/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/datasets/scripts/contiguous_preproc_criteo.py,sha256=8jjtDiQScJH6R4FfKLgJ3fm-FzfnJxyfbV52zj3SM_8,2448
 torchrec/datasets/scripts/npy_preproc_criteo.py,sha256=QOyHZpPGL6HtPrVijk7qTALvnDqgecWPEZxKB_eVA94,2847
 torchrec/datasets/scripts/shuffle_preproc_criteo.py,sha256=PC1t5EkJkG6qu3ioewAVZM-Bnzo01HKMUH92IprFth0,3077
 torchrec/datasets/test_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/datasets/test_utils/criteo_test_utils.py,sha256=Ob2fJniGOsfbWNF_Gy2RJhrGAVnLAFPSlUTJOp2kay4,5308
+torchrec/datasets/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+torchrec/datasets/tests/test_criteo.py,sha256=Fg7V9iS_0hL8zRlYDVtvs-ej7Hc0b22l8qw9Zhk_BOw,22047
+torchrec/datasets/tests/test_movielens.py,sha256=ekGuqVDBScljcn5OTLMuN7boIxdH4N4yLS-vX7uBZlw,4659
+torchrec/datasets/tests/test_random.py,sha256=EzligSIrNlaulC3bDYjRXhSIzeCujzHKUIyAGzsRRnI,3925
+torchrec/datasets/tests/test_utils.py,sha256=Rkyq7SlqTLtS3HUuZaVM_czQdSe74mHuFLQk751hwxc,5684
 torchrec/distributed/__init__.py,sha256=VCy8GKOM-1dejxUWNSA3gozG3HQ4x5-Y9c9-WFbAMGg,1912
-torchrec/distributed/batched_embedding_kernel.py,sha256=wNLqxMtbcBasLfm7OBA77QfPfswrFkzy96wYaIfz7ZQ,37411
+torchrec/distributed/batched_embedding_kernel.py,sha256=uBFpJTxGTKKaye-kCA4Ou-sh6rpg_6K0JAfiZhqAyvw,37307
 torchrec/distributed/collective_utils.py,sha256=r7Aawq-KSVC-HjjEd6U8k0vNnRMx_-8_sAhYdElGaJw,2069
 torchrec/distributed/comm.py,sha256=21Std9n_HJCF3Nsw9O4yQQOJuL2DUVzZzoRhH3M6my8,4988
 torchrec/distributed/comm_ops.py,sha256=C63THNJOnJWkfRYGuNw5opFyKsdlpZs9_23u-DHSrAQ,55918
-torchrec/distributed/dist_data.py,sha256=pWuAzn98i5O4lNHmv2wMGa4gksYEh_DOJT4rzRp_nYg,35580
-torchrec/distributed/embedding.py,sha256=xbzsxuqclElhNIN7lQxF-i06Cx4jBw4R8M6j-fUz4tg,32013
+torchrec/distributed/dist_data.py,sha256=zU88BP5WYHsqDoVUZmfCJbXuzHj5lThvZ0NN7dfj6iQ,36506
+torchrec/distributed/embedding.py,sha256=ctrHHtWFq5ITPOucAbO2UQ2cRdeDPKRFyHd04lhYmPo,32295
 torchrec/distributed/embedding_kernel.py,sha256=9OA5PDofQZ-ZRORNR4Ca1pJoEZk5Oj2gE6axYwcXIds,4947
-torchrec/distributed/embedding_lookup.py,sha256=Cyl1osqBbk1wpQlcHjSYp-9nsOJ-l_9A55x9VuAMg4U,29176
-torchrec/distributed/embedding_sharding.py,sha256=jhbxU4mCMCCLE3NnV3bLHvzJKRgTiL-rPJPbqutl3WQ,20599
-torchrec/distributed/embedding_tower_sharding.py,sha256=ypr4JbTZUh_35dYUoKWoOSJNEVG3c6gV9g5gt-fs6lQ,37089
+torchrec/distributed/embedding_lookup.py,sha256=-rExTGufuH2qcRzeR2FSSdB9TfqsnVXdz-lghXceVZs,29185
+torchrec/distributed/embedding_sharding.py,sha256=Uvybimnwvf991uX840txCxO0xfKThKXwW-bqh9__3EY,20950
+torchrec/distributed/embedding_tower_sharding.py,sha256=eDHPHzjCstJJRJlE-n8a9lC54lCDsi1iAt4SmkLfza0,36853
 torchrec/distributed/embedding_types.py,sha256=QbDVqeT2wb1RpnGZxrFtFdHYDsOHKW7SH8fLWmN_d0E,15030
-torchrec/distributed/embeddingbag.py,sha256=ILPW9XGRYGVPFwKGNU8DF5zk0Oj70-duRz2JUdxxlMo,35218
+torchrec/distributed/embeddingbag.py,sha256=ddy1uo1Sg2TWISw03bvlp_kaHHvpqkztUm-8pegEq2c,37214
 torchrec/distributed/fbgemm_qcomm_codec.py,sha256=StYltKC6Eq6SE_YiX6GsVW3ZF0VyqTcGHXuCYmPAFlU,7373
 torchrec/distributed/fp_embeddingbag.py,sha256=sC7ZIECzJtwn5LNRrUzf0OH7phI3kQHqQ6wBPaGGvPQ,6137
 torchrec/distributed/fused_embedding.py,sha256=1VJeW5Dl7EFMvyOfhBvDKZlp39GYucBo8vNFJY2alFI,5243
-torchrec/distributed/fused_embeddingbag.py,sha256=7DIMc5sHdsDAgqCnNomcPo6V4aIH1wlkzyshHeJB3pc,5110
+torchrec/distributed/fused_embeddingbag.py,sha256=tG_BrUlCdsek87jgHPKbxg3-z13sAgSWPNRBArf2_ss,5080
 torchrec/distributed/fused_params.py,sha256=YEbH5KUphcSWkwLi-JzXUR9SRDm2OykFxP46CJj6nTM,2271
 torchrec/distributed/grouped_position_weighted.py,sha256=q-QE0U306BiPkXIAlJGIQ80EUDZj-FXTbWwjz3EyvLI,3807
-torchrec/distributed/model_parallel.py,sha256=YzXWgCmmeA_ccHtqfzeDM5ZTnnFUXfYCtocx1pKHV7Q,19786
-torchrec/distributed/quant_embedding.py,sha256=cyawhiEPlefP3pAAJB8A0uegGnlUj41OOYIlRt8qNBc,14686
-torchrec/distributed/quant_embedding_kernel.py,sha256=3WRKuTrKi8dJvhfAsb_vYDp3aqOc2YOrKPeMhZ7MDJk,14976
-torchrec/distributed/quant_embeddingbag.py,sha256=f_yZU9nKlmdzpJNHpugfmAbyIkTYZGiY_H1NzDExRno,11770
+torchrec/distributed/model_parallel.py,sha256=VV9Vsyas0VKNHr8sX9pq1iT_xJ2b9xjenY3pYAY5HYw,19750
+torchrec/distributed/quant_embedding.py,sha256=9hTS4oUYkoCEHInYO7r0IQjfAJi4fsw5WNiTOHGUJuM,20748
+torchrec/distributed/quant_embedding_kernel.py,sha256=VsROr4bXBkYysS0H7NnlZzF7IvGgZFtgws5jsnPf6g4,15112
+torchrec/distributed/quant_embeddingbag.py,sha256=SJPY-nL95LKozfT8iR4SHt1BNLx4OcoAfFvqKzy1Gf4,12621
+torchrec/distributed/quant_state.py,sha256=PDQ7qUwhFt-q1WvTkoSbWE3rotiFOYyKNFsQ5vJQ36U,13928
 torchrec/distributed/shard.py,sha256=4Dr5ixWCoMEFEuL5WN4fL2gIdl9wmSUjZWsiF-kdCdQ,9261
-torchrec/distributed/sharding_plan.py,sha256=vVQhmXy2w4FmXyuJa1t6PyfaqEEVSxoLZ5ChWlc7TbU,19411
-torchrec/distributed/train_pipeline.py,sha256=pQ_bIP5dI70_ypkE2OWcv_pVwKa1nNjdT6oBZaTunpI,36724
-torchrec/distributed/types.py,sha256=tNd_B5PXjaOqPmUXxSZLXB3a71sjU8LBtSY9kuGxe7I,24927
-torchrec/distributed/utils.py,sha256=PbVfo9_QBugfSOvwmySdjXlhWOAYSl9eGpYYH0d0SqI,11873
+torchrec/distributed/sharding_plan.py,sha256=DftThfyzPvfFzg7SvqsNo7X5n-1rxWhp1RlcQCcpq2o,19646
+torchrec/distributed/train_pipeline.py,sha256=JTFXhso9xuGusvWcSYYTPptcnmn8TEPk0Xkq83AlF8k,39755
+torchrec/distributed/types.py,sha256=aqJ4ipEsMTy9WoTWCRfXg0KhHNcXYC-QRdBp0Db2rHY,27865
+torchrec/distributed/utils.py,sha256=dwNuXu5_OOK0YsGZhGPIdtZu4GzvT6X1MPsARINy10U,15470
 torchrec/distributed/composable/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/distributed/composable/table_batched_embedding_slice.py,sha256=x439M8TTXQtzoihan1OKKbmGYkqJlAxxTHCDz5295RY,3207
 torchrec/distributed/planner/__init__.py,sha256=UWnxb-SuE211uJGdwtSkKRVADT3plQozB2l6fvs6Ve0,1025
 torchrec/distributed/planner/constants.py,sha256=MkeVqYO2QGg57i6fs29lZb2dScaaR9mdQVsee4NxyFc,3135
-torchrec/distributed/planner/enumerators.py,sha256=hZzhnfMrOz65lBoddxTKBb01hm43R_5tdpysJFSzCLE,10318
+torchrec/distributed/planner/enumerators.py,sha256=JoQ1WcrU12Fyy57aBHitcKIpBTASJVnyLhkOxN7V4J4,11430
+torchrec/distributed/planner/parallelized_planners.py,sha256=MDRP5L61bX2pmGwk62iD4zcoMt4wjwzfd2nmtqvfDG4,11739
 torchrec/distributed/planner/partitioners.py,sha256=k-rzm6oMZ_sLpGHT8yAu2tIMkMumhJMvAFeY0cdNirk,12642
 torchrec/distributed/planner/perf_models.py,sha256=vYIjVr0NG6sZItfxVuRWF7AS8lGGtbRn66O0flNJpoU,835
-torchrec/distributed/planner/planners.py,sha256=LjMOoQTu_IlwlG-wl03H39c886oxBgfEQMKsouYI1pM,13288
+torchrec/distributed/planner/planners.py,sha256=4b_TkQQ8yZOxb4VTDAAcRlpt6E61crkiDuYjuTfnMx0,13530
 torchrec/distributed/planner/proposers.py,sha256=tfhI0DavpRYfY4UN5diXBMl8fWHIEm8wNco5R6yBIGI,11236
-torchrec/distributed/planner/shard_estimators.py,sha256=JTdL0OI0kpFbkxdCZN9qK46PN6v2kv2mIMdXLIZMsOE,40395
-torchrec/distributed/planner/stats.py,sha256=oIhRnFQybUdx-2NEH3ZBhyx0nqtiR4VkQKnS7YLW6CY,23617
-torchrec/distributed/planner/storage_reservations.py,sha256=rPqeD03f3mg8yoSqy9CZfOmxVMUGrCz98nPqwvxhApc,9125
-torchrec/distributed/planner/types.py,sha256=JG39UMXzWQ7_G38aG2qo3h601s2UsII_OPyHJ068kOM,13899
+torchrec/distributed/planner/shard_estimators.py,sha256=QTW2OdGRaBnOp79xRiUz5W3O9oxS9m4wlAqP-goHCi4,41291
+torchrec/distributed/planner/stats.py,sha256=sptST5uG_JL136gUzngAu_pbJELfIJKMlTHMEk_I3es,23791
+torchrec/distributed/planner/storage_reservations.py,sha256=QcIYMAgoAABXJ8loO8wsEPlSYJJDBl5cRXMhk-wJwZQ,9643
+torchrec/distributed/planner/types.py,sha256=FHe0shRgJJ8Kvqnb9IpNV7Aphqsga2wcZ6dXTmI_M7s,14582
 torchrec/distributed/planner/utils.py,sha256=YwOUrqb-D6HaVtWCRFz9RWhBdMRBqjMaYYhoQgyOkQg,1119
 torchrec/distributed/sharding/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-torchrec/distributed/sharding/cw_sequence_sharding.py,sha256=o8RZAs2zivNP8MZ5QUWF0alw7KwWZnJVG9iKHM4EJdE,2539
-torchrec/distributed/sharding/cw_sharding.py,sha256=PLJHgxkQvX_sNI8RJlz4xIemb4vO2KHOe_9PylZ2je8,9519
+torchrec/distributed/sharding/cw_sequence_sharding.py,sha256=N5qRxCxDkhT0ZcOAUBDTuhQTAz3_I7B1cN_pFeleBbk,2479
+torchrec/distributed/sharding/cw_sharding.py,sha256=K6Nc8JaQxENSaOPv4rMZytW6FE7wGlKxXj78RZOx6QE,12945
 torchrec/distributed/sharding/dp_sequence_sharding.py,sha256=zQmERguEGVd5IAbmVsIhqdKXb0f2g8tQamN838qVvfM,2802
 torchrec/distributed/sharding/dp_sharding.py,sha256=HSedwv3zCoi-WGElzucyqDMolrviB6tyqs1jN-6RTEY,7681
-torchrec/distributed/sharding/rw_sequence_sharding.py,sha256=66tW1TyIp8kSdT3t8EsVsHcv7_kAzbCX3xT_pDmc_NE,5041
-torchrec/distributed/sharding/rw_sharding.py,sha256=k3ym1GGjdQeRnLeUheZm5o9D8co_U4dUQgHrF771XUQ,12850
-torchrec/distributed/sharding/sequence_sharding.py,sha256=LBUW1PvAV9WNwf-m-x9bYIcU96PL75mPE_uQK9dLAOU,3114
-torchrec/distributed/sharding/tw_sequence_sharding.py,sha256=SR_G_rniSZx_DBnrWW14HEMoeqwRnMPN3LdQlnptLL8,7692
-torchrec/distributed/sharding/tw_sharding.py,sha256=JtI2GW9YR-eg1VuQDwDa6qaR6sOgBAzGx3Y3XkEOBZM,16315
+torchrec/distributed/sharding/rw_sequence_sharding.py,sha256=xhgtuuzXgj29k2CRFMHaYDXhvdf2v5C7uoyCSP0yH-A,7640
+torchrec/distributed/sharding/rw_sharding.py,sha256=a7tTyVTMA_8NzlZhWCoJbrfv8nqowUnTMkpFO-BmI_Q,17911
+torchrec/distributed/sharding/sequence_sharding.py,sha256=Df7Rodg34MDUSbQBYGHLnUCoNT-6fKhnbrE-FQPRy9E,3627
+torchrec/distributed/sharding/tw_sequence_sharding.py,sha256=vEjhuY38hhtkYGHtzvIOvK3wLN1B9IGNpVjrlnAVhi8,7632
+torchrec/distributed/sharding/tw_sharding.py,sha256=DFgTgMeG8FrzAqGAczb4VQSJ1R99ybm_ScOG6444O2w,16097
 torchrec/distributed/sharding/twcw_sharding.py,sha256=LyOowcADWmRdkRn-eEW6QB0b0xYi0vM-Ubrr6N2zwwA,1284
-torchrec/distributed/sharding/twrw_sharding.py,sha256=k69AX5oKj3ep38tM_RI_NkwyZ4z_U8kVQpLtDjRYPKI,19898
+torchrec/distributed/sharding/twrw_sharding.py,sha256=V2Jjkzx2YyY6Aph21GBrW_1u_85BX874Vf9rOD3KTDg,19871
 torchrec/distributed/test_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-torchrec/distributed/test_utils/infer_utils.py,sha256=r2HdvqgADtAbP5-S5FCANaO734GF68hdCtB1vJ7Lgfs,10453
+torchrec/distributed/test_utils/infer_utils.py,sha256=AYqO1zXl7P3U5DiW6PeTN8wmDoJKSAWqqNfMGu3eFIE,11237
 torchrec/distributed/test_utils/multi_process.py,sha256=6AxYe2cO44EGdw-Lt5YNwqmWZW8Ldu7bVGTluIIOFbA,4868
-torchrec/distributed/test_utils/test_model.py,sha256=ACqCdD3bcxX74JihIg7jTcLvBsV8U-Bvwvy9-Pbj7nI,34246
-torchrec/distributed/test_utils/test_model_parallel.py,sha256=oN_fl-QOaAarrZwnr7q5Lz4f9xiqxxof9Bk_4PM13hM,11193
-torchrec/distributed/test_utils/test_model_parallel_base.py,sha256=I7q2IIZLN79RdqYCrg6hr_yBysZr2VO4AlESYsCtq5g,25308
+torchrec/distributed/test_utils/test_model.py,sha256=vnV6I2SCvUtFvJsjbGF8Nmc_13PuOkH0TskGBUSEjwg,34091
+torchrec/distributed/test_utils/test_model_parallel.py,sha256=C2LDYBo6cuB44yWQEPsCh72Ffj48dVzM3RZ-2fOHvcg,11197
+torchrec/distributed/test_utils/test_model_parallel_base.py,sha256=r1v_Dfy52WvN7sSzNnuzspJlCyV5GA4kirhfcVeLgfM,25310
 torchrec/distributed/test_utils/test_sharding.py,sha256=DlB6N5-qlRp-xQfEEFElDkNffnEX6LO4vOrDCGp8VkQ,15367
+torchrec/distributed/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+torchrec/distributed/tests/collective_utils_test.py,sha256=3z0muj9GIXNDGo3t8dWorAQzP9QR5DGWd4POIMbdY4I,4747
+torchrec/distributed/tests/test_apply_optim_per_param.py,sha256=EHMjiA1u3rjh360ZeH_ITFHjAe4spnoNka4MD3qp41I,16544
+torchrec/distributed/tests/test_awaitable.py,sha256=iUblz-nd4T6CCef2KKt1Ro7f7TSVIlO1pinGQ6ZkzOY,1122
+torchrec/distributed/tests/test_comm.py,sha256=RVCms01GnRApm2jQei0SyG_lg-m2Grn1oZkS4q0Cuo0,6614
+torchrec/distributed/tests/test_dist_data.py,sha256=IureSWY158PAnSvNz6ReFO36BsNu9HbisDUhTNRI5tM,33737
+torchrec/distributed/tests/test_fbgemm_qcomm_codec.py,sha256=hd89H-v0Q-iB_t_M03CB9YhYYmoi7ihwGpxLXUk5vTM,2801
+torchrec/distributed/tests/test_fused_embedding_bag_collection.py,sha256=ck2OhQ_QfGcnaDzZnAazTCGso_P4GiQ-XfU1HrqBoss,7157
+torchrec/distributed/tests/test_fused_embedding_collection.py,sha256=yzqWUX45p3IkFAYkFcDEp92IbgCwLreu_krUjS3_A0I,7477
+torchrec/distributed/tests/test_fused_optim.py,sha256=xymZK1O8BsCpWX0iWKXAqZbUAng2IJz4cQrONMfTeYk,10230
+torchrec/distributed/tests/test_lazy_awaitable.py,sha256=xPB_fZdYGnnaqB9cMng4Z1kmzu4i1mbNywFKzNhNZkA,7993
+torchrec/distributed/tests/test_model_parallel_gloo.py,sha256=Qg_hOyKKIRUu8U2Y2PXAYdZcqiIeEPNjyWv7YtH5tpo,667
+torchrec/distributed/tests/test_model_parallel_hierarchical.py,sha256=1dTQxWD7RILk02pe-zKlQ8V5TQ-py8azmhQo-8eld1g,11105
+torchrec/distributed/tests/test_model_parallel_nccl.py,sha256=NXKka-O_cuRWTpHSW3zM-Hlw1DPvwlBP5h_f6BuPd9Y,667
+torchrec/distributed/tests/test_qcomms_embedding_modules.py,sha256=InB-MKVVyzuohVwLCfiKZSxwDashLSJKstdU6ueAhic,9363
+torchrec/distributed/tests/test_quant_model_parallel.py,sha256=4OAj47yhMJLR76eVJsxCeohXkhJjPPhE3K8rekQe7Mg,22396
+torchrec/distributed/tests/test_quant_sequence_model_parallel.py,sha256=6WfO3kkUeIVJ4uy2gBeIeo80HWt2YAjog8iKnSr5yEE,5835
+torchrec/distributed/tests/test_quantize.py,sha256=ql9SoR2d5IPFyZLCI7Oneoo0b-BsNImdN4Biut49-hw,6409
+torchrec/distributed/tests/test_sequence_model.py,sha256=d78u7rlfacqXWSXhRjif_mbS46hDk54-A2-e7yDw5W8,11072
+torchrec/distributed/tests/test_sequence_model_parallel.py,sha256=QA0vnAUps-9eOzf-D8wqXx206Tyts7InyQHhJNVNZwc,11060
+torchrec/distributed/tests/test_sequence_model_parallel_hierarchical.py,sha256=ipJ9Jzw6oCFpVus6DLTAZTK04BS7qB4rBROn4tXetv0,4396
+torchrec/distributed/tests/test_sharding_plan.py,sha256=EJDStPlnpgydRacW-ohQFJ8hO4hheT82e9kSi69jy30,22707
+torchrec/distributed/tests/test_train_pipeline.py,sha256=QQjNUSrQ4n3nuv0V7Zff5CODTNcSeZCtz-sxYEcd3DY,12988
+torchrec/distributed/tests/test_utils.py,sha256=zWNtNM64H3Oqb3pS2gAEGPKcvuC1sACi2VnK_BBCX7k,13178
 torchrec/fx/__init__.py,sha256=TxNjllMWlB_rpDy4SNSA_e-xbZbhxGGTb9AxpZGcaFk,422
-torchrec/fx/tracer.py,sha256=iXfWWgPNdFlRs89RbA18Nel0Tl9z8UprRWPfTQbLx5k,6477
-torchrec/fx/utils.py,sha256=N50AfwlUhyS9r1Sv21fSbqRxiOk4KRX0MX9sDjCaQcA,4401
+torchrec/fx/tracer.py,sha256=kieodGiTo1HH1TGTgAIG2DJGTCDOCQxQCge7Et5RR1U,6451
+torchrec/fx/utils.py,sha256=RKh_viVHMgKNi9-rA7waBIGiN2p8auQWfWkpuZz5KOA,4524
 torchrec/inference/__init__.py,sha256=vi2C_o1Bvsp6hS3_uVZTL7kShgxw5qFZp248Svee2Og,1223
 torchrec/inference/client.py,sha256=jS6ldQxBRY3Bp_LwDLUNSlPt2VYMc-Hsd4iKKoHfDVU,3614
 torchrec/inference/model_packager.py,sha256=HxOEbnqXB2K4uUB9dBBJAL49ZYJME4xTFyVzKjpsjy4,3957
 torchrec/inference/modules.py,sha256=Cx4wYzrc7xG9CmvEb_xCL5sNJ7fqpnQo6G93G-euzw8,8068
 torchrec/inference/state_dict_transform.py,sha256=eFejfFRzU3pL7CmiJtkjq2mpz6Ue_NOUuO2g8-LnLig,3797
 torchrec/metrics/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/metrics/accuracy.py,sha256=q5TVzSDBpXHN8YbiAanvwxloGmqmyxr9IBQ2gkQE-g0,4168
 torchrec/metrics/auc.py,sha256=vyUUEJc6Kp1R5kSHBH0t0lI1ZdZzCr0dad6v0aVxJIA,12549
 torchrec/metrics/calibration.py,sha256=hngIvPjcAHusdz1KBrPvwMZX6OkyS0nv18EAmMcyIl0,3703
 torchrec/metrics/ctr.py,sha256=2HY53CX9If6wYcOErvYCT73NH8UdY8oI0UIitoREsMs,3465
 torchrec/metrics/mae.py,sha256=QDPT7l4LCBtTgoxEeEm9vFzCEDtEIlfzs58PtH1oS_U,3836
 torchrec/metrics/metric_module.py,sha256=8XXa5DJ5eYrS1Pat34_FZ3E9OKUj--8i80nCqXqtJsg,17909
-torchrec/metrics/metrics_config.py,sha256=tL9etUu4FsA_Dr9kUKCf3zIixK6VbIgVi4UoBTZ1GnM,6778
-torchrec/metrics/metrics_namespace.py,sha256=fodij0OglzAGOWNEefuPw0UL1cYfQZAAedCjTErDV6M,3695
+torchrec/metrics/metrics_config.py,sha256=A29AmBe-ExE_JBmoPJT73iP4aGUCYEoIYoIkgkF_Eg0,6796
+torchrec/metrics/metrics_namespace.py,sha256=qvsnqhVLOyFZ7UKl9pisLMJGhaWSlWGYDSO1HcBc3dE,3731
 torchrec/metrics/model_utils.py,sha256=WNMsAKK9b5OVPWeuRrNDZ2HjwKuAw3gjNG3OdE99EXw,3904
 torchrec/metrics/mse.py,sha256=tkK3yBV8Uu9Z8Mw_3c1k4kYAhp1jUQkFEJxc0l2LtWU,4631
 torchrec/metrics/multiclass_recall.py,sha256=7NqjkA4IUy4Db90du3hVt8cJxoWS18PBaOourHETkEs,5605
 torchrec/metrics/ne.py,sha256=wXEb9Eh5Mn3D_uuAIaUb3CvJ1eDs06ahVxaWOjR4CtU,6811
 torchrec/metrics/rec_metric.py,sha256=j1ias-rsD1nlCx_iR1Wmvw0BLoe9DHgjHfzAwd5Uvjs,33554
 torchrec/metrics/recall_session.py,sha256=24aDBSi8V5XXSnwpqCR5bWcm2CWslBBZ9_a0LQ6VGeg,10490
 torchrec/metrics/throughput.py,sha256=A_WqccFNgu4XpBZzZxnGxAT84Xp2ld43qQM6R1zaqik,6057
 torchrec/metrics/tower_qps.py,sha256=PXTBsLGjEEbQV5q2kGQriRq8GCneNkhBKTFAgNXzc-0,11160
 torchrec/metrics/weighted_avg.py,sha256=dX-qwha2__F-p-R5u27152OwlGRS6Xfnbt1DEIBw8NQ,2867
 torchrec/metrics/test_utils/__init__.py,sha256=p_uep7Hg7_aY3rOg8CxtS-REopQ4ywQq075KFoso1Lw,16441
 torchrec/models/__init__.py,sha256=iYpG-yLxFaa3ZdN-UU9PWNIdgm9EXoEj_QzJ2OLKGJQ,913
 torchrec/models/deepfm.py,sha256=-SxFKF-kHKFEzC0XIsLigQh673-B_Lu6xFlZPkR5t2g,11410
-torchrec/models/dlrm.py,sha256=37v6MOb8P06DtXfDDqokvSKSDyhDVGFEPsRoBSRtCTY,30000
+torchrec/models/dlrm.py,sha256=4wsQSNvdxZOsr2wnF25WW9g5m2g-Ewy-sJrGi8aDvAg,29965
 torchrec/models/experimental/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/models/experimental/test_transformerdlrm.py,sha256=pxdu5k-EdTdYX5RblAe1A97GuiHAUmm6oJwfG_qX8Vw,9825
 torchrec/models/experimental/transformerdlrm.py,sha256=-mWI0-_Au5wIIzGuXBri59RWHs4u5SiEal4rzm5DOeE,7434
+torchrec/models/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+torchrec/models/tests/test_deepfm.py,sha256=hREXsmtv1ieYQKHh20e538yHJcF1rfijYcKgKwB06-g,5892
+torchrec/models/tests/test_dlrm.py,sha256=dh84OAO2IzZKidkvIJaNJN7r1vIM0V11XPRtW4XEztE,34899
 torchrec/modules/__init__.py,sha256=Eho7Nd68vOa0p-WuM7-cRSc_vhA38JU88PTcdfuWEvA,1179
 torchrec/modules/activation.py,sha256=o3rGyy40bmmsplyxQy3dDMe8kITRERLJQF7oa5VTKfE,1456
-torchrec/modules/crossnet.py,sha256=hiE375Y0atKsyWYK3GLPtx5VzqkaoNl79r9HsxtMBVA,15163
+torchrec/modules/crossnet.py,sha256=nkl21C9_MZf7R4IOTbFGK6EIfQlOBNp2LXV2kQ5ZXsE,14636
 torchrec/modules/deepfm.py,sha256=05ZM2sB1YMVliZwrLHvtMYf3eWGguLFopaZwGZK16bs,8415
-torchrec/modules/embedding_configs.py,sha256=97g9ui8baC7RdqzB6EPxgkLvGaiX_-r24igTSlXyfcs,5537
+torchrec/modules/embedding_configs.py,sha256=5lb9NeX-hSx6HTwiwV9at70mvAKGjfaKiSpKfx37rBw,6468
 torchrec/modules/embedding_modules.py,sha256=ezRcQ2BqgEEdDF-86Aeribm44YHtaA21NrgOvfr_KYM,14021
 torchrec/modules/embedding_tower.py,sha256=rHiMEUUMoMZUxIPKBE2HyI7I5uNthGQsZIxH038TmoI,4858
 torchrec/modules/feature_processor.py,sha256=UqDELZQ7cRpAQb_6LyxwVByJDdM5NPDfAyEk4qYQmKM,12360
-torchrec/modules/feature_processor_.py,sha256=Cvhuim-U8t84jL_h5EEAM7Yiwo1SOoSLHA5Gtkf4Hfc,4830
+torchrec/modules/feature_processor_.py,sha256=y6OSfvgmNSvhe00Xwy69Yqu5mwkF24nO2I4G5iu_ONc,4832
 torchrec/modules/fp_embedding_modules.py,sha256=AdUxhEODvE-h0FbqQoD0o-haLBgMRhXl2O0gvcstxI0,4403
-torchrec/modules/fused_embedding_modules.py,sha256=FsScroCb_IN8WhI_CjM0IkPgQrlrv7aU0XPm7dtsNkM,31453
-torchrec/modules/lazy_extension.py,sha256=iYkjlFGzpI1dbVZ7ofTN1OIA7FI-IlNgM57v3EymPE0,10894
+torchrec/modules/fused_embedding_modules.py,sha256=4nyD7aJYasPXqQElg8u3Wmh1n_t-BSe3rd2qxN4WO-k,31545
+torchrec/modules/lazy_extension.py,sha256=bulbZhpIB5QMDy4I7SlE3lLNO0lovKxj5BmqRWfVMpA,10541
 torchrec/modules/mlp.py,sha256=lV3vCEmNLI1kDtF4eGlCaGvtG3FQ8UEMs4Hcc6Nf3pM,6309
-torchrec/modules/utils.py,sha256=Ohx144TmZCEHbv3oEUsBf8e4DkGjmyPf98N4mA8kCxo,4022
+torchrec/modules/utils.py,sha256=4xCBc_dTQ8CFNLdGtJcCa3Ei0zScfkZCSmnSxOq51vk,3897
+torchrec/modules/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+torchrec/modules/tests/test_activation.py,sha256=kU7vmPjPTaDaLbwPj0CM-OG8KPvxhcyBj86jzjEEyVg,855
+torchrec/modules/tests/test_code_quality.py,sha256=-lzTUi2Gbqoio4efoY9_V5o7ZlOnslVutfqFsvmjPzk,1145
+torchrec/modules/tests/test_crossnet.py,sha256=mBQ2mHTsKyuxwKyS9mK-QHxJPw7Sx9fWyagGqi4uAN0,5328
+torchrec/modules/tests/test_deepfm.py,sha256=vtSbjUBC2KL1wZmyx7UAjCXgPplEd8FMmDm6Rs8rH6g,5095
+torchrec/modules/tests/test_embedding_modules.py,sha256=m1p6nEk45R2PgcxLwVTuPl1fTuMhgxSV5eb0IfyhBp0,10958
+torchrec/modules/tests/test_feature_processor.py,sha256=D4FSWy8mKL_xewqE558HQsxpwXXxr8H_2Kq9XumsDSU,3476
+torchrec/modules/tests/test_fused_embedding_modules.py,sha256=Um7pe58FkpNhu6xq24Q5G36HOQBqFRkKIkvb6X5twEo,36277
+torchrec/modules/tests/test_lazy_extension.py,sha256=EghXMcRVL_nA0R3IerV8tYxolGuSsqQXMxGX52f6xlU,11158
+torchrec/modules/tests/test_mlp.py,sha256=w-AZaY5LG9UBsrVPtptfcq6BMmVLSaVH2DO8j23PvOQ,3325
 torchrec/optim/__init__.py,sha256=4-nuv6JsmuWBtzyUvCKJ0b9-m7oFi8QB2b3krFF0KgQ,1639
 torchrec/optim/apply_optimizer_in_backward.py,sha256=0wjamGai9i0rXvIf4GNYNhCz7NtkH_9expuepk1qcbI,2012
 torchrec/optim/clipping.py,sha256=sDotlb8Sf4D7-lbBxhzRDFHoiO_DVx34F1J8vOEWq8I,1569
 torchrec/optim/fused.py,sha256=J4u2PWaHD65PIEdg0wTWoK_riZCoSKAVKYPGuZtfKLY,1353
 torchrec/optim/keyed.py,sha256=5QASHSkw2oYwu3OVHU5JJ2mm5tQaSCOQ3z_vBVRLPtk,16069
 torchrec/optim/optimizers.py,sha256=tmf-ww_47F_tu04ufffVCczM2AOMR5yTNh_8S-gJl-8,4420
 torchrec/optim/rowwise_adagrad.py,sha256=jHpCZDFWRrXbwlKiwROg2dl0qK1lG2uXMJkTtbZ_uSg,7405
 torchrec/optim/warmup.py,sha256=QaMcWU-jMZbDOfRHEH_x9r7EsjtI_LRgOGAmEgzJWSQ,4865
 torchrec/optim/test_utils/__init__.py,sha256=mkNZr5iNV3kseuamPBnnAeknjbv4ELPFMGyJ1lWiJGU,560
+torchrec/optim/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+torchrec/optim/tests/test_apply_optimizer_in_backward.py,sha256=jyZspVuT_u0LgrexNaertJDOeIujNpM_EAO7W_WB2Ho,3377
+torchrec/optim/tests/test_clipping.py,sha256=DZ_2Hcx8x4ryU3seWT5jerrEJRaKZn27vDELgs3C45Y,8255
+torchrec/optim/tests/test_keyed.py,sha256=zr7grUrhrodwXob4P7RqiARkzC7xMkeo_wjVuWV0Wmw,12347
+torchrec/optim/tests/test_rowwise_adagrad.py,sha256=ynH9rHH452Dl6NOuzUSOXd49lYDy_Ti1clYkVqRB82s,1973
+torchrec/optim/tests/test_warmup.py,sha256=Z7PKIe0KmifAYMAcNYoZ5oo5P4Vd5rlU9f_cmwF9fbw,2486
 torchrec/quant/__init__.py,sha256=A6NIA6ztq6iP1JTLRLNzlgnCcd-LaN8efnxGub3Ii4A,1140
-torchrec/quant/embedding_modules.py,sha256=EKWK6_AkLSSj3Hc-capmN2_VXY52s0pfuNqyDvjPX5M,25656
-torchrec/quant/utils.py,sha256=ab7J2QfHjeB7UF1BRh20KygcJR5ZHKwRMImgyCZOagE,4296
+torchrec/quant/embedding_modules.py,sha256=-_5_HaoNpt3AmL7fapO2Wj2r6WPjbq2VvATNmGhrai0,26618
+torchrec/quant/utils.py,sha256=rcyo5LDcLK49VLs6ZFxOHeutblWZunDAM_T-0NsraDE,4292
 torchrec/sparse/__init__.py,sha256=dLqSye4Jo6obnNNTUKdPDxPQb9sL2U4weemSn-DjpYk,1163
-torchrec/sparse/jagged_tensor.py,sha256=3874Ka-1XE6nsvHIVu8iGM6l3nNlSF7PQW-fM5rnl4c,55583
+torchrec/sparse/jagged_tensor.py,sha256=f0t3I-I8E-9El17qp5ip9n8Ap7nftlrZGQj-TKH4_2I,56945
 torchrec/sparse/test_utils/__init__.py,sha256=BLxfGKJvwjjCiQM64O5wGAA_Cea0sG-buw9lTDWuqug,1430
+torchrec/sparse/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+torchrec/sparse/tests/test_jagged_tensor.py,sha256=EKSwn5v-6iOux6l8McqkwhWdz1foj4H8-nViCn5zdUs,53408
 torchrec/test_utils/__init__.py,sha256=JncJcXS4N3gI7-fsizQ2-qiWM6MhIrpvskF_9gDf0Go,5661
-torchrec_nightly-2023.6.9.dist-info/LICENSE,sha256=e0Eotbf_rHOYPuEUlppIbvwy4SN98CZnl_hqwvbDA4Q,1530
-torchrec_nightly-2023.6.9.dist-info/METADATA,sha256=mRb6bQBNu8fDMGkIss2u0G4F8zWTV4sjjEH7LX0f13Q,5011
-torchrec_nightly-2023.6.9.dist-info/WHEEL,sha256=ns_9KNZvwSNZtRgVV_clzMUG_fXjGc5Z8Tx4hxQ0gkw,93
-torchrec_nightly-2023.6.9.dist-info/top_level.txt,sha256=LoLcTAPLj_7x62AuyYmhEVBcx2WJ1Z1Nrknv0Jnk_gQ,9
-torchrec_nightly-2023.6.9.dist-info/RECORD,,
+torchrec_nightly-2023.7.12.dist-info/LICENSE,sha256=e0Eotbf_rHOYPuEUlppIbvwy4SN98CZnl_hqwvbDA4Q,1530
+torchrec_nightly-2023.7.12.dist-info/METADATA,sha256=5risJtJa2pluhlm7fe4YuXOMqTADOD-XSS_rW7xZQ28,5012
+torchrec_nightly-2023.7.12.dist-info/WHEEL,sha256=ulNLUY3a1ygklsCRR-EsvmfrndvYrXDy4w6NgU-PhwQ,106
+torchrec_nightly-2023.7.12.dist-info/top_level.txt,sha256=LoLcTAPLj_7x62AuyYmhEVBcx2WJ1Z1Nrknv0Jnk_gQ,9
+torchrec_nightly-2023.7.12.dist-info/RECORD,,
```


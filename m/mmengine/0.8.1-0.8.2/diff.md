# Comparing `tmp/mmengine-0.8.1.tar.gz` & `tmp/mmengine-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmengine-0.8.1.tar", last modified: Thu Jul  6 02:23:14 2023, max compression
+gzip compressed data, was "dist/mmengine-0.8.2.tar", last modified: Wed Jul 12 03:01:45 2023, max compression
```

## Comparing `mmengine-0.8.1.tar` & `mmengine-0.8.2.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-06 02:21:50.000000 mmengine-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-07-06 02:23:14.000000 mmengine-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17510 2023-07-06 02:21:50.000000 mmengine-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/_strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/_strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39482 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/_strategy/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/_strategy/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/_strategy/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    26640 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/_strategy/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/_strategy/single_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/_strategy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/analysis/complexity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/analysis/jit_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/analysis/jit_handles.py
--rw-r--r--   0 runner    (1001) docker     (123)    31115 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/analysis/print_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/config/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71175 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/config/lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33863 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dataset/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dataset/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dataset/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/device/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/device/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43256 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dist/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/evaluator/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/evaluator/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/evaluator/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/evaluator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/fileio/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/http_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/lmdb_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/memcached_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/petrel_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/handlers/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29409 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/early_stopping_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/ema_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/empty_cache_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/iter_timer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/logger_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/naive_visualization_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/param_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/profiler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/runtime_info_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/sampler_seed_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/sync_buffer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/test_time_aug_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hub/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hub/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hub/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hub/openmmlab.json
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hub/torchvision_0.12.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/infer/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/infer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27712 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/infer/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/logging/history_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/logging/message_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/averaged_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/model/base_model/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/base_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/base_model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/base_model/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/model/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/wrappers/_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/wrappers/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/wrappers/fully_sharded_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/wrappers/seperate_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/wrappers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/optim/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/amp_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/apex_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/optimizer_wrapper_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/zero_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/optim/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/scheduler/momentum_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    64430 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/scheduler/param_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/registry/build_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/registry/default_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    26948 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/registry/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/registry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66277 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/_flexible_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/base_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    30359 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/log_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/loops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)   101587 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/structures/base_data_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/structures/instance_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/structures/label_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/structures/pixel_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/testing/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/testing/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/testing/_internal/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/testing/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/testing/runner_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/utils/dl_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/torch_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36637 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/visualization/vis_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    53917 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/visualization/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-06 02:23:14.000000 mmengine-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-06 02:21:50.000000 mmengine-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 03:00:23.000000 mmengine-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-07-12 03:01:45.000000 mmengine-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17510 2023-07-12 03:00:23.000000 mmengine-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/_strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/_strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39482 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/_strategy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/_strategy/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/_strategy/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26640 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/_strategy/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/_strategy/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/_strategy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/analysis/complexity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/analysis/jit_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/analysis/jit_handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31115 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/analysis/print_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72405 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/config/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33863 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dataset/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dataset/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dataset/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/device/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43256 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dist/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/evaluator/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/evaluator/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/evaluator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/fileio/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/http_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/lmdb_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/memcached_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/petrel_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/handlers/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29409 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/early_stopping_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/ema_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/empty_cache_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/iter_timer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/logger_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/naive_visualization_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/param_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/profiler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/runtime_info_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/sampler_seed_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/sync_buffer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/test_time_aug_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hub/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hub/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hub/openmmlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hub/torchvision_0.12.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/infer/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27712 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/infer/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/logging/history_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/logging/message_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/averaged_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/model/base_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/base_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/base_model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/base_model/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/model/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/wrappers/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/wrappers/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/wrappers/fully_sharded_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/wrappers/seperate_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/wrappers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/optim/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/amp_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/apex_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/optimizer_wrapper_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/zero_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/optim/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/scheduler/momentum_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64430 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/scheduler/param_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/registry/build_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/registry/default_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26948 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/registry/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/registry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66277 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/_flexible_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/base_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30359 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/log_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101587 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/structures/base_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/structures/instance_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/structures/label_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/structures/pixel_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/testing/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/testing/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/testing/_internal/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/testing/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/testing/runner_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/utils/dl_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/torch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36637 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/visualization/vis_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53917 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/visualization/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-12 03:01:45.000000 mmengine-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-12 03:00:23.000000 mmengine-0.8.2/setup.py
```

### Comparing `mmengine-0.8.1/PKG-INFO` & `mmengine-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine
-Version: 0.8.1
+Version: 0.8.2
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmengine Version: 0.8.1 Summary: Engine of
+Metadata-Version: 2.1 Name: mmengine Version: 0.8.2 Summary: Engine of
 OpenMMLab projects Home-page: https://github.com/open-mmlab/mmengine Author:
 MMEngine Authors Author-email: openmmlab@gmail.com License: UNKNOWN
 Description:
  [https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-
                           429b-9354-c6fac64b7ef8.jpg]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
```

### Comparing `mmengine-0.8.1/README.md` & `mmengine-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/_strategy/__init__.py` & `mmengine-0.8.2/mmengine/_strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/_strategy/base.py` & `mmengine-0.8.2/mmengine/_strategy/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/_strategy/deepspeed.py` & `mmengine-0.8.2/mmengine/_strategy/deepspeed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/_strategy/distributed.py` & `mmengine-0.8.2/mmengine/_strategy/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/_strategy/fsdp.py` & `mmengine-0.8.2/mmengine/_strategy/fsdp.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/_strategy/single_device.py` & `mmengine-0.8.2/mmengine/_strategy/single_device.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/_strategy/utils.py` & `mmengine-0.8.2/mmengine/_strategy/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/analysis/complexity_analysis.py` & `mmengine-0.8.2/mmengine/analysis/complexity_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/analysis/jit_analysis.py` & `mmengine-0.8.2/mmengine/analysis/jit_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/analysis/jit_handles.py` & `mmengine-0.8.2/mmengine/analysis/jit_handles.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/analysis/print_helper.py` & `mmengine-0.8.2/mmengine/analysis/print_helper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/config/config.py` & `mmengine-0.8.2/mmengine/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,32 @@
                 return a if a is not default else b
 
         merged = _merge_a_into_b(copy.deepcopy(other), copy.deepcopy(self))
         self.clear()
         for key, value in merged.items():
             self[key] = value
 
+    def __getstate__(self):
+        state = {}
+        for key, value in super().items():
+            state[key] = value
+        return state
+
+    def __setstate__(self, state):
+        for key, value in state.items():
+            self[key] = value
+
+    def __eq__(self, other):
+        if isinstance(other, ConfigDict):
+            return other.to_dict() == self.to_dict()
+        elif isinstance(other, dict):
+            return {k: v for k, v in self.items()} == other
+        else:
+            return False
+
     def _to_lazy_dict(self):
         """Convert the ConfigDict to a normal dictionary recursively, and keep
         the ``LazyObject`` or ``LazyAttr`` object not built."""
 
         def _to_dict(data):
             if isinstance(data, ConfigDict):
                 return {
@@ -277,16 +295,16 @@
                 return type(data)(_to_dict(item) for item in data)
             else:
                 return data
 
         return _to_dict(self)
 
     def to_dict(self):
-        """Convert the ConfigDict to a normal dictionary recursively, and keep
-        the ``LazyObject`` or ``LazyAttr`` object not built."""
+        """Convert the ConfigDict to a normal dictionary recursively, and
+        convert the ``LazyObject`` or ``LazyAttr`` to string."""
         return _lazy2string(self, dict_type=dict)
 
 
 def add_args(parser: ArgumentParser,
              cfg: dict,
              prefix: str = '') -> ArgumentParser:
     """Add config fields into argument parser.
@@ -359,20 +377,22 @@
         "{'item1': [1, 2], 'item2': {'a': 0}, 'item3': True, 'item4': 'test'}"
 
     You can find more advance usage in the `config tutorial`_.
 
     .. _config tutorial: https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html
     """  # noqa: E501
 
-    def __init__(self,
-                 cfg_dict: dict = None,
-                 cfg_text: Optional[str] = None,
-                 filename: Optional[Union[str, Path]] = None,
-                 env_variables: Optional[dict] = None,
-                 format_python_code: bool = True):
+    def __init__(
+        self,
+        cfg_dict: dict = None,
+        cfg_text: Optional[str] = None,
+        filename: Optional[Union[str, Path]] = None,
+        env_variables: Optional[dict] = None,
+        format_python_code: bool = True,
+    ):
         filename = str(filename) if isinstance(filename, Path) else filename
         if cfg_dict is None:
             cfg_dict = dict()
         elif not isinstance(cfg_dict, dict):
             raise TypeError('cfg_dict must be a dict, but '
                             f'got {type(cfg_dict)}')
         for key in cfg_dict:
@@ -380,14 +400,17 @@
                 raise KeyError(f'{key} is reserved for config file')
 
         if not isinstance(cfg_dict, ConfigDict):
             cfg_dict = ConfigDict(cfg_dict)
         super().__setattr__('_cfg_dict', cfg_dict)
         super().__setattr__('_filename', filename)
         super().__setattr__('_format_python_code', format_python_code)
+        if not hasattr(self, '_imported_names'):
+            super().__setattr__('_imported_names', set())
+
         if cfg_text:
             text = cfg_text
         elif filename:
             with open(filename, encoding='utf-8') as f:
                 text = f.read()
         else:
             text = ''
@@ -417,19 +440,19 @@
             format_python_code (bool): Whether to format Python code by yapf.
                 Defaults to True.
 
         Returns:
             Config: Config instance built from config file.
         """
         filename = str(filename) if isinstance(filename, Path) else filename
-        if lazy_import is None:
-            lazy_import = Config._is_lazy_import(filename)
-        if not lazy_import:
+        if lazy_import is False or \
+           lazy_import is None and not Config._is_lazy_import(filename):
             cfg_dict, cfg_text, env_variables = Config._file2dict(
-                filename, use_predefined_variables, use_environment_variables)
+                filename, use_predefined_variables, use_environment_variables,
+                lazy_import)
             if import_custom_modules and cfg_dict.get('custom_imports', None):
                 try:
                     import_modules_from_strings(**cfg_dict['custom_imports'])
                 except ImportError as e:
                     err_msg = (
                         'Failed to import custom modules from '
                         f"{cfg_dict['custom_imports']}, the current sys.path "
@@ -441,35 +464,31 @@
                         'include the directory which contains your custom '
                         'module')
                     raise ImportError(err_msg) from e
             return Config(
                 cfg_dict,
                 cfg_text=cfg_text,
                 filename=filename,
-                env_variables=env_variables)
+                env_variables=env_variables,
+            )
         else:
             # Enable lazy import when parsing the config.
             # Using try-except to make sure ``ConfigDict.lazy`` will be reset
             # to False. See more details about lazy in the docstring of
             # ConfigDict
             ConfigDict.lazy = True
             try:
                 cfg_dict, imported_names = Config._parse_lazy_import(filename)
             except Exception as e:
                 raise e
             finally:
+                # disable lazy import to get the real type. See more details
+                # about lazy in the docstring of ConfigDict
                 ConfigDict.lazy = False
 
-            # delete builtin imported objects
-            for key, value in list(cfg_dict._to_lazy_dict().items()):
-                if isinstance(value, (types.FunctionType, types.ModuleType)):
-                    cfg_dict.pop(key)
-
-            # disable lazy import to get the real type. See more details about
-            # lazy in the docstring of ConfigDict
             cfg = Config(
                 cfg_dict,
                 filename=filename,
                 format_python_code=format_python_code)
             object.__setattr__(cfg, '_imported_names', imported_names)
             return cfg
 
@@ -790,26 +809,30 @@
 
         return cfg
 
     @staticmethod
     def _file2dict(
             filename: str,
             use_predefined_variables: bool = True,
-            use_environment_variables: bool = True) -> Tuple[dict, str, dict]:
+            use_environment_variables: bool = True,
+            lazy_import: Optional[bool] = None) -> Tuple[dict, str, dict]:
         """Transform file to variables dictionary.
 
         Args:
             filename (str): Name of config file.
             use_predefined_variables (bool, optional): Whether to use
                 predefined variables. Defaults to True.
+            lazy_import (bool): Whether to load config in `lazy_import` mode.
+                If it is `None`, it will be deduced by the content of the
+                config file. Defaults to None.
 
         Returns:
             Tuple[dict, str]: Variables dictionary and text of Config.
         """
-        if Config._is_lazy_import(filename):
+        if lazy_import is None and Config._is_lazy_import(filename):
             raise RuntimeError(
                 'The configuration file type in the inheritance chain '
                 'must match the current configuration file type, either '
                 '"lazy_import" or non-"lazy_import". You got this error '
                 'since you use the syntax like `with read_base(): ...` '
                 f'or import non-builtin module in {filename}. See more '
                 'information in https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html'  # noqa: E501
@@ -848,15 +871,17 @@
                 for base_cfg_path in Config._get_base_files(
                         temp_config_file.name):
                     base_cfg_path, scope = Config._get_cfg_path(
                         base_cfg_path, filename)
                     _cfg_dict, _cfg_text, _env_variables = Config._file2dict(
                         filename=base_cfg_path,
                         use_predefined_variables=use_predefined_variables,
-                        use_environment_variables=use_environment_variables)
+                        use_environment_variables=use_environment_variables,
+                        lazy_import=lazy_import,
+                    )
                     cfg_text_list.append(_cfg_text)
                     env_variables.update(_env_variables)
                     duplicate_keys = base_cfg_dict.keys() & _cfg_dict.keys()
                     if len(duplicate_keys) > 0:
                         raise KeyError(
                             'Duplicate key is not allowed among bases. '
                             f'Duplicate keys: {duplicate_keys}')
@@ -992,15 +1017,15 @@
         #    with the base_dict.
         #
         # 4. During the parsing process, all imported variable will be
         #    recorded in the `imported_names` set. These variables can be
         #    accessed, but will not be dumped by default.
 
         with open(filename, encoding='utf-8') as f:
-            global_dict = {'LazyObject': LazyObject}
+            global_dict = {'LazyObject': LazyObject, '__file__': filename}
             base_dict = {}
 
             parsed_codes = ast.parse(f.read())
             # get the names of base modules, and remove the
             # `with read_base():'` statement
             base_modules = Config._get_base_modules(parsed_codes.body)
             base_imported_names = set()
@@ -1466,17 +1491,21 @@
         if isinstance(value, dict):
             value = ConfigDict(value)
         self._cfg_dict.__setitem__(name, value)
 
     def __iter__(self):
         return iter(self._cfg_dict)
 
-    def __getstate__(self) -> Tuple[dict, Optional[str], Optional[str], dict]:
-        return (self._cfg_dict, self._filename, self._text,
-                self._env_variables)
+    def __getstate__(
+            self
+    ) -> Tuple[dict, Optional[str], Optional[str], dict, bool, set]:
+        state = (self._cfg_dict, self._filename, self._text,
+                 self._env_variables, self._format_python_code,
+                 self._imported_names)
+        return state
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         other = cls.__new__(cls)
         memo[id(self)] = other
 
         for key, value in self.__dict__.items():
@@ -1491,20 +1520,21 @@
         super(Config, other).__setattr__('_cfg_dict', self._cfg_dict.copy())
 
         return other
 
     copy = __copy__
 
     def __setstate__(self, state: Tuple[dict, Optional[str], Optional[str],
-                                        dict]):
-        _cfg_dict, _filename, _text, _env_variables = state
-        super().__setattr__('_cfg_dict', _cfg_dict)
-        super().__setattr__('_filename', _filename)
-        super().__setattr__('_text', _text)
-        super().__setattr__('_text', _env_variables)
+                                        dict, bool, set]):
+        super().__setattr__('_cfg_dict', state[0])
+        super().__setattr__('_filename', state[1])
+        super().__setattr__('_text', state[2])
+        super().__setattr__('_env_variables', state[3])
+        super().__setattr__('_format_python_code', state[4])
+        super().__setattr__('_imported_names', state[5])
 
     def dump(self, file: Optional[Union[str, Path]] = None):
         """Dump config to file or return config text.
 
         Args:
             file (str or Path, optional): If not specified, then the object
             is dumped to a str, otherwise to a file specified by the filename.
@@ -1612,16 +1642,16 @@
             if isinstance(node, ast.Import):
                 for alias_node in node.names:
                     if not _is_builtin_module(alias_node.name):
                         return True
         return False
 
     def _to_lazy_dict(self, keep_imported: bool = False) -> dict:
-        """Convert config object to dictionary and filter the imported
-        object."""
+        """Convert config object to dictionary with lazy object, and filter the
+        imported object."""
         res = self._cfg_dict._to_lazy_dict()
         if hasattr(self, '_imported_names') and not keep_imported:
             res = {
                 key: value
                 for key, value in res.items()
                 if key not in self._imported_names
             }
@@ -1633,15 +1663,22 @@
         Args:
             keep_imported (bool): Whether to keep the imported field.
                 Defaults to False
 
         If you import third-party objects in the config file, all imported
         objects will be converted to a string like ``torch.optim.SGD``
         """
-        return self._cfg_dict.to_dict()
+        cfg_dict = self._cfg_dict.to_dict()
+        if hasattr(self, '_imported_names') and not keep_imported:
+            cfg_dict = {
+                key: value
+                for key, value in cfg_dict.items()
+                if key not in self._imported_names
+            }
+        return cfg_dict
 
 
 class DictAction(Action):
     """
     argparse action to split an argument into KEY=VALUE form
     on the first = and append to a dictionary. List options can
     be passed as comma separated values, i.e 'KEY=V1,V2,V3', or with explicit
```

### Comparing `mmengine-0.8.1/mmengine/config/lazy.py` & `mmengine-0.8.2/mmengine/config/lazy.py`

 * *Files 14% similar despite different names*

```diff
@@ -117,14 +117,24 @@
     def __str__(self) -> str:
         if self._imported is not None:
             return self._imported
         return self.module
 
     __repr__ = __str__
 
+    # `pickle.dump` will try to get the `__getstate__` and `__setstate__`
+    # methods of the dumped object. If these two methods are not defined,
+    # LazyObject will return a `__getstate__` LazyObject` or `__setstate__`
+    # LazyObject.
+    def __getstate__(self):
+        return self.__dict__
+
+    def __setstate__(self, state):
+        self.__dict__ = state
+
 
 class LazyAttr:
     """The attribute of the LazyObject.
 
     When parsing the configuration file, the imported syntax will be
     parsed as the assignment ``LazyObject``. During the subsequent parsing
     process, users may reference the attributes of the LazyObject.
@@ -215,7 +225,17 @@
         except ImportError as e:
             raise e
 
     def __str__(self) -> str:
         return self.name
 
     __repr__ = __str__
+
+    # `pickle.dump` will try to get the `__getstate__` and `__setstate__`
+    # methods of the dumped object. If these two methods are not defined,
+    # LazyAttr will return a `__getstate__` LazyAttr` or `__setstate__`
+    # LazyAttr.
+    def __getstate__(self):
+        return self.__dict__
+
+    def __setstate__(self, state):
+        self.__dict__ = state
```

### Comparing `mmengine-0.8.1/mmengine/config/utils.py` & `mmengine-0.8.2/mmengine/config/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,14 +161,16 @@
     Arg:
         module_name: name of module.
     """
     if module_name.startswith('.'):
         return False
     if module_name.startswith('mmengine.config'):
         return True
+    if module_name in sys.builtin_module_names:
+        return True
     spec = find_spec(module_name.split('.')[0])
     # Module not found
     if spec is None:
         return False
     origin_path = getattr(spec, 'origin', None)
     if origin_path is None:
         return False
@@ -310,14 +312,23 @@
                   node will be directly returned
                 * Otherwise, it will return the assignment statements of
                   ``LazyObject``.
         """
         # Built-in modules will not be parsed as LazyObject
         module = f'{node.level*"."}{node.module}'
         if _is_builtin_module(module):
+            # Make sure builtin module will be added into `self.imported_obj`
+            for alias in node.names:
+                if alias.asname is not None:
+                    self.imported_obj.add(alias.asname)
+                elif alias.name == '*':
+                    raise ConfigParsingError(
+                        'Cannot import * from non-base config')
+                else:
+                    self.imported_obj.add(alias.name)
             return node
 
         if module in self.base_dict:
             for alias_node in node.names:
                 if alias_node.name == '*':
                     self.global_dict.update(self.base_dict[module])
                     return None
@@ -405,14 +416,16 @@
         assert len(alias_list) == 1, (
             'Illegal syntax in config! import multiple modules in one line is '
             'not supported')
         # TODO Support multiline import
         alias = alias_list[0]
         if alias.asname is not None:
             self.imported_obj.add(alias.asname)
+            if _is_builtin_module(alias.name.split('.')[0]):
+                return node
             return ast.parse(  # type: ignore
                 f'{alias.asname} = LazyObject('
                 f'"{alias.name}",'
                 f'location="{self.filename}, line {node.lineno}")').body[0]
         return node
```

### Comparing `mmengine-0.8.1/mmengine/dataset/__init__.py` & `mmengine-0.8.2/mmengine/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/dataset/base_dataset.py` & `mmengine-0.8.2/mmengine/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/dataset/dataset_wrapper.py` & `mmengine-0.8.2/mmengine/dataset/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/dataset/sampler.py` & `mmengine-0.8.2/mmengine/dataset/sampler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/dataset/utils.py` & `mmengine-0.8.2/mmengine/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/device/utils.py` & `mmengine-0.8.2/mmengine/device/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/dist/__init__.py` & `mmengine-0.8.2/mmengine/dist/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/dist/dist.py` & `mmengine-0.8.2/mmengine/dist/dist.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/dist/utils.py` & `mmengine-0.8.2/mmengine/dist/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/evaluator/evaluator.py` & `mmengine-0.8.2/mmengine/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/evaluator/metric.py` & `mmengine-0.8.2/mmengine/evaluator/metric.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/evaluator/utils.py` & `mmengine-0.8.2/mmengine/evaluator/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/__init__.py` & `mmengine-0.8.2/mmengine/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/backends/__init__.py` & `mmengine-0.8.2/mmengine/fileio/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/backends/base.py` & `mmengine-0.8.2/mmengine/fileio/backends/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/backends/http_backend.py` & `mmengine-0.8.2/mmengine/fileio/backends/http_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/backends/lmdb_backend.py` & `mmengine-0.8.2/mmengine/fileio/backends/lmdb_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/backends/local_backend.py` & `mmengine-0.8.2/mmengine/fileio/backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/backends/memcached_backend.py` & `mmengine-0.8.2/mmengine/fileio/backends/memcached_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/backends/petrel_backend.py` & `mmengine-0.8.2/mmengine/fileio/backends/petrel_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/backends/registry_utils.py` & `mmengine-0.8.2/mmengine/fileio/backends/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/file_client.py` & `mmengine-0.8.2/mmengine/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/handlers/base.py` & `mmengine-0.8.2/mmengine/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/handlers/json_handler.py` & `mmengine-0.8.2/mmengine/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/handlers/pickle_handler.py` & `mmengine-0.8.2/mmengine/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/handlers/registry_utils.py` & `mmengine-0.8.2/mmengine/fileio/handlers/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/handlers/yaml_handler.py` & `mmengine-0.8.2/mmengine/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/io.py` & `mmengine-0.8.2/mmengine/fileio/io.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/fileio/parse.py` & `mmengine-0.8.2/mmengine/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hooks/__init__.py` & `mmengine-0.8.2/mmengine/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hooks/checkpoint_hook.py` & `mmengine-0.8.2/mmengine/hooks/checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hooks/early_stopping_hook.py` & `mmengine-0.8.2/mmengine/hooks/early_stopping_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hooks/ema_hook.py` & `mmengine-0.8.2/mmengine/hooks/ema_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hooks/empty_cache_hook.py` & `mmengine-0.8.2/mmengine/hooks/empty_cache_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hooks/hook.py` & `mmengine-0.8.2/mmengine/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hooks/iter_timer_hook.py` & `mmengine-0.8.2/mmengine/hooks/iter_timer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hooks/logger_hook.py` & `mmengine-0.8.2/mmengine/hooks/logger_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hooks/naive_visualization_hook.py` & `mmengine-0.8.2/mmengine/hooks/naive_visualization_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hooks/param_scheduler_hook.py` & `mmengine-0.8.2/mmengine/hooks/param_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hooks/profiler_hook.py` & `mmengine-0.8.2/mmengine/hooks/profiler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hooks/runtime_info_hook.py` & `mmengine-0.8.2/mmengine/hooks/runtime_info_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hooks/sampler_seed_hook.py` & `mmengine-0.8.2/mmengine/hooks/sampler_seed_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hooks/sync_buffer_hook.py` & `mmengine-0.8.2/mmengine/hooks/sync_buffer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hooks/test_time_aug_hook.py` & `mmengine-0.8.2/mmengine/hooks/test_time_aug_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hub/hub.py` & `mmengine-0.8.2/mmengine/hub/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hub/mmcls.json` & `mmengine-0.8.2/mmengine/hub/mmcls.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hub/openmmlab.json` & `mmengine-0.8.2/mmengine/hub/openmmlab.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/hub/torchvision_0.12.json` & `mmengine-0.8.2/mmengine/hub/torchvision_0.12.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/infer/infer.py` & `mmengine-0.8.2/mmengine/infer/infer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/logging/history_buffer.py` & `mmengine-0.8.2/mmengine/logging/history_buffer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/logging/logger.py` & `mmengine-0.8.2/mmengine/logging/logger.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/logging/message_hub.py` & `mmengine-0.8.2/mmengine/logging/message_hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/model/__init__.py` & `mmengine-0.8.2/mmengine/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/model/averaged_model.py` & `mmengine-0.8.2/mmengine/model/averaged_model.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/model/base_model/base_model.py` & `mmengine-0.8.2/mmengine/model/base_model/base_model.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/model/base_model/data_preprocessor.py` & `mmengine-0.8.2/mmengine/model/base_model/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/model/base_module.py` & `mmengine-0.8.2/mmengine/model/base_module.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/model/test_time_aug.py` & `mmengine-0.8.2/mmengine/model/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/model/utils.py` & `mmengine-0.8.2/mmengine/model/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/model/weight_init.py` & `mmengine-0.8.2/mmengine/model/weight_init.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/model/wrappers/__init__.py` & `mmengine-0.8.2/mmengine/model/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/model/wrappers/_deepspeed.py` & `mmengine-0.8.2/mmengine/model/wrappers/_deepspeed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/model/wrappers/distributed.py` & `mmengine-0.8.2/mmengine/model/wrappers/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/model/wrappers/fully_sharded_distributed.py` & `mmengine-0.8.2/mmengine/model/wrappers/fully_sharded_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/model/wrappers/seperate_distributed.py` & `mmengine-0.8.2/mmengine/model/wrappers/seperate_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/model/wrappers/utils.py` & `mmengine-0.8.2/mmengine/model/wrappers/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/optim/__init__.py` & `mmengine-0.8.2/mmengine/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/optim/optimizer/__init__.py` & `mmengine-0.8.2/mmengine/optim/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/optim/optimizer/_deepspeed.py` & `mmengine-0.8.2/mmengine/optim/optimizer/_deepspeed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/optim/optimizer/amp_optimizer_wrapper.py` & `mmengine-0.8.2/mmengine/optim/optimizer/amp_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/optim/optimizer/apex_optimizer_wrapper.py` & `mmengine-0.8.2/mmengine/optim/optimizer/apex_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/optim/optimizer/base.py` & `mmengine-0.8.2/mmengine/optim/optimizer/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/optim/optimizer/builder.py` & `mmengine-0.8.2/mmengine/optim/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/optim/optimizer/default_constructor.py` & `mmengine-0.8.2/mmengine/optim/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/optim/optimizer/optimizer_wrapper.py` & `mmengine-0.8.2/mmengine/optim/optimizer/optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/optim/optimizer/optimizer_wrapper_dict.py` & `mmengine-0.8.2/mmengine/optim/optimizer/optimizer_wrapper_dict.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/optim/optimizer/zero_optimizer.py` & `mmengine-0.8.2/mmengine/optim/optimizer/zero_optimizer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/optim/scheduler/__init__.py` & `mmengine-0.8.2/mmengine/optim/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/optim/scheduler/lr_scheduler.py` & `mmengine-0.8.2/mmengine/optim/scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/optim/scheduler/momentum_scheduler.py` & `mmengine-0.8.2/mmengine/optim/scheduler/momentum_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/optim/scheduler/param_scheduler.py` & `mmengine-0.8.2/mmengine/optim/scheduler/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/registry/__init__.py` & `mmengine-0.8.2/mmengine/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/registry/build_functions.py` & `mmengine-0.8.2/mmengine/registry/build_functions.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/registry/default_scope.py` & `mmengine-0.8.2/mmengine/registry/default_scope.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/registry/registry.py` & `mmengine-0.8.2/mmengine/registry/registry.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/registry/root.py` & `mmengine-0.8.2/mmengine/registry/root.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/registry/utils.py` & `mmengine-0.8.2/mmengine/registry/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/runner/__init__.py` & `mmengine-0.8.2/mmengine/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/runner/_flexible_runner.py` & `mmengine-0.8.2/mmengine/runner/_flexible_runner.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/runner/amp.py` & `mmengine-0.8.2/mmengine/runner/amp.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/runner/base_loop.py` & `mmengine-0.8.2/mmengine/runner/base_loop.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/runner/checkpoint.py` & `mmengine-0.8.2/mmengine/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/runner/log_processor.py` & `mmengine-0.8.2/mmengine/runner/log_processor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/runner/loops.py` & `mmengine-0.8.2/mmengine/runner/loops.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/runner/priority.py` & `mmengine-0.8.2/mmengine/runner/priority.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/runner/runner.py` & `mmengine-0.8.2/mmengine/runner/runner.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/runner/utils.py` & `mmengine-0.8.2/mmengine/runner/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/structures/base_data_element.py` & `mmengine-0.8.2/mmengine/structures/base_data_element.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/structures/instance_data.py` & `mmengine-0.8.2/mmengine/structures/instance_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/structures/label_data.py` & `mmengine-0.8.2/mmengine/structures/label_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/structures/pixel_data.py` & `mmengine-0.8.2/mmengine/structures/pixel_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/testing/__init__.py` & `mmengine-0.8.2/mmengine/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/testing/_internal/distributed.py` & `mmengine-0.8.2/mmengine/testing/_internal/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/testing/compare.py` & `mmengine-0.8.2/mmengine/testing/compare.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/testing/runner_test_case.py` & `mmengine-0.8.2/mmengine/testing/runner_test_case.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/__init__.py` & `mmengine-0.8.2/mmengine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/dl_utils/__init__.py` & `mmengine-0.8.2/mmengine/utils/dl_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/dl_utils/collect_env.py` & `mmengine-0.8.2/mmengine/utils/dl_utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/dl_utils/hub.py` & `mmengine-0.8.2/mmengine/utils/dl_utils/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/dl_utils/misc.py` & `mmengine-0.8.2/mmengine/utils/dl_utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/dl_utils/parrots_wrapper.py` & `mmengine-0.8.2/mmengine/utils/dl_utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/dl_utils/setup_env.py` & `mmengine-0.8.2/mmengine/utils/dl_utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/dl_utils/time_counter.py` & `mmengine-0.8.2/mmengine/utils/dl_utils/time_counter.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/dl_utils/torch_ops.py` & `mmengine-0.8.2/mmengine/utils/dl_utils/torch_ops.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/dl_utils/trace.py` & `mmengine-0.8.2/mmengine/utils/dl_utils/trace.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/dl_utils/visualize.py` & `mmengine-0.8.2/mmengine/utils/dl_utils/visualize.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/manager.py` & `mmengine-0.8.2/mmengine/utils/manager.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/misc.py` & `mmengine-0.8.2/mmengine/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/package_utils.py` & `mmengine-0.8.2/mmengine/utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/path.py` & `mmengine-0.8.2/mmengine/utils/path.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/progressbar.py` & `mmengine-0.8.2/mmengine/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/timer.py` & `mmengine-0.8.2/mmengine/utils/timer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/utils/version_utils.py` & `mmengine-0.8.2/mmengine/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/version.py` & `mmengine-0.8.2/mmengine/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 
-__version__ = '0.8.1'
+__version__ = '0.8.2'
 
 
 def parse_version_info(version_str):
     """Parse the version information.
 
     Args:
         version_str (str): version string like '0.1.0'.
```

### Comparing `mmengine-0.8.1/mmengine/visualization/utils.py` & `mmengine-0.8.2/mmengine/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/visualization/vis_backend.py` & `mmengine-0.8.2/mmengine/visualization/vis_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine/visualization/visualizer.py` & `mmengine-0.8.2/mmengine/visualization/visualizer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/mmengine.egg-info/PKG-INFO` & `mmengine-0.8.2/mmengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine
-Version: 0.8.1
+Version: 0.8.2
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmengine Version: 0.8.1 Summary: Engine of
+Metadata-Version: 2.1 Name: mmengine Version: 0.8.2 Summary: Engine of
 OpenMMLab projects Home-page: https://github.com/open-mmlab/mmengine Author:
 MMEngine Authors Author-email: openmmlab@gmail.com License: UNKNOWN
 Description:
  [https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-
                           429b-9354-c6fac64b7ef8.jpg]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
```

### Comparing `mmengine-0.8.1/mmengine.egg-info/SOURCES.txt` & `mmengine-0.8.2/mmengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.1/setup.py` & `mmengine-0.8.2/setup.py`

 * *Files identical despite different names*


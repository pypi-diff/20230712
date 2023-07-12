# Comparing `tmp/vision_datasets-1.0.1.tar.gz` & `tmp/vision_datasets-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_datasets-1.0.1.tar", last modified: Mon Jul 10 20:31:16 2023, max compression
+gzip compressed data, was "vision_datasets-1.0.2.tar", last modified: Wed Jul 12 21:53:05 2023, max compression
```

## Comparing `vision_datasets-1.0.1.tar` & `vision_datasets-1.0.2.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.921956 vision_datasets-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.921956 vision_datasets-1.0.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/resources/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_box_alteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/tests/test_coco_adaptor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/coco_adaptor_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_caption_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_matting_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_regression_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_text_matching_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_multiclass_classification_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_multilabel_classification_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_multitask_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_object_detection_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_text_2_image_retrieval_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_format_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_dataset_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    45616 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_dataset_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_dataset_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_detection_as_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_ic_od_as_image_text_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_iris_format_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/tests/test_manifest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_manifest/test_pickleable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_manifest_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/tests/test_manifest_to_coco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_manifest_to_coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_manifest_to_coco/test_manifest_to_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/tests/test_merge_manifest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_merge_manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_merge_manifest/test_manifest_merge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/tests/test_sample/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_sample/test_sample_manfiest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/tests/test_spawn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_spawn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_spawn/test_spawn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/tests/test_torch_dataest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_torch_dataest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_torch_dataest/test_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/vision_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.929956 vision_datasets-1.0.1/vision_datasets/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/check_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/converter_od_to_ic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/converter_to_aml_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/converter_to_tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/converter_tsv_to_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/download_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/list_operations_by_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.929956 vision_datasets-1.0.1/vision_datasets/common/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.929956 vision_datasets-1.0.1/vision_datasets/common/data_manifest/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/data_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/iris_data_manifest_adaptor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.929956 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/balanced_instance_weights_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/generate_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/remove_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.929956 vision_datasets-1.0.1/vision_datasets/common/data_reader/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_reader/dataset_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_reader/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_reader/image_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.933956 vision_datasets-1.0.1/vision_datasets/common/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset/torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset/vision_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.933956 vision_datasets-1.0.1/vision_datasets/common/dataset_management/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset_management/dataset_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset_management/dataset_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.933956 vision_datasets-1.0.1/vision_datasets/common/factory/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/coco_manifest_adaptor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/data_manifest_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.933956 vision_datasets-1.0.1/vision_datasets/common/factory/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/balanced_instance_weights_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/coco_generator_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/manifest_merger_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/sampler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/spawn_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/split_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/supported_operations_by_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.933956 vision_datasets-1.0.1/vision_datasets/image_caption/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_caption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_caption/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_caption/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_caption/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.933956 vision_datasets-1.0.1/vision_datasets/image_classification/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_classification/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_classification/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_classification/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.933956 vision_datasets-1.0.1/vision_datasets/image_matting/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_matting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_matting/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_matting/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_matting/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/vision_datasets/image_object_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_object_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_object_detection/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_object_detection/detection_as_classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_object_detection/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_object_detection/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/vision_datasets/image_regression/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_regression/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_regression/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_regression/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/vision_datasets/image_text_matching/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_text_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_text_matching/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_text_matching/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_text_matching/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_text_matching/vision_as_image_text_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/vision_datasets/multi_task/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/multi_task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/multi_task/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/multi_task/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/vision_datasets/text_2_image_retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/text_2_image_retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/text_2_image_retrieval/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/text_2_image_retrieval/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/text_2_image_retrieval/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/vision_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-07-10 20:31:16.000000 vision_datasets-1.0.1/vision_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-10 20:31:16.000000 vision_datasets-1.0.1/vision_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:31:16.000000 vision_datasets-1.0.1/vision_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-10 20:31:16.000000 vision_datasets-1.0.1/vision_datasets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-10 20:31:16.000000 vision_datasets-1.0.1/vision_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 20:31:16.000000 vision_datasets-1.0.1/vision_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.858955 vision_datasets-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-07-12 21:53:05.858955 vision_datasets-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 21:53:05.858955 vision_datasets-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.818954 vision_datasets-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.818954 vision_datasets-1.0.2/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/resources/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_box_alteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.822954 vision_datasets-1.0.2/tests/test_coco_adaptor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_coco_adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_coco_adaptor/coco_adaptor_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_coco_adaptor/test_image_caption_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_coco_adaptor/test_image_matting_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_coco_adaptor/test_image_regression_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_coco_adaptor/test_image_text_matching_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_coco_adaptor/test_multiclass_classification_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_coco_adaptor/test_multilabel_classification_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_coco_adaptor/test_multitask_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_coco_adaptor/test_object_detection_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_coco_adaptor/test_text_2_image_retrieval_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_coco_format_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_dataset_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45616 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_dataset_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_dataset_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_detection_as_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_ic_od_as_image_text_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_iris_format_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.822954 vision_datasets-1.0.2/tests/test_manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_manifest/test_pickleable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_manifest_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.822954 vision_datasets-1.0.2/tests/test_manifest_to_coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_manifest_to_coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_manifest_to_coco/test_manifest_to_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.826954 vision_datasets-1.0.2/tests/test_merge_manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_merge_manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_merge_manifest/test_manifest_merge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.826954 vision_datasets-1.0.2/tests/test_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_sample/test_sample_manfiest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.826954 vision_datasets-1.0.2/tests/test_spawn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_spawn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_spawn/test_spawn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.826954 vision_datasets-1.0.2/tests/test_torch_dataest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_torch_dataest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_torch_dataest/test_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.826954 vision_datasets-1.0.2/vision_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.830954 vision_datasets-1.0.2/vision_datasets/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/commands/check_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/commands/converter_od_to_ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/commands/converter_to_aml_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/commands/converter_to_tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/commands/converter_tsv_to_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/commands/download_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/commands/list_operations_by_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/commands/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.834955 vision_datasets-1.0.2/vision_datasets/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.834955 vision_datasets-1.0.2/vision_datasets/common/data_manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_manifest/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_manifest/data_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_manifest/iris_data_manifest_adaptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.838955 vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/balanced_instance_weights_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/generate_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/remove_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_manifest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.838955 vision_datasets-1.0.2/vision_datasets/common/data_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_reader/dataset_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_reader/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/data_reader/image_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.842955 vision_datasets-1.0.2/vision_datasets/common/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/dataset/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/dataset/torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/dataset/vision_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/dataset_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.842955 vision_datasets-1.0.2/vision_datasets/common/dataset_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/dataset_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/dataset_management/dataset_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/dataset_management/dataset_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.842955 vision_datasets-1.0.2/vision_datasets/common/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/factory/coco_manifest_adaptor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/factory/data_manifest_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.846955 vision_datasets-1.0.2/vision_datasets/common/factory/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/factory/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/factory/operations/balanced_instance_weights_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/factory/operations/coco_generator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/factory/operations/manifest_merger_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/factory/operations/sampler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/factory/operations/spawn_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/factory/operations/split_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/factory/operations/supported_operations_by_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.846955 vision_datasets-1.0.2/vision_datasets/image_caption/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_caption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_caption/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_caption/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_caption/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.850955 vision_datasets-1.0.2/vision_datasets/image_classification/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_classification/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_classification/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_classification/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.850955 vision_datasets-1.0.2/vision_datasets/image_matting/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_matting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_matting/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_matting/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_matting/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.850955 vision_datasets-1.0.2/vision_datasets/image_object_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_object_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_object_detection/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_object_detection/detection_as_classification_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_object_detection/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_object_detection/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.854955 vision_datasets-1.0.2/vision_datasets/image_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_regression/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_regression/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_regression/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.854955 vision_datasets-1.0.2/vision_datasets/image_text_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_text_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_text_matching/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_text_matching/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_text_matching/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/image_text_matching/vision_as_image_text_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.854955 vision_datasets-1.0.2/vision_datasets/multi_task/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/multi_task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/multi_task/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/multi_task/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.858955 vision_datasets-1.0.2/vision_datasets/text_2_image_retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/text_2_image_retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/text_2_image_retrieval/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/text_2_image_retrieval/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-12 21:52:55.000000 vision_datasets-1.0.2/vision_datasets/text_2_image_retrieval/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:53:05.830954 vision_datasets-1.0.2/vision_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-07-12 21:53:05.000000 vision_datasets-1.0.2/vision_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-12 21:53:05.000000 vision_datasets-1.0.2/vision_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:53:05.000000 vision_datasets-1.0.2/vision_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-12 21:53:05.000000 vision_datasets-1.0.2/vision_datasets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-12 21:53:05.000000 vision_datasets-1.0.2/vision_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 21:53:05.000000 vision_datasets-1.0.2/vision_datasets.egg-info/top_level.txt
```

### Comparing `vision_datasets-1.0.1/LICENSE` & `vision_datasets-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/PKG-INFO` & `vision_datasets-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision_datasets
-Version: 1.0.1
+Version: 1.0.2
 Summary: A utility repo for vision dataset access and management.
 Home-page: https://github.com/microsoft/vision-datasets
 Author: Ping Jin, Shohei Ono
 License: MIT
 Keywords: vision datasets classification detection
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `vision_datasets-1.0.1/README.md` & `vision_datasets-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/setup.py` & `vision_datasets-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 from os import path
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 
 # Get the long description from the README file
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(name='vision_datasets',
```

### Comparing `vision_datasets-1.0.1/tests/resources/util.py` & `vision_datasets-1.0.2/tests/resources/util.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_box_alteration.py` & `vision_datasets-1.0.2/tests/test_box_alteration.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_coco_adaptor/coco_adaptor_base.py` & `vision_datasets-1.0.2/tests/test_coco_adaptor/coco_adaptor_base.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_caption_coco_manifest_adaptor.py` & `vision_datasets-1.0.2/tests/test_coco_adaptor/test_image_caption_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_matting_coco_manifest_adaptor.py` & `vision_datasets-1.0.2/tests/test_coco_adaptor/test_image_matting_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_regression_coco_manifest_adaptor.py` & `vision_datasets-1.0.2/tests/test_coco_adaptor/test_image_regression_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_text_matching_coco_manifest_adaptor.py` & `vision_datasets-1.0.2/tests/test_coco_adaptor/test_image_text_matching_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_coco_adaptor/test_multiclass_classification_coco_manifest_adaptor.py` & `vision_datasets-1.0.2/tests/test_coco_adaptor/test_multiclass_classification_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_coco_adaptor/test_multilabel_classification_coco_manifest_adaptor.py` & `vision_datasets-1.0.2/tests/test_coco_adaptor/test_multilabel_classification_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_coco_adaptor/test_object_detection_coco_manifest_adaptor.py` & `vision_datasets-1.0.2/tests/test_coco_adaptor/test_object_detection_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_coco_adaptor/test_text_2_image_retrieval_coco_manifest_adaptor.py` & `vision_datasets-1.0.2/tests/test_coco_adaptor/test_text_2_image_retrieval_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_coco_format_manifest.py` & `vision_datasets-1.0.2/tests/test_coco_format_manifest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_dataset_downloader.py` & `vision_datasets-1.0.2/tests/test_dataset_downloader.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_dataset_manifest.py` & `vision_datasets-1.0.2/tests/test_dataset_manifest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_dataset_registry.py` & `vision_datasets-1.0.2/tests/test_dataset_registry.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_detection_as_classification.py` & `vision_datasets-1.0.2/tests/test_detection_as_classification.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_file_reader.py` & `vision_datasets-1.0.2/tests/test_file_reader.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_fixtures.py` & `vision_datasets-1.0.2/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_ic_od_as_image_text_dataset.py` & `vision_datasets-1.0.2/tests/test_ic_od_as_image_text_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_iris_format_manifest.py` & `vision_datasets-1.0.2/tests/test_iris_format_manifest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_manifest/test_pickleable.py` & `vision_datasets-1.0.2/tests/test_manifest/test_pickleable.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_manifest_dataset.py` & `vision_datasets-1.0.2/tests/test_manifest_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_manifest_to_coco/test_manifest_to_coco.py` & `vision_datasets-1.0.2/tests/test_manifest_to_coco/test_manifest_to_coco.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_merge_manifest/test_manifest_merge.py` & `vision_datasets-1.0.2/tests/test_merge_manifest/test_manifest_merge.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_sample/test_sample_manfiest.py` & `vision_datasets-1.0.2/tests/test_sample/test_sample_manfiest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_spawn/test_spawn.py` & `vision_datasets-1.0.2/tests/test_spawn/test_spawn.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_torch_dataest/test_torch_dataset.py` & `vision_datasets-1.0.2/tests/test_torch_dataest/test_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/tests/test_utils.py` & `vision_datasets-1.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/__init__.py` & `vision_datasets-1.0.2/vision_datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/commands/check_dataset.py` & `vision_datasets-1.0.2/vision_datasets/commands/check_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/commands/converter_od_to_ic.py` & `vision_datasets-1.0.2/vision_datasets/commands/converter_od_to_ic.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/commands/converter_to_aml_coco.py` & `vision_datasets-1.0.2/vision_datasets/commands/converter_to_aml_coco.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/commands/converter_to_tsv.py` & `vision_datasets-1.0.2/vision_datasets/commands/converter_to_tsv.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/commands/converter_tsv_to_coco.py` & `vision_datasets-1.0.2/vision_datasets/commands/converter_tsv_to_coco.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/commands/download_dataset.py` & `vision_datasets-1.0.2/vision_datasets/commands/download_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/commands/list_operations_by_data_type.py` & `vision_datasets-1.0.2/vision_datasets/commands/list_operations_by_data_type.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/commands/utils.py` & `vision_datasets-1.0.2/vision_datasets/commands/utils.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/__init__.py` & `vision_datasets-1.0.2/vision_datasets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/constants.py` & `vision_datasets-1.0.2/vision_datasets/common/constants.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_manifest/__init__.py` & `vision_datasets-1.0.2/vision_datasets/common/data_manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_manifest/coco_manifest_adaptor.py` & `vision_datasets-1.0.2/vision_datasets/common/data_manifest/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_manifest/data_manifest.py` & `vision_datasets-1.0.2/vision_datasets/common/data_manifest/data_manifest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_manifest/iris_data_manifest_adaptor.py` & `vision_datasets-1.0.2/vision_datasets/common/data_manifest/iris_data_manifest_adaptor.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,30 @@
     [c_id, left, top, right, bottom], ...] (absolute coordinates);
     """
 
     @property
     def category_id(self):
         return self.label_data[0]
 
+    @property
+    def left(self):
+        return self.label_data[1]
+
+    @property
+    def top(self):
+        return self.label_data[2]
+
+    @property
+    def right(self):
+        return self.label_data[3]
+
+    @property
+    def bottom(self):
+        return self.label_data[4]
+
     @category_id.setter
     def category_id(self, value):
         self._category_id_check(value)
         self.label_data[0] = value
 
     def _read_label_data(self):
         raise NotImplementedError
```

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/__init__.py` & `vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/balanced_instance_weights_generator.py` & `vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/balanced_instance_weights_generator.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/filter.py` & `vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/filter.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/generate_coco.py` & `vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/generate_coco.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/merge.py` & `vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/merge.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/remove_categories.py` & `vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/remove_categories.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/sample.py` & `vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/sample.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/spawn.py` & `vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/spawn.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/split.py` & `vision_datasets-1.0.2/vision_datasets/common/data_manifest/operations/split.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_manifest/utils.py` & `vision_datasets-1.0.2/vision_datasets/common/data_manifest/utils.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_reader/dataset_downloader.py` & `vision_datasets-1.0.2/vision_datasets/common/data_reader/dataset_downloader.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_reader/file_reader.py` & `vision_datasets-1.0.2/vision_datasets/common/data_reader/file_reader.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/data_reader/image_loader.py` & `vision_datasets-1.0.2/vision_datasets/common/data_reader/image_loader.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/dataset/base_dataset.py` & `vision_datasets-1.0.2/vision_datasets/common/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/dataset/dataset.py` & `vision_datasets-1.0.2/vision_datasets/common/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/dataset/torch_dataset.py` & `vision_datasets-1.0.2/vision_datasets/common/dataset/torch_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/dataset/vision_dataset.py` & `vision_datasets-1.0.2/vision_datasets/common/dataset/vision_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/dataset_info.py` & `vision_datasets-1.0.2/vision_datasets/common/dataset_info.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/dataset_management/dataset_hub.py` & `vision_datasets-1.0.2/vision_datasets/common/dataset_management/dataset_hub.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/dataset_management/dataset_registry.py` & `vision_datasets-1.0.2/vision_datasets/common/dataset_management/dataset_registry.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/factory/__init__.py` & `vision_datasets-1.0.2/vision_datasets/common/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/factory/data_manifest_factory.py` & `vision_datasets-1.0.2/vision_datasets/common/factory/data_manifest_factory.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/factory/operations/__init__.py` & `vision_datasets-1.0.2/vision_datasets/common/factory/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/factory/operations/balanced_instance_weights_factory.py` & `vision_datasets-1.0.2/vision_datasets/common/factory/operations/balanced_instance_weights_factory.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/factory/operations/coco_generator_factory.py` & `vision_datasets-1.0.2/vision_datasets/common/factory/operations/coco_generator_factory.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/factory/operations/manifest_merger_factory.py` & `vision_datasets-1.0.2/vision_datasets/common/factory/operations/manifest_merger_factory.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/factory/operations/sampler_factory.py` & `vision_datasets-1.0.2/vision_datasets/common/factory/operations/sampler_factory.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/factory/operations/spawn_factory.py` & `vision_datasets-1.0.2/vision_datasets/common/factory/operations/spawn_factory.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/factory/operations/split_factory.py` & `vision_datasets-1.0.2/vision_datasets/common/factory/operations/split_factory.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/common/utils.py` & `vision_datasets-1.0.2/vision_datasets/common/utils.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_caption/coco_manifest_adaptor.py` & `vision_datasets-1.0.2/vision_datasets/image_caption/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_caption/operations.py` & `vision_datasets-1.0.2/vision_datasets/image_caption/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_classification/coco_manifest_adaptor.py` & `vision_datasets-1.0.2/vision_datasets/image_classification/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_classification/manifest.py` & `vision_datasets-1.0.2/vision_datasets/image_classification/manifest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_classification/operations.py` & `vision_datasets-1.0.2/vision_datasets/image_classification/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_matting/coco_manifest_adaptor.py` & `vision_datasets-1.0.2/vision_datasets/image_matting/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_matting/manifest.py` & `vision_datasets-1.0.2/vision_datasets/image_matting/manifest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_matting/operations.py` & `vision_datasets-1.0.2/vision_datasets/image_matting/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_object_detection/__init__.py` & `vision_datasets-1.0.2/vision_datasets/image_object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_object_detection/coco_manifest_adaptor.py` & `vision_datasets-1.0.2/vision_datasets/image_object_detection/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_object_detection/detection_as_classification_dataset.py` & `vision_datasets-1.0.2/vision_datasets/image_object_detection/detection_as_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_object_detection/manifest.py` & `vision_datasets-1.0.2/vision_datasets/image_object_detection/manifest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_object_detection/operations.py` & `vision_datasets-1.0.2/vision_datasets/image_object_detection/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_regression/coco_manifest_adaptor.py` & `vision_datasets-1.0.2/vision_datasets/image_regression/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_regression/operations.py` & `vision_datasets-1.0.2/vision_datasets/image_regression/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_text_matching/coco_manifest_adaptor.py` & `vision_datasets-1.0.2/vision_datasets/image_text_matching/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_text_matching/operations.py` & `vision_datasets-1.0.2/vision_datasets/image_text_matching/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/image_text_matching/vision_as_image_text_dataset.py` & `vision_datasets-1.0.2/vision_datasets/image_text_matching/vision_as_image_text_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/multi_task/coco_manifest_adaptor.py` & `vision_datasets-1.0.2/vision_datasets/multi_task/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/multi_task/operations.py` & `vision_datasets-1.0.2/vision_datasets/multi_task/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/text_2_image_retrieval/coco_manifest_adaptor.py` & `vision_datasets-1.0.2/vision_datasets/text_2_image_retrieval/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets/text_2_image_retrieval/operations.py` & `vision_datasets-1.0.2/vision_datasets/text_2_image_retrieval/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.1/vision_datasets.egg-info/PKG-INFO` & `vision_datasets-1.0.2/vision_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-datasets
-Version: 1.0.1
+Version: 1.0.2
 Summary: A utility repo for vision dataset access and management.
 Home-page: https://github.com/microsoft/vision-datasets
 Author: Ping Jin, Shohei Ono
 License: MIT
 Keywords: vision datasets classification detection
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `vision_datasets-1.0.1/vision_datasets.egg-info/SOURCES.txt` & `vision_datasets-1.0.2/vision_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*


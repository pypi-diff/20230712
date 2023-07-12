# Comparing `tmp/refuel-autolabel-0.0.7.tar.gz` & `tmp/refuel-autolabel-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refuel-autolabel-0.0.7.tar", last modified: Mon Jul  3 03:33:57 2023, max compression
+gzip compressed data, was "refuel-autolabel-0.0.8.tar", last modified: Wed Jul 12 00:34:35 2023, max compression
```

## Comparing `refuel-autolabel-0.0.7.tar` & `refuel-autolabel-0.0.8.tar`

### file list

```diff
@@ -1,63 +1,67 @@
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.294360 refuel-autolabel-0.0.7/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1066 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/LICENSE
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    10384 2023-07-03 03:33:57.294155 refuel-autolabel-0.0.7/PKG-INFO
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8337 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/README.md
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2303 2023-07-03 03:32:59.000000 refuel-autolabel-0.0.7/pyproject.toml
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       38 2023-07-03 03:33:57.294419 refuel-autolabel-0.0.7/setup.cfg
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.280809 refuel-autolabel-0.0.7/src/
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.284286 refuel-autolabel-0.0.7/src/autolabel/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       63 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.7/src/autolabel/__init__.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.285054 refuel-autolabel-0.0.7/src/autolabel/cache/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       74 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/cache/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      924 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.7/src/autolabel/cache/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1817 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.7/src/autolabel/cache/sqlalchemy_cache.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9137 2023-06-15 00:37:32.000000 refuel-autolabel-0.0.7/src/autolabel/confidence.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.286283 refuel-autolabel-0.0.7/src/autolabel/configs/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       65 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/configs/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1401 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/configs/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7569 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/configs/config.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4114 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/configs/schema.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.287918 refuel-autolabel-0.0.7/src/autolabel/data_models/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      195 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/data_models/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2001 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.7/src/autolabel/data_models/annotation.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       71 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/data_models/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2036 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.7/src/autolabel/data_models/cache.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1071 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/data_models/dataset.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      928 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/data_models/task.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2625 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.7/src/autolabel/data_models/task_run.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.288496 refuel-autolabel-0.0.7/src/autolabel/database/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       77 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/database/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      643 2023-07-03 02:09:47.000000 refuel-autolabel-0.0.7/src/autolabel/database/engine.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2788 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.7/src/autolabel/database/state_manager.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8085 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/dataset_loader.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.289063 refuel-autolabel-0.0.7/src/autolabel/few_shot/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3233 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/few_shot/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1295 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/few_shot/fixed_example_selector.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11031 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.7/src/autolabel/few_shot/vector_store.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    19705 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/labeler.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.291076 refuel-autolabel-0.0.7/src/autolabel/models/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2107 2023-07-03 02:09:47.000000 refuel-autolabel-0.0.7/src/autolabel/models/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2496 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/models/anthropic.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4150 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/models/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1959 2023-07-03 02:09:47.000000 refuel-autolabel-0.0.7/src/autolabel/models/cohere.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3132 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/models/hf_pipeline.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     5682 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/models/openai.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3920 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.7/src/autolabel/models/palm.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3575 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.7/src/autolabel/models/refuel.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4707 2023-07-03 02:09:47.000000 refuel-autolabel-0.0.7/src/autolabel/schema.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.293133 refuel-autolabel-0.0.7/src/autolabel/tasks/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1298 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4319 2023-06-22 05:07:53.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7409 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/classification.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7419 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/entity_matching.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8221 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/multilabel_classification.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    12627 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/named_entity_recognition.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7508 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/question_answering.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1574 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/utils.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9773 2023-06-22 21:40:05.000000 refuel-autolabel-0.0.7/src/autolabel/utils.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.293951 refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    10384 2023-07-03 03:33:57.000000 refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/PKG-INFO
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1683 2023-07-03 03:33:57.000000 refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)        1 2023-07-03 03:33:57.000000 refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      903 2023-07-03 03:33:57.000000 refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/requires.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       10 2023-07-03 03:33:57.000000 refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/top_level.txt
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-07-12 00:34:35.406330 refuel-autolabel-0.0.8/
+-rw-r--r--   0 nihit      (501) staff       (20)     1066 2023-05-11 06:24:46.000000 refuel-autolabel-0.0.8/LICENSE
+-rw-r--r--   0 nihit      (501) staff       (20)    10381 2023-07-12 00:34:35.406104 refuel-autolabel-0.0.8/PKG-INFO
+-rw-r--r--   0 nihit      (501) staff       (20)     8334 2023-07-06 04:47:37.000000 refuel-autolabel-0.0.8/README.md
+-rw-r--r--   0 nihit      (501) staff       (20)     2328 2023-07-12 00:34:26.000000 refuel-autolabel-0.0.8/pyproject.toml
+-rw-r--r--   0 nihit      (501) staff       (20)       38 2023-07-12 00:34:35.406390 refuel-autolabel-0.0.8/setup.cfg
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-07-12 00:34:35.393523 refuel-autolabel-0.0.8/src/
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-07-12 00:34:35.396443 refuel-autolabel-0.0.8/src/autolabel/
+-rw-r--r--   0 nihit      (501) staff       (20)      263 2023-07-12 00:34:26.000000 refuel-autolabel-0.0.8/src/autolabel/__init__.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-07-12 00:34:35.397229 refuel-autolabel-0.0.8/src/autolabel/cache/
+-rw-r--r--   0 nihit      (501) staff       (20)       74 2023-05-16 00:22:56.000000 refuel-autolabel-0.0.8/src/autolabel/cache/__init__.py
+-rw-r--r--   0 nihit      (501) staff       (20)      924 2023-06-08 20:27:49.000000 refuel-autolabel-0.0.8/src/autolabel/cache/base.py
+-rw-r--r--   0 nihit      (501) staff       (20)     1817 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.8/src/autolabel/cache/sqlalchemy_cache.py
+-rw-r--r--   0 nihit      (501) staff       (20)     9137 2023-06-15 00:40:46.000000 refuel-autolabel-0.0.8/src/autolabel/confidence.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-07-12 00:34:35.398191 refuel-autolabel-0.0.8/src/autolabel/configs/
+-rw-r--r--   0 nihit      (501) staff       (20)       65 2023-05-29 00:22:31.000000 refuel-autolabel-0.0.8/src/autolabel/configs/__init__.py
+-rw-r--r--   0 nihit      (501) staff       (20)     1401 2023-06-26 23:56:08.000000 refuel-autolabel-0.0.8/src/autolabel/configs/base.py
+-rw-r--r--   0 nihit      (501) staff       (20)     7569 2023-07-06 04:47:37.000000 refuel-autolabel-0.0.8/src/autolabel/configs/config.py
+-rw-r--r--   0 nihit      (501) staff       (20)     4171 2023-07-11 21:30:59.000000 refuel-autolabel-0.0.8/src/autolabel/configs/schema.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-07-12 00:34:35.398862 refuel-autolabel-0.0.8/src/autolabel/data_loaders/
+-rw-r--r--   0 nihit      (501) staff       (20)     4248 2023-07-11 21:30:59.000000 refuel-autolabel-0.0.8/src/autolabel/data_loaders/__init__.py
+-rw-r--r--   0 nihit      (501) staff       (20)     7011 2023-07-10 22:40:36.000000 refuel-autolabel-0.0.8/src/autolabel/data_loaders/read_datasets.py
+-rw-r--r--   0 nihit      (501) staff       (20)     8498 2023-07-11 19:29:59.000000 refuel-autolabel-0.0.8/src/autolabel/data_loaders/validation.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-07-12 00:34:35.400368 refuel-autolabel-0.0.8/src/autolabel/data_models/
+-rw-r--r--   0 nihit      (501) staff       (20)      195 2023-05-16 00:22:56.000000 refuel-autolabel-0.0.8/src/autolabel/data_models/__init__.py
+-rw-r--r--   0 nihit      (501) staff       (20)     2001 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.8/src/autolabel/data_models/annotation.py
+-rw-r--r--   0 nihit      (501) staff       (20)       71 2023-05-14 02:11:15.000000 refuel-autolabel-0.0.8/src/autolabel/data_models/base.py
+-rw-r--r--   0 nihit      (501) staff       (20)     2036 2023-06-10 22:44:42.000000 refuel-autolabel-0.0.8/src/autolabel/data_models/cache.py
+-rw-r--r--   0 nihit      (501) staff       (20)     1071 2023-05-14 02:11:15.000000 refuel-autolabel-0.0.8/src/autolabel/data_models/dataset.py
+-rw-r--r--   0 nihit      (501) staff       (20)      928 2023-05-14 02:11:15.000000 refuel-autolabel-0.0.8/src/autolabel/data_models/task.py
+-rw-r--r--   0 nihit      (501) staff       (20)     2625 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.8/src/autolabel/data_models/task_run.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-07-12 00:34:35.400924 refuel-autolabel-0.0.8/src/autolabel/database/
+-rw-r--r--   0 nihit      (501) staff       (20)       77 2023-05-14 02:11:15.000000 refuel-autolabel-0.0.8/src/autolabel/database/__init__.py
+-rw-r--r--   0 nihit      (501) staff       (20)      643 2023-07-06 04:47:37.000000 refuel-autolabel-0.0.8/src/autolabel/database/engine.py
+-rw-r--r--   0 nihit      (501) staff       (20)     2788 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.8/src/autolabel/database/state_manager.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-07-12 00:34:35.401804 refuel-autolabel-0.0.8/src/autolabel/few_shot/
+-rw-r--r--   0 nihit      (501) staff       (20)     3928 2023-07-07 22:34:09.000000 refuel-autolabel-0.0.8/src/autolabel/few_shot/__init__.py
+-rw-r--r--   0 nihit      (501) staff       (20)     1295 2023-05-14 02:11:15.000000 refuel-autolabel-0.0.8/src/autolabel/few_shot/fixed_example_selector.py
+-rw-r--r--   0 nihit      (501) staff       (20)     6328 2023-07-07 22:34:09.000000 refuel-autolabel-0.0.8/src/autolabel/few_shot/label_diversity_example_selector.py
+-rw-r--r--   0 nihit      (501) staff       (20)    14119 2023-07-07 22:34:09.000000 refuel-autolabel-0.0.8/src/autolabel/few_shot/vector_store.py
+-rw-r--r--   0 nihit      (501) staff       (20)    19712 2023-07-11 19:29:59.000000 refuel-autolabel-0.0.8/src/autolabel/labeler.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-07-12 00:34:35.403329 refuel-autolabel-0.0.8/src/autolabel/models/
+-rw-r--r--   0 nihit      (501) staff       (20)     2107 2023-07-06 04:47:37.000000 refuel-autolabel-0.0.8/src/autolabel/models/__init__.py
+-rw-r--r--   0 nihit      (501) staff       (20)     2395 2023-07-11 21:30:59.000000 refuel-autolabel-0.0.8/src/autolabel/models/anthropic.py
+-rw-r--r--   0 nihit      (501) staff       (20)     4902 2023-07-11 21:30:59.000000 refuel-autolabel-0.0.8/src/autolabel/models/base.py
+-rw-r--r--   0 nihit      (501) staff       (20)     1902 2023-07-11 21:30:59.000000 refuel-autolabel-0.0.8/src/autolabel/models/cohere.py
+-rw-r--r--   0 nihit      (501) staff       (20)     3063 2023-07-11 21:30:59.000000 refuel-autolabel-0.0.8/src/autolabel/models/hf_pipeline.py
+-rw-r--r--   0 nihit      (501) staff       (20)     6063 2023-07-11 21:30:59.000000 refuel-autolabel-0.0.8/src/autolabel/models/openai.py
+-rw-r--r--   0 nihit      (501) staff       (20)     4840 2023-07-11 21:30:59.000000 refuel-autolabel-0.0.8/src/autolabel/models/palm.py
+-rw-r--r--   0 nihit      (501) staff       (20)     3575 2023-06-20 23:17:06.000000 refuel-autolabel-0.0.8/src/autolabel/models/refuel.py
+-rw-r--r--   0 nihit      (501) staff       (20)     4823 2023-07-07 22:34:09.000000 refuel-autolabel-0.0.8/src/autolabel/schema.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-07-12 00:34:35.405145 refuel-autolabel-0.0.8/src/autolabel/tasks/
+-rw-r--r--   0 nihit      (501) staff       (20)     1298 2023-07-06 04:47:37.000000 refuel-autolabel-0.0.8/src/autolabel/tasks/__init__.py
+-rw-r--r--   0 nihit      (501) staff       (20)     4319 2023-06-20 23:17:06.000000 refuel-autolabel-0.0.8/src/autolabel/tasks/base.py
+-rw-r--r--   0 nihit      (501) staff       (20)     7409 2023-06-19 23:05:19.000000 refuel-autolabel-0.0.8/src/autolabel/tasks/classification.py
+-rw-r--r--   0 nihit      (501) staff       (20)     7419 2023-06-19 23:05:19.000000 refuel-autolabel-0.0.8/src/autolabel/tasks/entity_matching.py
+-rw-r--r--   0 nihit      (501) staff       (20)     8221 2023-07-06 04:47:37.000000 refuel-autolabel-0.0.8/src/autolabel/tasks/multilabel_classification.py
+-rw-r--r--   0 nihit      (501) staff       (20)    12627 2023-06-19 23:05:19.000000 refuel-autolabel-0.0.8/src/autolabel/tasks/named_entity_recognition.py
+-rw-r--r--   0 nihit      (501) staff       (20)     7508 2023-06-19 23:05:19.000000 refuel-autolabel-0.0.8/src/autolabel/tasks/question_answering.py
+-rw-r--r--   0 nihit      (501) staff       (20)     1574 2023-06-08 20:27:49.000000 refuel-autolabel-0.0.8/src/autolabel/tasks/utils.py
+-rw-r--r--   0 nihit      (501) staff       (20)     9773 2023-06-22 21:37:13.000000 refuel-autolabel-0.0.8/src/autolabel/utils.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-07-12 00:34:35.405900 refuel-autolabel-0.0.8/src/refuel_autolabel.egg-info/
+-rw-r--r--   0 nihit      (501) staff       (20)    10381 2023-07-12 00:34:35.000000 refuel-autolabel-0.0.8/src/refuel_autolabel.egg-info/PKG-INFO
+-rw-r--r--   0 nihit      (501) staff       (20)     1834 2023-07-12 00:34:35.000000 refuel-autolabel-0.0.8/src/refuel_autolabel.egg-info/SOURCES.txt
+-rw-r--r--   0 nihit      (501) staff       (20)        1 2023-07-12 00:34:35.000000 refuel-autolabel-0.0.8/src/refuel_autolabel.egg-info/dependency_links.txt
+-rw-r--r--   0 nihit      (501) staff       (20)      919 2023-07-12 00:34:35.000000 refuel-autolabel-0.0.8/src/refuel_autolabel.egg-info/requires.txt
+-rw-r--r--   0 nihit      (501) staff       (20)       10 2023-07-12 00:34:35.000000 refuel-autolabel-0.0.8/src/refuel_autolabel.egg-info/top_level.txt
```

### Comparing `refuel-autolabel-0.0.7/LICENSE` & `refuel-autolabel-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/PKG-INFO` & `refuel-autolabel-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refuel-autolabel
-Version: 0.0.7
+Version: 0.0.8
 Summary: Label, clean and enrich text datasets with LLMs
 Author-email: "Refuel.ai" <support@refuel.ai>
 License: MIT License
         
         Copyright (c) 2023 refuel-ai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,15 +41,14 @@
 Provides-Extra: google
 Provides-Extra: cohere
 Provides-Extra: all
 License-File: LICENSE
 
 <img alt="Refuel logo" src="https://raw.githubusercontent.com/refuel-ai/autolabel/main/docs/assets/Autolabel_blk_w_background.png">
 
-
 <h4 align="center">
   <a href="https://discord.gg/fweVnRx6CU">Discord</a> |
   <a href="https://twitter.com/RefuelAI">Twitter</a> |
   <a href="https://www.refuel.ai/">Website</a> |
   <a href="https://www.refuel.ai/blog-posts/llm-labeling-technical-report">Benchmark</a>
 </h4>
 
@@ -95,15 +94,15 @@
         "delimiter": ","
     },
     "prompt": {
         "task_guidelines": "You are an expert at analyzing the sentiment of movie reviews. Your job is to classify the provided movie review into one of the following labels: {labels}",
         "labels": [
             "positive",
             "negative",
-            "neutral",
+            "neutral"
         ],
         "few_shot_examples": [
             {
                 "example": "I got a fairly uninspired stupid film about how human industry is bad for nature.",
                 "label": "negative"
             },
             {
@@ -208,15 +207,14 @@
 
 ## 🛠️ Roadmap
 
 Check out our [public roadmap](https://github.com/orgs/refuel-ai/projects/15) to learn more about ongoing and planned improvements to the Autolabel library.
 
 We are always looking for suggestions and contributions from the community. Join the discussion on [Discord](https://discord.gg/fweVnRx6CU) or open a [Github issue](https://github.com/refuel-ai/autolabel/issues) to report bugs and request features.
 
-
 ## 🙌 Contributing
 
 Autolabel is a rapidly developing project. We welcome contributions in all forms - bug reports, pull requests and ideas for improving the library.
 
 1. Join the conversation on [Discord](https://discord.gg/fweVnRx6CU)
 2. Open an [issue](https://github.com/refuel-ai/autolabel/issues) on Github for bugs and request features.
 3. Grab an open issue, and submit a [pull request](https://github.com/refuel-ai/autolabel/blob/main/CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.7 Summary: Label,
+Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.8 Summary: Label,
 clean and enrich text datasets with LLMs Author-email: "Refuel.ai"
 refuel.ai> License: MIT License Copyright (c) 2023 refuel-ai Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -49,15 +49,15 @@
 sentiment analysis of movie review. We have a dataset of movie reviews that
 we'd like to get labeled first. For this case, here's what the example dataset
 and configs will look like: ```python { "task_name": "MovieSentimentReview",
 "task_type": "classification", "model": { "provider": "openai", "name": "gpt-
 3.5-turbo" }, "dataset": { "label_column": "label", "delimiter": "," },
 "prompt": { "task_guidelines": "You are an expert at analyzing the sentiment of
 movie reviews. Your job is to classify the provided movie review into one of
-the following labels: {labels}", "labels": [ "positive", "negative", "neutral",
+the following labels: {labels}", "labels": [ "positive", "negative", "neutral"
 ], "few_shot_examples": [ { "example": "I got a fairly uninspired stupid film
 about how human industry is bad for nature.", "label": "negative" },
 { "example": "I loved this movie. I found it very heart warming to see Adam
 West, Burt Ward, Frank Gorshin, and Julie Newmar together again.", "label":
 "positive" }, { "example": "This movie will be played next week at the Chinese
 theater.", "label": "neutral" } ], "example_template": "Input:
 {example}\nOutput: {label}" } } ``` Initialize the labeling agent and pass it
```

### Comparing `refuel-autolabel-0.0.7/README.md` & `refuel-autolabel-0.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 <img alt="Refuel logo" src="https://raw.githubusercontent.com/refuel-ai/autolabel/main/docs/assets/Autolabel_blk_w_background.png">
 
-
 <h4 align="center">
   <a href="https://discord.gg/fweVnRx6CU">Discord</a> |
   <a href="https://twitter.com/RefuelAI">Twitter</a> |
   <a href="https://www.refuel.ai/">Website</a> |
   <a href="https://www.refuel.ai/blog-posts/llm-labeling-technical-report">Benchmark</a>
 </h4>
 
@@ -50,15 +49,15 @@
         "delimiter": ","
     },
     "prompt": {
         "task_guidelines": "You are an expert at analyzing the sentiment of movie reviews. Your job is to classify the provided movie review into one of the following labels: {labels}",
         "labels": [
             "positive",
             "negative",
-            "neutral",
+            "neutral"
         ],
         "few_shot_examples": [
             {
                 "example": "I got a fairly uninspired stupid film about how human industry is bad for nature.",
                 "label": "negative"
             },
             {
@@ -163,15 +162,14 @@
 
 ## 🛠️ Roadmap
 
 Check out our [public roadmap](https://github.com/orgs/refuel-ai/projects/15) to learn more about ongoing and planned improvements to the Autolabel library.
 
 We are always looking for suggestions and contributions from the community. Join the discussion on [Discord](https://discord.gg/fweVnRx6CU) or open a [Github issue](https://github.com/refuel-ai/autolabel/issues) to report bugs and request features.
 
-
 ## 🙌 Contributing
 
 Autolabel is a rapidly developing project. We welcome contributions in all forms - bug reports, pull requests and ideas for improving the library.
 
 1. Join the conversation on [Discord](https://discord.gg/fweVnRx6CU)
 2. Open an [issue](https://github.com/refuel-ai/autolabel/issues) on Github for bugs and request features.
 3. Grab an open issue, and submit a [pull request](https://github.com/refuel-ai/autolabel/blob/main/CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -25,15 +25,15 @@
 sentiment analysis of movie review. We have a dataset of movie reviews that
 we'd like to get labeled first. For this case, here's what the example dataset
 and configs will look like: ```python { "task_name": "MovieSentimentReview",
 "task_type": "classification", "model": { "provider": "openai", "name": "gpt-
 3.5-turbo" }, "dataset": { "label_column": "label", "delimiter": "," },
 "prompt": { "task_guidelines": "You are an expert at analyzing the sentiment of
 movie reviews. Your job is to classify the provided movie review into one of
-the following labels: {labels}", "labels": [ "positive", "negative", "neutral",
+the following labels: {labels}", "labels": [ "positive", "negative", "neutral"
 ], "few_shot_examples": [ { "example": "I got a fairly uninspired stupid film
 about how human industry is bad for nature.", "label": "negative" },
 { "example": "I loved this movie. I found it very heart warming to see Adam
 West, Burt Ward, Frank Gorshin, and Julie Newmar together again.", "label":
 "positive" }, { "example": "This movie will be played next week at the Chinese
 theater.", "label": "neutral" } ], "example_template": "Input:
 {example}\nOutput: {label}" } } ``` Initialize the labeling agent and pass it
```

### Comparing `refuel-autolabel-0.0.7/pyproject.toml` & `refuel-autolabel-0.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0.0", "wheel >= 0.38"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "refuel-autolabel"
-version = "0.0.7"
+version = "0.0.8"
 description = "Label, clean and enrich text datasets with LLMs"
 readme = "README.md"
 authors = [{ name = "Refuel.ai", email = "support@refuel.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
@@ -32,15 +32,16 @@
     "rich >= 13.3.5",
     "scipy >= 1.10.1",
     "pydantic >= 1.10.9",
     "torch >= 1.10.0",
     "matplotlib >= 3.5.0",
     "wget >= 3.2",
     "ipywidgets == 8.0.6",
-    "jsonschema >= 4.17.3"
+    "jsonschema >= 4.17.3",
+    "tabulate >= 0.9.0"
 ]
 requires-python = ">=3.6"
 
 [project.optional-dependencies]
 dev = [
     "black",
     "bumpver",
```

### Comparing `refuel-autolabel-0.0.7/src/autolabel/cache/base.py` & `refuel-autolabel-0.0.8/src/autolabel/cache/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/cache/sqlalchemy_cache.py` & `refuel-autolabel-0.0.8/src/autolabel/cache/sqlalchemy_cache.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/confidence.py` & `refuel-autolabel-0.0.8/src/autolabel/confidence.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/configs/base.py` & `refuel-autolabel-0.0.8/src/autolabel/configs/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/configs/config.py` & `refuel-autolabel-0.0.8/src/autolabel/configs/config.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/configs/schema.py` & `refuel-autolabel-0.0.8/src/autolabel/configs/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,15 @@
                     ]
                 },
                 "few_shot_selection": {
                     "enum": populate_few_shot_selection(),
                     "type": "string",
                 },
                 "few_shot_num": {"type": "number"},
+                "chain_of_thought": {"type": "boolean"},
             },
             "required": ["task_guidelines"],
             "additionalProperties": False,
         },
     },
     "required": [
         "task_name",
```

### Comparing `refuel-autolabel-0.0.7/src/autolabel/data_models/annotation.py` & `refuel-autolabel-0.0.8/src/autolabel/data_models/annotation.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/data_models/cache.py` & `refuel-autolabel-0.0.8/src/autolabel/data_models/cache.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/data_models/dataset.py` & `refuel-autolabel-0.0.8/src/autolabel/data_models/dataset.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/data_models/task.py` & `refuel-autolabel-0.0.8/src/autolabel/data_models/task.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/data_models/task_run.py` & `refuel-autolabel-0.0.8/src/autolabel/data_models/task_run.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/database/engine.py` & `refuel-autolabel-0.0.8/src/autolabel/database/engine.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/database/state_manager.py` & `refuel-autolabel-0.0.8/src/autolabel/database/state_manager.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/dataset_loader.py` & `refuel-autolabel-0.0.8/src/autolabel/data_loaders/read_datasets.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,233 +1,223 @@
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Union
 
 import logging
 import pandas as pd
-from sqlalchemy.sql.selectable import Selectable
-from datasets import Dataset
-
 
+from pydantic import BaseModel, validator
+from datasets import Dataset
+from sqlalchemy.sql.selectable import Selectable
 from autolabel.configs import AutolabelConfig
 
 logger = logging.getLogger(__name__)
 
 
-class DatasetLoader:
-    # TODO: add support for reading from SQL databases
-    # TODO: add support for reading and loading datasets in chunks
-
-    def __init__(
-        self,
-        dataset: Union[str, pd.DataFrame],
-        config: AutolabelConfig,
-        max_items: int = 0,
-        start_index: int = 0,
-    ) -> None:
-        """DatasetLoader class to read and load datasets.
+class AutolabelDataset(BaseModel):
+    """Data Attributes"""
 
-        Args:
-            dataset (Union[str, pd.DataFrame]): path to the dataset or the dataframe
-            config (AutolabelConfig): config object
-            max_items (int, optional): max number of items to read. Defaults to 0.
-            start_index (int, optional): start index to read from. Defaults to 0.
-        """
-        self.dataset = dataset
-        self.config = config
-        self.max_items = max_items
-        self.start_index = start_index
-
-        if isinstance(dataset, str):
-            self._read_file(dataset, config, max_items, start_index)
-        elif isinstance(dataset, Dataset):
-            self._read_hf_dataset(dataset, config, max_items, start_index)
-        elif isinstance(dataset, pd.DataFrame):
-            self._read_dataframe(dataset, config, start_index, max_items)
-
-    def _read_csv(
-        self,
+    columns: List
+    dataset: Union[pd.DataFrame, None]
+    inputs: List[Dict]
+    gt_labels: List
+
+    @validator("dataset", allow_reuse=True)
+    def validate_dataframe(cls, value):
+        if not isinstance(value, pd.DataFrame):
+            raise ValueError("Value must be a pandas DataFrame")
+        return value
+
+    class Config:
+        arbitrary_types_allowed = True
+
+
+class CSVReader:
+    @staticmethod
+    def read(
         csv_file: str,
         config: AutolabelConfig,
         max_items: int = None,
         start_index: int = 0,
-    ) -> None:
+    ) -> AutolabelDataset:
         """Read the csv file and sets dat, inputs and gt_labels
 
         Args:
             csv_file (str): path to the csv file
             config (AutolabelConfig): config object
             max_items (int, optional): max number of items to read. Defaults to None.
             start_index (int, optional): start index to read from. Defaults to 0.
         """
         logger.debug(f"reading the csv from: {start_index}")
         delimiter = config.delimiter()
         label_column = config.label_column()
 
-        self.dat = pd.read_csv(csv_file, sep=delimiter, dtype="str")[start_index:]
-        self.dat = self.dat.astype(str)
+        dat = pd.read_csv(csv_file, sep=delimiter, dtype="str")[start_index:]
+
+        dat = dat.astype(str)
         if max_items and max_items > 0:
-            max_items = min(max_items, len(self.dat))
-            self.dat = self.dat[:max_items]
+            max_items = min(max_items, len(dat))
+            dat = dat[:max_items]
 
-        self.inputs = self.dat.to_dict(orient="records")
-        self.gt_labels = (
+        inputs = dat.to_dict(orient="records")
+        gt_labels = (
             None
-            if not label_column
-            or not len(self.inputs)
-            or label_column not in self.inputs[0]
-            else self.dat[label_column].tolist()
+            if not label_column or not len(inputs) or label_column not in inputs[0]
+            else dat[label_column].tolist()
+        )
+        return AutolabelDataset(
+            columns=list(dat.columns),
+            dataset=dat,
+            inputs=inputs,
+            gt_labels=gt_labels,
         )
 
-    def _read_dataframe(
-        self,
-        df: pd.DataFrame,
+
+class JsonlReader:
+    @staticmethod
+    def read(
+        jsonl_file: str,
         config: AutolabelConfig,
         max_items: int = None,
         start_index: int = 0,
-    ) -> None:
-        """Read the csv file and sets dat, inputs and gt_labels
+    ) -> AutolabelDataset:
+        """Read the jsonl file and sets dat, inputs and gt_labels
 
         Args:
-            df (pd.DataFrame): dataframe to read
+            jsonl_file (str): path to the jsonl file
             config (AutolabelConfig): config object
             max_items (int, optional): max number of items to read. Defaults to None.
             start_index (int, optional): start index to read from. Defaults to 0.
         """
+        logger.debug(f"reading the jsonl from: {start_index}")
         label_column = config.label_column()
 
-        self.dat = df[start_index:].astype(str)
+        dat = pd.read_json(jsonl_file, lines=True, dtype="str")[start_index:]
+        dat = dat.astype(str)
         if max_items and max_items > 0:
-            max_items = min(max_items, len(self.dat))
-            self.dat = self.dat[:max_items]
+            max_items = min(max_items, len(dat))
+            dat = dat[:max_items]
 
-        self.inputs = self.dat.to_dict(orient="records")
-        self.gt_labels = (
+        inputs = dat.to_dict(orient="records")
+        gt_labels = (
             None
-            if not label_column
-            or not len(self.inputs)
-            or label_column not in self.inputs[0]
-            else self.dat[label_column].tolist()
+            if not label_column or not len(inputs) or label_column not in inputs[0]
+            else dat[label_column].tolist()
+        )
+        return AutolabelDataset(
+            columns=list(dat.columns),
+            dataset=dat,
+            inputs=inputs,
+            gt_labels=gt_labels,
         )
 
-    def _read_jsonl(
-        self,
-        jsonl_file: str,
+
+class HuggingFaceDatasetReader:
+    @staticmethod
+    def read(
+        dataset: Dataset,
         config: AutolabelConfig,
         max_items: int = None,
         start_index: int = 0,
-    ) -> None:
-        """Read the jsonl file and sets dat, inputs and gt_labels
+    ) -> AutolabelDataset:
+        """Read the huggingface dataset and sets dat, inputs and gt_labels
 
         Args:
-            jsonl_file (str): path to the jsonl file
+            dataset (Dataset): dataset object to read from
             config (AutolabelConfig): config object
             max_items (int, optional): max number of items to read. Defaults to None.
             start_index (int, optional): start index to read from. Defaults to 0.
         """
-        logger.debug(f"reading the jsonl from: {start_index}")
-        label_column = config.label_column()
-
-        self.dat = pd.read_json(jsonl_file, lines=True, dtype="str")[start_index:]
-        self.dat = self.dat.astype(str)
-        if max_items and max_items > 0:
-            max_items = min(max_items, len(self.dat))
-            self.dat = self.dat[:max_items]
+        dataset.set_format("pandas")
+        dat = dataset[
+            start_index : max_items if max_items and max_items > 0 else len(dataset)
+        ]
 
-        self.inputs = self.dat.to_dict(orient="records")
-        self.gt_labels = (
+        inputs = dat.to_dict(orient="records")
+        gt_labels = (
             None
-            if not label_column
-            or not len(self.inputs)
-            or label_column not in self.inputs[0]
-            else self.dat[label_column].tolist()
+            if not config.label_column()
+            or not len(inputs)
+            or config.label_column() not in inputs[0]
+            else dat[config.label_column()].tolist()
+        )
+        return AutolabelDataset(
+            columns=list(dat.columns),
+            dataset=dat,
+            inputs=inputs,
+            gt_labels=gt_labels,
         )
 
-    def _read_sql(
-        self,
+
+class SqlDatasetReader:
+    @staticmethod
+    def read(
         sql: Union[str, Selectable],
         connection: str,
         config: AutolabelConfig,
         max_items: int = None,
         start_index: int = 0,
-    ) -> None:
+    ) -> AutolabelDataset:
         """Read the sql query and sets dat, inputs and gt_labels
 
         Args:
             connection (str): connection string
             config (AutolabelConfig): config object
             max_items (int, optional): max number of items to read. Defaults to None.
             start_index (int, optional): start index to read from. Defaults to 0.
         """
         logger.debug(f"reading the sql from: {start_index}")
         label_column = config.label_column()
 
-        self.dat = pd.read_sql(sql, connection)[start_index:]
-        self.dat = self.dat.astype(str)
+        dat = pd.read_sql(sql, connection)[start_index:]
+        dat = dat.astype(str)
         if max_items and max_items > 0:
-            max_items = min(max_items, len(self.dat))
-            self.dat = self.dat[:max_items]
+            max_items = min(max_items, len(dat))
+            dat = dat[:max_items]
 
-        self.inputs = self.dat.to_dict(orient="records")
-        self.gt_labels = (
+        inputs = dat.to_dict(orient="records")
+        gt_labels = (
             None
-            if not label_column
-            or not len(self.inputs)
-            or label_column not in self.inputs[0]
-            else self.dat[label_column].tolist()
+            if not label_column or not len(inputs) or label_column not in inputs[0]
+            else dat[label_column].tolist()
+        )
+        return AutolabelDataset(
+            columns=list(dat.columns),
+            dataset=dat,
+            inputs=inputs,
+            gt_labels=gt_labels,
         )
 
-    def _read_file(
-        self,
-        file: str,
-        config: AutolabelConfig,
-        max_items: int = None,
-        start_index: int = 0,
-    ) -> None:
-        """Read the file and sets dat, inputs and gt_labels
-
-        Args:
-            file (str): path to the file
-            config (AutolabelConfig): config object
-            max_items (int, optional): max number of items to read. Defaults to None.
-            start_index (int, optional): start index to read from. Defaults to 0.
-
-        Raises:
-            ValueError: if the file format is not supported
-        """
-        if file.endswith(".csv"):
-            return self._read_csv(
-                file, config, max_items=max_items, start_index=start_index
-            )
-        elif file.endswith(".jsonl"):
-            return self._read_jsonl(
-                file, config, max_items=max_items, start_index=start_index
-            )
-        else:
-            raise ValueError(f"Unsupported file format: {file}")
 
-    def _read_hf_dataset(
-        self,
-        dataset: Dataset,
+class DataframeReader:
+    @staticmethod
+    def read(
+        df: pd.DataFrame,
         config: AutolabelConfig,
         max_items: int = None,
         start_index: int = 0,
-    ) -> None:
-        """Read the huggingface dataset and sets dat, inputs and gt_labels
+    ) -> AutolabelDataset:
+        """Read the csv file and sets dat, inputs and gt_labels
 
         Args:
-            dataset (Dataset): dataset object to read from
+            df (pd.DataFrame): dataframe to read
             config (AutolabelConfig): config object
             max_items (int, optional): max number of items to read. Defaults to None.
             start_index (int, optional): start index to read from. Defaults to 0.
         """
-        dataset.set_format("pandas")
-        self.dat = dataset[
-            start_index : max_items if max_items and max_items > 0 else len(dataset)
-        ]
+        label_column = config.label_column()
 
-        self.inputs = self.dat.to_dict(orient="records")
-        self.gt_labels = (
+        dat = df[start_index:].astype(str)
+        if max_items and max_items > 0:
+            max_items = min(max_items, len(dat))
+            dat = dat[:max_items]
+
+        inputs = dat.to_dict(orient="records")
+        gt_labels = (
             None
-            if not config.label_column()
-            or not len(self.inputs)
-            or config.label_column() not in self.inputs[0]
-            else self.dat[config.label_column()].tolist()
+            if not label_column or not len(inputs) or label_column not in inputs[0]
+            else dat[label_column].tolist()
+        )
+        return AutolabelDataset(
+            columns=list(dat.columns),
+            dataset=dat,
+            inputs=inputs,
+            gt_labels=gt_labels,
         )
```

### Comparing `refuel-autolabel-0.0.7/src/autolabel/few_shot/__init__.py` & `refuel-autolabel-0.0.8/src/autolabel/few_shot/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 import logging
 from typing import Dict, List
 
 from autolabel.configs import AutolabelConfig
 from autolabel.schema import FewShotAlgorithm, ModelProvider
 from langchain.embeddings import (
+    CohereEmbeddings,
     HuggingFaceEmbeddings,
     OpenAIEmbeddings,
     VertexAIEmbeddings,
 )
 from langchain.embeddings.base import Embeddings
 from langchain.prompts.example_selector import (
     MaxMarginalRelevanceExampleSelector,
     SemanticSimilarityExampleSelector,
 )
 from langchain.prompts.example_selector.base import BaseExampleSelector
 
 from .fixed_example_selector import FixedExampleSelector
+from .label_diversity_example_selector import (
+    LabelDiversityRandomExampleSelector,
+    LabelDiversitySimilarityExampleSelector,
+)
 from .vector_store import VectorStoreWrapper
 
 ALGORITHM_TO_IMPLEMENTATION: Dict[FewShotAlgorithm, BaseExampleSelector] = {
     FewShotAlgorithm.FIXED: FixedExampleSelector,
     FewShotAlgorithm.SEMANTIC_SIMILARITY: SemanticSimilarityExampleSelector,
     FewShotAlgorithm.MAX_MARGINAL_RELEVANCE: MaxMarginalRelevanceExampleSelector,
+    FewShotAlgorithm.LABEL_DIVERSITY_RANDOM: LabelDiversityRandomExampleSelector,
+    FewShotAlgorithm.LABEL_DIVERSITY_SIMILARITY: LabelDiversitySimilarityExampleSelector,
 }
 
 DEFAULT_EMBEDDING_PROVIDER = OpenAIEmbeddings
 
 PROVIDER_TO_MODEL: Dict[ModelProvider, Embeddings] = {
     ModelProvider.OPENAI: OpenAIEmbeddings,
     ModelProvider.GOOGLE: VertexAIEmbeddings,
     ModelProvider.HUGGINGFACE_PIPELINE: HuggingFaceEmbeddings,
+    ModelProvider.COHERE: CohereEmbeddings,
 }
 
 logger = logging.getLogger(__name__)
 
 
 class ExampleSelectorFactory:
     CANDIDATE_EXAMPLES_FACTOR = 5
@@ -56,14 +64,15 @@
             return None
 
         num_examples = config.few_shot_num_examples()
         params = {"examples": examples, "k": num_examples}
         if algorithm in [
             FewShotAlgorithm.SEMANTIC_SIMILARITY,
             FewShotAlgorithm.MAX_MARGINAL_RELEVANCE,
+            FewShotAlgorithm.LABEL_DIVERSITY_SIMILARITY,
         ]:
             model_provider = config.embedding_provider()
             embedding_model_class = PROVIDER_TO_MODEL.get(
                 model_provider, DEFAULT_EMBEDDING_PROVIDER
             )
             model_name = config.embedding_model_name()
             if model_name:
@@ -79,10 +88,16 @@
             ]
             params["input_keys"] = input_keys
         if algorithm == FewShotAlgorithm.MAX_MARGINAL_RELEVANCE:
             params["fetch_k"] = min(
                 ExampleSelectorFactory.MAX_CANDIDATE_EXAMPLES,
                 ExampleSelectorFactory.CANDIDATE_EXAMPLES_FACTOR * params["k"],
             )
+        if algorithm in [
+            FewShotAlgorithm.LABEL_DIVERSITY_RANDOM,
+            FewShotAlgorithm.LABEL_DIVERSITY_SIMILARITY,
+        ]:
+            params["label_key"] = config.label_column()
+            params["num_labels"] = len(config.labels_list())
 
         example_cls = ALGORITHM_TO_IMPLEMENTATION[algorithm]
         return example_cls.from_examples(**params)
```

### Comparing `refuel-autolabel-0.0.7/src/autolabel/few_shot/fixed_example_selector.py` & `refuel-autolabel-0.0.8/src/autolabel/few_shot/fixed_example_selector.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/few_shot/vector_store.py` & `refuel-autolabel-0.0.8/src/autolabel/few_shot/vector_store.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import heapq
+from itertools import groupby
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Type
 
 import numpy as np
 import torch
 from langchain.docstore.document import Document
 from langchain.embeddings.base import Embeddings
 from langchain.vectorstores.base import VectorStore
@@ -203,14 +204,90 @@
         )
         result_ids = [result["corpus_id"] for result in result_ids_and_scores[0]]
         scores = [result["score"] for result in result_ids_and_scores[0]]
         results = {}
         results["documents"] = [[self._texts[index] for index in result_ids]]
         results["distances"] = [scores]
         results["metadatas"] = [[self._metadatas[index] for index in result_ids]]
+        return _results_to_docs_and_scores(results)
+
+    def label_diversity_similarity_search(
+        self,
+        query: str,
+        label_key: str,
+        k: int = 4,
+        filter: Optional[Dict[str, str]] = None,
+        **kwargs: Any,
+    ) -> List[Document]:
+        """Run semantic similarity search.
+        Args:
+            query (str): Query text to search for.
+            k (int): Number of results to return per label.
+            filter (Optional[Dict[str, str]]): Filter by metadata. Defaults to None.
+        Returns:
+            List[Document]: List of documents most similar to the query text.
+        """
+        docs_and_scores = self.label_diversity_similarity_search_with_score(
+            query, label_key, k, filter=filter
+        )
+        return [doc for doc, _ in docs_and_scores]
+
+    def label_diversity_similarity_search_with_score(
+        self,
+        query: str,
+        label_key: str,
+        k: int = 4,
+        filter: Optional[Dict[str, str]] = None,
+        **kwargs: Any,
+    ) -> List[Tuple[Document, float]]:
+        """Run semantic similarity search and retrieve distances.
+        Args:
+            query (str): Query text to search for.
+            k (int): Number of results to return. Defaults to 4.
+            filter (Optional[Dict[str, str]]): Filter by metadata. Defaults to None.
+        Returns:
+            List[Tuple[Document, float]]: List of documents most similar to the query
+                text with distance in float.
+        """
+        query_embeddings = torch.tensor([self._embedding_function.embed_query(query)])
+        data = []
+        data = zip(self._corpus_embeddings, self._texts, self._metadatas)
+        sorted_data = sorted(data, key=lambda item: item[2].get(label_key))
+
+        documents = []
+        scores = []
+        metadatas = []
+        for label, label_examples in groupby(
+            sorted_data, key=lambda item: item[2].get(label_key)
+        ):
+            label_examples_list = list(label_examples)
+            label_embeddings = list(
+                map(lambda label_example: label_example[0], label_examples_list)
+            )
+            label_texts = list(
+                map(lambda label_example: label_example[1], label_examples_list)
+            )
+            label_metadatas = list(
+                map(lambda label_example: label_example[2], label_examples_list)
+            )
+
+            result_ids_and_scores = semantic_search(
+                corpus_embeddings=label_embeddings,
+                query_embeddings=query_embeddings,
+                top_k=k,
+            )
+            result_ids = [result["corpus_id"] for result in result_ids_and_scores[0]]
+            documents.extend([label_texts[index] for index in result_ids])
+            metadatas.extend([label_metadatas[index] for index in result_ids])
+            scores.extend([result["score"] for result in result_ids_and_scores[0]])
+        results = {}
+
+        results["documents"] = [documents]
+        results["distances"] = [scores]
+        results["metadatas"] = [metadatas]
 
         return _results_to_docs_and_scores(results)
 
     def max_marginal_relevance_search_by_vector(
         self,
         query: str,
         k: int = 4,
```

### Comparing `refuel-autolabel-0.0.7/src/autolabel/labeler.py` & `refuel-autolabel-0.0.8/src/autolabel/labeler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
+import logging
 import os
 import sys
 from typing import Dict, List, Optional, Tuple, Union
-import logging
 
 import numpy as np
 import pandas as pd
 from rich import print as pprint
 from rich.console import Console
 from rich.prompt import Confirm
-import pandas as pd
 
 from autolabel.cache import SQLAlchemyCache
 from autolabel.confidence import ConfidenceCalculator
 from autolabel.configs import AutolabelConfig
+from autolabel.data_loaders import DatasetLoader
 from autolabel.data_models import AnnotationModel, TaskRunModel
 from autolabel.database import StateManager
-from autolabel.dataset_loader import DatasetLoader
 from autolabel.few_shot import ExampleSelectorFactory
 from autolabel.models import BaseModel, ModelFactory
 from autolabel.schema import LLMAnnotation, MetricResult, TaskRun, TaskStatus
 from autolabel.tasks import TaskFactory
-from autolabel.utils import track, track_with_stats, print_table, maybe_round
+from autolabel.utils import maybe_round, print_table, track, track_with_stats
 
 console = Console()
 logger = logging.getLogger(__name__)
 
 COST_TABLE_STYLES = {
     "parameter": "magenta bold",
     "value": "green bold",
@@ -440,15 +439,16 @@
         self,
         seed_examples: Union[str, List[Dict]],
     ) -> List[Dict]:
         """Use LLM to generate explanations for why examples are labeled the way that they are."""
         out_file = None
         if isinstance(seed_examples, str):
             out_file = seed_examples
-            _, seed_examples, _ = DatasetLoader.read_file(seed_examples, self.config)
+            seed_loader = DatasetLoader(seed_examples, self.config)
+            seed_examples = seed_loader.inputs
 
         explanation_column = self.config.explanation_column()
         if not explanation_column:
             raise ValueError(
                 "The explanation column needs to be specified in the dataset config."
             )
```

### Comparing `refuel-autolabel-0.0.7/src/autolabel/models/__init__.py` & `refuel-autolabel-0.0.8/src/autolabel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/models/anthropic.py` & `refuel-autolabel-0.0.8/src/autolabel/models/anthropic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 from anthropic import tokenizer
 from autolabel.configs import AutolabelConfig
 from autolabel.models import BaseModel
 from autolabel.cache import BaseCache
 from langchain.chat_models import ChatAnthropic
-from langchain.schema import Generation, LLMResult, HumanMessage
+from langchain.schema import LLMResult, HumanMessage
 
 
 class AnthropicLLM(BaseModel):
     DEFAULT_MODEL = "claude-instant-v1"
     DEFAULT_PARAMS = {
         "max_tokens_to_sample": 1000,
         "temperature": 0.0,
@@ -36,20 +36,18 @@
         self.model_params = {**self.DEFAULT_PARAMS, **model_params}
         # initialize LLM
         self.llm = ChatAnthropic(model=self.model_name, **self.model_params)
 
     def _label(self, prompts: List[str]) -> LLMResult:
         prompts = [[HumanMessage(content=prompt)] for prompt in prompts]
         try:
-            response = self.llm.generate(prompts)
-            return response
+            return self.llm.generate(prompts)
         except Exception as e:
-            print(f"Error generating from LLM: {e}, returning empty result")
-            generations = [[Generation(text="")] for _ in prompts]
-            return LLMResult(generations=generations)
+            print(f"Error generating from LLM: {e}, retrying each prompt individually")
+            return self._label_individually(prompts)
 
     def get_cost(self, prompt: str, label: Optional[str] = "") -> float:
         num_prompt_toks = tokenizer.count_tokens(prompt)
         if label:
             num_label_toks = tokenizer.count_tokens(label)
         else:
             # get an upper bound
```

### Comparing `refuel-autolabel-0.0.7/src/autolabel/models/base.py` & `refuel-autolabel-0.0.8/src/autolabel/models/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Base interface that all model providers will implement."""
 
 from abc import ABC, abstractmethod
 from typing import List, Optional, Dict, Tuple
 
-from langchain.schema import LLMResult
+from langchain.schema import LLMResult, Generation
 
 from autolabel.configs import AutolabelConfig
 from autolabel.schema import CacheEntry
 from autolabel.cache import BaseCache
 
 
 class BaseModel(ABC):
@@ -48,14 +48,34 @@
                 self.update_cache(missing_prompt_idxs, new_results, prompts)
 
             llm_output = new_results.llm_output
 
         generations = [existing_prompts[i] for i in range(len(prompts))]
         return LLMResult(generations=generations, llm_output=llm_output), cost
 
+    def _label_individually(self, prompts: List[str]) -> LLMResult:
+        """Label each prompt individually. Should be used only after trying as a batch first.
+
+        Args:
+            prompts (List[str]): List of prompts to label
+
+        Returns:
+            LLMResult: LLMResult object with generations
+        """
+        generations = []
+        for prompt in prompts:
+            try:
+                response = self.llm.generate([prompt])
+                generations.append(response.generations[0])
+            except Exception as e:
+                print(f"Error generating from LLM: {e}, returning empty generation")
+                generations.append([Generation(text="")])
+
+        return LLMResult(generations=generations)
+
     @abstractmethod
     def _label(self, prompts: List[str]) -> LLMResult:
         # TODO: change return type to do parsing in the Model class
         pass
 
     @abstractmethod
     def get_cost(self, prompt: str, label: Optional[str] = "") -> float:
```

### Comparing `refuel-autolabel-0.0.7/src/autolabel/models/cohere.py` & `refuel-autolabel-0.0.8/src/autolabel/models/cohere.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,17 +37,16 @@
         self.llm = Cohere(model=self.model_name, **self.model_params)
         self.co = cohere.Client(api_key=os.environ["COHERE_API_KEY"])
 
     def _label(self, prompts: List[str]) -> LLMResult:
         try:
             return self.llm.generate(prompts)
         except Exception as e:
-            print(f"Error generating from LLM: {e}, returning empty result")
-            generations = [[Generation(text="")] for _ in prompts]
-            return LLMResult(generations=generations)
+            print(f"Error generating from LLM: {e}, retrying each prompt individually")
+            return self._label_individually(prompts)
 
     def get_cost(self, prompt: str, label: Optional[str] = "") -> float:
         num_prompt_toks = len(self.co.tokenize(prompt).tokens)
         if label:
             num_label_toks = len(self.co.tokenize(label).tokens)
         else:
             num_label_toks = self.model_params["max_tokens"]
```

### Comparing `refuel-autolabel-0.0.7/src/autolabel/models/hf_pipeline.py` & `refuel-autolabel-0.0.8/src/autolabel/models/hf_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional
 from langchain.llms import HuggingFacePipeline
-from langchain.schema import LLMResult, Generation
+from langchain.schema import LLMResult
 
 from autolabel.models import BaseModel
 from autolabel.configs import AutolabelConfig
 from autolabel.cache import BaseCache
 
 
 class HFPipelineLLM(BaseModel):
@@ -65,17 +65,16 @@
         # initialize LLM
         self.llm = HuggingFacePipeline(pipeline=pipe, model_kwargs=model_kwargs)
 
     def _label(self, prompts: List[str]) -> LLMResult:
         try:
             return self.llm.generate(prompts)
         except Exception as e:
-            print(f"Error generating from LLM: {e}, returning empty result")
-            generations = [[Generation(text="")] for _ in prompts]
-            return LLMResult(generations=generations)
+            print(f"Error generating from LLM: {e}, retrying each prompt individually")
+            return self._label_individually(prompts)
 
     def get_cost(self, prompt: str, label: Optional[str] = "") -> float:
         # Model inference for this model is being run locally
         # Revisit this in the future when we support HF inference endpoints
         return 0.0
 
     def returns_token_probs(self) -> bool:
```

### Comparing `refuel-autolabel-0.0.7/src/autolabel/models/openai.py` & `refuel-autolabel-0.0.8/src/autolabel/models/openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from functools import cached_property
 from typing import List, Optional
 import logging
 
 from langchain.chat_models import ChatOpenAI
 from langchain.llms import OpenAI
-from langchain.schema import LLMResult, HumanMessage, Generation
+from langchain.schema import LLMResult, HumanMessage
 import tiktoken
 
 from autolabel.models import BaseModel
 from autolabel.configs import AutolabelConfig
 from autolabel.cache import BaseCache
 
+import os
 
 logger = logging.getLogger(__name__)
 
 
 class OpenAILLM(BaseModel):
     CHAT_ENGINE_MODELS = [
         "gpt-3.5-turbo",
+        "gpt-3.5-turbo-0301",
         "gpt-3.5-turbo-0613",
         "gpt-3.5-turbo-16k",
         "gpt-3.5-turbo-16k-0613",
         "gpt-4",
+        "gpt-4-0314",
+        "gpt-4-32k-0314",
         "gpt-4-0613",
         "gpt-4-32k",
         "gpt-4-32k-0613",
     ]
     MODELS_WITH_TOKEN_PROBS = ["text-curie-001", "text-davinci-003"]
 
     # Default parameters for OpenAILLM
@@ -41,47 +45,56 @@
     }
 
     # Reference: https://openai.com/pricing
     COST_PER_PROMPT_TOKEN = {
         "text-davinci-003": 0.02 / 1000,
         "text-curie-001": 0.002 / 1000,
         "gpt-3.5-turbo": 0.0015 / 1000,
+        "gpt-3.5-turbo-0301": 0.0015 / 1000,
         "gpt-3.5-turbo-0613": 0.0015 / 1000,
         "gpt-3.5-turbo-16k": 0.003 / 1000,
         "gpt-3.5-turbo-16k-0613": 0.003 / 1000,
         "gpt-4": 0.03 / 1000,
         "gpt-4-0613": 0.03 / 1000,
         "gpt-4-32k": 0.06 / 1000,
         "gpt-4-32k-0613": 0.06 / 1000,
+        "gpt-4-0314": 0.03 / 1000,
+        "gpt-4-32k-0314": 0.06 / 1000,
     }
     COST_PER_COMPLETION_TOKEN = {
         "text-davinci-003": 0.02 / 1000,
         "text-curie-001": 0.002 / 1000,
         "gpt-3.5-turbo": 0.002 / 1000,
+        "gpt-3.5-turbo-0301": 0.002 / 1000,
         "gpt-3.5-turbo-0613": 0.002 / 1000,
         "gpt-3.5-turbo-16k": 0.004 / 1000,
         "gpt-3.5-turbo-16k-0613": 0.004 / 1000,
         "gpt-4": 0.06 / 1000,
         "gpt-4-0613": 0.06 / 1000,
         "gpt-4-32k": 0.12 / 1000,
         "gpt-4-32k-0613": 0.12 / 1000,
+        "gpt-4-0314": 0.06 / 1000,
+        "gpt-4-32k-0314": 0.12 / 1000,
     }
 
     @cached_property
     def _engine(self) -> str:
         if self.model_name is not None and self.model_name in self.CHAT_ENGINE_MODELS:
             return "chat"
         else:
             return "completion"
 
     def __init__(self, config: AutolabelConfig, cache: BaseCache = None) -> None:
         super().__init__(config, cache)
         # populate model name
         self.model_name = config.model_name() or self.DEFAULT_MODEL
 
+        if os.getenv("OPENAI_API_KEY") is None:
+            raise ValueError("OPENAI_API_KEY environment variable not set")
+
         # populate model params and initialize the LLM
         model_params = config.model_params()
         if config.logit_bias():
             logit_bias = self._generate_logit_bias(config)
             # if logit_bias or max_tokens is specified already, we don't want to overwrite it
             model_params = {
                 **logit_bias,
@@ -129,17 +142,16 @@
             # Need to convert list[prompts] -> list[messages]
             # Currently the entire prompt is stuck into the "human message"
             # We might consider breaking this up into human vs system message in future
             prompts = [[HumanMessage(content=prompt)] for prompt in prompts]
         try:
             return self.llm.generate(prompts)
         except Exception as e:
-            print(f"Error generating from LLM: {e}, returning empty result")
-            generations = [[Generation(text="")] for _ in prompts]
-            return LLMResult(generations=generations)
+            print(f"Error generating from LLM: {e}, retrying each prompt individually")
+            return self._label_individually(prompts)
 
     def get_cost(self, prompt: str, label: Optional[str] = "") -> float:
         encoding = tiktoken.encoding_for_model(self.model_name)
         num_prompt_toks = len(encoding.encode(prompt))
         if label:
             num_label_toks = len(encoding.encode(label))
         else:
```

### Comparing `refuel-autolabel-0.0.7/src/autolabel/models/palm.py` & `refuel-autolabel-0.0.8/src/autolabel/models/palm.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,14 +62,38 @@
         stop=stop_after_attempt(5),
         wait=wait_exponential(multiplier=1, min=2, max=10),
         before_sleep=before_sleep_log(logger, logging.WARNING),
     )
     def _label_with_retry(self, prompts: List[str]) -> LLMResult:
         return self.llm.generate(prompts)
 
+    def _label_individually(self, prompts: List[str]) -> LLMResult:
+        """Label each prompt individually. Should be used only after trying as a batch first.
+
+        Args:
+            prompts (List[str]): List of prompts to label
+
+        Returns:
+            LLMResult: LLMResult object with generations
+        """
+        generations = []
+        for i, prompt in enumerate(prompts):
+            try:
+                response = self._label_with_retry([prompt])
+                for generation in response.generations[0]:
+                    generation.text = generation.text.replace(
+                        self.SEP_REPLACEMENT_TOKEN, "\n"
+                    )
+                generations.append(response.generations[0])
+            except Exception as e:
+                print(f"Error generating from LLM: {e}, returning empty generation")
+                generations.append([Generation(text="")])
+
+        return LLMResult(generations=generations)
+
     def _label(self, prompts: List[str]) -> LLMResult:
         for prompt in prompts:
             if self.SEP_REPLACEMENT_TOKEN in prompt:
                 logger.warning(
                     f"""Current prompt contains {self.SEP_REPLACEMENT_TOKEN} 
                                 which is currently used as a separator token by refuel
                                 llm. It is highly recommended to avoid having any
@@ -90,17 +114,16 @@
             for generations in result.generations:
                 for generation in generations:
                     generation.text = generation.text.replace(
                         self.SEP_REPLACEMENT_TOKEN, "\n"
                     )
             return result
         except Exception as e:
-            logger.error(f"Error generating from LLM: {e}.")
-        generations = [[Generation(text="")] for _ in prompts]
-        return LLMResult(generations=generations)
+            print(f"Error generating from LLM: {e}, retrying each prompt individually")
+            self._label_individually(prompts)
 
     def get_cost(self, prompt: str, label: Optional[str] = "") -> float:
         if self.model_name is None:
             return 0.0
         cost_per_char = self.COST_PER_CHARACTER.get(self.model_name, 0.0)
         return cost_per_char * len(prompt)
```

### Comparing `refuel-autolabel-0.0.7/src/autolabel/models/refuel.py` & `refuel-autolabel-0.0.8/src/autolabel/models/refuel.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/schema.py` & `refuel-autolabel-0.0.8/src/autolabel/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from datetime import datetime
 from enum import Enum
-from typing import Any, Dict, Optional, List, Union
-import pandas as pd
+from typing import Any, Dict, List, Optional, Union
 
+import pandas as pd
+from langchain.schema import Generation
 from pydantic import BaseModel
 
 from autolabel.configs import AutolabelConfig
 from autolabel.utils import calculate_md5
-from langchain.schema import Generation
 
 
 class ModelProvider(str, Enum):
     """Enum containing all LLM providers currently supported by autolabeler"""
 
     OPENAI = "openai"
     ANTHROPIC = "anthropic"
@@ -33,14 +33,16 @@
 
 class FewShotAlgorithm(str, Enum):
     """Enum of supported algorithms for choosing which examples to provide the LLM in its instruction prompt"""
 
     FIXED = "fixed"
     SEMANTIC_SIMILARITY = "semantic_similarity"
     MAX_MARGINAL_RELEVANCE = "max_marginal_relevance"
+    LABEL_DIVERSITY_RANDOM = "label_diversity_random"
+    LABEL_DIVERSITY_SIMILARITY = "label_diversity_similarity"
 
 
 class TaskStatus(str, Enum):
     ACTIVE = "active"
 
 
 class Metric(str, Enum):
```

### Comparing `refuel-autolabel-0.0.7/src/autolabel/tasks/__init__.py` & `refuel-autolabel-0.0.8/src/autolabel/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/tasks/base.py` & `refuel-autolabel-0.0.8/src/autolabel/tasks/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/tasks/classification.py` & `refuel-autolabel-0.0.8/src/autolabel/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/tasks/entity_matching.py` & `refuel-autolabel-0.0.8/src/autolabel/tasks/entity_matching.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/tasks/multilabel_classification.py` & `refuel-autolabel-0.0.8/src/autolabel/tasks/multilabel_classification.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/tasks/named_entity_recognition.py` & `refuel-autolabel-0.0.8/src/autolabel/tasks/named_entity_recognition.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/tasks/question_answering.py` & `refuel-autolabel-0.0.8/src/autolabel/tasks/question_answering.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/tasks/utils.py` & `refuel-autolabel-0.0.8/src/autolabel/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/autolabel/utils.py` & `refuel-autolabel-0.0.8/src/autolabel/utils.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/PKG-INFO` & `refuel-autolabel-0.0.8/src/refuel_autolabel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refuel-autolabel
-Version: 0.0.7
+Version: 0.0.8
 Summary: Label, clean and enrich text datasets with LLMs
 Author-email: "Refuel.ai" <support@refuel.ai>
 License: MIT License
         
         Copyright (c) 2023 refuel-ai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,15 +41,14 @@
 Provides-Extra: google
 Provides-Extra: cohere
 Provides-Extra: all
 License-File: LICENSE
 
 <img alt="Refuel logo" src="https://raw.githubusercontent.com/refuel-ai/autolabel/main/docs/assets/Autolabel_blk_w_background.png">
 
-
 <h4 align="center">
   <a href="https://discord.gg/fweVnRx6CU">Discord</a> |
   <a href="https://twitter.com/RefuelAI">Twitter</a> |
   <a href="https://www.refuel.ai/">Website</a> |
   <a href="https://www.refuel.ai/blog-posts/llm-labeling-technical-report">Benchmark</a>
 </h4>
 
@@ -95,15 +94,15 @@
         "delimiter": ","
     },
     "prompt": {
         "task_guidelines": "You are an expert at analyzing the sentiment of movie reviews. Your job is to classify the provided movie review into one of the following labels: {labels}",
         "labels": [
             "positive",
             "negative",
-            "neutral",
+            "neutral"
         ],
         "few_shot_examples": [
             {
                 "example": "I got a fairly uninspired stupid film about how human industry is bad for nature.",
                 "label": "negative"
             },
             {
@@ -208,15 +207,14 @@
 
 ## 🛠️ Roadmap
 
 Check out our [public roadmap](https://github.com/orgs/refuel-ai/projects/15) to learn more about ongoing and planned improvements to the Autolabel library.
 
 We are always looking for suggestions and contributions from the community. Join the discussion on [Discord](https://discord.gg/fweVnRx6CU) or open a [Github issue](https://github.com/refuel-ai/autolabel/issues) to report bugs and request features.
 
-
 ## 🙌 Contributing
 
 Autolabel is a rapidly developing project. We welcome contributions in all forms - bug reports, pull requests and ideas for improving the library.
 
 1. Join the conversation on [Discord](https://discord.gg/fweVnRx6CU)
 2. Open an [issue](https://github.com/refuel-ai/autolabel/issues) on Github for bugs and request features.
 3. Grab an open issue, and submit a [pull request](https://github.com/refuel-ai/autolabel/blob/main/CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.7 Summary: Label,
+Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.8 Summary: Label,
 clean and enrich text datasets with LLMs Author-email: "Refuel.ai"
 refuel.ai> License: MIT License Copyright (c) 2023 refuel-ai Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -49,15 +49,15 @@
 sentiment analysis of movie review. We have a dataset of movie reviews that
 we'd like to get labeled first. For this case, here's what the example dataset
 and configs will look like: ```python { "task_name": "MovieSentimentReview",
 "task_type": "classification", "model": { "provider": "openai", "name": "gpt-
 3.5-turbo" }, "dataset": { "label_column": "label", "delimiter": "," },
 "prompt": { "task_guidelines": "You are an expert at analyzing the sentiment of
 movie reviews. Your job is to classify the provided movie review into one of
-the following labels: {labels}", "labels": [ "positive", "negative", "neutral",
+the following labels: {labels}", "labels": [ "positive", "negative", "neutral"
 ], "few_shot_examples": [ { "example": "I got a fairly uninspired stupid film
 about how human industry is bad for nature.", "label": "negative" },
 { "example": "I loved this movie. I found it very heart warming to see Adam
 West, Burt Ward, Frank Gorshin, and Julie Newmar together again.", "label":
 "positive" }, { "example": "This movie will be played next week at the Chinese
 theater.", "label": "neutral" } ], "example_template": "Input:
 {example}\nOutput: {label}" } } ``` Initialize the labeling agent and pass it
```

### Comparing `refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/SOURCES.txt` & `refuel-autolabel-0.0.8/src/refuel_autolabel.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 LICENSE
 README.md
 pyproject.toml
 src/autolabel/__init__.py
 src/autolabel/confidence.py
-src/autolabel/dataset_loader.py
 src/autolabel/labeler.py
 src/autolabel/schema.py
 src/autolabel/utils.py
 src/autolabel/cache/__init__.py
 src/autolabel/cache/base.py
 src/autolabel/cache/sqlalchemy_cache.py
 src/autolabel/configs/__init__.py
 src/autolabel/configs/base.py
 src/autolabel/configs/config.py
 src/autolabel/configs/schema.py
+src/autolabel/data_loaders/__init__.py
+src/autolabel/data_loaders/read_datasets.py
+src/autolabel/data_loaders/validation.py
 src/autolabel/data_models/__init__.py
 src/autolabel/data_models/annotation.py
 src/autolabel/data_models/base.py
 src/autolabel/data_models/cache.py
 src/autolabel/data_models/dataset.py
 src/autolabel/data_models/task.py
 src/autolabel/data_models/task_run.py
 src/autolabel/database/__init__.py
 src/autolabel/database/engine.py
 src/autolabel/database/state_manager.py
 src/autolabel/few_shot/__init__.py
 src/autolabel/few_shot/fixed_example_selector.py
+src/autolabel/few_shot/label_diversity_example_selector.py
 src/autolabel/few_shot/vector_store.py
 src/autolabel/models/__init__.py
 src/autolabel/models/anthropic.py
 src/autolabel/models/base.py
 src/autolabel/models/cohere.py
 src/autolabel/models/hf_pipeline.py
 src/autolabel/models/openai.py
```

### Comparing `refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/requires.txt` & `refuel-autolabel-0.0.8/src/refuel_autolabel.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 scipy>=1.10.1
 pydantic>=1.10.9
 torch>=1.10.0
 matplotlib>=3.5.0
 wget>=3.2
 ipywidgets==8.0.6
 jsonschema>=4.17.3
+tabulate>=0.9.0
 
 [all]
 black
 bumpver
 pip-tools
 pytest
 pytest-mock
```


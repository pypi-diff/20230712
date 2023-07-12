# Comparing `tmp/xturing-0.1.5.tar.gz` & `tmp/xturing-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xturing-0.1.5.tar", last modified: Wed Jun 14 11:35:01 2023, max compression
+gzip compressed data, was "xturing-0.1.6.tar", last modified: Wed Jul 12 11:45:19 2023, max compression
```

## Comparing `xturing-0.1.5.tar` & `xturing-0.1.6.tar`

### file list

```diff
@@ -1,118 +1,122 @@
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.557886 xturing-0.1.5/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    11357 2023-06-13 13:40:44.000000 xturing-0.1.5/LICENSE
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       34 2023-06-13 13:40:44.000000 xturing-0.1.5/MANIFEST.in
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    21821 2023-06-14 11:35:01.557886 xturing-0.1.5/PKG-INFO
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     7359 2023-06-13 13:40:44.000000 xturing-0.1.5/README.md
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2216 2023-06-14 11:34:56.000000 xturing-0.1.5/pyproject.toml
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       38 2023-06-14 11:35:01.557886 xturing-0.1.5/setup.cfg
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.541886 xturing-0.1.5/src/
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.545886 xturing-0.1.5/src/xturing/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       22 2023-06-14 11:34:56.000000 xturing-0.1.5/src/xturing/__about__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      438 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/__init__.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.545886 xturing-0.1.5/src/xturing/cli/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      561 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/cli/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2042 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/cli/api.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      989 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/cli/chat.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      131 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/cli/ui.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.549886 xturing-0.1.5/src/xturing/config/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      569 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/config/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      972 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/config/config_data_classes.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3593 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/config/finetuning_config.yaml
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3090 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/config/generation_config.yaml
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1892 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/config/read_config.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.549886 xturing-0.1.5/src/xturing/datasets/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      436 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/datasets/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      199 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/datasets/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8197 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/datasets/instruction_dataset.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      222 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/datasets/text2image_dataset.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/datasets/text_dataset.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.549886 xturing-0.1.5/src/xturing/engines/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4033 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      272 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1871 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/bloom_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     7209 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/causal.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1923 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/cerebras_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      804 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/distilgpt2_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2286 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/falcon_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1755 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/galactica_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1801 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/generic_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1446 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/gpt2_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2885 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/gptj_engine.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.549886 xturing-0.1.5/src/xturing/engines/gptj_utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/gptj_utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8053 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/gptj_utils/gptj.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6306 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/llama_engine.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.549886 xturing-0.1.5/src/xturing/engines/llama_utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       65 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/llama_utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    44506 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/llama_utils/llama.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.549886 xturing-0.1.5/src/xturing/engines/lora_engine/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       73 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/lora_engine/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    42467 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/lora_engine/lora.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3556 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/lora_engine/save_and_load.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/lora_engine/test.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/opt_engine.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.549886 xturing-0.1.5/src/xturing/engines/quant_utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       59 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/quant_utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8651 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/quant_utils/custom_autotune.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    28505 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/quant_utils/quant.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.553886 xturing-0.1.5/src/xturing/model_apis/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      864 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/model_apis/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1827 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/model_apis/ai21.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      573 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/model_apis/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1847 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/model_apis/cohere.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4600 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/model_apis/openai.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.553886 xturing-0.1.5/src/xturing/models/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3290 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2067 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1084 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/bloom.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8484 2023-06-14 11:34:56.000000 xturing-0.1.5/src/xturing/models/causal.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1135 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/cerebras.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      579 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/distilgpt2.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1101 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/falcon.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1152 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/galactica.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1664 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/generic.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1033 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/gpt2.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1067 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/gptj.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2259 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/llama.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1050 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/opt.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      808 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/stable_diffusion.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.553886 xturing-0.1.5/src/xturing/preprocessors/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      137 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/preprocessors/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      484 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/preprocessors/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4582 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/preprocessors/instruction_collator.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2252 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/preprocessors/text_collator.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      642 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/registry.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.557886 xturing-0.1.5/src/xturing/self_instruct/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     9891 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/bootstrap_instructions.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     5490 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/generate_instances.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3737 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/identify_if_classification.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    14280 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/prepare_for_finetuning.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2198 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/prepare_seed_tasks.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.557886 xturing-0.1.5/src/xturing/self_instruct/templates/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3580 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/templates/clf_task_template.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    12674 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/templates/instance_gen_template.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.557886 xturing-0.1.5/src/xturing/trainers/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       78 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/trainers/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      233 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/trainers/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6265 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/trainers/lightning_trainer.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.557886 xturing-0.1.5/src/xturing/ui/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/ui/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    13685 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/ui/playground.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.557886 xturing-0.1.5/src/xturing/utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      215 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/external_loggers.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3117 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/hub.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      304 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/interactive.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2147 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/logging.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      621 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/loss_fns.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1366 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/notebooks.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6886 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/text_splitter.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4034 2023-06-14 11:34:56.000000 xturing-0.1.5/src/xturing/utils/utils.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.545886 xturing-0.1.5/src/xturing.egg-info/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    21821 2023-06-14 11:35:01.000000 xturing-0.1.5/src/xturing.egg-info/PKG-INFO
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3335 2023-06-14 11:35:01.000000 xturing-0.1.5/src/xturing.egg-info/SOURCES.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        1 2023-06-14 11:35:01.000000 xturing-0.1.5/src/xturing.egg-info/dependency_links.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       48 2023-06-14 11:35:01.000000 xturing-0.1.5/src/xturing.egg-info/entry_points.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      243 2023-06-14 11:35:01.000000 xturing-0.1.5/src/xturing.egg-info/requires.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        8 2023-06-14 11:35:01.000000 xturing-0.1.5/src/xturing.egg-info/top_level.txt
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.369494 xturing-0.1.6/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    11357 2023-06-13 13:40:44.000000 xturing-0.1.6/LICENSE
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       34 2023-06-13 13:40:44.000000 xturing-0.1.6/MANIFEST.in
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    22233 2023-07-12 11:45:19.369494 xturing-0.1.6/PKG-INFO
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     7771 2023-07-12 11:43:55.000000 xturing-0.1.6/README.md
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2216 2023-07-12 11:43:55.000000 xturing-0.1.6/pyproject.toml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       38 2023-07-12 11:45:19.369494 xturing-0.1.6/setup.cfg
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.337494 xturing-0.1.6/src/
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.341494 xturing-0.1.6/src/xturing/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       22 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/__about__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      438 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/__init__.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.345494 xturing-0.1.6/src/xturing/cli/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      561 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/cli/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2042 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/cli/api.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      989 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/cli/chat.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      131 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/cli/ui.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.345494 xturing-0.1.6/src/xturing/config/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      569 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/config/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      972 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/config/config_data_classes.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4091 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/config/finetuning_config.yaml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3205 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/config/generation_config.yaml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1892 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/config/read_config.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.349494 xturing-0.1.6/src/xturing/datasets/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      436 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/datasets/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      199 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/datasets/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8197 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/datasets/instruction_dataset.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      222 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/datasets/text2image_dataset.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/datasets/text_dataset.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.349494 xturing-0.1.6/src/xturing/engines/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4254 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      272 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1871 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/bloom_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     9748 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/causal.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1923 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/cerebras_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      804 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/distilgpt2_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2986 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/falcon_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1755 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/galactica_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2310 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/generic_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1446 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/gpt2_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2885 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/gptj_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.353494 xturing-0.1.6/src/xturing/engines/gptj_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/gptj_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8053 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/gptj_utils/gptj.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6227 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/llama_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.353494 xturing-0.1.6/src/xturing/engines/llama_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       65 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/llama_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    44506 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/llama_utils/llama.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.353494 xturing-0.1.6/src/xturing/engines/lora_engine/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       73 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/lora_engine/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    47142 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/lora_engine/lora.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3556 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/lora_engine/save_and_load.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/lora_engine/test.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/opt_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.357494 xturing-0.1.6/src/xturing/engines/quant_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       59 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/quant_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2768 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/quant_utils/cachedistillationoutputs.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8651 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/quant_utils/custom_autotune.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    15980 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/quant_utils/lrec.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    12996 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/quant_utils/peft_utils.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2862 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/quant_utils/qerdataloading.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    28505 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/quant_utils/quant.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.357494 xturing-0.1.6/src/xturing/model_apis/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      864 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/model_apis/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1827 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/model_apis/ai21.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      573 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/model_apis/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1847 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/model_apis/cohere.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4600 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/model_apis/openai.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.361494 xturing-0.1.6/src/xturing/models/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3484 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/models/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2248 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/models/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1084 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/bloom.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8858 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/models/causal.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1135 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/cerebras.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      579 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/distilgpt2.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1373 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/models/falcon.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1152 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/galactica.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2851 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/models/generic.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1033 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/gpt2.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1067 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/gptj.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2331 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/models/llama.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1050 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/opt.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      808 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/stable_diffusion.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.361494 xturing-0.1.6/src/xturing/preprocessors/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      137 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/preprocessors/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      484 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/preprocessors/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4582 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/preprocessors/instruction_collator.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2252 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/preprocessors/text_collator.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      642 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/registry.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.365494 xturing-0.1.6/src/xturing/self_instruct/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     9891 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/bootstrap_instructions.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     5490 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/generate_instances.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3737 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/identify_if_classification.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    14280 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/prepare_for_finetuning.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2198 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/prepare_seed_tasks.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.365494 xturing-0.1.6/src/xturing/self_instruct/templates/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3580 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/templates/clf_task_template.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    12674 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/templates/instance_gen_template.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.365494 xturing-0.1.6/src/xturing/trainers/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       78 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/trainers/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      233 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/trainers/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6265 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/trainers/lightning_trainer.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.365494 xturing-0.1.6/src/xturing/ui/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/ui/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    13685 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/ui/playground.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.369494 xturing-0.1.6/src/xturing/utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      215 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/external_loggers.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3117 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/hub.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      304 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/interactive.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2147 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/logging.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      621 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/loss_fns.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1366 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/notebooks.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6886 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/text_splitter.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4034 2023-06-14 11:34:56.000000 xturing-0.1.6/src/xturing/utils/utils.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.341494 xturing-0.1.6/src/xturing.egg-info/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    22233 2023-07-12 11:45:19.000000 xturing-0.1.6/src/xturing.egg-info/PKG-INFO
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3531 2023-07-12 11:45:19.000000 xturing-0.1.6/src/xturing.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        1 2023-07-12 11:45:19.000000 xturing-0.1.6/src/xturing.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       48 2023-07-12 11:45:19.000000 xturing-0.1.6/src/xturing.egg-info/entry_points.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      243 2023-07-12 11:45:19.000000 xturing-0.1.6/src/xturing.egg-info/requires.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        8 2023-07-12 11:45:19.000000 xturing-0.1.6/src/xturing.egg-info/top_level.txt
```

### Comparing `xturing-0.1.5/LICENSE` & `xturing-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/PKG-INFO` & `xturing-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.1.5
+Version: 0.1.6
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -258,29 +258,23 @@
 - Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning) to reduce hardware costs by up to 90%
 - Explore different fine-tuning methods and benchmark them to find the best performing model
 - Evaluate fine-tuned models on well-defined metrics for in-depth analysis
 
 <br>
 
 ## 🌟 What's new?
-We are excited to announce the latest enhancements to our `xTuring` library: Falcon LLM integration and Generic model support. With this update, you can use and finetune Falcon-7B model with the off-the-shelf, off-the-shelf with INT8 precision, with LoRA architecture, and LoRA architecture with INT8 precision. Moreover, in case you do not find a model you want to run in the models' list, you can still us `xTuring` to run with the new `GenericModel` wrapper available to you. This new integration allows you to test and finetune any new model on xTuring without waiting for it to be integrated.
+We are excited to announce the latest enhancements to our `xTuring` library:
+1. __`Falcon LLM` integration__ - You can use and fine-tune the _`Falcon-7B`_ model in different configurations: _off-the-shelf_, _off-the-shelf with INT8 precision_, _LoRA fine-tuning_, and _LoRA fine-tuning with INT8 precision_.
+2. __`GenericModel` wrapper__ - This new integration allows you to test and fine-tune any new model on `xTuring` without waiting for it to be integrated using class _`GenericModel`_.
 
 You can check the  [Falcon LoRA INT8 working example](examples/falcon/falcon_lora_int8.py) repository to see how it works.
 Also, you can check the  [GenericModel working example](examples/generic/generic_model.py) repository to see how it works.
 
 <br>
 
-## CLI playground
-<img src=".github/cli-playground.gif" width="100%" style="margin: 0 1%;"/>
-
-## UI playground
-<img src=".github/ui-playground2.gif" width="100%" style="margin: 0 1%;"/>
-
-<br>
-
 ## ⚙️ Installation
 ```bash
 pip install xturing
 ```
 
 <br>
 
@@ -304,14 +298,43 @@
 print("Generated output by the model: {}".format(output))
 ```
 
 You can find the data folder [here](examples/llama/alpaca_data).
 
 <br>
 
+## CLI playground
+<img src=".github/cli-playground.gif" width="80%" style="margin: 0 1%;"/>
+
+```bash
+$ xturing chat -m "<path-to-model-folder>"
+
+```
+
+## UI playground
+<img src=".github/ui-playground2.gif" width="80%" style="margin: 0 1%;"/>
+
+```python
+from xturing.datasets import InstructionDataset
+from xturing.models import BaseModel
+from xturing.ui import Playground
+
+dataset = InstructionDataset("./alpaca_data")
+model = BaseModel.create("<model_name>")
+
+model.finetune(dataset=dataset)
+
+model.save("llama_lora_finetuned")
+
+Playground().launch() ## launches localhost UI
+
+```
+
+<br>
+
 ## 📚 Tutorials
 - [Preparing your dataset](examples/llama/preparing_your_dataset.py)
 - [Cerebras-GPT fine-tuning with LoRA and INT8](examples/cerebras/cerebras_lora_int8.ipynb) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eKq3oF7dnK8KuIfsTE70Gvvniwr1O9D0?usp=sharing)
 - [Cerebras-GPT fine-tuning with LoRA](examples/cerebras/cerebras_lora.ipynb) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VjqQhstm5pT4EjPjx4Je7b3W2X1V3vDo?usp=sharing)
 - [LLaMA fine-tuning with LoRA and INT8](examples/llama/llama_lora_int8.py) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1SQUXq1AMZPSLD4mk3A3swUIc6Y2dclme?usp=sharing)
 - [LLaMA fine-tuning with LoRA](examples/llama/llama_lora.py)
 - [LLaMA fine-tuning](examples/llama/llama.py)
@@ -334,19 +357,19 @@
 ```javascript
 {
   'maximum sequence length': 512,
   'batch size': 1,
 }
 ```
 
-|      LLaMA 7B      | DeepSpeed + CPU Offloading | LoRA + DeepSpeed  | LoRA + DeepSpeed + CPU Offloading |
-| --------- | ---- | ---- | ---- |
+|      LLaMA-7B      | DeepSpeed + CPU Offloading | LoRA + DeepSpeed  | LoRA + DeepSpeed + CPU Offloading |
+| :---------: | :----: | :----: | :----: |
 | GPU | 33.5 GB | 23.7 GB | 21.9 GB |
 | CPU | 190 GB  | 10.2 GB | 14.9 GB |
-| Time per epoch | 21 hours  | 20 mins | 20 mins |
+| Time/epoch | 21 hours  | 20 mins | 20 mins |
 
 Contribute to this by submitting your performance results on other GPUs by creating an issue with your hardware specifications, memory consumption and time per epoch.
 
 <br>
 
 ## 📎 Fine-tuned model checkpoints
 We have already fine-tuned some models that you can use as your base or start playing with.
@@ -361,25 +384,27 @@
 |---------------------|--------|---------------|
 | DistilGPT-2 LoRA | alpaca | `x/distilgpt2_lora_finetuned_alpaca` |
 | LLaMA LoRA          | alpaca | `x/llama_lora_finetuned_alpaca` |
 
 <br>
 
 ## 📈 Roadmap
-- [x] Support for LLaMA, GPT-J, GPT-2, OPT, Cerebras-GPT, Galactica and Bloom models
+- [x] Support for `LLaMA`, `GPT-J`, `GPT-2`, `OPT`, `Cerebras-GPT`, `Galactica` and `Bloom` models
 - [x] Dataset generation using self-instruction
 - [x] Low-precision LoRA fine-tuning and unsupervised fine-tuning
 - [x] INT8 low-precision fine-tuning support
 - [x] OpenAI, Cohere and AI21 Studio model APIs for dataset generation
 - [x] Added fine-tuned checkpoints for some models to the hub
 - [x] INT4 LLaMA LoRA fine-tuning demo
 - [x] INT4 LLaMA LoRA fine-tuning with INT4 generation
-- [x] Support for a generic model wrapper
-- [x] Support for Falcon-7B model
+- [x] Support for a `Generic model` wrapper
+- [x] Support for `Falcon-7B` model
+- [X] INT4 low-precision fine-tuning support
 - [ ] Evaluation of LLM models
+- [ ] INT3, INT2, INT1 low-precision fine-tuning support
 - [ ] Support for Stable Diffusion
 
 <br>
 
 ## 🤝 Help and Support
 If you have any questions, you can create an issue on this repository.
```

### Comparing `xturing-0.1.5/README.md` & `xturing-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -30,29 +30,23 @@
 - Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning) to reduce hardware costs by up to 90%
 - Explore different fine-tuning methods and benchmark them to find the best performing model
 - Evaluate fine-tuned models on well-defined metrics for in-depth analysis
 
 <br>
 
 ## 🌟 What's new?
-We are excited to announce the latest enhancements to our `xTuring` library: Falcon LLM integration and Generic model support. With this update, you can use and finetune Falcon-7B model with the off-the-shelf, off-the-shelf with INT8 precision, with LoRA architecture, and LoRA architecture with INT8 precision. Moreover, in case you do not find a model you want to run in the models' list, you can still us `xTuring` to run with the new `GenericModel` wrapper available to you. This new integration allows you to test and finetune any new model on xTuring without waiting for it to be integrated.
+We are excited to announce the latest enhancements to our `xTuring` library:
+1. __`Falcon LLM` integration__ - You can use and fine-tune the _`Falcon-7B`_ model in different configurations: _off-the-shelf_, _off-the-shelf with INT8 precision_, _LoRA fine-tuning_, and _LoRA fine-tuning with INT8 precision_.
+2. __`GenericModel` wrapper__ - This new integration allows you to test and fine-tune any new model on `xTuring` without waiting for it to be integrated using class _`GenericModel`_.
 
 You can check the  [Falcon LoRA INT8 working example](examples/falcon/falcon_lora_int8.py) repository to see how it works.
 Also, you can check the  [GenericModel working example](examples/generic/generic_model.py) repository to see how it works.
 
 <br>
 
-## CLI playground
-<img src=".github/cli-playground.gif" width="100%" style="margin: 0 1%;"/>
-
-## UI playground
-<img src=".github/ui-playground2.gif" width="100%" style="margin: 0 1%;"/>
-
-<br>
-
 ## ⚙️ Installation
 ```bash
 pip install xturing
 ```
 
 <br>
 
@@ -76,14 +70,43 @@
 print("Generated output by the model: {}".format(output))
 ```
 
 You can find the data folder [here](examples/llama/alpaca_data).
 
 <br>
 
+## CLI playground
+<img src=".github/cli-playground.gif" width="80%" style="margin: 0 1%;"/>
+
+```bash
+$ xturing chat -m "<path-to-model-folder>"
+
+```
+
+## UI playground
+<img src=".github/ui-playground2.gif" width="80%" style="margin: 0 1%;"/>
+
+```python
+from xturing.datasets import InstructionDataset
+from xturing.models import BaseModel
+from xturing.ui import Playground
+
+dataset = InstructionDataset("./alpaca_data")
+model = BaseModel.create("<model_name>")
+
+model.finetune(dataset=dataset)
+
+model.save("llama_lora_finetuned")
+
+Playground().launch() ## launches localhost UI
+
+```
+
+<br>
+
 ## 📚 Tutorials
 - [Preparing your dataset](examples/llama/preparing_your_dataset.py)
 - [Cerebras-GPT fine-tuning with LoRA and INT8](examples/cerebras/cerebras_lora_int8.ipynb) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eKq3oF7dnK8KuIfsTE70Gvvniwr1O9D0?usp=sharing)
 - [Cerebras-GPT fine-tuning with LoRA](examples/cerebras/cerebras_lora.ipynb) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VjqQhstm5pT4EjPjx4Je7b3W2X1V3vDo?usp=sharing)
 - [LLaMA fine-tuning with LoRA and INT8](examples/llama/llama_lora_int8.py) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1SQUXq1AMZPSLD4mk3A3swUIc6Y2dclme?usp=sharing)
 - [LLaMA fine-tuning with LoRA](examples/llama/llama_lora.py)
 - [LLaMA fine-tuning](examples/llama/llama.py)
@@ -106,19 +129,19 @@
 ```javascript
 {
   'maximum sequence length': 512,
   'batch size': 1,
 }
 ```
 
-|      LLaMA 7B      | DeepSpeed + CPU Offloading | LoRA + DeepSpeed  | LoRA + DeepSpeed + CPU Offloading |
-| --------- | ---- | ---- | ---- |
+|      LLaMA-7B      | DeepSpeed + CPU Offloading | LoRA + DeepSpeed  | LoRA + DeepSpeed + CPU Offloading |
+| :---------: | :----: | :----: | :----: |
 | GPU | 33.5 GB | 23.7 GB | 21.9 GB |
 | CPU | 190 GB  | 10.2 GB | 14.9 GB |
-| Time per epoch | 21 hours  | 20 mins | 20 mins |
+| Time/epoch | 21 hours  | 20 mins | 20 mins |
 
 Contribute to this by submitting your performance results on other GPUs by creating an issue with your hardware specifications, memory consumption and time per epoch.
 
 <br>
 
 ## 📎 Fine-tuned model checkpoints
 We have already fine-tuned some models that you can use as your base or start playing with.
@@ -133,25 +156,27 @@
 |---------------------|--------|---------------|
 | DistilGPT-2 LoRA | alpaca | `x/distilgpt2_lora_finetuned_alpaca` |
 | LLaMA LoRA          | alpaca | `x/llama_lora_finetuned_alpaca` |
 
 <br>
 
 ## 📈 Roadmap
-- [x] Support for LLaMA, GPT-J, GPT-2, OPT, Cerebras-GPT, Galactica and Bloom models
+- [x] Support for `LLaMA`, `GPT-J`, `GPT-2`, `OPT`, `Cerebras-GPT`, `Galactica` and `Bloom` models
 - [x] Dataset generation using self-instruction
 - [x] Low-precision LoRA fine-tuning and unsupervised fine-tuning
 - [x] INT8 low-precision fine-tuning support
 - [x] OpenAI, Cohere and AI21 Studio model APIs for dataset generation
 - [x] Added fine-tuned checkpoints for some models to the hub
 - [x] INT4 LLaMA LoRA fine-tuning demo
 - [x] INT4 LLaMA LoRA fine-tuning with INT4 generation
-- [x] Support for a generic model wrapper
-- [x] Support for Falcon-7B model
+- [x] Support for a `Generic model` wrapper
+- [x] Support for `Falcon-7B` model
+- [X] INT4 low-precision fine-tuning support
 - [ ] Evaluation of LLM models
+- [ ] INT3, INT2, INT1 low-precision fine-tuning support
 - [ ] Support for Stable Diffusion
 
 <br>
 
 ## 🤝 Help and Support
 If you have any questions, you can create an issue on this repository.
```

#### html2text {}

```diff
@@ -13,36 +13,38 @@
 `xTuring` you can, - Ingest data from different sources and preprocess them to
 a format LLMs can understand - Scale from single to multiple GPUs for faster
 fine-tuning - Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning)
 to reduce hardware costs by up to 90% - Explore different fine-tuning methods
 and benchmark them to find the best performing model - Evaluate fine-tuned
 models on well-defined metrics for in-depth analysis
 ## ð What's new? We are excited to announce the latest enhancements to our
-`xTuring` library: Falcon LLM integration and Generic model support. With this
-update, you can use and finetune Falcon-7B model with the off-the-shelf, off-
-the-shelf with INT8 precision, with LoRA architecture, and LoRA architecture
-with INT8 precision. Moreover, in case you do not find a model you want to run
-in the models' list, you can still us `xTuring` to run with the new
-`GenericModel` wrapper available to you. This new integration allows you to
-test and finetune any new model on xTuring without waiting for it to be
-integrated. You can check the [Falcon LoRA INT8 working example](examples/
-falcon/falcon_lora_int8.py) repository to see how it works. Also, you can check
-the [GenericModel working example](examples/generic/generic_model.py)
-repository to see how it works.
-## CLI playground [.github/cli-playground.gif] ## UI playground [.github/ui-
-playground2.gif]
+`xTuring` library: 1. __`Falcon LLM` integration__ - You can use and fine-tune
+the _`Falcon-7B`_ model in different configurations: _off-the-shelf_, _off-the-
+shelf with INT8 precision_, _LoRA fine-tuning_, and _LoRA fine-tuning with INT8
+precision_. 2. __`GenericModel` wrapper__ - This new integration allows you to
+test and fine-tune any new model on `xTuring` without waiting for it to be
+integrated using class _`GenericModel`_. You can check the [Falcon LoRA INT8
+working example](examples/falcon/falcon_lora_int8.py) repository to see how it
+works. Also, you can check the [GenericModel working example](examples/generic/
+generic_model.py) repository to see how it works.
 ## âï¸ Installation ```bash pip install xturing ```
 ## ð Quickstart ```python from xturing.datasets import InstructionDataset
 from xturing.models import BaseModel # Load the dataset instruction_dataset =
 InstructionDataset("./alpaca_data") # Initialize the model model =
 BaseModel.create("llama_lora") # Finetune the model model.finetune
 (dataset=instruction_dataset) # Perform inference output = model.generate
 (texts=["Why LLM models are becoming so important?"]) print("Generated output
 by the model: {}".format(output)) ``` You can find the data folder [here]
 (examples/llama/alpaca_data).
+## CLI playground [.github/cli-playground.gif] ```bash $ xturing chat -m "" ```
+## UI playground [.github/ui-playground2.gif] ```python from xturing.datasets
+import InstructionDataset from xturing.models import BaseModel from xturing.ui
+import Playground dataset = InstructionDataset("./alpaca_data") model =
+BaseModel.create("") model.finetune(dataset=dataset) model.save
+("llama_lora_finetuned") Playground().launch() ## launches localhost UI ```
 ## ð Tutorials - [Preparing your dataset](examples/llama/
 preparing_your_dataset.py) - [Cerebras-GPT fine-tuning with LoRA and INT8]
 (examples/cerebras/cerebras_lora_int8.ipynb) &ensp; [![Open in Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1eKq3oF7dnK8KuIfsTE70Gvvniwr1O9D0?usp=sharing)
 - [Cerebras-GPT fine-tuning with LoRA](examples/cerebras/cerebras_lora.ipynb)
 &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-
@@ -60,37 +62,38 @@
 tuning with LoRA](examples/gpt2/gpt2_lora.py) &ensp; [![Open in Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/
 file/d/1Sh-ocNpKn9pS7jv6oBb_Q8DitFyj1avL/view?usp=sharing)
 ## ð Performance Here is a comparison for the performance of different fine-
 tuning techniques on the LLaMA 7B model. We use the [Alpaca dataset](examples/
 llama/alpaca_data/) for fine-tuning. The dataset contains 52K instructions.
 Hardware: 4xA100 40GB GPU, 335GB CPU RAM Fine-tuning parameters: ```javascript
-{ 'maximum sequence length': 512, 'batch size': 1, } ``` | LLaMA 7B | DeepSpeed
-+ CPU Offloading | LoRA + DeepSpeed | LoRA + DeepSpeed + CPU Offloading | | ---
------- | ---- | ---- | ---- | | GPU | 33.5 GB | 23.7 GB | 21.9 GB | | CPU | 190
-GB | 10.2 GB | 14.9 GB | | Time per epoch | 21 hours | 20 mins | 20 mins |
-Contribute to this by submitting your performance results on other GPUs by
+{ 'maximum sequence length': 512, 'batch size': 1, } ``` | LLaMA-7B | DeepSpeed
++ CPU Offloading | LoRA + DeepSpeed | LoRA + DeepSpeed + CPU Offloading | | :--
+-------: | :----: | :----: | :----: | | GPU | 33.5 GB | 23.7 GB | 21.9 GB | |
+CPU | 190 GB | 10.2 GB | 14.9 GB | | Time/epoch | 21 hours | 20 mins | 20 mins
+| Contribute to this by submitting your performance results on other GPUs by
 creating an issue with your hardware specifications, memory consumption and
 time per epoch.
 ## ð Fine-tuned model checkpoints We have already fine-tuned some models
 that you can use as your base or start playing with. Here is how you would load
 them: ```python from xturing.models import BaseModel model = BaseModel.load("x/
 distilgpt2_lora_finetuned_alpaca") ``` | model | dataset | Path | |------------
 ---------|--------|---------------| | DistilGPT-2 LoRA | alpaca | `x/
 distilgpt2_lora_finetuned_alpaca` | | LLaMA LoRA | alpaca | `x/
 llama_lora_finetuned_alpaca` |
-## ð Roadmap - [x] Support for LLaMA, GPT-J, GPT-2, OPT, Cerebras-GPT,
-Galactica and Bloom models - [x] Dataset generation using self-instruction -
-[x] Low-precision LoRA fine-tuning and unsupervised fine-tuning - [x] INT8 low-
-precision fine-tuning support - [x] OpenAI, Cohere and AI21 Studio model APIs
-for dataset generation - [x] Added fine-tuned checkpoints for some models to
-the hub - [x] INT4 LLaMA LoRA fine-tuning demo - [x] INT4 LLaMA LoRA fine-
-tuning with INT4 generation - [x] Support for a generic model wrapper - [x]
-Support for Falcon-7B model - [ ] Evaluation of LLM models - [ ] Support for
-Stable Diffusion
+## ð Roadmap - [x] Support for `LLaMA`, `GPT-J`, `GPT-2`, `OPT`, `Cerebras-
+GPT`, `Galactica` and `Bloom` models - [x] Dataset generation using self-
+instruction - [x] Low-precision LoRA fine-tuning and unsupervised fine-tuning -
+[x] INT8 low-precision fine-tuning support - [x] OpenAI, Cohere and AI21 Studio
+model APIs for dataset generation - [x] Added fine-tuned checkpoints for some
+models to the hub - [x] INT4 LLaMA LoRA fine-tuning demo - [x] INT4 LLaMA LoRA
+fine-tuning with INT4 generation - [x] Support for a `Generic model` wrapper -
+[x] Support for `Falcon-7B` model - [X] INT4 low-precision fine-tuning support
+- [ ] Evaluation of LLM models - [ ] INT3, INT2, INT1 low-precision fine-tuning
+support - [ ] Support for Stable Diffusion
 ## ð¤ Help and Support If you have any questions, you can create an issue on
 this repository. You can also join our [Discord server](https://discord.gg/
 TgHXuSJEk6) and start a discussion in the `#xturing` channel.
 ## ð License This project is licensed under the Apache License 2.0 - see the
 [LICENSE](LICENSE) file for details.
 ## ð Contributing As an open source project in a rapidly evolving field, we
 welcome contributions of all kinds, including new features and better
```

### Comparing `xturing-0.1.5/pyproject.toml` & `xturing-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xturing"
-version = "0.1.5"
+version = "0.1.6"
 description = "Fine-tuning, evaluation and data generation for LLMs"
 
 authors = [
     { name = "Glenn Ko", email = "glenn@stochastic.ai" },
     { name = "Yuji Chai", email = "yuji.chai@stochastic.ai" },
     { name = "Roman Ageev", email = "roman.ageev@stochastic.ai" },
     { name = "Toan Do", email = "toan.do@stochastic.ai" },
```

### Comparing `xturing-0.1.5/src/xturing/cli/__init__.py` & `xturing-0.1.6/src/xturing/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/cli/api.py` & `xturing-0.1.6/src/xturing/cli/api.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/cli/chat.py` & `xturing-0.1.6/src/xturing/cli/chat.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/config/__init__.py` & `xturing-0.1.6/src/xturing/config/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/config/config_data_classes.py` & `xturing-0.1.6/src/xturing/config/config_data_classes.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/config/finetuning_config.yaml` & `xturing-0.1.6/src/xturing/config/finetuning_config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -10,88 +10,95 @@
   num_train_epochs: 1
   logging_steps: 10
   max_grad_norm: 2.0
   save_total_limit: 4
   optimizer_name: adamw
   output_dir: saved_model
 
-llama:
+bloom:
   learning_rate: 5e-5
   weight_decay: 0.01
   num_train_epochs: 3
-  optimizer_name: cpu_adam
-
-llama_lora:
-  learning_rate: 1e-4
-  weight_decay: 0.01
-  num_train_epochs: 3
-  batch_size: 1
 
-llama_lora_int8:
+bloom_lora:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
-  batch_size: 8
-  max_length: 256
+  batch_size: 4
 
-llama_lora_int4:
+bloom_lora_int8:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 8
   max_length: 256
 
-gptj:
+cerebras:
   learning_rate: 5e-5
   weight_decay: 0.01
   num_train_epochs: 3
-  optimizer_name: cpu_adam
 
-gptj_lora:
+cerebras_lora:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
-  batch_size: 1
+  batch_size: 4
 
-gptj_lora_int8:
+cerebras_lora_int8:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 8
   max_length: 256
 
-gpt2:
+distilgpt2:
   learning_rate: 1e-3
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 8
 
-gpt2_lora:
+distilgpt2_lora:
   learning_rate: 3e-3
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 16
 
-gpt2_lora_int8:
-  learning_rate: 3e-3
+falcon:
+  learning_rate: 5e-5
   weight_decay: 0.01
   num_train_epochs: 3
-  batch_size: 16
+  batch_size: 1
+  max_length: 256
 
-distilgpt2:
-  learning_rate: 1e-3
+falcon_int8:
+  learning_rate: 1e-4
+  weight_decay: 0.01
+  num_train_epochs: 3
+  batch_size: 1
+  max_length: 256
+
+falcon_lora:
+  learning_rate: 1e-4
+  weight_decay: 0.01
+  num_train_epochs: 3
+  batch_size: 1
+
+falcon_lora_int8:
+  learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 8
+  max_length: 256
 
-distilgpt2_lora:
-  learning_rate: 3e-3
+falcon_lora_kbit:
+  learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
-  batch_size: 16
+  batch_size: 8
+  max_length: 256
 
 galactica:
   learning_rate: 5e-5
   weight_decay: 0.01
   num_train_epochs: 3
   optimizer_name: cpu_adam
 
@@ -104,115 +111,136 @@
 galactica_lora_int8:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 8
   max_length: 256
 
-opt:
-  learning_rate: 5e-5
-  weight_decay: 0.01
-  num_train_epochs: 3
-
-opt_lora:
+generic:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
-  batch_size: 1
+  batch_size: 8
+  max_length: 256
 
-opt_lora_int8:
+generic_int8:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 8
   max_length: 256
 
-cerebras:
-  learning_rate: 5e-5
+generic_lora:
+  learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
+  batch_size: 8
+  max_length: 256
 
-cerebras_lora:
+generic_lora_int8:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
-  batch_size: 4
+  batch_size: 8
+  max_length: 256
 
-cerebras_lora_int8:
+generic_lora_kbit:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 8
   max_length: 256
 
-bloom:
+gptj:
   learning_rate: 5e-5
   weight_decay: 0.01
   num_train_epochs: 3
+  optimizer_name: cpu_adam
 
-bloom_lora:
+gptj_lora:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
-  batch_size: 4
+  batch_size: 1
 
-bloom_lora_int8:
+gptj_lora_int8:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 8
   max_length: 256
 
-generic:
-  learning_rate: 1e-4
+gpt2:
+  learning_rate: 1e-3
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 8
-  max_length: 256
 
-generic_int8:
-  learning_rate: 1e-4
+gpt2_lora:
+  learning_rate: 3e-3
   weight_decay: 0.01
   num_train_epochs: 3
-  batch_size: 8
-  max_length: 256
+  batch_size: 16
 
-generic_int8_lora:
+gpt2_lora_int8:
+  learning_rate: 3e-3
+  weight_decay: 0.01
+  num_train_epochs: 3
+  batch_size: 16
+
+llama:
+  learning_rate: 5e-5
+  weight_decay: 0.01
+  num_train_epochs: 3
+  optimizer_name: cpu_adam
+
+llama_lora:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
-  batch_size: 8
-  max_length: 256
+  batch_size: 1
 
-generic_lora:
+llama_lora_int8:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 8
   max_length: 256
-  
-falcon:
-  learning_rate: 5e-5
-  weight_decay: 0.01
+
+llama_lora_kbit:
+  learning_rate: 3e-4
   num_train_epochs: 3
   batch_size: 1
   max_length: 256
+  lora_r: 32
+  lora_alpha: 128
+  lora_groupsize: 128
+  lora_dropout: 0.05
+  seed: 0
+  cache: False
+  seqlen: 2048
+  kl_weight: 1.0
+  ce_weight: 200.0
+  save_freq: 1
+  trainable_kl_weight: False
+  trainable_ce_weight: False
+  weight_decay: 1e-5
+  intra_save_freq: 200
+  groupsize: 128
 
-falcon_int8:
-  learning_rate: 1e-4
+opt:
+  learning_rate: 5e-5
   weight_decay: 0.01
   num_train_epochs: 3
-  batch_size: 1
-  max_length: 256
 
-falcon_lora:
+opt_lora:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 1
 
-falcon_lora_int8:
+opt_lora_int8:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 8
   max_length: 256
```

### Comparing `xturing-0.1.5/src/xturing/config/generation_config.yaml` & `xturing-0.1.6/src/xturing/config/generation_config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -3,92 +3,89 @@
 
 
 # Contrastive search
 defaults:
   max_new_tokens: 256
 
 # Contrastive search
-llama:
+bloom:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
 
 # Contrastive search
-llama_lora:
+bloom_lora:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
 
 # Greedy search
-llama_lora_int8:
-  max_new_tokens: 256
-  do_sample: false
-
-# Contrastive search
-llama_lora_int4:
-  penalty_alpha: 0.6
-  top_k: 4
+bloom_lora_int8:
   max_new_tokens: 256
   do_sample: false
 
 # Contrastive search
-gptj:
+cerebras:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
 
 # Contrastive search
-gptj_lora:
+cerebras_lora:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
 
 # Greedy search
-gptj_lora_int8:
+cerebras_lora_int8:
   max_new_tokens: 256
   do_sample: false
 
 # Top-p sampling
-gpt2:
+distilgpt2:
   do_sample: true
   top_k: 0
   top_p: 0.92
   max_new_tokens: 256
 
 # Top-p sampling
-gpt2_lora:
+distilgpt2_lora:
   do_sample: true
   top_k: 0
   top_p: 0.92
   max_new_tokens: 256
 
-# Top-p sampling
-gpt2_lora_int8:
-  do_sample: true
-  top_k: 0
-  top_p: 0.92
+# Greedy search
+falcon:
   max_new_tokens: 256
+  do_sample: false
 
-# Top-p sampling
-distilgpt2:
-  do_sample: true
-  top_k: 0
-  top_p: 0.92
+# Greedy search
+falcon_int8:
   max_new_tokens: 256
+  do_sample: false
 
-# Top-p sampling
-distilgpt2_lora:
-  do_sample: true
-  top_k: 0
-  top_p: 0.92
+# Greedy search
+falcon_lora:
   max_new_tokens: 256
+  do_sample: false
+
+# Greedy search
+falcon_lora_int8:
+  max_new_tokens: 256
+  do_sample: false
+
+# Greedy search
+falcon_lora_kbit:
+  max_new_tokens: 256
+  do_sample: false
 
 # Contrastive search
 galactica:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
@@ -101,104 +98,114 @@
   do_sample: false
 
 # Greedy search
 galactica_lora_int8:
   max_new_tokens: 256
   do_sample: false
 
-# Contrastive search
-opt:
-  penalty_alpha: 0.6
-  top_k: 4
-  max_new_tokens: 256
-  do_sample: false
-
-# Contrastive search
-opt_lora:
-  penalty_alpha: 0.6
-  top_k: 4
+# Greedy search
+generic:
   max_new_tokens: 256
   do_sample: false
 
 # Greedy search
-opt_lora_int8:
+generic_int8:
   max_new_tokens: 256
   do_sample: false
 
-# Contrastive search
-cerebras:
-  penalty_alpha: 0.6
-  top_k: 4
+# Greedy search
+generic_lora:
   max_new_tokens: 256
   do_sample: false
 
-# Contrastive search
-cerebras_lora:
-  penalty_alpha: 0.6
-  top_k: 4
+# Greedy search
+generic_lora_int8:
   max_new_tokens: 256
   do_sample: false
 
 # Greedy search
-cerebras_lora_int8:
+generic_lora_kbit:
   max_new_tokens: 256
   do_sample: false
 
 # Contrastive search
-bloom:
+gptj:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
 
 # Contrastive search
-bloom_lora:
+gptj_lora:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
 
 # Greedy search
-bloom_lora_int8:
+gptj_lora_int8:
   max_new_tokens: 256
   do_sample: false
 
-# Greedy search
-generic:
+# Top-p sampling
+gpt2:
+  do_sample: true
+  top_k: 0
+  top_p: 0.92
   max_new_tokens: 256
-  do_sample: false
 
-# Greedy search
-generic_int8:
+# Top-p sampling
+gpt2_lora:
+  do_sample: true
+  top_k: 0
+  top_p: 0.92
   max_new_tokens: 256
-  do_sample: false
 
-# Greedy search
-generic_lora:
+# Top-p sampling
+gpt2_lora_int8:
+  do_sample: true
+  top_k: 0
+  top_p: 0.92
+  max_new_tokens: 256
+
+# Contrastive search
+llama:
+  penalty_alpha: 0.6
+  top_k: 4
   max_new_tokens: 256
   do_sample: false
 
+# Contrastive search
+llama_lora:
+  penalty_alpha: 0.6
+  top_k: 4
+  max_new_tokens: 256
+  do_sample: false
 
 # Greedy search
-generic_lora_int8:
+llama_lora_int8:
   max_new_tokens: 256
   do_sample: false
 
 # Greedy search
-falcon:
+llama_lora_kbit:
   max_new_tokens: 256
   do_sample: false
 
-# Greedy search
-falcon_lora:
+# Contrastive search
+opt:
+  penalty_alpha: 0.6
+  top_k: 4
   max_new_tokens: 256
   do_sample: false
 
-# Greedy search
-falcon_int8:
+# Contrastive search
+opt_lora:
+  penalty_alpha: 0.6
+  top_k: 4
   max_new_tokens: 256
   do_sample: false
 
 # Greedy search
-falcon_lora_int8:
+opt_lora_int8:
   max_new_tokens: 256
   do_sample: false
```

### Comparing `xturing-0.1.5/src/xturing/config/read_config.py` & `xturing-0.1.6/src/xturing/config/read_config.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/datasets/instruction_dataset.py` & `xturing-0.1.6/src/xturing/datasets/instruction_dataset.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/datasets/text_dataset.py` & `xturing-0.1.6/src/xturing/datasets/text_dataset.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/engines/__init__.py` & `xturing-0.1.6/src/xturing/engines/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,70 +13,74 @@
 )
 from .distilgpt2_engine import DistilGPT2Engine, DistilGPT2LoraEngine
 from .falcon_engine import (
     FalconEngine,
     FalconInt8Engine,
     FalconLoraEngine,
     FalconLoraInt8Engine,
+    FalconLoraKbitEngine,
 )
 from .galactica_engine import (
     GalacticaEngine,
     GalacticaInt8Engine,
     GalacticaLoraEngine,
     GalacticaLoraInt8Engine,
 )
 from .generic_engine import (
     GenericEngine,
     GenericInt8Engine,
     GenericLoraEngine,
     GenericLoraInt8Engine,
+    GenericLoraKbitEngine,
 )
 from .gpt2_engine import GPT2Engine, GPT2Int8Engine, GPT2LoraEngine, GPT2LoraInt8Engine
 from .gptj_engine import GPTJEngine, GPTJInt8Engine, GPTJLoraEngine, GPTJLoraInt8Engine
 from .llama_engine import (
     LLamaEngine,
     LLamaInt8Engine,
     LlamaLoraEngine,
-    LlamaLoraInt4Engine,
     LlamaLoraInt8Engine,
+    LlamaLoraKbitEngine,
 )
 from .opt_engine import OPTEngine, OPTInt8Engine, OPTLoraEngine, OPTLoraInt8Engine
 
+BaseEngine.add_to_registry(BloomEngine.config_name, BloomEngine)
+BaseEngine.add_to_registry(BloomInt8Engine.config_name, BloomInt8Engine)
+BaseEngine.add_to_registry(BloomLoraEngine.config_name, BloomLoraEngine)
+BaseEngine.add_to_registry(BloomLoraInt8Engine.config_name, BloomLoraInt8Engine)
+BaseEngine.add_to_registry(CerebrasEngine.config_name, CerebrasEngine)
+BaseEngine.add_to_registry(CerebrasInt8Engine.config_name, CerebrasInt8Engine)
+BaseEngine.add_to_registry(CerebrasLoraEngine.config_name, CerebrasLoraEngine)
+BaseEngine.add_to_registry(CerebrasLoraInt8Engine.config_name, CerebrasLoraInt8Engine)
 BaseEngine.add_to_registry(DistilGPT2Engine.config_name, DistilGPT2Engine)
 BaseEngine.add_to_registry(DistilGPT2LoraEngine.config_name, DistilGPT2LoraEngine)
+BaseEngine.add_to_registry(FalconEngine.config_name, FalconEngine)
+BaseEngine.add_to_registry(FalconInt8Engine.config_name, FalconInt8Engine)
+BaseEngine.add_to_registry(FalconLoraEngine.config_name, FalconLoraEngine)
+BaseEngine.add_to_registry(FalconLoraInt8Engine.config_name, FalconLoraInt8Engine)
+BaseEngine.add_to_registry(FalconLoraKbitEngine.config_name, FalconLoraKbitEngine)
+BaseEngine.add_to_registry(GalacticaEngine.config_name, GalacticaEngine)
+BaseEngine.add_to_registry(GalacticaInt8Engine.config_name, GalacticaInt8Engine)
+BaseEngine.add_to_registry(GalacticaLoraEngine.config_name, GalacticaLoraEngine)
+BaseEngine.add_to_registry(GalacticaLoraInt8Engine.config_name, GalacticaLoraInt8Engine)
+BaseEngine.add_to_registry(GenericEngine.config_name, GenericEngine)
+BaseEngine.add_to_registry(GenericInt8Engine.config_name, GenericInt8Engine)
+BaseEngine.add_to_registry(GenericLoraEngine.config_name, GenericLoraEngine)
+BaseEngine.add_to_registry(GenericLoraInt8Engine.config_name, GenericLoraInt8Engine)
+BaseEngine.add_to_registry(GenericLoraKbitEngine.config_name, GenericLoraKbitEngine)
 BaseEngine.add_to_registry(GPTJEngine.config_name, GPTJEngine)
-BaseEngine.add_to_registry(GPTJLoraEngine.config_name, GPTJLoraEngine)
 BaseEngine.add_to_registry(GPTJInt8Engine.config_name, GPTJInt8Engine)
+BaseEngine.add_to_registry(GPTJLoraEngine.config_name, GPTJLoraEngine)
 BaseEngine.add_to_registry(GPTJLoraInt8Engine.config_name, GPTJLoraInt8Engine)
 BaseEngine.add_to_registry(GPT2Engine.config_name, GPT2Engine)
-BaseEngine.add_to_registry(GPT2LoraEngine.config_name, GPT2LoraEngine)
 BaseEngine.add_to_registry(GPT2Int8Engine.config_name, GPT2Int8Engine)
+BaseEngine.add_to_registry(GPT2LoraEngine.config_name, GPT2LoraEngine)
 BaseEngine.add_to_registry(GPT2LoraInt8Engine.config_name, GPT2LoraInt8Engine)
 BaseEngine.add_to_registry(LLamaEngine.config_name, LLamaEngine)
-BaseEngine.add_to_registry(LlamaLoraEngine.config_name, LlamaLoraEngine)
 BaseEngine.add_to_registry(LLamaInt8Engine.config_name, LLamaInt8Engine)
+BaseEngine.add_to_registry(LlamaLoraEngine.config_name, LlamaLoraEngine)
 BaseEngine.add_to_registry(LlamaLoraInt8Engine.config_name, LlamaLoraInt8Engine)
-BaseEngine.add_to_registry(LlamaLoraInt4Engine.config_name, LlamaLoraInt4Engine)
-BaseEngine.add_to_registry(GalacticaEngine.config_name, GalacticaEngine)
-BaseEngine.add_to_registry(GalacticaInt8Engine.config_name, GalacticaInt8Engine)
-BaseEngine.add_to_registry(GalacticaLoraEngine.config_name, GalacticaLoraEngine)
-BaseEngine.add_to_registry(GalacticaLoraInt8Engine.config_name, GalacticaLoraInt8Engine)
+BaseEngine.add_to_registry(LlamaLoraKbitEngine.config_name, LlamaLoraKbitEngine)
 BaseEngine.add_to_registry(OPTEngine.config_name, OPTEngine)
-BaseEngine.add_to_registry(OPTLoraEngine.config_name, OPTLoraEngine)
 BaseEngine.add_to_registry(OPTInt8Engine.config_name, OPTInt8Engine)
+BaseEngine.add_to_registry(OPTLoraEngine.config_name, OPTLoraEngine)
 BaseEngine.add_to_registry(OPTLoraInt8Engine.config_name, OPTLoraInt8Engine)
-BaseEngine.add_to_registry(CerebrasEngine.config_name, CerebrasEngine)
-BaseEngine.add_to_registry(CerebrasLoraEngine.config_name, CerebrasLoraEngine)
-BaseEngine.add_to_registry(CerebrasInt8Engine.config_name, CerebrasInt8Engine)
-BaseEngine.add_to_registry(CerebrasLoraInt8Engine.config_name, CerebrasLoraInt8Engine)
-BaseEngine.add_to_registry(BloomEngine.config_name, BloomEngine)
-BaseEngine.add_to_registry(BloomLoraEngine.config_name, BloomLoraEngine)
-BaseEngine.add_to_registry(BloomInt8Engine.config_name, BloomInt8Engine)
-BaseEngine.add_to_registry(BloomLoraInt8Engine.config_name, BloomLoraInt8Engine)
-BaseEngine.add_to_registry(GenericEngine.config_name, GenericEngine)
-BaseEngine.add_to_registry(GenericInt8Engine.config_name, GenericInt8Engine)
-BaseEngine.add_to_registry(GenericLoraEngine.config_name, GenericLoraEngine)
-BaseEngine.add_to_registry(GenericLoraInt8Engine.config_name, GenericLoraInt8Engine)
-BaseEngine.add_to_registry(FalconEngine.config_name, FalconEngine)
-BaseEngine.add_to_registry(FalconLoraEngine.config_name, FalconLoraEngine)
-BaseEngine.add_to_registry(FalconInt8Engine.config_name, FalconInt8Engine)
-BaseEngine.add_to_registry(FalconLoraInt8Engine.config_name, FalconLoraInt8Engine)
```

### Comparing `xturing-0.1.5/src/xturing/engines/bloom_engine.py` & `xturing-0.1.6/src/xturing/engines/bloom_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/engines/causal.py` & `xturing-0.1.6/src/xturing/engines/causal.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,27 +13,30 @@
 )
 from xturing.engines.base import BaseEngine
 from xturing.engines.lora_engine import (
     LoraConfig,
     LoraModel,
     prepare_model_for_int8_training,
 )
+from xturing.engines.quant_utils.peft_utils import LoraConfig as peftLoraConfig
+from xturing.engines.quant_utils.peft_utils import prepare_model_for_kbit_training
 from xturing.utils.loss_fns import CrossEntropyLoss
 
 
 class CausalEngine(BaseEngine):
     def __init__(
         self,
         *,
         model_name: Optional[str] = None,
         weights_path: Optional[Union[str, Path]] = None,
         model: Optional[Any] = None,
         tokenizer: Optional[Any] = None,
         load_8bit: Optional[bool] = False,
         trust_remote_code: Optional[bool] = False,
+        **kwargs,
     ):
         self.model_name = model_name
 
         if weights_path is not None:
             assert Path(
                 weights_path
             ).is_dir(), "The weights path should be a existing directory"
@@ -41,42 +44,45 @@
                 device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
                 self.model = AutoModelForCausalLM.from_pretrained(
                     weights_path,
                     torch_dtype=DEFAULT_DTYPE,
                     load_in_8bit=True,
                     device_map=device_map,
                     trust_remote_code=trust_remote_code,
+                    **kwargs,
                 )
                 self.model = prepare_model_for_int8_training(self.model)
             else:
                 self.model = AutoModelForCausalLM.from_pretrained(
-                    weights_path, torch_dtype=DEFAULT_DTYPE
+                    weights_path, torch_dtype=DEFAULT_DTYPE, **kwargs
                 )
             self.tokenizer = AutoTokenizer.from_pretrained(weights_path)
         elif model is not None and tokenizer is not None:
             self.model = model
             self.tokenizer = tokenizer
         elif model_name is not None:
             if load_8bit:
                 device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
                 self.model = AutoModelForCausalLM.from_pretrained(
                     model_name,
                     torch_dtype=DEFAULT_DTYPE,
                     load_in_8bit=True,
                     device_map=device_map,
                     trust_remote_code=trust_remote_code,
+                    **kwargs,
                 )
                 for param in self.model.parameters():
                     param.data = param.data.contiguous()
                 self.model = prepare_model_for_int8_training(self.model)
             else:
                 self.model = AutoModelForCausalLM.from_pretrained(
                     model_name,
                     torch_dtype=DEFAULT_DTYPE,
                     trust_remote_code=trust_remote_code,
+                    **kwargs,
                 )
             self.tokenizer = AutoTokenizer.from_pretrained(model_name)
         else:
             raise ValueError(
                 "Please provide a model_name, the weights path or model and tokenizer."
             )
 
@@ -193,7 +199,75 @@
 
         torch.save(self.model.state_dict(), model_weights)
         # save adapter
         self.model.save_pretrained(saving_path)
 
         # Save tokenizer
         self.tokenizer.save_pretrained(saving_path)
+
+
+class CausalLoraKbitEngine(CausalEngine):
+    def __init__(
+        self,
+        *,
+        model_name: Optional[str] = None,
+        weights_path: Optional[Union[str, Path]] = None,
+        model: Optional[Any] = None,
+        tokenizer: Optional[Any] = None,
+        target_modules: Optional[Union[List[str], str]] = None,
+        trust_remote_code: Optional[bool] = False,
+    ):
+        if model is None:
+            device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
+            model = AutoModelForCausalLM.from_pretrained(
+                model_name,
+                torch_dtype=DEFAULT_DTYPE,
+                device_map=device_map,
+                load_in_4bit=True,
+                trust_remote_code=trust_remote_code,
+            )
+
+            model = prepare_model_for_kbit_training(model)
+
+        if tokenizer is None:
+            tokenizer = AutoTokenizer.from_pretrained(model_name)
+
+        super().__init__(
+            model_name=model_name,
+            weights_path=None,
+            model=model,
+            tokenizer=tokenizer,
+        )
+
+        self.print_trainable_parameters()
+
+        self.loss_fct = CrossEntropyLoss()
+
+    def set_from_state_dict(self, state_dict, strict=False):
+        self.model.load_state_dict(state_dict, strict=strict)
+
+    def save(self, saving_path: Union[str, Path]):
+        # Save HF config file
+        self.model.config.save_pretrained(str(saving_path))
+        # Save model weights
+        model_weights = str(Path(saving_path).resolve() / "pytorch_model.bin")
+
+        torch.save(self.model.state_dict(), model_weights)
+        # save adapter
+        self.model.save_pretrained(saving_path)
+
+        # Save tokenizer
+        self.tokenizer.save_pretrained(saving_path)
+
+    def print_trainable_parameters(self):
+        """
+        Prints the number of trainable parameters in the model.
+        """
+        trainable_params = 0
+        all_param = 0
+        for _, param in self.model.named_parameters():
+            all_param += param.numel()
+            if param.requires_grad:
+                trainable_params += param.numel()
+        print(
+            f"trainable params: {trainable_params} || all params: {all_param} || trainable%: {100 * trainable_params / all_param}"
+        )
```

### Comparing `xturing-0.1.5/src/xturing/engines/cerebras_engine.py` & `xturing-0.1.6/src/xturing/engines/cerebras_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/engines/distilgpt2_engine.py` & `xturing-0.1.6/src/xturing/engines/distilgpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/engines/falcon_engine.py` & `xturing-0.1.6/src/xturing/engines/falcon_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import Optional, Union
 
-from xturing.engines.causal import CausalEngine, CausalLoraEngine
+from xturing.engines.causal import CausalEngine, CausalLoraEngine, CausalLoraKbitEngine
 
 
 class FalconEngine(CausalEngine):
     config_name: str = "falcon_engine"
 
     def __init__(self, weights_path: Optional[Union[str, Path]] = None):
         super().__init__(
@@ -67,7 +67,29 @@
                 "dense_4h_to_h",
             ],
             trust_remote_code=True,
         )
 
         self.tokenizer.pad_token = self.tokenizer.eos_token
         self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
+
+
+class FalconLoraKbitEngine(CausalLoraKbitEngine):
+    config_name: str = "falcon_lora_kbit_engine"
+
+    def __init__(self, weights_path: Optional[Union[str, Path]] = None):
+        model_name = "tiiuae/falcon-7b"
+        super().__init__(
+            model_name=model_name,
+            weights_path=None,
+            target_modules=[
+                "query_key_value",
+                "dense",
+                "dense_h_to_4h",
+                "dense_4h_to_h",
+            ],
+            trust_remote_code=True,
+            load_4bit=True,
+        )
+
+        self.tokenizer.pad_token = self.tokenizer.eos_token
+        self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
```

### Comparing `xturing-0.1.5/src/xturing/engines/galactica_engine.py` & `xturing-0.1.6/src/xturing/engines/galactica_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/engines/generic_engine.py` & `xturing-0.1.6/src/xturing/engines/generic_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import os
 from pathlib import Path
 from typing import List, Optional, Union
 
-from xturing.engines.causal import CausalEngine, CausalLoraEngine
+from xturing.engines.causal import CausalEngine, CausalLoraEngine, CausalLoraKbitEngine
 
 
 class GenericEngine(CausalEngine):
     config_name: str = "generic_engine"
 
     def __init__(
-        self, model_name: str, weights_path: Optional[Union[str, Path]] = None
+        self, model_name: str, weights_path: Optional[Union[str, Path]] = None, **kwargs
     ):
-        super().__init__(
-            model_name=model_name,
-            weights_path=weights_path,
-        )
+        super().__init__(model_name=model_name, weights_path=weights_path, **kwargs)
 
         self.tokenizer.pad_token = self.tokenizer.eos_token
 
 
 class GenericLoraEngine(CausalLoraEngine):
     config_name: str = "generic_lora_engine"
 
@@ -61,7 +58,26 @@
             model_name=model_name,
             weights_path=weights_path,
             load_8bit=True,
             target_modules=target_modules,
         )
 
         self.tokenizer.pad_token = self.tokenizer.eos_token
+
+
+class GenericLoraKbitEngine(CausalLoraKbitEngine):
+    config_name: str = "generic+lora_kbit_engine"
+
+    def __init__(
+        self,
+        model_name: str,
+        target_modules: List[str],
+        weights_path: Optional[Union[str, Path]] = None,
+    ):
+        super().__init__(
+            model_name=model_name,
+            weights_path=weights_path,
+            load_4bit=True,
+            target_modules=target_modules,
+        )
+
+        self.tokenizer.pad_token = self.tokenizer.eos_token
```

### Comparing `xturing-0.1.5/src/xturing/engines/gpt2_engine.py` & `xturing-0.1.6/src/xturing/engines/gpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/engines/gptj_engine.py` & `xturing-0.1.6/src/xturing/engines/gptj_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/engines/gptj_utils/gptj.py` & `xturing-0.1.6/src/xturing/engines/gptj_utils/gptj.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/engines/llama_engine.py` & `xturing-0.1.6/src/xturing/engines/llama_engine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+import argparse
 import os
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import torch
 import transformers
 from torch import nn
 
-from xturing.engines.causal import CausalEngine, CausalLoraEngine
+from xturing.config.config_data_classes import FinetuningConfig, GenerationConfig
+from xturing.config.read_config import load_config, read_yaml
+from xturing.engines.causal import CausalEngine, CausalLoraEngine, CausalLoraKbitEngine
 from xturing.engines.llama_utils import LlamaConfig, LlamaForCausalLM, LlamaTokenizer
 from xturing.engines.lora_engine import prepare_model_for_int8_training
 from xturing.engines.quant_utils import autotune_warmup, make_quant
+from xturing.engines.quant_utils.lrec import get_c4, prepare_models, train_model
 from xturing.utils.hub import ModelHub
 
 
 class LLamaEngine(CausalEngine):
     config_name: str = "llama_engine"
 
     def __init__(self, weights_path: Optional[Union[str, Path]] = None):
@@ -113,80 +117,57 @@
             find_layers(
                 child, layers=layers, name=name + "." + name1 if name != "" else name1
             )
         )
     return res
 
 
-class LlamaLoraInt4Engine(CausalLoraEngine):
-    config_name: str = "llama_lora_int4_engine"
+class LlamaLoraKbitEngine(CausalLoraKbitEngine):
+    config_name: str = "llama_lora_kbit_engine"
 
     def __init__(self, weights_path: Optional[Union[str, Path]] = None):
         model_name = "decapoda-research/llama-7b-hf"
+        # lrec_config = {
+        #     "base_model": model_name,
+        #     "intq_checkpoint": str(
+        #         Path(__file__).parent / "llama7b-2bit-128g.pt"
+        #     ),  ## how to do this
+        #     "wbits": wbits,
+        #     "lora_target_modules": [
+        #         "q_proj",
+        #         "v_proj",
+        #         "k_proj",
+        #         "o_proj",
+        #         "up_proj",
+        #         "down_proj",
+        #         "gate_proj",
+        #     ],
+        #     # "n_samples": 100,
+        #     # "train_cache_dir": "./train_cache/",
+        #     # "val_cache_dir": "./val_cache/",
+        #     # "ckpt_dir": "./ckpts/",
+        #     # "save_dir": "./save/",
+        # }
+
+        # # Finetuning config
+        # yml_content = read_yaml(
+        #     Path(__file__).parent.parent / "config" / "finetuning_config.yaml",
+        # )
+        # lrec_config.update(yml_content["defaults"])
+        # lrec_config.update(yml_content[self.config_name.replace("_engine", "")])
 
-        if weights_path is None:
-            weights_path = ModelHub().load("x/llama_lora_int4")
+        # model, fp_model = prepare_models(argparse.Namespace(**lrec_config))
 
-        config = LlamaConfig.from_pretrained(model_name)
-
-        saved_kaiming_uniform_ = torch.nn.init.kaiming_uniform_
-        saved_uniform_ = torch.nn.init.uniform_
-        saved_normal_ = torch.nn.init.normal_
-
-        def noop(*args, **kwargs):
-            pass
-
-        torch.nn.init.kaiming_uniform_ = noop
-        torch.nn.init.uniform_ = noop
-        torch.nn.init.normal_ = noop
-
-        torch.set_default_dtype(torch.half)
-        transformers.modeling_utils._init_weights = False
-        torch.set_default_dtype(torch.half)
-        model = LlamaForCausalLM(config)
-        torch.set_default_dtype(torch.float)
-        model = model.eval()
-
-        layers = find_layers(model)
-
-        for name in ["lm_head"]:
-            if name in layers:
-                del layers[name]
-
-        wbits = 4
-        groupsize = 128
-        warmup_autotune = True
-
-        make_quant(model, layers, wbits, groupsize)
-
-        state_dict = torch.load(
-            weights_path / Path("pytorch_model.bin"), map_location="cpu"
-        )
-
-        if warmup_autotune:
-            autotune_warmup(model)
-
-        model.seqlen = 2048
-
-        model.gptq = True
-
-        model.gradient_checkpointing_enable()
-        model.enable_input_require_grads()
+        # # The model before applying LoRA
+        # self.base_model = fp_model
 
         tokenizer = LlamaTokenizer.from_pretrained(model_name, add_bos_token=False)
         tokenizer.pad_token = tokenizer.eos_token
         tokenizer.pad_token_id = tokenizer.eos_token_id
 
         super().__init__(
-            model=model,
+            model_name=model_name,
+            weights_path=None,
             tokenizer=tokenizer,
-            target_modules=[
-                "q_proj",
-                "v_proj",
-            ],
+            target_modules=["q_proj", "v_proj"],
+            load_4bit=True,
         )
-
-        torch.nn.init.kaiming_uniform_ = saved_kaiming_uniform_
-        torch.nn.init.uniform_ = saved_uniform_
-        torch.nn.init.normal_ = saved_normal_
-
-        self.set_from_state_dict(state_dict)
```

### Comparing `xturing-0.1.5/src/xturing/engines/llama_utils/llama.py` & `xturing-0.1.6/src/xturing/engines/llama_utils/llama.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/engines/lora_engine/lora.py` & `xturing-0.1.6/src/xturing/engines/lora_engine/lora.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,59 +8,66 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import enum
 import importlib
 import json
 import math
 import os
 import re
 import warnings
 from dataclasses import asdict, dataclass, field
 from enum import Enum
 from typing import List, Optional, Union
-import enum
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+import transformers
+from transformers import LlamaConfig, LlamaForCausalLM
 from transformers.pytorch_utils import Conv1D
 
 from xturing.engines.lora_engine.save_and_load import (
     get_peft_model_state_dict,
     set_peft_model_state_dict,
 )
+from xturing.engines.quant_utils import QuantLinear, autotune_warmup
 
 
 def is_bnb_available():
     return importlib.util.find_spec("bitsandbytes") is not None
 
 
 if is_bnb_available():
     import bitsandbytes as bnb
 
 
 def transpose(weight, fan_in_fan_out):
     return weight.T if fan_in_fan_out else weight
 
+
 def is_gptq_available():
     return importlib.util.find_spec("xturing.engines.quant_utils") is not None
 
+
 if is_gptq_available():
     from ..quant_utils import QuantLinear
 
+
 class PeftType(str, enum.Enum):
     PROMPT_TUNING = "PROMPT_TUNING"
     P_TUNING = "P_TUNING"
     PREFIX_TUNING = "PREFIX_TUNING"
     LORA = "LORA"
 
+
 WEIGHTS_NAME = "adapter_model.bin"
 CONFIG_NAME = "adapter_config.json"
 
 
 @dataclass
 class LoraConfig:
     """
@@ -86,22 +93,30 @@
             "help": "List of module names or regex expression of the module names to replace with Lora."
             "For example, ['q', 'v'] or '.*decoder.*(SelfAttention|EncDecAttention).*(q|v)$' "
         },
     )
     lora_alpha: int = field(default=None, metadata={"help": "Lora alpha"})
     lora_dropout: float = field(default=None, metadata={"help": "Lora dropout"})
     merge_weights: bool = field(
-        default=False, metadata={"help": "Merge weights of the original model and the Lora model"}
+        default=False,
+        metadata={"help": "Merge weights of the original model and the Lora model"},
     )
     fan_in_fan_out: bool = field(
         default=False,
-        metadata={"help": "Set this to True if the layer to replace stores weight like (fan_in, fan_out)"},
+        metadata={
+            "help": "Set this to True if the layer to replace stores weight like (fan_in, fan_out)"
+        },
+    )
+    enable_lora: Optional[List[bool]] = field(
+        default=None, metadata={"help": "Used with `lora.MergedLinear`."}
+    )
+    bias: str = field(
+        default="none",
+        metadata={"help": "Bias type for Lora. Can be 'none', 'all' or 'lora_only'"},
     )
-    enable_lora: Optional[List[bool]] = field(default=None, metadata={"help": "Used with `lora.MergedLinear`."})
-    bias: str = field(default="none", metadata={"help": "Bias type for Lora. Can be 'none', 'all' or 'lora_only'"})
     modules_to_save: Optional[List[str]] = field(
         default=None,
         metadata={
             "help": "List of modules apart from LoRA layers to be set as trainable and saved in the final checkpoint. "
             "For example, in Sequence Classification or Token Classification tasks, "
             "the final layer `classifier/score` are randomly initialized and as such need to be trainable and saved."
         },
@@ -227,37 +242,44 @@
         self.model = model
         self._find_and_replace()
         mark_only_lora_as_trainable(self.model, self.peft_config.bias)
         self.forward = self.model.forward
 
     def _find_and_replace(self):
         loaded_in_8bit = getattr(self.model, "is_loaded_in_8bit", False)
-        is_gtq_quantized = getattr(self.model, "gptq", False)  # Step 1: Check if the model is GTQ quantized
+        is_gtq_quantized = getattr(
+            self.model, "gptq", False
+        )  # Step 1: Check if the model is GTQ quantized
 
         if loaded_in_8bit and not is_bnb_available():
             raise ImportError(
                 "To use Lora with 8-bit quantization, please install the `bitsandbytes` package. "
                 "You can install it with `pip install bitsandbytes`."
             )
         is_target_modules_in_base_model = False
         is_hf_device_map_available = hasattr(self.model, "hf_device_map")
         kwargs = {
             "r": self.peft_config.r,
             "lora_alpha": self.peft_config.lora_alpha,
             "lora_dropout": self.peft_config.lora_dropout,
             "fan_in_fan_out": self.peft_config.fan_in_fan_out,
-            "merge_weights": (self.peft_config.merge_weights or self.peft_config.inference_mode)
+            "merge_weights": (
+                self.peft_config.merge_weights or self.peft_config.inference_mode
+            )
             and not is_hf_device_map_available,
         }
         key_list = [key for key, _ in self.model.named_modules()]
         for key in key_list:
             if isinstance(self.peft_config.target_modules, str):
                 target_module_found = re.fullmatch(self.peft_config.target_modules, key)
             else:
-                target_module_found = any(key.endswith(target_key) for target_key in self.peft_config.target_modules)
+                target_module_found = any(
+                    key.endswith(target_key)
+                    for target_key in self.peft_config.target_modules
+                )
             if target_module_found:
                 if not is_target_modules_in_base_model:
                     is_target_modules_in_base_model = True
                 parent, target, target_name = self._get_submodules(key)
                 bias = target.bias is not None
                 if loaded_in_8bit and isinstance(target, bnb.nn.Linear8bitLt):
                     kwargs.update(
@@ -265,57 +287,79 @@
                             "has_fp16_weights": target.state.has_fp16_weights,
                             "memory_efficient_backward": target.state.memory_efficient_backward,
                             "threshold": target.state.threshold,
                             "index": target.index,
                         }
                     )
                     if self.peft_config.enable_lora is None:
-                        new_module = Linear8bitLt(target.in_features, target.out_features, bias=bias, **kwargs)
+                        new_module = Linear8bitLt(
+                            target.in_features, target.out_features, bias=bias, **kwargs
+                        )
                     else:
                         kwargs.update({"enable_lora": self.peft_config.enable_lora})
-                        new_module = MergedLinear8bitLt(target.in_features, target.out_features, bias=bias, **kwargs)
+                        new_module = MergedLinear8bitLt(
+                            target.in_features, target.out_features, bias=bias, **kwargs
+                        )
                 elif is_gptq_available() and isinstance(target, QuantLinear):
                     kwargs.update(
                         {
                             "bits": target.bits,
                             "groupsize": target.groupsize,
                         }
                     )
                     if self.peft_config.enable_lora is None:
-                        new_module = LinearqbitLt(target.infeatures, target.outfeatures, bias=bias, **kwargs)
+                        new_module = LinearqbitLt(
+                            target.infeatures, target.outfeatures, bias=bias, **kwargs
+                        )
                         new_module.scales = target.scales
                         new_module.qzeros = target.qzeros
                         new_module.g_idx = target.g_idx
                         if target.bias:
                             new_module.bias = target.bias
                     else:
                         kwargs.update({"enable_lora": self.peft_config.enable_lora})
-                        new_module = MergedLinearqbitLt(target.infeatures, target.outfeatures, bias=bias, **kwargs)
+                        new_module = MergedLinearqbitLt(
+                            target.infeatures, target.outfeatures, bias=bias, **kwargs
+                        )
                         new_module.scales = target.scales
                         new_module.qzeros = target.qzeros
                         new_module.g_idx = target.g_idx
                         if target.bias:
                             new_module.bias = target.bias
-                elif isinstance(target, torch.nn.Linear) and self.peft_config.enable_lora is None:
-                    new_module = Linear(target.in_features, target.out_features, bias=bias, **kwargs)
+                elif (
+                    isinstance(target, torch.nn.Linear)
+                    and self.peft_config.enable_lora is None
+                ):
+                    new_module = Linear(
+                        target.in_features, target.out_features, bias=bias, **kwargs
+                    )
                 elif self.peft_config.enable_lora is not None:
                     kwargs.update({"enable_lora": self.peft_config.enable_lora})
                     if isinstance(target, Conv1D):
                         in_features, out_features = (
-                            target.weight.ds_shape if hasattr(target.weight, "ds_shape") else target.weight.shape
+                            target.weight.ds_shape
+                            if hasattr(target.weight, "ds_shape")
+                            else target.weight.shape
                         )
                     else:
-                        in_features, out_features = target.in_features, target.out_features
+                        in_features, out_features = (
+                            target.in_features,
+                            target.out_features,
+                        )
                         if kwargs["fan_in_fan_out"]:
                             warnings.warn(
                                 "fan_in_fan_out is set to True but the target module is not a Conv1D. "
                                 "Setting fan_in_fan_out to False."
                             )
-                            kwargs["fan_in_fan_out"] = self.peft_config.fan_in_fan_out = False
-                    new_module = MergedLinear(in_features, out_features, bias=bias, **kwargs)
+                            kwargs[
+                                "fan_in_fan_out"
+                            ] = self.peft_config.fan_in_fan_out = False
+                    new_module = MergedLinear(
+                        in_features, out_features, bias=bias, **kwargs
+                    )
                 self._replace_module(parent, target_name, new_module, target)
         if not is_target_modules_in_base_model:
             raise ValueError(
                 f"Target modules {self.peft_config.target_modules} not found in the base model. "
                 f"Please check the target modules and try again."
             )
 
@@ -360,15 +404,18 @@
             return getattr(self.model, name)
 
     @property
     def modules_to_save(self):
         return None
 
     def get_peft_config_as_dict(self, inference: bool = False):
-        config = {k: v.value if isinstance(v, Enum) else v for k, v in asdict(self.peft_config).items()}
+        config = {
+            k: v.value if isinstance(v, Enum) else v
+            for k, v in asdict(self.peft_config).items()
+        }
         if inference:
             config["inference_mode"] = True
         return config
 
     def _set_adapter_layers(self, enabled=True):
         for module in self.model.modules():
             if isinstance(module, LoraLayer):
@@ -508,15 +555,21 @@
         lora_alpha: int = 1,
         lora_dropout: float = 0.0,
         fan_in_fan_out: bool = False,  # Set this to True if the layer to replace stores weight like (fan_in, fan_out)
         merge_weights: bool = True,
         **kwargs,
     ):
         nn.Linear.__init__(self, in_features, out_features, **kwargs)
-        LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=merge_weights)
+        LoraLayer.__init__(
+            self,
+            r=r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            merge_weights=merge_weights,
+        )
 
         self.fan_in_fan_out = fan_in_fan_out
         # Actual trainable parameters
         if r > 0:
             self.lora_A = nn.Linear(in_features, r, bias=False)
             self.lora_B = nn.Linear(r, out_features, bias=False)
             self.scaling = self.lora_alpha / self.r
@@ -537,47 +590,64 @@
         nn.Linear.train(self, mode)
         self.lora_A.train(mode)
         self.lora_B.train(mode)
         if not mode and self.merge_weights and not self.merged:
             # Merge the weights and mark it
             if self.r > 0:
                 self.weight.data += (
-                    transpose(self.lora_B.weight @ self.lora_A.weight, self.fan_in_fan_out) * self.scaling
+                    transpose(
+                        self.lora_B.weight @ self.lora_A.weight, self.fan_in_fan_out
+                    )
+                    * self.scaling
                 )
             self.merged = True
         elif self.merge_weights and self.merged:
             # Make sure that the weights are not merged
             if self.r > 0:
                 self.weight.data -= (
-                    transpose(self.lora_B.weight @ self.lora_A.weight, self.fan_in_fan_out) * self.scaling
+                    transpose(
+                        self.lora_B.weight @ self.lora_A.weight, self.fan_in_fan_out
+                    )
+                    * self.scaling
                 )
             self.merged = False
 
     def eval(self):
         nn.Linear.eval(self)
         self.lora_A.eval()
         self.lora_B.eval()
 
     def forward(self, x: torch.Tensor):
         if self.disable_adapters:
             if self.r > 0 and self.merged:
                 self.weight.data -= (
-                    transpose(self.lora_B.weight @ self.lora_A.weight, self.fan_in_fan_out) * self.scaling
+                    transpose(
+                        self.lora_B.weight @ self.lora_A.weight, self.fan_in_fan_out
+                    )
+                    * self.scaling
                 )
                 self.merged = False
 
-            return F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
+            return F.linear(
+                x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias
+            )
         elif self.r > 0 and not self.merged:
-            result = F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
+            result = F.linear(
+                x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias
+            )
             if self.r > 0:
-                loraoutput = self.lora_B(self.lora_A(self.lora_dropout(x))) * self.scaling
+                loraoutput = (
+                    self.lora_B(self.lora_A(self.lora_dropout(x))) * self.scaling
+                )
                 result = result + loraoutput
             return result
         else:
-            return F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
+            return F.linear(
+                x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias
+            )
 
 
 class MergedLinear(nn.Linear, LoraLayer):
     # Lora implemented in a dense layer
     def __init__(
         self,
         in_features: int,
@@ -587,15 +657,21 @@
         lora_dropout: float = 0.0,
         enable_lora: List[bool] = [False],
         fan_in_fan_out: bool = False,
         merge_weights: bool = True,
         **kwargs,
     ):
         nn.Linear.__init__(self, in_features, out_features, **kwargs)
-        LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=merge_weights)
+        LoraLayer.__init__(
+            self,
+            r=r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            merge_weights=merge_weights,
+        )
         if out_features % len(enable_lora) != 0:
             raise ValueError("The length of enable_lora must divide out_features")
         self.enable_lora = enable_lora
         self.fan_in_fan_out = fan_in_fan_out
         # Actual trainable parameters
         if r > 0 and any(enable_lora):
             self.lora_A = nn.Linear(in_features, r * sum(enable_lora), bias=False)
@@ -606,15 +682,17 @@
                 groups=2,
                 bias=False,
             )
             self.scaling = self.lora_alpha / self.r
             # Freezing the pre-trained weight matrix
             self.weight.requires_grad = False
             # Compute the indices
-            self.lora_ind = self.weight.new_zeros((out_features,), dtype=torch.bool).view(len(enable_lora), -1)
+            self.lora_ind = self.weight.new_zeros(
+                (out_features,), dtype=torch.bool
+            ).view(len(enable_lora), -1)
             self.lora_ind[enable_lora, :] = True
             self.lora_ind = self.lora_ind.view(-1)
         self.reset_parameters()
         if fan_in_fan_out:
             self.weight.data = self.weight.data.T
 
     def reset_parameters(self):
@@ -623,15 +701,17 @@
             # initialize A the same way as the default for nn.Linear and B to zero
             nn.init.kaiming_uniform_(self.lora_A.weight, a=math.sqrt(5))
             nn.init.zeros_(self.lora_B.weight)
 
     def zero_pad(self, x):
         result = x.new_zeros((*x.shape[:-1], self.out_features))
         result = result.view(-1, self.out_features)
-        result[:, self.lora_ind] = x.reshape(-1, self.out_features // len(self.enable_lora) * sum(self.enable_lora))
+        result[:, self.lora_ind] = x.reshape(
+            -1, self.out_features // len(self.enable_lora) * sum(self.enable_lora)
+        )
         return result.view((*x.shape[:-1], self.out_features))
 
     def train(self, mode: bool = True):
         nn.Linear.train(self, mode)
         self.lora_A.train(mode)
         self.lora_B.train(mode)
         if not mode and self.merge_weights and not self.merged:
@@ -642,29 +722,33 @@
                         self.lora_A.weight.data.unsqueeze(0),
                         self.lora_B.weight.data,
                         groups=sum(self.enable_lora),
                     )
                     .squeeze(0)
                     .transpose(-2, -1)
                 )
-                self.weight.data += transpose(self.zero_pad(delta_w * self.scaling), not self.fan_in_fan_out)
+                self.weight.data += transpose(
+                    self.zero_pad(delta_w * self.scaling), not self.fan_in_fan_out
+                )
             self.merged = True
         elif self.merge_weights and self.merged:
             # Make sure that the weights are not merged
             if self.r > 0 and any(self.enable_lora):
                 delta_w = (
                     F.conv1d(
                         self.lora_A.weight.data.unsqueeze(0),
                         self.lora_B.weight.data,
                         groups=sum(self.enable_lora),
                     )
                     .squeeze(0)
                     .transpose(-2, -1)
                 )
-                self.weight.data -= transpose(self.zero_pad(delta_w * self.scaling), not self.fan_in_fan_out)
+                self.weight.data -= transpose(
+                    self.zero_pad(delta_w * self.scaling), not self.fan_in_fan_out
+                )
             self.merged = False
 
     def eval(self):
         nn.Linear.eval(self)
         self.lora_A.eval()
         self.lora_B.eval()
 
@@ -676,21 +760,29 @@
                         self.lora_A.weight.data.unsqueeze(0),
                         self.lora_B.weight.data,
                         groups=sum(self.enable_lora),
                     )
                     .squeeze(0)
                     .transpose(-2, -1)
                 )
-                self.weight.data -= transpose(self.zero_pad(delta_w * self.scaling), not self.fan_in_fan_out)
+                self.weight.data -= transpose(
+                    self.zero_pad(delta_w * self.scaling), not self.fan_in_fan_out
+                )
                 self.merged = False
-            return F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
+            return F.linear(
+                x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias
+            )
         elif self.merged:
-            return F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
+            return F.linear(
+                x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias
+            )
         else:
-            result = F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
+            result = F.linear(
+                x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias
+            )
             if self.r > 0:
                 after_A = self.lora_A(self.lora_dropout(x))
                 after_B = self.lora_B(after_A.transpose(-2, -1)).transpose(-2, -1)
                 result += self.zero_pad(after_B) * self.scaling
             return result
 
 
@@ -709,19 +801,27 @@
         ):
             bnb.nn.Linear8bitLt.__init__(
                 self,
                 in_features,
                 out_features,
                 bias=kwargs.get("bias", True),
                 has_fp16_weights=kwargs.get("has_fp16_weights", True),
-                memory_efficient_backward=kwargs.get("memory_efficient_backward", False),
+                memory_efficient_backward=kwargs.get(
+                    "memory_efficient_backward", False
+                ),
                 threshold=kwargs.get("threshold", 0.0),
                 index=kwargs.get("index", None),
             )
-            LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=False)
+            LoraLayer.__init__(
+                self,
+                r=r,
+                lora_alpha=lora_alpha,
+                lora_dropout=lora_dropout,
+                merge_weights=False,
+            )
             # Actual trainable parameters
             if r > 0:
                 self.lora_A = nn.Linear(in_features, r, bias=False)
                 self.lora_B = nn.Linear(r, out_features, bias=False)
                 self.scaling = self.lora_alpha / self.r
                 # Freezing the pre-trained weight matrix
                 self.weight.requires_grad = False
@@ -740,18 +840,25 @@
                 return result
             elif self.r > 0:
                 if not torch.is_autocast_enabled():
                     expected_dtype = result.dtype
 
                     if x.dtype != torch.float32:
                         x = x.float()
-                    output = self.lora_B(self.lora_A(self.lora_dropout(x))).to(expected_dtype) * self.scaling
+                    output = (
+                        self.lora_B(self.lora_A(self.lora_dropout(x))).to(
+                            expected_dtype
+                        )
+                        * self.scaling
+                    )
                     result += output
                 else:
-                    output = self.lora_B(self.lora_A(self.lora_dropout(x))) * self.scaling
+                    output = (
+                        self.lora_B(self.lora_A(self.lora_dropout(x))) * self.scaling
+                    )
                     result += output
             return result
 
     class MergedLinear8bitLt(bnb.nn.Linear8bitLt, LoraLayer):
         # Lora implemented in a dense layer
         def __init__(
             self,
@@ -765,19 +872,27 @@
         ):
             bnb.nn.Linear8bitLt.__init__(
                 self,
                 in_features,
                 out_features,
                 bias=kwargs.get("bias", True),
                 has_fp16_weights=kwargs.get("has_fp16_weights", True),
-                memory_efficient_backward=kwargs.get("memory_efficient_backward", False),
+                memory_efficient_backward=kwargs.get(
+                    "memory_efficient_backward", False
+                ),
                 threshold=kwargs.get("threshold", 0.0),
                 index=kwargs.get("index", None),
             )
-            LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=False)
+            LoraLayer.__init__(
+                self,
+                r=r,
+                lora_alpha=lora_alpha,
+                lora_dropout=lora_dropout,
+                merge_weights=False,
+            )
             if out_features % len(enable_lora) != 0:
                 raise ValueError("The length of enable_lora must divide out_features")
             self.enable_lora = enable_lora
             # Actual trainable parameters
             if r > 0 and any(enable_lora):
                 self.lora_A = nn.Linear(in_features, r * sum(enable_lora), bias=False)
                 self.lora_B = nn.Conv1d(
@@ -787,15 +902,17 @@
                     groups=2,
                     bias=False,
                 )
                 self.scaling = self.lora_alpha / self.r
                 # Freezing the pre-trained weight matrix
                 self.weight.requires_grad = False
                 # Compute the indices
-                self.lora_ind = self.weight.new_zeros((out_features,), dtype=torch.bool).view(len(enable_lora), -1)
+                self.lora_ind = self.weight.new_zeros(
+                    (out_features,), dtype=torch.bool
+                ).view(len(enable_lora), -1)
                 self.lora_ind[enable_lora, :] = True
                 self.lora_ind = self.lora_ind.view(-1)
             self.reset_parameters()
 
         def reset_parameters(self):
             if hasattr(self, "lora_A"):
                 # initialize A the same way as the default for nn.Linear and B to zero
@@ -826,37 +943,44 @@
                 else:
                     after_A = self.lora_A(self.lora_dropout(x))
                     after_B = self.lora_B(after_A.transpose(-2, -1)).transpose(-2, -1)
                     output = self.zero_pad(after_B) * self.scaling
                     result += output
             return result
 
+
 if is_gptq_available():
+
     class LinearqbitLt(QuantLinear, LoraLayer):
         # Lora implemented in a dense layer
         def __init__(
             self,
             in_features,
             out_features,
             r: int = 0,
             lora_alpha: int = 1,
             lora_dropout: float = 0.0,
             **kwargs,
         ):
-            
             QuantLinear.__init__(
                 self,
-                kwargs.get('bits', 4),
-                kwargs.get('groupsize', 128),
+                kwargs.get("bits", 4),
+                kwargs.get("groupsize", 128),
                 in_features,
                 out_features,
-                kwargs.get('bias', False),
+                kwargs.get("bias", False),
             )
 
-            LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=False)
+            LoraLayer.__init__(
+                self,
+                r=r,
+                lora_alpha=lora_alpha,
+                lora_dropout=lora_dropout,
+                merge_weights=False,
+            )
             # Actual trainable parameters
             if r > 0:
                 self.lora_A = nn.Linear(in_features, r, bias=False)
                 self.lora_B = nn.Linear(r, out_features, bias=False)
                 self.scaling = self.lora_alpha / self.r
                 # Freezing the pre-trained weight matrix
                 self.qweight.requires_grad = False
@@ -864,24 +988,28 @@
                 self.qzeros.requires_grad = False
             self.reset_parameters()
 
         def reset_parameters(self):
             if hasattr(self, "lora_A"):
                 # initialize A the same way as the default for nn.Linear and B to zero
                 # nn.init.kaiming_uniform_(self.lora_A.weight, a=math.sqrt(5))
-                self.lora_A.weight = torch.nn.Parameter(torch.nn.init.kaiming_uniform(self.lora_A.weight, a=math.sqrt(5)))
+                self.lora_A.weight = torch.nn.Parameter(
+                    torch.nn.init.kaiming_uniform(self.lora_A.weight, a=math.sqrt(5))
+                )
                 nn.init.zeros_(self.lora_B.weight)
 
         def forward(self, x: torch.Tensor):
             # x = x.detach()
             custom_layer_output = super().forward(x)
-            
+
             dtype = custom_layer_output.dtype
             x = x.float()
-            lora_output = self.lora_B(self.lora_A(self.lora_dropout(x))).to(dtype) * self.scaling
+            lora_output = (
+                self.lora_B(self.lora_A(self.lora_dropout(x))).to(dtype) * self.scaling
+            )
             result = custom_layer_output + lora_output
             return result
 
     class MergedLinearqbitLt(QuantLinear, LoraLayer):
         # Lora implemented in a dense layer
         def __init__(
             self,
@@ -891,20 +1019,26 @@
             lora_alpha: int = 1,
             lora_dropout: float = 0.0,
             enable_lora: List[bool] = [False],
             **kwargs,
         ):
             QuantLinear.__init__(
                 self,
-                kwargs.get('bits', 4),
-                kwargs.get('groupsize', 128),
+                kwargs.get("bits", 4),
+                kwargs.get("groupsize", 128),
                 in_features,
                 out_features,
             )
-            LoraLayer.__init__(self, r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout, merge_weights=False)
+            LoraLayer.__init__(
+                self,
+                r=r,
+                lora_alpha=lora_alpha,
+                lora_dropout=lora_dropout,
+                merge_weights=False,
+            )
             if out_features % len(enable_lora) != 0:
                 raise ValueError("The length of enable_lora must divide out_features")
             self.enable_lora = enable_lora
             # Actual trainable parameters
             if r > 0 and any(enable_lora):
                 self.lora_A = nn.Linear(in_features, r * sum(enable_lora), bias=False)
                 self.lora_B = nn.Conv1d(
@@ -914,15 +1048,17 @@
                     groups=2,
                     bias=False,
                 )
                 self.scaling = self.lora_alpha / self.r
                 # Freezing the pre-trained weight matrix
                 self.qweight.requires_grad = False
                 # Compute the indices
-                self.lora_ind = self.weight.new_zeros((out_features,), dtype=torch.bool).view(len(enable_lora), -1)
+                self.lora_ind = self.weight.new_zeros(
+                    (out_features,), dtype=torch.bool
+                ).view(len(enable_lora), -1)
                 self.lora_ind[enable_lora, :] = True
                 self.lora_ind = self.lora_ind.view(-1)
             self.reset_parameters()
 
         def reset_parameters(self):
             if hasattr(self, "lora_A"):
                 # initialize A the same way as the default for nn.Linear and B to zero
@@ -934,15 +1070,15 @@
             result = result.view(-1, self.out_features)
             result[:, self.lora_ind] = x.reshape(
                 -1, self.out_features // len(self.enable_lora) * sum(self.enable_lora)
             )
             return result.view((*x.shape[:-1], self.out_features))
 
         def forward(self, x: torch.Tensor):
-            result = super().forward(x)#.detach()
+            result = super().forward(x)  # .detach()
             if self.disable_adapters:
                 return result
             elif self.r > 0:
                 if not torch.is_autocast_enabled():
                     expected_dtype = result.dtype
                     if x.dtype != torch.float32:
                         x = x.float()
@@ -1015,7 +1151,85 @@
         setattr(
             model,
             output_embedding_layer_name,
             CastOutputToFloat(output_embedding_layer),
         )
 
     return model
+
+
+def make_quant(module, names, bits, groupsize, name=""):
+    if isinstance(module, QuantLinear):
+        return
+    for attr in dir(module):
+        tmp = getattr(module, attr)
+        name1 = name + "." + attr if name != "" else attr
+        if name1 in names:
+            delattr(module, attr)
+            setattr(
+                module,
+                attr,
+                QuantLinear(
+                    bits,
+                    groupsize,
+                    tmp.in_features,
+                    tmp.out_features,
+                    tmp.bias is not None,
+                ),
+            )
+    for name1, child in module.named_children():
+        make_quant(
+            child, names, bits, groupsize, name + "." + name1 if name != "" else name1
+        )
+
+
+def find_layers(module, layers=[nn.Conv2d, nn.Linear], name=""):
+    if type(module) in layers:
+        return {name: module}
+    res = {}
+    for name1, child in module.named_children():
+        res.update(
+            find_layers(
+                child, layers=layers, name=name + "." + name1 if name != "" else name1
+            )
+        )
+    return res
+
+
+def load_quant(
+    model, checkpoint, wbits, groupsize=128, warmup_autotune=True, model_seqlen=2048
+):
+    config = LlamaConfig.from_pretrained(model)
+
+    def noop(*args, **kwargs):
+        pass
+
+    torch.nn.init.kaiming_uniform_ = noop
+    torch.nn.init.uniform_ = noop
+    torch.nn.init.normal_ = noop
+
+    torch.set_default_dtype(torch.half)
+    transformers.modeling_utils._init_weights = False
+    torch.set_default_dtype(torch.half)
+    model = LlamaForCausalLM(config)
+    torch.set_default_dtype(torch.float)
+    model = model.eval()
+    layers = find_layers(model)
+    for name in ["lm_head"]:
+        if name in layers:
+            del layers[name]
+    make_quant(model, layers, wbits, groupsize)
+
+    del layers
+
+    print("Loading model ...")
+    if checkpoint.endswith(".safetensors"):
+        from safetensors.torch import load_file as safe_load
+
+        model.load_state_dict(safe_load(checkpoint), strict=False)
+    else:
+        model.load_state_dict(torch.load(checkpoint), strict=False)
+    if warmup_autotune:
+        autotune_warmup(model)
+    model.seqlen = model_seqlen
+    print("Done.")
+    return model
```

### Comparing `xturing-0.1.5/src/xturing/engines/lora_engine/save_and_load.py` & `xturing-0.1.6/src/xturing/engines/lora_engine/save_and_load.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/engines/opt_engine.py` & `xturing-0.1.6/src/xturing/engines/opt_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/engines/quant_utils/custom_autotune.py` & `xturing-0.1.6/src/xturing/engines/quant_utils/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/engines/quant_utils/quant.py` & `xturing-0.1.6/src/xturing/engines/quant_utils/quant.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/model_apis/__init__.py` & `xturing-0.1.6/src/xturing/model_apis/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/model_apis/ai21.py` & `xturing-0.1.6/src/xturing/model_apis/ai21.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/model_apis/base.py` & `xturing-0.1.6/src/xturing/model_apis/base.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/model_apis/cohere.py` & `xturing-0.1.6/src/xturing/model_apis/cohere.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/model_apis/openai.py` & `xturing-0.1.6/src/xturing/model_apis/openai.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/models/__init__.py` & `xturing-0.1.6/src/xturing/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 from .base import BaseModel
 from .bloom import Bloom, BloomInt8, BloomLora, BloomLoraInt8
 from .cerebras import Cerebras, CerebrasInt8, CerebrasLora, CerebrasLoraInt8
 from .distilgpt2 import DistilGPT2, DistilGPT2Lora
-from .falcon import Falcon, FalconInt8, FalconLora, FalconLoraInt8
+from .falcon import Falcon, FalconInt8, FalconLora, FalconLoraInt8, FalconLoraKbit
 from .galactica import Galactica, GalacticaInt8, GalacticaLora, GalacticaLoraInt8
 from .generic import (
     GenericInt8Model,
     GenericLoraInt8Model,
+    GenericLoraKbitModel,
     GenericLoraModel,
     GenericModel,
 )
 from .gpt2 import GPT2, GPT2Int8, GPT2Lora, GPT2LoraInt8
 from .gptj import GPTJ, GPTJInt8, GPTJLora, GPTJLoraInt8
-from .llama import Llama, LlamaInt8, LlamaLora, LlamaLoraInt4, LlamaLoraInt8
+from .llama import Llama, LlamaInt8, LlamaLora, LlamaLoraInt8, LlamaLoraKbit
 from .opt import OPT, OPTInt8, OPTLora, OPTLoraInt8
 from .stable_diffusion import StableDiffusion
 
+BaseModel.add_to_registry(Bloom.config_name, Bloom)
+BaseModel.add_to_registry(BloomInt8.config_name, BloomInt8)
+BaseModel.add_to_registry(BloomLora.config_name, BloomLora)
+BaseModel.add_to_registry(BloomLoraInt8.config_name, BloomLoraInt8)
+BaseModel.add_to_registry(Cerebras.config_name, Cerebras)
+BaseModel.add_to_registry(CerebrasInt8.config_name, CerebrasInt8)
+BaseModel.add_to_registry(CerebrasLora.config_name, CerebrasLora)
+BaseModel.add_to_registry(CerebrasLoraInt8.config_name, CerebrasLoraInt8)
 BaseModel.add_to_registry(DistilGPT2.config_name, DistilGPT2)
 BaseModel.add_to_registry(DistilGPT2Lora.config_name, DistilGPT2Lora)
-BaseModel.add_to_registry(GPT2.config_name, GPT2)
-BaseModel.add_to_registry(GPT2Lora.config_name, GPT2Lora)
-BaseModel.add_to_registry(GPT2Int8.config_name, GPT2Int8)
-BaseModel.add_to_registry(GPT2LoraInt8.config_name, GPT2LoraInt8)
+BaseModel.add_to_registry(Falcon.config_name, Falcon)
+BaseModel.add_to_registry(FalconInt8.config_name, FalconInt8)
+BaseModel.add_to_registry(FalconLora.config_name, FalconLora)
+BaseModel.add_to_registry(FalconLoraInt8.config_name, FalconLoraInt8)
+BaseModel.add_to_registry(FalconLoraKbit.config_name, FalconLoraKbit)
+BaseModel.add_to_registry(Galactica.config_name, Galactica)
+BaseModel.add_to_registry(GalacticaInt8.config_name, GalacticaInt8)
+BaseModel.add_to_registry(GalacticaLora.config_name, GalacticaLora)
+BaseModel.add_to_registry(GalacticaLoraInt8.config_name, GalacticaLoraInt8)
+BaseModel.add_to_registry(GenericModel.config_name, GenericModel)
+BaseModel.add_to_registry(GenericInt8Model.config_name, GenericInt8Model)
+BaseModel.add_to_registry(GenericLoraModel.config_name, GenericLoraModel)
+BaseModel.add_to_registry(GenericLoraInt8Model.config_name, GenericLoraInt8Model)
+BaseModel.add_to_registry(GenericLoraKbitModel.config_name, GenericLoraKbitModel)
 BaseModel.add_to_registry(GPTJ.config_name, GPTJ)
-BaseModel.add_to_registry(GPTJLora.config_name, GPTJLora)
 BaseModel.add_to_registry(GPTJInt8.config_name, GPTJInt8)
+BaseModel.add_to_registry(GPTJLora.config_name, GPTJLora)
 BaseModel.add_to_registry(GPTJLoraInt8.config_name, GPTJLoraInt8)
+BaseModel.add_to_registry(GPT2.config_name, GPT2)
+BaseModel.add_to_registry(GPT2Int8.config_name, GPT2Int8)
+BaseModel.add_to_registry(GPT2Lora.config_name, GPT2Lora)
+BaseModel.add_to_registry(GPT2LoraInt8.config_name, GPT2LoraInt8)
 BaseModel.add_to_registry(Llama.config_name, Llama)
-BaseModel.add_to_registry(LlamaLora.config_name, LlamaLora)
 BaseModel.add_to_registry(LlamaInt8.config_name, LlamaInt8)
+BaseModel.add_to_registry(LlamaLora.config_name, LlamaLora)
 BaseModel.add_to_registry(LlamaLoraInt8.config_name, LlamaLoraInt8)
-BaseModel.add_to_registry(LlamaLoraInt4.config_name, LlamaLoraInt4)
-BaseModel.add_to_registry(Galactica.config_name, Galactica)
-BaseModel.add_to_registry(GalacticaLora.config_name, GalacticaLora)
-BaseModel.add_to_registry(GalacticaInt8.config_name, GalacticaInt8)
-BaseModel.add_to_registry(GalacticaLoraInt8.config_name, GalacticaLoraInt8)
+BaseModel.add_to_registry(LlamaLoraKbit.config_name, LlamaLoraKbit)
 BaseModel.add_to_registry(OPT.config_name, OPT)
-BaseModel.add_to_registry(OPTLora.config_name, OPTLora)
 BaseModel.add_to_registry(OPTInt8.config_name, OPTInt8)
+BaseModel.add_to_registry(OPTLora.config_name, OPTLora)
 BaseModel.add_to_registry(OPTLoraInt8.config_name, OPTLoraInt8)
-BaseModel.add_to_registry(Cerebras.config_name, Cerebras)
-BaseModel.add_to_registry(CerebrasLora.config_name, CerebrasLora)
-BaseModel.add_to_registry(CerebrasInt8.config_name, CerebrasInt8)
-BaseModel.add_to_registry(CerebrasLoraInt8.config_name, CerebrasLoraInt8)
-BaseModel.add_to_registry(Bloom.config_name, Bloom)
-BaseModel.add_to_registry(BloomLora.config_name, BloomLora)
-BaseModel.add_to_registry(BloomInt8.config_name, BloomInt8)
-BaseModel.add_to_registry(BloomLoraInt8.config_name, BloomLoraInt8)
 BaseModel.add_to_registry(StableDiffusion.config_name, StableDiffusion)
-BaseModel.add_to_registry(GenericModel.config_name, GenericModel)
-BaseModel.add_to_registry(GenericLoraModel.config_name, GenericLoraModel)
-BaseModel.add_to_registry(GenericInt8Model.config_name, GenericInt8Model)
-BaseModel.add_to_registry(GenericLoraInt8Model.config_name, GenericLoraInt8Model)
-BaseModel.add_to_registry(Falcon.config_name, Falcon)
-BaseModel.add_to_registry(FalconLora.config_name, FalconLora)
-BaseModel.add_to_registry(FalconInt8.config_name, FalconInt8)
-BaseModel.add_to_registry(FalconLoraInt8.config_name, FalconLoraInt8)
```

### Comparing `xturing-0.1.5/src/xturing/models/base.py` & `xturing-0.1.6/src/xturing/models/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,19 @@
             model_name is not None
         ), "The xturing.json file is not correct. model_name is not available in the configuration"
 
         assert (
             cls.registry.get(model_name) is not None
         ), "The model_name {} is not valid".format(model_name)
 
-        model = cls.create(model_name, weights_path=weights_dir_path)
+        if "generic" in model_name:
+            model = cls.create(
+                model_name, model_name=model_name, weights_path=weights_dir_path
+            )
+        else:
+            model = cls.create(model_name, weights_path=weights_dir_path)
 
         return model
 
 
 # add_to_registry is a class method, so it's called on the class, not on an instance of the class
 # registration happens in __init__.py, to avoid circular imports
```

### Comparing `xturing-0.1.5/src/xturing/models/bloom.py` & `xturing-0.1.6/src/xturing/models/bloom.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/models/causal.py` & `xturing-0.1.6/src/xturing/models/causal.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,19 +27,21 @@
 class CausalModel(BaseModel):
     def __init__(
         self,
         engine: str,
         weights_path: Optional[str] = None,
         model_name: Optional[str] = None,
         target_modules: Optional[List[str]] = None,
+        **kwargs,
     ):
         arguments = dict(
             weights_path=weights_path,
             model_name=model_name,
             target_modules=target_modules,
+            **kwargs,
         )
 
         self.engine = BaseEngine.create(
             engine,
             **_filter_args(arguments),
         )
 
@@ -207,32 +209,37 @@
 
 class CausalInt8Model(CausalModel):
     def __init__(
         self,
         engine: str,
         weights_path: Optional[str] = None,
         model_name: Optional[str] = None,
+        **kwargs,
     ):
         assert_not_cpu_int8()
-        super().__init__(engine, weights_path=weights_path, model_name=model_name)
+        super().__init__(
+            engine, weights_path=weights_path, model_name=model_name, **kwargs
+        )
 
 
 class CausalLoraModel(CausalModel):
     def __init__(
         self,
         engine: str,
         weights_path: Optional[str] = None,
         model_name: Optional[str] = None,
         target_modules: Optional[List[str]] = None,
+        **kwargs,
     ):
         super().__init__(
             engine,
             weights_path=weights_path,
             model_name=model_name,
             target_modules=target_modules,
+            **kwargs,
         )
 
     def _make_trainer(
         self,
         dataset: Union[TextDataset, InstructionDataset],
         logger: Union[Logger, Iterable[Logger], bool] = True,
     ):
@@ -254,15 +261,23 @@
 class CausalLoraInt8Model(CausalLoraModel):
     def __init__(
         self,
         engine: str,
         weights_path: Optional[str] = None,
         model_name: Optional[str] = None,
         target_modules: Optional[List[str]] = None,
+        **kwargs,
     ):
         assert_not_cpu_int8()
         super().__init__(
             engine,
             weights_path=weights_path,
             model_name=model_name,
             target_modules=target_modules,
+            **kwargs,
         )
+        
+
+class CausalLoraKbitModel(CausalLoraModel):
+    def __init__(self, engine: str, weights_path: Optional[str] = None):
+        assert_not_cpu_int8()
+        super().__init__(engine, weights_path)
```

### Comparing `xturing-0.1.5/src/xturing/models/cerebras.py` & `xturing-0.1.6/src/xturing/models/cerebras.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/models/distilgpt2.py` & `xturing-0.1.6/src/xturing/models/distilgpt2.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/models/falcon.py` & `xturing-0.1.6/src/xturing/models/falcon.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import Optional
 
 from xturing.engines.falcon_engine import (
     FalconEngine,
     FalconInt8Engine,
     FalconLoraEngine,
     FalconLoraInt8Engine,
+    FalconLoraKbitEngine,
 )
 from xturing.models.causal import (
     CausalInt8Model,
     CausalLoraInt8Model,
+    CausalLoraKbitModel,
     CausalLoraModel,
     CausalModel,
 )
 
 
 class Falcon(CausalModel):
     config_name: str = "falcon"
@@ -36,7 +38,14 @@
 
 
 class FalconLoraInt8(CausalLoraInt8Model):
     config_name: str = "falcon_lora_int8"
 
     def __init__(self, weights_path: Optional[str] = None):
         super().__init__(FalconLoraInt8Engine.config_name, weights_path)
+
+
+class FalconLoraKbit(CausalLoraKbitModel):
+    config_name: str = "falcon_lora_kbit"
+
+    def __init__(self, weights_path: Optional[str] = None):
+        super().__init__(FalconLoraKbitEngine.config_name, weights_path)
```

### Comparing `xturing-0.1.5/src/xturing/models/galactica.py` & `xturing-0.1.6/src/xturing/models/galactica.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/models/gpt2.py` & `xturing-0.1.6/src/xturing/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/models/gptj.py` & `xturing-0.1.6/src/xturing/models/gptj.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/models/llama.py` & `xturing-0.1.6/src/xturing/models/llama.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from typing import Iterable, List, Optional, Union
+
 from pytorch_lightning.loggers import Logger
 
+from xturing.datasets.instruction_dataset import InstructionDataset
+from xturing.datasets.text_dataset import TextDataset
 from xturing.engines.llama_engine import (
     LLamaEngine,
     LLamaInt8Engine,
     LlamaLoraEngine,
     LlamaLoraInt8Engine,
-    LlamaLoraInt4Engine,
+    LlamaLoraKbitEngine,
 )
 from xturing.models.causal import (
     CausalInt8Model,
     CausalLoraInt8Model,
+    CausalLoraKbitModel,
     CausalLoraModel,
     CausalModel,
 )
 from xturing.trainers.base import BaseTrainer
-from xturing.datasets.instruction_dataset import InstructionDataset
-from xturing.datasets.text_dataset import TextDataset
 from xturing.trainers.lightning_trainer import LightningTrainer
 
 
 class Llama(CausalModel):
     config_name: str = "llama"
 
     def __init__(self, weights_path: Optional[str] = None):
@@ -44,29 +46,32 @@
 class LlamaLoraInt8(CausalLoraInt8Model):
     config_name: str = "llama_lora_int8"
 
     def __init__(self, weights_path: Optional[str] = None):
         super().__init__(LlamaLoraInt8Engine.config_name, weights_path)
 
 
-class LlamaLoraInt4(CausalLoraInt8Model):
-    config_name: str = "llama_lora_int4"
+class LlamaLoraKbit(CausalLoraKbitModel):
+    config_name: str = "llama_lora_kbit"
 
-    def _make_trainer(self, dataset: Union[TextDataset, InstructionDataset], 
-                      logger: Union[Logger, Iterable[Logger], bool] = True):
-        return BaseTrainer.create(
-            LightningTrainer.config_name,
-            self.engine,
-            dataset,
-            self._make_collate_fn(dataset),
-            int(self.finetuning_args.num_train_epochs),
-            int(self.finetuning_args.batch_size),
-            float(self.finetuning_args.learning_rate),
-            self.finetuning_args.optimizer_name,
-            True,
-            True,
-            lora_type=32,
-            logger=logger,
-        )
+    # def _make_trainer(
+    #     self,
+    #     dataset: Union[TextDataset, InstructionDataset],
+    #     logger: Union[Logger, Iterable[Logger], bool] = True,
+    # ):
+    #     return BaseTrainer.create(
+    #         LightningTrainer.config_name,
+    #         self.engine,
+    #         dataset,
+    #         self._make_collate_fn(dataset),
+    #         int(self.finetuning_args.num_train_epochs),
+    #         int(self.finetuning_args.batch_size),
+    #         float(self.finetuning_args.learning_rate),
+    #         self.finetuning_args.optimizer_name,
+    #         True,
+    #         True,
+    #         lora_type=32,
+    #         logger=logger,
+    #     )
 
     def __init__(self, weights_path: Optional[str] = None):
-        super().__init__(LlamaLoraInt4Engine.config_name, weights_path)
+        super().__init__(LlamaLoraKbitEngine.config_name, weights_path)
```

### Comparing `xturing-0.1.5/src/xturing/models/opt.py` & `xturing-0.1.6/src/xturing/models/opt.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/models/stable_diffusion.py` & `xturing-0.1.6/src/xturing/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/preprocessors/instruction_collator.py` & `xturing-0.1.6/src/xturing/preprocessors/instruction_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/preprocessors/text_collator.py` & `xturing-0.1.6/src/xturing/preprocessors/text_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/registry.py` & `xturing-0.1.6/src/xturing/registry.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/self_instruct/bootstrap_instructions.py` & `xturing-0.1.6/src/xturing/self_instruct/bootstrap_instructions.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/self_instruct/generate_instances.py` & `xturing-0.1.6/src/xturing/self_instruct/generate_instances.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/self_instruct/identify_if_classification.py` & `xturing-0.1.6/src/xturing/self_instruct/identify_if_classification.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/self_instruct/prepare_for_finetuning.py` & `xturing-0.1.6/src/xturing/self_instruct/prepare_for_finetuning.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/self_instruct/prepare_seed_tasks.py` & `xturing-0.1.6/src/xturing/self_instruct/prepare_seed_tasks.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/self_instruct/templates/clf_task_template.py` & `xturing-0.1.6/src/xturing/self_instruct/templates/clf_task_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/self_instruct/templates/instance_gen_template.py` & `xturing-0.1.6/src/xturing/self_instruct/templates/instance_gen_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/trainers/lightning_trainer.py` & `xturing-0.1.6/src/xturing/trainers/lightning_trainer.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/ui/playground.py` & `xturing-0.1.6/src/xturing/ui/playground.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/utils/hub.py` & `xturing-0.1.6/src/xturing/utils/hub.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/utils/logging.py` & `xturing-0.1.6/src/xturing/utils/logging.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/utils/loss_fns.py` & `xturing-0.1.6/src/xturing/utils/loss_fns.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/utils/notebooks.py` & `xturing-0.1.6/src/xturing/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/utils/text_splitter.py` & `xturing-0.1.6/src/xturing/utils/text_splitter.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing/utils/utils.py` & `xturing-0.1.6/src/xturing/utils/utils.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.5/src/xturing.egg-info/PKG-INFO` & `xturing-0.1.6/src/xturing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.1.5
+Version: 0.1.6
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -258,29 +258,23 @@
 - Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning) to reduce hardware costs by up to 90%
 - Explore different fine-tuning methods and benchmark them to find the best performing model
 - Evaluate fine-tuned models on well-defined metrics for in-depth analysis
 
 <br>
 
 ## 🌟 What's new?
-We are excited to announce the latest enhancements to our `xTuring` library: Falcon LLM integration and Generic model support. With this update, you can use and finetune Falcon-7B model with the off-the-shelf, off-the-shelf with INT8 precision, with LoRA architecture, and LoRA architecture with INT8 precision. Moreover, in case you do not find a model you want to run in the models' list, you can still us `xTuring` to run with the new `GenericModel` wrapper available to you. This new integration allows you to test and finetune any new model on xTuring without waiting for it to be integrated.
+We are excited to announce the latest enhancements to our `xTuring` library:
+1. __`Falcon LLM` integration__ - You can use and fine-tune the _`Falcon-7B`_ model in different configurations: _off-the-shelf_, _off-the-shelf with INT8 precision_, _LoRA fine-tuning_, and _LoRA fine-tuning with INT8 precision_.
+2. __`GenericModel` wrapper__ - This new integration allows you to test and fine-tune any new model on `xTuring` without waiting for it to be integrated using class _`GenericModel`_.
 
 You can check the  [Falcon LoRA INT8 working example](examples/falcon/falcon_lora_int8.py) repository to see how it works.
 Also, you can check the  [GenericModel working example](examples/generic/generic_model.py) repository to see how it works.
 
 <br>
 
-## CLI playground
-<img src=".github/cli-playground.gif" width="100%" style="margin: 0 1%;"/>
-
-## UI playground
-<img src=".github/ui-playground2.gif" width="100%" style="margin: 0 1%;"/>
-
-<br>
-
 ## ⚙️ Installation
 ```bash
 pip install xturing
 ```
 
 <br>
 
@@ -304,14 +298,43 @@
 print("Generated output by the model: {}".format(output))
 ```
 
 You can find the data folder [here](examples/llama/alpaca_data).
 
 <br>
 
+## CLI playground
+<img src=".github/cli-playground.gif" width="80%" style="margin: 0 1%;"/>
+
+```bash
+$ xturing chat -m "<path-to-model-folder>"
+
+```
+
+## UI playground
+<img src=".github/ui-playground2.gif" width="80%" style="margin: 0 1%;"/>
+
+```python
+from xturing.datasets import InstructionDataset
+from xturing.models import BaseModel
+from xturing.ui import Playground
+
+dataset = InstructionDataset("./alpaca_data")
+model = BaseModel.create("<model_name>")
+
+model.finetune(dataset=dataset)
+
+model.save("llama_lora_finetuned")
+
+Playground().launch() ## launches localhost UI
+
+```
+
+<br>
+
 ## 📚 Tutorials
 - [Preparing your dataset](examples/llama/preparing_your_dataset.py)
 - [Cerebras-GPT fine-tuning with LoRA and INT8](examples/cerebras/cerebras_lora_int8.ipynb) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eKq3oF7dnK8KuIfsTE70Gvvniwr1O9D0?usp=sharing)
 - [Cerebras-GPT fine-tuning with LoRA](examples/cerebras/cerebras_lora.ipynb) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VjqQhstm5pT4EjPjx4Je7b3W2X1V3vDo?usp=sharing)
 - [LLaMA fine-tuning with LoRA and INT8](examples/llama/llama_lora_int8.py) &ensp; [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1SQUXq1AMZPSLD4mk3A3swUIc6Y2dclme?usp=sharing)
 - [LLaMA fine-tuning with LoRA](examples/llama/llama_lora.py)
 - [LLaMA fine-tuning](examples/llama/llama.py)
@@ -334,19 +357,19 @@
 ```javascript
 {
   'maximum sequence length': 512,
   'batch size': 1,
 }
 ```
 
-|      LLaMA 7B      | DeepSpeed + CPU Offloading | LoRA + DeepSpeed  | LoRA + DeepSpeed + CPU Offloading |
-| --------- | ---- | ---- | ---- |
+|      LLaMA-7B      | DeepSpeed + CPU Offloading | LoRA + DeepSpeed  | LoRA + DeepSpeed + CPU Offloading |
+| :---------: | :----: | :----: | :----: |
 | GPU | 33.5 GB | 23.7 GB | 21.9 GB |
 | CPU | 190 GB  | 10.2 GB | 14.9 GB |
-| Time per epoch | 21 hours  | 20 mins | 20 mins |
+| Time/epoch | 21 hours  | 20 mins | 20 mins |
 
 Contribute to this by submitting your performance results on other GPUs by creating an issue with your hardware specifications, memory consumption and time per epoch.
 
 <br>
 
 ## 📎 Fine-tuned model checkpoints
 We have already fine-tuned some models that you can use as your base or start playing with.
@@ -361,25 +384,27 @@
 |---------------------|--------|---------------|
 | DistilGPT-2 LoRA | alpaca | `x/distilgpt2_lora_finetuned_alpaca` |
 | LLaMA LoRA          | alpaca | `x/llama_lora_finetuned_alpaca` |
 
 <br>
 
 ## 📈 Roadmap
-- [x] Support for LLaMA, GPT-J, GPT-2, OPT, Cerebras-GPT, Galactica and Bloom models
+- [x] Support for `LLaMA`, `GPT-J`, `GPT-2`, `OPT`, `Cerebras-GPT`, `Galactica` and `Bloom` models
 - [x] Dataset generation using self-instruction
 - [x] Low-precision LoRA fine-tuning and unsupervised fine-tuning
 - [x] INT8 low-precision fine-tuning support
 - [x] OpenAI, Cohere and AI21 Studio model APIs for dataset generation
 - [x] Added fine-tuned checkpoints for some models to the hub
 - [x] INT4 LLaMA LoRA fine-tuning demo
 - [x] INT4 LLaMA LoRA fine-tuning with INT4 generation
-- [x] Support for a generic model wrapper
-- [x] Support for Falcon-7B model
+- [x] Support for a `Generic model` wrapper
+- [x] Support for `Falcon-7B` model
+- [X] INT4 low-precision fine-tuning support
 - [ ] Evaluation of LLM models
+- [ ] INT3, INT2, INT1 low-precision fine-tuning support
 - [ ] Support for Stable Diffusion
 
 <br>
 
 ## 🤝 Help and Support
 If you have any questions, you can create an issue on this repository.
```

### Comparing `xturing-0.1.5/src/xturing.egg-info/SOURCES.txt` & `xturing-0.1.6/src/xturing.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,19 @@
 src/xturing/engines/llama_utils/__init__.py
 src/xturing/engines/llama_utils/llama.py
 src/xturing/engines/lora_engine/__init__.py
 src/xturing/engines/lora_engine/lora.py
 src/xturing/engines/lora_engine/save_and_load.py
 src/xturing/engines/lora_engine/test.py
 src/xturing/engines/quant_utils/__init__.py
+src/xturing/engines/quant_utils/cachedistillationoutputs.py
 src/xturing/engines/quant_utils/custom_autotune.py
+src/xturing/engines/quant_utils/lrec.py
+src/xturing/engines/quant_utils/peft_utils.py
+src/xturing/engines/quant_utils/qerdataloading.py
 src/xturing/engines/quant_utils/quant.py
 src/xturing/model_apis/__init__.py
 src/xturing/model_apis/ai21.py
 src/xturing/model_apis/base.py
 src/xturing/model_apis/cohere.py
 src/xturing/model_apis/openai.py
 src/xturing/models/__init__.py
```


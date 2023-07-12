# Comparing `tmp/zerospeech-benchmarks-0.9.1.tar.gz` & `tmp/zerospeech-benchmarks-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerospeech-benchmarks-0.9.1.tar", last modified: Mon Feb 27 12:34:52 2023, max compression
+gzip compressed data, was "zerospeech-benchmarks-0.9.2.tar", last modified: Wed Jul 12 14:54:32 2023, max compression
```

## Comparing `zerospeech-benchmarks-0.9.1.tar` & `zerospeech-benchmarks-0.9.2.tar`

### file list

```diff
@@ -1,139 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.912589 zerospeech-benchmarks-0.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.892588 zerospeech-benchmarks-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.896588 zerospeech-benchmarks-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/.github/workflows/build-conda-recipe.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/.github/workflows/pipy-pyblish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    47679 2023-02-27 12:34:52.912589 zerospeech-benchmarks-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/TODO.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.896588 zerospeech-benchmarks-0.9.1/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/conda-recipe/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.896588 zerospeech-benchmarks-0.9.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.900589 zerospeech-benchmarks-0.9.1/examples/benchmark_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/examples/benchmark_examples/abx17.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/examples/benchmark_examples/abxLS.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/examples/benchmark_examples/prosAudit.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/examples/benchmark_examples/sLM21.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/examples/benchmark_examples/tde17.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/examples/zr_testing.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.900589 zerospeech-benchmarks-0.9.1/imgs/
--rw-r--r--   0 runner    (1001) docker     (123)    72584 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/imgs/checkpoints.png
--rw-r--r--   0 runner    (1001) docker     (123)    58400 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/imgs/datasets.png
--rw-r--r--   0 runner    (1001) docker     (123)    77287 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/imgs/samples.png
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 12:34:52.912589 zerospeech-benchmarks-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.900589 zerospeech-benchmarks-0.9.1/zerospeech/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.900589 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.900589 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.900589 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_17/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_17/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_17/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_17/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_17/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.904589 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_LS/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_LS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_LS/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_LS/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_LS/instructions.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_LS/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_LS/scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_LS/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.904589 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/pros_audit/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/pros_audit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/pros_audit/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/pros_audit/instructions.md
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/pros_audit/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/pros_audit/submission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.904589 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/sLM_21/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/sLM_21/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/sLM_21/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/sLM_21/instructions.md
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/sLM_21/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/sLM_21/scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/sLM_21/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/sLM_21/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.904589 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/tde_17/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/tde_17/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/tde_17/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/tde_17/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/tde_17/instructions.md
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/tde_17/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/tde_17/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.904589 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/datasets/zrc_2015.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/datasets/zrc_2017.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/datasets/zrc_2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/datasets/zrc_2021.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.904589 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.904589 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/abx/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/abx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.908589 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/abx/abx_librispeech/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/abx/abx_librispeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/abx/abx_librispeech/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/abx/abx_librispeech/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.908589 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/abx/abx_phoneme/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/abx/abx_phoneme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/abx/abx_phoneme/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/abx/abx_phoneme/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.908589 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/lm/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/lm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/lm/lexical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/lm/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/lm/prosody.py
--rw-r--r--   0 runner    (1001) docker     (123)     8641 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/lm/semantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/lm/syntactic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/tde.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.908589 zerospeech-benchmarks-0.9.1/zerospeech/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/cmd/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/cmd/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/cmd/cli_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/cmd/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/cmd/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/cmd/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/cmd/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/cmd/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/cmd/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/data_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.912589 zerospeech-benchmarks-0.9.1/zerospeech/model/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/model/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/model/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/model/data_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/model/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/model/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/model/meta_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/model/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/model/score_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/networkio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/startup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.912589 zerospeech-benchmarks-0.9.1/zerospeech/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.912589 zerospeech-benchmarks-0.9.1/zerospeech/validators/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/validators/base_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-02-27 12:34:37.000000 zerospeech-benchmarks-0.9.1/zerospeech/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:34:52.912589 zerospeech-benchmarks-0.9.1/zerospeech_benchmarks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47679 2023-02-27 12:34:52.000000 zerospeech-benchmarks-0.9.1/zerospeech_benchmarks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-02-27 12:34:52.000000 zerospeech-benchmarks-0.9.1/zerospeech_benchmarks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 12:34:52.000000 zerospeech-benchmarks-0.9.1/zerospeech_benchmarks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-27 12:34:52.000000 zerospeech-benchmarks-0.9.1/zerospeech_benchmarks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-27 12:34:52.000000 zerospeech-benchmarks-0.9.1/zerospeech_benchmarks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-27 12:34:52.000000 zerospeech-benchmarks-0.9.1/zerospeech_benchmarks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.986902 zerospeech-benchmarks-0.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.958901 zerospeech-benchmarks-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.966901 zerospeech-benchmarks-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/.github/workflows/build-conda-recipe.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/.github/workflows/pipy-pyblish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    47928 2023-07-12 14:54:32.986902 zerospeech-benchmarks-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.966901 zerospeech-benchmarks-0.9.2/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/conda-recipe/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.966901 zerospeech-benchmarks-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/docs/abx17.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/docs/abxLS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/docs/prosAudit.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/docs/sLM21.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/docs/tde17.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.966901 zerospeech-benchmarks-0.9.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.966901 zerospeech-benchmarks-0.9.2/examples/benchmark_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/examples/benchmark_examples/abx17.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/examples/benchmark_examples/abxLS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/examples/benchmark_examples/prosAudit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/examples/benchmark_examples/sLM21.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/examples/benchmark_examples/tde17.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/examples/zr_testing.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.966901 zerospeech-benchmarks-0.9.2/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)    72584 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/imgs/checkpoints.png
+-rw-r--r--   0 runner    (1001) docker     (123)    58400 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/imgs/datasets.png
+-rw-r--r--   0 runner    (1001) docker     (123)    77287 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/imgs/samples.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:54:32.986902 zerospeech-benchmarks-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.970901 zerospeech-benchmarks-0.9.2/zerospeech/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.970901 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/abx17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/abxLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/prosAudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/sLM21.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/tde17.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.974902 zerospeech-benchmarks-0.9.2/zerospeech/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/cli_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.974902 zerospeech-benchmarks-0.9.2/zerospeech/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/datasets/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2021.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.974902 zerospeech-benchmarks-0.9.2/zerospeech/generics/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/generics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/generics/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/generics/data_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/generics/named_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/generics/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/generics/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/httpw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.978901 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/abxLS.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.978901 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/exporters/abxLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/exporters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/exporters/sLM21.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/exporters/tde17.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/prosaudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/sLM21.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/tde17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/vocolab_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/networkio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/startup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.978901 zerospeech-benchmarks-0.9.2/zerospeech/submissions/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.982902 zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/meta_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/score_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/validation_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/abx17.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/abxLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/prosAudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26111 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/sLM21.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/tde17.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.982902 zerospeech-benchmarks-0.9.2/zerospeech/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.982902 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.982902 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_librispeech/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_librispeech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_librispeech/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_librispeech/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.982902 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_phoneme/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_phoneme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_phoneme/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_phoneme/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.982902 zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/lexical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/prosody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/semantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/syntactic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/tde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.986902 zerospeech-benchmarks-0.9.2/zerospeech/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/upload/file_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/upload/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/upload/user_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.986902 zerospeech-benchmarks-0.9.2/zerospeech/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/validators/base_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.986902 zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47928 2023-07-12 14:54:32.000000 zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-12 14:54:32.000000 zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:54:32.000000 zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-12 14:54:32.000000 zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-12 14:54:32.000000 zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 14:54:32.000000 zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/top_level.txt
```

### Comparing `zerospeech-benchmarks-0.9.1/.github/workflows/build-conda-recipe.yaml` & `zerospeech-benchmarks-0.9.2/.github/workflows/build-conda-recipe.yaml`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/.github/workflows/pipy-pyblish.yaml` & `zerospeech-benchmarks-0.9.2/.github/workflows/pipy-pyblish.yaml`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/LICENSE.txt` & `zerospeech-benchmarks-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/PKG-INFO` & `zerospeech-benchmarks-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerospeech-benchmarks
-Version: 0.9.1
+Version: 0.9.2
 Summary: Toolset for usage of the Zero Resource Challenge Benchmarks.
 Author-email: Nicolas Hamilakis <nicolas.hamilakis@ens.psl.eu>, CoML Team <dev@zerospeech.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -678,20 +678,26 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: documentation, https://zerospeech.com/toolbox/
 Project-URL: homepage, https://zerospeech.com/
 Project-URL: repository, https://github.com/zerospeech/benchmarks
 Keywords: speech,machine-learning,challenges,research-tool,benchmark-speech,zerospeech
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: vocolab
+Provides-Extra: tts019
 Provides-Extra: abx
 Provides-Extra: abx2
 Provides-Extra: tde
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `zerospeech-benchmarks-0.9.1/README.md` & `zerospeech-benchmarks-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/TODO.md` & `zerospeech-benchmarks-0.9.2/TODO.md`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/conda-recipe/meta.yaml` & `zerospeech-benchmarks-0.9.2/conda-recipe/meta.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 {% set name = "zerospeech-benchmarks" %}
-{% set version = "0.9.1" %}
+{% set version = "0.9.2" %}
 
 package:
   name: {{ name|lower }}
   version: {{ version }}
 
 source:
   url: https://pypi.io/packages/source/{{ name[0] }}/{{ name }}/zerospeech-benchmarks-{{ version }}.tar.gz
-  sha256: 8b6ef91a910ac88187f00e35602985b884ed9af259bc8ee7bca90e0798b79cce
+  sha256: 59668c988d80386fa94940dbac3afd4a5ea408f8c0472747abbdd332b86e4d52
 
 build:
   entry_points:
     - zrc = zerospeech.startup:main
   noarch: python
   script: {{ PYTHON }} -m pip install . -vv
   number: 0
@@ -21,15 +21,15 @@
     - python >=3.8
     - setuptools >=45
     - setuptools-scm >=6.2
     - pip
   run:
     - python >=3.8
     - distro
-    - pydantic
+    - pydantic <2.0
     - email_validator >=1.3.0
     - rich
     - pycryptodome
     - pandas
     - numpy
     - scipy
     - humanize
```

### Comparing `zerospeech-benchmarks-0.9.1/examples/benchmark_examples/abx17.ipynb` & `zerospeech-benchmarks-0.9.2/examples/benchmark_examples/abx17.ipynb`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/examples/benchmark_examples/abxLS.ipynb` & `zerospeech-benchmarks-0.9.2/examples/benchmark_examples/abxLS.ipynb`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/examples/benchmark_examples/prosAudit.ipynb` & `zerospeech-benchmarks-0.9.2/examples/benchmark_examples/prosAudit.ipynb`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/examples/benchmark_examples/sLM21.ipynb` & `zerospeech-benchmarks-0.9.2/examples/benchmark_examples/sLM21.ipynb`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/examples/benchmark_examples/tde17.ipynb` & `zerospeech-benchmarks-0.9.2/examples/benchmark_examples/tde17.ipynb`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/imgs/checkpoints.png` & `zerospeech-benchmarks-0.9.2/imgs/checkpoints.png`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/imgs/datasets.png` & `zerospeech-benchmarks-0.9.2/imgs/datasets.png`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/imgs/samples.png` & `zerospeech-benchmarks-0.9.2/imgs/samples.png`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_17/benchmark.py` & `zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/abx17.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import Tuple, List, Dict, ClassVar
+from typing import Tuple, List, Dict, ClassVar, Type
 
 import pandas as pd
 from pydantic import Field
 
-from .data_model import ABX17Submission
-from ...datasets import ZRC2017Dataset
-from ...tasks.abx.abx_librispeech import SimpleABXTask
-from ....model import m_benchmark, m_data_items
+from zerospeech.datasets import ZRC2017Dataset
+from zerospeech.generics import FileListItem, FileItem
+from zerospeech.submissions import Submission
+from zerospeech.submissions.abx17 import ABX17Submission
+from zerospeech.tasks.abx.abx_librispeech import SimpleABXTask
+from ._model import Benchmark
 
-return_type = List[Tuple[str, m_data_items.FileListItem, m_data_items.FileItem]]
+return_type = List[Tuple[str, FileListItem, FileItem]]
 
 
 class ABX17Task(SimpleABXTask):
     """ ABX task for abx-17 """
 
     def format_results(self, results: Dict) -> pd.DataFrame:
         results = [
@@ -20,15 +22,15 @@
             for dset, v in results.items() for mode, score in v.items()
         ]
 
         return pd.DataFrame(
             results, columns=['language', 'duration', 'type', 'score']
         )
 
-    def extract_sets(self, submission: ABX17Submission, dataset: ZRC2017Dataset) -> return_type:
+    def extract_sets(self, submission: "ABX17Submission", dataset: ZRC2017Dataset) -> return_type:
         self.sets = submission.sets
         self.tasks = submission.tasks
         abx_sets = []
         if 'english' in self.tasks:
             if '1s' in self.sets:
                 abx_sets.append((
                     'english_1s',
@@ -122,34 +124,35 @@
                     'wolof_120s',
                     dataset.index.subsets.wolof.items.abx_120s_item,
                     submission.items.wolof_120s
                 ))
         return abx_sets
 
 
-class ABX17Benchmark(m_benchmark.Benchmark):
+class ABX17Benchmark(Benchmark):
     """abx-LS is a benchmark on acoustic Units using the ABX metric.
 
     This benchmark has 2 sub-tasks :
 
     - clean
     - other
 
     Each task has two subsets:  dev, test
     For ABX measuring we use this module : https://github.com/zerospeech/libri-light-abx
     """
     _name: ClassVar[str] = "abx17"
     _doc_url: ClassVar[str] = "https://zerospeech.com/tasks/task_1/tasks_goals/"
+    __submission_cls__: Type[Submission] = ABX17Submission
     dataset: ZRC2017Dataset = Field(default_factory=lambda: ZRC2017Dataset.load())
 
-    def run(self, submission: ABX17Submission):
+    def run(self, submission: "ABX17Submission"):
         """ Run abx-17 tasks """
         params = submission.params
         self.console.print(f'Running {self.name} benchmark on {submission.location.name}')
 
         # create output
         submission.score_dir.mkdir(exist_ok=True, parents=True)
-        task = ABX17Task(**params.get_task())
+        task = ABX17Task.parse_obj(params.get_task())
         task.eval(submission, self.dataset)
 
-        self.console.print(f'[green]:heavy_check_mark:[/green]Evaluation of benchmark completed successfully ')
+        self.console.print('[green]:heavy_check_mark:[/green]Evaluation of benchmark completed successfully ')
         self.console.print(f"Scores can be found @ {submission.score_dir}")
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_17/data_model.py` & `zerospeech-benchmarks-0.9.2/zerospeech/submissions/abx17.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import shutil
 from pathlib import Path
 from typing import Tuple
 
-from ....misc import load_obj
-from ....model import m_benchmark, m_datasets, m_data_items, m_meta_file
-from ...tasks.abx.abx_librispeech import ABXParameters
+from zerospeech.misc import load_obj
+from zerospeech.generics import (
+    FileTypes, FileListItem, Namespace, Item
+)
+from zerospeech.tasks.abx.abx_librispeech import ABXParameters
+from ._model import MetaFile, Submission
 
 
-class ABX17Submission(m_benchmark.Submission):
+class ABX17Submission(Submission):
     """ Submission for ABX-17 """
     sets: Tuple = ('1s', '10s', '120s')
     tasks: Tuple = ('english', 'french', 'mandarin', 'german', 'wolof')
 
     @classmethod
     def load(
             cls, path: Path, *,
@@ -29,94 +32,94 @@
         if not submission.params_file.is_file():
             params = ABXParameters()
             params.result_filename = "scores.csv"
             params.export(submission.params_file)
 
         # Load items
         file_ext = submission.params.score_file_type.replace('.', '')
-        file_ext = m_data_items.FileTypes(file_ext)
+        file_ext = FileTypes(file_ext)
         items = dict()
 
-        if 'english' is tasks:
+        if 'english' in tasks:
             if '1s' in sets:
-                items['english_1s'] = m_data_items.FileListItem.from_dir(
+                items['english_1s'] = FileListItem.from_dir(
                     path / 'english/1s', f_type=file_ext
                 )
             if '10s' in sets:
-                items['english_10s'] = m_data_items.FileListItem.from_dir(
+                items['english_10s'] = FileListItem.from_dir(
                     path / 'english/10s', f_type=file_ext
                 )
             if '120s' in sets:
-                items['english_120s'] = m_data_items.FileListItem.from_dir(
+                items['english_120s'] = FileListItem.from_dir(
                     path / 'english/120s', f_type=file_ext
                 )
         if 'french' in tasks:
             if '1s' in sets:
-                items['french_1s'] = m_data_items.FileListItem.from_dir(
+                items['french_1s'] = FileListItem.from_dir(
                     path / 'french/1s', f_type=file_ext
                 )
             if '10s' in sets:
-                items['french_10s'] = m_data_items.FileListItem.from_dir(
+                items['french_10s'] = FileListItem.from_dir(
                     path / 'french/10s', f_type=file_ext
                 )
             if '120s' in sets:
-                items['french_120s'] = m_data_items.FileListItem.from_dir(
+                items['french_120s'] = FileListItem.from_dir(
                     path / 'french/120s', f_type=file_ext
                 )
         if 'mandarin' in tasks:
             if '1s' in sets:
-                items['mandarin_1s'] = m_data_items.FileListItem.from_dir(
+                items['mandarin_1s'] = FileListItem.from_dir(
                     path / 'mandarin/1s', f_type=file_ext
                 )
             if '10s' in sets:
-                items['mandarin_10s'] = m_data_items.FileListItem.from_dir(
+                items['mandarin_10s'] = FileListItem.from_dir(
                     path / 'mandarin/10s', f_type=file_ext
                 )
             if '120s' in sets:
-                items['mandarin_120s'] = m_data_items.FileListItem.from_dir(
+                items['mandarin_120s'] = FileListItem.from_dir(
                     path / 'mandarin/120s', f_type=file_ext
                 )
         if 'german' in tasks:
             # retro-compatibility with old format
             gloc = path / 'LANG1'
             if not gloc.is_dir():
                 gloc = path / 'german'
 
             if '1s' in sets:
-                items['german_1s'] = m_data_items.FileListItem.from_dir(
+                items['german_1s'] = FileListItem.from_dir(
                     gloc / '1s', f_type=file_ext
                 )
             if '10s' in sets:
-                items['german_10s'] = m_data_items.FileListItem.from_dir(
+                items['german_10s'] = FileListItem.from_dir(
                     gloc / '10s', f_type=file_ext
                 )
             if '120s' in sets:
-                items['german_120s'] = m_data_items.FileListItem.from_dir(
+                items['german_120s'] = FileListItem.from_dir(
                     gloc / '120s', f_type=file_ext
                 )
         if 'wolof' in tasks:
             # retro-compatibility with old format
             gloc = path / 'LANG2'
             if not gloc.is_dir():
                 gloc = path / 'wolof'
 
             if '1s' in sets:
-                items['wolof_1s'] = m_data_items.FileListItem.from_dir(
+                items['wolof_1s'] = FileListItem.from_dir(
                     gloc / '1s', f_type=file_ext
                 )
             if '10s' in sets:
-                items['wolof_10s'] = m_data_items.FileListItem.from_dir(
+                items['wolof_10s'] = FileListItem.from_dir(
                     gloc / '10s', f_type=file_ext
                 )
             if '120s' in sets:
-                items['wolof_120s'] = m_data_items.FileListItem.from_dir(
+                items['wolof_120s'] = FileListItem.from_dir(
                     gloc / '120s', f_type=file_ext
                 )
 
-        submission.items = m_datasets.Namespace[m_data_items.Item](store=items)
+        submission.items = Namespace[Item](store=items)
         return submission
 
     def load_parameters(self) -> "ABXParameters":
         if self.params_file.is_file():
             obj = load_obj(self.params_file)
             return ABXParameters.parse_obj(obj)
         return ABXParameters()
@@ -174,17 +177,17 @@
 
         # scores dir
         (location / 'scores').mkdir(exist_ok=True, parents=True)
 
         # create parameters file
         ABXParameters().export(location / ABXParameters.file_stem)
         # create meta-template
-        template = m_meta_file.MetaFile.to_template(benchmark_name="abx17")
+        template = MetaFile.to_template(benchmark_name="abx17")
         template.to_yaml(
-            file=location / m_meta_file.MetaFile.file_stem,
+            file=location / MetaFile.file_stem,
             excluded={
                 "file_stem": True,
                 "model_info": {"model_id"},
                 "publication": {"bib_reference", "DOI"}
             }
         )
         instruction_file = Path(__file__).parent / "instructions.md"
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_LS/benchmark.py` & `zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/abxLS.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-from typing import Tuple, List, Dict, ClassVar
+from typing import Tuple, List, Dict, ClassVar, Type
 
 import pandas
 import pandas as pd
 from pydantic import Field
 
-from .data_model import AbxLSSubmission
-from ...datasets import AbxLSDataset
-from ...tasks.abx.abx_phoneme import SimpleABXPhonemeTask, ContextMode
-from ....model import m_benchmark, m_data_items
+from zerospeech.datasets import AbxLSDataset
+from zerospeech.generics import (
+    FileItem, FileListItem
+)
+from zerospeech.submissions.abxLS import AbxLSSubmission
+from zerospeech.submissions import Submission
+from zerospeech.tasks.abx.abx_phoneme import SimpleABXPhonemeTask, ContextMode
+from ._model import Benchmark
 
-return_type = Tuple[str, m_data_items.FileItem, m_data_items.FileListItem, ContextMode]
+return_type = Tuple[str, FileItem, FileListItem, ContextMode]
 
 
 class AbxLSTask(SimpleABXPhonemeTask):
     """ ABX task for abx-LS-Rob """
 
     def format_results(self, results: Dict) -> pd.DataFrame:
         formatted_results = []
@@ -144,15 +148,15 @@
                                 submission.items.test_other,
                                 context.phoneme_any
                             ))
 
             return abx_sets
 
 
-class AbxLSBenchmark(m_benchmark.Benchmark):
+class AbxLSBenchmark(Benchmark):
     """ abx-LS-Phoneme is a benchmark on acoustic Units using the ABX metric.
 
     It is a reimplementation of the ABX-LS benchmark with more robust .item files
 
 
     This benchmark has 2 sub-tasks :
 
@@ -160,20 +164,21 @@
     - other
 
     Each task has two subsets:  dev, test
     For ABX measuring we use this module : https://github.com/zerospeech/libri-light-abx2
     """
     _name: ClassVar[str] = "abxLS"
     _doc_url: ClassVar[str] = "https://zerospeech.com/tasks/task_1/tasks_goals/"
+    __submission_cls__: Type[Submission] = AbxLSSubmission
     dataset: AbxLSDataset = Field(default_factory=lambda: AbxLSDataset.load())
 
     def run(self, submission: AbxLSSubmission):
         """ run ABX-LSRob tasks """
         params = submission.params
         self.console.print(f'Running {self.name} benchmark on {submission.location.name}')
         # create output dir
         submission.score_dir.mkdir(exist_ok=True, parents=True)
-        task = AbxLSTask(**params.get_task())
+        task = AbxLSTask.parse_obj(params.get_task())
         task.eval(submission, self.dataset)
 
-        self.console.print(f'[green]:heavy_check_mark:[/green]Evaluation of benchmark completed successfully ')
+        self.console.print('[green]:heavy_check_mark:[/green]Evaluation of benchmark completed successfully ')
         self.console.print(f"Scores can be found @ {submission.score_dir}")
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/abx_LS/instructions.md` & `zerospeech-benchmarks-0.9.2/docs/abxLS.md`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/pros_audit/benchmark.py` & `zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/prosAudit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from typing import ClassVar, TYPE_CHECKING
+from typing import ClassVar, Type
 
 from pydantic import Field
 
-from ...datasets import ProsAuditLMDataset
-from ...tasks.lm import ProsodicTask
-from ....model import m_benchmark
+from zerospeech.datasets import ProsAuditLMDataset
+from zerospeech.submissions import Submission
+from zerospeech.submissions.prosAudit import ProsodySubmission
+from zerospeech.tasks.lm import ProsodicTask
+from ._model import Benchmark
 
-if TYPE_CHECKING:
-    from .submission import ProsodySubmission
 
-
-class SLMProsodyBenchmark(m_benchmark.Benchmark):
+class SLMProsodyBenchmark(Benchmark):
     """ sLMProsody is a benchmark on spoken language Modeling
 
     This benchmark evaluates speech on a prosodic level (todo: expand description a bit)
     """
     _name: ClassVar[str] = "prosAudit"
     _doc_url: ClassVar[str] = "https://zerospeech.com/tasks/task_4/tasks_goals/#prosody"
+    __submission_cls__: Type[Submission] = ProsodySubmission
     dataset: ProsAuditLMDataset = Field(default_factory=lambda: ProsAuditLMDataset.load())
 
     def run(self, submission: "ProsodySubmission"):
         """ Run sLMProsody benchmark """
         params = submission.params
         self.console.print(f'Running {self.name} benchmark on {submission.location.name}')
 
         # create output dir
         submission.score_dir.mkdir(exist_ok=True, parents=True)
         task = ProsodicTask(**params.dict())
         task.eval(submission, self.dataset)
 
-        self.console.print(f'[green]:heavy_check_mark:[/green]Evaluation of benchmark completed successfully ')
+        self.console.print('[green]:heavy_check_mark:[/green]Evaluation of benchmark completed successfully ')
         self.console.print(f"Scores can be found @ {submission.score_dir}")
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/pros_audit/instructions.md` & `zerospeech-benchmarks-0.9.2/docs/prosAudit.md`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/pros_audit/leaderboard.py` & `zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/prosaudit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import List, Dict
 
 from pydantic import BaseModel
 
-from zerospeech.model import m_leaderboard
+from ._models import LeaderboardScores, LeaderboardEntry, Leaderboard
+from ._types import LeaderboardBenchmarkName
 
 
 class ProsAuditScoreEntity(BaseModel):
     score: float
     n: int
     std: float
 
 
-class ProsAuditEntryScores(m_leaderboard.LeaderboardScores):
+class ProsAuditEntryScores(LeaderboardScores):
     protosyntax: Dict[str, ProsAuditScoreEntity]
     lexical: Dict[str, ProsAuditScoreEntity]
 
 
-class ProsAuditLeaderboardEntry(m_leaderboard.LeaderboardEntry):
+class ProsAuditLeaderboardEntry(LeaderboardEntry):
     scores: ProsAuditEntryScores
 
 
-class ProsAuditLeaderboard(m_leaderboard.Leaderboard):
+class ProsAuditLeaderboard(Leaderboard):
+    _type = LeaderboardBenchmarkName.prosAudit
     data: List[ProsAuditLeaderboardEntry]
-    _type = m_leaderboard.Benchmark.prosAudit
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/pros_audit/submission.py` & `zerospeech-benchmarks-0.9.2/zerospeech/submissions/prosAudit.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 from pathlib import Path
 from typing import Optional, Dict
 
 import pandas as pd
 from pydantic import Field
 
 from zerospeech import validators, data_loaders
+from zerospeech.datasets import ProsAuditLMDataset
+from zerospeech.generics import (
+    FileItem, Item, Namespace
+)
+from zerospeech.leaderboards import LeaderboardEntry
+from zerospeech.leaderboards.prosaudit import ProsAuditLeaderboardEntry, ProsAuditEntryScores
 from zerospeech.misc import load_obj
-from zerospeech.model import m_benchmark, m_data_items, m_datasets, m_meta_file, m_leaderboard
-from .leaderboard import ProsAuditLeaderboardEntry, ProsAuditEntryScores
-from ...datasets import ProsAuditLMDataset
-from ...tasks.lm import ProsodyLMParameters
+from zerospeech.tasks.lm import ProsodyLMParameters
+from ._model import ScoreDir, MetaFile, SubmissionValidation, validation_fn, Submission, add_item
 
 
-class ProsodySubmissionValidation(m_benchmark.SubmissionValidation):
+class ProsodySubmissionValidation(SubmissionValidation):
     """ Class that contains all function to validate a ProsAudit Submission"""
     dataset: ProsAuditLMDataset = Field(default_factory=lambda: ProsAuditLMDataset.load())
 
-    @m_benchmark.validation_fn(target="english_dev")
-    def validation_english_dev(self, english_dev: m_data_items.FileItem):
+    @validation_fn(target="english_dev")
+    def validation_english_dev(self, english_dev: FileItem):
         additional_df_checks = [
             # Verify that result df has expected columns
             functools.partial(
                 validators.dataframe_column_check, expected_columns=['score']),
             # Verify that result df has all filenames in set
             functools.partial(
                 validators.dataframe_index_check,
@@ -39,19 +43,19 @@
         ]
 
         # check dataframe
         results = validators.dataframe_check(english_dev, additional_df_checks, sep=' ', header=None,
                                              names=['filename', 'score'], index_col='filename')
 
         # add item tag
-        m_benchmark.add_item('english_dev', results)
+        add_item('english_dev', results)
         return results
 
-    @m_benchmark.validation_fn(target="english_test")
-    def validation_english_dev(self, english_test: m_data_items.FileItem):
+    @validation_fn(target="english_test")
+    def validation_english_dev(self, english_test: FileItem):
         additional_df_checks = [
             # Verify that result df has expected columns
             functools.partial(
                 validators.dataframe_column_check, expected_columns=['score']),
             # Verify that result df has all filenames in set
             functools.partial(
                 validators.dataframe_index_check,
@@ -66,19 +70,19 @@
         ]
 
         # check dataframe
         results = validators.dataframe_check(english_test, additional_df_checks, sep=' ', header=None,
                                              names=['filename', 'score'], index_col='filename')
 
         # add item tag
-        m_benchmark.add_item('english_test', results)
+        add_item('english_test', results)
         return results
 
 
-class ProsAuditScoreDir(m_benchmark.ScoreDir):
+class ProsAuditScoreDir(ScoreDir):
     params = ProsodyLMParameters
 
     @property
     def english_dev_score_by_pair(self) -> Optional[pd.DataFrame]:
         csv_file = self.location / self.params.results_filename.format('english', 'dev', 'by_pair')
         if csv_file.is_file():
             return data_loaders.load_dataframe(csv_file)
@@ -171,26 +175,26 @@
                 train_set=self.meta_file.model_info.train_set,
                 benchmarks=[],
                 gpu_budget=self.meta_file.model_info.gpu_budget,
                 parameters=dict(),
             )
         )
 
-    def build_leaderboard(self) -> m_leaderboard.LeaderboardEntry:
+    def build_leaderboard(self) -> LeaderboardEntry:
         """ Build leaderboard entry """
         self.load_meta()
         return ProsAuditLeaderboardEntry.parse_obj(
             dict(
                 **self.build_meta_data(),
                 scores=self.build_scores()
             )
         )
 
 
-class ProsodySubmission(m_benchmark.Submission):
+class ProsodySubmission(Submission):
     sets = ('dev', 'test')
     tasks = ('english',)
 
     @classmethod
     def load(cls, path: Path, *, sets=('dev', 'test'),
              tasks=('english', 'french', 'japanese')):
         """ Load sLMProsody submission """
@@ -202,19 +206,19 @@
 
         if not submission.params_file.is_file():
             ProsodyLMParameters().export(submission.params_file)
 
         items = dict()
         if 'english' in tasks:
             if 'dev' in sets:
-                items['english_dev'] = m_data_items.FileItem.from_file(path / 'english_dev.txt')
+                items['english_dev'] = FileItem.from_file(path / 'english_dev.txt')
             if 'test' in sets:
-                items['english_test'] = m_data_items.FileItem.from_file(path / 'english_test.txt')
+                items['english_test'] = FileItem.from_file(path / 'english_test.txt')
 
-        submission.items = m_datasets.Namespace[m_data_items.Item](store=items)
+        submission.items = Namespace[Item](store=items)
         return submission
 
     def __zippable__(self):
         """ Files to include in archive """
         return [
             ("", self.meta_file),
             ("", self.params_file),
@@ -229,18 +233,18 @@
         location.mkdir(exist_ok=True, parents=True)
         (location / 'english_dev.txt').touch(exist_ok=True)
         (location / 'english_test.txt').touch(exist_ok=True)
         # scores dir
         (location / 'scores').mkdir(exist_ok=True, parents=True)
         # create parameters file
         # create meta-template
-        template = m_meta_file.MetaFile.to_template(benchmark_name="sLMProsody")
+        template = MetaFile.to_template(benchmark_name="prosAudit")
         ProsodyLMParameters().export(location / ProsodyLMParameters.file_stem)
         template.to_yaml(
-            file=location / m_meta_file.MetaFile.file_stem,
+            file=location / MetaFile.file_stem,
             excluded={
                 "file_stem": True,
                 "model_info": {"model_id"},
                 "publication": {"bib_reference", "DOI"}
             }
         )
         instruction_file = Path(__file__).parent / "instructions.md"
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/sLM_21/instructions.md` & `zerospeech-benchmarks-0.9.2/docs/sLM21.md`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/sLM_21/leaderboard.py` & `zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/sLM21.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 from typing import List, Optional
 
 from pydantic import BaseModel, Field
 
-from zerospeech.model import m_leaderboard
+from ._models import LeaderboardScores, LeaderboardEntry, LeaderboardExtras, Leaderboard
+from ._types import LeaderboardBenchmarkName
 
 
 class LexicalByLength(BaseModel):
     length: int
     dev_score: float = Field(alias="score_dev")
     dev_std: float = Field(alias="std_dev")
     dev_n: float = Field(alias="n_dev")
     test_score: float = Field(alias="score_test")
     test_std: float = Field(alias="std_test")
     test_n: float = Field(alias="n_test")
 
+    class Config:
+        allow_population_by_field_name = True
+
 
 class LexicalByFrequency(BaseModel):
     frequency: str
     dev_score: float = Field(alias="score_dev")
     dev_std: float = Field(alias="std_dev")
     dev_n: float = Field(alias="n_dev")
     test_score: float = Field(alias="score_test")
     test_std: float = Field(alias="std_test")
     test_n: float = Field(alias="n_test")
 
+    class Config:
+        allow_population_by_field_name = True
+
 
 class LexicalExtras(BaseModel):
     by_length: List[LexicalByLength]
     by_frequency: List[LexicalByFrequency]
 
 
 class SyntacticExtras(BaseModel):
@@ -35,23 +42,26 @@
     dev_score: float = Field(alias="score_dev")
     dev_std: float = Field(alias="std_dev")
     dev_n: float = Field(alias="n_dev")
     test_score: float = Field(alias="score_test")
     test_std: float = Field(alias="std_test")
     test_n: float = Field(alias="n_test")
 
+    class Config:
+        allow_population_by_field_name = True
+
 
 class SemanticExtras(BaseModel):
     set: str
     dataset: str
     librispeech: float
     synthetic: float
 
 
-class SLM21Extras(m_leaderboard.LeaderboardExtras):
+class SLM21Extras(LeaderboardExtras):
     lexical: LexicalExtras
     syntactic: List[SyntacticExtras]
     semantic: List[SemanticExtras]
 
 
 class ScoreTuple(BaseModel):
     dev: Optional[float]
@@ -69,21 +79,21 @@
 
 
 class SemanticScores(BaseModel):
     normal: SemanticScoreSets
     weighted: SemanticScoreSets
 
 
-class SLM21Scores(m_leaderboard.LeaderboardScores):
+class SLM21Scores(LeaderboardScores):
     lexical: LexicalScores
     syntactic: ScoreTuple
     semantic: SemanticScores
 
 
-class SLM21LeaderboardEntry(m_leaderboard.LeaderboardEntry):
+class SLM21LeaderboardEntry(LeaderboardEntry):
     scores: SLM21Scores
     extras: SLM21Extras
 
 
-class SLM21Leaderboard(m_leaderboard.Leaderboard):
+class SLM21Leaderboard(Leaderboard):
     data: List[SLM21LeaderboardEntry]
-    _type = m_leaderboard.Benchmark.sLM_21
+    _type = LeaderboardBenchmarkName.sLM_21
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/_benchmarks/tde_17/benchmark.py` & `zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/tde17.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from typing import Tuple, ClassVar
+from typing import Tuple, ClassVar, Type
 
 from pydantic import Field
 
-from .data_model import TDE17Submission
-from ...datasets import ZRC2017Dataset
-from ...tasks import tde
-from ....model import m_benchmark, m_data_items
+from zerospeech.datasets import ZRC2017Dataset
+from zerospeech.generics import FileItem
+from zerospeech.submissions import Submission
+from zerospeech.submissions.tde17 import TDE17Submission
+from zerospeech.tasks import tde
+from ._model import Benchmark
 
 
 class TDE17Task(tde.TDETask):
     tasks: Tuple = ('english', 'french', 'mandarin', 'german', 'wolof')
 
-    def from_submission(self, submission: TDE17Submission, lang: str) -> m_data_items.FileItem:
+    def from_submission(self, submission: "TDE17Submission", lang: str) -> FileItem:
         """ Extract current input class file from submission """
         current_input_classes_file = submission.items.get(lang)
         if current_input_classes_file is None:
             raise ValueError(f'Language {lang} was not found in current submission : {submission.location}')
 
         return current_input_classes_file
 
@@ -28,15 +30,15 @@
         # load gold files
         return tde.Gold(
             wrd_path=str(current_data.items.alignment_words.file),
             phn_path=str(current_data.items.alignment_phones.file)
         )
 
 
-class TDE17Benchmark(m_benchmark.Benchmark):
+class TDE17Benchmark(Benchmark):
     """tde-17 is a benchmark on Spoken term Discovery / Word segmentation
 
     This benchmark has 5 sub-tasks (one for each language)
     - english
     - french
     - mandarin
     - german
@@ -48,23 +50,22 @@
     - 10s has 10-second segments
     - 120s has 120-second segments
 
     For the TDE eval we use this module : https://github.com/zerospeech/tdev2
     """
     _name: ClassVar[str] = "tde17"
     _doc_url: ClassVar[str] = "https://zerospeech.com/tasks/task_2/tasks_goals/"
+    __submission_cls__: Type[Submission] = TDE17Submission
     dataset: "ZRC2017Dataset" = Field(default_factory=lambda: ZRC2017Dataset.load())
 
-    def run(self, submission: TDE17Submission):
+    def run(self, submission: "TDE17Submission"):
         """ Run TDE-17 tasks """
         params = submission.params
         self.console.print(f'Running {self.name} benchmark on {submission.location.name}')
 
         # create output dir
         submission.score_dir.mkdir(exist_ok=True, parents=True)
         task = TDE17Task.parse_obj(params.dict())
         task.eval(submission, self.dataset)
 
-        self.console.print(f'[green]:heavy_check_mark:[/green]Evaluation of benchmark completed successfully ')
+        self.console.print('[green]:heavy_check_mark:[/green]Evaluation of benchmark completed successfully ')
         self.console.print(f"Scores can be found @ {submission.score_dir}")
-
-
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/datasets/zrc_2015.py` & `zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2015.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 import functools
 from typing import Optional, ClassVar
 
-from ...model import m_datasets
+from ._model import Dataset, DatasetNotFoundError, DatasetsDir, DatasetNotInstalledError
 
 
-class ZRC2015Buckeye(m_datasets.Dataset):
+class ZRC2015Buckeye(Dataset):
     """ Class interfacing usage of the ZRC 2019 test dataset """
     __dataset_name__: ClassVar[str] = "zr2015-buckeye"
 
     @classmethod
     @functools.lru_cache
     def load(cls, load_index: bool = True) -> Optional["ZRC2015Buckeye"]:
         """ Loads the dataset """
-        dataset = m_datasets.DatasetsDir.load().get(cls.__dataset_name__, cls=cls)
+        dataset = DatasetsDir.load().get(cls.__dataset_name__, cls=cls)
 
         if dataset is None:
-            raise m_datasets.DatasetNotFoundError(f"The {cls.__dataset_name__} does not exist")
+            raise DatasetNotFoundError(f"The {cls.__dataset_name__} does not exist")
 
         if not dataset.installed:
-            raise m_datasets.DatasetNotInstalledError(f"The {cls.__dataset_name__} is not installed locally")
+            raise DatasetNotInstalledError(f"The {cls.__dataset_name__} is not installed locally")
 
         if load_index:
             dataset.load_index()
             # convert all paths to absolute paths
             dataset.index.make_absolute()
 
         return dataset
 
 
-class ZRC2015NCHLT(m_datasets.Dataset):
+class ZRC2015NCHLT(Dataset):
     """ Class interfacing usage of the ZRC 2019 test dataset """
     __dataset_name__: ClassVar[str] = "zr2015-nchlt-tso"
 
     @classmethod
     @functools.lru_cache
     def load(cls, load_index: bool = True) -> Optional["ZRC2015NCHLT"]:
         """ Loads the dataset """
-        dataset = m_datasets.DatasetsDir.load().get(cls.__dataset_name__, cls=cls)
+        dataset = DatasetsDir.load().get(cls.__dataset_name__, cls=cls)
 
         if dataset is None:
-            raise m_datasets.DatasetNotFoundError(f"The {cls.__dataset_name__} does not exist")
+            raise DatasetNotFoundError(f"The {cls.__dataset_name__} does not exist")
 
         if not dataset.installed:
-            raise m_datasets.DatasetNotInstalledError(f"The {cls.__dataset_name__} is not installed locally")
+            raise DatasetNotInstalledError(f"The {cls.__dataset_name__} is not installed locally")
 
         if load_index:
             dataset.load_index()
             # convert all paths to absolute paths
             dataset.index.make_absolute()
 
         return dataset
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/datasets/zrc_2017.py` & `zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2017.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import functools
 from typing import Optional, ClassVar
 
-from ...model import m_datasets
+from ._model import Dataset, DatasetNotFoundError, DatasetsDir, DatasetNotInstalledError
 
 
-class ZRC2017Dataset(m_datasets.Dataset):
+class ZRC2017Dataset(Dataset):
     """ Class interfacing usage of the ZRC 2017 test dataset """
     __dataset_name__: ClassVar[str] = "zrc2017-test-dataset"
 
     @classmethod
     @functools.lru_cache
     def load(cls, load_index: bool = True) -> Optional["ZRC2017Dataset"]:
         """ Loads the dataset """
-        dataset = m_datasets.DatasetsDir.load().get(cls.__dataset_name__, cls=cls)
+        dataset = DatasetsDir.load().get(cls.__dataset_name__, cls=cls)
 
         if dataset is None:
-            raise m_datasets.DatasetNotFoundError(f"The zrc2017-test-dataset does not exist")
+            raise DatasetNotFoundError(f"The {cls.__dataset_name__} does not exist")
 
         if not dataset.installed:
-            raise m_datasets.DatasetNotInstalledError("The zrc2017-test-dataset is not installed locally")
+            raise DatasetNotInstalledError(f"The {cls.__dataset_name__} is not installed locally")
 
         if load_index:
             dataset.load_index()
             # convert all paths to absolute paths
             dataset.index.make_absolute()
 
         return dataset
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/datasets/zrc_2019.py` & `zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2019.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import functools
 from typing import Optional
 
-from ...model import m_datasets
+from ._model import Dataset, DatasetNotFoundError, DatasetsDir, DatasetNotInstalledError
 
 
-class ZRC2019Dataset(m_datasets.Dataset):
+class ZRC2019Dataset(Dataset):
     """ Class interfacing usage of the ZRC 2019 test dataset """
 
     @classmethod
     @functools.lru_cache
     def load(cls, load_index: bool = True) -> Optional["ZRC2019Dataset"]:
         """ Loads the dataset """
-        dataset = m_datasets.DatasetsDir.load().get("zrc2019-dataset", cls=cls)
+        dataset = DatasetsDir.load().get("zrc2019-dataset", cls=cls)
 
         if dataset is None:
-            raise m_datasets.DatasetNotFoundError(f"The zrc2019-dataset does not exist")
+            raise DatasetNotFoundError("The zrc2019-dataset does not exist")
 
         if not dataset.installed:
-            raise m_datasets.DatasetNotInstalledError("The zrc2019-dataset is not installed locally")
+            raise DatasetNotInstalledError("The zrc2019-dataset is not installed locally")
 
         if load_index:
             dataset.load_index()
             # convert all paths to absolute paths
             dataset.index.make_absolute()
 
         return dataset
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/datasets/zrc_2021.py` & `zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2021.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 import functools
 from typing import Optional, ClassVar
 
-from ...model import m_datasets
+from ._model import Dataset, DatasetNotFoundError, DatasetsDir, DatasetNotInstalledError
 
 
-class SLM21Dataset(m_datasets.Dataset):
+class SLM21Dataset(Dataset):
     """ Class interfacing usage of the sLM21 dataset"""
     __dataset_name__: ClassVar[str] = "sLM21-dataset"
 
     @classmethod
     @functools.lru_cache
     def load(cls, load_index: bool = True) -> Optional["SLM21Dataset"]:
         """ Load dataset from dir registry """
-        dataset = m_datasets.DatasetsDir.load().get(cls.__dataset_name__, cls)
+        dataset = DatasetsDir.load().get(cls.__dataset_name__, cls)
 
         if dataset is None:
-            raise m_datasets.DatasetNotFoundError(f"The sLM21-dataset does not exist")
+            raise DatasetNotFoundError("The sLM21-dataset does not exist")
 
         if not dataset.installed:
-            raise m_datasets.DatasetNotInstalledError("The sLM21-dataset is not installed locally")
+            raise DatasetNotInstalledError("The sLM21-dataset is not installed locally")
 
         if load_index:
             dataset.load_index()
             # convert all paths to absolute paths
             dataset.index.make_absolute()
 
         return dataset
 
 
-class AbxLSDataset(m_datasets.Dataset):
+class AbxLSDataset(Dataset):
     """ Class interfacing usage of the ABX-LS dataset"""
     __dataset_name__: ClassVar[str] = "abxLS-dataset"
 
     @classmethod
     @functools.lru_cache
     def load(cls, load_index: bool = True) -> Optional["AbxLSDataset"]:
         """ Load """
-        dataset = m_datasets.DatasetsDir.load().get(cls.__dataset_name__, cls=cls)
+        dataset = DatasetsDir.load().get(cls.__dataset_name__, cls=cls)
 
         if dataset is None:
-            raise m_datasets.DatasetNotFoundError(f"The abxLS-dataset does not exist")
+            raise DatasetNotFoundError(f"The {cls.__dataset_name__} does not exist")
 
         if not dataset.installed:
-            raise m_datasets.DatasetNotInstalledError("The abxLS-dataset is not installed locally")
+            raise DatasetNotInstalledError(f"The {cls.__dataset_name__} is not installed locally")
 
         if load_index:
             dataset.load_index()
             # convert all paths to absolute paths
             dataset.index.make_absolute()
 
         return dataset
 
 
-class ProsAuditLMDataset(m_datasets.Dataset):
+class ProsAuditLMDataset(Dataset):
     """ Class interfacing usage of the Prosody LM Benchmark """
     __dataset_name__: ClassVar[str] = "prosaudit-dataset"
 
     @classmethod
     @functools.lru_cache
     def load(cls, load_index: bool = True) -> Optional["ProsAuditLMDataset"]:
-        dataset = m_datasets.DatasetsDir.load().get(cls.__dataset_name__, cls=cls)
+        dataset = DatasetsDir.load().get(cls.__dataset_name__, cls=cls)
 
         if dataset is None:
-            raise m_datasets.DatasetNotFoundError(f"The {cls.__dataset_name__} does not exist")
+            raise DatasetNotFoundError(f"The {cls.__dataset_name__} does not exist")
 
         if not dataset.installed:
-            raise m_datasets.DatasetNotInstalledError(f"The {cls.__dataset_name__} is not installed locally")
+            raise DatasetNotInstalledError(f"The {cls.__dataset_name__} is not installed locally")
 
         if load_index:
             dataset.load_index()
             # convert all paths to absolute paths
             dataset.index.make_absolute()
 
         return dataset
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/abx/abx_librispeech/params.py` & `zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_librispeech/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from enum import Enum
 from pathlib import Path
 from typing import Optional, Dict, Any, Literal
 
 import yaml
 
-from .....model import m_benchmark
+from zerospeech.tasks import BenchmarkParameters
 
 
 class ABXMode(str, Enum):
     """ ABX mode of computation """
     all = 'all'
     within = 'within'
     across = 'across'
@@ -29,15 +29,15 @@
     kl_symmetric = 'kl_symmetric'
 
 
 FileNameType = Dict[str, Dict[str, str]]
 FileTypesTXT = Literal['.npy', '.txt']
 
 
-class ABXParameters(m_benchmark.BenchmarkParameters):
+class ABXParameters(BenchmarkParameters):
     # Path to a CPC checkpoint
     path_checkpoint: Optional[str] = None
     # size of a single feature
     feature_size: Optional[float] = float(0.1)
     # Use the GPU to compute distances
     cuda: bool = True
     # Choose the mode of the ABX score to compute
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/abx/abx_librispeech/task.py` & `zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_librispeech/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import abc
 import warnings
 from pathlib import Path
-from typing import Optional, Tuple, Dict, List
+from typing import Optional, Tuple, Dict, List, TYPE_CHECKING
 
 import pandas as pd
 
 try:
     import libriabx
 except ImportError:
     libriabx = ...
     warnings.warn("abx module not installed")
 
 from .params import ABXParameters, ABXMode, ABXDistanceMode
-from .....model import m_benchmark, m_data_items
-from .....settings import get_settings
-from .....out import warning_console
+from zerospeech.generics import FileListItem, FileItem
+from zerospeech.settings import get_settings
+from zerospeech.out import warning_console
+from zerospeech.tasks import Task
+
+if TYPE_CHECKING:
+    from zerospeech.datasets import Dataset
+    from zerospeech.submissions import Submission
 
 st = get_settings()
 
 default_params = ABXParameters()
-extract_return_type = Tuple[str, m_data_items.FileListItem, m_data_items.FileItem]
+extract_return_type = Tuple[str, FileListItem, FileItem]
 
 
-class SimpleABXTask(m_benchmark.Task, abc.ABC):
+class SimpleABXTask(Task, abc.ABC):
     """ Abstract abx-LS task """
     _name = "abx-LS"
     # Path to a CPC checkpoint
     path_checkpoint: Optional[str] = default_params.path_checkpoint
     # size of a single feature
     feature_size: Optional[float] = default_params.feature_size
     # Use the GPU to compute distances
@@ -64,15 +69,15 @@
             )
             # bugfix: _is_mounted is not set by constructor should be fixed in v1.0.6
             abx_args._is_mounted = True
             return abx_args
         else:
             raise ValueError('No abx backend detected')
 
-    def get_abx(self, sub_files: m_data_items.FileListItem, item_file: m_data_items.FileItem) -> Dict[str, float]:
+    def get_abx(self, sub_files: FileListItem, item_file: FileItem) -> Dict[str, float]:
         """  Run abx evaluations on a fileList using a specific .item file
 
         Returns:
             scores<Dict[str, float]>: where keys represent abx mode (across, within) and float represents the score.
         """
         if None in (sub_files, item_file):
             return {f'{t.value}': '-' for t in self.mode.as_set()}
@@ -82,24 +87,24 @@
             res = libriabx.abx_eval(arg_obj)
         else:
             raise ValueError('No abx backend detected')
 
         return res
 
     @abc.abstractmethod
-    def extract_sets(self, submission: m_benchmark.Submission, dataset: m_benchmark.Dataset) -> extract_return_type:
+    def extract_sets(self, submission: "Submission", dataset: "Dataset") -> extract_return_type:
         """ Extract relevant data for abx from submission & dataset """
         pass
 
     @abc.abstractmethod
     def format_results(self, results: Dict) -> pd.DataFrame:
         """ Format the results as a dataframe """
         pass
 
-    def eval(self, submission: m_benchmark.Submission, dataset: m_benchmark.Dataset):
+    def eval(self, submission: "Submission", dataset: "Dataset"):
         """ Simple ABX evaluation """
         output_dir = submission.score_dir
         results = {}
         abx_sets = self.extract_sets(submission, dataset)
 
         if self.cuda:
             warning_console.print("WARNING: gpu mode is set. You can disable this in the parameters.")
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/abx/abx_phoneme/params.py` & `zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_phoneme/params.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 try:
     from zrc_abx2.eval_ABX import SEED
 except ImportError:
     # use this default value if variable does not exist
     SEED = 3459
 
-from .....model import m_benchmark
+from zerospeech.tasks import BenchmarkParameters
 
 
 class ABXFileTypes(str, Enum):
     """ Input file type for abx"""
     pt = '.pt'
     npy = '.npy'
     txt = '.txt'
@@ -76,19 +76,19 @@
     hamming = "hamming"
 
 
 FileNameType = Dict[str, Dict[str, str]]
 FileTypesTXT = Literal['.npy', '.txt']
 
 
-class ABX2Parameters(m_benchmark.BenchmarkParameters):
+class ABX2Parameters(BenchmarkParameters):
     # Path to a CPC checkpoint
     path_checkpoint: Optional[str] = None
     # size of a single feature
-    feature_size: Optional[float] = float(0.1)
+    feature_size: Optional[float] = float(0.01)
     # Use the GPU to compute distances
     cuda: bool = True
     # Choose the mode of the ABX score to compute
     speaker_mode: ABXSpeakerMode = ABXSpeakerMode.all
     # Choose the context type of the ABX score to compute
     context: ContextMode = ContextMode.all
     # Choose the kind of distance to use to compute
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/abx/abx_phoneme/task.py` & `zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_phoneme/task.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 import abc
 import json
 import warnings
 from pathlib import Path
-from typing import Optional, Tuple, Dict, List, Any
+from typing import Optional, Tuple, Dict, List, Any, TYPE_CHECKING
 
 import pandas as pd
 
 try:
     import zrc_abx2
     from vdataset import mount, unmount
 except ImportError:
     zrc_abx2 = ...
     mount, unmount = ..., ...
     warnings.warn("abx2 module not installed")
 
 from .params import ABX2Parameters, ABXSpeakerMode, ABXDistanceMode, ContextMode
-from .....model import m_benchmark, m_data_items
-from .....settings import get_settings
-from .....out import warning_console
+from zerospeech.generics import  FileItem, FileListItem
+from zerospeech.settings import get_settings
+from zerospeech.out import warning_console
+from zerospeech.tasks import Task
+
+if TYPE_CHECKING:
+    from zerospeech.datasets import Dataset
+    from zerospeech.submissions import Submission
 
 st = get_settings()
 
 default_params = ABX2Parameters()
-extract_return_type = Tuple[str, m_data_items.FileItem, m_data_items.FileListItem, ContextMode]
+extract_return_type = Tuple[str, FileItem, FileListItem, ContextMode]
 
 
-class SimpleABXPhonemeTask(m_benchmark.Task, abc.ABC):
+class SimpleABXPhonemeTask(Task, abc.ABC):
     """ Abstract abx-LS task """
     _name = "abx-LS"
     # Path to a CPC checkpoint
     path_checkpoint: Optional[str] = default_params.path_checkpoint
     # size of a single feature
     feature_size: Optional[float] = default_params.feature_size
     # Use the GPU to compute distances
@@ -74,15 +79,15 @@
                 seed=self.seed
             )
             return abx_args
         else:
             raise ValueError('No abx backend detected')
 
     def get_abx(
-            self, sub_files: m_data_items.FileListItem, item_file: m_data_items.FileItem, context: ContextMode
+            self, sub_files: FileListItem, item_file: FileItem, context: ContextMode
     ) -> List[Dict[str, Any]]:
         """  Run abx evaluations on a fileList using a specific .item file
 
         Returns:
             scores<Dict[str, float]>: where keys represent abx mode (across, within) and float represents the score.
         """
         if None in (sub_files, item_file):
@@ -95,25 +100,25 @@
             raise ValueError('No abx backend detected')
 
         # release folder location
         unmount(arg_obj.path_data)
         return res
 
     @abc.abstractmethod
-    def extract_sets(self, submission: m_benchmark.Submission,
-                     dataset: m_benchmark.Dataset, context: ContextMode = ContextMode.all) -> List[extract_return_type]:
+    def extract_sets(self, submission: "Submission",
+                     dataset: "Dataset", context: ContextMode = ContextMode.all) -> List[extract_return_type]:
         """ Extract relevant data for abx from submission & dataset """
         pass
 
     @abc.abstractmethod
     def format_results(self, results: Dict) -> pd.DataFrame:
         """ Format the results as a dataframe """
         pass
 
-    def eval(self, submission: m_benchmark.Submission, dataset: m_benchmark.Dataset):
+    def eval(self, submission: "Submission", dataset: "Dataset"):
         """ Simple Phoneme ABX evaluation """
         output_dir = submission.score_dir
         results = {}
         abx_sets = self.extract_sets(submission, dataset)
 
         if self.cuda:
             warning_console.print("WARNING: gpu mode is set. You can disable this in the parameters.")
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/lm/lexical.py` & `zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/lexical.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from typing import Tuple, TYPE_CHECKING
 
 import pandas as pd
 
 from .params import LexicalParams
-from ....data_loaders import load_dataframe
-from ....model import m_benchmark, m_data_items
+from zerospeech.data_loaders import load_dataframe
+from zerospeech.generics import FileItem
+from zerospeech.tasks import Task
 
 if TYPE_CHECKING:
-    from ..._benchmarks.sLM_21 import SLM21Submission
-    from ...datasets import SLM21Dataset
+    from zerospeech.submissions.sLM21 import SLM21Submission
+    from zerospeech.datasets import SLM21Dataset
 
 
 default_params = LexicalParams()
 
 
-class LexicalTask(m_benchmark.Task):
+class LexicalTask(Task):
     _name = "lexical"
     by_pair: bool = default_params.by_pair
     by_length: bool = default_params.by_length
     by_frequency: bool = default_params.by_frequency
     result_filenames = default_params.result_filenames
     sets: Tuple = ('dev', 'test')
 
     @staticmethod
-    def load_and_format(lexical_item: m_data_items.FileItem, gold_item: m_data_items.FileItem):
+    def load_and_format(lexical_item: FileItem, gold_item: FileItem):
         """ Loads & formats submission data and gold data """
         gold_values = load_dataframe(gold_item, header=0, index_col='filename').astype(
             {'frequency': pd.Int64Dtype()})
 
         lexical_values = load_dataframe(lexical_item, sep=' ', header=None,
                                         names=['filename', 'score'], index_col='filename')
 
@@ -136,15 +137,15 @@
             The score collapsed on word length, the data frame has the
             following columns: 'length', 'score'.
 
         """
         return data.score.groupby(data.length).agg(
             n='count', score='mean', std='std').reset_index()
 
-    def run_lexical_eval(self, lexical_item: m_data_items.FileItem, gold_item: m_data_items.FileItem):
+    def run_lexical_eval(self, lexical_item: FileItem, gold_item: FileItem):
         data = self.load_and_format(lexical_item, gold_item)
         by_pair, by_frequency, by_length = None, None, None
         by_pair = self.eval_by_pair(data)
 
         if self.by_frequency:
             by_frequency = self.eval_by_frequency(by_pair)
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/lm/params.py` & `zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from typing import Any, Dict, Literal
 
 import numpy as np
 import yaml
 from pydantic import BaseModel
 
-from ....model import m_benchmark
+from zerospeech.tasks import BenchmarkParameters
 
 FileNameType = Dict[str, Dict[str, str]]
 
 # using metrics from scipy.spatial.distance.cdist
 _SciPyMetrics = ['braycurtis', 'canberra', 'chebyshev', 'cityblock', 'correlation', 'cosine', 'dice',
                  'euclidean', 'hamming', 'jaccard', 'jensenshannon', 'kulczynski1', 'mahalanobis',
                  'matching', 'minkowski', 'rogerstanimoto', 'russellrao', 'seuclidean',
@@ -108,15 +108,15 @@
         test=dict(
             by_pair='score_syntactic_test_by_pair.csv',
             by_type='score_syntactic_test_by_type.csv'
         )
     )
 
 
-class SLM21BenchmarkParameters(m_benchmark.BenchmarkParameters):
+class SLM21BenchmarkParameters(BenchmarkParameters):
     lexical: LexicalParams = LexicalParams()
     syntactic: SyntacticParams = SyntacticParams()
     semantic: SemanticParams = SemanticParams()
 
     def get_lexical(self) -> Dict[str, Any]:
         return {
             "quiet": self.quiet,
@@ -159,15 +159,15 @@
         # self -> pydict -> yaml leaves those unserialised and the yaml serializer fails.
         # see https://pydantic-docs.helpmanual.io/usage/types/#standard-library-types
         as_obj = json.loads(self.json(exclude=excluded))
         with file.open('w') as fp:
             yaml.dump(as_obj, fp)
 
 
-class ProsodyLMParameters(m_benchmark.BenchmarkParameters):
+class ProsodyLMParameters(BenchmarkParameters):
     """ Parameters for the prosodic benchmark """
     results_filename: str = "score_prosodic_{0}_{1}_{2}.csv"
 
 
     def to_meta(self) -> Dict[str, Any]:
         """ Convert into leaderboard meta entry """
         # filtering non-interfaced param values
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/lm/prosody.py` & `zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/prosody.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import sys
 from typing import TYPE_CHECKING
 
 import pandas as pd
 
+from zerospeech.data_loaders import load_dataframe
+from zerospeech.generics import FileItem
+from zerospeech.tasks import Task
 from .params import ProsodyLMParameters
-from ....model import m_benchmark, m_data_items
-from ....data_loaders import load_dataframe
 
 if TYPE_CHECKING:
-    from ..._benchmarks.pros_audit import ProsodySubmission
-    from ...datasets import ProsAuditLMDataset
+    from zerospeech.submissions.prosAudit import ProsodySubmission
+    from zerospeech.datasets import ProsAuditLMDataset
 
 default_params = ProsodyLMParameters()
 
 
-class ProsodicTask(m_benchmark.Task):
+class ProsodicTask(Task):
     """ Allows computation of the score for the prosodic task (todo: write better desc)"""
     _name = "prosaudit"
     sets = ('dev', 'test')
     tasks = ('english',)
     result_filename: str = default_params.results_filename
 
     @staticmethod
@@ -49,15 +49,15 @@
 
     @staticmethod
     def prosodic_by_type(data: pd.DataFrame) -> pd.DataFrame:
         """Returns a data frame with mean scores by syntax error type"""
         return data.score.groupby([data['type']]).agg(
             n='count', score='mean', std='std').reset_index()
 
-    def run_prosodic_comparison(self, gold: m_data_items.FileItem, sub_file: m_data_items.FileItem):
+    def run_prosodic_comparison(self, gold: FileItem, sub_file: FileItem):
         """ This function create a prosodic comparison based on inputs
 
         data_formatting:
             Each line of the data frame contains a pair of (correct, incorrect) sentences
             and has the following column: 'id', 'filename', 'type', 'correct'
         """
         gold_df = load_dataframe(gold, header=0, index_col='filename')
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/lm/semantic.py` & `zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/semantic.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 
 import joblib
 import numpy as np
 import pandas as pd
 import scipy.spatial
 import scipy.stats
 
+from zerospeech.data_loaders import load_dataframe, load_numpy_array
+from zerospeech.generics import FileItem, FileListItem
+from zerospeech.tasks import Task
 from .params import SemanticParams, SemanticMetrics, SemanticPooling
-from ....data_loaders import load_dataframe, load_numpy_array
-from ....model import m_data_items, benchmark
 
 if TYPE_CHECKING:
-    from ..._benchmarks.sLM_21 import SLM21Submission
+    from zerospeech.submissions.sLM21 import SLM21Submission
     from ...datasets import SLM21Dataset
 
 default_params = SemanticParams()
 
 
-class SemanticTask(benchmark.Task):
+class SemanticTask(Task):
     _name = "semantic"
     metric: SemanticMetrics = default_params.metric
     pooling: SemanticPooling = default_params.pooling
     synthetic: bool = default_params.synthetic
     librispeech: bool = default_params.librispeech
     correlations: bool = default_params.correlations
     n_jobs: int = default_params.n_jobs
@@ -77,15 +78,15 @@
                 y = pool[pool['filename'] == filename_y]['pooling'].item()
                 dist += scipy.spatial.distance.cdist(  # noqa: bad __init__ for scipy.spatial ??
                     np.atleast_2d(x), np.atleast_2d(y), metric=str(self.metric.value))[0][0]
 
             return dist / len(tokens)
 
     def build_file_index(
-            self, synthetic: m_data_items.FileListItem, librispeech: m_data_items.FileListItem
+            self, synthetic: FileListItem, librispeech: FileListItem
     ) -> Dict[str, Dict[str, Path]]:
         file_index = {}
         if self.librispeech:
             file_index['librispeech'] = {
                 f"{p.stem}": p
                 for p in librispeech
             }
@@ -94,15 +95,15 @@
                 f"{p.stem}": p
                 for p in synthetic
             }
 
         return file_index
 
     def semantic_eval(self, file_index: Dict[str, Dict[str, Path]],
-                      gold: m_data_items.FileItem, pairs: m_data_items.FileItem):
+                      gold: FileItem, pairs: FileItem):
         """ Semantically evaluate a subset """
         pairs_df = load_dataframe(pairs, header=0)
         gold_df = load_dataframe(gold, header=0)
 
         if not self.synthetic:
             gold_df = gold_df.drop(gold_df[gold_df['type'] == 'synthetic'].index)
             pairs_df = pairs_df.drop(pairs_df[pairs_df['type'] == 'synthetic'].index)
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/lm/syntactic.py` & `zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/syntactic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import TYPE_CHECKING
 
 import pandas as pd
 
+from zerospeech.data_loaders import load_dataframe
+from zerospeech.generics import FileItem
+from zerospeech.tasks import Task
 from .params import SyntacticParams
-from ....data_loaders import load_dataframe
-from ....model import m_benchmark, m_data_items
 
 if TYPE_CHECKING:
-    from ..._benchmarks.sLM_21 import SLM21Submission
+    from zerospeech.submissions.sLM21 import SLM21Submission
     from ...datasets import SLM21Dataset
 
 default_params = SyntacticParams()
 
 
-class SyntacticTask(m_benchmark.Task):
+class SyntacticTask(Task):
     """Allows the computation of the score by sentences pair and by syntax type."""
     _name = "syntactic"
     sets = ('dev', 'test')
     result_filenames = default_params.result_filenames
 
     @staticmethod
     def syntactic_by_pair(data: pd.DataFrame) -> pd.DataFrame:
@@ -43,15 +44,15 @@
 
     @staticmethod
     def syntactic_by_type(data: pd.DataFrame) -> pd.DataFrame:
         """Returns a data frame with mean scores by syntax error type"""
         return data.score.groupby([data['type']]).agg(
             n='count', score='mean', std='std').reset_index()
 
-    def run_syntactic_comparison(self, gold: m_data_items.FileItem, sub_file: m_data_items.FileItem):
+    def run_syntactic_comparison(self, gold: FileItem, sub_file: FileItem):
         """ This function creates a syntactic comparison based on inputs
 
         data_formatting:
             Each line of the data frame contains a pair of (correct,
         incorrect) sentences and has the following columns: 'id', 'voice', 'type',
         'sentence', 'score sentence', 'non sentence', 'score non sentence'.
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/benchmarks/tasks/tde.py` & `zerospeech-benchmarks-0.9.2/zerospeech/tasks/tde.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 import json
 import os
 import signal
 import sys
-from typing import Tuple, Set
 import warnings
+from typing import Tuple, Set, TYPE_CHECKING
 
 import joblib
 
 try:
     from tde.measures.boundary import Boundary
     from tde.measures.coverage import Coverage
     from tde.measures.grouping import Grouping
@@ -17,28 +17,34 @@
     from tde.readers.disc_reader import Disc
     from tde.readers.gold_reader import Gold
 except ImportError:
     Boundary, Coverage, Grouping, Ned = ..., ..., ..., ...
     TokenType, Disc, Gold = ..., ..., ...
     warnings.warn('tde module was not installed')
 
-from ...model import m_benchmark, m_data_items
+from zerospeech.misc import exit_after
+from zerospeech.generics import FileItem
+from zerospeech.tasks import Task
 
+if TYPE_CHECKING:
+    from zerospeech.datasets import Dataset
+    from zerospeech.submissions import Submission
 
-class TDETask(m_benchmark.Task, abc.ABC):
+
+class TDETask(Task, abc.ABC):
     """ TDE Task """
     _name = "tde-task"
     tasks: Tuple
     metrics: Set = {'grouping', 'matching', 'boundary', 'token_type', 'nlp'}
     n_jobs: int = 1
     result_filename: str = "scores.json"
     grouping_max_time: int = 7200
 
     @staticmethod
-    def read_discovered(item: m_data_items.FileItem, gold: Gold):
+    def read_discovered(item: FileItem, gold: Gold):
         """ Load discovered Intervals """
         # Disc class prints a bunch of nonsense, so we force it to be quiet
         sys.stdout = open(os.devnull, 'w')
         try:
             return Disc(str(item.file), gold)
         finally:
             sys.stdout = sys.__stdout__
@@ -85,34 +91,32 @@
                     coverage=coverage.coverage,
                     npairs=ned.n_pairs
                 ))
             self.console.print(f"NLP computed for {lang} :heavy_check_mark:", style="bold green")
 
         # Grouping
         if 'grouping' in self.metrics:
-            def handler(signum, frame): # noqa: needs to follow signature
-                self.console.print(f'==> Grouping of {lang} takes too long, skipping..', style='red bold')
-                raise TimeoutError('timeout')
-
-            # todo: investigate why a timeout is needed ?
-            # todo investigate if a better way exists to add a timeout
-            signal.signal(signal.SIGALRM, handler)
-            signal.alarm(self.grouping_max_time)
 
-            try:
+            @exit_after(self.grouping_max_time)
+            def compute_grouping():
+                """ Compute grouping within allocated time """
                 with self.console.status(f"Computing {lang} Grouping"):
                     grouping = Grouping(discovered)
                     grouping.compute_grouping()
-                    scores['grouping'].update(dict(
+                    return dict(
                         precision=grouping.precision,
                         recall=grouping.recall,
                         fscore=grouping.fscore
-                    ))
+                    )
+
+            try:
+                grouping_score = compute_grouping()
+                scores['grouping'].update(grouping_score)
                 self.console.print(f"Grouping computed for {lang} :heavy_check_mark:", style="bold green")
-            except TimeoutError:
+            except KeyboardInterrupt:
                 scores['grouping'].update(dict(
                     precision=None,
                     recall=None,
                     fscore=None
                 ))
                 self.console.print(f"Grouping computing for {lang} was aborted due to timeout !!", style="bold red")
 
@@ -120,40 +124,40 @@
             if len(data):
                 return data
             return None
 
         return {m: score_or_none(score) for m, score in scores.items()}
 
     @abc.abstractmethod
-    def from_submission(self, submission: m_benchmark.Submission, lang: str) -> m_data_items.FileItem:
+    def from_submission(self, submission: "Submission", lang: str) -> FileItem:
         """ Extract current input class file from submission """
         pass
 
     @abc.abstractmethod
-    def load_gold(self, dataset: m_benchmark.Dataset, lang: str) -> Gold:
+    def load_gold(self, dataset: "Dataset", lang: str) -> Gold:
         """ Load gold object for current language set """
         pass
 
-    def _eval_lang(self, submission: m_benchmark.Submission, dataset: m_benchmark.Dataset, lang: str):
+    def _eval_lang(self, submission: "Submission", dataset: "Dataset", lang: str):
         """ Evaluate tde for specific language """
         current_input_classes_file = self.from_submission(submission, lang)
-        with self.console.status(f"Loading gold for {lang}..."):
-            gold = self.load_gold(dataset, lang)
+        self.console.print(f"Loading gold for {lang}...")
+        gold = self.load_gold(dataset, lang)
 
         # load discovered intervals
-        with self.console.status(f"Loading disc for {lang}..."):
-            discovered = self.read_discovered(
-                current_input_classes_file, gold
-            )
+        self.console.print(f"Loading class discovery for {lang}...")
+        discovered = self.read_discovered(
+            current_input_classes_file, gold
+        )
 
         # return results
-        self.console(f"Gathering metrics for {lang} ...")
+        self.console.print(f"Gathering metrics for {lang} ...")
         return lang, self.gather_metrics(gold, discovered, lang)
 
-    def eval(self, submission: m_benchmark.Submission, dataset: m_benchmark.Dataset):
+    def eval(self, submission: "Submission", dataset: "Dataset"):
         """ Evaluate the submission """
 
         # Run evaluation with multiprocess if specified
         res = joblib.Parallel(n_jobs=self.n_jobs)(
             joblib.delayed(self._eval_lang)(submission, dataset, lang) for lang in self.tasks
         )
         scores = dict(res)
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/cmd/benchmarks.py` & `zerospeech-benchmarks-0.9.2/zerospeech/cmd/benchmarks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import argparse
 import sys
 from pathlib import Path
 
 from rich.markdown import Markdown
 
+from zerospeech.benchmarks import BenchmarkList
+from zerospeech.out import error_console, warning_console
+from zerospeech.submissions import show_errors
 from .cli_lib import CMD
-from ..benchmarks import BenchmarkList
-from ..model import m_benchmark
-from ..out import error_console, warning_console
 
 
 class BenchmarksCMD(CMD):
     """ List available benchmarks """
     COMMAND = "benchmarks"
     NAMESPACE = ""
 
     def init_parser(self, parser: argparse.ArgumentParser):
+        """ No extra arguments"""
         pass
 
+    # noinspection PyUnresolvedReferences
     def run(self, argv: argparse.Namespace):
         markdown_text = """#### List of Benchmarks\n\n"""
         for nb, bench in enumerate(BenchmarkList):
-            markdown_text += f"{nb+1}) **{bench.value}**\n\n"
-            markdown_text += f"\t{len(bench.value)* '='} documentation ===> [{bench.doc_url}]({bench.doc_url})\n"
+            markdown_text += f"{nb + 1}) **{bench.value}**\n\n"
+            markdown_text += f"\t{len(bench.value) * '='} documentation ===> [{bench.doc_url}]({bench.doc_url})\n"
         self.console.print(Markdown(markdown_text))
 
 
 class BenchmarkRunCMD(CMD):
     """ Run a benchmark """
     COMMAND = "run"
     NAMESPACE = "benchmarks"
@@ -40,57 +42,57 @@
         parser.add_argument("-t", "--tasks", nargs='*', action='store', default=('all',),
                             help="Limit the tasks the benchmark runs")
         parser.add_argument('-q', '--quiet', action='store_true', default=False,
                             help="Do not print information to stdout")
 
     def run(self, argv: argparse.Namespace):
         try:
-            bench = BenchmarkList(argv.name)
+            benchmark_type = BenchmarkList(argv.name)
         except ValueError:
             error_console.log(f"Specified benchmark ({argv.name}) does not exist !!!!")
             warning_console.log(f"Use one of the following : {','.join(b for b in BenchmarkList)}")
             sys.exit(1)
 
+        # Load benchmark
+        benchmark = benchmark_type.benchmark(quiet=argv.quiet)
+
         spinner = self.console.status("Loading submission !")
         spinner.start()
 
         sub_dir = Path(argv.submission_dir)
         if not sub_dir.is_dir():
-            error_console.log(f"Submission directory given does not exist !!!")
+            error_console.log("Submission directory given does not exist !!!")
             sys.exit(1)
 
         load_args = {}
         if 'all' not in argv.sets and len(argv.sets) > 0:
             load_args['sets'] = argv.sets
 
         if 'all' not in argv.tasks and len(argv.sets) > 0:
             load_args['tasks'] = argv.tasks
 
-        submission = bench.submission.load(path=sub_dir, **load_args)
+        submission = benchmark.load_submission(location=sub_dir, **load_args)
         spinner.stop()
         self.console.print(":heavy_check_mark: Submission loaded successfully", style="bold green")
 
         if not argv.skip_validation:
             with self.console.status("Validating submission... ", spinner="aesthetic"):
                 if not submission.valid:
                     error_console.print(f"Found Errors in submission: {submission.location}")
-                    m_benchmark.show_errors(submission.validation_output)
+                    show_errors(submission.validation_output)
                     sys.exit(1)
 
             self.console.print(":heavy_check_mark: Submission Valid", style="bold green")
 
         # load saved parameters
         self.console.print(f"Loaded parameters from :arrow_right: {submission.params_file}")
         submission.params_obj = submission.load_parameters()
-
         # update values from args
         submission.params.quiet = argv.quiet
-
-        # Load & run benchmark
-        benchmark = bench.benchmark(quiet=argv.quiet)
+        # run benchmark
         benchmark.run(submission)
 
 
 class BenchmarksInfoCMD(CMD):
     """ List information on a benchmark """
     COMMAND = "info"
     NAMESPACE = "benchmarks"
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/cmd/checkpoints.py` & `zerospeech-benchmarks-0.9.2/zerospeech/cmd/checkpoints.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import argparse
 
 from rich.padding import Padding
 from rich.table import Table
 
+from zerospeech.generics import checkpoints
+from zerospeech.networkio import check_update_repo_index, update_repo_index
+from zerospeech.out import console, error_console
+from zerospeech.settings import get_settings
 from .cli_lib import CMD
-from ..model import checkpoints
-from ..networkio import check_update_repo_index, update_repo_index
-from ..out import console, error_console
-from ..settings import get_settings
 
 st = get_settings()
 
 
 class CheckpointsCMD(CMD):
     """Manipulate Checkpoints """
     COMMAND = "checkpoints"
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/cmd/cli_lib.py` & `zerospeech-benchmarks-0.9.2/zerospeech/cmd/cli_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import uuid
 from collections import namedtuple
 from typing import Optional, Type
 
 from treelib import Tree, Node
 
-from ..out import console, void_console
+from zerospeech.out import console, void_console
 
 NAMESPACE_SEP = ":"
 LIST_OF_COMMANDS = []
 
 
 class CMD(abc.ABC):
     COMMAND = "<cmd_name>"
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/cmd/datasets.py` & `zerospeech-benchmarks-0.9.2/zerospeech/cmd/datasets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import argparse
 from pathlib import Path
 
-from rich.table import Table
 from rich.padding import Padding
+from rich.table import Table
 
-
+from zerospeech.datasets import DatasetsDir, Dataset
+from zerospeech.networkio import check_update_repo_index, update_repo_index
+from zerospeech.out import console, error_console
+from zerospeech.settings import get_settings
 from .cli_lib import CMD
-from ..model import datasets
-from ..networkio import check_update_repo_index, update_repo_index
-from ..out import console, error_console
-from ..settings import get_settings
 
 st = get_settings()
 
 
 class DatasetCMD(CMD):
     """ Manipulate Datasets """
     COMMAND = "datasets"
     NAMESPACE = ""
 
     def init_parser(self, parser: argparse.ArgumentParser):
         parser.add_argument("--local", action="store_true", help="List local datasets only")
 
     def run(self, argv: argparse.Namespace):
-        datasets_dir = datasets.DatasetsDir.load()
+        datasets_dir = DatasetsDir.load()
 
         table = Table(show_header=True, header_style="bold magenta")
         table.add_column("Name")
         table.add_column("Origin")
         table.add_column("Size")
         table.add_column("Installed")
 
@@ -62,16 +61,16 @@
         parser.add_argument('-q', '--quiet', action='store_true', help='Suppress download info output')
 
     def run(self, argv: argparse.Namespace):
         # update repo index if necessary
         if check_update_repo_index():
             update_repo_index()
 
-        datasets_dir = datasets.DatasetsDir.load()
-        dataset = datasets_dir.get(argv.name, cls=datasets.Dataset)
+        datasets_dir = DatasetsDir.load()
+        dataset = datasets_dir.get(argv.name, cls=Dataset)
         dataset.pull(quiet=argv.quiet, show_progress=True, verify=not argv.skip_verification)
 
 
 class ImportDatasetCMD(CMD):
     """ Import a dataset """
     COMMAND = "import"
     NAMESPACE = "datasets"
@@ -80,30 +79,30 @@
         parser.add_argument('name')
         parser.add_argument('source')
         parser.add_argument('-q', '--quiet', action='store_true', help='Suppress download info output')
 
     def run(self, argv: argparse.Namespace):
         error_console.print("This functionality has not been tested !!!!!")
 
-        datasets_dir = datasets.DatasetsDir.load()
-        dataset = datasets_dir.get(argv.name, cls=datasets.Dataset)
+        datasets_dir = DatasetsDir.load()
+        dataset = datasets_dir.get(argv.name, cls=Dataset)
 
         # import the dataset from source
         dataset.import_(location=Path(argv.source), quiet=argv.quiet, show_progress=True)
 
 
 class RemoveDatasetCMD(CMD):
     """ Remove a dataset item """
     COMMAND = "rm"
     NAMESPACE = "datasets"
 
     def init_parser(self, parser: argparse.ArgumentParser):
         parser.add_argument('name')
 
     def run(self, argv: argparse.Namespace):
-        dataset_dir = datasets.DatasetsDir.load()
+        dataset_dir = DatasetsDir.load()
         dts = dataset_dir.get(argv.name)
         if dts:
             dts.uninstall()
             console.log("[green] Dataset uninstalled successfully !")
         else:
             error_console.log(f"Failed to find dataset named :{argv.name}")
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/cmd/generic.py` & `zerospeech-benchmarks-0.9.2/zerospeech/cmd/generic.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,39 +6,41 @@
 from importlib.metadata import version, PackageNotFoundError
 from typing import Optional
 
 import distro
 from rich.table import Table
 
 from .cli_lib import CMD
-from ..settings import get_settings
-from ..out import error_console, console as std_console
+from zerospeech.settings import get_settings
+from zerospeech.out import error_console, console as std_console
 
 st = get_settings()
 
 
 class ResetIndex(CMD):
     """ Reset remote index """
     COMMAND = "reset-index"
     NAMESPACE = ""
 
     def init_parser(self, parser: argparse.ArgumentParser):
+        """ """
         pass
 
     def run(self, argv: argparse.Namespace):
         st.repository_index.unlink(missing_ok=True)
         std_console.print("Index has been reset successfully !!", style="bold green")
 
 
 class Version(CMD):
     """ Print the current version used """
     COMMAND = "version"
     NAMESPACE = ""
 
     def init_parser(self, parser: argparse.ArgumentParser):
+        """ """
         pass
 
     @staticmethod
     def get_package_version(pkg_name: str) -> Optional[str]:
         try:
             return version(pkg_name)
         except PackageNotFoundError:
@@ -75,31 +77,33 @@
         if torch:
             table.add_row("torch", torch)
         if torchaudio:
             table.add_row("torchaudio", torchaudio)
         table.add_row(end_section=True)
 
         table.add_row("python", sys.version, end_section=True)
-        os_alias = platform.platform(aliased=True)
+        _ = platform.platform(aliased=True)  # os_alias
         if 'linux' in platform.system().lower():
             table.add_row("Operating System", f"{distro.name(pretty=True)}\n{platform.platform(aliased=True)}")
         else:
             table.add_row("Operating System", f"{platform.platform(aliased=True)}")
         std_console.print(table)
 
 
 class HelpCMD(CMD):
     """  """
     COMMAND = "support"
     NAMESPACE = ""
 
     def init_parser(self, parser: argparse.ArgumentParser):
+        """  """
         pass
 
     def run(self, argv: argparse.Namespace):
+        """  """
         pass
 
 
 class AskHelpCMD(CMD):
     """ Send an email to ask for help """
     COMMAND = "email"
     NAMESPACE = "support"
@@ -118,11 +122,12 @@
 
 class DocumentationCMD(CMD):
     """ Opens our documentation """
     COMMAND = "docs"
     NAMESPACE = "support"
 
     def init_parser(self, parser: argparse.ArgumentParser):
+        """  """
         pass
 
     def run(self, argv: argparse.Namespace):
-        webbrowser.open(f'https://zerospeech.com/', new=1)
+        webbrowser.open('https://zerospeech.com/', new=1)
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/cmd/samples.py` & `zerospeech-benchmarks-0.9.2/zerospeech/cmd/samples.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 import argparse
 
 from rich.padding import Padding
 from rich.table import Table
 
+from zerospeech.generics import samples
+from zerospeech.networkio import check_update_repo_index, update_repo_index
+from zerospeech.out import console, error_console
+from zerospeech.settings import get_settings
 from .cli_lib import CMD
-from ..model import samples
-from ..networkio import check_update_repo_index, update_repo_index
-from ..out import console, error_console
-from ..settings import get_settings
 
 st = get_settings()
 
 
 class SamplesCMD(CMD):
     """ Manipulate Samples """
     COMMAND = "samples"
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/cmd/submission.py` & `zerospeech-benchmarks-0.9.2/zerospeech/cmd/submission.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,58 @@
 import argparse
 import sys
 from pathlib import Path
 
+from zerospeech.benchmarks import BenchmarkList
+from zerospeech.out import error_console, warning_console, console as std_console
+from zerospeech.submissions import MetaFile, show_errors
+from zerospeech.tasks import BenchmarkParameters
 from .cli_lib import CMD
-from ..benchmarks import BenchmarkList
-from ..model import m_benchmark, m_meta_file
-from ..out import error_console, warning_console, console as std_console
 
 
 class Submission(CMD):
     """ Submission manager subcommand """
     COMMAND = "submission"
     NAMESPACE = ""
 
     def init_parser(self, parser: argparse.ArgumentParser):
         parser.print_help()
 
     def run(self, argv: argparse.Namespace):
+        """ """
         pass
 
 
 class SubmissionInit(CMD):
     """ Initialise a directory for a specific benchmark """
     COMMAND = "init"
     NAMESPACE = "submission"
 
     def init_parser(self, parser: argparse.ArgumentParser):
         parser.add_argument("name")
         parser.add_argument("location")
 
     def run(self, argv: argparse.Namespace):
         try:
-            bench = BenchmarkList(argv.name)
+            benchmark_type = BenchmarkList(argv.name)
         except ValueError:
             error_console.log(f"Specified benchmark ({argv.name}) does not exist !!!!")
             warning_console.log(f"Use one of the following : {','.join(b for b in BenchmarkList)}")
             sys.exit(1)
 
+        # Load benchmark
+        benchmark = benchmark_type.benchmark(quiet=argv.quiet)
+
         location = Path(argv.location)
         if location.is_dir():
-            error_console.log(f"Location specified already exists !!!")
+            error_console.log("Location specified already exists !!!")
             sys.exit(2)
 
         with std_console.status("Initialising submission dir"):
-            bench.submission.init_dir(location)
+            benchmark.init_submission_dir(location)
 
         std_console.print(f"Submission directory created @ {location}", style="green bold")
 
 
 class BenchmarkParamsCMD(CMD):
     """ Create template params.yaml """
     COMMAND = "params"
@@ -56,38 +61,41 @@
     def init_parser(self, parser: argparse.ArgumentParser):
         parser.add_argument("submission_dir")
         parser.add_argument('-r', '--reset', action="store_true", help="Reset params.yaml to default values")
 
     def run(self, argv: argparse.Namespace):
         location = Path(argv.submission_dir)
         if not location.is_dir():
-            error_console(f"Location specified does not exist !!!")
+            error_console("Location specified does not exist !!!")
             sys.exit(2)
 
         benchmark_name = None
         try:
-            benchmark_name = m_meta_file.MetaFile.benchmark_from_submission(location)
+            benchmark_name = MetaFile.benchmark_from_submission(location)
             if benchmark_name is None:
                 raise TypeError("benchmark not found")
 
-            bench = BenchmarkList(benchmark_name)
+            benchmark_type = BenchmarkList(benchmark_name)
         except TypeError:
-            error_console.log(f"Specified submission does not have a valid {m_meta_file.MetaFile.file_stem}"
+            error_console.log(f"Specified submission does not have a valid {MetaFile.file_stem}"
                               f"\nCannot find benchmark type")
             sys.exit(1)
         except ValueError:
             error_console.log(f"Specified benchmark ({benchmark_name}) does not exist !!!!")
             warning_console.log(f"Use one of the following : {','.join(b for b in BenchmarkList)}")
             sys.exit(1)
 
+        # Load benchmark
+        benchmark = benchmark_type.benchmark(quiet=argv.quiet)
+
         if argv.reset:
             # remove old params file if exists
-            (location / m_benchmark.BenchmarkParameters.file_stem).unlink(missing_ok=True)
+            (location / BenchmarkParameters.file_stem).unlink(missing_ok=True)
 
-        submission = bench.submission.load(path=location)
+        submission = benchmark.load_submission(location)
         if argv.reset:
             self.console.log(f"Params file created/reset at @ {submission.params_file}")
 
         self.console.print(submission.params)
 
 
 class SubmissionVerify(CMD):
@@ -97,35 +105,37 @@
 
     def init_parser(self, parser: argparse.ArgumentParser):
         parser.add_argument("location")
 
     def run(self, argv: argparse.Namespace):
         location = Path(argv.location)
         if not location.is_dir():
-            error_console(f"Location specified does not exist !!!")
+            error_console("Location specified does not exist !!!")
             sys.exit(2)
 
         benchmark_name = None
         try:
-            benchmark_name = m_meta_file.MetaFile.benchmark_from_submission(location)
+            benchmark_name = MetaFile.benchmark_from_submission(location)
             if benchmark_name is None:
                 raise TypeError("benchmark not found")
 
-            bench = BenchmarkList(benchmark_name)
+            benchmark_type = BenchmarkList(benchmark_name)
         except TypeError:
-            error_console.log(f"Specified submission does not have a valid {m_meta_file.MetaFile.file_stem}"
+            error_console.log(f"Specified submission does not have a valid {MetaFile.file_stem}"
                               f"\nCannot find benchmark type")
             sys.exit(1)
         except ValueError:
             error_console.log(f"Specified benchmark ({benchmark_name}) does not exist !!!!")
             warning_console.log(f"Use one of the following : {','.join(b for b in BenchmarkList)}")
             sys.exit(1)
 
-        submission = bench.submission.load(location)
+        # Load benchmark
+        benchmark = benchmark_type.benchmark(quiet=argv.quiet)
+        submission = benchmark.load_submission(location)
         with std_console.status(f"Validating submission @ {location}"):
             _ = submission.valid
 
         if submission.valid:
             std_console.print(f"Submission @ {location} is a valid submission for {bench} :heavy_check_mark:",
                               style='bold green')
         else:
-            m_benchmark.show_errors(submission.validation_output)
+            show_errors(submission.validation_output)
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/cmd/user.py` & `zerospeech-benchmarks-0.9.2/zerospeech/cmd/user.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,26 +2,30 @@
 import sys
 
 from rich.prompt import Confirm
 from rich.table import Table
 
 from .cli_lib import CMD
 from ..out import console as std_console, error_console, warning_console
-from ..auth import CurrentUser
+from zerospeech.upload import CurrentUser
 
 
 class User(CMD):
     """ User management command """
     COMMAND = "user"
     NAMESPACE = ""
 
     def init_parser(self, parser: argparse.ArgumentParser):
+        """ """
         pass
 
     def run(self, argv: argparse.Namespace):
+        std_console.print("Feature Not Yet Available !!!", style="red bold")
+
+    def _run(self, argv: argparse.Namespace):
         current = CurrentUser.load()
         if current is None:
             error_console.print("No current user session, please use login to create a session !")
             sys.exit(1)
 
         table = Table(show_header=False)
         table.add_column("****")
@@ -37,17 +41,21 @@
 
 class UserLogin(CMD):
     """ User loging to the zerospeech.com platform """
     COMMAND = "login"
     NAMESPACE = "user"
 
     def init_parser(self, parser: argparse.ArgumentParser):
+        """ """
         pass
 
     def run(self, argv: argparse.Namespace):
+        std_console.print("Feature Not Yet Available !!!", style="red bold")
+
+    def _run(self, argv: argparse.Namespace):
         if CurrentUser.session_file.is_file():
             CurrentUser.clear()
         try:
             usr = CurrentUser.login()
             std_console.print(f"User {usr.username} was logged in successfully !", style="bold green")
         except ValueError:
             error_console.print("User authentication failed, bad credentials")
@@ -55,13 +63,13 @@
 
 class UserClear(CMD):
     """ Clear the saved login """
     COMMAND = "clear"
     NAMESPACE = "user"
 
     def init_parser(self, parser: argparse.ArgumentParser):
+        """ """
         pass
 
     def run(self, argv: argparse.Namespace):
         if Confirm("Are you sure you want to clear the current session ?", console=warning_console):
             CurrentUser.clear()
-
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/data_loaders.py` & `zerospeech-benchmarks-0.9.2/zerospeech/data_loaders.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,53 +2,54 @@
 from typing import Callable, Any, Union, Protocol, Tuple, List
 from zipfile import ZipFile
 
 import numpy
 import numpy as np
 import pandas as pd
 
-from .model import data_items
+from .generics import FileItem, FileTypes
 
-FileLoaderType = Callable[[data_items.FileItem], Any]
+FileLoaderType = Callable[[FileItem], Any]
 
 
 class FileError(Exception):
     """ Error while accessing file data """
 
 
-def load_dataframe(file_item: Union[data_items.FileItem, Path], **extras) -> pd.DataFrame:
+def load_dataframe(file_item: Union[FileItem, Path], **extras) -> pd.DataFrame:
     """ Open a column based file as dataframe """
     if isinstance(file_item, Path):
-        file_item = data_items.FileItem.from_file(file_item)
+        file_item = FileItem.from_file(file_item)
 
     if not file_item.file.is_file():
         raise FileNotFoundError(f'File :{file_item.file} does not exist')
 
-    if file_item.file_type not in data_items.FileTypes.dataframe_types():
+    if file_item.file_type not in FileTypes.dataframe_types():
         raise FileError(f"current type {file_item.file_type} cannot be converted to Dataframe")
 
     # open as dataframe
     return pd.read_csv(file_item.file, **extras)
 
 
-def load_numpy_array(file_item: Union[data_items.FileItem, Path]) -> numpy.ndarray:
+def load_numpy_array(file_item: Union[FileItem, Path]) -> numpy.ndarray:
     if isinstance(file_item, Path):
-        file_item = data_items.FileItem.from_file(file_item)
+        file_item = FileItem.from_file(file_item)
 
-    if file_item.file_type not in data_items.FileTypes.numpy_types():
+    if file_item.file_type not in FileTypes.numpy_types():
         raise FileError(f"current type {file_item.file_type} cannot be converted to a numpy array")
 
-    if file_item.file_type == data_items.FileTypes.txt:
+    if file_item.file_type == FileTypes.txt:
         return np.loadtxt(file_item.file)
-    elif file_item.file_type == data_items.FileTypes.npy:
+    elif file_item.file_type == FileTypes.npy:
         return np.load(str(file_item.file))
 
 
 class Zippable(Protocol):
     def __zippable__(self) -> List[Tuple[str, Path]]:
+        """ protocol definition """
         pass
 
 
 def zip_zippable(item: Zippable, archive_file: Path = Path("archive.zip")):
     """ Create a zip archive from an item that uses the Zippable protocol"""
     items_list = item.__zippable__()
     with ZipFile(archive_file, 'w') as zip_obj:
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/misc.py` & `zerospeech-benchmarks-0.9.2/zerospeech/misc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,123 @@
 import contextlib
-import enum
 import io
 import json
 import sys
+import sys
+import threading
+import _thread as thread
+from time import sleep
 from pathlib import Path
-from typing import Dict, List, Union
+from typing import Dict, List, Union, Optional, Protocol
 from zipfile import ZipFile
 
-import humanize
-# from datasize import DataSize todo: find out why this was deleted ? maybe on unpushed thing on laptop?
-from pydantic import ByteSize, BaseModel
 import requests
 from Crypto.Hash import MD5  # noqa: the package name is not the same
+# from datasize import DataSize todo: find out why this was deleted ? maybe on unpushed thing on laptop?
+from pydantic import ByteSize, BaseModel
 
 try:
     import yaml
 except ImportError:
     yaml = None
 try:
-    import tomli # noqa: is not a strict requirement
+    import tomli  # noqa: is not a strict requirement
 except ImportError:
     tomli = None
 
 from .out import with_progress, void_console, console
 from .settings import get_settings
 
 st = get_settings()
 
 
+def exit_after(s):
+    """ Decorator that kills function after s number of seconds
+    Usage:
+
+        @exit_after(10)
+        def f():
+            # complex computation
+
+
+        try:
+            f()
+        except KeyboardInterrupt:
+            print('Function f could not finish in 10 seconds and was interrupted')
+
+    """
+
+    def process_quit():
+        """ Raise a Keyboard interrupt"""
+        thread.interrupt_main()  # raises KeyboardInterrupt
+
+    def outer(fn):
+        def inner(*args, **kwargs):
+            """
+            Uses a timer from threading module to raise a KeyboardInterrupt after s seconds.
+            """
+            timer = threading.Timer(s, process_quit)
+            timer.start()
+            try:
+                result = fn(*args, **kwargs)
+            finally:
+                """ Cancel timer if function finished processing """
+                timer.cancel()
+            return result
+
+        return inner
+
+    return outer
+
+
+class ContextualItem(Protocol):
+    """ Item providing context to exceptions """
+
+    def print(self, allow_warnings: bool = False):
+        """ protocol function allowing to print context """
+        pass
+
+
+class ContextualException(Exception):
+    """ Custom exception providing a context """
+
+    def __init__(self, msg: str, ctx: Optional[ContextualItem] = None):
+        self._context: ContextualItem = ctx
+        super().__init__(msg)
+
+    def print_context(self, allow_warnings: bool = False):
+        """ Prints the current context """
+        if self._context:
+            self._context.print(allow_warnings)
+
+
+class ScoresNotFound(ContextualException):
+    pass
+
+
+class MetaYamlNotValid(ContextualException):
+    pass
+
+
+class InvalidSubmissionError(ContextualException):
+    pass
+
+
 class SizeUnit(BaseModel):
     __root__: ByteSize
 
     @property
     def human_readable(self):
         return self.__root__.human_readable(decimal=True)
 
     @property
     def as_bytes(self):
         return self.__root__
 
+
 # todo: see if i can remove this from the codebase ?
 # todo can we remove humanize from requirements ? or is it still used ?
 # class SizeUnit(enum.Enum):
 #     BYTES = 1
 #     KB = 2
 #     MB = 3
 #     GB = 4
@@ -113,50 +188,51 @@
     """ Create a zip archive from a folder """
     with ZipFile(archive_file, 'w') as zip_obj:
         for file in filter(lambda x: x.is_file(), location.rglob("*")):
             zip_obj.write(file, str(file.relative_to(location)))
 
 
 def download_extract_zip(
-        zip_url: str, target_location: Path,  size_in_bytes: int, *, filename: str = "",
+        zip_url: str, target_location: Path, size_in_bytes: int, *, filename: str = "",
         md5sum_hash: str = "", quiet: bool = False, show_progress: bool = True,
 ):
     tmp_dir = st.mkdtemp()
     response = requests.get(zip_url, stream=True)
+    tmp_filename = tmp_dir / "download.zip"
 
     if quiet:
         _console = void_console
         show_progress = False
     else:
         _console = console
 
     with with_progress(show=show_progress, file_transfer=True) as progress:
         total = int(size_in_bytes)
         task1 = progress.add_task(f"[red]Downloading {filename}...", total=total)
 
-        with (tmp_dir / f"download.zip").open("wb") as stream:
+        with tmp_filename.open("wb") as stream:
             for chunk in response.iter_content(chunk_size=1024):
                 stream.write(chunk)
                 progress.update(task1, advance=1024)
 
         progress.update(task1, completed=total, visible=False)
         _console.print("[green]Download completed Successfully!")
 
     if md5sum_hash != "":
         with _console.status("[red]Verifying md5sum from repository..."):
-            h = md5sum(tmp_dir / f"download.zip")
+            h = md5sum(tmp_filename)
 
         if h == md5sum_hash:
             _console.print("[green]MD5 sum verified!")
         else:
             _console.print("[green]MD5sum Failed, Check with repository administrator.\nExiting...")
             sys.exit(1)
 
     with _console.status("[red]Unzipping archive..."):
-        unzip(tmp_dir / f"download.zip", target_location)
+        unzip(tmp_filename, target_location)
 
 
 def symlink_dir_contents(source: Path, dest: Path):
     """ create symlinks of all content in a directory into another """
     dest.mkdir(exist_ok=True, parents=True)
     for item in source.iterdir():
         (dest / item.name).symlink_to(item, target_is_directory=item.is_dir())
@@ -172,8 +248,7 @@
 @contextlib.contextmanager
 def nostdout():
     """ Redirect stdout to /dev/null """
     save_stdout = sys.stdout
     sys.stdout = io.BytesIO()
     yield
     sys.stdout = save_stdout
-
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/model/checkpoints.py` & `zerospeech-benchmarks-0.9.2/zerospeech/generics/checkpoints.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/model/data_items.py` & `zerospeech-benchmarks-0.9.2/zerospeech/generics/data_items.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,23 +13,24 @@
     flac = "flac"
     item = "item"  # abx task file
     tsv = "tsv"
     json = "json"
     yaml = "yaml"
     phn = "phn"  # phone alignment file
     wrd = "wrd"  # words alignment file
+    vad = "vad.csv" # vad segmentation file in csv format
 
     @property
     def ext(self) -> str:
         return f".{self.value}"
 
     @classmethod
     def dataframe_types(cls):
         return {
-            cls.csv, cls.txt, cls.tsv, cls.item
+            cls.csv, cls.txt, cls.tsv, cls.item, cls.vad, cls.wrd, cls.phn
         }
 
     @classmethod
     def audio_types(cls):
         return {
             cls.wav, cls.flac
         }
@@ -52,15 +53,15 @@
     item_type: ItemType = ItemType.base_item
     file_type: FileTypes
     relative_path: bool
 
     @validator('file_type', pre=True)
     def fix_file_extension(cls, v):
         if isinstance(v, str):
-            return v.replace('.', '')
+            return v.lstrip('.')
         return v
 
     def relative_to(self, path: Path):
         """ Convert internal path to relative paths """
         self.relative_path = True
 
     def absolute_to(self, path: Path):
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/model/leaderboard.py` & `zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/_models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,69 @@
 from datetime import datetime
-from enum import Enum
 from typing import List, Optional, Dict, Union
 
-from pydantic import BaseModel, AnyHttpUrl, Field
+from pydantic import BaseModel, AnyHttpUrl, Field, validator
 
-
-class Benchmark(str, Enum):
-    ABX_15 = "ABX-15"
-    ABX_17 = "ABX-17"
-    ABX_LS = "ABX-LS"
-    TDE_15 = "TDE-15"
-    TDE_17 = "TDE-17"
-    TTS0_19 = "TTS0-19"
-    TTS0_LSLJ = "TTS0-LSLJ"
-    sLM_21 = "sLM-21"
-    prosAudit = "prosAudit"
+from ._types import LeaderboardBenchmarkName
 
 
 class ABXScoreTuple(BaseModel):
     within: Optional[float]
     across: Optional[float]
 
 
 class CatScores(BaseModel):
     precision: Optional[float]
     recall: Optional[float]
     fscore: Optional[float]
 
+    @validator('*', pre=True)
+    def fix_float(cls, v):
+        """ Sometimes NoneType is not marked as None but as a string"""
+        try:
+            return float(v)
+        except (ValueError, TypeError):
+            return None
+
 
 class NLPScores(BaseModel):
     ned: Optional[float]
     coverage: Optional[float]
     nwords: Optional[int]
     npairs: Optional[int]
 
+    @validator('ned', 'npairs', pre=True)
+    def fix_float(cls, v):
+        """ Sometimes NoneType is not marked as None but as a string"""
+        try:
+            return int(v)
+        except (ValueError, TypeError):
+            return None
+
+    @validator('nwords', 'coverage', pre=True)
+    def fix_int(cls, v):
+        """ Sometimes NoneType is not marked as None but as a string"""
+        try:
+            return float(v)
+        except (ValueError, TypeError):
+            return None
+
 
 class TDEScoreTuple(BaseModel):
     grouping: Optional[CatScores]
     token: Optional[CatScores]
     type: Optional[CatScores]
     boundary: Optional[CatScores]
     matching: Optional[CatScores]
     nlp: Optional[NLPScores]
 
 
 class EntryDetails(BaseModel):
     train_set: Optional[str]
-    benchmarks: List[Benchmark]
+    benchmarks: List[LeaderboardBenchmarkName]
     gpu_budget: Optional[str]
     parameters: Dict = Field(default_factory=dict)
 
 
 class PublicationEntry(BaseModel):
     author_short: Optional[str]
     authors: Optional[str]
@@ -84,14 +97,14 @@
     publication: PublicationEntry
     details: EntryDetails
     scores: LeaderboardScores
     extras: Optional[LeaderboardExtras]
 
 
 class Leaderboard(BaseModel):
-    _type: Benchmark
-    last_modified: datetime
+    _type: LeaderboardBenchmarkName
+    last_modified: datetime = Field(default_factory=lambda: datetime.now())
     data: List[LeaderboardEntry]
 
     def sort_by(self, key: str):
         """ Sort entries of leaderboard by a specific key"""
         self.data.sort(key=lambda x: getattr(x, key))
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/model/repository.py` & `zerospeech-benchmarks-0.9.2/zerospeech/generics/repository.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/model/samples.py` & `zerospeech-benchmarks-0.9.2/zerospeech/generics/samples.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/model/score_dir.py` & `zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/score_dir.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import abc
 from typing import Optional, Any
 
 from pydantic import BaseModel, DirectoryPath
 
-from .leaderboard import LeaderboardEntry, PublicationEntry
+from zerospeech.leaderboards import LeaderboardEntry, PublicationEntry
+from zerospeech.misc import load_obj
 from .meta_file import MetaFile
-from ..misc import load_obj
 
 
 class ScoreDir(BaseModel, abc.ABC):
     submission_dir: DirectoryPath
     location: DirectoryPath
     params: Optional[Any] = None
     meta_file: Optional[MetaFile] = None
+    leaderboard_file_name: str = "leaderboard.json"
 
     def load_meta(self):
         """ Load metadata from submission """
         obj = load_obj(self.submission_dir / MetaFile.file_stem)
         self.meta_file = MetaFile.parse_obj(obj)
 
     @abc.abstractmethod
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/networkio.py` & `zerospeech-benchmarks-0.9.2/zerospeech/networkio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import sys
 import warnings
 from datetime import datetime
 
 from .settings import get_settings
 from .out import console, error_console
-from .model import repository
+from .generics import repository
 
 import requests
 from pydantic import ValidationError
 
 st = get_settings()
 
 
@@ -17,15 +17,15 @@
     """ Updates the repositories index from remote """
     r = requests.get(st.repo_origin)
     data = r.json()
     try:
         _ = repository.RepositoryIndex(**data)
     except ValidationError:
         error_console.log(f"The given repository @ {st.repository_index} is not valid")
-        error_console.log(f"Please contact the administrator to resolve this issue...")
+        error_console.log("Please contact the administrator to resolve this issue...")
         sys.exit(1)
 
     with st.repository_index.open('w') as fp:
         json.dump(data, fp)
     console.log("RepositoryIndex has been updated successfully !!")
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/startup.py` & `zerospeech-benchmarks-0.9.2/zerospeech/startup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .cmd import (
-    CommandTree, CLI, LIST_OF_COMMANDS
+    CommandTree, CLI
 )
 from .networkio import update_repo_index, check_update_repo_index
 from .out import console
 from .settings import get_settings
 
 st = get_settings()
 
@@ -30,14 +30,14 @@
 
 
 def main():
     """ Main Function """
     cli = CLI(
         CommandTree("zrc"),
         description="A command line tool to help with the use of the Zerospeech Benchmarks.",
-        usage=f"zrc <command> [<args>]"
+        usage="zrc <command> [<args>]"
     )
     cli.run()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/validators/base_validators.py` & `zerospeech-benchmarks-0.9.2/zerospeech/validators/base_validators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import functools
 from pathlib import Path
 from typing import List, Callable, Any, Type
 
 import numpy as np
 import pandas as pd
 
-from ..model import data_items, m_benchmark
+from zerospeech.generics import FileListItem
+from zerospeech.submissions import ValidationResponse, ValidationOK, ValidationError
 
 # Type for base functions
-BASE_VALIDATOR_FN_TYPE = Callable[[Any], List[m_benchmark.ValidationResponse]]
-return_type = List[m_benchmark.ValidationResponse]
+BASE_VALIDATOR_FN_TYPE = Callable[[Any], List[ValidationResponse]]
+return_type = List[ValidationResponse]
 
 
 def list_checker(given: List[str], expected: List[str]) -> return_type:
     """ Check a list of strings to find if expected items are in it """
     given = set(given)
     expected = set(expected)
 
@@ -22,89 +22,89 @@
         has_more_files = given - expected
         res = []
 
         if len(has_more_files) > 0:
 
             for e_file in has_more_files:
                 res.append(
-                    m_benchmark.ValidationError(
+                    ValidationError(
                         "extra file found",
                         filename=e_file
                     )
                 )
         elif len(has_less_files) > 0:
             res = []
             for e_file in has_less_files:
-                res.append(m_benchmark.ValidationError(
+                res.append(ValidationError(
                     "expected file not found",
                     filename=e_file
                 ))
 
         return res
     else:
-        return [m_benchmark.ValidationOK('expected files found')]
+        return [ValidationOK('expected files found')]
 
 
 def file_list_checker(
-        item: data_items.FileListItem, expected: List[Path]
+        item: FileListItem, expected: List[Path]
 ) -> return_type:
     """ Check if a file list has expected files in it """
     file_names = [f.stem for f in item.files_list]
     expected_names = [f.stem for f in expected]
     return list_checker(given=file_names, expected=expected_names)
 
 
 def dataframe_column_check(df: pd.DataFrame, expected_columns: List[str]) -> return_type:
     """ Check that all columns are present in a dataframe """
     columns = list(df.columns)
     if columns != expected_columns:
-        return [m_benchmark.ValidationError(f'columns are not expected '
+        return [ValidationError(f'columns are not expected '
                                             f'expected: {expected_columns}, found: {columns}')]
 
-    return [m_benchmark.ValidationOK(f'Columns of dataframe are valid')]
+    return [ValidationOK('Columns of dataframe are valid')]
 
 
 def dataframe_index_check(df: pd.DataFrame, expected: List[str]) -> return_type:
     """ Check that specific values are contained in each row"""
     # check if all files from the dataset are represented in the filenames
     index = list(df.index)
     return list_checker(index, expected)
 
 
 def dataframe_type_check(df: pd.DataFrame, col_name: str, expected_type: Type[Any]) -> return_type:
     """ Verify column type matches expected type """
     try:
         df[col_name].astype(expected_type)
     except ValueError:
-        return [m_benchmark.ValidationError(f'Column {col_name} does not march expected type {expected_type}')]
+        return [ValidationError(f'Column {col_name} does not march expected type {expected_type}')]
     return []
 
 
 def numpy_dimensions_check(array: np.ndarray, ndim: int):
     """ Check ndarray matches specified dimensions"""
     if array.ndim != ndim:
-        return [m_benchmark.ValidationError(
+        return [ValidationError(
             f'Array should be of dimensions: {ndim}')]
     return []
 
 
 def numpy_dtype_check(array: np.ndarray, dtype: np.dtype):
     """ Check ndarray matches specified type """
     if array.dtype != dtype:
-        return [m_benchmark.ValidationError(
+        return [ValidationError(
             f'Array should be of type: {dtype}')]
     return []
 
 
 def numpy_col_comparison(dim: int):
     ncols = []
 
     def comparison(array: np.ndarray):
         ncols.append(array.shape[dim])
 
         if len(set(ncols)) != 1:
             return [
-                m_benchmark.ValidationError(f'Arrays do not match dimensions {dim}')
+                ValidationError(f'Arrays do not match dimensions {dim}')
             ]
         return []
 
     return comparison
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech/validators/validators.py` & `zerospeech-benchmarks-0.9.2/zerospeech/validators/validators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 import warnings
 from pathlib import Path
 from typing import List, Union, Callable, Any
 
+from zerospeech.data_loaders import load_dataframe, load_numpy_array, FileError
+from zerospeech.generics import FileItem, FileListItem, FileTypes
+from .base_validators import ValidationError, ValidationOK, ValidationResponse
 from .base_validators import BASE_VALIDATOR_FN_TYPE
-from ..data_loaders import load_dataframe, load_numpy_array, FileError
-from ..model import data_items, m_benchmark
 
-return_type = List[m_benchmark.ValidationResponse]
+return_type = List[ValidationResponse]
 COMPLEX_VALIDATION_FN = Callable[[Any, List[BASE_VALIDATOR_FN_TYPE]], return_type]
 
 
 def dataframe_check(
-        item: data_items.FileItem,
+        item: FileItem,
         additional_checks: List[BASE_VALIDATOR_FN_TYPE], **kwargs
 ) -> return_type:
     """ Check validity & apply additional checks to a Dataframe fileItem """
     results = []
 
-    if item.file_type not in data_items.FileTypes.dataframe_types():
-        return [m_benchmark.ValidationError(f'file type {item.file_type} cannot be converted into a dataframe',
+    if item.file_type not in FileTypes.dataframe_types():
+        return [ValidationError(f'file type {item.file_type} cannot be converted into a dataframe',
                                             data=item.file)]
 
     try:
         df = load_dataframe(item, **kwargs)
     except Exception as e:  # noqa: broad exception is on purpose
-        return [m_benchmark.ValidationError(f'{e}', data=item.file)]
+        return [ValidationError(f'{e}', data=item.file)]
 
-    results.append(m_benchmark.ValidationOK(f"File {item.file} is a valid dataframe !"))
+    results.append(ValidationOK(f"File {item.file} is a valid dataframe !"))
 
     for fn in additional_checks:
         results.extend(fn(df))
 
     return results
 
 
-def numpy_array_check(file_item: Union[data_items.FileItem, Path],
+def numpy_array_check(file_item: Union[FileItem, Path],
                       additional_checks: List[BASE_VALIDATOR_FN_TYPE]) -> return_type:
     """ Check validity & apply additional checks to a Numpy fileItem """
     warnings.filterwarnings("error")
     try:
         array = load_numpy_array(file_item)
     except (FileError, ValueError, UserWarning):
-        return [m_benchmark.ValidationError(f'File does not contain a numpy array', data=file_item)]
+        return [ValidationError('File does not contain a numpy array', data=file_item)]
 
-    results = [m_benchmark.ValidationOK(f'File contains a numpy array !', data=file_item)]
+    results = [ValidationOK('File contains a numpy array !', data=file_item)]
 
     for fn in additional_checks:
         results.extend(fn(array))
 
     return results
 
 
 def numpy_array_list_check(
-    item: data_items.FileListItem, f_list_checks: List[BASE_VALIDATOR_FN_TYPE],
+    item: FileListItem, f_list_checks: List[BASE_VALIDATOR_FN_TYPE],
     additional_checks: List[BASE_VALIDATOR_FN_TYPE]
 ) -> return_type:
     """ Check validity & apply additional checks to a list of Numpy fileItems """
     results = []
 
     for fn in f_list_checks:
         r = fn(item)
```

### Comparing `zerospeech-benchmarks-0.9.1/zerospeech_benchmarks.egg-info/PKG-INFO` & `zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerospeech-benchmarks
-Version: 0.9.1
+Version: 0.9.2
 Summary: Toolset for usage of the Zero Resource Challenge Benchmarks.
 Author-email: Nicolas Hamilakis <nicolas.hamilakis@ens.psl.eu>, CoML Team <dev@zerospeech.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -678,20 +678,26 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: documentation, https://zerospeech.com/toolbox/
 Project-URL: homepage, https://zerospeech.com/
 Project-URL: repository, https://github.com/zerospeech/benchmarks
 Keywords: speech,machine-learning,challenges,research-tool,benchmark-speech,zerospeech
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: vocolab
+Provides-Extra: tts019
 Provides-Extra: abx
 Provides-Extra: abx2
 Provides-Extra: tde
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE.txt
```


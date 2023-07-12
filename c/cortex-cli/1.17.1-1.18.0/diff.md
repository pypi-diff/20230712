# Comparing `tmp/cortex_cli-1.17.1.tar.gz` & `tmp/cortex_cli-1.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_cli-1.17.1.tar", last modified: Mon Jul 10 13:28:47 2023, max compression
+gzip compressed data, was "cortex_cli-1.18.0.tar", last modified: Wed Jul 12 14:01:45 2023, max compression
```

## Comparing `cortex_cli-1.17.1.tar` & `cortex_cli-1.18.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5733 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/README.md
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       22 2023-07-10 13:28:21.000000 cortex_cli-1.17.1/cortex_cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/cli/api/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/cli/api/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3992 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/cli/api/github_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/cli/api/http_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/cli/cli_api_base.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/cli/cli_api_base_config.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4179 2023-07-03 13:20:35.000000 cortex_cli-1.17.1/cortex_cli/cli/cli_multipart_upload.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/cli/clients.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2027 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/cli/configure.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      973 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/cli/cortex_cli.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/cli/generic_get.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/cli/inferences.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    24883 2023-07-03 17:51:56.000000 cortex_cli-1.17.1/cortex_cli/cli/models.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3259 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/cli/pipelines.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/core/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/core/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     6919 2023-07-03 18:05:46.000000 cortex_cli-1.17.1/cortex_cli/core/cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/core/drift_checks.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/core/ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/core/mlflow/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/core/mlflow/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    14671 2023-07-03 20:20:44.000000 cortex_cli-1.17.1/cortex_cli/core/mlflow/mlflow_cortex.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/core/models/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/core/models/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     8121 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/core/models/cortex_model.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2828 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/core/secrets_manager.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/model_templates/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      322 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1654 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      455 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli/tests/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/tests/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/tests/test_cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/cortex_cli/tests/test_ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/cortex_cli.egg-info/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-07-10 13:28:47.000000 cortex_cli-1.17.1/cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3162 2023-07-10 13:28:47.000000 cortex_cli-1.17.1/cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-07-10 13:28:47.000000 cortex_cli-1.17.1/cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-07-10 13:28:47.000000 cortex_cli-1.17.1/cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      146 2023-07-10 13:28:47.000000 cortex_cli-1.17.1/cortex_cli.egg-info/requires.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-07-10 13:28:47.000000 cortex_cli-1.17.1/cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       91 2023-06-28 17:58:15.000000 cortex_cli-1.17.1/pyproject.toml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-07-10 13:28:47.958727 cortex_cli-1.17.1/setup.cfg
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1104 2023-07-03 18:07:49.000000 cortex_cli-1.17.1/setup.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5733 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/README.md
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.529944 cortex_cli-1.18.0/cortex_cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       22 2023-07-12 13:56:07.000000 cortex_cli-1.18.0/cortex_cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.529944 cortex_cli-1.18.0/cortex_cli/cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/cli/api/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/cli/api/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3992 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/cli/api/github_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/cli/api/http_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/cli/cli_api_base.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/cli/cli_api_base_config.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4179 2023-07-03 13:20:35.000000 cortex_cli-1.18.0/cortex_cli/cli/cli_multipart_upload.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/cli/clients.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2051 2023-07-12 04:09:22.000000 cortex_cli-1.18.0/cortex_cli/cli/configure.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      973 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/cli/cortex_cli.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/cli/generic_get.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/cli/inferences.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    25020 2023-07-11 01:18:12.000000 cortex_cli-1.18.0/cortex_cli/cli/models.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3259 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/cli/pipelines.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/core/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/core/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     6935 2023-07-12 04:07:38.000000 cortex_cli-1.18.0/cortex_cli/core/cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/core/drift_checks.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/core/ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/core/mlflow/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/core/mlflow/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    14671 2023-07-11 01:13:56.000000 cortex_cli-1.18.0/cortex_cli/core/mlflow/mlflow_cortex.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/core/models/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/core/models/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     8121 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/core/models/cortex_model.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2828 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/core/secrets_manager.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/model_templates/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      365 2023-07-12 13:54:23.000000 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.529944 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1654 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      498 2023-07-12 13:54:41.000000 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.529944 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/cortex_cli/tests/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/tests/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/tests/test_cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/cortex_cli/tests/test_ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-12 14:01:45.529944 cortex_cli-1.18.0/cortex_cli.egg-info/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-07-12 14:01:45.000000 cortex_cli-1.18.0/cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3162 2023-07-12 14:01:45.000000 cortex_cli-1.18.0/cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-07-12 14:01:45.000000 cortex_cli-1.18.0/cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-07-12 14:01:45.000000 cortex_cli-1.18.0/cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      146 2023-07-12 14:01:45.000000 cortex_cli-1.18.0/cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-07-12 14:01:45.000000 cortex_cli-1.18.0/cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       91 2023-06-28 17:58:15.000000 cortex_cli-1.18.0/pyproject.toml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-07-12 14:01:45.539944 cortex_cli-1.18.0/setup.cfg
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1104 2023-07-11 01:13:56.000000 cortex_cli-1.18.0/setup.py
```

### Comparing `cortex_cli-1.17.1/README.md` & `cortex_cli-1.18.0/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/cli/api/github_api.py` & `cortex_cli-1.18.0/cortex_cli/cli/api/github_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/cli/api/http_api.py` & `cortex_cli-1.18.0/cortex_cli/cli/api/http_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/cli/cli_api_base.py` & `cortex_cli-1.18.0/cortex_cli/cli/cli_api_base.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/cli/cli_api_base_config.py` & `cortex_cli-1.18.0/cortex_cli/cli/cli_api_base_config.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/cli/cli_multipart_upload.py` & `cortex_cli-1.18.0/cortex_cli/cli/cli_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/cli/configure.py` & `cortex_cli-1.18.0/cortex_cli/cli/configure.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,21 +44,21 @@
         except FileNotFoundError:
             # Ok for now, file will be created later
             pass
 
 
         # Prompt whenever switches are not used
         if not self._profile:
-            self._profile = plumbum.cli.terminal.prompt('Profile:', type=str, default='default')
+            self._profile = plumbum.cli.terminal.prompt('Profile:', type=str, default='default').strip()
 
         if not self._api_url:
-            self._api_url = plumbum.cli.terminal.prompt('API Url:', type=str, default='https://api.nearlyhuman.ai')
+            self._api_url = plumbum.cli.terminal.prompt('API Url:', type=str, default='https://api.nearlyhuman.ai').strip()
 
         if not self._api_key:          
-            self._api_key = plumbum.cli.terminal.prompt('API Key:', type=str, default='')
+            self._api_key = plumbum.cli.terminal.prompt('API Key:', type=str, default='').strip()
 
 
         config[self._profile] = {
             'api_url': self._api_url,
             'api_key': self._api_key
         }
```

### Comparing `cortex_cli-1.17.1/cortex_cli/cli/cortex_cli.py` & `cortex_cli-1.18.0/cortex_cli/cli/cortex_cli.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/cli/generic_get.py` & `cortex_cli-1.18.0/cortex_cli/cli/generic_get.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/cli/inferences.py` & `cortex_cli-1.18.0/cortex_cli/cli/inferences.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/cli/models.py` & `cortex_cli-1.18.0/cortex_cli/cli/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -677,24 +677,27 @@
         self._info('Saving pipeline artifacts...')
         signature = infer_signature(self.model.input_example, self.model.output_example)
 
         # Save model
         modules = list(self._modules.keys())
         modules.append(self._model_module)
         if self.model.model_type == 'cortex':
+            # Handle no deployment steps
+            deployment_steps = self._config['deployment_steps'] if self._config['deployment_steps'] else []
+
             mlflow_cortex.save_model(
                 python_model=self.model, 
                 path=self._artifacts_dir,                   # Where artifacts are stored locally
                 code_path=list(modules),                    # Local code paths not on
                 conda_env='conda.yml',
                 artifacts={},
                 custom_objects=self.model.custom_objects,
                 signature=signature,
                 pipeline_steps=self._config['pipeline_steps'],
-                deployment_steps=self._config['deployment_steps']
+                deployment_steps=deployment_steps
             )
         else:
             self._error_message = f"An error occurred while detecting the Cortex model type. \
             Found '{self.model.model_type}', but only ['cortex'] are acceptable values"
             raise Exception
 
         return f'Saved the pipeline artifacts to disk: ({self._artifacts_dir})'
```

### Comparing `cortex_cli-1.17.1/cortex_cli/cli/pipelines.py` & `cortex_cli-1.18.0/cortex_cli/cli/pipelines.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/core/cortex_data.py` & `cortex_cli-1.18.0/cortex_cli/core/cortex_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                         text = ''
                         for paragraph in doc.content:
                             text += paragraph.plain_text()
                         
                         self._loaded_data = text
                         
                     if self.type=='txt':
-                        self._loaded_data = file.read()
+                        self._loaded_data = file.read().decode('utf-8')
 
                     if self.type=='yml':
                         self._loaded_data = yaml.load(file)
                     
             return self._loaded_data
         except IOError:
             # Throw an exception if there is an unsupported file type
```

### Comparing `cortex_cli-1.17.1/cortex_cli/core/drift_checks.py` & `cortex_cli-1.18.0/cortex_cli/core/drift_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/core/ethics_checks.py` & `cortex_cli-1.18.0/cortex_cli/core/ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/core/mlflow/mlflow_cortex.py` & `cortex_cli-1.18.0/cortex_cli/core/mlflow/mlflow_cortex.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/core/models/cortex_model.py` & `cortex_cli-1.18.0/cortex_cli/core/models/cortex_model.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/core/secrets_manager.py` & `cortex_cli-1.18.0/cortex_cli/core/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/.gitignore` & `cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/README.md` & `cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.18.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/.gitignore` & `cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/README.md` & `cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.18.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/tests/test_cortex_data.py` & `cortex_cli-1.18.0/cortex_cli/tests/test_cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli/tests/test_ethics_checks.py` & `cortex_cli-1.18.0/cortex_cli/tests/test_ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/cortex_cli.egg-info/SOURCES.txt` & `cortex_cli-1.18.0/cortex_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1/setup.py` & `cortex_cli-1.18.0/setup.py`

 * *Files identical despite different names*


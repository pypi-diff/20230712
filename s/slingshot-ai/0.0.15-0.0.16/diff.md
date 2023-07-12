# Comparing `tmp/slingshot_ai-0.0.15.tar.gz` & `tmp/slingshot_ai-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slingshot_ai-0.0.15.tar", max compression
+gzip compressed data, was "slingshot_ai-0.0.16.tar", max compression
```

## Comparing `slingshot_ai-0.0.15.tar` & `slingshot_ai-0.0.16.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0      827 2023-07-10 21:48:51.271390 slingshot_ai-0.0.15/pyproject.toml
--rw-r--r--   0        0        0      156 2023-06-20 09:58:42.891207 slingshot_ai-0.0.15/src/slingshot/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.738131 slingshot_ai-0.0.15/src/slingshot/cli/__init__.py
--rw-r--r--   0        0        0    17919 2023-07-10 15:40:42.647885 slingshot_ai-0.0.15/src/slingshot/cli/add.py
--rw-r--r--   0        0        0     2091 2023-06-27 10:21:25.506818 slingshot_ai-0.0.15/src/slingshot/cli/apply.py
--rw-r--r--   0        0        0     6421 2023-07-05 17:23:48.992824 slingshot_ai-0.0.15/src/slingshot/cli/apps.py
--rw-r--r--   0        0        0     5916 2023-06-23 10:00:55.765161 slingshot_ai-0.0.15/src/slingshot/cli/artifact.py
--rw-r--r--   0        0        0     5263 2023-06-27 10:21:25.507053 slingshot_ai-0.0.15/src/slingshot/cli/auth.py
--rw-r--r--   0        0        0      970 2023-06-08 16:54:38.738871 slingshot_ai-0.0.15/src/slingshot/cli/code.py
--rw-r--r--   0        0        0        0 2023-06-13 14:12:37.848609 slingshot_ai-0.0.15/src/slingshot/cli/config/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.738965 slingshot_ai-0.0.15/src/slingshot/cli/config/py.typed
--rw-r--r--   0        0        0      850 2023-06-20 09:58:42.891910 slingshot_ai-0.0.15/src/slingshot/cli/config/sentry_setup.py
--rw-r--r--   0        0        0    13774 2023-06-27 10:21:25.507213 slingshot_ai-0.0.15/src/slingshot/cli/config/slingshot_cli.py
--rw-r--r--   0        0        0     1234 2023-06-08 16:54:38.739227 slingshot_ai-0.0.15/src/slingshot/cli/dev.py
--rw-r--r--   0        0        0     1123 2023-06-27 10:21:25.507291 slingshot_ai-0.0.15/src/slingshot/cli/environment.py
--rw-r--r--   0        0        0     5323 2023-07-05 17:23:48.992981 slingshot_ai-0.0.15/src/slingshot/cli/inference.py
--rw-r--r--   0        0        0     3059 2023-06-08 16:54:38.739428 slingshot_ai-0.0.15/src/slingshot/cli/logs.py
--rw-r--r--   0        0        0     1951 2023-06-30 17:31:08.610192 slingshot_ai-0.0.15/src/slingshot/cli/machine.py
--rw-r--r--   0        0        0     2759 2023-07-05 17:23:48.993098 slingshot_ai-0.0.15/src/slingshot/cli/main.py
--rw-r--r--   0        0        0     2433 2023-07-03 15:58:05.510535 slingshot_ai-0.0.15/src/slingshot/cli/project.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.739665 slingshot_ai-0.0.15/src/slingshot/cli/py.typed
--rw-r--r--   0        0        0     8920 2023-07-07 09:11:42.963260 slingshot_ai-0.0.15/src/slingshot/cli/run.py
--rw-r--r--   0        0        0     3648 2023-06-08 16:54:38.739947 slingshot_ai-0.0.15/src/slingshot/cli/secret.py
--rw-r--r--   0        0        0     3845 2023-07-05 17:23:48.993362 slingshot_ai-0.0.15/src/slingshot/cli/session.py
--rw-r--r--   0        0        0       67 2023-06-08 16:54:38.740233 slingshot_ai-0.0.15/src/slingshot/cli/shared/__init__.py
--rw-r--r--   0        0        0     6260 2023-06-23 10:00:55.765417 slingshot_ai-0.0.15/src/slingshot/cli/shared/code_sync.py
--rw-r--r--   0        0        0     7029 2023-06-20 09:58:42.892817 slingshot_ai-0.0.15/src/slingshot/cli/shared/prompt.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.740473 slingshot_ai-0.0.15/src/slingshot/cli/shared/py.typed
--rw-r--r--   0        0        0      191 2023-06-08 16:54:38.740573 slingshot_ai-0.0.15/src/slingshot/cli/shared/settings.py
--rw-r--r--   0        0        0     5985 2023-07-07 09:11:42.964178 slingshot_ai-0.0.15/src/slingshot/cli/shared/utils.py
--rw-r--r--   0        0        0     1388 2023-06-08 16:54:38.740763 slingshot_ai-0.0.15/src/slingshot/cli/volume.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.740862 slingshot_ai-0.0.15/src/slingshot/code/__init__.py
--rw-r--r--   0        0        0        1 2023-06-08 16:54:38.741013 slingshot_ai-0.0.15/src/slingshot/code/annotation.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741087 slingshot_ai-0.0.15/src/slingshot/code/py.typed
--rw-r--r--   0        0        0       56 2023-06-20 09:58:42.893069 slingshot_ai-0.0.15/src/slingshot/inference_model/__init__.py
--rw-r--r--   0        0        0     3941 2023-06-20 09:58:42.893206 slingshot_ai-0.0.15/src/slingshot/inference_model/inference_model.py
--rw-r--r--   0        0        0      205 2023-06-08 16:54:38.741497 slingshot_ai-0.0.15/src/slingshot/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741599 slingshot_ai-0.0.15/src/slingshot/schemas/generated/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741656 slingshot_ai-0.0.15/src/slingshot/schemas/generated/py.typed
--rw-r--r--   0        0        0    26670 2023-07-10 20:40:20.793233 slingshot_ai-0.0.15/src/slingshot/schemas/generated/schemas.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741863 slingshot_ai-0.0.15/src/slingshot/schemas/py.typed
--rw-r--r--   0        0        0    10181 2023-06-27 10:21:25.507893 slingshot_ai-0.0.15/src/slingshot/schemas/schema_extensions.py
--rw-r--r--   0        0        0    15236 2023-07-10 20:40:20.793400 slingshot_ai-0.0.15/src/slingshot/schemas/slingshot-schema.config.json
--rw-r--r--   0        0        0    19518 2023-07-10 20:40:20.793564 slingshot_ai-0.0.15/src/slingshot/schemas/slingshot_schema.py
--rw-r--r--   0        0        0      125 2023-07-07 09:11:36.011571 slingshot_ai-0.0.15/src/slingshot/sdk/__init__.py
--rw-r--r--   0        0        0    45606 2023-07-10 20:40:20.793788 slingshot_ai-0.0.15/src/slingshot/sdk/apply.py
--rw-r--r--   0        0        0     2217 2023-06-08 16:54:38.742780 slingshot_ai-0.0.15/src/slingshot/sdk/auth.py
--rw-r--r--   0        0        0     2073 2023-06-27 10:21:25.508229 slingshot_ai-0.0.15/src/slingshot/sdk/config.py
--rw-r--r--   0        0        0     1856 2023-06-20 09:58:42.894424 slingshot_ai-0.0.15/src/slingshot/sdk/config_utils.py
--rw-r--r--   0        0        0     2372 2023-07-07 09:11:36.011656 slingshot_ai-0.0.15/src/slingshot/sdk/data_collector.py
--rw-r--r--   0        0        0     5334 2023-06-08 16:54:38.743055 slingshot_ai-0.0.15/src/slingshot/sdk/errors.py
--rw-r--r--   0        0        0      126 2023-06-08 16:54:38.743167 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/__init__.py
--rw-r--r--   0        0        0     3293 2023-06-08 16:54:38.743260 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/base_graphql.py
--rw-r--r--   0        0        0    18027 2023-06-27 10:21:25.508389 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/fragments.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.743421 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/py.typed
--rw-r--r--   0        0        0      138 2023-06-08 16:54:38.743578 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/__init__.py
--rw-r--r--   0        0        0     5265 2023-06-08 16:54:38.743672 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/apps.py
--rw-r--r--   0        0        0      986 2023-06-08 16:54:38.743759 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/deployment.py
--rw-r--r--   0        0        0     3671 2023-06-08 16:54:38.743873 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/environment.py
--rw-r--r--   0        0        0     5247 2023-06-27 10:21:25.508545 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/project.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.744004 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/py.typed
--rw-r--r--   0        0        0     2416 2023-07-07 09:11:42.964546 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/run.py
--rw-r--r--   0        0        0     3578 2023-06-08 16:54:38.744228 slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/storage.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.744264 slingshot_ai-0.0.15/src/slingshot/sdk/py.typed
--rw-r--r--   0        0        0    48216 2023-07-10 20:40:20.794010 slingshot_ai-0.0.15/src/slingshot/sdk/slingshot_api.py
--rw-r--r--   0        0        0    52406 2023-07-10 20:40:20.794271 slingshot_ai-0.0.15/src/slingshot/sdk/slingshot_sdk.py
--rw-r--r--   0        0        0     5420 2023-06-08 16:54:38.744840 slingshot_ai-0.0.15/src/slingshot/sdk/sync.py
--rw-r--r--   0        0        0     2862 2023-06-08 16:54:38.744928 slingshot_ai-0.0.15/src/slingshot/sdk/upload_download_utils.py
--rw-r--r--   0        0        0     2876 2023-06-20 09:58:42.895639 slingshot_ai-0.0.15/src/slingshot/sdk/utils.py
--rw-r--r--   0        0        0     4361 2023-07-05 17:23:48.994648 slingshot_ai-0.0.15/src/slingshot/sdk/web_path_util.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.745196 slingshot_ai-0.0.15/src/slingshot/shared/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.745256 slingshot_ai-0.0.15/src/slingshot/shared/py.typed
--rw-r--r--   0        0        0     6308 2023-06-29 15:16:46.917807 slingshot_ai-0.0.15/src/slingshot/shared/utils.py
--rw-r--r--   0        0        0       23 2023-07-10 21:49:00.875930 slingshot_ai-0.0.15/src/slingshot/slingshot_version.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.745526 slingshot_ai-0.0.15/src/slingshot/templates/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-29 15:13:56.504338 slingshot_ai-0.0.15/src/slingshot/templates/inference_template.py
--rw-r--r--   0        0        0     1090 2023-06-08 16:54:38.745977 slingshot_ai-0.0.15/src/slingshot/templates/label_studio_data_export_template.py
--rw-r--r--   0        0        0        0 2023-06-08 16:54:38.746012 slingshot_ai-0.0.15/src/slingshot/templates/py.typed
--rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 slingshot_ai-0.0.15/PKG-INFO
+-rw-r--r--   0        0        0      831 2023-07-12 16:16:00.198753 slingshot_ai-0.0.16/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-06-14 01:36:51.753575 slingshot_ai-0.0.16/src/slingshot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.733834 slingshot_ai-0.0.16/src/slingshot/cli/__init__.py
+-rw-r--r--   0        0        0    17378 2023-07-12 16:07:14.032130 slingshot_ai-0.0.16/src/slingshot/cli/add.py
+-rw-r--r--   0        0        0     2125 2023-07-12 13:35:06.558558 slingshot_ai-0.0.16/src/slingshot/cli/apply.py
+-rw-r--r--   0        0        0     6431 2023-07-12 16:07:14.032400 slingshot_ai-0.0.16/src/slingshot/cli/apps.py
+-rw-r--r--   0        0        0     5916 2023-06-20 21:48:49.557285 slingshot_ai-0.0.16/src/slingshot/cli/artifact.py
+-rw-r--r--   0        0        0     5263 2023-06-27 15:26:50.737721 slingshot_ai-0.0.16/src/slingshot/cli/auth.py
+-rw-r--r--   0        0        0      970 2023-06-08 13:51:24.734880 slingshot_ai-0.0.16/src/slingshot/cli/code.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:23:44.406584 slingshot_ai-0.0.16/src/slingshot/cli/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.734966 slingshot_ai-0.0.16/src/slingshot/cli/config/py.typed
+-rw-r--r--   0        0        0      850 2023-06-14 16:35:36.287763 slingshot_ai-0.0.16/src/slingshot/cli/config/sentry_setup.py
+-rw-r--r--   0        0        0    13774 2023-06-27 15:26:50.739279 slingshot_ai-0.0.16/src/slingshot/cli/config/slingshot_cli.py
+-rw-r--r--   0        0        0     1234 2023-06-08 13:51:24.735333 slingshot_ai-0.0.16/src/slingshot/cli/dev.py
+-rw-r--r--   0        0        0     1123 2023-07-03 01:17:17.281267 slingshot_ai-0.0.16/src/slingshot/cli/environment.py
+-rw-r--r--   0        0        0     5323 2023-07-05 13:59:49.265273 slingshot_ai-0.0.16/src/slingshot/cli/inference.py
+-rw-r--r--   0        0        0     3059 2023-06-08 13:51:24.735634 slingshot_ai-0.0.16/src/slingshot/cli/logs.py
+-rw-r--r--   0        0        0     1951 2023-07-03 17:32:15.325020 slingshot_ai-0.0.16/src/slingshot/cli/machine.py
+-rw-r--r--   0        0        0     2759 2023-07-04 04:36:55.756325 slingshot_ai-0.0.16/src/slingshot/cli/main.py
+-rw-r--r--   0        0        0     3011 2023-07-12 16:07:14.032658 slingshot_ai-0.0.16/src/slingshot/cli/project.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.735998 slingshot_ai-0.0.16/src/slingshot/cli/py.typed
+-rw-r--r--   0        0        0     8920 2023-07-07 20:43:45.117337 slingshot_ai-0.0.16/src/slingshot/cli/run.py
+-rw-r--r--   0        0        0     3648 2023-06-08 14:01:51.180092 slingshot_ai-0.0.16/src/slingshot/cli/secret.py
+-rw-r--r--   0        0        0     3845 2023-07-04 04:36:55.756967 slingshot_ai-0.0.16/src/slingshot/cli/session.py
+-rw-r--r--   0        0        0       67 2023-06-08 13:51:24.737453 slingshot_ai-0.0.16/src/slingshot/cli/shared/__init__.py
+-rw-r--r--   0        0        0     6260 2023-06-20 21:48:49.557743 slingshot_ai-0.0.16/src/slingshot/cli/shared/code_sync.py
+-rw-r--r--   0        0        0     7036 2023-07-12 16:07:14.033096 slingshot_ai-0.0.16/src/slingshot/cli/shared/prompt.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738086 slingshot_ai-0.0.16/src/slingshot/cli/shared/py.typed
+-rw-r--r--   0        0        0      191 2023-06-08 13:51:24.738326 slingshot_ai-0.0.16/src/slingshot/cli/shared/settings.py
+-rw-r--r--   0        0        0     6504 2023-07-12 16:07:14.033408 slingshot_ai-0.0.16/src/slingshot/cli/shared/utils.py
+-rw-r--r--   0        0        0     1388 2023-06-08 13:51:24.738677 slingshot_ai-0.0.16/src/slingshot/cli/volume.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738829 slingshot_ai-0.0.16/src/slingshot/code/__init__.py
+-rw-r--r--   0        0        0        1 2023-06-08 13:51:24.739138 slingshot_ai-0.0.16/src/slingshot/code/annotation.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.739256 slingshot_ai-0.0.16/src/slingshot/code/py.typed
+-rw-r--r--   0        0        0       56 2023-06-14 01:36:51.755302 slingshot_ai-0.0.16/src/slingshot/inference_model/__init__.py
+-rw-r--r--   0        0        0     3941 2023-06-14 14:56:40.736423 slingshot_ai-0.0.16/src/slingshot/inference_model/inference_model.py
+-rw-r--r--   0        0        0      205 2023-06-08 13:51:24.739905 slingshot_ai-0.0.16/src/slingshot/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740119 slingshot_ai-0.0.16/src/slingshot/schemas/generated/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740282 slingshot_ai-0.0.16/src/slingshot/schemas/generated/py.typed
+-rw-r--r--   0        0        0    26727 2023-07-12 16:07:23.000000 slingshot_ai-0.0.16/src/slingshot/schemas/generated/schemas.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740843 slingshot_ai-0.0.16/src/slingshot/schemas/py.typed
+-rw-r--r--   0        0        0    10181 2023-06-27 15:26:50.747432 slingshot_ai-0.0.16/src/slingshot/schemas/schema_extensions.py
+-rw-r--r--   0        0        0    15216 2023-07-12 16:07:14.034110 slingshot_ai-0.0.16/src/slingshot/schemas/slingshot-schema.config.json
+-rw-r--r--   0        0        0    19713 2023-07-12 16:07:14.034438 slingshot_ai-0.0.16/src/slingshot/schemas/slingshot_schema.py
+-rw-r--r--   0        0        0      125 2023-07-06 14:31:59.119085 slingshot_ai-0.0.16/src/slingshot/sdk/__init__.py
+-rw-r--r--   0        0        0    45791 2023-07-12 16:07:14.034882 slingshot_ai-0.0.16/src/slingshot/sdk/apply.py
+-rw-r--r--   0        0        0     2217 2023-06-08 13:51:24.742861 slingshot_ai-0.0.16/src/slingshot/sdk/auth.py
+-rw-r--r--   0        0        0     2073 2023-06-27 15:26:50.749266 slingshot_ai-0.0.16/src/slingshot/sdk/config.py
+-rw-r--r--   0        0        0     1856 2023-06-14 17:13:24.234357 slingshot_ai-0.0.16/src/slingshot/sdk/config_utils.py
+-rw-r--r--   0        0        0     2372 2023-07-06 15:25:20.145323 slingshot_ai-0.0.16/src/slingshot/sdk/data_collector.py
+-rw-r--r--   0        0        0     5334 2023-06-08 13:51:24.743481 slingshot_ai-0.0.16/src/slingshot/sdk/errors.py
+-rw-r--r--   0        0        0      126 2023-06-08 13:51:24.743741 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/__init__.py
+-rw-r--r--   0        0        0     3293 2023-06-08 13:51:24.743943 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/base_graphql.py
+-rw-r--r--   0        0        0    18365 2023-07-12 16:07:14.035297 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/fragments.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.744284 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/py.typed
+-rw-r--r--   0        0        0      138 2023-06-08 13:51:24.744487 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/__init__.py
+-rw-r--r--   0        0        0     5265 2023-07-06 15:15:48.339951 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/apps.py
+-rw-r--r--   0        0        0      986 2023-06-08 13:51:24.744887 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/deployment.py
+-rw-r--r--   0        0        0     3671 2023-06-08 13:51:24.745123 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/environment.py
+-rw-r--r--   0        0        0     5247 2023-06-27 15:26:50.751307 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/project.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745499 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/py.typed
+-rw-r--r--   0        0        0     2416 2023-07-07 20:43:45.118845 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/run.py
+-rw-r--r--   0        0        0     3578 2023-06-08 13:51:24.745899 slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/storage.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745963 slingshot_ai-0.0.16/src/slingshot/sdk/py.typed
+-rw-r--r--   0        0        0    48311 2023-07-12 16:07:14.035714 slingshot_ai-0.0.16/src/slingshot/sdk/slingshot_api.py
+-rw-r--r--   0        0        0    51951 2023-07-12 16:07:14.036162 slingshot_ai-0.0.16/src/slingshot/sdk/slingshot_sdk.py
+-rw-r--r--   0        0        0     5420 2023-06-08 13:51:24.747044 slingshot_ai-0.0.16/src/slingshot/sdk/sync.py
+-rw-r--r--   0        0        0     2862 2023-06-08 13:51:24.747244 slingshot_ai-0.0.16/src/slingshot/sdk/upload_download_utils.py
+-rw-r--r--   0        0        0     2876 2023-06-14 14:56:40.739250 slingshot_ai-0.0.16/src/slingshot/sdk/utils.py
+-rw-r--r--   0        0        0     4361 2023-07-05 13:59:49.269504 slingshot_ai-0.0.16/src/slingshot/sdk/web_path_util.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747738 slingshot_ai-0.0.16/src/slingshot/shared/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747833 slingshot_ai-0.0.16/src/slingshot/shared/py.typed
+-rw-r--r--   0        0        0     6753 2023-07-12 16:07:14.036481 slingshot_ai-0.0.16/src/slingshot/shared/utils.py
+-rw-r--r--   0        0        0       23 2023-07-12 17:47:47.333786 slingshot_ai-0.0.16/src/slingshot/slingshot_version.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748427 slingshot_ai-0.0.16/src/slingshot/templates/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-28 22:37:34.391674 slingshot_ai-0.0.16/src/slingshot/templates/inference_template.py
+-rw-r--r--   0        0        0     1090 2023-06-08 13:51:24.748859 slingshot_ai-0.0.16/src/slingshot/templates/label_studio_data_export_template.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748968 slingshot_ai-0.0.16/src/slingshot/templates/py.typed
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 slingshot_ai-0.0.16/PKG-INFO
```

### Comparing `slingshot_ai-0.0.15/pyproject.toml` & `slingshot_ai-0.0.16/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [project]
 name = "slingshot-ai"
-version = "0.0.15"
+version = "0.0.16"
 
 [tool.poetry]
 name = "slingshot-ai"
-version = "0.0.15"
+version = "0.0.16"
 description = ""
 authors = ["Slingshot AI <service-account@slingshot.xyz>"]
 packages = [ { include = "slingshot", from = "src" } ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "~=3.8.1"
 urllib3 = "~=1.26.11"
-pydantic = "==1.9"
+pydantic = "<=1.10.11"
 typer = {extras = ["all"], version = "~0.7.0"}
 requests = "~=2.28.1"
 sh = "~=1.14.3"
 pyyaml = "~=6.0"
 "ruamel.yaml" = "~=0.17.0"
 simple-term-menu = "~=1.6.0"
 deepdiff = "~=6.3.0"
 fastapi = "~=0.88.0"
 uvicorn = {extras = ["standard"], version = "~=0.18.0"}
 tqdm = "~=4.63.0"
-sentry-sdk = "~=1.13.0"
+sentry-sdk = "~=1.16.0"
 backoff = "~=2.0.0"
 openai = "~=0.27.8"
 
 [tool.poetry.scripts]
 slingshot = "slingshot.cli.main:app"
 
 [build-system]
```

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/add.py` & `slingshot_ai-0.0.16/src/slingshot/cli/add.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 from __future__ import annotations
 
-import json
 import re
 import shutil
 import uuid
 from pathlib import Path
-from typing import Any, Callable, Literal, Optional, Type, cast
+from typing import Callable, Literal, Optional, Type, cast
 
 import typer
-from pydantic import BaseModel, ValidationError
-from ruamel import yaml as r_yaml
+from pydantic import ValidationError
 
 from slingshot.cli.config.slingshot_cli import SlingshotCLIApp
-from slingshot.cli.shared import prompt_confirm, prompt_for_single_choice
+from slingshot.cli.shared import create_empty_project_manifest, prompt_confirm, prompt_for_single_choice
 from slingshot.schemas import SlingshotAbstractAppSpec
 from slingshot.schemas import slingshot_schema as slingshot_yaml_schemas
 from slingshot.sdk import SlingshotSDK
 from slingshot.sdk.config import client_settings
 from slingshot.sdk.utils import console, edit_slingshot_yaml
 
 from .. import schemas
 from ..sdk.errors import SlingshotException
-from ..shared.utils import load_slingshot_project_config
+from ..shared.utils import load_slingshot_project_config, pydantic_to_dict
 from .project import list_and_set_project_id
 
 app = SlingshotCLIApp()
-yaml = r_yaml.YAML()
 
 OPTIONS = ["run", "deployment", "app", "environment", "label-studio", "session"]
 OPTION_TO_SPEC_CLASS: dict[str, Type[SlingshotAbstractAppSpec] | Type[slingshot_yaml_schemas.EnvironmentSpec]] = {
     "run": slingshot_yaml_schemas.RunSpec,
     "deployment": slingshot_yaml_schemas.DeploymentSpec,
     "app": slingshot_yaml_schemas.SlingshotCustomAppSpec,
     "environment": slingshot_yaml_schemas.EnvironmentSpec,
 }
 
 
-def pydantic_to_dict(pydantic: BaseModel, *, exclude_unset: bool = True) -> dict[str, Any]:
-    # Convert enums to strings
-    return json.loads(pydantic.json(exclude_none=True, exclude_defaults=True, exclude_unset=exclude_unset))
-
-
 def _display_name_to_id(input_str: str) -> str:
     """Converts a name to a valid project ID by removing special characters and replacing spaces with hyphens."""
     lower = input_str.strip().lower()
     single_space = re.sub(r"\s+", "-", lower)
     single_hyphen = re.sub(r"-+", "-", single_space)
     alphanumeric_hyphen_underscore = re.sub(r"[^a-z0-9-_]", "", single_hyphen)
     return alphanumeric_hyphen_underscore
@@ -97,22 +89,15 @@
         console.print(
             "This project already has a `slingshot yaml`. You can add components to it with [bold]slingshot add[/bold]"
         )
         if not typer.confirm("Do you want to reinitialize this project from scratch?"):
             await sdk.apply_project(and_wait=True)
             return
 
-    # Touch the file
-    client_settings.slingshot_config_path.touch()
-
-    # Insert an empty schemas.SlingshotAppSpec
-    doc = pydantic_to_dict(slingshot_yaml_schemas.ProjectManifest(), exclude_unset=False)
-    yaml.indent(mapping=2, sequence=4, offset=2)
-    with client_settings.slingshot_config_path.open("w") as f:
-        yaml.dump(doc, f)
+    create_empty_project_manifest(client_settings.slingshot_config_path)
 
     first = True
     while True:
         prompt = "Do you want to add another component?" if not first else "Do you want to add a component?"
         if not prompt_confirm(prompt, default=False):
             break
         await add_component.function(sdk=sdk, component=None)
```

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/apply.py` & `slingshot_ai-0.0.16/src/slingshot/cli/apply.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 from slingshot.shared.utils import load_slingshot_project_config
 
 app = SlingshotCLIApp()
 
 
 @app.command(name="apply", requires_project=True, top_level=True, requires_auth=True)
 async def apply(
-    *, sdk: SlingshotSDK, y: bool = typer.Option(False, "--yes", "-y", help="Skip confirmation and apply changes")
+    *,
+    sdk: SlingshotSDK,
+    y: bool = typer.Option(False, "--force", "-f", help="Ignore conflicts and apply the local version to the remote"),
 ) -> None:
     """Apply the slingshot.yaml file to the current project
 
     Applies the slingshot.yaml file in the current directory to the project on Slingshot
     """
     any_changes = await sdk.apply_project(and_wait=True, force=y)
     if not any_changes:
```

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/apps.py` & `slingshot_ai-0.0.16/src/slingshot/cli/apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,17 @@
         elif sessions:
             console.print("Creating a new session")
             name = _create_session()
             await sdk.apply_project(force=applied)  # If applied, the user was already prompted. Just quietly apply.
 
             # If the user doesn't apply the prompt with the session, exit because there will not be a session to start.
             all_app_specs = await sdk.list_apps()
-            session_specs = [app_spec for app_spec in all_app_specs if app_spec.app_type == schemas.AppType.SESSION]
+            session_specs = [
+                app_spec for app_spec in all_app_specs if app_spec.app_sub_type == schemas.AppSubType.SESSION
+            ]
             if not session_specs:
                 raise SlingshotException("Session not created, exiting")
         else:
             raise typer.Exit(1)
 
     assert sdk.project
     app_spec = await sdk.api.get_app_spec_by_name(name, sdk.project.project_id)
@@ -126,15 +128,15 @@
     typer.launch(app_instance.app_instance_url)
 
 
 @app.command("list", requires_project=True)
 async def list_apps(*, sdk: SlingshotSDK) -> None:
     """List all Slingshot apps as a table"""
     app_specs = await sdk.list_apps()
-    app_specs = [spec for spec in app_specs if spec.app_type in {schemas.AppType.CUSTOM, schemas.AppType.SESSION}]
+    app_specs = [spec for spec in app_specs if spec.app_type == schemas.AppType.CUSTOM]
     if not app_specs:
         console.print(
             "No apps found! Edit [yellow]slingshot.yaml[/yellow] or use [yellow]slingshot add[/yellow] to add one."
         )
         return
 
     table = Table(title="Apps")
```

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/artifact.py` & `slingshot_ai-0.0.16/src/slingshot/cli/artifact.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/auth.py` & `slingshot_ai-0.0.16/src/slingshot/cli/auth.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/code.py` & `slingshot_ai-0.0.16/src/slingshot/cli/code.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/config/sentry_setup.py` & `slingshot_ai-0.0.16/src/slingshot/cli/config/sentry_setup.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/config/slingshot_cli.py` & `slingshot_ai-0.0.16/src/slingshot/cli/config/slingshot_cli.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/dev.py` & `slingshot_ai-0.0.16/src/slingshot/cli/dev.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/environment.py` & `slingshot_ai-0.0.16/src/slingshot/cli/environment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/inference.py` & `slingshot_ai-0.0.16/src/slingshot/cli/inference.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/logs.py` & `slingshot_ai-0.0.16/src/slingshot/cli/logs.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/machine.py` & `slingshot_ai-0.0.16/src/slingshot/cli/machine.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/main.py` & `slingshot_ai-0.0.16/src/slingshot/cli/main.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/project.py` & `slingshot_ai-0.0.16/src/slingshot/cli/project.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from typing import Optional
 
 import typer
 from rich.table import Table
 
-from slingshot.sdk.config import project_config
-
+from ..sdk.config import client_settings, project_config
 from ..sdk.errors import SlingshotException
 from ..sdk.slingshot_sdk import SlingshotSDK
 from ..sdk.utils import console
+from ..shared.utils import SlingshotFileNotFoundException, load_slingshot_project_config
 from .config.slingshot_cli import SlingshotCLIApp
-from .shared import prompt_for_single_choice
+from .shared import create_empty_project_manifest, prompt_for_single_choice
 
 app = SlingshotCLIApp()
 
 
 @app.command("list", requires_auth=True)
 async def list_projects(sdk: SlingshotSDK) -> None:
     """Lists all projects that the current user has access to."""
@@ -40,34 +40,44 @@
 
 @app.command("use", requires_auth=True, requires_project=False, top_level=True)
 async def set_tracked_project(project_id: Optional[str] = typer.Argument(None), *, sdk: SlingshotSDK) -> None:
     """
     Select which project to use for the current directory.
     """
     if project_id:
-        _set_project_id(project_id)
+        await _set_project_id(sdk, project_id)
         return
     await list_and_set_project_id(sdk)
 
 
-async def list_and_set_project_id(sdk: SlingshotSDK) -> None:
-    me = await sdk.me()
+async def list_and_set_project_id(sdk_: SlingshotSDK) -> None:
+    me = await sdk_.me()
     if not me:
         raise SlingshotException("You must be logged in to use this command.")
     projects = me.projects
     if not projects:
         console.print("No projects found.")
         return  # Can't set a project ID if user has no projects
     choice = prompt_for_single_choice(
         f"Select the project you want to work on", [i.project_id for i in projects], skip_if_one_value=True
     )
 
     project_id = projects[choice].project_id
-    _set_project_id(project_id)
+    await _set_project_id(sdk_, project_id)
 
 
-def _set_project_id(project_id: str) -> None:
+async def _set_project_id(sdk_: SlingshotSDK, project_id: str) -> None:
     old_project_id = project_config.project_id
     project_config.project_id = project_id
     if old_project_id != project_id:
         project_config.last_pushed_manifest = None
     console.print(f"This directory is now associated with the project: [bold]{project_id}[/bold]")
+    await sdk_.use_project(project_id)
+
+    try:
+        load_slingshot_project_config()
+    except SlingshotFileNotFoundException:
+        console.print("No 'slingshot.yaml' file found -- initializing one from the remote project manifest...")
+
+        create_empty_project_manifest(client_settings.slingshot_config_path)
+        await sdk_.apply_to_local(force=True)
+        console.print("Done.")
```

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/run.py` & `slingshot_ai-0.0.16/src/slingshot/cli/run.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/secret.py` & `slingshot_ai-0.0.16/src/slingshot/cli/secret.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/session.py` & `slingshot_ai-0.0.16/src/slingshot/cli/session.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/shared/code_sync.py` & `slingshot_ai-0.0.16/src/slingshot/cli/shared/code_sync.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/shared/prompt.py` & `slingshot_ai-0.0.16/src/slingshot/cli/shared/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     return (
         app.app_instance_status == schemas.AppInstanceStatus.READY
         or app.app_instance_status == schemas.AppInstanceStatus.STARTING
     )
 
 
 def filter_for_sessions(app: fragments.AppSpec) -> bool:
-    return app.app_type == schemas.AppType.SESSION
+    return app.app_sub_type == schemas.AppSubType.SESSION
 
 
 @typing.overload
 async def prompt_for_app_spec(
     sdk: SlingshotSDK,
     *filters: Callable[[fragments.AppSpec], bool],
     app_display_name: Literal['app', 'run', 'deployment', 'session'],
```

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/shared/utils.py` & `slingshot_ai-0.0.16/src/slingshot/cli/shared/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 import typer
 
 from slingshot import schemas
 from slingshot.cli.shared import prompt_confirm
+from slingshot.schemas import slingshot_schema as slingshot_yaml_schemas
 from slingshot.sdk.errors import SlingshotException
 from slingshot.sdk.slingshot_api import JSONType
+from slingshot.sdk.utils import yaml
+from slingshot.shared.utils import pydantic_to_dict
 
 if TYPE_CHECKING:
     from slingshot.sdk.slingshot_sdk import SlingshotSDK
 
 
 def format_logline(logline: schemas.LogLine) -> str:
     return logline.log
@@ -150,7 +153,18 @@
         if (
             status == schemas.AppInstanceStatus.READY
             or status == schemas.AppInstanceStatus.ERROR
             or status == schemas.AppInstanceStatus.STOPPED
         ):
             return status
     raise AssertionError("Unreachable")
+
+
+def create_empty_project_manifest(manifest_path: Path) -> None:
+    # Touch the file
+    manifest_path.touch()
+
+    # Insert an empty project manifest
+    doc = pydantic_to_dict(slingshot_yaml_schemas.ProjectManifest(), exclude_unset=False)
+    yaml.indent(mapping=2, sequence=4, offset=2)
+    with manifest_path.open("w") as f:
+        yaml.dump(doc, f)
```

### Comparing `slingshot_ai-0.0.15/src/slingshot/cli/volume.py` & `slingshot_ai-0.0.16/src/slingshot/cli/volume.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/inference_model/inference_model.py` & `slingshot_ai-0.0.16/src/slingshot/inference_model/inference_model.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/schemas/generated/schemas.py` & `slingshot_ai-0.0.16/src/slingshot/schemas/generated/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 from pydantic import BaseModel, Field, PositiveInt, constr
 
 
 class AppSpecId(BaseModel):
     app_spec_id: str = Field(..., title='App Spec Id')
 
 
+class AppSubType(str, Enum):
+    SESSION = 'SESSION'
+    LABEL_STUDIO = 'LABEL_STUDIO'
+
+
 class AppType(str, Enum):
     CUSTOM = 'CUSTOM'
-    SESSION = 'SESSION'
-    TENSORBOARD = 'TENSORBOARD'
-    GRADIO = 'GRADIO'
     RUN = 'RUN'
     DEPLOYMENT = 'DEPLOYMENT'
 
 
 class Auth0Metadata(BaseModel):
     auth0_domain: str = Field(..., title='Auth0 Domain')
     auth0_client_id: str = Field(..., title='Auth0 Client Id')
@@ -537,14 +539,15 @@
     ] = Field(..., title='Mounts')
     config_variables: Optional[Dict[str, Any]] = Field(None, title='Config Variables')
     app_port: Optional[int] = Field(None, title='App Port')
     batch_size: Optional[PositiveInt] = Field(None, title='Batch Size')
     batch_interval: Optional[PositiveInt] = Field(None, title='Batch Interval')
     soft_concurrency: Optional[PositiveInt] = Field(None, title='Soft Concurrency')
     app_type: AppType
+    app_sub_type: Optional[AppSubType] = None
 
 
 class CreateEnvironmentSpecResponse(BaseModel):
     data: Optional[List[Union[ExecutionEnvironmentSpecId, bool]]] = Field(
         None, max_items=2, min_items=2, title='Data'
     )
     error: Optional[SlingshotLogicalError] = None
```

### Comparing `slingshot_ai-0.0.15/src/slingshot/schemas/schema_extensions.py` & `slingshot_ai-0.0.16/src/slingshot/schemas/schema_extensions.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/schemas/slingshot-schema.config.json` & `slingshot_ai-0.0.16/src/slingshot/schemas/slingshot-schema.config.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999873408564816%*

 * *Differences: {"'definitions'": "{'SlingshotCustomAppSpec': {'properties': {'mounts': {'description': 'The "*

 * *                  "mounts to be attached.'}}}, 'SessionAppSpec': {'properties': {'mounts': "*

 * *                  "{'description': 'The mounts to be attached.'}}}, 'RunSpec': {'properties': "*

 * *                  "{'mounts': {'description': 'The mounts to be attached.'}}}, 'DeploymentSpec': "*

 * *                  "{'properties': {'mounts': {'description': 'The mounts to be attached.'}}}}"}*

```diff
@@ -35,15 +35,15 @@
                         }
                     ],
                     "default": "CPU_SMALL",
                     "description": "The machine size to be used.",
                     "title": "Machine size"
                 },
                 "mounts": {
-                    "description": "The mounts for the environment.",
+                    "description": "The mounts to be attached.",
                     "items": {
                         "anyOf": [
                             {
                                 "$ref": "#/definitions/DownloadByNameMountSpec"
                             },
                             {
                                 "$ref": "#/definitions/DownloadByTagMountSpec"
@@ -234,15 +234,15 @@
                         }
                     ],
                     "default": "CPU_SMALL",
                     "description": "The machine size to be used.",
                     "title": "Machine size"
                 },
                 "mounts": {
-                    "description": "The mounts for the environment.",
+                    "description": "The mounts to be attached.",
                     "items": {
                         "anyOf": [
                             {
                                 "$ref": "#/definitions/DownloadByNameMountSpec"
                             },
                             {
                                 "$ref": "#/definitions/DownloadByTagMountSpec"
@@ -307,15 +307,15 @@
                         }
                     ],
                     "default": "CPU_SMALL",
                     "description": "The machine size to be used.",
                     "title": "Machine size"
                 },
                 "mounts": {
-                    "description": "The mounts for the environment.",
+                    "description": "The mounts to be attached.",
                     "items": {
                         "anyOf": [
                             {
                                 "$ref": "#/definitions/DownloadByNameMountSpec"
                             },
                             {
                                 "$ref": "#/definitions/DownloadByTagMountSpec"
@@ -393,15 +393,15 @@
                         }
                     ],
                     "default": "CPU_SMALL",
                     "description": "The machine size to be used.",
                     "title": "Machine size"
                 },
                 "mounts": {
-                    "description": "The mounts for the environment.",
+                    "description": "The mounts to be attached.",
                     "items": {
                         "anyOf": [
                             {
                                 "$ref": "#/definitions/DownloadByNameMountSpec"
                             },
                             {
                                 "$ref": "#/definitions/DownloadByTagMountSpec"
```

### Comparing `slingshot_ai-0.0.15/src/slingshot/schemas/slingshot_schema.py` & `slingshot_ai-0.0.16/src/slingshot/schemas/slingshot_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 
 class DownloadByNameMountSpec(BaseMountSpec):
     mode: Literal["DOWNLOAD"] = Field("DOWNLOAD", title="Mode", description="The mode to use for the mount.")
     name: str = Field(
         ..., title="Name", description="The name of the asset to mount. Either name or tag should be set, but not both."
     )
 
+    class Config:
+        exclude_defaults = False
+
     def diff(self, other: BaseMountSpec) -> list[str]:
         d = super().diff(other)
         if isinstance(other, DownloadByNameMountSpec) and self.name != other.name:
             d.append(f"name: {other.name} → {self.name}")
         elif isinstance(other, DownloadByTagMountSpec):
             d.append(f"replaced tag='{other.tag}' → name='{self.name}'")
         return d
@@ -60,38 +63,47 @@
     tag: str = Field(
         ...,
         title="Tag",
         description="The artifact selector. If multiple matching artifacts contain the tag, the "
         "latest one will be used.  Either name or tag should be set, but not both.",
     )
 
+    class Config:
+        exclude_defaults = False
+
     def diff(self, other: BaseMountSpec) -> list[str]:
         d = super().diff(other)
         if isinstance(other, DownloadByTagMountSpec) and self.tag != other.tag:
             d.append(f"tag: {other.tag} → {self.tag}")
         elif isinstance(other, DownloadByNameMountSpec):
             d.append(f"replaced name='{other.name}' → tag='{self.tag}'")
         return d
 
 
 class UploadMountSpec(BaseMountSpec):
     mode: Literal["UPLOAD"] = Field("UPLOAD", title="Mode", description="The mode to use for the mount.")
     tag: Optional[str] = Field(None, title="Tag", description="Optional tag to attach to the written asset.")
 
+    class Config:
+        exclude_defaults = False
+
     def diff(self, other: BaseMountSpec) -> list[str]:
         d = super().diff(other)
         if isinstance(other, UploadMountSpec) and self.tag != other.tag:
             d.append(f"tag: {other.tag} → {self.tag}")
         return d
 
 
 class VolumeMountSpec(BaseMountSpec):
     mode: Literal["VOLUME"] = Field("VOLUME", title="Mode", description="The mode to use for the mount.")
     name: str = Field(..., title="Name", description="The name of the volume to mount.")
 
+    class Config:
+        exclude_defaults = False
+
     def diff(self, other: BaseMountSpec) -> list[str]:
         d = super().diff(other)
         if isinstance(other, VolumeMountSpec) and self.name != other.name:
             d.append(f"name: {other.name} → {self.name}")
         return d
 
 
@@ -127,14 +139,15 @@
 
     class Config:
         title = "Environment"
         description = "The environment to use for the job."
         schema_extra = {
             "example": {"gpu_drivers": True, "python_version": "3.10", "python_packages": ["numpy", "pandas"]}
         }
+        exclude_defaults = True
 
     # All python packages can be converted to RequestedRequirement
     # noinspection PyMethodParameters
     @validator("python_packages")
     def convert_python_packages(cls, v: list[str]) -> list[str]:
         for i in v:
             try:
@@ -201,30 +214,29 @@
         schemas.MachineType.CPU_SMALL, title="Machine size", description="The machine size to be used."
     )
     num_gpu: int = Field(0, title="Number of GPUs", description="The number of GPUs to use.")
     config_variables: dict[str, Any] = Field(
         default_factory=dict, title="Arguments", description="Optional user defined arguments to pass to the app."
     )
 
-    mounts: list[MountSpecUnion] = Field(
-        default_factory=list, title="Mounts", description="The mounts for the environment."
-    )
+    mounts: list[MountSpecUnion] = Field(default_factory=list, title="Mounts", description="The mounts to be attached.")
     attach_project_credentials: bool = Field(
         True,
         title="Attach project credentials",
         description=(
             "If true, will make an API key available to instances under the `SLINGSHOT_API_KEY` environment"
             "variable so that they can make requests using the Slingshot SDK for this project"
         ),
     )
 
     class Config:
         title = "App"
         description = "An app script."
         schema_extra = {"example": {"cmd": "python app.py", "environment": "slackbot"}}
+        exclude_defaults = True
 
     # noinspection PyMethodParameters
     @validator("mounts")
     def validate_mount_paths_unique(cls, v: list[MountSpecUnion]) -> list[MountSpecUnion]:
         """
         Verify that all download mount paths are unique, and all upload mount paths are unique.
         However, it should be possible for download and upload mounts to share the same mount path.
@@ -266,14 +278,18 @@
             diff.append(f"Environment changed from '{environment}' → '{self.environment}'")
         if deepdiff.DeepDiff(config_variables, self.config_variables, ignore_order=True):
             diff.append(f'Config variables changed from {config_variables} → {self.config_variables}')
         if self_machine_type != existing_machine_type:
             diff.append(f"Machine type changed from '{existing_machine_type}' → '{self_machine_type}'")
         if self_num_gpu != existing_num_gpu:
             diff.append(f"Number of GPUs changed from '{existing_num_gpu}' → '{self_num_gpu}'")
+        if self.attach_project_credentials and not existing.service_account:
+            diff.append(f"Project credentials added")
+        elif not self.attach_project_credentials and existing.service_account:
+            diff.append(f"Project credentials removed")
 
         my_mount_path = {f"{i.mode}: {i.path}": i for i in self.mounts}
         existing_mounts = {f"{i.mode}: {i.path}": i for i in existing.mount_specs}
         added_keys = set(my_mount_path.keys()) - set(existing_mounts.keys())
         for i in added_keys:
             diff.append(f"Added mount '{i}'")
         removed_keys = set(existing_mounts.keys()) - set(my_mount_path.keys())
@@ -288,104 +304,94 @@
                 diff.append(f"Changed mount '{i}': {d}")
 
         return diff
 
 
 class SlingshotCustomAppSpec(SlingshotAbstractAppSpec):
     port: Optional[int] = Field(None, title="Port", description="The port to expose.")
-
     cmd: str = Field(..., title="Command", description="The command to run.")
 
+    class Config:
+        exclude_defaults = True
+
     def diff(self, existing: fragments.AppSpec) -> list[str]:
         """Returns a list of differences between this and another app spec."""
+        if existing.app_type != schemas.AppType.CUSTOM:
+            raise ValueError(f"Cannot diff an app against a non-app.")
         diff = super().diff(existing)
         if self.cmd != existing.app_spec_command:
             diff.append(f"Command changed from '{existing.app_spec_command}' → '{self.cmd}'")
-        if existing.app_type != "CUSTOM":
-            diff.append(f"Changed to 'app'")
         if self.port != existing.app_port:
             diff.append(f"Port changed from '{existing.app_port}' → '{self.port}'")
-
-        if self.attach_project_credentials and not existing.service_account:
-            diff.append(f"Project credentials added")
-        elif not self.attach_project_credentials and existing.service_account:
-            diff.append(f"Project credentials account removed")
         return diff
 
 
 class SessionAppSpec(SlingshotAbstractAppSpec):
     using: Literal["session"] = Field(
         ...,
         title="Using",
         description="Which package to use. When specified, this feature automatically adjusts the behavior of the app.",
     )
 
+    class Config:
+        exclude_defaults = True
+
     @property
     def port(self) -> int:
         return 8080
 
     def diff(self, existing: fragments.AppSpec) -> list[str]:
         """Returns a list of differences between this and another app spec."""
+        if existing.app_sub_type != schemas.AppSubType.SESSION:
+            raise ValueError(f"Cannot diff session app against a non-session.")
         diff = super().diff(existing)
-        if self.using and self.using != existing.app_type.lower():
-            diff.append(f"Using changed from '{existing.app_type.lower()}' → '{self.using}'")
+        if self.using and self.using != existing.app_sub_type.lower():
+            diff.append(f"Plugin changed from '{existing.app_sub_type.lower()}' → '{self.using}'")
         if self.port != existing.app_port:
             diff.append(f"Port changed from '{existing.app_port}' → '{self.port}'")
-        if self.attach_project_credentials and not existing.service_account:
-            diff.append(f"Project credentials added")
-        elif not self.attach_project_credentials and existing.service_account:
-            diff.append(f"Project credentials removed")
         return diff
 
 
 class RunSpec(SlingshotAbstractAppSpec):
     name: str = Field("run", title="Name", description="The name of the run.")
-    mounts: list[MountSpecUnion] = Field(
-        default_factory=list, title="Mounts", description="The mounts for the environment."
-    )
     cmd: str = Field(..., title="Command", description="The command to run.")
 
     class Config:
         title = "Run"
         description = "Model training run"
         schema_extra = {"example": {"cmd": "python train.py", "environment": "training"}}
+        exclude_defaults = True
 
     def diff(self, existing: fragments.AppSpec) -> list[str]:
         """Returns a list of differences between this and another app spec."""
+        if existing.app_type != schemas.AppType.RUN:
+            raise ValueError(f"Cannot diff a run against a non-run.")
         diff = super().diff(existing)
         if self.cmd != existing.app_spec_command:
             diff.append(f"Command changed from '{existing.app_spec_command}' → '{self.cmd}'")
-        if self.attach_project_credentials and not existing.service_account:
-            diff.append(f"Project credentials added")
-        elif not self.attach_project_credentials and existing.service_account:
-            diff.append(f"Project credentials removed")
         return diff
 
 
 class DeploymentSpec(SlingshotAbstractAppSpec):
     name: str = Field("deployment", title="Name", description="The name of the deployment.")
     cmd: str = Field(..., title="Command", description="The command to run.")
 
     class Config:
         title = "Deployment"
         description = "Model inference deployment"
         schema_extra = {"example": {"environment": "deployment"}}
+        exclude_defaults = True
 
     def diff(self, existing: fragments.AppSpec) -> list[str]:
         """Returns a list of differences between this and another app spec."""
+        if existing.app_type != schemas.AppType.DEPLOYMENT:
+            raise ValueError(f"Cannot diff a run against a non-deployment.")
         diff = super().diff(existing)
         if self.cmd != existing.app_spec_command:
             diff.append(f"Command changed from '{existing.app_spec_command}' → '{self.cmd}'")
-        if existing.app_type != schemas.AppType.DEPLOYMENT:
-            diff.append(f"Changed to 'deployment'")
-
-        if self.attach_project_credentials and not existing.service_account:
-            diff.append(f"Project credentials added")
-        elif not self.attach_project_credentials and existing.service_account:
-            diff.append(f"Project credentials removed")
         return diff
 
 
 class ProjectManifest(BaseModel):
     environments: dict[str, EnvironmentSpec] = Field(
         default_factory=dict, title="Environments", description="The environments to use for the job."
     )
@@ -401,21 +407,26 @@
         default_factory=list, title=DeploymentSpec.Config.title, description=DeploymentSpec.Config.description
     )
 
     class Config:
         title = "Slingshot Config Spec"
         description = "The Slingshot config file."
         schema_extra = {"$schema": "http://json-schema.org/draft/2020-12/schema", "$id": FILE_LOCATION}
+        exclude_defaults = True
 
     # noinspection PyMethodParameters
-    @pydantic.root_validator
+    @pydantic.root_validator(pre=True)
     def validate_environment_names(cls, values: dict[str, Any]) -> dict[str, Any]:
         # Validate that jupyter is in all session environments:
-        sessions = [app for app in values["apps"] if isinstance(app, SessionAppSpec)]
-        envs: dict[str, EnvironmentSpec] = values["environments"]
+        sessions = [app for app in values.get("apps", []) if isinstance(app, SessionAppSpec)]
+        envs: dict[str, EnvironmentSpec] = values.get("environments", {})
+
+        if not isinstance(envs, dict):
+            raise SlingshotException(f"'environments' must be a YAML mapping (was: {type(envs)})")
+
         session_envs = {
             env_name: env
             for env_name, env in envs.items()
             if any(session.environment == env_name for session in sessions)
         }
         for session_env_name, session_env in session_envs.items():
             requested_python_requirements = session_env.python_packages
@@ -426,15 +437,20 @@
 
         # Validate that all referenced environments are in the environments list:
         for app_or_run_or_deployment in [
             *values.get("apps", []),
             *values.get("runs", []),
             *values.get("deployments", []),
         ]:
-            env = app_or_run_or_deployment.environment
+            app_ = (
+                app_or_run_or_deployment.dict()
+                if not isinstance(app_or_run_or_deployment, dict)
+                else app_or_run_or_deployment
+            )
+            env = app_.get("environment", '')
             if env not in envs:
                 raise SlingshotException(f"Environment '{env}' not found in 'environments' {list(envs.keys())}")
         return values
 
 
 if __name__ == "__main__":
     with open(Path(PATH_TO_FILE) / FILENAME, "w") as f:
```

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/apply.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/apply.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,17 @@
             custom_app_change_msgs,
         ) = _diff_existing_app_yaml_specs(existing_app_specs, custom_apps, schemas.AppType.CUSTOM, updated_env_names)
         (
             custom_session_app_specs_to_create,
             custom_session_app_specs_to_update,
             custom_session_app_specs_to_delete,
             custom_session_app_change_msgs,
-        ) = _diff_existing_app_yaml_specs(existing_app_specs, sessions, schemas.AppType.SESSION, updated_env_names)
+        ) = _diff_existing_app_yaml_specs(
+            existing_app_specs, sessions, schemas.AppType.CUSTOM, updated_env_names, schemas.AppSubType.SESSION
+        )
         (
             run_specs_to_create,
             run_specs_to_update,
             run_specs_to_delete,
             run_change_msgs,
         ) = _diff_existing_app_yaml_specs(existing_app_specs, config.runs, schemas.AppType.RUN, updated_env_names)
         (
@@ -292,19 +294,21 @@
                 raise SlingshotException(f"Failed to delete app: {e}") from e
 
     async def create_app_spec(
         self, app_spec: schemas.SlingshotAbstractAppSpec, exec_env_spec_id: str
     ) -> schemas.HasAppSpecId:
         console.print(f"Creating '{app_spec.name}'...", end="")
         app_type = _get_app_type(app_spec)
+        app_sub_type = _get_app_sub_type(app_spec)
         machine_size = machine_type_gpu_count_to_machine_size(app_spec.machine_type, app_spec.num_gpu)
         app_spec_id_response = await self._sdk.create_app(
             name=app_spec.name,
             command=app_spec.cmd if hasattr(app_spec, "cmd") else None,
             app_type=app_type,
+            app_sub_type=app_sub_type,
             exec_env_spec_id=exec_env_spec_id,
             machine_size=machine_size,
             mounts=app_spec.mounts,
             attach_project_credentials=(
                 app_spec.attach_project_credentials if hasattr(app_spec, "attach_project_credentials") else False
             ),
             config_variables=app_spec.config_variables,
@@ -323,15 +327,17 @@
             app_spec_id=existing_app_spec_id,
             name=app_spec.name,
             command=app_spec.cmd if hasattr(app_spec, "cmd") else None,
             env_spec_id=exec_env_spec_id,
             machine_size=machine_size,
             config_variables=app_spec.config_variables,
             mounts=app_spec.mounts,
-            attach_project_credentials=app_spec.service_account if hasattr(app_spec, "service_account") else False,
+            attach_project_credentials=(
+                app_spec.attach_project_credentials if hasattr(app_spec, "attach_project_credentials") else False
+            ),
             app_port=app_spec.port if hasattr(app_spec, "port") else None,
             batch_size=app_spec.batch_size if hasattr(app_spec, "batch_size") else None,
             batch_interval=app_spec.batch_interval if hasattr(app_spec, "batch_interval") else None,
         )
         console.print("✅ ")
 
     async def delete_app_spec(self, app_spec: fragments.AppSpec) -> None:
@@ -496,14 +502,16 @@
         keys = parse_keys(key_path)
         d = local_slingshot_yaml
         for k in keys[:-1]:
             d = d[k]  # type: ignore[index]
         new_value = value["new_value"]
         if isinstance(new_value, Enum):
             new_value = new_value.value
+        if isinstance(new_value, dict):
+            new_value = {k: v.value if isinstance(v, Enum) else v for k, v in new_value.items()}
         d[keys[-1]] = new_value  # type: ignore[index]
     for key_path in diff.get("dictionary_item_added", []):
         keys = parse_keys(key_path)
         d = local_slingshot_yaml
         d_ref = remote_manifest.dict()
         for k in keys[:-1]:
             d = d[k]  # type: ignore[index]
@@ -729,24 +737,26 @@
     if force:
         diff = DeepDiff(load_slingshot_project_config().dict(), reference_manifest.dict(), ignore_order=True)
     with edit_slingshot_yaml(raise_if_absent=True) as slingshot_yaml:
         apply_diff(slingshot_yaml, diff, reference_manifest)
 
 
 def _get_app_type(spec: schemas.SlingshotAbstractAppSpec) -> schemas.AppType:
-    if isinstance(spec, (schemas.RunSpec, schemas.RunSpec)):
+    if isinstance(spec, schemas.RunSpec):
         return schemas.AppType.RUN
-    elif isinstance(spec, (schemas.DeploymentSpec, schemas.DeploymentSpec)):
+    elif isinstance(spec, schemas.DeploymentSpec):
         return schemas.AppType.DEPLOYMENT
-    elif isinstance(spec, (schemas.SessionAppSpec, schemas.SessionAppSpec)):
-        return schemas.AppType.SESSION
-    elif isinstance(spec, (schemas.SlingshotCustomAppSpec, schemas.SlingshotCustomAppSpec)):
-        return schemas.AppType.CUSTOM
     else:
-        raise SlingshotException(f"Unknown app type: {spec}")
+        return schemas.AppType.CUSTOM
+
+
+def _get_app_sub_type(spec: schemas.SlingshotAbstractAppSpec) -> schemas.AppSubType | None:
+    if isinstance(spec, schemas.SessionAppSpec):
+        return schemas.AppSubType.SESSION
+    return None
 
 
 def _get_envs_requiring_gpu(config: schemas.ProjectManifest) -> set[str]:
     apps_runs_deployments = config.apps + config.runs + config.deployments
     envs_that_require_gpu = {app.environment for app in apps_runs_deployments if app.num_gpu and app.num_gpu > 0}
     return envs_that_require_gpu
 
@@ -801,26 +811,27 @@
 
 
 def _diff_existing_app_yaml_specs(
     all_existing_app_specs: list[fragments.AppSpec],
     yaml_app_specs: list[schemas.SlingshotAbstractAppSpec],
     app_type: schemas.AppType,
     updated_env_names: set[str],
+    app_sub_type: schemas.AppSubType | None = None,
 ) -> tuple[
     list[schemas.SlingshotAbstractAppSpec],
     list[tuple[schemas.SlingshotAbstractAppSpec, str]],
     list[fragments.AppSpec],
     list[str],
 ]:
     spec_display_type = "app"
     if app_type == schemas.AppType.DEPLOYMENT:
         spec_display_type = "deployment"
     elif app_type == schemas.AppType.RUN:
         spec_display_type = "run"
-    elif app_type == schemas.AppType.SESSION:
+    if app_sub_type == schemas.AppSubType.SESSION:
         spec_display_type = "session"
 
     app_specs_to_create: list[schemas.SlingshotAbstractAppSpec] = []
     app_specs_to_update: list[tuple[schemas.SlingshotAbstractAppSpec, str]] = []
     app_specs_to_delete: list[fragments.AppSpec] = []
 
     existing_app_specs = [spec for spec in all_existing_app_specs if spec.app_type == app_type]
@@ -836,29 +847,29 @@
             app_specs_to_create.append(app_spec)
             continue
 
         existing_app_spec = existing_spec_name_to_spec[app_spec.name]
         _change_msgs: list[str] = []
         if app_spec_diff := app_spec.diff(existing_app_spec):
             _change_msgs.extend(f"\t- {i}" for i in app_spec_diff)
-        #     Experiment with removing these, see if things get less annoying
-        # if app_spec.environment in updated_env_names:
-        #     _change_msgs.append(f"\t- Environment '{app_spec.environment}' has been updated")
         if _change_msgs:
             change_msgs.append(f"Detected [yellow]changes[/yellow] to {spec_display_type} '{app_spec.name}'")
             change_msgs.extend(_change_msgs)
-            if app_type in (schemas.AppType.CUSTOM, schemas.AppType.DEPLOYMENT, schemas.AppType.SESSION):
+            if app_type in (schemas.AppType.CUSTOM, schemas.AppType.DEPLOYMENT):
                 change_msgs.append(f"\t(Your {spec_display_type} will not be restarted)")
 
         # Only update if there are changes to the app spec itself, not just the environment
         if len(app_spec_diff) > 0:
             app_specs_to_update.append((app_spec, existing_app_spec.app_spec_id))
 
     for existing_app_spec in existing_app_specs:
-        if existing_app_spec.app_spec_name not in yaml_app_spec_names:
+        if (
+            existing_app_spec.app_spec_name not in yaml_app_spec_names
+            and existing_app_spec.app_sub_type == app_sub_type
+        ):
             console.print(
                 f"Detected {spec_display_type} '{existing_app_spec.app_spec_name}' has been [red]deleted[/red]"
             )
             console.print(f"\t- {spec_display_type.title()} will be [red]deleted[/red]")
             app_specs_to_delete.append(existing_app_spec)
 
     return app_specs_to_create, app_specs_to_update, app_specs_to_delete, change_msgs
@@ -901,29 +912,29 @@
         cmd = spec.app_spec_command
         machine_type, num_gpu = machine_size_to_machine_type_gpu_count(spec.machine_size)
 
         mounts = [
             parse_obj_as(schemas.MountSpecUnion, {"mode": i.mode, "name": i.name, "path": i.path, "tag": i.tag})
             for i in spec.mount_specs
         ]
-        if spec.app_type == schemas.AppType.CUSTOM:
+        if spec.app_type == schemas.AppType.CUSTOM and spec.app_sub_type is None:
             app_specs.append(
                 schemas.SlingshotCustomAppSpec(
                     name=name,
                     environment=environment,
                     machine_type=machine_type,
                     num_gpu=num_gpu,
                     config_variables=config_variables,
                     port=port,
                     attach_project_credentials=attach_project_credentials,
                     cmd=cmd,
                     mounts=mounts,
                 )
             )
-        elif spec.app_type == schemas.AppType.SESSION:
+        elif spec.app_type == schemas.AppType.CUSTOM and spec.app_sub_type == schemas.AppSubType.SESSION:
             app_specs.append(
                 schemas.SessionAppSpec(
                     name=name,
                     environment=environment,
                     machine_type=machine_type,
                     num_gpu=num_gpu,
                     config_variables=config_variables,
```

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/auth.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/config.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/config.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/config_utils.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/config_utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/data_collector.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/errors.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/errors.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/base_graphql.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/base_graphql.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/fragments.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/fragments.py`

 * *Files 5% similar despite different names*

```diff
@@ -244,19 +244,21 @@
     _depends_on = []
     _fragment = """
         fragment BillingLineItem on BillingLineItems {
           appInstanceId
           deploymentId
           runId
           computeCostCredits
+          computeCostCreditsInProgress
         } """
     app_instance_id: Optional[str] = Field(..., alias="appInstanceId")
     deployment_id: Optional[str] = Field(..., alias="deploymentId")
     run_id: Optional[str] = Field(..., alias="runId")
     compute_cost_credits: Optional[int] = Field(..., alias="computeCostCredits")
+    compute_cost_credits_in_progress: int = Field(..., alias="computeCostCreditsInProgress")
 
 
 class ProjectProjection(BaseModel):
     project: Optional[ProjectFields]
 
 
 class UserWithProjects(BaseGraphQLEntity):
@@ -391,14 +393,15 @@
     _depends_on = [ExecutionEnvironmentSpec, MountSpec, Deployment]
     _fragment = """
         fragment SlingshotAppSpec on AppSpecs {
             appSpecId
             appSpecName
             appSpecCommand
             appType
+            appSubType
             projectId
             machineSize
             configVariables
             serviceAccount
             appPort
             batchSize
             batchInterval
@@ -419,14 +422,15 @@
             }
         }
     """
     app_spec_id: str = Field(..., alias="appSpecId")
     app_spec_name: str = Field(..., alias="appSpecName")
     app_spec_command: Optional[str] = Field(..., alias="appSpecCommand")
     app_type: schemas.AppType = Field(..., alias="appType")
+    app_sub_type: Optional[schemas.AppSubType] = Field(..., alias="appSubType")
     app_port: Optional[int] = Field(..., alias="appPort")
     config_variables: Optional[str] = Field(..., alias="configVariables")
     batch_size: Optional[int] = Field(..., alias="batchSize")
     batch_interval: Optional[int] = Field(..., alias="batchInterval")
     project_id: str = Field(..., alias="projectId")
     machine_size: schemas.MachineSize = Field(..., alias="machineSize")
     service_account: bool = Field(..., alias="serviceAccount")
@@ -466,14 +470,15 @@
     _depends_on = [AppSpec]
     _fragment = """
         fragment AppInstance on AppInstances {
             appInstanceId
             appInstanceStatus
             appInstanceUrl
             appType
+            appSubType
             appPort
             sshPort
             executionEnvironmentId
             createdAt
             appSpecCommand
             appSpecId
             appSpec {
@@ -481,14 +486,15 @@
             }
         }
     """
     app_instance_id: str = Field(..., alias="appInstanceId")
     app_instance_status: schemas.AppInstanceStatus = Field(..., alias="appInstanceStatus")
     app_instance_url: Optional[str] = Field(..., alias="appInstanceUrl")
     app_type: schemas.AppType = Field(..., alias="appType")
+    app_sub_type: Optional[schemas.AppSubType] = Field(..., alias="appSubType")
     app_port: Optional[int] = Field(..., alias="appPort")
     ssh_port: Optional[int] = Field(..., alias="sshPort")
     execution_environment_id: str = Field(..., alias="executionEnvironmentId")
     created_at: datetime = Field(..., alias="createdAt")
     app_spec_command: str = Field(..., alias="appSpecCommand")
     app_spec_id: str = Field(..., alias="appSpecId")
     app_spec: AppSpec = Field(..., alias="appSpec")
```

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/apps.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/apps.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/deployment.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/deployment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/environment.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/environment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/project.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/project.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/run.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/run.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/graphql/queries/storage.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/graphql/queries/storage.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/slingshot_api.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/slingshot_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -630,14 +630,15 @@
         )
 
     async def create_app(
         self,
         name: str,
         command: str | None,
         app_type: schemas.AppType,
+        app_sub_type: schemas.AppSubType | None,
         exec_env_spec_id: str,
         machine_size: schemas.MachineSize,
         mounts: list[schemas.MountSpecUnion],
         attach_project_credentials: bool,
         config_variables: JSONType | None = None,
         app_port: int | None = None,
         *,
@@ -645,14 +646,15 @@
     ) -> schemas.AppSpecIdResponse:
         """Create an app spec."""
         mount_requests = [parse_obj_as(schemas.MountRequestUnion, i) for i in mounts]
         body = schemas.CreateAppBody(
             name=name,
             command=command,
             app_type=app_type,
+            app_sub_type=app_sub_type,
             exec_env_spec_id=exec_env_spec_id,
             machine_size=machine_size,
             mounts=mount_requests,
             attach_project_credentials=attach_project_credentials,
             config_variables=config_variables,
             app_port=app_port,
         ).dict()
@@ -800,15 +802,15 @@
         attach_project_credentials: bool | None = None,
         app_port: int | None = None,
         project_id: str,
     ) -> schemas.HasAppInstanceIdResponse:
         """Start an app."""
         # TODO: Separate the SDK logic (using existing spec) from the API logic
 
-        if app_spec.app_type == schemas.AppType.SESSION:
+        if app_spec.app_sub_type == schemas.AppSubType.SESSION:
             cmd = """bash -c "echo 'This command should never run!'; exit 1"""
 
         machine_size = machine_size or app_spec.machine_size
         command = cmd or app_spec.app_spec_command
         if mount_specs is None:
             mount_specs = [schemas.mount_spec_from_remote(mount_spec) for mount_spec in app_spec.mount_specs]
         if config_variables is None and app_spec.config_variables is not None:
```

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/slingshot_sdk.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/slingshot_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -828,22 +828,14 @@
         project_id = await self._get_current_project_id_or_raise()
         return await self._api.list_secrets(project_id=project_id)
 
     async def list_machine_types(self) -> list[schemas.MachineTypeListItem]:
         """List all machine types."""
         return await self._api.list_machine_types()
 
-    # TODO: remove this method and refactor session-related methods to reuse logic for apps
-    async def get_session_app_spec(self) -> fragments.AppSpec | None:
-        """Get the first session in the current project."""
-        project_id = await self._get_current_project_id_or_raise()
-        app_specs = await self._api.list_app_specs(project_id=project_id)
-        session_app_specs = [app_spec for app_spec in app_specs if app_spec.app_type == schemas.AppType.SESSION.value]
-        return session_app_specs[0] if session_app_specs else None
-
     """
     Get SDK methods
     """
 
     async def get_app(self, app_name: str) -> fragments.AppSpec | None:
         """Get an app by name."""
         project_id = await self._get_current_project_id_or_raise()
@@ -887,24 +879,26 @@
         name: str,
         command: str | None,
         app_type: schemas.AppType,
         exec_env_spec_id: str,
         machine_size: schemas.MachineSize,
         mounts: list[schemas.MountSpecUnion],
         attach_project_credentials: bool,
+        app_sub_type: schemas.AppSubType | None = None,
         config_variables: JSONType | None = None,
         app_port: int | None = None,
     ) -> schemas.AppSpecIdResponse:
         """Create a new app with the given name and configuration."""
         # TODO: this also supports creating runs/templates, but not sure if we should keep this behavior
         project_id = await self._get_current_project_id_or_raise()
         return await self._api.create_app(
             name=name,
             command=command,
             app_type=app_type,
+            app_sub_type=app_sub_type,
             exec_env_spec_id=exec_env_spec_id,
             machine_size=machine_size,
             mounts=mounts,
             attach_project_credentials=attach_project_credentials,
             config_variables=config_variables,
             app_port=app_port,
             project_id=project_id,
```

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/sync.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/sync.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/upload_download_utils.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/upload_download_utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/utils.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/sdk/web_path_util.py` & `slingshot_ai-0.0.16/src/slingshot/sdk/web_path_util.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/shared/utils.py` & `slingshot_ai-0.0.16/src/slingshot/shared/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 from __future__ import annotations
 
+import json
 import typing
+from typing import Any
 
-import yaml
-from pydantic import ValidationError
+from pydantic import BaseModel, ValidationError
+from ruamel import yaml as r_yaml
 
 from slingshot import schemas
 from slingshot.sdk.config import client_settings
 from slingshot.sdk.errors import SlingshotException
 
+yaml = r_yaml.YAML()
+
+
+class SlingshotFileNotFoundException(SlingshotException):
+    pass
+
 
 def load_slingshot_project_config() -> schemas.ProjectManifest:
     try:
         text = client_settings.slingshot_config_path.read_text()
     except FileNotFoundError as e:
-        raise SlingshotException(
+        raise SlingshotFileNotFoundException(
             f"Could not find slingshot.yaml at {client_settings.slingshot_config_path}.\n"
             f"You can add one by running 'slingshot init'"
         ) from e
     try:
-        d = yaml.safe_load(text)
-    except yaml.YAMLError as e:
+        d = r_yaml.safe_load(text)
+    except r_yaml.YAMLError as e:
         raise SlingshotException(f"Could not parse slingshot.yaml in {client_settings.slingshot_config_path}") from e
     if not d:
         raise SlingshotException(
             f"Empty slingshot.yaml in {client_settings.slingshot_config_path}. Please run 'slingshot init'"
         )
     try:
         return schemas.ProjectManifest.parse_obj(d)
@@ -95,14 +103,17 @@
                         )
                         return SlingshotException(message)
                     except Exception:
                         pass
                 except Exception:
                     pass
 
+    if isinstance(e, SlingshotException):
+        return e
+
     return SlingshotException(f"Invalid slingshot.yaml: {e=}")
 
 
 T = typing.TypeVar("T")
 
 
 class ResponseProtocol(typing.Protocol[T]):
@@ -140,7 +151,12 @@
     return _machine_size_to_machine_type_gpu_count[machine_size]
 
 
 def machine_type_gpu_count_to_machine_size(machine_type: schemas.MachineType, gpu_count: int) -> schemas.MachineSize:
     if (machine_type, gpu_count) not in _machine_type_gpu_count_to_machine_size:
         raise ValueError(f"Unknown machine type {machine_type} with {gpu_count} GPUs")
     return _machine_type_gpu_count_to_machine_size[(machine_type, gpu_count)]
+
+
+def pydantic_to_dict(pydantic: BaseModel, *, exclude_unset: bool = True) -> dict[str, Any]:
+    # Convert enums to strings
+    return json.loads(pydantic.json(exclude_none=True, exclude_unset=exclude_unset))
```

### Comparing `slingshot_ai-0.0.15/src/slingshot/templates/inference_template.py` & `slingshot_ai-0.0.16/src/slingshot/templates/inference_template.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/src/slingshot/templates/label_studio_data_export_template.py` & `slingshot_ai-0.0.16/src/slingshot/templates/label_studio_data_export_template.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.15/PKG-INFO` & `slingshot_ai-0.0.16/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: slingshot-ai
-Version: 0.0.15
+Version: 0.0.16
 Summary: 
 Author: Slingshot AI
 Author-email: service-account@slingshot.xyz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.1,<3.9.0)
 Requires-Dist: backoff (>=2.0.0,<2.1.0)
 Requires-Dist: deepdiff (>=6.3.0,<6.4.0)
 Requires-Dist: fastapi (>=0.88.0,<0.89.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: pydantic (==1.9)
+Requires-Dist: pydantic (<=1.10.11)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.1,<2.29.0)
 Requires-Dist: ruamel.yaml (>=0.17.0,<0.18.0)
-Requires-Dist: sentry-sdk (>=1.13.0,<1.14.0)
+Requires-Dist: sentry-sdk (>=1.16.0,<1.17.0)
 Requires-Dist: sh (>=1.14.3,<1.15.0)
 Requires-Dist: simple-term-menu (>=1.6.0,<1.7.0)
 Requires-Dist: tqdm (>=4.63.0,<4.64.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Requires-Dist: urllib3 (>=1.26.11,<1.27.0)
 Requires-Dist: uvicorn[standard] (>=0.18.0,<0.19.0)
```


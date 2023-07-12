# Comparing `tmp/proteus_cli-1.0.0.tar.gz` & `tmp/proteus_cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus_cli-1.0.0.tar", max compression
+gzip compressed data, was "proteus_cli-1.1.0.tar", max compression
```

## Comparing `proteus_cli-1.0.0.tar` & `proteus_cli-1.1.0.tar`

### file list

```diff
@@ -1,49 +1,53 @@
--rw-r--r--   0        0        0     3124 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/__init__.py
--rw-r--r--   0        0        0      384 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/api/__init__.py
--rw-r--r--   0        0        0     1784 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/api/decorators.py
--rw-r--r--   0        0        0      849 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/api/hooks.py
--rw-r--r--   0        0        0        0 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/buckets/__init__.py
--rw-r--r--   0        0        0     1092 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/buckets/commands.py
--rw-r--r--   0        0        0     2810 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/config.py
--rw-r--r--   0        0        0        0 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/__init__.py
--rw-r--r--   0        0        0     1277 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/commands.py
--rw-r--r--   0        0        0        0 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/__init__.py
--rw-r--r--   0        0        0     6754 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/__init__.py
--rw-r--r--   0        0        0     1068 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/cnn_pca/__init__.py
--rw-r--r--   0        0        0      789 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/cnn_pca/case.py
--rw-r--r--   0        0        0     2381 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/cnn_pca/common.py
--rw-r--r--   0        0        0      142 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/cnn_pca/step.py
--rw-r--r--   0        0        0      167 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/well_model/__init__.py
--rw-r--r--   0        0        0     2762 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/well_model/case.py
--rw-r--r--   0        0        0     1415 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/well_model/common.py
--rw-r--r--   0        0        0      145 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/well_model/step.py
--rw-r--r--   0        0        0      673 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/init_keywords.json
--rw-r--r--   0        0        0    12408 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/preprocess_functions.py
--rw-r--r--   0        0        0     7051 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/process_step.py
--rw-r--r--   0        0        0      411 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/well_init_keywords.json
--rw-r--r--   0        0        0        0 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/sources/__init__.py
--rw-r--r--   0        0        0     8822 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/sources/az.py
--rw-r--r--   0        0        0     1289 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/sources/common.py
--rw-r--r--   0        0        0     3895 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/sources/local.py
--rw-r--r--   0        0        0     1783 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/sources/s3.py
--rw-r--r--   0        0        0     6930 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/upload.py
--rw-r--r--   0        0        0        0 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/debugger/__init__.py
--rw-r--r--   0        0        0     2265 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/debugger/commands.py
--rw-r--r--   0        0        0     3926 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/debugger/init_keyword_check.py
--rw-r--r--   0        0        0        0 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/debugger/restart_keyword_check.py
--rw-r--r--   0        0        0        0 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/jobs/__init__.py
--rw-r--r--   0        0        0     1283 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/jobs/commands.py
--rw-r--r--   0        0        0     3026 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/jobs/list.py
--rw-r--r--   0        0        0      100 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/runtime.py
--rw-r--r--   0        0        0        0 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/simulations/__init__.py
--rw-r--r--   0        0        0     2460 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/simulations/commands.py
--rw-r--r--   0        0        0     7603 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/simulations/create.py
--rw-r--r--   0        0        0     4119 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/simulations/dependencySolver.py
--rw-r--r--   0        0        0     5190 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/simulations/opm.py
--rw-r--r--   0        0        0        0 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/utils/__init__.py
--rw-r--r--   0        0        0     8114 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/utils/files.py
--rw-r--r--   0        0        0      385 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/utils/sssh.py
--rw-r--r--   0        0        0     1917 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/utils/sync.py
--rw-r--r--   0        0        0      449 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/logging.ini
--rw-r--r--   0        0        0     1528 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 proteus_cli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3124 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/__init__.py
+-rw-r--r--   0        0        0      384 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/api/__init__.py
+-rw-r--r--   0        0        0     1784 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/api/decorators.py
+-rw-r--r--   0        0        0      849 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/api/hooks.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/buckets/__init__.py
+-rw-r--r--   0        0        0     1092 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/buckets/commands.py
+-rw-r--r--   0        0        0     2810 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/config.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     1277 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/commands.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/__init__.py
+-rw-r--r--   0        0        0     6754 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/config/__init__.py
+-rw-r--r--   0        0        0     1068 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/config/cnn_pca/__init__.py
+-rw-r--r--   0        0        0      789 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/config/cnn_pca/case.py
+-rw-r--r--   0        0        0     2381 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/config/cnn_pca/common.py
+-rw-r--r--   0        0        0      142 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/config/cnn_pca/step.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/config/facilities/__init__.py
+-rw-r--r--   0        0        0     1166 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/config/facilities/case.py
+-rw-r--r--   0        0        0      825 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/config/facilities/common.py
+-rw-r--r--   0        0        0      146 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/config/facilities/step.py
+-rw-r--r--   0        0        0      167 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/config/well_model/__init__.py
+-rw-r--r--   0        0        0     2762 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/config/well_model/case.py
+-rw-r--r--   0        0        0     1415 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/config/well_model/common.py
+-rw-r--r--   0        0        0      145 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/config/well_model/step.py
+-rw-r--r--   0        0        0      673 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/init_keywords.json
+-rw-r--r--   0        0        0    12408 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/preprocess_functions.py
+-rw-r--r--   0        0        0     7051 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/process_step.py
+-rw-r--r--   0        0        0      411 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/preprocessor/well_init_keywords.json
+-rw-r--r--   0        0        0        0 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/sources/__init__.py
+-rw-r--r--   0        0        0     8822 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/sources/az.py
+-rw-r--r--   0        0        0     1289 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/sources/common.py
+-rw-r--r--   0        0        0     3895 2023-07-12 10:35:32.370653 proteus_cli-1.1.0/cli/datasets/sources/local.py
+-rw-r--r--   0        0        0     1783 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/datasets/sources/s3.py
+-rw-r--r--   0        0        0     6930 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/datasets/upload.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/debugger/__init__.py
+-rw-r--r--   0        0        0     2265 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/debugger/commands.py
+-rw-r--r--   0        0        0     3926 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/debugger/init_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/debugger/restart_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/jobs/__init__.py
+-rw-r--r--   0        0        0     1283 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/jobs/commands.py
+-rw-r--r--   0        0        0     3026 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/jobs/list.py
+-rw-r--r--   0        0        0      100 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/runtime.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/simulations/__init__.py
+-rw-r--r--   0        0        0     2460 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/simulations/commands.py
+-rw-r--r--   0        0        0     7603 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/simulations/create.py
+-rw-r--r--   0        0        0     4119 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/simulations/dependencySolver.py
+-rw-r--r--   0        0        0     5190 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/simulations/opm.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/utils/__init__.py
+-rw-r--r--   0        0        0     8114 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/utils/files.py
+-rw-r--r--   0        0        0      385 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/utils/sssh.py
+-rw-r--r--   0        0        0     1917 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/cli/utils/sync.py
+-rw-r--r--   0        0        0      449 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/logging.ini
+-rw-r--r--   0        0        0     1528 2023-07-12 10:35:32.374653 proteus_cli-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 proteus_cli-1.1.0/PKG-INFO
```

### Comparing `proteus_cli-1.0.0/cli/__init__.py` & `proteus_cli-1.1.0/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/api/decorators.py` & `proteus_cli-1.1.0/cli/api/decorators.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/api/hooks.py` & `proteus_cli-1.1.0/cli/api/hooks.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/buckets/commands.py` & `proteus_cli-1.1.0/cli/buckets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/config.py` & `proteus_cli-1.1.0/cli/config.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/datasets/commands.py` & `proteus_cli-1.1.0/cli/datasets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/datasets/preprocessor/config/__init__.py` & `proteus_cli-1.1.0/cli/datasets/preprocessor/config/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/datasets/preprocessor/config/cnn_pca/__init__.py` & `proteus_cli-1.1.0/cli/datasets/preprocessor/config/cnn_pca/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/datasets/preprocessor/config/cnn_pca/case.py` & `proteus_cli-1.1.0/cli/datasets/preprocessor/config/cnn_pca/case.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/datasets/preprocessor/config/cnn_pca/common.py` & `proteus_cli-1.1.0/cli/datasets/preprocessor/config/cnn_pca/common.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/datasets/preprocessor/config/well_model/case.py` & `proteus_cli-1.1.0/cli/datasets/preprocessor/config/well_model/case.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/datasets/preprocessor/config/well_model/common.py` & `proteus_cli-1.1.0/cli/datasets/preprocessor/config/well_model/common.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/datasets/preprocessor/init_keywords.json` & `proteus_cli-1.1.0/cli/datasets/preprocessor/init_keywords.json`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/datasets/preprocessor/preprocess_functions.py` & `proteus_cli-1.1.0/cli/datasets/preprocessor/preprocess_functions.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/datasets/preprocessor/process_step.py` & `proteus_cli-1.1.0/cli/datasets/preprocessor/process_step.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/datasets/sources/az.py` & `proteus_cli-1.1.0/cli/datasets/sources/az.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/datasets/sources/common.py` & `proteus_cli-1.1.0/cli/datasets/sources/common.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/datasets/sources/local.py` & `proteus_cli-1.1.0/cli/datasets/sources/local.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/datasets/sources/s3.py` & `proteus_cli-1.1.0/cli/datasets/sources/s3.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/datasets/upload.py` & `proteus_cli-1.1.0/cli/datasets/upload.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/debugger/commands.py` & `proteus_cli-1.1.0/cli/debugger/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/debugger/init_keyword_check.py` & `proteus_cli-1.1.0/cli/debugger/init_keyword_check.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/jobs/commands.py` & `proteus_cli-1.1.0/cli/jobs/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/jobs/list.py` & `proteus_cli-1.1.0/cli/jobs/list.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/simulations/commands.py` & `proteus_cli-1.1.0/cli/simulations/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/simulations/create.py` & `proteus_cli-1.1.0/cli/simulations/create.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/simulations/dependencySolver.py` & `proteus_cli-1.1.0/cli/simulations/dependencySolver.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/simulations/opm.py` & `proteus_cli-1.1.0/cli/simulations/opm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/utils/files.py` & `proteus_cli-1.1.0/cli/utils/files.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/cli/utils/sync.py` & `proteus_cli-1.1.0/cli/utils/sync.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.0.0/pyproject.toml` & `proteus_cli-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proteus-cli"
-version = "1.0.0"
+version = "1.1.0"
 description = ""
 authors = []
 packages = [
     {include="cli"},
     {include="logging.ini"}
 ]
 
@@ -18,15 +18,15 @@
 tqdm = "^4.61.0"
 tabulate = "^0.8.9"
 azure-storage-blob = "^12.8.1"
 readchar = "^3.0.4"
 azure-identity = "^1.12.0"
 markupsafe = "2.0.1"
 proteus-runtime = "0.3.0"
-proteus-preprocessing = "0.3.0"
+proteus-preprocessing = "0.4.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 pre-commit = "^2.9.3"
 pytest-mock = "^3.5.1"
 requests-mock = "^1.8.0"
 pytest-bdd = "^5.0.0"
```

### Comparing `proteus_cli-1.0.0/PKG-INFO` & `proteus_cli-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: proteus-cli
-Version: 1.0.0
+Version: 1.1.0
 Summary: 
 Requires-Python: >=3.8,<3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: azure-identity (>=1.12.0,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.8.1,<13.0.0)
 Requires-Dist: boto3 (>=1.17.79,<2.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: cryptography (>=3.3.2,<4.0.0)
 Requires-Dist: jwt (>=1.2.0,<2.0.0)
 Requires-Dist: markupsafe (==2.0.1)
-Requires-Dist: proteus-preprocessing (==0.3.0)
+Requires-Dist: proteus-preprocessing (==0.4.0)
 Requires-Dist: proteus-runtime (==0.3.0)
 Requires-Dist: pycryptodome (>=3.10.1,<4.0.0)
 Requires-Dist: readchar (>=3.0.4,<4.0.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: tqdm (>=4.61.0,<5.0.0)
```


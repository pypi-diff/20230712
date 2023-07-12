# Comparing `tmp/silverback-0.1.0b6.tar.gz` & `tmp/silverback-0.1.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silverback-0.1.0b6.tar", last modified: Mon Jun 19 21:57:26 2023, max compression
+gzip compressed data, was "silverback-0.1.0b7.tar", last modified: Wed Jul 12 02:49:20 2023, max compression
```

## Comparing `silverback-0.1.0b6.tar` & `silverback-0.1.0b7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:26.218118 silverback-0.1.0b6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:26.214118 silverback-0.1.0b6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:26.214118 silverback-0.1.0b6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:26.214118 silverback-0.1.0b6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-19 21:56:12.000000 silverback-0.1.0b6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-19 21:56:12.000000 silverback-0.1.0b6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-19 21:56:12.000000 silverback-0.1.0b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-19 21:57:26.218118 silverback-0.1.0b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-19 21:56:12.000000 silverback-0.1.0b6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-19 21:56:12.000000 silverback-0.1.0b6/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-19 21:56:12.000000 silverback-0.1.0b6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-19 21:57:26.218118 silverback-0.1.0b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-19 21:56:12.000000 silverback-0.1.0b6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:26.214118 silverback-0.1.0b6/silverback/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-19 21:57:25.000000 silverback-0.1.0b6/silverback/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:26.218118 silverback-0.1.0b6/silverback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-19 21:57:25.000000 silverback-0.1.0b6/silverback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-19 21:57:26.000000 silverback-0.1.0b6/silverback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:57:25.000000 silverback-0.1.0b6/silverback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 21:57:25.000000 silverback-0.1.0b6/silverback.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:57:25.000000 silverback-0.1.0b6/silverback.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-19 21:57:25.000000 silverback-0.1.0b6/silverback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 21:57:25.000000 silverback-0.1.0b6/silverback.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:26.218118 silverback-0.1.0b6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:56:12.000000 silverback-0.1.0b6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-19 21:56:12.000000 silverback-0.1.0b6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-19 21:56:12.000000 silverback-0.1.0b6/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:49:20.381355 silverback-0.1.0b7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:49:20.377355 silverback-0.1.0b7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:49:20.381355 silverback-0.1.0b7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-12 02:48:11.000000 silverback-0.1.0b7/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-12 02:48:11.000000 silverback-0.1.0b7/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-12 02:48:11.000000 silverback-0.1.0b7/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-12 02:48:11.000000 silverback-0.1.0b7/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-12 02:48:11.000000 silverback-0.1.0b7/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:49:20.381355 silverback-0.1.0b7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-12 02:48:11.000000 silverback-0.1.0b7/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-12 02:48:11.000000 silverback-0.1.0b7/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-12 02:48:11.000000 silverback-0.1.0b7/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-12 02:48:11.000000 silverback-0.1.0b7/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-12 02:48:11.000000 silverback-0.1.0b7/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-12 02:48:11.000000 silverback-0.1.0b7/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-12 02:48:11.000000 silverback-0.1.0b7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-12 02:48:11.000000 silverback-0.1.0b7/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-12 02:48:11.000000 silverback-0.1.0b7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-12 02:48:11.000000 silverback-0.1.0b7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-12 02:48:11.000000 silverback-0.1.0b7/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-12 02:48:11.000000 silverback-0.1.0b7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-12 02:49:20.381355 silverback-0.1.0b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-12 02:48:11.000000 silverback-0.1.0b7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-12 02:48:11.000000 silverback-0.1.0b7/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-12 02:48:11.000000 silverback-0.1.0b7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-12 02:49:20.381355 silverback-0.1.0b7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-12 02:48:11.000000 silverback-0.1.0b7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:49:20.381355 silverback-0.1.0b7/silverback/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-12 02:48:11.000000 silverback-0.1.0b7/silverback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-12 02:48:11.000000 silverback-0.1.0b7/silverback/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-12 02:48:11.000000 silverback-0.1.0b7/silverback/_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-12 02:48:11.000000 silverback-0.1.0b7/silverback/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-12 02:48:11.000000 silverback-0.1.0b7/silverback/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-12 02:48:11.000000 silverback-0.1.0b7/silverback/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:48:11.000000 silverback-0.1.0b7/silverback/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-12 02:48:11.000000 silverback-0.1.0b7/silverback/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-12 02:48:11.000000 silverback-0.1.0b7/silverback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-12 02:48:11.000000 silverback-0.1.0b7/silverback/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-12 02:49:20.000000 silverback-0.1.0b7/silverback/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:49:20.381355 silverback-0.1.0b7/silverback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-12 02:49:20.000000 silverback-0.1.0b7/silverback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-12 02:49:20.000000 silverback-0.1.0b7/silverback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 02:49:20.000000 silverback-0.1.0b7/silverback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 02:49:20.000000 silverback-0.1.0b7/silverback.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 02:49:20.000000 silverback-0.1.0b7/silverback.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-12 02:49:20.000000 silverback-0.1.0b7/silverback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 02:49:20.000000 silverback-0.1.0b7/silverback.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:49:20.381355 silverback-0.1.0b7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:48:11.000000 silverback-0.1.0b7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-12 02:48:11.000000 silverback-0.1.0b7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-12 02:48:11.000000 silverback-0.1.0b7/tests/test_cli.py
```

### Comparing `silverback-0.1.0b6/.github/ISSUE_TEMPLATE/bug.md` & `silverback-0.1.0b7/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/.github/ISSUE_TEMPLATE/feature.md` & `silverback-0.1.0b7/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/.github/ISSUE_TEMPLATE/work-item.md` & `silverback-0.1.0b7/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/.github/release-drafter.yml` & `silverback-0.1.0b7/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/.github/workflows/codeql.yaml` & `silverback-0.1.0b7/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/.github/workflows/commitlint.yaml` & `silverback-0.1.0b7/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/.github/workflows/prtitle.yaml` & `silverback-0.1.0b7/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/.github/workflows/publish.yaml` & `silverback-0.1.0b7/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/.github/workflows/test.yaml` & `silverback-0.1.0b7/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/.gitignore` & `silverback-0.1.0b7/.gitignore`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/.pre-commit-config.yaml` & `silverback-0.1.0b7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/CONTRIBUTING.md` & `silverback-0.1.0b7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/LICENSE` & `silverback-0.1.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/PKG-INFO` & `silverback-0.1.0b7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.1.0b6
+Version: 0.1.0b7
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/SilverBackLtd/sdk
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
         
@@ -43,16 +43,15 @@
         ```sh
         $ silverback run "example:app" --network :mainnet:alchemy
         ```
         
         ## Docker Usage
         
         ```sh
-        $ docker build -t silverback .
-        $ docker run --volume $PWD:/home/harambe/project silverback run "example:app" --network :mainnet:alchemy
+        $ docker run --volume $PWD:/home/harambe/project --volume ~/.tokenlists:/home/harambe/.tokenlists apeworx/silverback:latest run "example:app" --network :mainnet:alchemy
         ```
         
         ## Development
         
         This project is in development and should be considered a beta.
         Things might not be in their final state and breaking changes may occur.
         Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `silverback-0.1.0b6/README.md` & `silverback-0.1.0b7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -35,16 +35,15 @@
 ```sh
 $ silverback run "example:app" --network :mainnet:alchemy
 ```
 
 ## Docker Usage
 
 ```sh
-$ docker build -t silverback .
-$ docker run --volume $PWD:/home/harambe/project silverback run "example:app" --network :mainnet:alchemy
+$ docker run --volume $PWD:/home/harambe/project --volume ~/.tokenlists:/home/harambe/.tokenlists apeworx/silverback:latest run "example:app" --network :mainnet:alchemy
 ```
 
 ## Development
 
 This project is in development and should be considered a beta.
 Things might not be in their final state and breaking changes may occur.
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `silverback-0.1.0b6/example.py` & `silverback-0.1.0b7/example.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 # This is how we trigger off of new blocks
 @app.on_(chain.blocks)
 def exec_block(block: BlockAPI):
     return len(block.transactions)
 
 
 # This is how we trigger off of events
-@app.on_(USDC.Transfer)
+# Set new_block_timeout to adjust the expected block time.
+@app.on_(USDC.Transfer, new_block_timeout=25)
 # NOTE: Typing isn't required
 def exec_event1(log):
     if log.log_index % 7 == 3:
         # If you ever want the app to shutdown under some scenario, call this exception
         raise CircuitBreaker("Oopsie!")
     return log.amount
```

### Comparing `silverback-0.1.0b6/pyproject.toml` & `silverback-0.1.0b7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/setup.py` & `silverback-0.1.0b7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/SilverBackLtd/sdk",
     include_package_data=True,
     install_requires=[
         "eth-ape>=0.6.11,<1.0",
         "taskiq[metrics]>=0.6.0,<0.7.0",
+        # Can loosen constraint once https://github.com/pallets/click/issues/2558 resolved
+        "click==8.1.3",
     ],
     entry_points={
         "console_scripts": ["silverback=silverback._cli:cli"],
     },
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["silverback"],
```

### Comparing `silverback-0.1.0b6/silverback/_cli.py` & `silverback-0.1.0b7/silverback/_cli.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/silverback/_importer.py` & `silverback-0.1.0b7/silverback/_importer.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/silverback/exceptions.py` & `silverback-0.1.0b7/silverback/exceptions.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/silverback/middlewares.py` & `silverback-0.1.0b7/silverback/middlewares.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
         message.args = [(fix_dict(arg) if isinstance(arg, dict) else arg) for arg in message.args]
 
         return message
 
     def _create_label(self, message: TaskiqMessage) -> str:
         if message.task_name == "block":
-            args = f"[block={message.args[0].hash}]"
+            args = f"[block={message.args[0].hash.hex()}]"
 
         elif "event" in message.task_name:
             args = f"[txn={message.args[0].transaction_hash},log_index={message.args[0].log_index}]"
 
         else:
             args = ""
```

### Comparing `silverback-0.1.0b6/silverback/settings.py` & `silverback-0.1.0b7/silverback/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
     RESULT_BACKEND_CLASS: str = ""
     RESULT_BACKEND_URI: str = ""
 
     NETWORK_CHOICE: str = ""
     SIGNER_ALIAS: str = ""
 
+    NEW_BLOCK_TIMEOUT: Optional[int] = None
+
     class Config:
         env_prefix = "SILVERBACK_"
         case_sensitive = True
 
     def get_broker(self) -> AsyncBroker:
         broker_class = import_from_string(self.BROKER_CLASS)
         if broker_class == InMemoryBroker:
```

### Comparing `silverback-0.1.0b6/silverback/utils.py` & `silverback-0.1.0b7/silverback/utils.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b6/silverback.egg-info/PKG-INFO` & `silverback-0.1.0b7/silverback.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.1.0b6
+Version: 0.1.0b7
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/SilverBackLtd/sdk
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
         
@@ -43,16 +43,15 @@
         ```sh
         $ silverback run "example:app" --network :mainnet:alchemy
         ```
         
         ## Docker Usage
         
         ```sh
-        $ docker build -t silverback .
-        $ docker run --volume $PWD:/home/harambe/project silverback run "example:app" --network :mainnet:alchemy
+        $ docker run --volume $PWD:/home/harambe/project --volume ~/.tokenlists:/home/harambe/.tokenlists apeworx/silverback:latest run "example:app" --network :mainnet:alchemy
         ```
         
         ## Development
         
         This project is in development and should be considered a beta.
         Things might not be in their final state and breaking changes may occur.
         Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `silverback-0.1.0b6/silverback.egg-info/SOURCES.txt` & `silverback-0.1.0b7/silverback.egg-info/SOURCES.txt`

 * *Files identical despite different names*


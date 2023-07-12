# Comparing `tmp/stac-asset-0.0.4.tar.gz` & `tmp/stac-asset-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-asset-0.0.4.tar", last modified: Fri Jun  9 18:32:33 2023, max compression
+gzip compressed data, was "stac-asset-0.1.0.tar", last modified: Wed Jul 12 18:18:22 2023, max compression
```

## Comparing `stac-asset-0.0.4.tar` & `stac-asset-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:32:33.380683 stac-asset-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 18:32:23.000000 stac-asset-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-09 18:32:33.380683 stac-asset-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-06-09 18:32:23.000000 stac-asset-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-09 18:32:23.000000 stac-asset-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 18:32:33.380683 stac-asset-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:32:33.376683 stac-asset-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:32:33.380683 stac-asset-0.0.4/src/stac_asset/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/earthdata_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/filesystem_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/planetary_computer_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/s3_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-09 18:32:23.000000 stac-asset-0.0.4/src/stac_asset/usgs_eros_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:32:33.380683 stac-asset-0.0.4/src/stac_asset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-09 18:32:33.000000 stac-asset-0.0.4/src/stac_asset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-09 18:32:33.000000 stac-asset-0.0.4/src/stac_asset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:32:33.000000 stac-asset-0.0.4/src/stac_asset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 18:32:33.000000 stac-asset-0.0.4/src/stac_asset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-09 18:32:33.000000 stac-asset-0.0.4/src/stac_asset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 18:32:33.000000 stac-asset-0.0.4/src/stac_asset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:32:33.380683 stac-asset-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-09 18:32:23.000000 stac-asset-0.0.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-09 18:32:23.000000 stac-asset-0.0.4/tests/test_earthdata_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-09 18:32:23.000000 stac-asset-0.0.4/tests/test_filesystem_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-09 18:32:23.000000 stac-asset-0.0.4/tests/test_planetary_computer_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-09 18:32:23.000000 stac-asset-0.0.4/tests/test_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-09 18:32:23.000000 stac-asset-0.0.4/tests/test_usgs_eros_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:18:22.610945 stac-asset-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 18:18:06.000000 stac-asset-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-12 18:18:22.610945 stac-asset-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-12 18:18:06.000000 stac-asset-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-12 18:18:06.000000 stac-asset-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:18:22.610945 stac-asset-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:18:22.598945 stac-asset-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:18:22.602945 stac-asset-0.1.0/src/stac_asset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/usgs_eros_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:18:22.606945 stac-asset-0.1.0/src/stac_asset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-12 18:18:22.000000 stac-asset-0.1.0/src/stac_asset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-12 18:18:22.000000 stac-asset-0.1.0/src/stac_asset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:18:22.000000 stac-asset-0.1.0/src/stac_asset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 18:18:22.000000 stac-asset-0.1.0/src/stac_asset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-12 18:18:22.000000 stac-asset-0.1.0/src/stac_asset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 18:18:22.000000 stac-asset-0.1.0/src/stac_asset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:18:22.610945 stac-asset-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-12 18:18:06.000000 stac-asset-0.1.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-12 18:18:06.000000 stac-asset-0.1.0/tests/test_earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-12 18:18:06.000000 stac-asset-0.1.0/tests/test_filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-12 18:18:06.000000 stac-asset-0.1.0/tests/test_planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-12 18:18:06.000000 stac-asset-0.1.0/tests/test_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-12 18:18:06.000000 stac-asset-0.1.0/tests/test_usgs_eros_client.py
```

### Comparing `stac-asset-0.0.4/LICENSE` & `stac-asset-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/PKG-INFO` & `stac-asset-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.0.4
+Version: 0.1.0
 Summary: Read and download STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
-Project-URL: repository, https://github.com/gadomski/stac-asset
-Project-URL: changelog, https://github.com/gadomski/stac-asset/blob/main/CHANGELOG.md
+Project-URL: repository, https://github.com/stac-utils/stac-asset
+Project-URL: changelog, https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md
 Keywords: stac,async
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cli
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # stac-asset
 
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/gadomski/stac-asset/ci.yaml?style=for-the-badge)](https://github.com/gadomski/stac-asset/actions/workflows/ci.yaml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/stac-utils/stac-asset/ci.yaml?style=for-the-badge)](https://github.com/stac-utils/stac-asset/actions/workflows/ci.yaml)
 [![Read the Docs](https://img.shields.io/readthedocs/stac-asset?style=for-the-badge)](https://stac-asset.readthedocs.io/en/stable/)
 [![PyPI](https://img.shields.io/pypi/v/stac-asset?style=for-the-badge)](https://pypi.org/project/stac-asset)
 
 Download STAC Assets using a variety of authentication schemes.
 
 ## Installation
 
@@ -124,59 +124,32 @@
 
 1. Create a new personal access token by going to <https://urs.earthdata.nasa.gov/profile> and then clicking "Generate Token" (you'll need to log in).
 2. Set an enviornment variable named `EARTHDATA_PAT` to your token.
 3. Use `EarthdataClient.default()` to create a new client.
 
 You can also provide your token directly to `EarthdataClient.login()`.
 
-## Design goals
-
-As determined during a meeting at the Element 84 offices (formerly Azavea offices) on 2023-05-24.
-
-- [x] `async`-first
-- [ ] Allow range requests
-- [x] Download functionality
-- [x] Update STAC items to point to new hrefs on download
-- [x] Allow byte-stream access
-- [ ] Protocols:
-  - [x] http
-  - [x] s3
-    - [x] requestor pays
-    - [ ] custom endpoint
-  - [x] custom authentication
-    - [x] Planetary Computer
-    - [x] USGS EROS
-    - [x]  NASA
-- [ ] Copy directly from source to destination ("skip local")
-- [ ] Add new assets to an item
-- [ ] Update an existing asset
-- [ ] Delete assets
-- [ ] Templated paths on download
-- [ ] (possible) Support the file extension's local path
-- [ ] Checksum validation and creation
-- [x] CLI
-
 ## Versioning
 
 This project does its best to adhere to [semantic versioning](https://semver.org/).
 Any module, class, constant, or function that does not begin with a `_` is considered part of our public API for versioning purposes.
 Our command-line interface (CLI) is NOT considered part of our public API, and may change in breaking ways at any time.
 If you need stability promises, use our API.
 
 ## Contributing
 
-Use Github [issues](https://github.com/gadomski/stac-asset/issues) to report bugs and request new features.
-Use Github [pull requests](https://github.com/gadomski/stac-asset/pulls) to fix bugs and propose new features.
+Use Github [issues](https://github.com/stac-utils/stac-asset/issues) to report bugs and request new features.
+Use Github [pull requests](https://github.com/stac-utils/stac-asset/pulls) to fix bugs and propose new features.
 
 ## Developing
 
 Clone, install with the dev dependencies, and install **pre-commit**:
 
 ```shell
-git clone git@github.com:gadomski/stac-asset.git
+git clone git@github.com:stac-utils/stac-asset.git
 cd stac-asset
 pip install '.[dev]'
 pre-commit install
 ```
 
 ### Testing
 
@@ -210,8 +183,8 @@
 ```shell
 pip install sphinx-autobuild
 sphinx-autobuild docs docs/_build/html
 ```
 
 ## License
 
-[Apache-2.0](https://github.com/gadomski/stac-asset/blob/main/LICENSE)
+[Apache-2.0](https://github.com/stac-utils/stac-asset/blob/main/LICENSE)
```

### Comparing `stac-asset-0.0.4/README.md` & `stac-asset-0.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # stac-asset
 
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/gadomski/stac-asset/ci.yaml?style=for-the-badge)](https://github.com/gadomski/stac-asset/actions/workflows/ci.yaml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/stac-utils/stac-asset/ci.yaml?style=for-the-badge)](https://github.com/stac-utils/stac-asset/actions/workflows/ci.yaml)
 [![Read the Docs](https://img.shields.io/readthedocs/stac-asset?style=for-the-badge)](https://stac-asset.readthedocs.io/en/stable/)
 [![PyPI](https://img.shields.io/pypi/v/stac-asset?style=for-the-badge)](https://pypi.org/project/stac-asset)
 
 Download STAC Assets using a variety of authentication schemes.
 
 ## Installation
 
@@ -101,59 +101,32 @@
 
 1. Create a new personal access token by going to <https://urs.earthdata.nasa.gov/profile> and then clicking "Generate Token" (you'll need to log in).
 2. Set an enviornment variable named `EARTHDATA_PAT` to your token.
 3. Use `EarthdataClient.default()` to create a new client.
 
 You can also provide your token directly to `EarthdataClient.login()`.
 
-## Design goals
-
-As determined during a meeting at the Element 84 offices (formerly Azavea offices) on 2023-05-24.
-
-- [x] `async`-first
-- [ ] Allow range requests
-- [x] Download functionality
-- [x] Update STAC items to point to new hrefs on download
-- [x] Allow byte-stream access
-- [ ] Protocols:
-  - [x] http
-  - [x] s3
-    - [x] requestor pays
-    - [ ] custom endpoint
-  - [x] custom authentication
-    - [x] Planetary Computer
-    - [x] USGS EROS
-    - [x]  NASA
-- [ ] Copy directly from source to destination ("skip local")
-- [ ] Add new assets to an item
-- [ ] Update an existing asset
-- [ ] Delete assets
-- [ ] Templated paths on download
-- [ ] (possible) Support the file extension's local path
-- [ ] Checksum validation and creation
-- [x] CLI
-
 ## Versioning
 
 This project does its best to adhere to [semantic versioning](https://semver.org/).
 Any module, class, constant, or function that does not begin with a `_` is considered part of our public API for versioning purposes.
 Our command-line interface (CLI) is NOT considered part of our public API, and may change in breaking ways at any time.
 If you need stability promises, use our API.
 
 ## Contributing
 
-Use Github [issues](https://github.com/gadomski/stac-asset/issues) to report bugs and request new features.
-Use Github [pull requests](https://github.com/gadomski/stac-asset/pulls) to fix bugs and propose new features.
+Use Github [issues](https://github.com/stac-utils/stac-asset/issues) to report bugs and request new features.
+Use Github [pull requests](https://github.com/stac-utils/stac-asset/pulls) to fix bugs and propose new features.
 
 ## Developing
 
 Clone, install with the dev dependencies, and install **pre-commit**:
 
 ```shell
-git clone git@github.com:gadomski/stac-asset.git
+git clone git@github.com:stac-utils/stac-asset.git
 cd stac-asset
 pip install '.[dev]'
 pre-commit install
 ```
 
 ### Testing
 
@@ -187,8 +160,8 @@
 ```shell
 pip install sphinx-autobuild
 sphinx-autobuild docs docs/_build/html
 ```
 
 ## License
 
-[Apache-2.0](https://github.com/gadomski/stac-asset/blob/main/LICENSE)
+[Apache-2.0](https://github.com/stac-utils/stac-asset/blob/main/LICENSE)
```

### Comparing `stac-asset-0.0.4/pyproject.toml` & `stac-asset-0.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "stac-asset"
-version = "0.0.4"
+version = "0.1.0"
 description = "Read and download STAC assets across platforms and providers"
 authors = [
     { name = "Pete Gadomski", email = "pete.gadomski@gmail.com" }
 ]
 readme = "README.md"
 keywords = ["stac", "async"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
 ]
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 dependencies = [
     "aiofiles>=23.1.0",
     "aiobotocore>=2.5.0",
     "aiohttp>=3.8.4",
@@ -33,28 +33,28 @@
 dev = [
     "black~=23.3",
     "mypy~=1.3",
     "pre-commit~=3.3",
     "pytest~=7.3",
     "pytest-asyncio~=0.21",
     "pytest-cov~=4.1",
-    "ruff==0.0.270",
+    "ruff==0.0.278",
     "types-aiofiles~=23.1",
 ]
 docs = [
     "pydata-sphinx-theme~=0.13",
     "sphinx~=7.0",
 ]
 
 [project.scripts]
 stac-asset = "stac_asset._cli:cli"
 
 [project.urls]
-repository = "https://github.com/gadomski/stac-asset"
-changelog = "https://github.com/gadomski/stac-asset/blob/main/CHANGELOG.md"
+repository = "https://github.com/stac-utils/stac-asset"
+changelog = "https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md"
 
 [tool.mypy]
 strict = true
 
 [tool.ruff]
 select = ["F", "E", "W", "I", "ERA", "RUF", "D"]
 ignore = ["D100", "D105", "D107"]
```

### Comparing `stac-asset-0.0.4/src/stac_asset/__init__.py` & `stac-asset-0.1.0/src/stac_asset/__init__.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/src/stac_asset/_cli.py` & `stac-asset-0.1.0/src/stac_asset/_cli.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/src/stac_asset/client.py` & `stac-asset-0.1.0/src/stac_asset/client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/src/stac_asset/earthdata_client.py` & `stac-asset-0.1.0/src/stac_asset/earthdata_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/src/stac_asset/errors.py` & `stac-asset-0.1.0/src/stac_asset/errors.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/src/stac_asset/filesystem_client.py` & `stac-asset-0.1.0/src/stac_asset/filesystem_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/src/stac_asset/functions.py` & `stac-asset-0.1.0/src/stac_asset/functions.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/src/stac_asset/http_client.py` & `stac-asset-0.1.0/src/stac_asset/http_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/src/stac_asset/planetary_computer_client.py` & `stac-asset-0.1.0/src/stac_asset/planetary_computer_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/src/stac_asset/s3_client.py` & `stac-asset-0.1.0/src/stac_asset/s3_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/src/stac_asset/types.py` & `stac-asset-0.1.0/src/stac_asset/types.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/src/stac_asset/usgs_eros_client.py` & `stac-asset-0.1.0/src/stac_asset/usgs_eros_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/src/stac_asset.egg-info/PKG-INFO` & `stac-asset-0.1.0/src/stac_asset.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.0.4
+Version: 0.1.0
 Summary: Read and download STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
-Project-URL: repository, https://github.com/gadomski/stac-asset
-Project-URL: changelog, https://github.com/gadomski/stac-asset/blob/main/CHANGELOG.md
+Project-URL: repository, https://github.com/stac-utils/stac-asset
+Project-URL: changelog, https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md
 Keywords: stac,async
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cli
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # stac-asset
 
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/gadomski/stac-asset/ci.yaml?style=for-the-badge)](https://github.com/gadomski/stac-asset/actions/workflows/ci.yaml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/stac-utils/stac-asset/ci.yaml?style=for-the-badge)](https://github.com/stac-utils/stac-asset/actions/workflows/ci.yaml)
 [![Read the Docs](https://img.shields.io/readthedocs/stac-asset?style=for-the-badge)](https://stac-asset.readthedocs.io/en/stable/)
 [![PyPI](https://img.shields.io/pypi/v/stac-asset?style=for-the-badge)](https://pypi.org/project/stac-asset)
 
 Download STAC Assets using a variety of authentication schemes.
 
 ## Installation
 
@@ -124,59 +124,32 @@
 
 1. Create a new personal access token by going to <https://urs.earthdata.nasa.gov/profile> and then clicking "Generate Token" (you'll need to log in).
 2. Set an enviornment variable named `EARTHDATA_PAT` to your token.
 3. Use `EarthdataClient.default()` to create a new client.
 
 You can also provide your token directly to `EarthdataClient.login()`.
 
-## Design goals
-
-As determined during a meeting at the Element 84 offices (formerly Azavea offices) on 2023-05-24.
-
-- [x] `async`-first
-- [ ] Allow range requests
-- [x] Download functionality
-- [x] Update STAC items to point to new hrefs on download
-- [x] Allow byte-stream access
-- [ ] Protocols:
-  - [x] http
-  - [x] s3
-    - [x] requestor pays
-    - [ ] custom endpoint
-  - [x] custom authentication
-    - [x] Planetary Computer
-    - [x] USGS EROS
-    - [x]  NASA
-- [ ] Copy directly from source to destination ("skip local")
-- [ ] Add new assets to an item
-- [ ] Update an existing asset
-- [ ] Delete assets
-- [ ] Templated paths on download
-- [ ] (possible) Support the file extension's local path
-- [ ] Checksum validation and creation
-- [x] CLI
-
 ## Versioning
 
 This project does its best to adhere to [semantic versioning](https://semver.org/).
 Any module, class, constant, or function that does not begin with a `_` is considered part of our public API for versioning purposes.
 Our command-line interface (CLI) is NOT considered part of our public API, and may change in breaking ways at any time.
 If you need stability promises, use our API.
 
 ## Contributing
 
-Use Github [issues](https://github.com/gadomski/stac-asset/issues) to report bugs and request new features.
-Use Github [pull requests](https://github.com/gadomski/stac-asset/pulls) to fix bugs and propose new features.
+Use Github [issues](https://github.com/stac-utils/stac-asset/issues) to report bugs and request new features.
+Use Github [pull requests](https://github.com/stac-utils/stac-asset/pulls) to fix bugs and propose new features.
 
 ## Developing
 
 Clone, install with the dev dependencies, and install **pre-commit**:
 
 ```shell
-git clone git@github.com:gadomski/stac-asset.git
+git clone git@github.com:stac-utils/stac-asset.git
 cd stac-asset
 pip install '.[dev]'
 pre-commit install
 ```
 
 ### Testing
 
@@ -210,8 +183,8 @@
 ```shell
 pip install sphinx-autobuild
 sphinx-autobuild docs docs/_build/html
 ```
 
 ## License
 
-[Apache-2.0](https://github.com/gadomski/stac-asset/blob/main/LICENSE)
+[Apache-2.0](https://github.com/stac-utils/stac-asset/blob/main/LICENSE)
```

### Comparing `stac-asset-0.0.4/src/stac_asset.egg-info/SOURCES.txt` & `stac-asset-0.1.0/src/stac_asset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/tests/test_cli.py` & `stac-asset-0.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/tests/test_earthdata_client.py` & `stac-asset-0.1.0/tests/test_earthdata_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/tests/test_filesystem_client.py` & `stac-asset-0.1.0/tests/test_filesystem_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/tests/test_planetary_computer_client.py` & `stac-asset-0.1.0/tests/test_planetary_computer_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/tests/test_s3_client.py` & `stac-asset-0.1.0/tests/test_s3_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.0.4/tests/test_usgs_eros_client.py` & `stac-asset-0.1.0/tests/test_usgs_eros_client.py`

 * *Files identical despite different names*


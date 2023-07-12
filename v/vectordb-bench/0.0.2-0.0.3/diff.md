# Comparing `tmp/vectordb-bench-0.0.2.tar.gz` & `tmp/vectordb-bench-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectordb-bench-0.0.2.tar", last modified: Wed Jun 21 12:43:37 2023, max compression
+gzip compressed data, was "vectordb-bench-0.0.3.tar", last modified: Wed Jul 12 12:32:52 2023, max compression
```

## Comparing `vectordb-bench-0.0.2.tar` & `vectordb-bench-0.0.3.tar`

### file list

```diff
@@ -1,102 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.906935 vectordb-bench-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.874934 vectordb-bench-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.886934 vectordb-bench-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/.github/workflows/publish_package_on_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/.ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-21 12:43:37.906935 vectordb-bench-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 12:43:37.906935 vectordb-bench-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.890935 vectordb-bench-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/test_bench_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/test_elasticsearch_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/ut_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.894935 vectordb-bench-0.0.2/vectordb_bench/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.898934 vectordb-bench-0.0.2/vectordb_bench/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/assembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.898934 vectordb-bench-0.0.2/vectordb_bench/backend/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.898934 vectordb-bench-0.0.2/vectordb_bench/backend/clients/elastic_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/elastic_cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/elastic_cloud/elastic_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.898934 vectordb-bench-0.0.2/vectordb_bench/backend/clients/milvus/
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/milvus/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/milvus/milvus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.898934 vectordb-bench-0.0.2/vectordb_bench/backend/clients/pinecone/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/pinecone/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/pinecone/pinecone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.898934 vectordb-bench-0.0.2/vectordb_bench/backend/clients/qdrant_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/qdrant_cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/qdrant_cloud/qdrant_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.898934 vectordb-bench-0.0.2/vectordb_bench/backend/clients/weaviate_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/weaviate_cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/weaviate_cloud/weaviate_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.902935 vectordb-bench-0.0.2/vectordb_bench/backend/clients/zilliz_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/zilliz_cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/zilliz_cloud/zilliz_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/result_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.902935 vectordb-bench-0.0.2/vectordb_bench/backend/runner/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/runner/mp_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/runner/serial_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/task_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.902935 vectordb-bench-0.0.2/vectordb_bench/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.882934 vectordb-bench-0.0.2/vectordb_bench/frontend/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.902935 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/charts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/expanderStyle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/footer.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/headerIcon.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/priceTable.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/stPageConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.902935 vectordb-bench-0.0.2/vectordb_bench/frontend/components/get_results/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/get_results/saveAsImage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.906935 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/autoRefresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/caseSelector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/dbConfigSetting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/dbSelector.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/generateTasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/hideSidebar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/submitTask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.906935 vectordb-bench-0.0.2/vectordb_bench/frontend/const/
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/const/dbCaseConfigs.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/const/dbPrices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/const/styles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.906935 vectordb-bench-0.0.2/vectordb_bench/frontend/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/pages/quries_per_dollar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/pages/run_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/vdb_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/log_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.906935 vectordb-bench-0.0.2/vectordb_bench/results/
--rw-r--r--   0 runner    (1001) docker     (123)    86206 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/results/result_20230609_standard.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.894935 vectordb-bench-0.0.2/vectordb_bench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-21 12:43:37.000000 vectordb-bench-0.0.2/vectordb_bench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-21 12:43:37.000000 vectordb-bench-0.0.2/vectordb_bench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:43:37.000000 vectordb-bench-0.0.2/vectordb_bench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-21 12:43:37.000000 vectordb-bench-0.0.2/vectordb_bench.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-21 12:43:37.000000 vectordb-bench-0.0.2/vectordb_bench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 12:43:37.000000 vectordb-bench-0.0.2/vectordb_bench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.163529 vectordb-bench-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.135527 vectordb-bench-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.143528 vectordb-bench-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/.github/workflows/publish_package_on_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18290 2023-07-12 12:32:52.163529 vectordb-bench-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:32:52.163529 vectordb-bench-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.143528 vectordb-bench-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/tests/test_bench_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/tests/test_elasticsearch_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/tests/ut_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.147528 vectordb-bench-0.0.3/vectordb_bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.151528 vectordb-bench-0.0.3/vectordb_bench/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/assembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.151528 vectordb-bench-0.0.3/vectordb_bench/backend/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.151528 vectordb-bench-0.0.3/vectordb_bench/backend/clients/elastic_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/elastic_cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/elastic_cloud/elastic_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.151528 vectordb-bench-0.0.3/vectordb_bench/backend/clients/milvus/
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/milvus/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/milvus/milvus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.151528 vectordb-bench-0.0.3/vectordb_bench/backend/clients/pgvector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/pgvector/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/pgvector/pgvector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.151528 vectordb-bench-0.0.3/vectordb_bench/backend/clients/pinecone/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/pinecone/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/pinecone/pinecone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.155529 vectordb-bench-0.0.3/vectordb_bench/backend/clients/qdrant_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/qdrant_cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/qdrant_cloud/qdrant_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.155529 vectordb-bench-0.0.3/vectordb_bench/backend/clients/weaviate_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/weaviate_cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/weaviate_cloud/weaviate_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.155529 vectordb-bench-0.0.3/vectordb_bench/backend/clients/zilliz_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/zilliz_cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/clients/zilliz_cloud/zilliz_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/result_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.155529 vectordb-bench-0.0.3/vectordb_bench/backend/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/runner/mp_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/runner/serial_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/task_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/backend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.155529 vectordb-bench-0.0.3/vectordb_bench/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.139528 vectordb-bench-0.0.3/vectordb_bench/frontend/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.159529 vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/expanderStyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/headerIcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/priceTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/stPageConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.159529 vectordb-bench-0.0.3/vectordb_bench/frontend/components/get_results/
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/get_results/saveAsImage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.159529 vectordb-bench-0.0.3/vectordb_bench/frontend/components/run_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/run_test/autoRefresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/run_test/caseSelector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/run_test/dbConfigSetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/run_test/dbSelector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/run_test/generateTasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/run_test/hideSidebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/components/run_test/submitTask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.163529 vectordb-bench-0.0.3/vectordb_bench/frontend/const/
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/const/dbCaseConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/const/dbPrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/const/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.163529 vectordb-bench-0.0.3/vectordb_bench/frontend/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/pages/quries_per_dollar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/pages/run_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/frontend/vdb_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/log_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.163529 vectordb-bench-0.0.3/vectordb_bench/results/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/results/dbPrices.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/results/getLeaderboardData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26502 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/results/leaderboard.json
+-rw-r--r--   0 runner    (1001) docker     (123)    96237 2023-07-12 12:32:40.000000 vectordb-bench-0.0.3/vectordb_bench/results/result_20230705_standard.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:32:52.147528 vectordb-bench-0.0.3/vectordb_bench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18290 2023-07-12 12:32:52.000000 vectordb-bench-0.0.3/vectordb_bench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-12 12:32:52.000000 vectordb-bench-0.0.3/vectordb_bench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:32:52.000000 vectordb-bench-0.0.3/vectordb_bench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 12:32:52.000000 vectordb-bench-0.0.3/vectordb_bench.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-12 12:32:52.000000 vectordb-bench-0.0.3/vectordb_bench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-12 12:32:52.000000 vectordb-bench-0.0.3/vectordb_bench.egg-info/top_level.txt
```

### Comparing `vectordb-bench-0.0.2/.github/workflows/publish_package_on_release.yml` & `vectordb-bench-0.0.3/.github/workflows/publish_package_on_release.yml`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/.ruff.toml` & `vectordb-bench-0.0.3/.ruff.toml`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/LICENSE` & `vectordb-bench-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/PKG-INFO` & `vectordb-bench-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,13 @@
-Metadata-Version: 2.1
-Name: vectordb-bench
-Version: 0.0.2
-Summary: VectorDBBench is not just an offering of benchmark results for mainstream vector databases and cloud services, it's your go-to tool for the ultimate performance and cost-effectiveness comparison. Designed with ease-of-use in mind, VectorDBBench is devised to help users, even non-professionals, reproduce results or test new systems, making the hunt for the optimal choice amongst a plethora of cloud services and open-source vector databases a breeze.
-Author-email: XuanYang-cn <xuan.yang@zilliz.com>
-Project-URL: repository, https://github.com/zilliztech/VectorDBBench
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # VectorDBBench: A Benchmark Tool for VectorDB
 
 [![version](https://img.shields.io/pypi/v/vectordb-bench.svg?color=blue)](https://pypi.org/project/vectordb-bench/)
 [![Downloads](https://pepy.tech/badge/vectordb-bench)](https://pepy.tech/project/vectordb-bench)
 
+**Leaderboard:** https://zilliz.com/benchmark
 ## Quick Start
 ### Prerequirement
 ``` shell
 python >= 3.11
 ```
 ### Install
 ``` shell
@@ -37,14 +24,32 @@
 Understanding the importance of user experience, we provide an intuitive visual interface. This not only empowers users to initiate benchmarks at ease, but also to view comparative result reports, thereby reproducing benchmark results effortlessly.
 To add more relevance and practicality, we provide cost-effectiveness reports particularly for cloud services. This allows for a more realistic and applicable benchmarking process.
 
 Closely mimicking real-world production environments, we've set up diverse testing scenarios including insertion, searching, and filtered searching. To provide you with credible and reliable data, we've included public datasets from actual production scenarios, such as [SIFT](http://corpus-texmex.irisa.fr/), [GIST](http://corpus-texmex.irisa.fr/), [Cohere](https://huggingface.co/datasets/Cohere/wikipedia-22-12/tree/main/en), and more. It's fascinating to discover how a relatively unknown open-source database might excel in certain circumstances!
 
 Prepare to delve into the world of VectorDBBench, and let it guide you in uncovering your perfect vector database match.  
 
+## Leaderboard
+### Introduction
+To facilitate the presentation of test results and provide a comprehensive performance analysis report, we offer a [leaderboard page](https://zilliz.com/benchmark). It allows us to choose from QPS, QP$, and latency metrics, and provides a comprehensive assessment of a system's performance based on the test results of various cases and a set of scoring mechanisms (to be introduced later). On this leaderboard, we can select the systems and models to be compared, and filter out cases we do not want to consider. Comprehensive scores are always ranked from best to worst, and the specific test results of each query will be presented in the list below.
+
+### Scoring Rules
+
+1. For each case, select a base value and score each system based on relative values. 
+    - For QPS and QP$, we use the highest value as the reference, denoted as `base_QPS` or `base_QP$`, and the score of each system is `(QPS/base_QPS) * 100` or `(QP$/base_QP$) * 100`. 
+    - For Latency, we use the lowest value as the reference, that is, `base_Latency`, and the score of each system is `(Latency + 10ms)/(base_Latency + 10ms)`. 
+
+    We want to give equal weight to different cases, and not let a case with high absolute result values become the sole reason for the overall scoring. Therefore, when scoring different systems in each case, we need to use relative values. 
+
+    Also, for Latency, we add 10ms to the numerator and denominator to ensure that if every system performs particularly well in a case, its advantage will not be infinitely magnified when latency tends to 0.
+
+2. For systems that fail or timeout in a particular case, we will give them a score based on a value worse than the worst result by a factor of two. For example, in QPS or QP$, it would be half the lowest value. For Latency, it would be twice the maximum value.
+
+3. For each system, we will take the geometric mean of its scores in all cases as its comprehensive score for a particular metric.
+
 ## Build on your own
 ### Install requirements
 ``` shell
 pip install -e '.[test]'
 ```
 ### Run test server
 ```
@@ -65,18 +70,20 @@
 
 ```shell
 $ ruff check vectordb_bench --fix
 ```
 
 ## How does it work?
 ### Result Page
-![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/66ab83c4-656e-41a8-a643-d9790faccbeb)
+![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/7f5cdae7-f9f2-4a81-b2e0-e5c6268cd970)
 This is the main page of VectorDBBench, which displays the standard benchmark results we provide. Additionally, results of all tests performed by users themselves will also be shown here. We also offer the ability to select and compare results from multiple tests simultaneously.
 
 The standard benchmark results displayed here include all 9 cases that we currently support for all our clients (Milvus, Zilliz Cloud, Elastic Search, Qdrant Cloud, and Weaviate Cloud). However, as some systems may not be able to complete all the tests successfully due to issues like Out of Memory (OOM) or timeouts, not all clients are included in every case.
+
+All standard benchmark results are generated by a client running on an 8 core, 32 GB host, which is located in the same region as the server being tested. The client host is equipped with an `Intel(R) Xeon(R) Platinum 8375C CPU @ 2.90GHz` processor. Also all the servers for the open-source systems tested in our benchmarks run on hosts with the same type of processor.
 ### Run Test Page
 ![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/a789099a-3707-4214-8052-b73463b8f2c6)
 This is the page to run a test:
 1. Initially, you select the systems to be tested - multiple selections are allowed. Once selected, corresponding forms will pop up to gather necessary information for using the chosen databases. The db_label is used to differentiate different instances of the same system. We recommend filling in the host size or instance type here (as we do in our standard results).
 2. The next step is to select the test cases you want to perform. You can select multiple cases at once, and a form to collect corresponding parameters will appear.
 3. Finally, you'll need to provide a task label to distinguish different test results. Using the same label for different tests will result in the previous results being overwritten.
 Now we can only run one task at the same time. 
@@ -98,25 +105,25 @@
 #### Filtering Search Performance Case
 - **Large Dataset, Low Filtering Rate:** Evaluates search performance with a large dataset (Cohere 10M vectors, 768 dimensions) under a low filtering rate (1% vectors) at different parallel levels.
 - **Medium Dataset, Low Filtering Rate:** This case uses a medium dataset (Cohere 1M vectors, 768 dimensions) with a similar low filtering rate.
 - **Large Dataset, High Filtering Rate:** It tests with a large dataset (Cohere 10M vectors, 768 dimensions) but under a high filtering rate (99% vectors).
 - **Medium Dataset, High Filtering Rate:** This case uses a medium dataset (Cohere 1M vectors, 768 dimensions) with a high filtering rate.
 For a quick reference, here is a table summarizing the key aspects of each case:
 
-Case No. | Case Type | Dataset Size | Dataset Type | Filtering Rate | Results |
-|----------|-----------|--------------|--------------|----------------|---------|
-1 | Capacity Case | Large Dim | GIST 100K vectors, 960 dimensions | N/A | Number of inserted vectors |
-2 | Capacity Case | Small Dim | SIFT 100K vectors, 128 dimensions | N/A | Number of inserted vectors |
-3 | Search Performance Case | XLarge Dataset | LAION 100M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
-4 | Search Performance Case | Large Dataset | Cohere 10M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
-5 | Search Performance Case | Medium Dataset | Cohere 1M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
-6 | Filtering Search Performance Case | Large Dataset, Low Filtering Rate | Cohere 10M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
-7 | Filtering Search Performance Case | Medium Dataset, Low Filtering Rate | Cohere 1M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
-8 | Filtering Search Performance Case | Large Dataset, High Filtering Rate | Cohere 10M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
-9 | Filtering Search Performance Case | Medium Dataset, High Filtering Rate | Cohere 1M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
+Case No. | Case Type | Dataset Size  | Filtering Rate | Results |
+|----------|-----------|--------------|----------------|---------|
+1 | Capacity Case | GIST 100K vectors, 960 dimensions | N/A | Number of inserted vectors |
+2 | Capacity Case | SIFT 100K vectors, 128 dimensions | N/A | Number of inserted vectors |
+3 | Search Performance Case | LAION 100M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
+4 | Search Performance Case | Cohere 10M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
+5 | Search Performance Case | Cohere 1M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
+6 | Filtering Search Performance Case | Cohere 10M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
+7 | Filtering Search Performance Case | Cohere 1M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
+8 | Filtering Search Performance Case | Cohere 10M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
+9 | Filtering Search Performance Case | Cohere 1M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
 
 Each case provides an in-depth examination of a vector database's abilities, providing you a comprehensive view of the database's performance.
 
 ## Goals
 Our goals of this benchmark are:
 ### Reproducibility & Usability
 One of the primary goals of VectorDBBench is to enable users to reproduce benchmark results swiftly and easily, or to test their customized scenarios. We believe that lowering the barriers to entry for conducting these tests will enhance the community's understanding and improvement of vector databases. We aim to create an environment where any user, regardless of their technical expertise, can quickly set up and run benchmarks, and view and analyze results in an intuitive manner.
@@ -196,7 +203,68 @@
 ### Fine-Tuning
 For the system under test, we use the default server-side configuration to maintain the authenticity and representativeness of our results.
 For the Client, we welcome any parameter tuning to obtain better results.
 ### Incomplete Results
 Many databases may not be able to complete all test cases due to issues such as Out of Memory (OOM), crashes, or timeouts. In these scenarios, we will clearly state these occurrences in the test results.
 ### Mistake Or Misrepresentation 
 We strive for accuracy in learning and supporting various vector databases, yet there might be oversights or misapplications. For any such occurrences, feel free to [raise an issue](https://github.com/zilliztech/VectorDBBench/issues/new) or make amendments on our GitHub page.
+## Timeout
+In our pursuit to ensure that our benchmark reflects the reality of a production environment while guaranteeing the practicality of the system, we have implemented a timeout plan based on our experiences for various tests.
+
+**1. Capacity Case:**
+- For Capacity Case, we have assigned an overall timeout.
+
+**2. Other Cases:**
+
+For other cases, we have set two timeouts:
+
+- **Data Loading Timeout:** This timeout is designed to filter out systems that are too slow in inserting data, thus ensuring that we are only considering systems that is able to cope with the demands of a real-world production environment within a reasonable time frame.
+
+- **Optimization Preparation Timeout**: This timeout is established to avoid excessive optimization strategies that might work for benchmarks but fail to deliver in real production environments. By doing this, we ensure that the systems we consider are not only suitable for testing environments but also applicable and efficient in production scenarios.
+
+This multi-tiered timeout approach allows our benchmark to be more representative of actual production environments and assists us in identifying systems that can truly perform in real-world scenarios.
+<table>
+    <tr>
+        <th>Case</th>
+        <th>Data Size</th>
+        <th>Timeout Type</th>
+        <th>Value</th>
+    </tr>
+    <tr>
+        <td>Capacity Case</td>
+        <td>N/A</td>
+        <td>Loading timeout</td>
+        <td>24 hours</td>
+    </tr>
+    <tr>
+        <td rowspan="2">Other Cases</td>
+        <td rowspan="2">1M vectors, 768 dimensions</td>
+        <td>Loading timeout</td>
+        <td>2.5 hours</td>
+    </tr>
+    <tr>
+        <td>Optimization timeout</td>
+        <td>15 mins</td>
+    </tr>
+    <tr>
+        <td rowspan="2">Other Cases</td>
+        <td rowspan="2">10M vectors, 768 dimensions</td>
+        <td>Loading timeout</td>
+        <td>25 hours</td>
+    </tr>
+    <tr>
+        <td>Optimization timeout</td>
+        <td>2.5 hours</td>
+    </tr>
+    <tr>
+        <td rowspan="2">Other Cases</td>
+        <td rowspan="2">100M vectors, 768 dimensions</td>
+        <td>Loading timeout</td>
+        <td>250 hours</td>
+    </tr>
+    <tr>
+        <td>Optimization timeout</td>
+        <td>25 hours</td>
+    </tr>
+</table>
+
+**Note:** Some datapoints in the standard benchmark results that voilate this timeout will be kept for now for reference. We will remove them in the future.
```

### Comparing `vectordb-bench-0.0.2/README.md` & `vectordb-bench-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,27 @@
+Metadata-Version: 2.1
+Name: vectordb-bench
+Version: 0.0.3
+Summary: VectorDBBench is not just an offering of benchmark results for mainstream vector databases and cloud services, it's your go-to tool for the ultimate performance and cost-effectiveness comparison. Designed with ease-of-use in mind, VectorDBBench is devised to help users, even non-professionals, reproduce results or test new systems, making the hunt for the optimal choice amongst a plethora of cloud services and open-source vector databases a breeze.
+Author-email: XuanYang-cn <xuan.yang@zilliz.com>
+Project-URL: repository, https://github.com/zilliztech/VectorDBBench
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # VectorDBBench: A Benchmark Tool for VectorDB
 
 [![version](https://img.shields.io/pypi/v/vectordb-bench.svg?color=blue)](https://pypi.org/project/vectordb-bench/)
 [![Downloads](https://pepy.tech/badge/vectordb-bench)](https://pepy.tech/project/vectordb-bench)
 
+**Leaderboard:** https://zilliz.com/benchmark
 ## Quick Start
 ### Prerequirement
 ``` shell
 python >= 3.11
 ```
 ### Install
 ``` shell
@@ -23,14 +38,32 @@
 Understanding the importance of user experience, we provide an intuitive visual interface. This not only empowers users to initiate benchmarks at ease, but also to view comparative result reports, thereby reproducing benchmark results effortlessly.
 To add more relevance and practicality, we provide cost-effectiveness reports particularly for cloud services. This allows for a more realistic and applicable benchmarking process.
 
 Closely mimicking real-world production environments, we've set up diverse testing scenarios including insertion, searching, and filtered searching. To provide you with credible and reliable data, we've included public datasets from actual production scenarios, such as [SIFT](http://corpus-texmex.irisa.fr/), [GIST](http://corpus-texmex.irisa.fr/), [Cohere](https://huggingface.co/datasets/Cohere/wikipedia-22-12/tree/main/en), and more. It's fascinating to discover how a relatively unknown open-source database might excel in certain circumstances!
 
 Prepare to delve into the world of VectorDBBench, and let it guide you in uncovering your perfect vector database match.  
 
+## Leaderboard
+### Introduction
+To facilitate the presentation of test results and provide a comprehensive performance analysis report, we offer a [leaderboard page](https://zilliz.com/benchmark). It allows us to choose from QPS, QP$, and latency metrics, and provides a comprehensive assessment of a system's performance based on the test results of various cases and a set of scoring mechanisms (to be introduced later). On this leaderboard, we can select the systems and models to be compared, and filter out cases we do not want to consider. Comprehensive scores are always ranked from best to worst, and the specific test results of each query will be presented in the list below.
+
+### Scoring Rules
+
+1. For each case, select a base value and score each system based on relative values. 
+    - For QPS and QP$, we use the highest value as the reference, denoted as `base_QPS` or `base_QP$`, and the score of each system is `(QPS/base_QPS) * 100` or `(QP$/base_QP$) * 100`. 
+    - For Latency, we use the lowest value as the reference, that is, `base_Latency`, and the score of each system is `(Latency + 10ms)/(base_Latency + 10ms)`. 
+
+    We want to give equal weight to different cases, and not let a case with high absolute result values become the sole reason for the overall scoring. Therefore, when scoring different systems in each case, we need to use relative values. 
+
+    Also, for Latency, we add 10ms to the numerator and denominator to ensure that if every system performs particularly well in a case, its advantage will not be infinitely magnified when latency tends to 0.
+
+2. For systems that fail or timeout in a particular case, we will give them a score based on a value worse than the worst result by a factor of two. For example, in QPS or QP$, it would be half the lowest value. For Latency, it would be twice the maximum value.
+
+3. For each system, we will take the geometric mean of its scores in all cases as its comprehensive score for a particular metric.
+
 ## Build on your own
 ### Install requirements
 ``` shell
 pip install -e '.[test]'
 ```
 ### Run test server
 ```
@@ -51,18 +84,20 @@
 
 ```shell
 $ ruff check vectordb_bench --fix
 ```
 
 ## How does it work?
 ### Result Page
-![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/66ab83c4-656e-41a8-a643-d9790faccbeb)
+![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/7f5cdae7-f9f2-4a81-b2e0-e5c6268cd970)
 This is the main page of VectorDBBench, which displays the standard benchmark results we provide. Additionally, results of all tests performed by users themselves will also be shown here. We also offer the ability to select and compare results from multiple tests simultaneously.
 
 The standard benchmark results displayed here include all 9 cases that we currently support for all our clients (Milvus, Zilliz Cloud, Elastic Search, Qdrant Cloud, and Weaviate Cloud). However, as some systems may not be able to complete all the tests successfully due to issues like Out of Memory (OOM) or timeouts, not all clients are included in every case.
+
+All standard benchmark results are generated by a client running on an 8 core, 32 GB host, which is located in the same region as the server being tested. The client host is equipped with an `Intel(R) Xeon(R) Platinum 8375C CPU @ 2.90GHz` processor. Also all the servers for the open-source systems tested in our benchmarks run on hosts with the same type of processor.
 ### Run Test Page
 ![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/a789099a-3707-4214-8052-b73463b8f2c6)
 This is the page to run a test:
 1. Initially, you select the systems to be tested - multiple selections are allowed. Once selected, corresponding forms will pop up to gather necessary information for using the chosen databases. The db_label is used to differentiate different instances of the same system. We recommend filling in the host size or instance type here (as we do in our standard results).
 2. The next step is to select the test cases you want to perform. You can select multiple cases at once, and a form to collect corresponding parameters will appear.
 3. Finally, you'll need to provide a task label to distinguish different test results. Using the same label for different tests will result in the previous results being overwritten.
 Now we can only run one task at the same time. 
@@ -84,25 +119,25 @@
 #### Filtering Search Performance Case
 - **Large Dataset, Low Filtering Rate:** Evaluates search performance with a large dataset (Cohere 10M vectors, 768 dimensions) under a low filtering rate (1% vectors) at different parallel levels.
 - **Medium Dataset, Low Filtering Rate:** This case uses a medium dataset (Cohere 1M vectors, 768 dimensions) with a similar low filtering rate.
 - **Large Dataset, High Filtering Rate:** It tests with a large dataset (Cohere 10M vectors, 768 dimensions) but under a high filtering rate (99% vectors).
 - **Medium Dataset, High Filtering Rate:** This case uses a medium dataset (Cohere 1M vectors, 768 dimensions) with a high filtering rate.
 For a quick reference, here is a table summarizing the key aspects of each case:
 
-Case No. | Case Type | Dataset Size | Dataset Type | Filtering Rate | Results |
-|----------|-----------|--------------|--------------|----------------|---------|
-1 | Capacity Case | Large Dim | GIST 100K vectors, 960 dimensions | N/A | Number of inserted vectors |
-2 | Capacity Case | Small Dim | SIFT 100K vectors, 128 dimensions | N/A | Number of inserted vectors |
-3 | Search Performance Case | XLarge Dataset | LAION 100M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
-4 | Search Performance Case | Large Dataset | Cohere 10M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
-5 | Search Performance Case | Medium Dataset | Cohere 1M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
-6 | Filtering Search Performance Case | Large Dataset, Low Filtering Rate | Cohere 10M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
-7 | Filtering Search Performance Case | Medium Dataset, Low Filtering Rate | Cohere 1M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
-8 | Filtering Search Performance Case | Large Dataset, High Filtering Rate | Cohere 10M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
-9 | Filtering Search Performance Case | Medium Dataset, High Filtering Rate | Cohere 1M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
+Case No. | Case Type | Dataset Size  | Filtering Rate | Results |
+|----------|-----------|--------------|----------------|---------|
+1 | Capacity Case | GIST 100K vectors, 960 dimensions | N/A | Number of inserted vectors |
+2 | Capacity Case | SIFT 100K vectors, 128 dimensions | N/A | Number of inserted vectors |
+3 | Search Performance Case | LAION 100M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
+4 | Search Performance Case | Cohere 10M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
+5 | Search Performance Case | Cohere 1M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
+6 | Filtering Search Performance Case | Cohere 10M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
+7 | Filtering Search Performance Case | Cohere 1M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
+8 | Filtering Search Performance Case | Cohere 10M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
+9 | Filtering Search Performance Case | Cohere 1M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
 
 Each case provides an in-depth examination of a vector database's abilities, providing you a comprehensive view of the database's performance.
 
 ## Goals
 Our goals of this benchmark are:
 ### Reproducibility & Usability
 One of the primary goals of VectorDBBench is to enable users to reproduce benchmark results swiftly and easily, or to test their customized scenarios. We believe that lowering the barriers to entry for conducting these tests will enhance the community's understanding and improvement of vector databases. We aim to create an environment where any user, regardless of their technical expertise, can quickly set up and run benchmarks, and view and analyze results in an intuitive manner.
@@ -182,7 +217,68 @@
 ### Fine-Tuning
 For the system under test, we use the default server-side configuration to maintain the authenticity and representativeness of our results.
 For the Client, we welcome any parameter tuning to obtain better results.
 ### Incomplete Results
 Many databases may not be able to complete all test cases due to issues such as Out of Memory (OOM), crashes, or timeouts. In these scenarios, we will clearly state these occurrences in the test results.
 ### Mistake Or Misrepresentation 
 We strive for accuracy in learning and supporting various vector databases, yet there might be oversights or misapplications. For any such occurrences, feel free to [raise an issue](https://github.com/zilliztech/VectorDBBench/issues/new) or make amendments on our GitHub page.
+## Timeout
+In our pursuit to ensure that our benchmark reflects the reality of a production environment while guaranteeing the practicality of the system, we have implemented a timeout plan based on our experiences for various tests.
+
+**1. Capacity Case:**
+- For Capacity Case, we have assigned an overall timeout.
+
+**2. Other Cases:**
+
+For other cases, we have set two timeouts:
+
+- **Data Loading Timeout:** This timeout is designed to filter out systems that are too slow in inserting data, thus ensuring that we are only considering systems that is able to cope with the demands of a real-world production environment within a reasonable time frame.
+
+- **Optimization Preparation Timeout**: This timeout is established to avoid excessive optimization strategies that might work for benchmarks but fail to deliver in real production environments. By doing this, we ensure that the systems we consider are not only suitable for testing environments but also applicable and efficient in production scenarios.
+
+This multi-tiered timeout approach allows our benchmark to be more representative of actual production environments and assists us in identifying systems that can truly perform in real-world scenarios.
+<table>
+    <tr>
+        <th>Case</th>
+        <th>Data Size</th>
+        <th>Timeout Type</th>
+        <th>Value</th>
+    </tr>
+    <tr>
+        <td>Capacity Case</td>
+        <td>N/A</td>
+        <td>Loading timeout</td>
+        <td>24 hours</td>
+    </tr>
+    <tr>
+        <td rowspan="2">Other Cases</td>
+        <td rowspan="2">1M vectors, 768 dimensions</td>
+        <td>Loading timeout</td>
+        <td>2.5 hours</td>
+    </tr>
+    <tr>
+        <td>Optimization timeout</td>
+        <td>15 mins</td>
+    </tr>
+    <tr>
+        <td rowspan="2">Other Cases</td>
+        <td rowspan="2">10M vectors, 768 dimensions</td>
+        <td>Loading timeout</td>
+        <td>25 hours</td>
+    </tr>
+    <tr>
+        <td>Optimization timeout</td>
+        <td>2.5 hours</td>
+    </tr>
+    <tr>
+        <td rowspan="2">Other Cases</td>
+        <td rowspan="2">100M vectors, 768 dimensions</td>
+        <td>Loading timeout</td>
+        <td>250 hours</td>
+    </tr>
+    <tr>
+        <td>Optimization timeout</td>
+        <td>25 hours</td>
+    </tr>
+</table>
+
+**Note:** Some datapoints in the standard benchmark results that voilate this timeout will be kept for now for reference. We will remove them in the future.
```

### Comparing `vectordb-bench-0.0.2/pyproject.toml` & `vectordb-bench-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     "elasticsearch",
     "plotly",
     "pydantic==v1.10.7", # for qdrant-client
     "environs",
     "scikit-learn",
     "s3fs",
     "psutil",
+    "polars",
+    "pgvector",
+    "sqlalchemy"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
     "ruff",
     "pytest",
```

### Comparing `vectordb-bench-0.0.2/tests/test_bench_runner.py` & `vectordb-bench-0.0.3/tests/test_bench_runner.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/tests/test_elasticsearch_cloud.py` & `vectordb-bench-0.0.3/tests/test_elasticsearch_cloud.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/tests/test_models.py` & `vectordb-bench-0.0.3/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,10 +61,10 @@
             task_label="standard",
             results=all_results,
         )
         tr.write_file()
 
     def test_test_result_display(self):
         result_dir = config.RESULTS_LOCAL_DIR
-        for json_file in result_dir.glob("*.json"):
+        for json_file in result_dir.glob("result*.json"):
             res = TestResult.read_file(json_file)
             res.display()
```

### Comparing `vectordb-bench-0.0.2/tests/test_utils.py` & `vectordb-bench-0.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/tests/ut_cases.py` & `vectordb-bench-0.0.3/tests/ut_cases.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,33 @@
 from vectordb_bench.backend.cases import (
     PerformanceCase,
     CaseType,
 )
 
-import vectordb_bench.backend.dataset as ds
-from pydantic.dataclasses import dataclass
-
-@dataclass
-class Cohere_S(ds.Cohere):
-    label: str = "SMALL"
-    size: int  = 100_000
-
-@dataclass
-class Glove_S(ds.Glove):
-    label: str = "SMALL"
-    size : int = 100_000
+from vectordb_bench.backend.datase import Dataset, DatasetManager
 
 
 class Performance100K99p(PerformanceCase):
-    case_id: CaseType = CaseType.PerformanceSHigh
+    case_id: CaseType = 100
     filter_rate: float | int | None = 0.99
-    dataset: ds.DataSet = ds.get(ds.Name.Cohere, ds.Label.SMALL)
+    dataset: DatasetManager = Dataset.COHERE.manager(100_000)
     name: str = "Filtering Search Performance Test (100K Dataset, 768 Dim, Filter 99%)"
     description: str = """This case tests the search performance of a vector database with a small dataset (<b>Cohere 100K vectors</b>, 768 dimensions) under a high filtering rate (<b>99% vectors</b>), at varying parallel levels.
 Results will show index building time, recall, and maximum QPS."""
 
 class Performance100K1p(PerformanceCase):
-    case_id: CaseType = CaseType.PerformanceSLow
+    case_id: CaseType = 100
     filter_rate: float | int | None = 0.01
-    dataset: ds.DataSet = ds.get(ds.Name.Cohere, ds.Label.SMALL)
+    dataset: DatasetManager = Dataset.COHERE.manager(100_000)
     name: str = "Filtering Search Performance Test (100K Dataset, 768 Dim, Filter 1%)"
     description: str = (
         """This case tests the search performance of a vector database with a small dataset (<b>Cohere 100K vectors</b>, 768 dimensions) under a low filtering rate (<b>1% vectors</b>), at varying parallel levels.
 Results will show index building time, recall, and maximum QPS.""",
     )
 
 
 class Performance100K(PerformanceCase):
-    case_id: CaseType = CaseType.PerformanceSZero
-    dataset: ds.DataSet = ds.get(ds.Name.Cohere, ds.Label.SMALL)
+    case_id: CaseType = 100
+    dataset: DatasetManager = Dataset.COHERE.manager(100_000)
     name: str = "Search Performance Test (100K Dataset, 768 Dim)"
     description: str = """This case tests the search performance of a vector database with a small dataset (<b>Cohere 100K vectors</b>, 768 dimensions) at varying parallel levels.
 Results will show index building time, recall, and maximum QPS."""
-
-
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/__main__.py` & `vectordb-bench-0.0.3/vectordb_bench/__main__.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/assembler.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/assembler.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/cases.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/cases.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import typing
 import logging
 from enum import Enum, auto
 
-from . import dataset as ds
-from ..base import BaseModel
+from vectordb_bench import config
+from vectordb_bench.base import BaseModel
+
+from .dataset import Dataset, DatasetManager
 
 
 log = logging.getLogger(__name__)
 
 Case = typing.TypeVar("Case")
 
 
@@ -40,15 +42,15 @@
 
     @property
     def case_name(self) -> str:
         c = self.case_cls
         if c is not None:
             return c().name
         raise ValueError("Case unsupported")
-    
+
     @property
     def case_description(self) -> str:
         c = self.case_cls
         if c is not None:
             return c().description
         raise ValueError("Case unsupported")
 
@@ -69,15 +71,18 @@
         filters(dict | None): filters for search
     """
 
     case_id: CaseType
     label: CaseLabel
     name: str
     description: str
-    dataset: ds.DataSet
+    dataset: DatasetManager
+
+    load_timeout: float | int
+    optimize_timeout: float | int | None
 
     filter_rate: float | None
 
     @property
     def filters(self) -> dict | None:
         if self.filter_rate is not None:
             ID = round(self.filter_rate * self.dataset.data.size)
@@ -88,97 +93,113 @@
 
         return None
 
 
 class CapacityCase(Case, BaseModel):
     label: CaseLabel = CaseLabel.Load
     filter_rate: float | None = None
+    load_timeout: float | int = config.CAPACITY_TIMEOUT_IN_SECONDS
+    optimize_timeout: float | int | None = None
 
 
 class PerformanceCase(Case, BaseModel):
     label: CaseLabel = CaseLabel.Performance
     filter_rate: float | None = None
 
 
 class CapacityDim960(CapacityCase):
     case_id: CaseType = CaseType.CapacityDim960
-    dataset: ds.DataSet = ds.get(ds.Name.GIST, ds.Label.SMALL)
+    dataset: DatasetManager = Dataset.GIST.manager(100_000)
     name: str = "Capacity Test (960 Dim Repeated)"
     description: str = """This case tests the vector database's loading capacity by repeatedly inserting large-dimension vectors (GIST 100K vectors, <b>960 dimensions</b>) until it is fully loaded.
 Number of inserted vectors will be reported."""
 
 
 class CapacityDim128(CapacityCase):
     case_id: CaseType = CaseType.CapacityDim128
-    dataset: ds.DataSet = ds.get(ds.Name.SIFT, ds.Label.SMALL)
+    dataset: DatasetManager = Dataset.SIFT.manager(500_000)
     name: str = "Capacity Test (128 Dim Repeated)"
     description: str = """This case tests the vector database's loading capacity by repeatedly inserting small-dimension vectors (SIFT 100K vectors, <b>128 dimensions</b>) until it is fully loaded.
 Number of inserted vectors will be reported."""
 
 
 class Performance10M(PerformanceCase):
     case_id: CaseType = CaseType.Performance10M
-    dataset: ds.DataSet = ds.get(ds.Name.Cohere, ds.Label.LARGE)
+    dataset: DatasetManager = Dataset.COHERE.manager(10_000_000)
     name: str = "Search Performance Test (10M Dataset, 768 Dim)"
     description: str = """This case tests the search performance of a vector database with a large dataset (<b>Cohere 10M vectors</b>, 768 dimensions) at varying parallel levels.
 Results will show index building time, recall, and maximum QPS."""
+    load_timeout: float | int = config.LOAD_TIMEOUT_10M
+    optimize_timeout: float | int | None = config.OPTIMIZE_TIMEOUT_10M
 
 
 class Performance1M(PerformanceCase):
     case_id: CaseType = CaseType.Performance1M
-    dataset: ds.DataSet = ds.get(ds.Name.Cohere, ds.Label.MEDIUM)
+    dataset: DatasetManager = Dataset.COHERE.manager(1_000_000)
     name: str = "Search Performance Test (1M Dataset, 768 Dim)"
     description: str = """This case tests the search performance of a vector database with a medium dataset (<b>Cohere 1M vectors</b>, 768 dimensions) at varying parallel levels.
 Results will show index building time, recall, and maximum QPS."""
+    load_timeout: float | int = config.LOAD_TIMEOUT_1M
+    optimize_timeout: float | int | None = config.OPTIMIZE_TIMEOUT_1M
 
 
 class Performance10M1P(PerformanceCase):
     case_id: CaseType = CaseType.Performance10M1P
     filter_rate: float | int | None = 0.01
-    dataset: ds.DataSet = ds.get(ds.Name.Cohere, ds.Label.LARGE)
+    dataset: DatasetManager = Dataset.COHERE.manager(10_000_000)
     name: str = "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)"
     description: str = """This case tests the search performance of a vector database with a large dataset (<b>Cohere 10M vectors</b>, 768 dimensions) under a low filtering rate (<b>1% vectors</b>), at varying parallel levels.
 Results will show index building time, recall, and maximum QPS."""
+    load_timeout: float | int = config.LOAD_TIMEOUT_10M
+    optimize_timeout: float | int | None = config.OPTIMIZE_TIMEOUT_10M
 
 
 class Performance1M1P(PerformanceCase):
     case_id: CaseType = CaseType.Performance1M1P
     filter_rate: float | int | None = 0.01
-    dataset: ds.DataSet = ds.get(ds.Name.Cohere, ds.Label.MEDIUM)
+    dataset: DatasetManager = Dataset.COHERE.manager(1_000_000)
     name: str = "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)"
     description: str = """This case tests the search performance of a vector database with a medium dataset (<b>Cohere 1M vectors</b>, 768 dimensions) under a low filtering rate (<b>1% vectors</b>), at varying parallel levels.
 Results will show index building time, recall, and maximum QPS."""
+    load_timeout: float | int = config.LOAD_TIMEOUT_1M
+    optimize_timeout: float | int | None = config.OPTIMIZE_TIMEOUT_1M
 
 
 class Performance10M99P(PerformanceCase):
     case_id: CaseType = CaseType.Performance10M99P
     filter_rate: float | int | None = 0.99
-    dataset: ds.DataSet = ds.get(ds.Name.Cohere, ds.Label.LARGE)
+    dataset: DatasetManager = Dataset.COHERE.manager(10_000_000)
     name: str = "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)"
     description: str = """This case tests the search performance of a vector database with a large dataset (<b>Cohere 10M vectors</b>, 768 dimensions) under a high filtering rate (<b>99% vectors</b>), at varying parallel levels.
 Results will show index building time, recall, and maximum QPS."""
+    load_timeout: float | int = config.LOAD_TIMEOUT_10M
+    optimize_timeout: float | int | None = config.OPTIMIZE_TIMEOUT_10M
 
 
 class Performance1M99P(PerformanceCase):
     case_id: CaseType = CaseType.Performance1M99P
     filter_rate: float | int | None = 0.99
-    dataset: ds.DataSet = ds.get(ds.Name.Cohere, ds.Label.MEDIUM)
+    dataset: DatasetManager = Dataset.COHERE.manager(1_000_000)
     name: str = "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)"
     description: str = """This case tests the search performance of a vector database with a medium dataset (<b>Cohere 1M vectors</b>, 768 dimensions) under a high filtering rate (<b>99% vectors</b>), at varying parallel levels.
 Results will show index building time, recall, and maximum QPS."""
+    load_timeout: float | int = config.LOAD_TIMEOUT_1M
+    optimize_timeout: float | int | None = config.OPTIMIZE_TIMEOUT_1M
 
 
 
 class Performance100M(PerformanceCase):
     case_id: CaseType = CaseType.Performance100M
     filter_rate: float | int | None = None
-    dataset: ds.DataSet = ds.get(ds.Name.LAION, ds.Label.LARGE)
+    dataset: DatasetManager = Dataset.LAION.manager(100_000_000)
     name: str = "Search Performance Test (100M Dataset, 768 Dim)"
     description: str = """This case tests the search performance of a vector database with a large 100M dataset (<b>LAION 100M vectors</b>, 768 dimensions), at varying parallel levels.
 Results will show index building time, recall, and maximum QPS."""
+    load_timeout: float | int = config.LOAD_TIMEOUT_100M
+    optimize_timeout: float | int | None = config.OPTIMIZE_TIMEOUT_100M
 
 
 type2case = {
     CaseType.CapacityDim960: CapacityDim960,
     CaseType.CapacityDim128: CapacityDim128,
 
     CaseType.Performance100M: Performance100M,
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/clients/__init__.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/clients/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from .milvus.milvus import Milvus
 from .elastic_cloud.elastic_cloud import ElasticCloud
 from .pinecone.pinecone import Pinecone
 from .weaviate_cloud.weaviate_cloud import WeaviateCloud
 from .qdrant_cloud.qdrant_cloud import QdrantCloud
 from .zilliz_cloud.zilliz_cloud import ZillizCloud
-
+from .pgvector.pgvector import PgVector
 
 class DB(Enum):
     """Database types
 
     Examples:
         >>> DB.Milvus
         <DB.Milvus: 'Milvus'>
@@ -31,27 +31,32 @@
 
     Milvus = "Milvus"
     ZillizCloud = "ZillizCloud"
     Pinecone = "Pinecone"
     ElasticCloud = "ElasticCloud"
     QdrantCloud = "QdrantCloud"
     WeaviateCloud = "WeaviateCloud"
+    PgVector = "PgVector"
 
 
     @property
     def init_cls(self) -> Type[VectorDB]:
         return db2client.get(self)
 
 
 db2client = {
     DB.Milvus: Milvus,
     DB.ZillizCloud: ZillizCloud,
     DB.WeaviateCloud: WeaviateCloud,
     DB.ElasticCloud: ElasticCloud,
     DB.QdrantCloud: QdrantCloud,
     DB.Pinecone: Pinecone,
+    DB.PgVector: PgVector
 }
 
+for db in DB:
+    assert issubclass(db.init_cls, VectorDB)
+
 
 __all__ = [
     "DB", "VectorDB", "DBConfig", "DBCaseConfig", "IndexType", "MetricType", "EmptyDBCaseConfig",
 ]
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/clients/api.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/clients/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 
 class VectorDB(ABC):
     """Each VectorDB will be __init__ once for one case, the object will be copied into multiple processes.
 
     In each process, the benchmark cases ensure VectorDB.init() calls before any other methods operations
 
-    insert_embeddings, search_embedding, and, ready_to_search will be timed for each call.
+    insert_embeddings, search_embedding, and, optimize will be timed for each call.
 
     Examples:
         >>> milvus = Milvus()
         >>> with milvus.init():
         >>>     milvus.insert_embeddings()
         >>>     milvus.search_embedding()
     """
@@ -86,17 +86,20 @@
     def __init__(
         self,
         dim: int,
         db_config: dict,
         db_case_config: DBCaseConfig | None,
         collection_name: str,
         drop_old: bool = False,
-        **kwargs
+        **kwargs,
     ) -> None:
-        """Initialize wrapper around the vector database client
+        """Initialize wrapper around the vector database client.
+
+        Please drop the existing collection if drop_old is True. And create collection
+        if collection not in the Vector Database
 
         Args:
             dim(int): the dimension of the dataset
             db_config(dict): configs to establish connections with the vector database
             db_case_config(DBCaseConfig | None): case specific configs for indexing and searching
             drop_old(bool): whether to drop the existing collection of the dataset.
         """
@@ -126,23 +129,23 @@
         raise NotImplementedError
 
     @abstractmethod
     def insert_embeddings(
         self,
         embeddings: list[list[float]],
         metadata: list[int],
-        kwargs: Any,
+        **kwargs,
     ) -> (int, Exception):
         """Insert the embeddings to the vector database. The default number of embeddings for
         each insert_embeddings is 5000.
 
         Args:
             embeddings(list[list[float]]): list of embedding to add to the vector database.
             metadatas(list[int]): metadata associated with the embeddings, for filtering.
-            kwargs(Any): vector database specific parameters.
+            **kwargs(Any): vector database specific parameters.
 
         Returns:
             int: inserted data count
         """
         raise NotImplementedError
 
     @abstractmethod
@@ -162,21 +165,22 @@
         Returns:
             list[int]: list of k most similar embeddings IDs to the query embedding.
         """
         raise NotImplementedError
 
     # TODO: remove
     @abstractmethod
-    def ready_to_search(self):
-        """ready_to_search will be called between insertion and search in performance cases.
+    def optimize(self):
+        """optimize will be called between insertion and search in performance cases.
 
         Should be blocked until the vectorDB is ready to be tested on
         heavy performance cases.
 
-        Time(insert the dataset) + Time(ready_to_search) will be recorded as "load_duration" metric
+        Time(insert the dataset) + Time(optimize) will be recorded as "load_duration" metric
+        Optimize's execution time is limited, the limited time is based on cases.
         """
         raise NotImplementedError
 
     # TODO: remove
     @abstractmethod
     def ready_to_load(self):
         """ready_to_load will be called before load in load cases.
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/clients/elastic_cloud/config.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/clients/elastic_cloud/config.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/clients/elastic_cloud/elastic_cloud.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/clients/elastic_cloud/elastic_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         dim: int,
         db_config: dict,
         db_case_config: ElasticCloudIndexConfig,
         indice: str = "vdb_bench_indice",  # must be lowercase
         id_col_name: str = "id",
         vector_col_name: str = "vector",
         drop_old: bool = False,
+        **kwargs,
     ):
         self.dim = dim
         self.db_config = db_config
         self.case_config = db_case_config
         self.indice = indice
         self.id_col_name = id_col_name
         self.vector_col_name = vector_col_name
@@ -79,14 +80,15 @@
             log.warning(f"Failed to create indice: {self.indice} error: {str(e)}")
             raise e from None
 
     def insert_embeddings(
         self,
         embeddings: Iterable[list[float]],
         metadata: list[int],
+        **kwargs,
     ) -> (int, Exception):
         """Insert the embeddings to the elasticsearch."""
         assert self.client is not None, "should self.init() first"
 
         insert_data = [
             {
                 "_index": self.indice,
@@ -139,14 +141,14 @@
             res = [d["_source"][self.id_col_name] for d in search_res["hits"]["hits"]]
 
             return res
         except Exception as e:
             log.warning(f"Failed to search: {self.indice} error: {str(e)}")
             raise e from None
 
-    def ready_to_search(self):
-        """ready_to_search will be called between insertion and search in performance cases."""
+    def optimize(self):
+        """optimize will be called between insertion and search in performance cases."""
         pass
 
     def ready_to_load(self):
         """ready_to_load will be called before load in load cases."""
         pass
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/clients/milvus/config.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/clients/milvus/config.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/clients/milvus/milvus.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/clients/milvus/milvus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Wrapper around the Milvus vector database over VectorDB"""
 
 import logging
 from contextlib import contextmanager
-from typing import Any, Iterable, Type
+from typing import Iterable, Type
 
 from pymilvus import Collection, utility
 from pymilvus import CollectionSchema, DataType, FieldSchema, MilvusException
 
 from ..api import VectorDB, DBCaseConfig, DBConfig, IndexType
 from .config import MilvusConfig, _milvus_case_config
 
@@ -20,14 +20,15 @@
         self,
         dim: int,
         db_config: dict,
         db_case_config: DBCaseConfig,
         collection_name: str = "VectorDBBenchCollection",
         drop_old: bool = False,
         name: str = "Milvus",
+        **kwargs,
     ):
         """Initialize wrapper around the milvus vector database."""
         self.name = name
         self.db_config = db_config
         self.case_config = db_case_config
         self.collection_name = collection_name
         self.batch_size = int(MILVUS_LOAD_REQS_SIZE / (dim *4))
@@ -49,15 +50,15 @@
                 FieldSchema(self._scalar_field, DataType.INT64),
                 FieldSchema(self._vector_field, DataType.FLOAT_VECTOR, dim=dim)
             ]
 
             log.info(f"{self.name} create collection: {self.collection_name}")
 
             # Create the collection
-            coll = Collection(
+            Collection(
                 name=self.collection_name,
                 schema=CollectionSchema(fields),
                 consistency_level="Session",
             )
 
             #  self._pre_load(coll)
 
@@ -104,65 +105,71 @@
             except Exception as e:
                 log.warning(f"{self.name} pre load error: {e}")
                 raise e from None
 
     def _optimize(self):
         log.info(f"{self.name} optimizing before search")
         try:
+            self.col.load()
+        except Exception as e:
+            log.warning(f"{self.name} optimize error: {e}")
+            raise e from None
+
+    def _post_insert(self):
+        log.info(f"{self.name} post insert before optimize")
+        try:
             self.col.flush()
             self.col.compact()
             self.col.wait_for_compaction_completed()
 
             # wait for index done and load refresh
             self.col.create_index(
                 self._vector_field,
                 self.case_config.index_param(),
                 index_name=self._index_name,
             )
             utility.wait_for_index_building_complete(self.collection_name)
-            self.col.load()
-            #  self.col.load(_refresh=True)
-            #  utility.wait_for_loading_complete(self.collection_name)
-            #  import time; time.sleep(10)
         except Exception as e:
             log.warning(f"{self.name} optimize error: {e}")
             raise e from None
 
     def ready_to_load(self):
         assert self.col, "Please call self.init() before"
         self._pre_load(self.col)
         pass
 
-    def ready_to_search(self):
+    def optimize(self):
         assert self.col, "Please call self.init() before"
         self._optimize()
 
     def insert_embeddings(
         self,
         embeddings: Iterable[list[float]],
         metadata: list[int],
-        **kwargs: Any,
+        **kwargs,
     ) -> (int, Exception):
         """Insert embeddings into Milvus. should call self.init() first"""
         # use the first insert_embeddings to init collection
         assert self.col is not None
         assert len(embeddings) == len(metadata)
         insert_count = 0
         try:
             for batch_start_offset in range(0, len(embeddings), self.batch_size):
                 batch_end_offset = min(batch_start_offset + self.batch_size, len(embeddings))
                 insert_data = [
                         metadata[batch_start_offset : batch_end_offset],
                         metadata[batch_start_offset : batch_end_offset],
                         embeddings[batch_start_offset : batch_end_offset],
                 ]
-                res = self.col.insert(insert_data, **kwargs)
+                res = self.col.insert(insert_data)
                 insert_count += len(res.primary_keys)
+            if kwargs.get("last_batch"):
+                self._post_insert()
         except MilvusException as e:
-            log.warning("Failed to insert data")
+            log.info(f"Failed to insert data: {e}")
             return (insert_count, e)
         return (insert_count, None)
 
     def search_embedding(
         self,
         query: list[float],
         k: int = 100,
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/clients/pinecone/pinecone.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/clients/pinecone/pinecone.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Wrapper around the Pinecone vector database over VectorDB"""
 
 import logging
 from contextlib import contextmanager
-from typing import Any, Type
+from typing import Type
 
 from ..api import VectorDB, DBConfig, DBCaseConfig, EmptyDBCaseConfig, IndexType
 from .config import PineconeConfig
 
 
 log = logging.getLogger(__name__)
 
@@ -16,14 +16,15 @@
 class Pinecone(VectorDB):
     def __init__(
         self,
         dim,
         db_config: dict,
         db_case_config: DBCaseConfig,
         drop_old: bool = False,
+        **kwargs,
     ):
         """Initialize wrapper around the milvus vector database."""
         self.index_name = db_config["index_name"]
         self.api_key = db_config["api_key"]
         self.environment = db_config["environment"]
         self.batch_size = int(min(PINECONE_MAX_SIZE_PER_BATCH / (dim * 5), PINECONE_MAX_NUM_PER_BATCH))
         # Pincone will make connections with server while import
@@ -65,21 +66,22 @@
         self.index = pinecone.Index(self.index_name)
         yield
         self.index.close()
 
     def ready_to_load(self):
         pass
 
-    def ready_to_search(self):
+    def optimize(self):
         pass
 
     def insert_embeddings(
         self,
         embeddings: list[list[float]],
         metadata: list[int],
+        **kwargs,
     ) -> (int, Exception):
         assert len(embeddings) == len(metadata)
         insert_count = 0
         try:
             for batch_start_offset in range(0, len(embeddings), self.batch_size):
                 batch_end_offset = min(batch_start_offset + self.batch_size, len(embeddings))
                 insert_datas = []
@@ -95,15 +97,14 @@
 
     def search_embedding(
         self,
         query: list[float],
         k: int = 100,
         filters: dict | None = None,
         timeout: int | None = None,
-        **kwargs: Any,
     ) -> list[tuple[int, float]]:
         if filters is None:
             pinecone_filters = {}
         else:
             pinecone_filters = {self._metadata_key: {"$gte": filters["id"]}}
         try:
             res = self.index.query(
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/clients/qdrant_cloud/qdrant_cloud.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/clients/qdrant_cloud/qdrant_cloud.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Wrapper around the QdrantCloud vector database over VectorDB"""
 
 import logging
 import time
 from contextlib import contextmanager
-from typing import Any, Type
+from typing import Type
 
-from ..api import VectorDB, DBConfig, DBCaseConfig, EmptyDBCaseConfig, IndexType
-from .config import QdrantConfig
+from ..api import VectorDB, DBConfig, DBCaseConfig, IndexType
+from .config import QdrantConfig, QdrantIndexConfig
 from qdrant_client.http.models import (
     CollectionStatus,
-    Distance,
     VectorParams,
     PayloadSchemaType,
     Batch,
     Filter,
     FieldCondition,
     Range,
 )
@@ -28,14 +27,15 @@
     def __init__(
         self,
         dim: int,
         db_config: dict,
         db_case_config: DBCaseConfig,
         collection_name: str = "QdrantCloudCollection",
         drop_old: bool = False,
+        **kwargs,
     ):
         """Initialize wrapper around the QdrantCloud vector database."""
         self.db_config = db_config
         self.case_config = db_case_config
         self.collection_name = collection_name
 
         self._primary_field = "pk"
@@ -51,15 +51,15 @@
 
     @classmethod
     def config_cls(cls) -> Type[DBConfig]:
         return QdrantConfig
 
     @classmethod
     def case_config_cls(cls, index_type: IndexType | None = None) -> Type[DBCaseConfig]:
-        return EmptyDBCaseConfig
+        return QdrantIndexConfig
 
     @contextmanager
     def init(self) -> None:
         """
         Examples:
             >>> with self.init():
             >>>     self.insert_embeddings()
@@ -70,15 +70,15 @@
         self.qdrant_client = None
         del(self.qdrant_client)
 
     def ready_to_load(self):
         pass
 
 
-    def ready_to_search(self):
+    def optimize(self):
         assert self.qdrant_client, "Please call self.init() before"
         # wait for vectors to be fully indexed
         SECONDS_WAITING_FOR_INDEXING_API_CALL = 5
         try:
             while True:
                 info = self.qdrant_client.get_collection(self.collection_name)
                 time.sleep(SECONDS_WAITING_FOR_INDEXING_API_CALL)
@@ -93,15 +93,15 @@
 
     def _create_collection(self, dim, qdrant_client: int):
         log.info(f"Create collection: {self.collection_name}")
 
         try:
             qdrant_client.create_collection(
                 collection_name=self.collection_name,
-                vectors_config=VectorParams(size=dim, distance=Distance.EUCLID)
+                vectors_config=VectorParams(size=dim, distance=self.case_config.index_param()["distance"])
             )
 
             qdrant_client.create_payload_index(
                 collection_name=self.collection_name,
                 field_name=self._primary_field,
                 field_schema=PayloadSchemaType.INTEGER,
             )
@@ -112,37 +112,37 @@
             log.warning(f"Failed to create collection: {self.collection_name} error: {e}")
             raise e from None
 
     def insert_embeddings(
         self,
         embeddings: list[list[float]],
         metadata: list[int],
-        **kwargs: Any,
+        **kwargs,
     ) -> (int, Exception):
         """Insert embeddings into Milvus. should call self.init() first"""
         assert self.qdrant_client is not None
         try:
             # TODO: counts
             _ = self.qdrant_client.upsert(
                 collection_name=self.collection_name,
                 wait=True,
                 points=Batch(ids=metadata, payloads=[{self._primary_field: v} for v in metadata], vectors=embeddings)
             )
-            return (len(metadata), None)
         except Exception as e:
             log.info(f"Failed to insert data, {e}")
-            return (0, e)
+            return 0, e
+        else:
+            return len(metadata), None
 
     def search_embedding(
         self,
         query: list[float],
         k: int = 100,
         filters: dict | None = None,
         timeout: int | None = None,
-        **kwargs: Any,
     ) -> list[int]:
         """Perform a search on a query embedding and return results with score.
         Should call self.init() first.
         """
         assert self.qdrant_client is not None
 
         f = None
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/clients/weaviate_cloud/config.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/clients/weaviate_cloud/config.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/clients/weaviate_cloud/weaviate_cloud.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/clients/weaviate_cloud/weaviate_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Wrapper around the Weaviate vector database over VectorDB"""
 
 import logging
-from typing import Any, Iterable, Type
+from typing import Iterable, Type
 from contextlib import contextmanager
 
 from weaviate.exceptions import WeaviateBaseError
 
 from ..api import VectorDB, DBConfig, DBCaseConfig, IndexType
 from .config import WeaviateConfig, WeaviateIndexConfig
 
@@ -17,14 +17,15 @@
     def __init__(
         self,
         dim: int,
         db_config: dict,
         db_case_config: DBCaseConfig,
         collection_name: str = "VectorDBBenchCollection",
         drop_old: bool = False,
+        **kwargs,
     ):
         """Initialize wrapper around the weaviate vector database."""
         self.db_config = db_config
         self.case_config = db_case_config
         self.collection_name = collection_name
 
         self._scalar_field = "key"
@@ -66,15 +67,15 @@
         self.client = None
         del(self.client)
 
     def ready_to_load(self):
         """Should call insert first, do nothing"""
         pass
 
-    def ready_to_search(self):
+    def optimize(self):
         assert self.client.schema.exists(self.collection_name)
         self.client.schema.update_config(self.collection_name, {"vectorIndexConfig": self.case_config.search_param() } )
 
     def _create_collection(self, client):
         if not client.schema.exists(self.collection_name):
             log.info(f"Create collection: {self.collection_name}")
             class_obj = {
@@ -94,21 +95,21 @@
                 log.warning(f"Failed to create collection: {self.collection_name} error: {str(e)}")
                 raise e from None
 
     def insert_embeddings(
         self,
         embeddings: Iterable[list[float]],
         metadata: list[int],
-        **kwargs: Any,
+        **kwargs,
     ) -> (int, Exception):
         """Insert embeddings into Weaviate"""
         assert self.client.schema.exists(self.collection_name)
         insert_count = 0
         try:
-            with self.client.batch as batch:               
+            with self.client.batch as batch:
                 batch.batch_size = len(metadata)
                 batch.dynamic = True
                 res = []
                 for i in range(len(metadata)):
                     res.append(batch.add_data_object(
                         {self._scalar_field: metadata[i]},
                         class_name=self.collection_name,
@@ -122,15 +123,14 @@
 
     def search_embedding(
         self,
         query: list[float],
         k: int = 100,
         filters: dict | None = None,
         timeout: int | None = None,
-        **kwargs: Any,
     ) -> list[int]:
         """Perform a search on a query embedding and return results with distance.
         Should call self.init() first.
         """
         assert self.client.schema.exists(self.collection_name)
 
         query_obj = self.client.query.get(self.collection_name, [self._scalar_field]).with_additional("distance").with_near_vector({"vector": query}).with_limit(k)
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/clients/zilliz_cloud/config.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/clients/zilliz_cloud/config.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/clients/zilliz_cloud/zilliz_cloud.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/clients/zilliz_cloud/zilliz_cloud.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,23 +10,25 @@
     def __init__(
         self,
         dim: int,
         db_config: dict,
         db_case_config: DBCaseConfig,
         collection_name: str = "ZillizCloudVectorDBBench",
         drop_old: bool = False,
-        name: str = "ZillizCloud"
+        name: str = "ZillizCloud",
+        **kwargs, 
     ):
         super().__init__(
             dim=dim,
             db_config=db_config,
             db_case_config=db_case_config,
             collection_name=collection_name,
             drop_old=drop_old,
             name=name,
+            **kwargs,
         )
 
     @classmethod
     def config_cls(cls) -> Type[DBConfig]:
         return ZillizCloudConfig
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/dataset.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,152 +1,124 @@
 """
 Usage:
-    >>> from xxx import dataset as ds
-    >>> gist_s = ds.get(ds.Name.GIST, ds.Label.SMALL)
-    >>> gist_s.dict()
-    dataset: {'data': {'name': 'GIST', 'dim': 128, 'metric_type': 'L2', 'label': 'SMALL', 'size': 50000000}, 'data_dir': 'xxx'}
+    >>> from xxx.dataset import Dataset
+    >>> Dataset.Cohere.get(100_000)
 """
 
 import os
 import logging
 import pathlib
-import math
 from hashlib import md5
-from enum import Enum, auto
-from typing import Any
-
+from enum import Enum
 import s3fs
 import pandas as pd
 from tqdm import tqdm
-from pydantic.dataclasses import dataclass
+from pydantic import validator, PrivateAttr
+import polars as pl
+from pyarrow.parquet import ParquetFile
 
 from ..base import BaseModel
 from .. import config
 from ..backend.clients import MetricType
 from . import utils
 
 log = logging.getLogger(__name__)
 
-@dataclass
-class LAION:
+
+class BaseDataset(BaseModel):
+    name: str
+    size: int
+    dim: int
+    metric_type: MetricType
+    use_shuffled: bool
+    _size_label: dict = PrivateAttr()
+
+    @validator("size")
+    def verify_size(cls, v):
+        if v not in cls._size_label:
+            raise ValueError(f"Size {v} not supported for the dataset, expected: {cls._size_label.keys()}")
+        return v
+
+    @property
+    def label(self) -> str:
+        return self._size_label.get(self.size)
+
+    @property
+    def dir_name(self) -> str:
+        return f"{self.name}_{self.label}_{utils.numerize(self.size)}".lower()
+
+
+class LAION(BaseDataset):
     name: str = "LAION"
     dim: int = 768
     metric_type: MetricType = MetricType.L2
     use_shuffled: bool = False
+    _size_label: dict = {100_000_000: "LARGE"}
 
-    @property
-    def dir_name(self) -> str:
-        return f"{self.name}_{self.label}_{utils.numerize(self.size)}".lower()
 
-@dataclass
-class GIST:
+class GIST(BaseDataset):
     name: str = "GIST"
     dim: int = 960
     metric_type: MetricType = MetricType.L2
     use_shuffled: bool = False
+    _size_label: dict = {
+        100_000: "SMALL",
+        1_000_000: "MEDIUM",
+    }
 
-    @property
-    def dir_name(self) -> str:
-        return f"{self.name}_{self.label}_{utils.numerize(self.size)}".lower()
 
-@dataclass
-class Cohere:
+class Cohere(BaseDataset):
     name: str = "Cohere"
     dim: int = 768
     metric_type: MetricType = MetricType.COSINE
     use_shuffled: bool = config.USE_SHUFFLED_DATA
+    _size_label: dict = {
+        100_000: "SMALL",
+        1_000_000: "MEDIUM",
+        10_000_000: "LARGE",
+    }
 
-    @property
-    def dir_name(self) -> str:
-        return f"{self.name}_{self.label}_{utils.numerize(self.size)}".lower()
 
-@dataclass
-class Glove:
+class Glove(BaseDataset):
     name: str = "Glove"
     dim: int = 200
     metric_type: MetricType = MetricType.COSINE
     use_shuffled: bool = False
+    _size_label: dict = {1_000_000: "MEDIUM"}
 
-    @property
-    def dir_name(self) -> str:
-        return f"{self.name}_{self.label}_{utils.numerize(self.size)}".lower()
 
-@dataclass
-class SIFT:
+class SIFT(BaseDataset):
     name: str = "SIFT"
     dim: int = 128
-    metric_type: MetricType = MetricType.COSINE
+    metric_type: MetricType = MetricType.L2
     use_shuffled: bool = False
+    _size_label: dict = {
 
-    @property
-    def dir_name(self) -> str:
-        return f"{self.name}_{self.label}_{utils.numerize(self.size)}".lower()
+        500_000: "SMALL",
+        5_000_000: "MEDIUM",
+        50_000_000: "LARGE",
+    }
 
-@dataclass
-class LAION_L(LAION):
-    label: str = "LARGE"
-    size: int  = 100_000_000
-
-@dataclass
-class GIST_S(GIST):
-    label: str = "SMALL"
-    size: int  = 100_000
-
-@dataclass
-class GIST_M(GIST):
-    label: str = "MEDIUM"
-    size: int  = 1_000_000
-
-@dataclass
-class Cohere_M(Cohere):
-    label: str = "MEDIUM"
-    size: int = 1_000_000
-
-@dataclass
-class Cohere_L(Cohere):
-    label : str = "LARGE"
-    size  : int = 10_000_000
-
-@dataclass
-class Glove_M(Glove):
-    label: str = "MEDIUM"
-    size : int = 1_000_000
-
-@dataclass
-class SIFT_S(SIFT):
-    label: str = "SMALL"
-    size : int = 500_000
-
-@dataclass
-class SIFT_M(SIFT):
-    label: str = "MEDIUM"
-    size : int = 5_000_000
-
-@dataclass
-class SIFT_L(SIFT):
-    label: str = "LARGE"
-    size : int = 50_000_000
 
-
-class DataSet(BaseModel):
+class DatasetManager(BaseModel):
     """Download dataset if not int the local directory. Provide data for cases.
 
     DataSet is iterable, each iteration will return the next batch of data in pandas.DataFrame
 
     Examples:
         >>> cohere_s = DataSet(data=Cohere_S)
         >>> for data in cohere_s:
         >>>    print(data.columns)
     """
-    data:   GIST | Cohere | Glove | SIFT | Any
+    data:   BaseDataset
     test_data: pd.DataFrame | None = None
     train_files : list[str] = []
 
     def __eq__(self, obj):
-        if isinstance(obj, DataSet):
+        if isinstance(obj, DatasetManager):
             return self.data.name == obj.data.name and \
                 self.data.label == obj.data.label
         return False
 
     @property
     def data_dir(self) -> pathlib.Path:
         """ data local directory: config.DATASET_LOCAL_DIR/{dataset_name}/{dataset_dirname}
@@ -290,92 +262,70 @@
             file_name = "neighbors_tail_1p.parquet"
         else:
             raise ValueError(f"Filters not supported: {filters}")
         return self._read_file(file_name)
 
     def _read_file(self, file_name: str) -> pd.DataFrame:
         """read one file from disk into memory"""
-        import pyarrow.parquet as pq
-
+        log.info(f"Read the entire file into memory: {file_name}")
         p = pathlib.Path(self.data_dir, file_name)
-        log.info(f"reading file into memory: {p}")
         if not p.exists():
             log.warning(f"No such file: {p}")
             return pd.DataFrame()
-        data = pq.read_table(p)
-        df = data.to_pandas()
-        return df
+
+        return pl.read_parquet(p)
 
 
 class DataSetIterator:
-    def __init__(self, dataset: DataSet):
+    def __init__(self, dataset: DatasetManager):
         self._ds = dataset
         self._idx = 0  # file number
-        self._curr: pd.DataFrame | None = None
+        self._cur = None
         self._sub_idx = [0 for i in range(len(self._ds.train_files))] # iter num for each file
 
+    def _get_iter(self, file_name: str):
+        p = pathlib.Path(self._ds.data_dir, file_name)
+        log.info(f"Get iterator for {p.name}")
+        if not p.exists():
+            raise IndexError(f"No such file {p}")
+            log.warning(f"No such file: {p}")
+        return ParquetFile(p).iter_batches(config.NUM_PER_BATCH)
+
     def __next__(self) -> pd.DataFrame:
         """return the data in the next file of the training list"""
         if self._idx < len(self._ds.train_files):
-            _sub = self._sub_idx[self._idx]
-            if _sub == 0 and self._idx == 0: # init
+            if self._cur is None:
                 file_name = self._ds.train_files[self._idx]
-                self._curr = self._ds._read_file(file_name)
-                self._iter_num = math.ceil(self._curr.shape[0]/100_000)
+                self._cur = self._get_iter(file_name)
 
-            if _sub == self._iter_num:
+            try:
+                return next(self._cur).to_pandas()
+            except StopIteration:
                 if self._idx == len(self._ds.train_files) - 1:
-                    self._curr = None
-                    raise StopIteration
-                else:
-                    self._idx += 1
-                    _sub = self._sub_idx[self._idx]
-
-                    self._curr = None
-                    file_name = self._ds.train_files[self._idx]
-                    self._curr = self._ds._read_file(file_name)
-
-            sub_df = self._curr[_sub*100_000: (_sub+1)*100_000]
-            self._sub_idx[self._idx] += 1
-            log.info(f"Get the [{_sub+1}/{self._iter_num}] batch of {self._idx+1}/{len(self._ds.train_files)} train file")
-            return sub_df
-        self._curr = None
+                    raise StopIteration from None
+
+                self._idx += 1
+                file_name = self._ds.train_files[self._idx]
+                self._cur = self._get_iter(file_name)
+                return next(self._cur).to_pandas()
         raise StopIteration
 
 
-class Name(Enum):
-    GIST = auto()
-    Cohere = auto()
-    Glove = auto()
-    SIFT = auto()
-    LAION = auto()
-
-
-class Label(Enum):
-    SMALL = auto()
-    MEDIUM = auto()
-    LARGE = auto()
-
-_global_ds_mapping = {
-    Name.GIST: {
-        Label.SMALL: DataSet(data=GIST_S()),
-        Label.MEDIUM: DataSet(data=GIST_M()),
-    },
-    Name.Cohere: {
-        Label.MEDIUM: DataSet(data=Cohere_M()),
-        Label.LARGE: DataSet(data=Cohere_L()),
-    },
-    Name.Glove:{
-        Label.MEDIUM: DataSet(data=Glove_M()),
-    },
-    Name.SIFT: {
-        Label.SMALL: DataSet(data=SIFT_S()),
-        Label.MEDIUM: DataSet(data=SIFT_M()),
-        Label.LARGE: DataSet(data=SIFT_L()),
-    },
-    Name.LAION: {
-        Label.LARGE: DataSet(data=LAION_L()),
-    },
-}
+class Dataset(Enum):
+    """
+    Value is Dataset classes, DO NOT use it
+    Example:
+        >>> all_dataset = [ds.name for ds in Dataset]
+        >>> Dataset.COHERE.manager(100_000)
+        >>> Dataset.COHERE.get(100_000)
+    """
+    LAION = LAION
+    GIST = GIST
+    COHERE = Cohere
+    GLOVE = Glove
+    SIFT = SIFT
+
+    def get(self, size: int) -> BaseDataset:
+        return self.value(size=size)
 
-def get(ds: Name, label: Label):
-    return _global_ds_mapping.get(ds, {}).get(label)
+    def manager(self, size: int) -> DatasetManager:
+        return DatasetManager(data=self.get(size))
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/runner/mp_runner.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/runner/mp_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,20 @@
         self.filters = filters
         self.concurrencies = concurrencies
         self.duration = duration
 
         self.test_data = utils.SharedNumpyArray(test_data)
         log.debug(f"test dataset columns: {len(test_data)}")
 
-    def search(self, test_np: utils.SharedNumpyArray) -> tuple[int, float]:
+    def search(self, test_np: utils.SharedNumpyArray, q: mp.Queue, cond: mp.Condition) -> tuple[int, float]:
+        # sync all process
+        q.put(1)
+        with cond:
+            cond.wait()
+
         with self.db.init():
             test_data = test_np.read().tolist()
             num, idx = len(test_data), 0
 
             start_time = time.perf_counter()
             count = 0
             while time.perf_counter() < start_time + self.duration:
@@ -73,37 +78,48 @@
             f"actual_dur={total_dur}s, count={count}, qps in this process: {round(count / total_dur, 4):3}"
          )
 
         return (count, total_dur)
 
     @staticmethod
     def get_mp_context():
-        mp_start_method = "forkserver" if "forkserver" in mp.get_all_start_methods() else "spawn"
+        mp_start_method = "spawn"
         log.debug(f"MultiProcessingSearchRunner get multiprocessing start method: {mp_start_method}")
         return mp.get_context(mp_start_method)
 
     def _run_all_concurrencies_mem_efficient(self) -> float:
         max_qps = 0
         try:
             for conc in self.concurrencies:
-                with concurrent.futures.ProcessPoolExecutor(mp_context=self.get_mp_context(), max_workers=conc) as executor:
-                    start = time.perf_counter()
-                    log.info(f"start search {self.duration}s in concurrency {conc}, filters: {self.filters}")
-                    future_iter = executor.map(self.search, [self.test_data for i in range(conc)])
-                    all_count = sum([r[0] for r in future_iter])
-
-                    cost = time.perf_counter() - start
-                    qps = round(all_count / cost, 4)
-                    log.info(f"end search in concurrency {conc}: dur={cost}s, total_count={all_count}, qps={qps}")
+                with mp.Manager() as m:
+                    q, cond = m.Queue(), m.Condition()
+                    with concurrent.futures.ProcessPoolExecutor(mp_context=self.get_mp_context(), max_workers=conc) as executor:
+                        log.info(f"Start search {self.duration}s in concurrency {conc}, filters: {self.filters}")
+                        future_iter = [executor.submit(self.search, self.test_data, q, cond) for i in range(conc)]
+                        # Sync all processes
+                        while q.qsize() < conc:
+                            sleep_t = conc if conc < 10 else 10
+                            time.sleep(sleep_t)
+
+                        with cond:
+                            cond.notify_all()
+                            log.info(f"Syncing all process and start concurrency search, concurrency={conc}")
+
+                        start = time.perf_counter()
+                        all_count = sum([r.result()[0] for r in future_iter])
+                        cost = time.perf_counter() - start
+
+                        qps = round(all_count / cost, 4)
+                        log.info(f"End search in concurrency {conc}: dur={cost}s, total_count={all_count}, qps={qps}")
 
                 if qps > max_qps:
                     max_qps = qps
-                    log.info(f"update largest qps with concurrency {conc}: current max_qps={max_qps}")
+                    log.info(f"Update largest qps with concurrency {conc}: current max_qps={max_qps}")
         except Exception as e:
-            log.warning(f"fail to search all concurrencies: {self.concurrencies}, max_qps before failure={max_qps}, reason={e}")
+            log.warning(f"Fail to search all concurrencies: {self.concurrencies}, max_qps before failure={max_qps}, reason={e}")
             traceback.print_exc()
 
             # No results available, raise exception
             if max_qps == 0.0:
                 raise e from None
 
         finally:
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/runner/serial_runner.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/runner/serial_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,135 +1,153 @@
 import time
 import logging
 import traceback
 import concurrent
 import multiprocessing as mp
 import math
+import psutil
+
 import numpy as np
 import pandas as pd
 
 from ..clients import api
 from ...metric import calc_recall
-from ...models import LoadTimeoutError
+from ...models import LoadTimeoutError, PerformanceTimeoutError
 from .. import utils
 from ... import config
+from vectordb_bench.backend.dataset import DatasetManager
 
 NUM_PER_BATCH = config.NUM_PER_BATCH
-LOAD_TIMEOUT = 24 * 60 * 60
 LOAD_MAX_TRY_COUNT = 10
 WAITTING_TIME = 60
 
 log = logging.getLogger(__name__)
 
-
 class SerialInsertRunner:
-    def __init__(self, db: api.VectorDB, train_emb: list[list[float]], train_id: list[int]):
-        log.debug(f"Dataset shape: {len(train_emb)}")
+    def __init__(self, db: api.VectorDB, dataset: DatasetManager, normalize: bool, timeout: float | None = None):
+        self.timeout = timeout if isinstance(timeout, (int, float)) else None
+        self.dataset = dataset
         self.db = db
-        self.shared_emb = train_emb
-        self.train_id = train_id
-
-        self.seq_batches = math.ceil(len(train_emb)/NUM_PER_BATCH)
+        self.normalize = normalize
 
-    def insert_data(self, left_id: int = 0) -> int:
+    def task(self) -> int:
+        count = 0
         with self.db.init():
-            all_embeddings = self.shared_emb
-
-            # unique id for endlessness insertion
-            all_metadata = [i+left_id for i in self.train_id]
+            log.info(f"({mp.current_process().name:16}) Start inserting embeddings in batch {config.NUM_PER_BATCH}")
+            start = time.perf_counter()
+            for data_df in self.dataset:
+                all_metadata = data_df['id'].tolist()
+
+                emb_np = np.stack(data_df['emb'])
+                if self.normalize:
+                    log.debug("normalize the 100k train data")
+                    all_embeddings = emb_np / np.linalg.norm(emb_np, axis=1)[:, np.newaxis].tolist()
+                else:
+                    all_embeddings = emb_np.tolist()
+                del(emb_np)
+                log.debug(f"batch dataset size: {len(all_embeddings)}, {len(all_metadata)}")
 
-            num_conc_batches = math.ceil(len(all_embeddings)/NUM_PER_BATCH)
-            log.info(f"({mp.current_process().name:16}) Start inserting {len(all_embeddings)} embeddings in batch {NUM_PER_BATCH}")
-            count = 0
-            for batch_id in range(self.seq_batches):
-                metadata = all_metadata[batch_id*NUM_PER_BATCH: (batch_id+1)*NUM_PER_BATCH]
-                embeddings = all_embeddings[batch_id*NUM_PER_BATCH: (batch_id+1)*NUM_PER_BATCH]
-
-                log.debug(f"({mp.current_process().name:16}) batch [{batch_id:3}/{num_conc_batches}], Start inserting {len(metadata)} embeddings")
+                last_batch = self.dataset.data.size - count == len(all_metadata)
                 insert_count, error = self.db.insert_embeddings(
-                    embeddings=embeddings,
-                    metadata=metadata,
+                    embeddings=all_embeddings,
+                    metadata=all_metadata,
+                    last_batch=last_batch,
                 )
-                if error != None:
+                if error is not None:
                     raise error
-                log.debug(f"({mp.current_process().name:16}) batch [{batch_id:3}/{num_conc_batches}], Finish inserting {len(metadata)} embeddings")
 
-                assert insert_count == len(metadata)
+                assert insert_count == len(all_metadata)
                 count += insert_count
-            log.info(f"({mp.current_process().name:16}) Finish inserting {len(all_embeddings)} embeddings in batch {NUM_PER_BATCH}")
-        return count
+                if count % 100_000 == 0:
+                    log.info(f"({mp.current_process().name:16}) Loaded {count} embeddings into VectorDB")
 
-    def endless_insert_data(self, left_id: int = 0) -> int:
-        with self.db.init():
-            all_embeddings = self.shared_emb
+            log.info(f"({mp.current_process().name:16}) Finish loading all dataset into VectorDB, dur={time.perf_counter()-start}")
+            return count
 
+    def endless_insert_data(self, all_embeddings, all_metadata, left_id: int = 0) -> int:
+        with self.db.init():
             # unique id for endlessness insertion
-            all_metadata = [i+left_id for i in self.train_id]
+            all_metadata = [i+left_id for i in all_metadata]
 
-            num_conc_batches = math.ceil(len(all_embeddings)/NUM_PER_BATCH)
+            NUM_BATCHES = math.ceil(len(all_embeddings)/NUM_PER_BATCH)
             log.info(f"({mp.current_process().name:16}) Start inserting {len(all_embeddings)} embeddings in batch {NUM_PER_BATCH}")
             count = 0
-            for batch_id in range(self.seq_batches):
+            for batch_id in range(NUM_BATCHES):
                 retry_count = 0
                 already_insert_count = 0
                 metadata = all_metadata[batch_id*NUM_PER_BATCH : (batch_id+1)*NUM_PER_BATCH]
                 embeddings = all_embeddings[batch_id*NUM_PER_BATCH : (batch_id+1)*NUM_PER_BATCH]
 
-                log.debug(f"({mp.current_process().name:16}) batch [{batch_id:3}/{num_conc_batches}], Start inserting {len(metadata)} embeddings")
+                log.debug(f"({mp.current_process().name:16}) batch [{batch_id:3}/{NUM_BATCHES}], Start inserting {len(metadata)} embeddings")
                 while retry_count < LOAD_MAX_TRY_COUNT:
-                    previous_beg, current_beg = 0, 0
                     insert_count, error = self.db.insert_embeddings(
                         embeddings=embeddings[already_insert_count :],
                         metadata=metadata[already_insert_count :],
                     )
                     already_insert_count += insert_count
-                    if error != None:
+                    if error is not None:
                         retry_count += 1
                         time.sleep(WAITTING_TIME)
-                       
+
                         log.info(f"Failed to insert data, try {retry_count} time")
                         if retry_count >= LOAD_MAX_TRY_COUNT:
                             raise error
                     else:
                         break
-                log.debug(f"({mp.current_process().name:16}) batch [{batch_id:3}/{num_conc_batches}], Finish inserting {len(metadata)} embeddings")
+                log.debug(f"({mp.current_process().name:16}) batch [{batch_id:3}/{NUM_BATCHES}], Finish inserting {len(metadata)} embeddings")
 
                 assert already_insert_count == len(metadata)
                 count += already_insert_count
             log.info(f"({mp.current_process().name:16}) Finish inserting {len(all_embeddings)} embeddings in batch {NUM_PER_BATCH}")
         return count
 
     @utils.time_it
     def _insert_all_batches(self) -> int:
         """Performance case only"""
         with concurrent.futures.ProcessPoolExecutor(mp_context=mp.get_context('spawn'), max_workers=1) as executor:
-            future = executor.submit(self.insert_data)
-            count = future.result()
-            return count
+            future = executor.submit(self.task)
+            try:
+                count = future.result(timeout=self.timeout)
+            except TimeoutError as e:
+                msg = f"VectorDB load dataset timeout in {self.timeout}"
+                log.warning(msg)
+                for pid, _ in executor._processes.items():
+                    psutil.Process(pid).kill()
+                raise PerformanceTimeoutError(msg) from e
+            except Exception as e:
+                log.warning(f"VectorDB load dataset error: {e}")
+                raise e from e
+            else:
+                return count
 
     def run_endlessness(self) -> int:
         """run forever util DB raises exception or crash"""
+        # datasets for load tests are quite small, can fit into memory
+        # only 1 file
+        data_df = [data_df for data_df in self.dataset][0]
+        all_embeddings, all_metadata = np.stack(data_df["emb"]).tolist(), data_df['id'].tolist()
+
         start_time = time.perf_counter()
         max_load_count, times = 0, 0
         try:
             with self.db.init():
                 self.db.ready_to_load()
-            while time.perf_counter() - start_time < config.CASE_TIMEOUT_IN_SECOND:
-                count = self.endless_insert_data(left_id=max_load_count)
+            while time.perf_counter() - start_time < self.timeout:
+                count = self.endless_insert_data(all_embeddings, all_metadata, left_id=max_load_count)
                 max_load_count += count
                 times += 1
                 log.info(f"Loaded {times} entire dataset, current max load counts={utils.numerize(max_load_count)}, {max_load_count}")
-            raise LoadTimeoutError("capacity case load timeout and stop")
-        except LoadTimeoutError as e:
-            log.info("load timetout, stop the load case")
-            raise e from None
         except Exception as e:
             log.info(f"Capacity case load reach limit, insertion counts={utils.numerize(max_load_count)}, {max_load_count}, err={e}")
             traceback.print_exc()
             return max_load_count
+        else:
+            msg = f"capacity case load timeout in {self.timeout}s"
+            log.info(msg)
+            raise LoadTimeoutError(msg)
 
     def run(self) -> int:
         count, dur = self._insert_all_batches()
         return count
 
 
 class SerialSearchRunner:
@@ -153,15 +171,15 @@
 
     def search(self, args: tuple[list, pd.DataFrame]):
         log.info(f"{mp.current_process().name:14} start search the entire test_data to get recall and latency")
         with self.db.init():
             test_data, ground_truth = args
 
             log.debug(f"test dataset size: {len(test_data)}")
-            log.info(f"ground truth size: {ground_truth.columns}, shape: {ground_truth.shape}")
+            log.debug(f"ground truth size: {ground_truth.columns}, shape: {ground_truth.shape}")
 
             latencies, recalls = [], []
             for idx, emb in enumerate(test_data):
                 s = time.perf_counter()
                 try:
                     results = self.db.search_embedding(
                         emb,
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/task_runner.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/task_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
+import psutil
 import traceback
 import concurrent
 import numpy as np
 from enum import Enum, auto
 
 from . import utils
 from .cases import Case, CaseLabel
 from ..base import BaseModel
-from ..models import TaskConfig
+from ..models import TaskConfig, PerformanceTimeoutError
 
 from .clients import (
     api,
     ZillizCloud,
     Milvus,
     MetricType
 )
@@ -88,88 +89,78 @@
             log.warning(f"pre run case error: {e}")
             raise e from None
 
     def run(self, drop_old: bool = True) -> Metric:
         self._pre_run(drop_old)
 
         if self.ca.label == CaseLabel.Load:
-            return self._run_load_case()
+            return self._run_capacity_case()
         elif self.ca.label == CaseLabel.Performance:
             return self._run_perf_case(drop_old)
         else:
-            log.warning(f"unknown case type: {self.ca.label}")
-            raise ValueError(f"Unknown case type: {self.ca.label}")
+            msg = f"unknown case type: {self.ca.label}"
+            log.warning(msg)
+            raise ValueError(msg)
 
-
-    def _run_load_case(self) -> Metric:
-        """ run load cases
+    def _run_capacity_case(self) -> Metric:
+        """ run capacity cases
 
         Returns:
             Metric: the max load count
         """
         log.info("Start capacity case")
-        # datasets for load tests are quite small, can fit into memory
-        # only 1 file
-        data_df = [data_df for data_df in self.ca.dataset][0]
-
-        all_embeddings, all_metadata = np.stack(data_df["emb"]).tolist(), data_df['id'].tolist()
-        runner = SerialInsertRunner(self.db, all_embeddings, all_metadata)
         try:
+            runner = SerialInsertRunner(self.db, self.ca.dataset, self.normalize, self.ca.load_timeout)
             count = runner.run_endlessness()
-            log.info(f"load reach limit: insertion counts={count}")
-            return Metric(max_load_count=count)
         except Exception as e:
-            log.warning(f"run capacity case error: {e}")
+            log.warning(f"Failed to run capacity case, reason = {e}")
             raise e from None
-        log.info("End capacity case")
-
+        else:
+            log.info(f"Capacity case loading dataset reaches VectorDB's limit: max capacity = {count}")
+            return Metric(max_load_count=count)
 
     def _run_perf_case(self, drop_old: bool = True) -> Metric:
+        """ run performance cases
+
+        Returns:
+            Metric: load_duration, recall, serial_latency_p99, and, qps
+        """
         try:
             m = Metric()
             if drop_old:
                 _, load_dur = self._load_train_data()
                 build_dur = self._optimize()
                 m.load_duration = round(load_dur+build_dur, 4)
+                log.info(
+                    f"Finish loading the entire dataset into VectorDB,"
+                    f" insert_duration={load_dur}, optimize_duration={build_dur}"
+                    f" load_duration(insert + optimize) = {m.load_duration}"
+                )
 
             self._init_search_runner()
             m.recall, m.serial_latency_p99 = self._serial_search()
             m.qps = self._conc_search()
-
-            log.info(f"got results: {m}")
-            return m
         except Exception as e:
-            log.warning(f"performance case run error: {e}")
+            log.warning(f"Failed to run performance case, reason = {e}")
             traceback.print_exc()
-            raise e
+            raise e from None
+        else:
+            log.info(f"Performance case got result: {m}")
+            return m
 
     @utils.time_it
     def _load_train_data(self):
         """Insert train data and get the insert_duration"""
-        for data_df in self.ca.dataset:
-            try:
-                all_metadata = data_df['id'].tolist()
-
-                emb_np = np.stack(data_df['emb'])
-                if self.normalize:
-                    log.debug("normalize the 100k train data")
-                    all_embeddings = emb_np / np.linalg.norm(emb_np, axis=1)[:, np.newaxis].tolist()
-                else:
-                    all_embeddings = emb_np.tolist()
-
-                del(emb_np)
-                log.debug(f"normalized size: {len(all_embeddings)}, {len(all_metadata)}")
-
-                runner = SerialInsertRunner(self.db, all_embeddings, all_metadata)
-                runner.run()
-            except Exception as e:
-                raise e from None
-            finally:
-                runner = None
-
+        try:
+            runner = SerialInsertRunner(self.db, self.ca.dataset, self.normalize, self.ca.load_timeout)
+            runner.run()
+        except Exception as e:
+            raise e from None
+        finally:
+            runner = None
 
     def _serial_search(self) -> tuple[float, float]:
         """Performance serial tests, search the entire test data once,
         calculate the recall, serial_latency_p99
 
         Returns:
             tuple[float, float]: recall, serial_latency_p99
@@ -194,25 +185,29 @@
             log.warning(f"search error: {str(e)}, {e}")
             raise e from None
         finally:
             self.stop()
 
     @utils.time_it
     def _task(self) -> None:
-        """"""
         with self.db.init():
-            self.db.ready_to_search()
+            self.db.optimize()
 
     def _optimize(self) -> float:
         with concurrent.futures.ProcessPoolExecutor(max_workers=1) as executor:
             future = executor.submit(self._task)
             try:
-                return future.result()[1]
+                return future.result(timeout=self.ca.optimize_timeout)[1]
+            except TimeoutError as e:
+                log.warning(f"VectorDB optimize timeout in {self.ca.optimize_timeout}")
+                for pid, _ in executor._processes.items():
+                    psutil.Process(pid).kill()
+                raise PerformanceTimeoutError("Performance case optimize timeout") from e
             except Exception as e:
-                log.warning(f"VectorDB ready_to_search error: {e}")
+                log.warning(f"VectorDB optimize error: {e}")
                 raise e from None
 
     def _init_search_runner(self):
         test_emb = np.stack(self.ca.dataset.test_data["emb"])
         if self.normalize:
             test_emb = test_emb / np.linalg.norm(test_emb, axis=1)[:, np.newaxis]
         self.test_emb = test_emb
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/backend/utils.py` & `vectordb-bench-0.0.3/vectordb_bench/backend/utils.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/charts.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/charts.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/data.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/data.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/expanderStyle.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/expanderStyle.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/filters.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/filters.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/nav.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/nav.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/priceTable.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/components/check_results/priceTable.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/components/get_results/saveAsImage.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/components/get_results/saveAsImage.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,21 +28,23 @@
 
 const streamlitDoc = window.parent.document;
 const stApp = streamlitDoc.querySelector('.main > .block-container');
 
 const buttons = Array.from(streamlitDoc.querySelectorAll('.stButton > button'));
 const imgButton = buttons.find(el => el.innerText === '{buttonText}');
 
-imgButton.innerText = 'Creating Image...';
+if (imgButton)
+    imgButton.innerText = 'Creating Image...';
 
 html2canvas(stApp, {{ allowTaint: false, useCORS: true }}).then(function (canvas) {{
     a = document.createElement('a');
     a.href = canvas.toDataURL("image/jpeg", 1.0).replace("image/jpeg", "image/octet-stream");
     a.download = '{pageName}.png';
     a.click();
     
-    imgButton.innerText = '{buttonText}';
+    if (imgButton)
+        imgButton.innerText = '{buttonText}';
 }})
 </script>""",
             height=0,
             width=0,
         )
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/caseSelector.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/components/run_test/caseSelector.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/dbConfigSetting.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/components/run_test/dbConfigSetting.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/dbSelector.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/components/run_test/dbSelector.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/generateTasks.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/components/run_test/generateTasks.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/submitTask.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/components/run_test/submitTask.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/const/dbCaseConfigs.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/const/dbCaseConfigs.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     DIVIDER,
     CaseType.CapacityDim960,
     CaseType.CapacityDim128,
 ]
 
 CASE_LIST = [item for item in CASE_LIST_WITH_DIVIDER if isinstance(item, CaseType)]
 
+
 class InputType(IntEnum):
     Text = 20001
     Number = 20002
     Option = 20003
 
 
 class CaseConfigInput(BaseModel):
@@ -181,52 +182,71 @@
         "max": 65536,
         "value": 10,
     },
     isDisplayed=lambda config: config.get(CaseConfigParamType.IndexType, None)
     == IndexType.IVFFlat.value,
 )
 
+CaseConfigParamInput_Lists = CaseConfigInput(
+    label=CaseConfigParamType.lists,
+    inputType=InputType.Number,
+    inputConfig={
+        "min": 1,
+        "max": 65536,
+        "value": 10,
+    },
+)
+
+CaseConfigParamInput_Probes = CaseConfigInput(
+    label=CaseConfigParamType.probes,
+    inputType=InputType.Number,
+    inputConfig={
+        "min": 1,
+        "max": 65536,
+        "value": 1,
+    },
+)
+
 
 MilvusLoadConfig = [
     CaseConfigParamInput_IndexType,
     CaseConfigParamInput_M,
     CaseConfigParamInput_EFConstruction_Milvus,
     CaseConfigParamInput_Nlist,
 ]
-
-
 MilvusPerformanceConfig = [
     CaseConfigParamInput_IndexType,
     CaseConfigParamInput_M,
     CaseConfigParamInput_EFConstruction_Milvus,
     CaseConfigParamInput_EF_Milvus,
     CaseConfigParamInput_SearchList,
     CaseConfigParamInput_Nlist,
     CaseConfigParamInput_Nprobe,
 ]
 
 WeaviateLoadConfig = [
     CaseConfigParamInput_MaxConnections,
     CaseConfigParamInput_EFConstruction_Weaviate,
 ]
-
 WeaviatePerformanceConfig = [
     CaseConfigParamInput_MaxConnections,
     CaseConfigParamInput_EFConstruction_Weaviate,
     CaseConfigParamInput_EF_Weaviate,
 ]
 
 ESLoadingConfig = [CaseConfigParamInput_EFConstruction_ES, CaseConfigParamInput_M_ES]
-
 ESPerformanceConfig = [
     CaseConfigParamInput_EFConstruction_ES,
     CaseConfigParamInput_M_ES,
     CaseConfigParamInput_NumCandidates_ES,
 ]
 
+PgVectorLoadingConfig = [CaseConfigParamInput_Lists]
+PgVectorPerformanceConfig = [CaseConfigParamInput_Lists, CaseConfigParamInput_Probes]
+
 CASE_CONFIG_MAP = {
     DB.Milvus: {
         CaseType.CapacityDim960: MilvusLoadConfig,
         CaseType.CapacityDim128: MilvusLoadConfig,
         CaseType.Performance100M: MilvusPerformanceConfig,
         CaseType.Performance10M: MilvusPerformanceConfig,
         CaseType.Performance1M: MilvusPerformanceConfig,
@@ -253,8 +273,19 @@
         CaseType.Performance10M: ESPerformanceConfig,
         CaseType.Performance1M: ESPerformanceConfig,
         CaseType.Performance10M1P: ESPerformanceConfig,
         CaseType.Performance1M1P: ESPerformanceConfig,
         CaseType.Performance10M99P: ESPerformanceConfig,
         CaseType.Performance1M99P: ESPerformanceConfig,
     },
+    DB.PgVector: {
+        CaseType.CapacityDim960: PgVectorLoadingConfig,
+        CaseType.CapacityDim128: PgVectorLoadingConfig,
+        CaseType.Performance100M: PgVectorPerformanceConfig,
+        CaseType.Performance10M: PgVectorPerformanceConfig,
+        CaseType.Performance1M: PgVectorPerformanceConfig,
+        CaseType.Performance10M1P: PgVectorPerformanceConfig,
+        CaseType.Performance1M1P: PgVectorPerformanceConfig,
+        CaseType.Performance10M99P: PgVectorPerformanceConfig,
+        CaseType.Performance1M99P: PgVectorPerformanceConfig,
+    },
 }
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/const/dbPrices.py` & `vectordb-bench-0.0.3/vectordb_bench/results/dbPrices.json`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,36 @@
-00000000: 6672 6f6d 2076 6563 746f 7264 625f 6265  from vectordb_be
-00000010: 6e63 682e 6261 636b 656e 642e 636c 6965  nch.backend.clie
-00000020: 6e74 7320 696d 706f 7274 2044 420a 0a0a  nts import DB...
-00000030: 4442 5f44 424c 4142 454c 5f54 4f5f 5052  DB_DBLABEL_TO_PR
-00000040: 4943 4520 3d20 7b0a 2020 2020 4442 2e4d  ICE = {.    DB.M
-00000050: 696c 7675 732e 7661 6c75 653a 207b 7d2c  ilvus.value: {},
-00000060: 0a20 2020 2044 422e 5a69 6c6c 697a 436c  .    DB.ZillizCl
-00000070: 6f75 642e 7661 6c75 653a 207b 0a20 2020  oud.value: {.   
-00000080: 2020 2020 2022 3163 752d 7065 7266 223a       "1cu-perf":
-00000090: 2030 2e31 3539 2c0a 2020 2020 2020 2020   0.159,.        
-000000a0: 2238 6375 2d70 6572 6622 3a20 312e 3237  "8cu-perf": 1.27
-000000b0: 322c 0a20 2020 2020 2020 2022 3163 752d  2,.        "1cu-
-000000c0: 6361 7022 3a20 302e 3135 392c 0a20 2020  cap": 0.159,.   
-000000d0: 2020 2020 2022 3263 752d 6361 7022 3a20       "2cu-cap": 
-000000e0: 302e 3331 382c 0a20 2020 207d 2c0a 2020  0.318,.    },.  
-000000f0: 2020 4442 2e57 6561 7669 6174 6543 6c6f    DB.WeaviateClo
-00000100: 7564 2e76 616c 7565 3a20 7b0a 2020 2020  ud.value: {.    
-00000110: 2020 2020 2320 2273 616e 646f 7822 3a20      # "sandox": 
-00000120: 302c 0a20 2020 2020 2020 2022 7374 616e  0,.        "stan
-00000130: 6461 7264 223a 2031 302e 3130 2c0a 2020  dard": 10.10,.  
-00000140: 2020 2020 2020 2262 7573 5f63 7269 7422        "bus_crit"
-00000150: 3a20 3332 2e36 302c 0a20 2020 207d 2c0a  : 32.60,.    },.
-00000160: 2020 2020 4442 2e45 6c61 7374 6963 436c      DB.ElasticCl
-00000170: 6f75 642e 7661 6c75 653a 207b 0a20 2020  oud.value: {.   
-00000180: 2020 2020 2022 7570 546f 322e 3563 3867       "upTo2.5c8g
-00000190: 223a 2030 2e34 3739 332c 0a20 2020 207d  ": 0.4793,.    }
-000001a0: 2c0a 2020 2020 4442 2e51 6472 616e 7443  ,.    DB.QdrantC
-000001b0: 6c6f 7564 2e76 616c 7565 3a20 7b0a 2020  loud.value: {.  
-000001c0: 2020 2020 2020 2230 2e35 6334 672d 316e        "0.5c4g-1n
-000001d0: 6f64 6522 3a20 302e 3035 322c 0a20 2020  ode": 0.052,.   
-000001e0: 2020 2020 2022 3263 3867 2d31 6e6f 6465       "2c8g-1node
-000001f0: 223a 2030 2e31 3636 2c0a 2020 2020 2020  ": 0.166,.      
-00000200: 2020 2234 6331 3667 2d35 6e6f 6465 223a    "4c16g-5node":
-00000210: 2031 2e34 3236 2c0a 2020 2020 7d2c 0a20   1.426,.    },. 
-00000220: 2020 2044 422e 5069 6e65 636f 6e65 2e76     DB.Pinecone.v
-00000230: 616c 7565 3a20 7b0a 2020 2020 2020 2020  alue: {.        
-00000240: 2273 312e 7831 223a 2030 2e30 3937 332c  "s1.x1": 0.0973,
-00000250: 0a20 2020 2020 2020 2022 7331 2e78 3222  .        "s1.x2"
-00000260: 3a20 302e 3139 342c 0a20 2020 2020 2020  : 0.194,.       
-00000270: 2022 7031 2e78 3122 3a20 302e 3039 3733   "p1.x1": 0.0973
-00000280: 2c0a 2020 2020 2020 2020 2270 322e 7831  ,.        "p2.x1
-00000290: 223a 2030 2e31 3436 2c0a 2020 2020 2020  ": 0.146,.      
-000002a0: 2020 2270 322e 7831 2d38 6e6f 6465 223a    "p2.x1-8node":
-000002b0: 2031 2e31 3638 2c0a 2020 2020 2020 2020   1.168,.        
-000002c0: 2270 312e 7831 2d38 6e6f 6465 223a 2030  "p1.x1-8node": 0
-000002d0: 2e37 3739 2c0a 2020 2020 2020 2020 2273  .779,.        "s
-000002e0: 312e 7831 2d32 6e6f 6465 223a 2030 2e31  1.x1-2node": 0.1
-000002f0: 3935 2c0a 2020 2020 7d2c 0a7d 0a         95,.    },.}.
+00000000: 7b0a 2020 224d 696c 7675 7322 3a20 7b7d  {.  "Milvus": {}
+00000010: 2c0a 2020 225a 696c 6c69 7a43 6c6f 7564  ,.  "ZillizCloud
+00000020: 223a 207b 0a20 2020 2022 3163 752d 7065  ": {.    "1cu-pe
+00000030: 7266 223a 2030 2e31 3539 2c0a 2020 2020  rf": 0.159,.    
+00000040: 2238 6375 2d70 6572 6622 3a20 312e 3237  "8cu-perf": 1.27
+00000050: 322c 0a20 2020 2022 3163 752d 6361 7022  2,.    "1cu-cap"
+00000060: 3a20 302e 3135 392c 0a20 2020 2022 3263  : 0.159,.    "2c
+00000070: 752d 6361 7022 3a20 302e 3331 380a 2020  u-cap": 0.318.  
+00000080: 7d2c 0a20 2022 5765 6176 6961 7465 436c  },.  "WeaviateCl
+00000090: 6f75 6422 3a20 7b0a 2020 2020 2273 7461  oud": {.    "sta
+000000a0: 6e64 6172 6422 3a20 3130 2e31 2c0a 2020  ndard": 10.1,.  
+000000b0: 2020 2262 7573 5f63 7269 7422 3a20 3332    "bus_crit": 32
+000000c0: 2e36 0a20 207d 2c0a 2020 2245 6c61 7374  .6.  },.  "Elast
+000000d0: 6963 436c 6f75 6422 3a20 7b0a 2020 2020  icCloud": {.    
+000000e0: 2275 7054 6f32 2e35 6338 6722 3a20 302e  "upTo2.5c8g": 0.
+000000f0: 3437 3933 0a20 207d 2c0a 2020 2251 6472  4793.  },.  "Qdr
+00000100: 616e 7443 6c6f 7564 223a 207b 0a20 2020  antCloud": {.   
+00000110: 2022 302e 3563 3467 2d31 6e6f 6465 223a   "0.5c4g-1node":
+00000120: 2030 2e30 3532 2c0a 2020 2020 2232 6338   0.052,.    "2c8
+00000130: 672d 316e 6f64 6522 3a20 302e 3136 362c  g-1node": 0.166,
+00000140: 0a20 2020 2022 3463 3136 672d 316e 6f64  .    "4c16g-1nod
+00000150: 6522 3a20 302e 3238 3532 2c0a 2020 2020  e": 0.2852,.    
+00000160: 2234 6331 3667 2d35 6e6f 6465 223a 2031  "4c16g-5node": 1
+00000170: 2e34 3236 0a20 207d 2c0a 2020 2250 696e  .426.  },.  "Pin
+00000180: 6563 6f6e 6522 3a20 7b0a 2020 2020 2273  econe": {.    "s
+00000190: 312e 7831 223a 2030 2e30 3937 332c 0a20  1.x1": 0.0973,. 
+000001a0: 2020 2022 7331 2e78 3222 3a20 302e 3139     "s1.x2": 0.19
+000001b0: 342c 0a20 2020 2022 7031 2e78 3122 3a20  4,.    "p1.x1": 
+000001c0: 302e 3039 3733 2c0a 2020 2020 2270 322e  0.0973,.    "p2.
+000001d0: 7831 223a 2030 2e31 3436 2c0a 2020 2020  x1": 0.146,.    
+000001e0: 2270 322e 7831 2d38 6e6f 6465 223a 2031  "p2.x1-8node": 1
+000001f0: 2e31 3638 2c0a 2020 2020 2270 312e 7831  .168,.    "p1.x1
+00000200: 2d38 6e6f 6465 223a 2030 2e37 3739 2c0a  -8node": 0.779,.
+00000210: 2020 2020 2273 312e 7831 2d32 6e6f 6465      "s1.x1-2node
+00000220: 223a 2030 2e31 3935 0a20 207d 2c0a 2020  ": 0.195.  },.  
+00000230: 2250 6756 6563 746f 7222 3a20 7b7d 0a7d  "PgVector": {}.}
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/const/styles.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/const/styles.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,25 +28,31 @@
 MAX_AUTO_REFRESH_COUNT = 999999
 MAX_AUTO_REFRESH_INTERVAL = 5000  # 5s
 
 PAGE_TITLE = "VectorDB Benchmark"
 FAVICON = "https://assets.zilliz.com/favicon_f7f922fe27.png"
 HEADER_ICON = "https://assets.zilliz.com/vdb_benchmark_db790b5387.png"
 
+# RedisCloud icon: https://assets.zilliz.com/Redis_Cloud_74b8bfef39.png
+# Elasticsearch icon: https://assets.zilliz.com/elasticsearch_beffeadc29.png
+# Chroma icon: https://assets.zilliz.com/chroma_ceb3f06ed7.png
 DB_TO_ICON = {
     DB.Milvus: "https://assets.zilliz.com/milvus_c30b0d1994.png",
     DB.ZillizCloud: "https://assets.zilliz.com/zilliz_5f4cc9b050.png",
-    DB.ElasticCloud: "https://assets.zilliz.com/elasticsearch_beffeadc29.png",
+    DB.ElasticCloud: "https://assets.zilliz.com/Elatic_Cloud_dad8d6a3a3.png",
     DB.Pinecone: "https://assets.zilliz.com/pinecone_94d8154979.png",
     DB.QdrantCloud: "https://assets.zilliz.com/qdrant_b691674fcd.png",
     DB.WeaviateCloud: "https://assets.zilliz.com/weaviate_4f6f171ebe.png",
+    DB.PgVector: "https://assets.zilliz.com/PG_Vector_d464f2ef5f.png",
 }
 
-
+# RedisCloud color: #0D6EFD
+# Chroma color: #FFC107
 COLOR_MAP = {
     DB.Milvus.value: "#0DCAF0",
     DB.ZillizCloud.value: "#0D6EFD",
-    DB.ElasticCloud.value: "#fdc613",
+    DB.ElasticCloud.value: "#04D6C8",
     DB.Pinecone.value: "#6610F2",
     DB.QdrantCloud.value: "#D91AD9",
     DB.WeaviateCloud.value: "#20C997",
+    DB.PgVector.value: "#4C779A",
 }
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/pages/quries_per_dollar.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/pages/quries_per_dollar.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/pages/run_test.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/pages/run_test.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/frontend/vdb_benchmark.py` & `vectordb-bench-0.0.3/vectordb_bench/frontend/vdb_benchmark.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/interface.py` & `vectordb-bench-0.0.3/vectordb_bench/interface.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/log_util.py` & `vectordb-bench-0.0.3/vectordb_bench/log_util.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.2/vectordb_bench/metric.py` & `vectordb-bench-0.0.3/vectordb_bench/metric.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     max_load_count: int = 0
 
     # for performance cases
     load_duration: float = 0.0  # duration to load all dataset into DB
     qps: float = 0.0
     serial_latency_p99: float = 0.0
     recall: float = 0.0
-    quries_per_dollar: float = 0.0
 
 
 QURIES_PER_DOLLAR_METRIC = "QP$ (Quries per Dollar)"
 LOAD_DURATION_METRIC = "load_duration"
 SERIAL_LATENCY_P99_METRIC = "serial_latency_p99"
 MAX_LOAD_COUNT_METRIC = "max_load_count"
 QPS_METRIC = "qps"
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/models.py` & `vectordb-bench-0.0.3/vectordb_bench/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     EFConstruction = "efConstruction"
     EF = "ef"
     SearchList = "search_list"
     Nlist = "nlist"
     Nprobe = "nprobe"
     MaxConnections = "maxConnections"
     numCandidates = "num_candidates"
+    lists = "lists"
+    probes = "probes"
 
 
 class CustomizedCase(BaseModel):
     pass
 
 
 class CaseConfig(BaseModel):
@@ -163,28 +165,29 @@
         max_db = max(map(len, [f.task_config.db.name for f in filtered_results]))
         max_db_labels = max(map(len, [f.task_config.db_config.db_label for f in filtered_results])) + 3
         max_case = max(map(len, [f.task_config.case_config.case_id.name for f in filtered_results]))
         max_load_dur = max(map(len, [str(f.metrics.load_duration) for f in filtered_results])) + 3
         max_qps = max(map(len, [str(f.metrics.qps) for f in filtered_results])) + 3
         max_recall = max(map(len, [str(f.metrics.recall) for f in filtered_results])) + 3
 
-        max_db_labels = 8 if max_db_labels == 0 else max_db_labels
-        max_load_dur = 11 if max_load_dur == 0 else max_load_dur + 3
-        max_qps = 10 if max_qps == 0 else max_load_dur + 3
-        max_recall = 13 if max_recall == 0 else max_recall + 3
+        max_db_labels = 8 if max_db_labels < 8 else max_db_labels
+        max_load_dur = 11 if max_load_dur < 11 else max_load_dur
+        max_qps = 10 if max_qps < 10 else max_qps
+        max_recall = 13 if max_recall < 13 else max_recall
 
-        LENGTH = (max_db, max_db_labels, max_case, len(self.task_label), max_load_dur, max_qps, 15, max_recall, 14)
+        LENGTH = (max_db, max_db_labels, max_case, len(self.task_label), max_load_dur, max_qps, 15, max_recall, 14, 5)
 
         DATA_FORMAT = (
-            f"%-{max_db}s | %-{max_db_labels}s %-{max_case}s %-{len(self.task_label)}s "
-            f"| %-{max_load_dur}s %-{max_qps}s %-15s %-{max_recall}s %-14s"
+            f"%-{max_db}s | %-{max_db_labels}s %-{max_case}s %-{len(self.task_label)}s"
+            f" | %-{max_load_dur}s %-{max_qps}s %-15s %-{max_recall}s %-14s"
+            f" | %-5s"
         )
 
         TITLE = DATA_FORMAT % (
-            "DB", "db_label", "case", "label", "load_dur", "qps", "latency(p99)", "recall", "max_load_count")
+            "DB", "db_label", "case", "label", "load_dur", "qps", "latency(p99)", "recall", "max_load_count", "label")
         SPLIT = DATA_FORMAT%tuple(map(lambda x:"-"*x, LENGTH))
         SUMMERY_FORMAT = ("Task summery: run_id=%s, task_label=%s") % (self.run_id[:5], self.task_label)
         fmt = [SUMMERY_FORMAT, TITLE, SPLIT]
 
 
         for f in filtered_results:
             fmt.append(DATA_FORMAT%(
@@ -193,12 +196,13 @@
                 f.task_config.case_config.case_id.name,
                 self.task_label,
                 f.metrics.load_duration,
                 f.metrics.qps,
                 f.metrics.serial_latency_p99,
                 f.metrics.recall,
                 f.metrics.max_load_count,
+                f.label.value,
             ))
 
         tmp_logger = logging.getLogger("no_color")
         for f in fmt:
             tmp_logger.info(f)
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench/results/result_20230609_standard.json` & `vectordb-bench-0.0.3/vectordb_bench/results/result_20230705_standard.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9789596688034189%*

 * *Differences: {"'results'": "{8: {'metrics': {'load_duration': 6003.7507, 'qps': 100.6667, 'serial_latency_p99': "*

 * *              "0.0211, 'recall': 0.9909}}, 9: {'metrics': {'load_duration': 6003.7507, 'qps': "*

 * *              "101.1399, 'serial_latency_p99': 0.0197, 'recall': 0.9907}}, 10: {'metrics': "*

 * *              "{'load_duration': 6003.7507, 'qps': 52.2606, 'serial_latency_p99': 0.0183}}, 14: "*

 * *              "{'metrics': {'load_duration': 18790.8759, 'qps': 61.0661, 'serial_latency_p99': "*

 * *              "0.0498, 'rec […]*

```diff
@@ -239,19 +239,19 @@
                     "password": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 5869.4929,
+                "load_duration": 6003.7507,
                 "max_load_count": 0,
-                "qps": 89.4473,
-                "recall": 0.9875,
-                "serial_latency_p99": 0.0219
+                "qps": 100.6667,
+                "recall": 0.9909,
+                "serial_latency_p99": 0.0211
             },
             "task_config": {
                 "case_config": {
                     "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "Milvus",
@@ -265,19 +265,19 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 5869.4929,
+                "load_duration": 6003.7507,
                 "max_load_count": 0,
-                "qps": 87.8616,
-                "recall": 0.9871,
-                "serial_latency_p99": 0.0215
+                "qps": 101.1399,
+                "recall": 0.9907,
+                "serial_latency_p99": 0.0197
             },
             "task_config": {
                 "case_config": {
                     "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "Milvus",
@@ -291,19 +291,19 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 5869.4929,
+                "load_duration": 6003.7507,
                 "max_load_count": 0,
-                "qps": 62.5257,
+                "qps": 52.2606,
                 "recall": 1,
-                "serial_latency_p99": 0.0261
+                "serial_latency_p99": 0.0183
             },
             "task_config": {
                 "case_config": {
                     "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "Milvus",
@@ -395,19 +395,19 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 29829.7671,
+                "load_duration": 18790.8759,
                 "max_load_count": 0,
-                "qps": 48.3866,
-                "recall": 0.9909,
-                "serial_latency_p99": 0.0443
+                "qps": 61.0661,
+                "recall": 0.9911,
+                "serial_latency_p99": 0.0498
             },
             "task_config": {
                 "case_config": {
                     "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "Milvus",
@@ -421,19 +421,19 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 29829.7671,
+                "load_duration": 18790.8759,
                 "max_load_count": 0,
-                "qps": 48.8021,
-                "recall": 0.9909,
-                "serial_latency_p99": 0.0347
+                "qps": 58.9326,
+                "recall": 0.9911,
+                "serial_latency_p99": 0.0446
             },
             "task_config": {
                 "case_config": {
                     "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "Milvus",
@@ -447,19 +447,19 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 29829.7671,
+                "load_duration": 18790.8759,
                 "max_load_count": 0,
-                "qps": 30.5848,
+                "qps": 42.5977,
                 "recall": 1,
-                "serial_latency_p99": 0.0473
+                "serial_latency_p99": 0.0549
             },
             "task_config": {
                 "case_config": {
                     "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "Milvus",
@@ -473,19 +473,19 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1455.573,
+                "load_duration": 1782.0061,
                 "max_load_count": 0,
-                "qps": 290.695,
-                "recall": 0.9801,
-                "serial_latency_p99": 0.0075
+                "qps": 536.0726,
+                "recall": 0.9728,
+                "serial_latency_p99": 0.0082
             },
             "task_config": {
                 "case_config": {
                     "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "Milvus",
@@ -501,19 +501,19 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1455.573,
+                "load_duration": 1782.0061,
                 "max_load_count": 0,
-                "qps": 284.9882,
-                "recall": 0.9803,
-                "serial_latency_p99": 0.0087
+                "qps": 467.179,
+                "recall": 0.9697,
+                "serial_latency_p99": 0.007
             },
             "task_config": {
                 "case_config": {
                     "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "Milvus",
@@ -531,17 +531,17 @@
             }
         },
         {
             "label": ":)",
             "metrics": {
                 "load_duration": 1455.573,
                 "max_load_count": 0,
-                "qps": 390.2579,
+                "qps": 431.7512,
                 "recall": 1,
-                "serial_latency_p99": 0.0073
+                "serial_latency_p99": 0.0083
             },
             "task_config": {
                 "case_config": {
                     "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "Milvus",
@@ -611,19 +611,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 3478.7882,
+                "load_duration": 2412.0463,
                 "max_load_count": 0,
-                "qps": 164.3866,
-                "recall": 0.95,
-                "serial_latency_p99": 0.0131
+                "qps": 330.0144,
+                "recall": 0.9507,
+                "serial_latency_p99": 0.009
             },
             "task_config": {
                 "case_config": {
                     "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -638,19 +638,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 3478.7882,
+                "load_duration": 2412.0463,
                 "max_load_count": 0,
-                "qps": 139.0901,
-                "recall": 0.9669,
-                "serial_latency_p99": 0.0172
+                "qps": 271.6585,
+                "recall": 0.9678,
+                "serial_latency_p99": 0.0101
             },
             "task_config": {
                 "case_config": {
                     "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -665,19 +665,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 3478.7882,
+                "load_duration": 2412.0463,
                 "max_load_count": 0,
-                "qps": 115.3193,
+                "qps": 216.5226,
                 "recall": 1,
-                "serial_latency_p99": 0.0157
+                "serial_latency_p99": 0.0129
             },
             "task_config": {
                 "case_config": {
                     "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -773,19 +773,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 14485.1106,
+                "load_duration": 14521.4008,
                 "max_load_count": 0,
-                "qps": 100.23,
-                "recall": 0.972,
-                "serial_latency_p99": 0.0288
+                "qps": 123.9553,
+                "recall": 0.971,
+                "serial_latency_p99": 0.023
             },
             "task_config": {
                 "case_config": {
                     "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -800,19 +800,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 14485.1106,
+                "load_duration": 14521.4008,
                 "max_load_count": 0,
-                "qps": 48.7675,
-                "recall": 0.9911,
-                "serial_latency_p99": 0.0352
+                "qps": 59.1479,
+                "recall": 0.9906,
+                "serial_latency_p99": 0.0445
             },
             "task_config": {
                 "case_config": {
                     "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -827,19 +827,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 14485.1106,
+                "load_duration": 14521.4008,
                 "max_load_count": 0,
-                "qps": 30.5627,
+                "qps": 40.999,
                 "recall": 1,
-                "serial_latency_p99": 0.0471
+                "serial_latency_p99": 0.0553
             },
             "task_config": {
                 "case_config": {
                     "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -854,19 +854,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 3253.6402,
+                "load_duration": 2340.5671,
                 "max_load_count": 0,
-                "qps": 352.1345,
+                "qps": 579.9416,
                 "recall": 0.9213,
-                "serial_latency_p99": 0.0093
+                "serial_latency_p99": 0.0094
             },
             "task_config": {
                 "case_config": {
                     "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -881,19 +881,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 3253.6402,
+                "load_duration": 2340.5671,
                 "max_load_count": 0,
-                "qps": 264.539,
-                "recall": 0.9684,
-                "serial_latency_p99": 0.0099
+                "qps": 425.2529,
+                "recall": 0.9686,
+                "serial_latency_p99": 0.0113
             },
             "task_config": {
                 "case_config": {
                     "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -908,19 +908,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 3253.6402,
+                "load_duration": 2340.5671,
                 "max_load_count": 0,
-                "qps": 232.8041,
+                "qps": 397.0539,
                 "recall": 1,
-                "serial_latency_p99": 0.0109
+                "serial_latency_p99": 0.0138
             },
             "task_config": {
                 "case_config": {
                     "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -1661,19 +1661,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1165.833,
+                "load_duration": 1100.6681,
                 "max_load_count": 0,
-                "qps": 457.3331,
-                "recall": 0.9473,
-                "serial_latency_p99": 0.0056
+                "qps": 516.27,
+                "recall": 0.9463,
+                "serial_latency_p99": 0.007
             },
             "task_config": {
                 "case_config": {
                     "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -1688,19 +1688,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1165.833,
+                "load_duration": 1100.6681,
                 "max_load_count": 0,
-                "qps": 308.5526,
-                "recall": 0.9805,
-                "serial_latency_p99": 0.0077
+                "qps": 354.8416,
+                "recall": 0.9802,
+                "serial_latency_p99": 0.01
             },
             "task_config": {
                 "case_config": {
                     "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -1715,19 +1715,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1165.833,
+                "load_duration": 1100.6681,
                 "max_load_count": 0,
-                "qps": 408.1209,
+                "qps": 427.5229,
                 "recall": 1,
-                "serial_latency_p99": 0.0057
+                "serial_latency_p99": 0.0087
             },
             "task_config": {
                 "case_config": {
                     "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -1823,19 +1823,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1229.3664,
+                "load_duration": 1575.253,
                 "max_load_count": 0,
-                "qps": 2867.9092,
-                "recall": 0.8769,
-                "serial_latency_p99": 0.0037
+                "qps": 2884.689,
+                "recall": 0.8801,
+                "serial_latency_p99": 0.0053
             },
             "task_config": {
                 "case_config": {
                     "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -1850,19 +1850,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1229.3664,
+                "load_duration": 1853.989,
                 "max_load_count": 0,
                 "qps": 1689.5799,
-                "recall": 0.9486,
-                "serial_latency_p99": 0.0054
+                "recall": 0.9493,
+                "serial_latency_p99": 0.0066
             },
             "task_config": {
                 "case_config": {
                     "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -1877,19 +1877,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1229.3664,
+                "load_duration": 1575.253,
                 "max_load_count": 0,
-                "qps": 1371.0535,
+                "qps": 1517.6792,
                 "recall": 1,
-                "serial_latency_p99": 0.0079
+                "serial_latency_p99": 0.01
             },
             "task_config": {
                 "case_config": {
                     "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -1904,19 +1904,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 7772.641,
+                "load_duration": 7635.0576,
                 "max_load_count": 0,
-                "qps": 723.9371,
-                "recall": 0.9285,
-                "serial_latency_p99": 0.0052
+                "qps": 822.5318,
+                "recall": 0.9294,
+                "serial_latency_p99": 0.0056
             },
             "task_config": {
                 "case_config": {
                     "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -1931,19 +1931,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 7772.641,
+                "load_duration": 7635.0576,
                 "max_load_count": 0,
-                "qps": 315.5653,
-                "recall": 0.9757,
-                "serial_latency_p99": 0.0089
+                "qps": 378.9146,
+                "recall": 0.9758,
+                "serial_latency_p99": 0.0103
             },
             "task_config": {
                 "case_config": {
                     "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -1958,19 +1958,19 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 7772.641,
+                "load_duration": 7635.0576,
                 "max_load_count": 0,
-                "qps": 147.6055,
+                "qps": 218.6854,
                 "recall": 1,
-                "serial_latency_p99": 0.0132
+                "serial_latency_p99": 0.0162
             },
             "task_config": {
                 "case_config": {
                     "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
@@ -2209,19 +2209,19 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 5530.3545,
+                "load_duration": 5713.7159,
                 "max_load_count": 0,
-                "qps": 133.6633,
-                "recall": 0.9842,
-                "serial_latency_p99": 0.0133
+                "qps": 178.6585,
+                "recall": 0.9843,
+                "serial_latency_p99": 0.0137
             },
             "task_config": {
                 "case_config": {
                     "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "Milvus",
@@ -2237,19 +2237,19 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 5530.3545,
+                "load_duration": 5713.7159,
                 "max_load_count": 0,
-                "qps": 127.0729,
-                "recall": 0.9843,
-                "serial_latency_p99": 0.0154
+                "qps": 178.3732,
+                "recall": 0.9844,
+                "serial_latency_p99": 0.015
             },
             "task_config": {
                 "case_config": {
                     "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "Milvus",
@@ -2265,19 +2265,19 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 5530.3545,
+                "load_duration": 5713.7159,
                 "max_load_count": 0,
-                "qps": 182.826,
+                "qps": 229.3526,
                 "recall": 1,
-                "serial_latency_p99": 0.0122
+                "serial_latency_p99": 0.0125
             },
             "task_config": {
                 "case_config": {
                     "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "Milvus",
@@ -2293,19 +2293,19 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 607.0437,
+                "load_duration": 581.8141,
                 "max_load_count": 0,
-                "qps": 1118.5178,
-                "recall": 0.9796,
-                "serial_latency_p99": 0.0043
+                "qps": 1258.7043,
+                "recall": 0.9799,
+                "serial_latency_p99": 0.0049
             },
             "task_config": {
                 "case_config": {
                     "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "Milvus",
@@ -2321,19 +2321,19 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 607.0437,
+                "load_duration": 581.8141,
                 "max_load_count": 0,
-                "qps": 963.5486,
-                "recall": 0.9799,
-                "serial_latency_p99": 0.0048
+                "qps": 1075.8776,
+                "recall": 0.98,
+                "serial_latency_p99": 0.0053
             },
             "task_config": {
                 "case_config": {
                     "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "Milvus",
@@ -2349,19 +2349,19 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 607.0437,
+                "load_duration": 581.8141,
                 "max_load_count": 0,
-                "qps": 1381.2118,
+                "qps": 1494.8493,
                 "recall": 1,
-                "serial_latency_p99": 0.0039
+                "serial_latency_p99": 0.0047
             },
             "task_config": {
                 "case_config": {
                     "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "Milvus",
@@ -2377,19 +2377,71 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2559.3758,
+                "load_duration": 0.0,
+                "max_load_count": 4000000,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 1,
+                    "custom_case": {}
+                },
+                "db": "QdrantCloud",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "2c8g-1node",
+                    "prefer_grpc": true,
+                    "url": "**********"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 900000,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 2,
+                    "custom_case": {}
+                },
+                "db": "QdrantCloud",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "2c8g-1node",
+                    "prefer_grpc": true,
+                    "url": "**********"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
                 "max_load_count": 0,
-                "qps": 76.672,
-                "recall": 0.7964,
-                "serial_latency_p99": 0.0569
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
                     "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "QdrantCloud",
@@ -2401,21 +2453,21 @@
                     "db_label": "2c8g-1node",
                     "prefer_grpc": true,
                     "url": "**********"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
-                "load_duration": 2519.4009,
+                "load_duration": 0.0,
                 "max_load_count": 0,
-                "qps": 51.9266,
-                "recall": 0.7952,
-                "serial_latency_p99": 0.0535
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
                     "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "QdrantCloud",
@@ -2427,21 +2479,21 @@
                     "db_label": "2c8g-1node",
                     "prefer_grpc": true,
                     "url": "**********"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
-                "load_duration": 2528.1643,
+                "load_duration": 0.0,
                 "max_load_count": 0,
-                "qps": 128.3939,
-                "recall": 0.8613,
-                "serial_latency_p99": 0.0397
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
                     "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "QdrantCloud",
@@ -2533,19 +2585,19 @@
                     "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2571.4912,
+                "load_duration": 1647.857,
                 "max_load_count": 0,
-                "qps": 720.0978,
-                "recall": 0.7942,
-                "serial_latency_p99": 0.0347
+                "qps": 537.4975,
+                "recall": 0.8903,
+                "serial_latency_p99": 0.0189
             },
             "task_config": {
                 "case_config": {
                     "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "QdrantCloud",
@@ -2558,19 +2610,19 @@
                     "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2571.4912,
+                "load_duration": 1647.857,
                 "max_load_count": 0,
-                "qps": 553.2483,
-                "recall": 0.7942,
-                "serial_latency_p99": 0.0356
+                "qps": 372.0466,
+                "recall": 0.8904,
+                "serial_latency_p99": 0.0178
             },
             "task_config": {
                 "case_config": {
                     "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "QdrantCloud",
@@ -2583,19 +2635,19 @@
                     "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2571.4912,
+                "load_duration": 1647.857,
                 "max_load_count": 0,
-                "qps": 796.9777,
-                "recall": 0.8587,
-                "serial_latency_p99": 0.035
+                "qps": 1156.2898,
+                "recall": 0.9989,
+                "serial_latency_p99": 0.0144
             },
             "task_config": {
                 "case_config": {
                     "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "QdrantCloud",
@@ -2608,19 +2660,19 @@
                     "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 25181.5505,
+                "load_duration": 14623.578,
                 "max_load_count": 0,
-                "qps": 115.4696,
-                "recall": 0.7861,
-                "serial_latency_p99": 0.0677
+                "qps": 110.248,
+                "recall": 0.898,
+                "serial_latency_p99": 0.069
             },
             "task_config": {
                 "case_config": {
                     "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "QdrantCloud",
@@ -2634,19 +2686,19 @@
                     "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 24106.79,
+                "load_duration": 14623.578,
                 "max_load_count": 0,
-                "qps": 87.881,
-                "recall": 0.7836,
-                "serial_latency_p99": 0.0485
+                "qps": 87.2601,
+                "recall": 0.898,
+                "serial_latency_p99": 0.0278
             },
             "task_config": {
                 "case_config": {
                     "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "QdrantCloud",
@@ -2660,19 +2712,19 @@
                     "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 24106.79,
+                "load_duration": 14623.578,
                 "max_load_count": 0,
-                "qps": 130.1864,
-                "recall": 0.8412,
-                "serial_latency_p99": 0.0411
+                "qps": 125.7846,
+                "recall": 0.975,
+                "serial_latency_p99": 0.0231
             },
             "task_config": {
                 "case_config": {
                     "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "QdrantCloud",
@@ -2686,14 +2738,170 @@
                     "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
+                "load_duration": 1503.1147,
+                "max_load_count": 0,
+                "qps": 240.7209,
+                "recall": 0.8887,
+                "serial_latency_p99": 0.0174
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 5,
+                    "custom_case": {}
+                },
+                "db": "QdrantCloud",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "4c16g-1node",
+                    "prefer_grpc": true,
+                    "url": "**********"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 1503.1147,
+                "max_load_count": 0,
+                "qps": 189.4399,
+                "recall": 0.8889,
+                "serial_latency_p99": 0.0175
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 7,
+                    "custom_case": {}
+                },
+                "db": "QdrantCloud",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "4c16g-1node",
+                    "prefer_grpc": true,
+                    "url": "**********"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 1503.1147,
+                "max_load_count": 0,
+                "qps": 313.5116,
+                "recall": 0.9999,
+                "serial_latency_p99": 0.0161
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 9,
+                    "custom_case": {}
+                },
+                "db": "QdrantCloud",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "4c16g-1node",
+                    "prefer_grpc": true,
+                    "url": "**********"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 4,
+                    "custom_case": {}
+                },
+                "db": "QdrantCloud",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "4c16g-1node",
+                    "prefer_grpc": true,
+                    "url": "**********"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 6,
+                    "custom_case": {}
+                },
+                "db": "QdrantCloud",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "4c16g-1node",
+                    "prefer_grpc": true,
+                    "url": "**********"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 8,
+                    "custom_case": {}
+                },
+                "db": "QdrantCloud",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "4c16g-1node",
+                    "prefer_grpc": true,
+                    "url": "**********"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
                 "load_duration": 0.0,
                 "max_load_count": 5500000,
                 "qps": 0.0,
                 "recall": 0.0,
                 "serial_latency_p99": 0.0
             },
             "task_config": {
@@ -2738,19 +2946,19 @@
                     "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1259.961,
+                "load_duration": 1129.4487,
                 "max_load_count": 0,
-                "qps": 19.9197,
-                "recall": 0.8733,
-                "serial_latency_p99": 0.0697
+                "qps": 18.7634,
+                "recall": 0.8737,
+                "serial_latency_p99": 0.1537
             },
             "task_config": {
                 "case_config": {
                     "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "Pinecone",
@@ -2764,19 +2972,19 @@
                     "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1259.961,
+                "load_duration": 1129.4487,
                 "max_load_count": 0,
-                "qps": 19.358,
-                "recall": 0.8733,
-                "serial_latency_p99": 0.0697
+                "qps": 18.3619,
+                "recall": 0.8741,
+                "serial_latency_p99": 0.0798
             },
             "task_config": {
                 "case_config": {
                     "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "Pinecone",
@@ -2790,19 +2998,19 @@
                     "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1259.961,
+                "load_duration": 1129.4487,
                 "max_load_count": 0,
-                "qps": 29.3414,
-                "recall": 0.9356,
-                "serial_latency_p99": 0.0706
+                "qps": 25.2744,
+                "recall": 0.9979,
+                "serial_latency_p99": 0.0612
             },
             "task_config": {
                 "case_config": {
                     "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "Pinecone",
@@ -2946,19 +3154,19 @@
                     "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1450.5834,
+                "load_duration": 1582.9409,
                 "max_load_count": 0,
-                "qps": 237.946,
-                "recall": 0.9268,
-                "serial_latency_p99": 0.0204
+                "qps": 261.798,
+                "recall": 0.9262,
+                "serial_latency_p99": 0.0231
             },
             "task_config": {
                 "case_config": {
                     "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "Pinecone",
@@ -2972,19 +3180,19 @@
                     "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1450.5834,
+                "load_duration": 1582.9409,
                 "max_load_count": 0,
-                "qps": 207.6451,
-                "recall": 0.9268,
-                "serial_latency_p99": 0.0217
+                "qps": 166.1851,
+                "recall": 0.9264,
+                "serial_latency_p99": 0.0239
             },
             "task_config": {
                 "case_config": {
                     "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "Pinecone",
@@ -2998,19 +3206,19 @@
                     "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1450.5834,
+                "load_duration": 1582.9409,
                 "max_load_count": 0,
-                "qps": 66.6749,
-                "recall": 0.9191,
-                "serial_latency_p99": 0.0322
+                "qps": 121.7169,
+                "recall": 0.9693,
+                "serial_latency_p99": 0.029
             },
             "task_config": {
                 "case_config": {
                     "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "Pinecone",
@@ -3154,19 +3362,19 @@
                     "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1235.8487,
+                "load_duration": 1123.9889,
                 "max_load_count": 0,
-                "qps": 46.4164,
-                "recall": 0.8733,
-                "serial_latency_p99": 0.0348
+                "qps": 46.6189,
+                "recall": 0.8737,
+                "serial_latency_p99": 0.0431
             },
             "task_config": {
                 "case_config": {
                     "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "Pinecone",
@@ -3180,19 +3388,19 @@
                     "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1235.8474,
+                "load_duration": 1123.9889,
                 "max_load_count": 0,
-                "qps": 44.5978,
-                "recall": 0.8733,
-                "serial_latency_p99": 0.0394
+                "qps": 42.4856,
+                "recall": 0.8741,
+                "serial_latency_p99": 0.044
             },
             "task_config": {
                 "case_config": {
                     "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "Pinecone",
@@ -3206,19 +3414,19 @@
                     "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1235.8474,
+                "load_duration": 1123.9889,
                 "max_load_count": 0,
-                "qps": 127.9003,
-                "recall": 0.9356,
-                "serial_latency_p99": 0.0232
+                "qps": 138.9479,
+                "recall": 0.9979,
+                "serial_latency_p99": 0.0262
             },
             "task_config": {
                 "case_config": {
                     "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "Pinecone",
@@ -3388,19 +3596,19 @@
                     "index_name": "benchmark-test"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 14991.9752,
+                "load_duration": 11374.7189,
                 "max_load_count": 0,
-                "qps": 8.2809,
+                "qps": 8.6675,
                 "recall": 0.8369,
-                "serial_latency_p99": 0.1549
+                "serial_latency_p99": 0.1802
             },
             "task_config": {
                 "case_config": {
                     "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "Pinecone",
@@ -3414,19 +3622,19 @@
                     "index_name": "benchmark-test"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 14991.9752,
+                "load_duration": 11374.7189,
                 "max_load_count": 0,
-                "qps": 7.6488,
+                "qps": 7.8121,
                 "recall": 0.8369,
-                "serial_latency_p99": 0.1618
+                "serial_latency_p99": 0.1677
             },
             "task_config": {
                 "case_config": {
                     "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "Pinecone",
@@ -3440,19 +3648,19 @@
                     "index_name": "benchmark-test"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 14991.9752,
+                "load_duration": 11374.7189,
                 "max_load_count": 0,
-                "qps": 16.5246,
+                "qps": 16.869,
                 "recall": 0.9814,
-                "serial_latency_p99": 0.0803
+                "serial_latency_p99": 0.0878
             },
             "task_config": {
                 "case_config": {
                     "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "Pinecone",
@@ -3544,19 +3752,19 @@
                     "index_name": "benchmark-test"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 12658.5938,
+                "load_duration": 14165.6504,
                 "max_load_count": 0,
-                "qps": 283.5304,
+                "qps": 303.2044,
                 "recall": 0.9246,
-                "serial_latency_p99": 0.0256
+                "serial_latency_p99": 0.0274
             },
             "task_config": {
                 "case_config": {
                     "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "Pinecone",
@@ -3570,19 +3778,19 @@
                     "index_name": "benchmark-test"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 12658.5938,
+                "load_duration": 14165.6504,
                 "max_load_count": 0,
-                "qps": 136.1829,
-                "recall": 0.9245,
-                "serial_latency_p99": 0.029
+                "qps": 136.0345,
+                "recall": 0.9244,
+                "serial_latency_p99": 0.0319
             },
             "task_config": {
                 "case_config": {
                     "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "Pinecone",
@@ -3596,19 +3804,19 @@
                     "index_name": "benchmark-test"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 12658.5938,
+                "load_duration": 14165.6504,
                 "max_load_count": 0,
-                "qps": 71.5744,
+                "qps": 66.7221,
                 "recall": 0.963,
-                "serial_latency_p99": 0.0345
+                "serial_latency_p99": 0.0421
             },
             "task_config": {
                 "case_config": {
                     "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "Pinecone",
@@ -3774,12 +3982,244 @@
                 "db_config": {
                     "api_key": "**********",
                     "db_label": "p1.x1-8node",
                     "environment": "**********",
                     "index_name": "benchmark-test"
                 }
             }
+        },
+        {
+            "label": "?",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 1,
+                    "custom_case": {}
+                },
+                "db": "PgVector",
+                "db_case_config": {
+                    "lists": 10,
+                    "metric_type": "L2",
+                    "probes": 2
+                },
+                "db_config": {
+                    "db_label": "2c8g-1node",
+                    "db_name": "**********",
+                    "password": "**********",
+                    "url": "**********",
+                    "user_name": "**********"
+                }
+            }
+        },
+        {
+            "label": "?",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 2,
+                    "custom_case": {}
+                },
+                "db": "PgVector",
+                "db_case_config": {
+                    "lists": 10,
+                    "metric_type": "L2",
+                    "probes": 2
+                },
+                "db_config": {
+                    "db_label": "2c8g-1node",
+                    "db_name": "**********",
+                    "password": "**********",
+                    "url": "**********",
+                    "user_name": "**********"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 10247.5034,
+                "max_load_count": 0,
+                "qps": 10.6271,
+                "recall": 0.8898,
+                "serial_latency_p99": 0.7307
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 5,
+                    "custom_case": {}
+                },
+                "db": "PgVector",
+                "db_case_config": {
+                    "lists": 10,
+                    "metric_type": "COSINE",
+                    "probes": 2
+                },
+                "db_config": {
+                    "db_label": "2c8g-1node",
+                    "db_name": "**********",
+                    "password": "**********",
+                    "url": "**********",
+                    "user_name": "**********"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 10247.5034,
+                "max_load_count": 0,
+                "qps": 10.8507,
+                "recall": 0.8897,
+                "serial_latency_p99": 0.7332
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 7,
+                    "custom_case": {}
+                },
+                "db": "PgVector",
+                "db_case_config": {
+                    "lists": 10,
+                    "metric_type": "COSINE",
+                    "probes": 2
+                },
+                "db_config": {
+                    "db_label": "2c8g-1node",
+                    "db_name": "**********",
+                    "password": "**********",
+                    "url": "**********",
+                    "user_name": "**********"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 10247.5034,
+                "max_load_count": 0,
+                "qps": 75.7055,
+                "recall": 0.9999,
+                "serial_latency_p99": 0.1212
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 9,
+                    "custom_case": {}
+                },
+                "db": "PgVector",
+                "db_case_config": {
+                    "lists": 10,
+                    "metric_type": "COSINE",
+                    "probes": 2
+                },
+                "db_config": {
+                    "db_label": "2c8g-1node",
+                    "db_name": "**********",
+                    "password": "**********",
+                    "url": "**********",
+                    "user_name": "**********"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0,
+                "max_load_count": 0,
+                "qps": 0,
+                "recall": 0,
+                "serial_latency_p99": 0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 4,
+                    "custom_case": {}
+                },
+                "db": "PgVector",
+                "db_case_config": {
+                    "lists": 10,
+                    "metric_type": "COSINE",
+                    "probes": 2
+                },
+                "db_config": {
+                    "db_label": "2c8g-1node",
+                    "db_name": "**********",
+                    "password": "**********",
+                    "url": "**********",
+                    "user_name": "**********"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0,
+                "max_load_count": 0,
+                "qps": 0,
+                "recall": 0,
+                "serial_latency_p99": 0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 6,
+                    "custom_case": {}
+                },
+                "db": "PgVector",
+                "db_case_config": {
+                    "lists": 10,
+                    "metric_type": "COSINE",
+                    "probes": 2
+                },
+                "db_config": {
+                    "db_label": "2c8g-1node",
+                    "db_name": "**********",
+                    "password": "**********",
+                    "url": "**********",
+                    "user_name": "**********"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0,
+                "max_load_count": 0,
+                "qps": 0,
+                "recall": 0,
+                "serial_latency_p99": 0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 8,
+                    "custom_case": {}
+                },
+                "db": "PgVector",
+                "db_case_config": {
+                    "lists": 10,
+                    "metric_type": "COSINE",
+                    "probes": 2
+                },
+                "db_config": {
+                    "db_label": "2c8g-1node",
+                    "db_name": "**********",
+                    "password": "**********",
+                    "url": "**********",
+                    "user_name": "**********"
+                }
+            }
         }
     ],
     "run_id": "5c1e8bd468224ffda1b39b08cdc342c3",
     "task_label": "standard"
 }
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench.egg-info/PKG-INFO` & `vectordb-bench-0.0.3/vectordb_bench.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectordb-bench
-Version: 0.0.2
+Version: 0.0.3
 Summary: VectorDBBench is not just an offering of benchmark results for mainstream vector databases and cloud services, it's your go-to tool for the ultimate performance and cost-effectiveness comparison. Designed with ease-of-use in mind, VectorDBBench is devised to help users, even non-professionals, reproduce results or test new systems, making the hunt for the optimal choice amongst a plethora of cloud services and open-source vector databases a breeze.
 Author-email: XuanYang-cn <xuan.yang@zilliz.com>
 Project-URL: repository, https://github.com/zilliztech/VectorDBBench
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -13,14 +13,15 @@
 License-File: LICENSE
 
 # VectorDBBench: A Benchmark Tool for VectorDB
 
 [![version](https://img.shields.io/pypi/v/vectordb-bench.svg?color=blue)](https://pypi.org/project/vectordb-bench/)
 [![Downloads](https://pepy.tech/badge/vectordb-bench)](https://pepy.tech/project/vectordb-bench)
 
+**Leaderboard:** https://zilliz.com/benchmark
 ## Quick Start
 ### Prerequirement
 ``` shell
 python >= 3.11
 ```
 ### Install
 ``` shell
@@ -37,14 +38,32 @@
 Understanding the importance of user experience, we provide an intuitive visual interface. This not only empowers users to initiate benchmarks at ease, but also to view comparative result reports, thereby reproducing benchmark results effortlessly.
 To add more relevance and practicality, we provide cost-effectiveness reports particularly for cloud services. This allows for a more realistic and applicable benchmarking process.
 
 Closely mimicking real-world production environments, we've set up diverse testing scenarios including insertion, searching, and filtered searching. To provide you with credible and reliable data, we've included public datasets from actual production scenarios, such as [SIFT](http://corpus-texmex.irisa.fr/), [GIST](http://corpus-texmex.irisa.fr/), [Cohere](https://huggingface.co/datasets/Cohere/wikipedia-22-12/tree/main/en), and more. It's fascinating to discover how a relatively unknown open-source database might excel in certain circumstances!
 
 Prepare to delve into the world of VectorDBBench, and let it guide you in uncovering your perfect vector database match.  
 
+## Leaderboard
+### Introduction
+To facilitate the presentation of test results and provide a comprehensive performance analysis report, we offer a [leaderboard page](https://zilliz.com/benchmark). It allows us to choose from QPS, QP$, and latency metrics, and provides a comprehensive assessment of a system's performance based on the test results of various cases and a set of scoring mechanisms (to be introduced later). On this leaderboard, we can select the systems and models to be compared, and filter out cases we do not want to consider. Comprehensive scores are always ranked from best to worst, and the specific test results of each query will be presented in the list below.
+
+### Scoring Rules
+
+1. For each case, select a base value and score each system based on relative values. 
+    - For QPS and QP$, we use the highest value as the reference, denoted as `base_QPS` or `base_QP$`, and the score of each system is `(QPS/base_QPS) * 100` or `(QP$/base_QP$) * 100`. 
+    - For Latency, we use the lowest value as the reference, that is, `base_Latency`, and the score of each system is `(Latency + 10ms)/(base_Latency + 10ms)`. 
+
+    We want to give equal weight to different cases, and not let a case with high absolute result values become the sole reason for the overall scoring. Therefore, when scoring different systems in each case, we need to use relative values. 
+
+    Also, for Latency, we add 10ms to the numerator and denominator to ensure that if every system performs particularly well in a case, its advantage will not be infinitely magnified when latency tends to 0.
+
+2. For systems that fail or timeout in a particular case, we will give them a score based on a value worse than the worst result by a factor of two. For example, in QPS or QP$, it would be half the lowest value. For Latency, it would be twice the maximum value.
+
+3. For each system, we will take the geometric mean of its scores in all cases as its comprehensive score for a particular metric.
+
 ## Build on your own
 ### Install requirements
 ``` shell
 pip install -e '.[test]'
 ```
 ### Run test server
 ```
@@ -65,18 +84,20 @@
 
 ```shell
 $ ruff check vectordb_bench --fix
 ```
 
 ## How does it work?
 ### Result Page
-![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/66ab83c4-656e-41a8-a643-d9790faccbeb)
+![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/7f5cdae7-f9f2-4a81-b2e0-e5c6268cd970)
 This is the main page of VectorDBBench, which displays the standard benchmark results we provide. Additionally, results of all tests performed by users themselves will also be shown here. We also offer the ability to select and compare results from multiple tests simultaneously.
 
 The standard benchmark results displayed here include all 9 cases that we currently support for all our clients (Milvus, Zilliz Cloud, Elastic Search, Qdrant Cloud, and Weaviate Cloud). However, as some systems may not be able to complete all the tests successfully due to issues like Out of Memory (OOM) or timeouts, not all clients are included in every case.
+
+All standard benchmark results are generated by a client running on an 8 core, 32 GB host, which is located in the same region as the server being tested. The client host is equipped with an `Intel(R) Xeon(R) Platinum 8375C CPU @ 2.90GHz` processor. Also all the servers for the open-source systems tested in our benchmarks run on hosts with the same type of processor.
 ### Run Test Page
 ![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/a789099a-3707-4214-8052-b73463b8f2c6)
 This is the page to run a test:
 1. Initially, you select the systems to be tested - multiple selections are allowed. Once selected, corresponding forms will pop up to gather necessary information for using the chosen databases. The db_label is used to differentiate different instances of the same system. We recommend filling in the host size or instance type here (as we do in our standard results).
 2. The next step is to select the test cases you want to perform. You can select multiple cases at once, and a form to collect corresponding parameters will appear.
 3. Finally, you'll need to provide a task label to distinguish different test results. Using the same label for different tests will result in the previous results being overwritten.
 Now we can only run one task at the same time. 
@@ -98,25 +119,25 @@
 #### Filtering Search Performance Case
 - **Large Dataset, Low Filtering Rate:** Evaluates search performance with a large dataset (Cohere 10M vectors, 768 dimensions) under a low filtering rate (1% vectors) at different parallel levels.
 - **Medium Dataset, Low Filtering Rate:** This case uses a medium dataset (Cohere 1M vectors, 768 dimensions) with a similar low filtering rate.
 - **Large Dataset, High Filtering Rate:** It tests with a large dataset (Cohere 10M vectors, 768 dimensions) but under a high filtering rate (99% vectors).
 - **Medium Dataset, High Filtering Rate:** This case uses a medium dataset (Cohere 1M vectors, 768 dimensions) with a high filtering rate.
 For a quick reference, here is a table summarizing the key aspects of each case:
 
-Case No. | Case Type | Dataset Size | Dataset Type | Filtering Rate | Results |
-|----------|-----------|--------------|--------------|----------------|---------|
-1 | Capacity Case | Large Dim | GIST 100K vectors, 960 dimensions | N/A | Number of inserted vectors |
-2 | Capacity Case | Small Dim | SIFT 100K vectors, 128 dimensions | N/A | Number of inserted vectors |
-3 | Search Performance Case | XLarge Dataset | LAION 100M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
-4 | Search Performance Case | Large Dataset | Cohere 10M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
-5 | Search Performance Case | Medium Dataset | Cohere 1M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
-6 | Filtering Search Performance Case | Large Dataset, Low Filtering Rate | Cohere 10M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
-7 | Filtering Search Performance Case | Medium Dataset, Low Filtering Rate | Cohere 1M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
-8 | Filtering Search Performance Case | Large Dataset, High Filtering Rate | Cohere 10M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
-9 | Filtering Search Performance Case | Medium Dataset, High Filtering Rate | Cohere 1M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
+Case No. | Case Type | Dataset Size  | Filtering Rate | Results |
+|----------|-----------|--------------|----------------|---------|
+1 | Capacity Case | GIST 100K vectors, 960 dimensions | N/A | Number of inserted vectors |
+2 | Capacity Case | SIFT 100K vectors, 128 dimensions | N/A | Number of inserted vectors |
+3 | Search Performance Case | LAION 100M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
+4 | Search Performance Case | Cohere 10M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
+5 | Search Performance Case | Cohere 1M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
+6 | Filtering Search Performance Case | Cohere 10M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
+7 | Filtering Search Performance Case | Cohere 1M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
+8 | Filtering Search Performance Case | Cohere 10M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
+9 | Filtering Search Performance Case | Cohere 1M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
 
 Each case provides an in-depth examination of a vector database's abilities, providing you a comprehensive view of the database's performance.
 
 ## Goals
 Our goals of this benchmark are:
 ### Reproducibility & Usability
 One of the primary goals of VectorDBBench is to enable users to reproduce benchmark results swiftly and easily, or to test their customized scenarios. We believe that lowering the barriers to entry for conducting these tests will enhance the community's understanding and improvement of vector databases. We aim to create an environment where any user, regardless of their technical expertise, can quickly set up and run benchmarks, and view and analyze results in an intuitive manner.
@@ -196,7 +217,68 @@
 ### Fine-Tuning
 For the system under test, we use the default server-side configuration to maintain the authenticity and representativeness of our results.
 For the Client, we welcome any parameter tuning to obtain better results.
 ### Incomplete Results
 Many databases may not be able to complete all test cases due to issues such as Out of Memory (OOM), crashes, or timeouts. In these scenarios, we will clearly state these occurrences in the test results.
 ### Mistake Or Misrepresentation 
 We strive for accuracy in learning and supporting various vector databases, yet there might be oversights or misapplications. For any such occurrences, feel free to [raise an issue](https://github.com/zilliztech/VectorDBBench/issues/new) or make amendments on our GitHub page.
+## Timeout
+In our pursuit to ensure that our benchmark reflects the reality of a production environment while guaranteeing the practicality of the system, we have implemented a timeout plan based on our experiences for various tests.
+
+**1. Capacity Case:**
+- For Capacity Case, we have assigned an overall timeout.
+
+**2. Other Cases:**
+
+For other cases, we have set two timeouts:
+
+- **Data Loading Timeout:** This timeout is designed to filter out systems that are too slow in inserting data, thus ensuring that we are only considering systems that is able to cope with the demands of a real-world production environment within a reasonable time frame.
+
+- **Optimization Preparation Timeout**: This timeout is established to avoid excessive optimization strategies that might work for benchmarks but fail to deliver in real production environments. By doing this, we ensure that the systems we consider are not only suitable for testing environments but also applicable and efficient in production scenarios.
+
+This multi-tiered timeout approach allows our benchmark to be more representative of actual production environments and assists us in identifying systems that can truly perform in real-world scenarios.
+<table>
+    <tr>
+        <th>Case</th>
+        <th>Data Size</th>
+        <th>Timeout Type</th>
+        <th>Value</th>
+    </tr>
+    <tr>
+        <td>Capacity Case</td>
+        <td>N/A</td>
+        <td>Loading timeout</td>
+        <td>24 hours</td>
+    </tr>
+    <tr>
+        <td rowspan="2">Other Cases</td>
+        <td rowspan="2">1M vectors, 768 dimensions</td>
+        <td>Loading timeout</td>
+        <td>2.5 hours</td>
+    </tr>
+    <tr>
+        <td>Optimization timeout</td>
+        <td>15 mins</td>
+    </tr>
+    <tr>
+        <td rowspan="2">Other Cases</td>
+        <td rowspan="2">10M vectors, 768 dimensions</td>
+        <td>Loading timeout</td>
+        <td>25 hours</td>
+    </tr>
+    <tr>
+        <td>Optimization timeout</td>
+        <td>2.5 hours</td>
+    </tr>
+    <tr>
+        <td rowspan="2">Other Cases</td>
+        <td rowspan="2">100M vectors, 768 dimensions</td>
+        <td>Loading timeout</td>
+        <td>250 hours</td>
+    </tr>
+    <tr>
+        <td>Optimization timeout</td>
+        <td>25 hours</td>
+    </tr>
+</table>
+
+**Note:** Some datapoints in the standard benchmark results that voilate this timeout will be kept for now for reference. We will remove them in the future.
```

### Comparing `vectordb-bench-0.0.2/vectordb_bench.egg-info/SOURCES.txt` & `vectordb-bench-0.0.3/vectordb_bench.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 vectordb_bench/backend/utils.py
 vectordb_bench/backend/clients/__init__.py
 vectordb_bench/backend/clients/api.py
 vectordb_bench/backend/clients/elastic_cloud/config.py
 vectordb_bench/backend/clients/elastic_cloud/elastic_cloud.py
 vectordb_bench/backend/clients/milvus/config.py
 vectordb_bench/backend/clients/milvus/milvus.py
+vectordb_bench/backend/clients/pgvector/config.py
+vectordb_bench/backend/clients/pgvector/pgvector.py
 vectordb_bench/backend/clients/pinecone/config.py
 vectordb_bench/backend/clients/pinecone/pinecone.py
 vectordb_bench/backend/clients/qdrant_cloud/config.py
 vectordb_bench/backend/clients/qdrant_cloud/qdrant_cloud.py
 vectordb_bench/backend/clients/weaviate_cloud/config.py
 vectordb_bench/backend/clients/weaviate_cloud/weaviate_cloud.py
 vectordb_bench/backend/clients/zilliz_cloud/config.py
@@ -70,8 +72,11 @@
 vectordb_bench/frontend/components/run_test/hideSidebar.py
 vectordb_bench/frontend/components/run_test/submitTask.py
 vectordb_bench/frontend/const/dbCaseConfigs.py
 vectordb_bench/frontend/const/dbPrices.py
 vectordb_bench/frontend/const/styles.py
 vectordb_bench/frontend/pages/quries_per_dollar.py
 vectordb_bench/frontend/pages/run_test.py
-vectordb_bench/results/result_20230609_standard.json
+vectordb_bench/results/dbPrices.json
+vectordb_bench/results/getLeaderboardData.py
+vectordb_bench/results/leaderboard.json
+vectordb_bench/results/result_20230705_standard.json
```


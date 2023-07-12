# Comparing `tmp/smart_vector-0.1.dev737.tar.gz` & `tmp/smart_vector-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/johnyan/Documents/project/chroma/dist/.tmp-9828_6_k/smart_vector-0.1.dev737.tar", last modified: Wed Jul 12 08:43:08 2023, max compression
+gzip compressed data, was "/Users/johnyan/Documents/project/smartvector/dist/.tmp-dibqify5/smart_vector-1.0.tar", last modified: Wed Jul 12 09:10:44 2023, max compression
```

## Comparing `smart_vector-0.1.dev737.tar` & `smart_vector-1.0.tar`

### file list

```diff
@@ -1,237 +1,15 @@
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.696127 smart_vector-0.1.dev737/
--rw-r--r--   0 johnyan    (501) staff       (20)       84 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/.dockerignore
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.400746 smart_vector-0.1.dev737/.github/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.435393 smart_vector-0.1.dev737/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 johnyan    (501) staff       (20)     1512 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 johnyan    (501) staff       (20)     1520 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 johnyan    (501) staff       (20)     1384 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/.github/ISSUE_TEMPLATE/installation_trouble.yaml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.440639 smart_vector-0.1.dev737/.github/workflows/
--rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/.github/workflows/chroma-client-integration-test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/.github/workflows/chroma-integration-test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1338 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/.github/workflows/chroma-release-python-client.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     4169 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/.github/workflows/chroma-release.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1205 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/.github/workflows/chroma-test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1734 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/.github/workflows/pr-review-checklist.yml
--rw-r--r--   0 johnyan    (501) staff       (20)      228 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/.gitignore
--rw-r--r--   0 johnyan    (501) staff       (20)     1167 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/.pre-commit-config.yaml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.441613 smart_vector-0.1.dev737/.vscode/
--rw-r--r--   0 johnyan    (501) staff       (20)     1020 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/.vscode/settings.json
--rw-r--r--   0 johnyan    (501) staff       (20)     3323 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/DEVELOP.md
--rw-r--r--   0 johnyan    (501) staff       (20)      647 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/Dockerfile
--rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/LICENSE
--rw-r--r--   0 johnyan    (501) staff       (20)      379 2023-07-12 08:43:08.695401 smart_vector-0.1.dev737/PKG-INFO
--rw-r--r--   0 johnyan    (501) staff       (20)      619 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/RELEASE_PROCESS.md
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.454831 smart_vector-0.1.dev737/bin/
--rw-r--r--   0 johnyan    (501) staff       (20)     1610 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/bin/backup.sh
--rwxr-xr-x   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/bin/build
--rwxr-xr-x   0 johnyan    (501) staff       (20)      234 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/bin/docker_entrypoint.sh
--rw-r--r--   0 johnyan    (501) staff       (20)     6462 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/bin/generate_cloudformation.py
--rwxr-xr-x   0 johnyan    (501) staff       (20)      463 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/bin/integration-test
--rw-r--r--   0 johnyan    (501) staff       (20)     1688 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/bin/restore.sh
--rw-r--r--   0 johnyan    (501) staff       (20)     1105 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/bin/setup_linux.sh
--rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/bin/setup_mac.sh
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.455830 smart_vector-0.1.dev737/bin/templates/
--rw-r--r--   0 johnyan    (501) staff       (20)      985 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/bin/templates/docker-compose.yml
--rwxr-xr-x   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/bin/test-package.sh
--rwxr-xr-x   0 johnyan    (501) staff       (20)      297 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/bin/test-remote
--rw-r--r--   0 johnyan    (501) staff       (20)      205 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/bin/test.py
--rwxr-xr-x   0 johnyan    (501) staff       (20)      151 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/bin/version
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.464471 smart_vector-0.1.dev737/chromadb/
--rw-r--r--   0 johnyan    (501) staff       (20)      894 2023-07-04 08:34:52.000000 smart_vector-0.1.dev737/chromadb/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.473088 smart_vector-0.1.dev737/chromadb/api/
--rw-r--r--   0 johnyan    (501) staff       (20)    10943 2023-07-06 08:22:49.000000 smart_vector-0.1.dev737/chromadb/api/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12493 2023-07-07 00:28:31.000000 smart_vector-0.1.dev737/chromadb/api/fastapi.py
--rw-r--r--   0 johnyan    (501) staff       (20)    17939 2023-07-10 00:46:47.000000 smart_vector-0.1.dev737/chromadb/api/local.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.474492 smart_vector-0.1.dev737/chromadb/api/models/
--rw-r--r--   0 johnyan    (501) staff       (20)    15101 2023-07-06 06:54:49.000000 smart_vector-0.1.dev737/chromadb/api/models/Collection.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1297 2023-07-10 00:46:47.000000 smart_vector-0.1.dev737/chromadb/api/smartapi.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11283 2023-07-03 09:25:09.000000 smart_vector-0.1.dev737/chromadb/api/types.py
--rw-r--r--   0 johnyan    (501) staff       (20)      168 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/app.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7231 2023-07-03 08:16:05.000000 smart_vector-0.1.dev737/chromadb/config.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.493006 smart_vector-0.1.dev737/chromadb/db/
--rw-r--r--   0 johnyan    (501) staff       (20)     3417 2023-07-07 00:28:30.000000 smart_vector-0.1.dev737/chromadb/db/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6017 2023-07-07 00:28:30.000000 smart_vector-0.1.dev737/chromadb/db/base.py
--rw-r--r--   0 johnyan    (501) staff       (20)    22388 2023-07-10 00:46:47.000000 smart_vector-0.1.dev737/chromadb/db/clickhouse.py
--rw-r--r--   0 johnyan    (501) staff       (20)    18856 2023-07-07 03:46:58.000000 smart_vector-0.1.dev737/chromadb/db/duckdb.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.495102 smart_vector-0.1.dev737/chromadb/db/impl/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/db/impl/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6234 2023-07-07 00:28:31.000000 smart_vector-0.1.dev737/chromadb/db/impl/sqlite.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.497660 smart_vector-0.1.dev737/chromadb/db/index/
--rw-r--r--   0 johnyan    (501) staff       (20)      447 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/db/index/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11087 2023-07-10 00:46:47.000000 smart_vector-0.1.dev737/chromadb/db/index/hnswlib.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8096 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/db/migrations.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.508539 smart_vector-0.1.dev737/chromadb/db/mixins/
--rw-r--r--   0 johnyan    (501) staff       (20)     9206 2023-07-07 00:28:30.000000 smart_vector-0.1.dev737/chromadb/db/mixins/embeddings_queue.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15571 2023-07-07 00:28:30.000000 smart_vector-0.1.dev737/chromadb/db/mixins/sysdb.py
--rw-r--r--   0 johnyan    (501) staff       (20)    17789 2023-07-10 00:46:47.000000 smart_vector-0.1.dev737/chromadb/db/smartdb.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2669 2023-07-07 00:28:31.000000 smart_vector-0.1.dev737/chromadb/db/system.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1293 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/errors.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.509677 smart_vector-0.1.dev737/chromadb/ingest/
--rw-r--r--   0 johnyan    (501) staff       (20)     3643 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/ingest/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.510748 smart_vector-0.1.dev737/chromadb/segment/
--rw-r--r--   0 johnyan    (501) staff       (20)     3059 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/segment/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.404307 smart_vector-0.1.dev737/chromadb/segment/impl/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.511715 smart_vector-0.1.dev737/chromadb/segment/impl/manager/
--rw-r--r--   0 johnyan    (501) staff       (20)     4358 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/segment/impl/manager/local.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.512943 smart_vector-0.1.dev737/chromadb/segment/impl/metadata/
--rw-r--r--   0 johnyan    (501) staff       (20)    17879 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/segment/impl/metadata/sqlite.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.514088 smart_vector-0.1.dev737/chromadb/segment/impl/vector/
--rw-r--r--   0 johnyan    (501) staff       (20)    11965 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/segment/impl/vector/local_hnsw.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.514966 smart_vector-0.1.dev737/chromadb/server/
--rw-r--r--   0 johnyan    (501) staff       (20)      172 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/server/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.517556 smart_vector-0.1.dev737/chromadb/server/fastapi/
--rw-r--r--   0 johnyan    (501) staff       (20)     9064 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/server/fastapi/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2134 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/server/fastapi/types.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.521223 smart_vector-0.1.dev737/chromadb/telemetry/
--rw-r--r--   0 johnyan    (501) staff       (20)     3214 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/telemetry/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)      591 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/telemetry/events.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1161 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/telemetry/posthog.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.528456 smart_vector-0.1.dev737/chromadb/test/
--rw-r--r--   0 johnyan    (501) staff       (20)     3993 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/conftest.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.535278 smart_vector-0.1.dev737/chromadb/test/db/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.557124 smart_vector-0.1.dev737/chromadb/test/db/migrations/
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/db/migrations/00001-migration-1.psql.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/db/migrations/00002-migration-2.psql.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/db/migrations/00003-migration-3.psql.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)     1168 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/db/test_base.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5026 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/db/test_migrations.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9773 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/db/test_system.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.558372 smart_vector-0.1.dev737/chromadb/test/hnswlib/
--rw-r--r--   0 johnyan    (501) staff       (20)     2337 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/hnswlib/test_hnswlib.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.567936 smart_vector-0.1.dev737/chromadb/test/ingest/
--rw-r--r--   0 johnyan    (501) staff       (20)     8117 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/ingest/test_producer_consumer.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.598892 smart_vector-0.1.dev737/chromadb/test/property/
--rw-r--r--   0 johnyan    (501) staff       (20)    11294 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/property/invariants.py
--rw-r--r--   0 johnyan    (501) staff       (20)    18662 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/property/strategies.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2213 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/property/test_add.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6211 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/property/test_collections.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9123 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/property/test_cross_version_persist.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11073 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/property/test_embeddings.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9062 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/property/test_filtering.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5146 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/property/test_persist.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.601187 smart_vector-0.1.dev737/chromadb/test/segment/
--rw-r--r--   0 johnyan    (501) staff       (20)    15026 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/segment/test_metadata.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12132 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/segment/test_vector.py
--rw-r--r--   0 johnyan    (501) staff       (20)    40340 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/test_api.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2234 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/test_chroma.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4127 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/test_config.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.602180 smart_vector-0.1.dev737/chromadb/test/utils/
--rw-r--r--   0 johnyan    (501) staff       (20)     3544 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/test/utils/test_messagid.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3702 2023-06-30 03:21:44.000000 smart_vector-0.1.dev737/chromadb/types.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.605063 smart_vector-0.1.dev737/chromadb/utils/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/utils/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    16311 2023-06-30 06:12:24.000000 smart_vector-0.1.dev737/chromadb/utils/embedding_functions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2301 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/chromadb/utils/messageid.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.412305 smart_vector-0.1.dev737/clients/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.630995 smart_vector-0.1.dev737/clients/js/
--rw-r--r--   0 johnyan    (501) staff       (20)       66 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/.gitignore
--rw-r--r--   0 johnyan    (501) staff       (20)       32 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/.prettierignore
--rw-r--r--   0 johnyan    (501) staff       (20)        3 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/.prettierrc.json
--rw-r--r--   0 johnyan    (501) staff       (20)     1256 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/DEVELOP.md
--rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/LICENSE
--rw-r--r--   0 johnyan    (501) staff       (20)     1266 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)      324 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/config.yml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.410378 smart_vector-0.1.dev737/clients/js/examples/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.637838 smart_vector-0.1.dev737/clients/js/examples/browser/
--rw-r--r--   0 johnyan    (501) staff       (20)      358 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/examples/browser/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)     1787 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/examples/browser/app.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      834 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/examples/browser/index.html
--rw-r--r--   0 johnyan    (501) staff       (20)      409 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/examples/browser/package.json
--rw-r--r--   0 johnyan    (501) staff       (20)    71072 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/examples/browser/yarn.lock
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.643524 smart_vector-0.1.dev737/clients/js/examples/node/
--rw-r--r--   0 johnyan    (501) staff       (20)       57 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/examples/node/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)     1191 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/examples/node/app.js
--rw-r--r--   0 johnyan    (501) staff       (20)    46542 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/examples/node/package-lock.json
--rw-r--r--   0 johnyan    (501) staff       (20)      503 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/examples/node/package.json
--rw-r--r--   0 johnyan    (501) staff       (20)    17116 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/examples/node/yarn.lock
--rwxr-xr-x   0 johnyan    (501) staff       (20)     1075 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/genapi.sh
--rw-r--r--   0 johnyan    (501) staff       (20)      469 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/jest.config.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      153 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/openapitools.json
--rw-r--r--   0 johnyan    (501) staff       (20)   450648 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/package-lock.json
--rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/package.json
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.650302 smart_vector-0.1.dev737/clients/js/src/
--rw-r--r--   0 johnyan    (501) staff       (20)     8171 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/ChromaClient.ts
--rw-r--r--   0 johnyan    (501) staff       (20)    19403 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/Collection.ts
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.655296 smart_vector-0.1.dev737/clients/js/src/embeddings/
--rw-r--r--   0 johnyan    (501) staff       (20)      938 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/embeddings/CohereEmbeddingFunction.ts
--rw-r--r--   0 johnyan    (501) staff       (20)       92 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/embeddings/IEmbeddingFunction.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1563 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2493 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
--rwxr-xr-x   0 johnyan    (501) staff       (20)     3402 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.663177 smart_vector-0.1.dev737/clients/js/src/generated/
--rw-r--r--   0 johnyan    (501) staff       (20)      921 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/generated/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)    56700 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/generated/api.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1478 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/generated/configuration.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      429 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/generated/index.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     5862 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/generated/models.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1307 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/generated/runtime.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      490 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/index.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1715 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/types.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2002 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/src/utils.ts
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.676701 smart_vector-0.1.dev737/clients/js/test/
--rw-r--r--   0 johnyan    (501) staff       (20)     2625 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/test/add.collections.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     7586 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/test/client.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     3284 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/test/collection.client.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2551 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/test/collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/test/data.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/test/delete.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2599 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/test/get.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      206 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/test/initClient.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      577 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/test/peek.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1990 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/test/query.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2160 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/test/update.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      802 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/test/upsert.collections.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      367 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/tsconfig.json
--rw-r--r--   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/tsconfig.module.json
--rw-r--r--   0 johnyan    (501) staff       (20)   157735 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/js/yarn.lock
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.679658 smart_vector-0.1.dev737/clients/python/
--rw-r--r--   0 johnyan    (501) staff       (20)     1627 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/python/README.md
--rwxr-xr-x   0 johnyan    (501) staff       (20)     1257 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/python/build_python_thin_client.sh
--rwxr-xr-x   0 johnyan    (501) staff       (20)      826 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/python/integration-test.sh
--rw-r--r--   0 johnyan    (501) staff       (20)       22 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/python/is_thin_client.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1166 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/clients/python/pyproject.toml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.681305 smart_vector-0.1.dev737/config/
--rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/config/backup_disk.xml
--rw-r--r--   0 johnyan    (501) staff       (20)      233 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/config/chroma_users.xml
--rw-r--r--   0 johnyan    (501) staff       (20)     1080 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/docker-compose.server.example.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1221 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/docker-compose.test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1226 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/docker-compose.yml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.683420 smart_vector-0.1.dev737/examples/
--rw-r--r--   0 johnyan    (501) staff       (20)    10346 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/examples/alternative_embeddings.ipynb
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.413586 smart_vector-0.1.dev737/examples/deployments/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.687131 smart_vector-0.1.dev737/examples/deployments/google-cloud-compute/
--rw-r--r--   0 johnyan    (501) staff       (20)      611 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/examples/deployments/google-cloud-compute/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)      752 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/examples/deployments/google-cloud-compute/chroma.tf
--rw-r--r--   0 johnyan    (501) staff       (20)      125 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/examples/deployments/google-cloud-compute/main.tf
--rw-r--r--   0 johnyan    (501) staff       (20)     2271 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/examples/deployments/google-cloud-compute/startup.sh
--rw-r--r--   0 johnyan    (501) staff       (20)      181 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/examples/deployments/google-cloud-compute/variables.tf
--rw-r--r--   0 johnyan    (501) staff       (20)     5830 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/examples/local_persistence.ipynb
--rw-r--r--   0 johnyan    (501) staff       (20)     5493 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/examples/where_filtering.ipynb
--rw-r--r--   0 johnyan    (501) staff       (20)      495 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/log_config.yml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.415539 smart_vector-0.1.dev737/migrations/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.687724 smart_vector-0.1.dev737/migrations/embeddings_queue/
--rw-r--r--   0 johnyan    (501) staff       (20)      261 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/migrations/embeddings_queue/00001-embeddings.sqlite.sql
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.688455 smart_vector-0.1.dev737/migrations/metadb/
--rw-r--r--   0 johnyan    (501) staff       (20)      620 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/migrations/metadb/00001-embedding-metadata.sqlite.sql
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.689872 smart_vector-0.1.dev737/migrations/sysdb/
--rw-r--r--   0 johnyan    (501) staff       (20)      336 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/migrations/sysdb/00001-collections.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/migrations/sysdb/00002-segments.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)      372 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/pull_request_template.md
--rw-r--r--   0 johnyan    (501) staff       (20)      792 2023-07-11 09:50:53.000000 smart_vector-0.1.dev737/pyproject.toml
--rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-26 07:09:55.000000 smart_vector-0.1.dev737/pyproject_chroma.toml
--rw-r--r--   0 johnyan    (501) staff       (20)      352 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/requirements.txt
--rw-r--r--   0 johnyan    (501) staff       (20)      161 2023-06-25 09:21:06.000000 smart_vector-0.1.dev737/requirements_dev.txt
--rw-r--r--   0 johnyan    (501) staff       (20)       38 2023-07-12 08:43:08.696319 smart_vector-0.1.dev737/setup.cfg
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.691774 smart_vector-0.1.dev737/smart_vector/
--rw-r--r--   0 johnyan    (501) staff       (20)       79 2023-07-12 07:56:49.000000 smart_vector-0.1.dev737/smart_vector/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2713 2023-07-11 09:50:53.000000 smart_vector-0.1.dev737/smart_vector/readme.md
--rw-r--r--   0 johnyan    (501) staff       (20)     5345 2023-07-12 08:29:59.000000 smart_vector-0.1.dev737/smart_vector/smart_vector.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 08:43:08.694653 smart_vector-0.1.dev737/smart_vector.egg-info/
--rw-r--r--   0 johnyan    (501) staff       (20)      379 2023-07-12 08:43:08.000000 smart_vector-0.1.dev737/smart_vector.egg-info/PKG-INFO
--rw-r--r--   0 johnyan    (501) staff       (20)     5904 2023-07-12 08:43:08.000000 smart_vector-0.1.dev737/smart_vector.egg-info/SOURCES.txt
--rw-r--r--   0 johnyan    (501) staff       (20)        1 2023-07-12 08:43:08.000000 smart_vector-0.1.dev737/smart_vector.egg-info/dependency_links.txt
--rw-r--r--   0 johnyan    (501) staff       (20)       11 2023-07-12 08:43:08.000000 smart_vector-0.1.dev737/smart_vector.egg-info/requires.txt
--rw-r--r--   0 johnyan    (501) staff       (20)       13 2023-07-12 08:43:08.000000 smart_vector-0.1.dev737/smart_vector.egg-info/top_level.txt
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 09:10:44.843938 smart_vector-1.0/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1240 2023-07-12 09:10:44.843301 smart_vector-1.0/PKG-INFO
+-rw-r--r--   0 johnyan    (501) staff       (20)      889 2023-07-12 09:05:32.000000 smart_vector-1.0/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      786 2023-07-12 09:10:14.000000 smart_vector-1.0/pyproject.toml
+-rw-r--r--   0 johnyan    (501) staff       (20)       11 2023-07-12 09:07:38.000000 smart_vector-1.0/requirements.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)       38 2023-07-12 09:10:44.844076 smart_vector-1.0/setup.cfg
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 09:10:44.840174 smart_vector-1.0/smart_vector/
+-rw-r--r--   0 johnyan    (501) staff       (20)       79 2023-07-12 07:56:49.000000 smart_vector-1.0/smart_vector/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5344 2023-07-12 09:05:32.000000 smart_vector-1.0/smart_vector/smart_vector.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-12 09:10:44.842490 smart_vector-1.0/smart_vector.egg-info/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1240 2023-07-12 09:10:44.000000 smart_vector-1.0/smart_vector.egg-info/PKG-INFO
+-rw-r--r--   0 johnyan    (501) staff       (20)      274 2023-07-12 09:10:44.000000 smart_vector-1.0/smart_vector.egg-info/SOURCES.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)        1 2023-07-12 09:10:44.000000 smart_vector-1.0/smart_vector.egg-info/dependency_links.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)       11 2023-07-12 09:10:44.000000 smart_vector-1.0/smart_vector.egg-info/requires.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)       13 2023-07-12 09:10:44.000000 smart_vector-1.0/smart_vector.egg-info/top_level.txt
```

### Comparing `smart_vector-0.1.dev737/pyproject.toml` & `smart_vector-1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "smart_vector"
-dynamic = ["version"]
+version = '1.0'
 
 authors = [
   { name="John Yan", email="yanxiaohua@smartchart.cn" },
 ]
 description = "smart vector db"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `smart_vector-0.1.dev737/smart_vector/smart_vector.py` & `smart_vector-1.0/smart_vector/smart_vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from smart_chart.common.connect_db import DB_conn
 import requests
 import json, re
 
-
 class Text2VecEmbeddingFunction():
     def __init__(self, model_name: str = "shibing624/text2vec-base-chinese"):
         self._model = None
         self.model_name = model_name
 
     def __call__(self, texts):
         if not self._model:
```


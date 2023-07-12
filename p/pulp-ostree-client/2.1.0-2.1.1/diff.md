# Comparing `tmp/pulp_ostree-client-2.1.0.tar.gz` & `tmp/pulp_ostree-client-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp_ostree-client-2.1.0.tar", last modified: Sun May 28 21:30:16 2023, max compression
+gzip compressed data, was "pulp_ostree-client-2.1.1.tar", last modified: Wed Jul 12 13:23:40 2023, max compression
```

## Comparing `pulp_ostree-client-2.1.0.tar` & `pulp_ostree-client-2.1.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.581306 pulp_ostree-client-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-28 21:30:16.581306 pulp_ostree-client-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.561306 pulp_ostree-client-2.1.0/pulp_ostree_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-28 21:30:16.000000 pulp_ostree-client-2.1.0/pulp_ostree_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-28 21:30:16.000000 pulp_ostree-client-2.1.0/pulp_ostree_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:30:16.000000 pulp_ostree-client-2.1.0/pulp_ostree_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 21:30:16.000000 pulp_ostree-client-2.1.0/pulp_ostree_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-28 21:30:16.000000 pulp_ostree-client-2.1.0/pulp_ostree_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.561306 pulp_ostree-client-2.1.0/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.561306 pulp_ostree-client-2.1.0/pulpcore/client/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.561306 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.565306 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_commits_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_configs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_content_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17576 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_objects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_refs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_summaries_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/distributions_ostree_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    47216 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/remotes_ostree_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    73841 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/repositories_ostree_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33859 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/repositories_ostree_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26289 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.573306 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_import_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_import_commits_to_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_commit_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_content_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_object_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_ref_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    30086 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    27467 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response_hidden_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_commit_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_config_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_content_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_object_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_ref_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_summary_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/patchedostree_ostree_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    30479 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/patchedostree_ostree_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/patchedostree_ostree_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repair.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-28 21:30:16.581306 pulp_ostree-client-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.581306 pulp_ostree-client-2.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/test/test_async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_content_commits_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_content_configs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_content_content_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_content_objects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_content_refs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_content_summaries_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/test/test_content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_distributions_ostree_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/test/test_ostree_import_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/test/test_ostree_import_commits_to_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_commit_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_content_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_object_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_ref_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_remote_response_hidden_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_commit_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_config_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_content_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_object_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_ref_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_summary_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_patchedostree_ostree_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_patchedostree_ostree_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_patchedostree_ostree_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_remotes_ostree_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_repair.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_repositories_ostree_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_repositories_ostree_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_repository_version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:23:40.290205 pulp_ostree-client-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-12 13:23:40.290205 pulp_ostree-client-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:23:40.274205 pulp_ostree-client-2.1.1/pulp_ostree_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-12 13:23:40.000000 pulp_ostree-client-2.1.1/pulp_ostree_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-12 13:23:40.000000 pulp_ostree-client-2.1.1/pulp_ostree_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:23:40.000000 pulp_ostree-client-2.1.1/pulp_ostree_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 13:23:40.000000 pulp_ostree-client-2.1.1/pulp_ostree_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 13:23:40.000000 pulp_ostree-client-2.1.1/pulp_ostree_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:23:40.274205 pulp_ostree-client-2.1.1/pulpcore/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-12 13:23:39.000000 pulp_ostree-client-2.1.1/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:23:40.278205 pulp_ostree-client-2.1.1/pulpcore/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-12 13:23:39.000000 pulp_ostree-client-2.1.1/pulpcore/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:23:40.278205 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-12 13:23:39.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:23:40.278205 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-12 13:23:39.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/content_commits_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/content_configs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/content_content_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17576 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/content_objects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/content_refs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/content_summaries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45316 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/distributions_ostree_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47216 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/remotes_ostree_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73841 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/repositories_ostree_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33859 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/repositories_ostree_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26289 2023-07-12 13:23:39.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-07-12 13:23:39.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-12 13:23:39.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:23:40.282205 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-12 13:23:39.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_import_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_import_commits_to_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_commit_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_content_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_object_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_ref_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30086 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27467 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response_hidden_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_commit_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_config_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_content_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_object_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_ref_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_summary_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/patchedostree_ostree_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30479 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/patchedostree_ostree_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/patchedostree_ostree_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/repair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-07-12 13:23:39.000000 pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-12 13:23:40.290205 pulp_ostree-client-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:23:40.290205 pulp_ostree-client-2.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_content_commits_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_content_configs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_content_content_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_content_objects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_content_refs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_content_summaries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_distributions_ostree_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_ostree_import_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_ostree_import_commits_to_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_ostree_ostree_commit_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_ostree_ostree_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_ostree_ostree_content_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_ostree_ostree_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_ostree_ostree_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_ostree_ostree_object_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_ostree_ostree_ref_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_ostree_ostree_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_ostree_ostree_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_ostree_ostree_remote_response_hidden_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_ostree_ostree_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_ostree_ostree_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_ostree_ostree_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_commit_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_config_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_content_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_object_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_ref_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_summary_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_patchedostree_ostree_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_patchedostree_ostree_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_patchedostree_ostree_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_remotes_ostree_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_repair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_repositories_ostree_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_repositories_ostree_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-12 13:23:38.000000 pulp_ostree-client-2.1.1/test/test_repository_version_response.py
```

### Comparing `pulp_ostree-client-2.1.0/README.md` & `pulp_ostree-client-2.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pulp_ostree-client
 Fetch, Upload, Organize, and Distribute Software Packages
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v3
-- Package version: 2.1.0
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pulpproject.org](https://pulpproject.org)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `pulp_ostree-client-2.1.0/pulp_ostree_client.egg-info/SOURCES.txt` & `pulp_ostree-client-2.1.1/pulp_ostree_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/__init__.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: pulp-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 # import apis into sdk package
 from pulpcore.client.pulp_ostree.api.content_commits_api import ContentCommitsApi
 from pulpcore.client.pulp_ostree.api.content_configs_api import ContentConfigsApi
 from pulpcore.client.pulp_ostree.api.content_content_api import ContentContentApi
 from pulpcore.client.pulp_ostree.api.content_objects_api import ContentObjectsApi
 from pulpcore.client.pulp_ostree.api.content_refs_api import ContentRefsApi
```

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/__init__.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_commits_api.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/content_commits_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_configs_api.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/content_configs_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_content_api.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/content_content_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_objects_api.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/content_objects_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_refs_api.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/content_refs_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_summaries_api.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/content_summaries_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/distributions_ostree_api.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/distributions_ostree_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,15 @@
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `base_path` - Base path * `-base_path` - Base path (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `base_path` - Base path * `-base_path` - Base path (descending) * `hidden` - Hidden * `-hidden` - Hidden (descending) * `pk` - Pk * `-pk` - Pk (descending)
         :param list[str] pulp_href__in: Multiple values may be separated by commas.
         :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str pulp_label_select: Filter labels by search string
         :param str repository: Filter results where repository matches value
         :param list[str] repository__in: Filter results where repository is in a comma-separated list of values
         :param str with_content: Filter distributions based on the content served by them
         :param list[str] fields: A list of fields to include in the response.
@@ -330,15 +330,15 @@
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `base_path` - Base path * `-base_path` - Base path (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `base_path` - Base path * `-base_path` - Base path (descending) * `hidden` - Hidden * `-hidden` - Hidden (descending) * `pk` - Pk * `-pk` - Pk (descending)
         :param list[str] pulp_href__in: Multiple values may be separated by commas.
         :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str pulp_label_select: Filter labels by search string
         :param str repository: Filter results where repository matches value
         :param list[str] repository__in: Filter results where repository is in a comma-separated list of values
         :param str with_content: Filter distributions based on the content served by them
         :param list[str] fields: A list of fields to include in the response.
```

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/remotes_ostree_api.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/remotes_ostree_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/repositories_ostree_api.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/repositories_ostree_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/repositories_ostree_versions_api.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api/repositories_ostree_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api_client.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.1.0/python'
+        self.user_agent = 'OpenAPI-Generator/2.1.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/configuration.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3\n"\
-               "SDK Package Version: 2.1.0".\
+               "SDK Package Version: 2.1.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/exceptions.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/__init__.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/async_operation_response.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/content_summary_response.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_import_all.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_import_all.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_import_commits_to_ref.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_import_commits_to_ref.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_commit_response.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_commit_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_config_response.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_config_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_content_response.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_content_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,45 +32,50 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'base_path': 'str',
         'content_guard': 'str',
+        'hidden': 'bool',
         'pulp_labels': 'dict(str, str)',
         'name': 'str',
         'repository': 'str',
         'repository_version': 'str'
     }
 
     attribute_map = {
         'base_path': 'base_path',
         'content_guard': 'content_guard',
+        'hidden': 'hidden',
         'pulp_labels': 'pulp_labels',
         'name': 'name',
         'repository': 'repository',
         'repository_version': 'repository_version'
     }
 
-    def __init__(self, base_path=None, content_guard=None, pulp_labels=None, name=None, repository=None, repository_version=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, base_path=None, content_guard=None, hidden=False, pulp_labels=None, name=None, repository=None, repository_version=None, local_vars_configuration=None):  # noqa: E501
         """OstreeOstreeDistribution - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._base_path = None
         self._content_guard = None
+        self._hidden = None
         self._pulp_labels = None
         self._name = None
         self._repository = None
         self._repository_version = None
         self.discriminator = None
 
         self.base_path = base_path
         self.content_guard = content_guard
+        if hidden is not None:
+            self.hidden = hidden
         if pulp_labels is not None:
             self.pulp_labels = pulp_labels
         self.name = name
         self.repository = repository
         self.repository_version = repository_version
 
     @property
@@ -121,14 +126,37 @@
         :param content_guard: The content_guard of this OstreeOstreeDistribution.  # noqa: E501
         :type: str
         """
 
         self._content_guard = content_guard
 
     @property
+    def hidden(self):
+        """Gets the hidden of this OstreeOstreeDistribution.  # noqa: E501
+
+        Whether this distribution should be shown in the content app.  # noqa: E501
+
+        :return: The hidden of this OstreeOstreeDistribution.  # noqa: E501
+        :rtype: bool
+        """
+        return self._hidden
+
+    @hidden.setter
+    def hidden(self, hidden):
+        """Sets the hidden of this OstreeOstreeDistribution.
+
+        Whether this distribution should be shown in the content app.  # noqa: E501
+
+        :param hidden: The hidden of this OstreeOstreeDistribution.  # noqa: E501
+        :type: bool
+        """
+
+        self._hidden = hidden
+
+    @property
     def pulp_labels(self):
         """Gets the pulp_labels of this OstreeOstreeDistribution.  # noqa: E501
 
 
         :return: The pulp_labels of this OstreeOstreeDistribution.  # noqa: E501
         :rtype: dict(str, str)
         """
```

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution_response.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,57 +35,62 @@
     """
     openapi_types = {
         'pulp_href': 'str',
         'pulp_created': 'datetime',
         'base_path': 'str',
         'base_url': 'str',
         'content_guard': 'str',
+        'hidden': 'bool',
         'pulp_labels': 'dict(str, str)',
         'name': 'str',
         'repository': 'str',
         'repository_version': 'str'
     }
 
     attribute_map = {
         'pulp_href': 'pulp_href',
         'pulp_created': 'pulp_created',
         'base_path': 'base_path',
         'base_url': 'base_url',
         'content_guard': 'content_guard',
+        'hidden': 'hidden',
         'pulp_labels': 'pulp_labels',
         'name': 'name',
         'repository': 'repository',
         'repository_version': 'repository_version'
     }
 
-    def __init__(self, pulp_href=None, pulp_created=None, base_path=None, base_url=None, content_guard=None, pulp_labels=None, name=None, repository=None, repository_version=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, pulp_href=None, pulp_created=None, base_path=None, base_url=None, content_guard=None, hidden=False, pulp_labels=None, name=None, repository=None, repository_version=None, local_vars_configuration=None):  # noqa: E501
         """OstreeOstreeDistributionResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._pulp_href = None
         self._pulp_created = None
         self._base_path = None
         self._base_url = None
         self._content_guard = None
+        self._hidden = None
         self._pulp_labels = None
         self._name = None
         self._repository = None
         self._repository_version = None
         self.discriminator = None
 
         if pulp_href is not None:
             self.pulp_href = pulp_href
         if pulp_created is not None:
             self.pulp_created = pulp_created
         self.base_path = base_path
         if base_url is not None:
             self.base_url = base_url
         self.content_guard = content_guard
+        if hidden is not None:
+            self.hidden = hidden
         if pulp_labels is not None:
             self.pulp_labels = pulp_labels
         self.name = name
         self.repository = repository
         self.repository_version = repository_version
 
     @property
@@ -200,14 +205,37 @@
         :param content_guard: The content_guard of this OstreeOstreeDistributionResponse.  # noqa: E501
         :type: str
         """
 
         self._content_guard = content_guard
 
     @property
+    def hidden(self):
+        """Gets the hidden of this OstreeOstreeDistributionResponse.  # noqa: E501
+
+        Whether this distribution should be shown in the content app.  # noqa: E501
+
+        :return: The hidden of this OstreeOstreeDistributionResponse.  # noqa: E501
+        :rtype: bool
+        """
+        return self._hidden
+
+    @hidden.setter
+    def hidden(self, hidden):
+        """Sets the hidden of this OstreeOstreeDistributionResponse.
+
+        Whether this distribution should be shown in the content app.  # noqa: E501
+
+        :param hidden: The hidden of this OstreeOstreeDistributionResponse.  # noqa: E501
+        :type: bool
+        """
+
+        self._hidden = hidden
+
+    @property
     def pulp_labels(self):
         """Gets the pulp_labels of this OstreeOstreeDistributionResponse.  # noqa: E501
 
 
         :return: The pulp_labels of this OstreeOstreeDistributionResponse.  # noqa: E501
         :rtype: dict(str, str)
         """
```

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_object_response.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_object_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_ref_response.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_ref_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_remote.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response_hidden_fields.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response_hidden_fields.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_repository.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_repository_response.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_summary_response.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/ostree_ostree_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginated_repository_version_response_list.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_commit_response_list.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_commit_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_config_response_list.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_config_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_content_response_list.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_content_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_distribution_response_list.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_object_response_list.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_object_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_ref_response_list.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_ref_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_remote_response_list.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_repository_response_list.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_summary_response_list.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_summary_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/patchedostree_ostree_distribution.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/patchedostree_ostree_distribution.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,46 +32,51 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'base_path': 'str',
         'content_guard': 'str',
+        'hidden': 'bool',
         'pulp_labels': 'dict(str, str)',
         'name': 'str',
         'repository': 'str',
         'repository_version': 'str'
     }
 
     attribute_map = {
         'base_path': 'base_path',
         'content_guard': 'content_guard',
+        'hidden': 'hidden',
         'pulp_labels': 'pulp_labels',
         'name': 'name',
         'repository': 'repository',
         'repository_version': 'repository_version'
     }
 
-    def __init__(self, base_path=None, content_guard=None, pulp_labels=None, name=None, repository=None, repository_version=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, base_path=None, content_guard=None, hidden=False, pulp_labels=None, name=None, repository=None, repository_version=None, local_vars_configuration=None):  # noqa: E501
         """PatchedostreeOstreeDistribution - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._base_path = None
         self._content_guard = None
+        self._hidden = None
         self._pulp_labels = None
         self._name = None
         self._repository = None
         self._repository_version = None
         self.discriminator = None
 
         if base_path is not None:
             self.base_path = base_path
         self.content_guard = content_guard
+        if hidden is not None:
+            self.hidden = hidden
         if pulp_labels is not None:
             self.pulp_labels = pulp_labels
         if name is not None:
             self.name = name
         self.repository = repository
         self.repository_version = repository_version
 
@@ -121,14 +126,37 @@
         :param content_guard: The content_guard of this PatchedostreeOstreeDistribution.  # noqa: E501
         :type: str
         """
 
         self._content_guard = content_guard
 
     @property
+    def hidden(self):
+        """Gets the hidden of this PatchedostreeOstreeDistribution.  # noqa: E501
+
+        Whether this distribution should be shown in the content app.  # noqa: E501
+
+        :return: The hidden of this PatchedostreeOstreeDistribution.  # noqa: E501
+        :rtype: bool
+        """
+        return self._hidden
+
+    @hidden.setter
+    def hidden(self, hidden):
+        """Sets the hidden of this PatchedostreeOstreeDistribution.
+
+        Whether this distribution should be shown in the content app.  # noqa: E501
+
+        :param hidden: The hidden of this PatchedostreeOstreeDistribution.  # noqa: E501
+        :type: bool
+        """
+
+        self._hidden = hidden
+
+    @property
     def pulp_labels(self):
         """Gets the pulp_labels of this PatchedostreeOstreeDistribution.  # noqa: E501
 
 
         :return: The pulp_labels of this PatchedostreeOstreeDistribution.  # noqa: E501
         :rtype: dict(str, str)
         """
```

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/patchedostree_ostree_remote.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/patchedostree_ostree_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/patchedostree_ostree_repository.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/patchedostree_ostree_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/policy_enum.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repair.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/repair.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repository_add_remove_content.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repository_sync_url.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repository_version_response.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/models/repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/rest.py` & `pulp_ostree-client-2.1.1/pulpcore/client/pulp_ostree/rest.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/setup.py` & `pulp_ostree-client-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pulp_ostree-client"
-VERSION = "2.1.0"
+VERSION = "2.1.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pulp_ostree-client-2.1.0/test/test_async_operation_response.py` & `pulp_ostree-client-2.1.1/test/test_async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_content_commits_api.py` & `pulp_ostree-client-2.1.1/test/test_content_commits_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_content_configs_api.py` & `pulp_ostree-client-2.1.1/test/test_content_configs_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_content_content_api.py` & `pulp_ostree-client-2.1.1/test/test_content_content_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_content_objects_api.py` & `pulp_ostree-client-2.1.1/test/test_content_objects_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_content_refs_api.py` & `pulp_ostree-client-2.1.1/test/test_content_refs_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_content_summaries_api.py` & `pulp_ostree-client-2.1.1/test/test_content_summaries_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_content_summary_response.py` & `pulp_ostree-client-2.1.1/test/test_content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_distributions_ostree_api.py` & `pulp_ostree-client-2.1.1/test/test_distributions_ostree_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_ostree_import_all.py` & `pulp_ostree-client-2.1.1/test/test_ostree_import_all.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_ostree_import_commits_to_ref.py` & `pulp_ostree-client-2.1.1/test/test_ostree_import_commits_to_ref.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_ostree_ostree_commit_response.py` & `pulp_ostree-client-2.1.1/test/test_ostree_ostree_commit_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_ostree_ostree_config_response.py` & `pulp_ostree-client-2.1.1/test/test_ostree_ostree_config_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_ostree_ostree_content_response.py` & `pulp_ostree-client-2.1.1/test/test_ostree_ostree_content_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_ostree_ostree_distribution.py` & `pulp_ostree-client-2.1.1/test/test_ostree_ostree_distribution.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             params are included, when True both required and
             optional params are included """
         # model = pulpcore.client.pulp_ostree.models.ostree_ostree_distribution.OstreeOstreeDistribution()  # noqa: E501
         if include_optional :
             return OstreeOstreeDistribution(
                 base_path = '0', 
                 content_guard = '0', 
+                hidden = True, 
                 pulp_labels = {
                     'key' : '0'
                     }, 
                 name = '0', 
                 repository = '0', 
                 repository_version = '0'
             )
```

### Comparing `pulp_ostree-client-2.1.0/test/test_ostree_ostree_distribution_response.py` & `pulp_ostree-client-2.1.1/test/test_ostree_ostree_distribution_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         if include_optional :
             return OstreeOstreeDistributionResponse(
                 pulp_href = '0', 
                 pulp_created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 base_path = '0', 
                 base_url = '0', 
                 content_guard = '0', 
+                hidden = True, 
                 pulp_labels = {
                     'key' : '0'
                     }, 
                 name = '0', 
                 repository = '0', 
                 repository_version = '0'
             )
```

### Comparing `pulp_ostree-client-2.1.0/test/test_ostree_ostree_object_response.py` & `pulp_ostree-client-2.1.1/test/test_ostree_ostree_object_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_ostree_ostree_ref_response.py` & `pulp_ostree-client-2.1.1/test/test_ostree_ostree_ref_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_ostree_ostree_remote.py` & `pulp_ostree-client-2.1.1/test/test_ostree_ostree_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_ostree_ostree_remote_response.py` & `pulp_ostree-client-2.1.1/test/test_ostree_ostree_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_ostree_ostree_remote_response_hidden_fields.py` & `pulp_ostree-client-2.1.1/test/test_ostree_ostree_remote_response_hidden_fields.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_ostree_ostree_repository.py` & `pulp_ostree-client-2.1.1/test/test_ostree_ostree_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_ostree_ostree_repository_response.py` & `pulp_ostree-client-2.1.1/test/test_ostree_ostree_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_ostree_ostree_summary_response.py` & `pulp_ostree-client-2.1.1/test/test_ostree_ostree_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_paginated_repository_version_response_list.py` & `pulp_ostree-client-2.1.1/test/test_paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_commit_response_list.py` & `pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_commit_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_config_response_list.py` & `pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_config_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_content_response_list.py` & `pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_content_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_distribution_response_list.py` & `pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_distribution_response_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
                 results = [
                     pulpcore.client.pulp_ostree.models.ostree/ostree_distribution_response.ostree.OstreeDistributionResponse(
                         pulp_href = '0', 
                         pulp_created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         base_path = '0', 
                         base_url = '0', 
                         content_guard = '0', 
+                        hidden = True, 
                         pulp_labels = {
                             'key' : '0'
                             }, 
                         name = '0', 
                         repository = '0', 
                         repository_version = '0', )
                     ]
```

### Comparing `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_object_response_list.py` & `pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_object_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_ref_response_list.py` & `pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_ref_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_remote_response_list.py` & `pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_repository_response_list.py` & `pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_summary_response_list.py` & `pulp_ostree-client-2.1.1/test/test_paginatedostree_ostree_summary_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_patchedostree_ostree_distribution.py` & `pulp_ostree-client-2.1.1/test/test_patchedostree_ostree_distribution.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             params are included, when True both required and
             optional params are included """
         # model = pulpcore.client.pulp_ostree.models.patchedostree_ostree_distribution.PatchedostreeOstreeDistribution()  # noqa: E501
         if include_optional :
             return PatchedostreeOstreeDistribution(
                 base_path = '0', 
                 content_guard = '0', 
+                hidden = True, 
                 pulp_labels = {
                     'key' : '0'
                     }, 
                 name = '0', 
                 repository = '0', 
                 repository_version = '0'
             )
```

### Comparing `pulp_ostree-client-2.1.0/test/test_patchedostree_ostree_remote.py` & `pulp_ostree-client-2.1.1/test/test_patchedostree_ostree_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_patchedostree_ostree_repository.py` & `pulp_ostree-client-2.1.1/test/test_patchedostree_ostree_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_policy_enum.py` & `pulp_ostree-client-2.1.1/test/test_policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_remotes_ostree_api.py` & `pulp_ostree-client-2.1.1/test/test_remotes_ostree_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_repair.py` & `pulp_ostree-client-2.1.1/test/test_repair.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_repositories_ostree_api.py` & `pulp_ostree-client-2.1.1/test/test_repositories_ostree_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_repositories_ostree_versions_api.py` & `pulp_ostree-client-2.1.1/test/test_repositories_ostree_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_repository_add_remove_content.py` & `pulp_ostree-client-2.1.1/test/test_repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_repository_sync_url.py` & `pulp_ostree-client-2.1.1/test/test_repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.1.0/test/test_repository_version_response.py` & `pulp_ostree-client-2.1.1/test/test_repository_version_response.py`

 * *Files identical despite different names*


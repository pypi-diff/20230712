# Comparing `tmp/pyontutils-0.1.8.tar.gz` & `tmp/pyontutils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyontutils-0.1.8.tar", last modified: Mon Nov 25 22:55:29 2019, max compression
+gzip compressed data, was "dist/pyontutils-0.1.9.tar", last modified: Thu Dec  5 01:09:05 2019, max compression
```

## Comparing `pyontutils-0.1.8.tar` & `pyontutils-0.1.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-11-25 22:55:29.000000 pyontutils-0.1.8/
--rw-r--r--   0 tom       (1000) tom       (1000)     1085 2019-10-30 06:48:34.000000 pyontutils-0.1.8/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     7833 2019-11-25 22:55:29.000000 pyontutils-0.1.8/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      674 2019-11-10 01:27:50.000000 pyontutils-0.1.8/Pipfile
--rw-r--r--   0 tom       (1000) tom       (1000)     6143 2019-10-30 06:48:34.000000 pyontutils-0.1.8/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-11-25 22:55:29.000000 pyontutils-0.1.8/docs/
--rw-r--r--   0 tom       (1000) tom       (1000)    15013 2019-11-25 22:55:29.000000 pyontutils-0.1.8/docs/release.org
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-11-25 22:55:29.000000 pyontutils-0.1.8/nifstd/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-11-25 22:55:29.000000 pyontutils-0.1.8/nifstd/scigraph/
--rw-r--r--   0 tom       (1000) tom       (1000)     8111 2019-11-25 22:55:29.000000 pyontutils-0.1.8/nifstd/scigraph/curie_map.yaml
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-11-25 22:55:29.000000 pyontutils-0.1.8/pyontutils/
--rw-r--r--   0 tom       (1000) tom       (1000)       22 2019-11-25 22:55:29.000000 pyontutils-0.1.8/pyontutils/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2125 2019-10-30 06:48:34.000000 pyontutils-0.1.8/pyontutils/annotation.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2329 2019-11-25 22:55:29.000000 pyontutils-0.1.8/pyontutils/auth-config.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4493 2019-10-30 06:48:34.000000 pyontutils-0.1.8/pyontutils/clifun.py
--rw-r--r--   0 tom       (1000) tom       (1000)    17096 2019-11-10 01:27:50.000000 pyontutils-0.1.8/pyontutils/closed_namespaces.py
--rw-r--r--   0 tom       (1000) tom       (1000)    32483 2019-11-10 01:27:50.000000 pyontutils-0.1.8/pyontutils/combinators.py
--rw-r--r--   0 tom       (1000) tom       (1000)    13528 2019-11-12 10:00:29.000000 pyontutils-0.1.8/pyontutils/config.py
--rw-r--r--   0 tom       (1000) tom       (1000)    93395 2019-11-14 08:12:21.000000 pyontutils-0.1.8/pyontutils/core.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    23536 2019-11-12 10:00:29.000000 pyontutils-0.1.8/pyontutils/graphml_to_ttl.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    26822 2019-11-12 10:00:29.000000 pyontutils-0.1.8/pyontutils/hierarchies.py
--rw-r--r--   0 tom       (1000) tom       (1000)    20267 2019-10-30 06:48:34.000000 pyontutils-0.1.8/pyontutils/identity_bnode.py
--rw-r--r--   0 tom       (1000) tom       (1000)    12594 2019-11-10 01:27:50.000000 pyontutils-0.1.8/pyontutils/integration_test_helper.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     3193 2019-11-12 10:00:29.000000 pyontutils-0.1.8/pyontutils/make_catalog.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1409 2019-11-10 01:27:50.000000 pyontutils-0.1.8/pyontutils/map-identifiers.py
--rw-r--r--   0 tom       (1000) tom       (1000)    12755 2019-11-25 22:55:29.000000 pyontutils-0.1.8/pyontutils/namespaces.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     5996 2019-11-12 10:00:29.000000 pyontutils-0.1.8/pyontutils/necromancy.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    44426 2019-10-30 06:48:34.000000 pyontutils-0.1.8/pyontutils/obo_io.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    33669 2019-11-12 10:00:29.000000 pyontutils-0.1.8/pyontutils/ontload.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    34100 2019-11-10 01:27:50.000000 pyontutils-0.1.8/pyontutils/ontutils.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     1479 2019-10-30 06:48:34.000000 pyontutils-0.1.8/pyontutils/overlaps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1177 2019-10-30 06:48:34.000000 pyontutils-0.1.8/pyontutils/process_fixed.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     3611 2019-10-30 06:48:34.000000 pyontutils-0.1.8/pyontutils/qnamefix.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     7063 2019-10-30 06:48:34.000000 pyontutils-0.1.8/pyontutils/rdflib_profile.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    14430 2019-11-12 10:00:29.000000 pyontutils-0.1.8/pyontutils/scig.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1445 2019-11-10 01:27:50.000000 pyontutils-0.1.8/pyontutils/scigraph.py
--rw-r--r--   0 tom       (1000) tom       (1000)    87715 2019-11-10 01:27:50.000000 pyontutils-0.1.8/pyontutils/scigraph_client.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    31234 2019-11-12 10:00:29.000000 pyontutils-0.1.8/pyontutils/scigraph_codegen.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    35926 2019-11-12 10:00:29.000000 pyontutils-0.1.8/pyontutils/scigraph_deploy.py
--rw-r--r--   0 tom       (1000) tom       (1000)    11432 2019-11-10 01:27:50.000000 pyontutils-0.1.8/pyontutils/sheets.py
--rw-r--r--   0 tom       (1000) tom       (1000)    24266 2019-10-30 06:48:34.000000 pyontutils-0.1.8/pyontutils/utils.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2517 2019-10-30 06:48:34.000000 pyontutils-0.1.8/pyontutils/utils_extra.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-11-25 22:55:29.000000 pyontutils-0.1.8/pyontutils.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     7833 2019-11-25 22:55:29.000000 pyontutils-0.1.8/pyontutils.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1376 2019-11-25 22:55:29.000000 pyontutils-0.1.8/pyontutils.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2019-11-25 22:55:29.000000 pyontutils-0.1.8/pyontutils.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      422 2019-11-25 22:55:29.000000 pyontutils-0.1.8/pyontutils.egg-info/entry_points.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      288 2019-11-25 22:55:29.000000 pyontutils-0.1.8/pyontutils.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       11 2019-11-25 22:55:29.000000 pyontutils-0.1.8/pyontutils.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      166 2019-11-25 22:55:29.000000 pyontutils-0.1.8/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     2877 2019-11-25 22:55:29.000000 pyontutils-0.1.8/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-11-25 22:55:29.000000 pyontutils-0.1.8/test/
--rw-r--r--   0 tom       (1000) tom       (1000)       18 2019-11-10 01:27:50.000000 pyontutils-0.1.8/test/.gitignore
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-10-30 06:48:34.000000 pyontutils-0.1.8/test/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      258 2019-11-10 01:27:50.000000 pyontutils-0.1.8/test/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)   414630 2019-10-30 06:48:34.000000 pyontutils-0.1.8/test/prefix.ttl
--rw-r--r--   0 tom       (1000) tom       (1000)      480 2019-10-30 06:48:34.000000 pyontutils-0.1.8/test/test_cli.py
--rw-r--r--   0 tom       (1000) tom       (1000)      334 2019-10-30 06:48:34.000000 pyontutils-0.1.8/test/test_clifun.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1596 2019-11-12 10:00:29.000000 pyontutils-0.1.8/test/test_config.py
--rw-r--r--   0 tom       (1000) tom       (1000)      990 2019-10-30 06:48:34.000000 pyontutils-0.1.8/test/test_core.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7667 2019-11-10 01:27:50.000000 pyontutils-0.1.8/test/test_ibnode.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4706 2019-11-14 00:30:16.000000 pyontutils-0.1.8/test/test_integration.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1448 2019-10-30 06:48:34.000000 pyontutils-0.1.8/test/test_oboio.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1617 2019-10-30 06:48:34.000000 pyontutils-0.1.8/test/test_ontgraph.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1831 2019-11-10 01:27:50.000000 pyontutils-0.1.8/test/test_streams.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1745 2019-10-30 06:48:34.000000 pyontutils-0.1.8/test/test_utils.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-11-25 22:55:29.000000 pyontutils-0.1.8/ttlser/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-11-25 22:55:29.000000 pyontutils-0.1.8/ttlser/test/
--rw-r--r--   0 tom       (1000) tom       (1000)    15442 2019-10-30 06:48:34.000000 pyontutils-0.1.8/ttlser/test/nasty.ttl
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-05 01:09:05.000000 pyontutils-0.1.9/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1085 2019-10-30 06:48:34.000000 pyontutils-0.1.9/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)     7833 2019-12-05 01:09:05.000000 pyontutils-0.1.9/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      674 2019-11-10 01:27:50.000000 pyontutils-0.1.9/Pipfile
+-rw-r--r--   0 tom       (1000) tom       (1000)     6143 2019-10-30 06:48:34.000000 pyontutils-0.1.9/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-05 01:09:05.000000 pyontutils-0.1.9/docs/
+-rw-r--r--   0 tom       (1000) tom       (1000)    15013 2019-11-25 22:55:29.000000 pyontutils-0.1.9/docs/release.org
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-05 01:09:05.000000 pyontutils-0.1.9/nifstd/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-05 01:09:05.000000 pyontutils-0.1.9/nifstd/scigraph/
+-rw-r--r--   0 tom       (1000) tom       (1000)     8111 2019-11-25 22:55:29.000000 pyontutils-0.1.9/nifstd/scigraph/curie_map.yaml
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-05 01:09:05.000000 pyontutils-0.1.9/pyontutils/
+-rw-r--r--   0 tom       (1000) tom       (1000)       22 2019-12-05 01:09:04.000000 pyontutils-0.1.9/pyontutils/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2125 2019-10-30 06:48:34.000000 pyontutils-0.1.9/pyontutils/annotation.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2329 2019-11-25 22:55:29.000000 pyontutils-0.1.9/pyontutils/auth-config.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4493 2019-10-30 06:48:34.000000 pyontutils-0.1.9/pyontutils/clifun.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    17096 2019-11-10 01:27:50.000000 pyontutils-0.1.9/pyontutils/closed_namespaces.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    32483 2019-11-10 01:27:50.000000 pyontutils-0.1.9/pyontutils/combinators.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    13528 2019-11-12 10:00:29.000000 pyontutils-0.1.9/pyontutils/config.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    93395 2019-11-14 08:12:21.000000 pyontutils-0.1.9/pyontutils/core.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    23536 2019-11-12 10:00:29.000000 pyontutils-0.1.9/pyontutils/graphml_to_ttl.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    26822 2019-11-12 10:00:29.000000 pyontutils-0.1.9/pyontutils/hierarchies.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    20267 2019-10-30 06:48:34.000000 pyontutils-0.1.9/pyontutils/identity_bnode.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    12594 2019-11-10 01:27:50.000000 pyontutils-0.1.9/pyontutils/integration_test_helper.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     3193 2019-11-12 10:00:29.000000 pyontutils-0.1.9/pyontutils/make_catalog.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1409 2019-11-10 01:27:50.000000 pyontutils-0.1.9/pyontutils/map-identifiers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    12760 2019-12-05 01:08:21.000000 pyontutils-0.1.9/pyontutils/namespaces.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     5996 2019-11-12 10:00:29.000000 pyontutils-0.1.9/pyontutils/necromancy.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    44426 2019-10-30 06:48:34.000000 pyontutils-0.1.9/pyontutils/obo_io.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    33669 2019-11-12 10:00:29.000000 pyontutils-0.1.9/pyontutils/ontload.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    34100 2019-11-10 01:27:50.000000 pyontutils-0.1.9/pyontutils/ontutils.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     1479 2019-10-30 06:48:34.000000 pyontutils-0.1.9/pyontutils/overlaps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1177 2019-10-30 06:48:34.000000 pyontutils-0.1.9/pyontutils/process_fixed.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     3611 2019-10-30 06:48:34.000000 pyontutils-0.1.9/pyontutils/qnamefix.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     7063 2019-10-30 06:48:34.000000 pyontutils-0.1.9/pyontutils/rdflib_profile.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    14430 2019-11-12 10:00:29.000000 pyontutils-0.1.9/pyontutils/scig.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1445 2019-11-10 01:27:50.000000 pyontutils-0.1.9/pyontutils/scigraph.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    87715 2019-11-10 01:27:50.000000 pyontutils-0.1.9/pyontutils/scigraph_client.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    31234 2019-11-12 10:00:29.000000 pyontutils-0.1.9/pyontutils/scigraph_codegen.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    35926 2019-11-12 10:00:29.000000 pyontutils-0.1.9/pyontutils/scigraph_deploy.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    11432 2019-11-10 01:27:50.000000 pyontutils-0.1.9/pyontutils/sheets.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    24291 2019-12-05 01:08:21.000000 pyontutils-0.1.9/pyontutils/utils.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2517 2019-10-30 06:48:34.000000 pyontutils-0.1.9/pyontutils/utils_extra.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-05 01:09:05.000000 pyontutils-0.1.9/pyontutils.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     7833 2019-12-05 01:09:04.000000 pyontutils-0.1.9/pyontutils.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1376 2019-12-05 01:09:05.000000 pyontutils-0.1.9/pyontutils.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2019-12-05 01:09:04.000000 pyontutils-0.1.9/pyontutils.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      422 2019-12-05 01:09:04.000000 pyontutils-0.1.9/pyontutils.egg-info/entry_points.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      288 2019-12-05 01:09:04.000000 pyontutils-0.1.9/pyontutils.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       11 2019-12-05 01:09:04.000000 pyontutils-0.1.9/pyontutils.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      166 2019-12-05 01:09:05.000000 pyontutils-0.1.9/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)     2877 2019-11-25 22:55:29.000000 pyontutils-0.1.9/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-05 01:09:05.000000 pyontutils-0.1.9/test/
+-rw-r--r--   0 tom       (1000) tom       (1000)       18 2019-11-10 01:27:50.000000 pyontutils-0.1.9/test/.gitignore
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-10-30 06:48:34.000000 pyontutils-0.1.9/test/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      258 2019-11-10 01:27:50.000000 pyontutils-0.1.9/test/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)   414630 2019-10-30 06:48:34.000000 pyontutils-0.1.9/test/prefix.ttl
+-rw-r--r--   0 tom       (1000) tom       (1000)      480 2019-10-30 06:48:34.000000 pyontutils-0.1.9/test/test_cli.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      334 2019-10-30 06:48:34.000000 pyontutils-0.1.9/test/test_clifun.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1596 2019-11-12 10:00:29.000000 pyontutils-0.1.9/test/test_config.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      990 2019-10-30 06:48:34.000000 pyontutils-0.1.9/test/test_core.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7667 2019-11-10 01:27:50.000000 pyontutils-0.1.9/test/test_ibnode.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4706 2019-11-14 00:30:16.000000 pyontutils-0.1.9/test/test_integration.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1448 2019-10-30 06:48:34.000000 pyontutils-0.1.9/test/test_oboio.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1617 2019-10-30 06:48:34.000000 pyontutils-0.1.9/test/test_ontgraph.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1831 2019-11-10 01:27:50.000000 pyontutils-0.1.9/test/test_streams.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1745 2019-10-30 06:48:34.000000 pyontutils-0.1.9/test/test_utils.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-05 01:09:05.000000 pyontutils-0.1.9/ttlser/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-05 01:09:05.000000 pyontutils-0.1.9/ttlser/test/
+-rw-r--r--   0 tom       (1000) tom       (1000)    15442 2019-10-30 06:48:34.000000 pyontutils-0.1.9/ttlser/test/nasty.ttl
```

### Comparing `pyontutils-0.1.8/LICENSE` & `pyontutils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/PKG-INFO` & `pyontutils-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyontutils
-Version: 0.1.8
+Version: 0.1.9
 Summary: utilities for working with the NIF ontology, SciGraph, and turtle
 Home-page: https://github.com/tgbugs/pyontutils
 Author: Tom Gillespie
 Author-email: tgbugs@gmail.com
 License: MIT
 Description: # pyontutils
         [![PyPI version](https://badge.fury.io/py/pyontutils.svg)](https://pypi.org/project/pyontutils/)
```

### Comparing `pyontutils-0.1.8/Pipfile` & `pyontutils-0.1.9/Pipfile`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/README.md` & `pyontutils-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/docs/release.org` & `pyontutils-0.1.9/docs/release.org`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/nifstd/scigraph/curie_map.yaml` & `pyontutils-0.1.9/nifstd/scigraph/curie_map.yaml`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/annotation.py` & `pyontutils-0.1.9/pyontutils/annotation.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/auth-config.py` & `pyontutils-0.1.9/pyontutils/auth-config.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/clifun.py` & `pyontutils-0.1.9/pyontutils/clifun.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/closed_namespaces.py` & `pyontutils-0.1.9/pyontutils/closed_namespaces.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/combinators.py` & `pyontutils-0.1.9/pyontutils/combinators.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/config.py` & `pyontutils-0.1.9/pyontutils/config.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/core.py` & `pyontutils-0.1.9/pyontutils/core.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/graphml_to_ttl.py` & `pyontutils-0.1.9/pyontutils/graphml_to_ttl.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/hierarchies.py` & `pyontutils-0.1.9/pyontutils/hierarchies.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/identity_bnode.py` & `pyontutils-0.1.9/pyontutils/identity_bnode.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/integration_test_helper.py` & `pyontutils-0.1.9/pyontutils/integration_test_helper.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/make_catalog.py` & `pyontutils-0.1.9/pyontutils/make_catalog.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/map-identifiers.py` & `pyontutils-0.1.9/pyontutils/map-identifiers.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/namespaces.py` & `pyontutils-0.1.9/pyontutils/namespaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 
         'PROTEGE':'http://protege.stanford.edu/plugins/owl/protege#',
         'TEMP': interlex_namespace('temp/uris/'),
         'TEMPRAW': interlex_namespace('temp/uris/raw/'),
         'TEMPIND': interlex_namespace('temp/uris/phenotype-indicators/'),
         'lex': str(lex),
         'npokb': str(npokb),
-        'tech': interlex_namespace('tgbugs/readable/technique/'),
+        'tech': interlex_namespace('tgbugs/uris/readable/technique/'),
         'FIXME':'http://FIXME.org/',
         'NIFRAW':'https://raw.githubusercontent.com/SciCrunch/NIF-Ontology/',
         'NIFTTL':'http://ontology.neuinfo.org/NIF/ttl/',
         'NIFRET':'http://ontology.neuinfo.org/NIF/Retired/NIF-Retired.owl#',
         'NLXWIKI':'http://neurolex.org/wiki/',
         # FIXME a thought: was # intentionally used to increase user privacy? or is this just happenstance?
         'nsu':'http://www.FIXME.org/nsupper#',
```

### Comparing `pyontutils-0.1.8/pyontutils/necromancy.py` & `pyontutils-0.1.9/pyontutils/necromancy.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/obo_io.py` & `pyontutils-0.1.9/pyontutils/obo_io.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/ontload.py` & `pyontutils-0.1.9/pyontutils/ontload.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/ontutils.py` & `pyontutils-0.1.9/pyontutils/ontutils.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/overlaps.py` & `pyontutils-0.1.9/pyontutils/overlaps.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/process_fixed.py` & `pyontutils-0.1.9/pyontutils/process_fixed.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/qnamefix.py` & `pyontutils-0.1.9/pyontutils/qnamefix.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/rdflib_profile.py` & `pyontutils-0.1.9/pyontutils/rdflib_profile.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/scig.py` & `pyontutils-0.1.9/pyontutils/scig.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/scigraph.py` & `pyontutils-0.1.9/pyontutils/scigraph.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/scigraph_client.py` & `pyontutils-0.1.9/pyontutils/scigraph_client.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/scigraph_codegen.py` & `pyontutils-0.1.9/pyontutils/scigraph_codegen.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/scigraph_deploy.py` & `pyontutils-0.1.9/pyontutils/scigraph_deploy.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/sheets.py` & `pyontutils-0.1.9/pyontutils/sheets.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils/utils.py` & `pyontutils-0.1.9/pyontutils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,22 +200,23 @@
     else:
         index = -1
 
     return stack[index][0].f_locals
 
 
 def subclasses(start):
-    try:
-        for sc in start.__subclasses__():
-            if sc is not None:
-                yield sc
-                yield from subclasses(sc)
-    except TypeError as e:
-        log.exception(e)
+    if issubclass(start, type):
+        scs = start.__subclasses__(start)
+    else:
+        scs = start.__subclasses__()
 
+    for sc in scs:
+        if sc is not None:
+            yield sc
+            yield from subclasses(sc)
 
 
 def getSourceLine(cls):
     tc = TermColors
     try:
         return inspect.getsourcelines(cls)[-1]
     except OSError:  # we are probably in a debugger
```

### Comparing `pyontutils-0.1.8/pyontutils/utils_extra.py` & `pyontutils-0.1.9/pyontutils/utils_extra.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/pyontutils.egg-info/PKG-INFO` & `pyontutils-0.1.9/pyontutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyontutils
-Version: 0.1.8
+Version: 0.1.9
 Summary: utilities for working with the NIF ontology, SciGraph, and turtle
 Home-page: https://github.com/tgbugs/pyontutils
 Author: Tom Gillespie
 Author-email: tgbugs@gmail.com
 License: MIT
 Description: # pyontutils
         [![PyPI version](https://badge.fury.io/py/pyontutils.svg)](https://pypi.org/project/pyontutils/)
```

### Comparing `pyontutils-0.1.8/pyontutils.egg-info/SOURCES.txt` & `pyontutils-0.1.9/pyontutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/setup.py` & `pyontutils-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/test/prefix.ttl` & `pyontutils-0.1.9/test/prefix.ttl`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/test/test_config.py` & `pyontutils-0.1.9/test/test_config.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/test/test_core.py` & `pyontutils-0.1.9/test/test_core.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/test/test_ibnode.py` & `pyontutils-0.1.9/test/test_ibnode.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/test/test_integration.py` & `pyontutils-0.1.9/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/test/test_oboio.py` & `pyontutils-0.1.9/test/test_oboio.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/test/test_ontgraph.py` & `pyontutils-0.1.9/test/test_ontgraph.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/test/test_streams.py` & `pyontutils-0.1.9/test/test_streams.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/test/test_utils.py` & `pyontutils-0.1.9/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyontutils-0.1.8/ttlser/test/nasty.ttl` & `pyontutils-0.1.9/ttlser/test/nasty.ttl`

 * *Files identical despite different names*


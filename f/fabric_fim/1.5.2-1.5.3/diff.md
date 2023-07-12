# Comparing `tmp/fabric_fim-1.5.2.tar.gz` & `tmp/fabric_fim-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric_fim-1.5.2.tar", last modified: Sat Jun 17 00:16:08 2023, max compression
+gzip compressed data, was "fabric_fim-1.5.3.tar", last modified: Wed Jul 12 02:04:56 2023, max compression
```

## Comparing `fabric_fim-1.5.2.tar` & `fabric_fim-1.5.3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0     2208 2023-06-15 15:30:40.226765 fabric_fim-1.5.2/.gitignore
--rw-r--r--   0        0        0       26 2020-07-24 21:42:44.564662 fabric_fim-1.5.2/AUTHORS
--rw-r--r--   0        0        0     1071 2020-07-14 22:09:49.459777 fabric_fim-1.5.2/LICENSE
--rw-r--r--   0        0        0    11110 2023-06-15 15:20:12.737600 fabric_fim-1.5.2/README.md
--rw-r--r--   0        0        0    18690 2021-05-25 21:09:37.024101 fabric_fim-1.5.2/figs/fim-structure.png
--rw-r--r--   0        0        0      557 2021-03-15 22:13:52.784044 fabric_fim-1.5.2/fim/README.md
--rw-r--r--   0        0        0      103 2023-06-17 00:14:43.162647 fabric_fim-1.5.2/fim/__init__.py
--rw-r--r--   0        0        0        1 2022-04-27 22:22:19.299449 fabric_fim-1.5.2/fim/authz/__init__.py
--rw-r--r--   0        0        0    16139 2023-02-02 01:41:56.403069 fabric_fim-1.5.2/fim/authz/attribute_collector.py
--rw-r--r--   0        0        0      334 2020-09-12 23:24:52.369007 fabric_fim-1.5.2/fim/graph/README.md
--rw-r--r--   0        0        0        1 2020-09-02 18:31:38.004468 fabric_fim-1.5.2/fim/graph/__init__.py
--rw-r--r--   0        0        0    69843 2023-06-15 15:19:01.141154 fabric_fim-1.5.2/fim/graph/abc_property_graph.py
--rw-r--r--   0        0        0     4093 2023-02-02 01:41:56.406333 fabric_fim-1.5.2/fim/graph/abc_property_graph_constants.py
--rw-r--r--   0        0        0        1 2020-08-18 21:34:07.036009 fabric_fim-1.5.2/fim/graph/data/__init__.py
--rw-r--r--   0        0        0      283 2020-09-03 22:10:53.500264 fabric_fim-1.5.2/fim/graph/data/capacity_types.json
--rw-r--r--   0        0        0      100 2020-08-27 20:41:23.401941 fabric_fim-1.5.2/fim/graph/data/constraint_types.json
--rw-r--r--   0        0        0     3886 2023-06-15 15:19:01.141376 fabric_fim-1.5.2/fim/graph/data/graph_validation_rules.json
--rw-r--r--   0        0        0     3845 2023-06-15 15:19:01.141499 fabric_fim-1.5.2/fim/graph/data/graph_validation_rules_neo4j_v4.json
--rw-r--r--   0        0        0      547 2020-09-03 22:10:39.822590 fabric_fim-1.5.2/fim/graph/data/label_types.json
--rw-r--r--   0        0        0       91 2020-08-27 20:40:54.261031 fabric_fim-1.5.2/fim/graph/data/location_types.json
--rw-r--r--   0        0        0      861 2023-05-10 14:54:24.189132 fabric_fim-1.5.2/fim/graph/data/neo4j_indexes.json
--rw-r--r--   0        0        0     3320 2023-06-15 15:19:01.141615 fabric_fim-1.5.2/fim/graph/graph_util.py
--rw-r--r--   0        0        0    44293 2023-06-15 15:19:01.154588 fabric_fim-1.5.2/fim/graph/neo4j_property_graph.py
--rw-r--r--   0        0        0     6160 2022-10-06 17:38:08.214224 fabric_fim-1.5.2/fim/graph/networkx_mixin.py
--rw-r--r--   0        0        0    42211 2023-06-15 15:19:01.141889 fabric_fim-1.5.2/fim/graph/networkx_property_graph.py
--rw-r--r--   0        0        0     8354 2022-10-07 03:05:34.849246 fabric_fim-1.5.2/fim/graph/networkx_property_graph_disjoint.py
--rw-r--r--   0        0        0     1501 2021-03-15 22:13:52.788626 fabric_fim-1.5.2/fim/graph/resources/README.md
--rw-r--r--   0        0        0        1 2020-09-02 18:32:04.638774 fabric_fim-1.5.2/fim/graph/resources/__init__.py
--rw-r--r--   0        0        0     4484 2021-05-25 21:09:37.029370 fabric_fim-1.5.2/fim/graph/resources/abc_adm.py
--rw-r--r--   0        0        0    13570 2023-05-10 14:54:24.193783 fabric_fim-1.5.2/fim/graph/resources/abc_arm.py
--rw-r--r--   0        0        0     2991 2022-02-18 19:27:15.586527 fabric_fim-1.5.2/fim/graph/resources/abc_bqm.py
--rw-r--r--   0        0        0     4547 2021-03-31 01:14:29.518807 fabric_fim-1.5.2/fim/graph/resources/abc_cbm.py
--rw-r--r--   0        0        0     2297 2021-03-07 22:42:30.018249 fabric_fim-1.5.2/fim/graph/resources/neo4j_adm.py
--rw-r--r--   0        0        0     2106 2021-05-25 21:09:37.031668 fabric_fim-1.5.2/fim/graph/resources/neo4j_arm.py
--rw-r--r--   0        0        0    18591 2023-06-15 15:19:01.148045 fabric_fim-1.5.2/fim/graph/resources/neo4j_cbm.py
--rw-r--r--   0        0        0     5017 2022-02-18 19:27:15.587881 fabric_fim-1.5.2/fim/graph/resources/networkx_abqm.py
--rw-r--r--   0        0        0     2341 2021-03-07 22:42:30.020154 fabric_fim-1.5.2/fim/graph/resources/networkx_adm.py
--rw-r--r--   0        0        0     2122 2021-05-25 21:09:37.033196 fabric_fim-1.5.2/fim/graph/resources/networkx_arm.py
--rw-r--r--   0        0        0      301 2021-03-15 22:13:52.789768 fabric_fim-1.5.2/fim/graph/slices/README.md
--rw-r--r--   0        0        0        1 2020-09-02 18:32:24.788341 fabric_fim-1.5.2/fim/graph/slices/__init__.py
--rw-r--r--   0        0        0     8223 2022-02-18 19:27:15.588460 fabric_fim-1.5.2/fim/graph/slices/abc_asm.py
--rw-r--r--   0        0        0     3733 2023-05-10 14:54:24.196715 fabric_fim-1.5.2/fim/graph/slices/neo4j_asm.py
--rw-r--r--   0        0        0     4298 2021-06-04 19:43:14.989790 fabric_fim-1.5.2/fim/graph/slices/networkx_asm.py
--rw-r--r--   0        0        0     8615 2021-03-03 19:57:54.288231 fabric_fim-1.5.2/fim/graph/typed_tuples.py
--rw-r--r--   0        0        0        0 2023-02-02 01:41:56.409002 fabric_fim-1.5.2/fim/logging/__init__.py
--rw-r--r--   0        0        0     1526 2023-06-15 15:19:01.033709 fabric_fim-1.5.2/fim/logging/fim_logger.py
--rw-r--r--   0        0        0     9071 2023-02-02 01:41:56.410072 fabric_fim-1.5.2/fim/logging/log_collector.py
--rw-r--r--   0        0        0     9555 2021-03-24 00:18:51.063382 fabric_fim-1.5.2/fim/pluggable.py
--rw-r--r--   0        0        0      189 2021-06-04 19:43:14.990352 fabric_fim-1.5.2/fim/slivers/README.md
--rw-r--r--   0        0        0      217 2021-06-14 18:36:21.931262 fabric_fim-1.5.2/fim/slivers/__init__.py
--rw-r--r--   0        0        0     3641 2023-02-02 01:41:56.410512 fabric_fim-1.5.2/fim/slivers/attached_components.py
--rw-r--r--   0        0        0    13021 2023-02-02 01:41:56.411041 fabric_fim-1.5.2/fim/slivers/base_sliver.py
--rw-r--r--   0        0        0    26010 2023-06-15 15:20:12.767056 fabric_fim-1.5.2/fim/slivers/capacities_labels.py
--rw-r--r--   0        0        0    11537 2023-06-13 15:16:11.169736 fabric_fim-1.5.2/fim/slivers/component_catalog.py
--rw-r--r--   0        0        0        1 2021-03-03 19:57:54.291739 fabric_fim-1.5.2/fim/slivers/data/__init__.py
--rw-r--r--   0        0        0     1691 2023-05-10 14:54:24.202981 fabric_fim-1.5.2/fim/slivers/data/component_catalog.json
--rw-r--r--   0        0        0    76943 2022-09-10 21:18:41.714675 fabric_fim-1.5.2/fim/slivers/data/instance_sizes.json
--rw-r--r--   0        0        0    23524 2022-02-18 19:27:15.591229 fabric_fim-1.5.2/fim/slivers/delegations.py
--rw-r--r--   0        0        0     3593 2022-02-18 19:27:15.591744 fabric_fim-1.5.2/fim/slivers/gateway.py
--rw-r--r--   0        0        0      919 2021-06-29 20:04:13.972162 fabric_fim-1.5.2/fim/slivers/identifiers.py
--rw-r--r--   0        0        0     3444 2022-02-18 19:27:15.592250 fabric_fim-1.5.2/fim/slivers/instance_catalog.py
--rw-r--r--   0        0        0     3225 2023-02-02 01:41:56.413360 fabric_fim-1.5.2/fim/slivers/interface_info.py
--rw-r--r--   0        0        0     2702 2021-09-22 14:46:40.423027 fabric_fim-1.5.2/fim/slivers/json.py
--rw-r--r--   0        0        0     3869 2023-02-02 01:41:56.413720 fabric_fim-1.5.2/fim/slivers/json_data.py
--rw-r--r--   0        0        0     5983 2023-02-02 01:41:56.414203 fabric_fim-1.5.2/fim/slivers/maintenance_mode.py
--rw-r--r--   0        0        0     1566 2021-03-03 19:57:54.294274 fabric_fim-1.5.2/fim/slivers/network_attached_storage.py
--rw-r--r--   0        0        0     3910 2023-02-02 01:41:56.414662 fabric_fim-1.5.2/fim/slivers/network_link.py
--rw-r--r--   0        0        0    10283 2023-06-16 22:13:30.912936 fabric_fim-1.5.2/fim/slivers/network_node.py
--rw-r--r--   0        0        0    22052 2023-06-16 22:05:08.616280 fabric_fim-1.5.2/fim/slivers/network_service.py
--rw-r--r--   0        0        0     6795 2021-06-04 19:43:14.993329 fabric_fim-1.5.2/fim/slivers/path_info.py
--rw-r--r--   0        0        0     3024 2022-02-18 19:27:15.594931 fabric_fim-1.5.2/fim/slivers/tags.py
--rw-r--r--   0        0        0     2622 2023-02-02 01:41:56.416090 fabric_fim-1.5.2/fim/slivers/topology_diff.py
--rw-r--r--   0        0        0     8706 2022-02-18 19:27:15.595505 fabric_fim-1.5.2/fim/user/README.md
--rw-r--r--   0        0        0     1914 2023-02-02 01:41:56.417286 fabric_fim-1.5.2/fim/user/__init__.py
--rw-r--r--   0        0        0    11730 2022-09-10 21:18:41.716394 fabric_fim-1.5.2/fim/user/component.py
--rw-r--r--   0        0        0     5668 2022-09-10 21:18:41.716675 fabric_fim-1.5.2/fim/user/composite_node.py
--rw-r--r--   0        0        0     7660 2023-02-02 01:41:56.418568 fabric_fim-1.5.2/fim/user/interface.py
--rw-r--r--   0        0        0     8381 2022-09-10 21:18:41.717280 fabric_fim-1.5.2/fim/user/link.py
--rw-r--r--   0        0        0     1219 2021-03-03 19:57:54.300001 fabric_fim-1.5.2/fim/user/measurement.py
--rw-r--r--   0        0        0     9668 2023-04-05 18:48:29.319327 fabric_fim-1.5.2/fim/user/model_element.py
--rw-r--r--   0        0        0    29219 2023-05-10 14:54:24.206616 fabric_fim-1.5.2/fim/user/network_service.py
--rw-r--r--   0        0        0    22636 2023-02-14 21:58:39.970039 fabric_fim-1.5.2/fim/user/node.py
--rw-r--r--   0        0        0    58158 2023-06-01 15:42:31.904936 fabric_fim-1.5.2/fim/user/topology.py
--rw-r--r--   0        0        0        2 2023-06-15 15:19:24.419545 fabric_fim-1.5.2/fim/util/__init__.py
--rw-r--r--   0        0        0    14139 2023-06-15 15:20:12.712509 fabric_fim-1.5.2/fim/util/fim_util.py
--rw-r--r--   0        0        0      595 2021-03-13 20:40:37.643107 fabric_fim-1.5.2/fim/view_only_dict.py
--rw-r--r--   0        0        0        0 2023-02-02 01:41:56.421372 fabric_fim-1.5.2/neo4j/data/.empty
--rw-r--r--   0        0        0        0 2023-02-02 01:41:56.421489 fabric_fim-1.5.2/neo4j/imports/.empty
--rw-r--r--   0        0        0      863 2023-06-15 15:20:12.720926 fabric_fim-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     4632 2022-03-09 00:58:31.583145 fabric_fim-1.5.2/test/ad_topology_test.py
--rw-r--r--   0        0        0     4834 2022-09-10 21:18:41.719406 fabric_fim-1.5.2/test/after.graphml
--rw-r--r--   0        0        0    17550 2023-06-15 15:20:12.731835 fabric_fim-1.5.2/test/attribute_collector_test.py
--rw-r--r--   0        0        0     4696 2022-09-10 21:18:41.719615 fabric_fim-1.5.2/test/before.graphml
--rw-r--r--   0        0        0     2729 2022-09-10 21:18:41.719876 fabric_fim-1.5.2/test/catalog_test.py
--rw-r--r--   0        0        0     4319 2022-02-18 19:27:15.602412 fabric_fim-1.5.2/test/delegation_label_test.py
--rw-r--r--   0        0        0     1653 2023-02-02 01:41:56.423551 fabric_fim-1.5.2/test/maintenance_test.py
--rw-r--r--   0        0        0    51613 2023-05-10 17:34:04.562843 fabric_fim-1.5.2/test/models/advertised_topo.graphml
--rw-r--r--   0        0        0    49696 2023-05-10 17:34:04.565992 fabric_fim-1.5.2/test/models/graph-template.graphml
--rw-r--r--   0        0        0    82994 2023-05-10 17:34:04.568753 fabric_fim-1.5.2/test/models/network-am-ad.graphml
--rw-r--r--   0        0        0    57411 2023-05-10 17:34:04.571919 fabric_fim-1.5.2/test/models/site-2-am-1broker-ad.graphml
--rw-r--r--   0        0        0    52887 2023-05-10 17:34:04.574274 fabric_fim-1.5.2/test/models/site-3-am-1broker-ad.graphml
--rw-r--r--   0        0        0   131407 2023-05-10 17:34:04.575177 fabric_fim-1.5.2/test/models/site-am-2broker-ad.graphml
--rw-r--r--   0        0        0    18708 2023-06-17 00:08:51.570025 fabric_fim-1.5.2/test/modify_test.py
--rw-r--r--   0        0        0    13135 2021-05-23 19:50:30.753072 fabric_fim-1.5.2/test/networkxx_pg_disjoint_test.py
--rw-r--r--   0        0        0    14091 2021-05-23 19:50:30.753595 fabric_fim-1.5.2/test/networkxx_pg_test.py
--rw-r--r--   0        0        0     2572 2021-03-24 00:18:51.064667 fabric_fim-1.5.2/test/pluggable_test.py
--rw-r--r--   0        0        0    42428 2023-06-15 15:20:12.777803 fabric_fim-1.5.2/test/slice_topology_test.py
--rw-r--r--   0        0        0     1869 2022-04-27 22:22:19.322857 fabric_fim-1.5.2/test/sliver_json_test.py
--rw-r--r--   0        0        0     6030 2023-06-15 15:20:12.763581 fabric_fim-1.5.2/test/sliver_test.py
--rw-r--r--   0        0        0    97162 2023-02-02 01:41:56.427682 fabric_fim-1.5.2/test/substrate_topology_test.py
--rw-r--r--   0        0        0      654 2022-02-18 19:27:15.604787 fabric_fim-1.5.2/test/test_load.py
--rw-r--r--   0        0        0     2362 2022-02-18 19:27:15.605244 fabric_fim-1.5.2/test/tuple_test.py
--rw-r--r--   0        0        0    15663 2023-06-15 15:19:01.186763 fabric_fim-1.5.2/test/zz_neo4j_pg_test.py
--rw-r--r--   0        0        0    11890 1970-01-01 00:00:00.000000 fabric_fim-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     2208 2023-06-29 20:04:50.927833 fabric_fim-1.5.3/.gitignore
+-rw-r--r--   0        0        0       26 2020-07-24 21:42:44.564662 fabric_fim-1.5.3/AUTHORS
+-rw-r--r--   0        0        0     1071 2020-07-14 22:09:49.459777 fabric_fim-1.5.3/LICENSE
+-rw-r--r--   0        0        0    11110 2023-06-29 20:04:50.929195 fabric_fim-1.5.3/README.md
+-rw-r--r--   0        0        0    18690 2021-05-25 21:09:37.024101 fabric_fim-1.5.3/figs/fim-structure.png
+-rw-r--r--   0        0        0      557 2021-03-15 22:13:52.784044 fabric_fim-1.5.3/fim/README.md
+-rw-r--r--   0        0        0      103 2023-07-12 02:03:41.054269 fabric_fim-1.5.3/fim/__init__.py
+-rw-r--r--   0        0        0        1 2022-04-27 22:22:19.299449 fabric_fim-1.5.3/fim/authz/__init__.py
+-rw-r--r--   0        0        0    16139 2023-02-02 01:41:56.403069 fabric_fim-1.5.3/fim/authz/attribute_collector.py
+-rw-r--r--   0        0        0      334 2020-09-12 23:24:52.369007 fabric_fim-1.5.3/fim/graph/README.md
+-rw-r--r--   0        0        0        1 2020-09-02 18:31:38.004468 fabric_fim-1.5.3/fim/graph/__init__.py
+-rw-r--r--   0        0        0    69843 2023-06-29 20:04:50.931915 fabric_fim-1.5.3/fim/graph/abc_property_graph.py
+-rw-r--r--   0        0        0     4093 2023-02-02 01:41:56.406333 fabric_fim-1.5.3/fim/graph/abc_property_graph_constants.py
+-rw-r--r--   0        0        0        1 2020-08-18 21:34:07.036009 fabric_fim-1.5.3/fim/graph/data/__init__.py
+-rw-r--r--   0        0        0      283 2020-09-03 22:10:53.500264 fabric_fim-1.5.3/fim/graph/data/capacity_types.json
+-rw-r--r--   0        0        0      100 2020-08-27 20:41:23.401941 fabric_fim-1.5.3/fim/graph/data/constraint_types.json
+-rw-r--r--   0        0        0     3886 2023-06-29 20:04:50.934312 fabric_fim-1.5.3/fim/graph/data/graph_validation_rules.json
+-rw-r--r--   0        0        0     3845 2023-06-29 20:04:50.935401 fabric_fim-1.5.3/fim/graph/data/graph_validation_rules_neo4j_v4.json
+-rw-r--r--   0        0        0      547 2020-09-03 22:10:39.822590 fabric_fim-1.5.3/fim/graph/data/label_types.json
+-rw-r--r--   0        0        0       91 2020-08-27 20:40:54.261031 fabric_fim-1.5.3/fim/graph/data/location_types.json
+-rw-r--r--   0        0        0      861 2023-05-10 14:54:24.189132 fabric_fim-1.5.3/fim/graph/data/neo4j_indexes.json
+-rw-r--r--   0        0        0     3320 2023-06-29 20:04:50.935954 fabric_fim-1.5.3/fim/graph/graph_util.py
+-rw-r--r--   0        0        0    44293 2023-06-29 20:04:50.936734 fabric_fim-1.5.3/fim/graph/neo4j_property_graph.py
+-rw-r--r--   0        0        0     6160 2022-10-06 17:38:08.214224 fabric_fim-1.5.3/fim/graph/networkx_mixin.py
+-rw-r--r--   0        0        0    42211 2023-06-29 20:04:50.937608 fabric_fim-1.5.3/fim/graph/networkx_property_graph.py
+-rw-r--r--   0        0        0     8354 2022-10-07 03:05:34.849246 fabric_fim-1.5.3/fim/graph/networkx_property_graph_disjoint.py
+-rw-r--r--   0        0        0     1501 2021-03-15 22:13:52.788626 fabric_fim-1.5.3/fim/graph/resources/README.md
+-rw-r--r--   0        0        0        1 2020-09-02 18:32:04.638774 fabric_fim-1.5.3/fim/graph/resources/__init__.py
+-rw-r--r--   0        0        0     4484 2021-05-25 21:09:37.029370 fabric_fim-1.5.3/fim/graph/resources/abc_adm.py
+-rw-r--r--   0        0        0    13570 2023-05-10 14:54:24.193783 fabric_fim-1.5.3/fim/graph/resources/abc_arm.py
+-rw-r--r--   0        0        0     2991 2022-02-18 19:27:15.586527 fabric_fim-1.5.3/fim/graph/resources/abc_bqm.py
+-rw-r--r--   0        0        0     5284 2023-07-12 02:03:15.009169 fabric_fim-1.5.3/fim/graph/resources/abc_cbm.py
+-rw-r--r--   0        0        0     2297 2021-03-07 22:42:30.018249 fabric_fim-1.5.3/fim/graph/resources/neo4j_adm.py
+-rw-r--r--   0        0        0     2106 2021-05-25 21:09:37.031668 fabric_fim-1.5.3/fim/graph/resources/neo4j_arm.py
+-rw-r--r--   0        0        0    20998 2023-07-12 02:01:38.603373 fabric_fim-1.5.3/fim/graph/resources/neo4j_cbm.py
+-rw-r--r--   0        0        0     5017 2022-02-18 19:27:15.587881 fabric_fim-1.5.3/fim/graph/resources/networkx_abqm.py
+-rw-r--r--   0        0        0     2341 2021-03-07 22:42:30.020154 fabric_fim-1.5.3/fim/graph/resources/networkx_adm.py
+-rw-r--r--   0        0        0     2122 2021-05-25 21:09:37.033196 fabric_fim-1.5.3/fim/graph/resources/networkx_arm.py
+-rw-r--r--   0        0        0      301 2021-03-15 22:13:52.789768 fabric_fim-1.5.3/fim/graph/slices/README.md
+-rw-r--r--   0        0        0        1 2020-09-02 18:32:24.788341 fabric_fim-1.5.3/fim/graph/slices/__init__.py
+-rw-r--r--   0        0        0     8223 2022-02-18 19:27:15.588460 fabric_fim-1.5.3/fim/graph/slices/abc_asm.py
+-rw-r--r--   0        0        0     3733 2023-05-10 14:54:24.196715 fabric_fim-1.5.3/fim/graph/slices/neo4j_asm.py
+-rw-r--r--   0        0        0     4298 2021-06-04 19:43:14.989790 fabric_fim-1.5.3/fim/graph/slices/networkx_asm.py
+-rw-r--r--   0        0        0     8615 2021-03-03 19:57:54.288231 fabric_fim-1.5.3/fim/graph/typed_tuples.py
+-rw-r--r--   0        0        0        0 2023-02-02 01:41:56.409002 fabric_fim-1.5.3/fim/logging/__init__.py
+-rw-r--r--   0        0        0     1526 2023-06-15 15:19:01.033709 fabric_fim-1.5.3/fim/logging/fim_logger.py
+-rw-r--r--   0        0        0     9071 2023-02-02 01:41:56.410072 fabric_fim-1.5.3/fim/logging/log_collector.py
+-rw-r--r--   0        0        0     9555 2021-03-24 00:18:51.063382 fabric_fim-1.5.3/fim/pluggable.py
+-rw-r--r--   0        0        0      189 2021-06-04 19:43:14.990352 fabric_fim-1.5.3/fim/slivers/README.md
+-rw-r--r--   0        0        0      217 2021-06-14 18:36:21.931262 fabric_fim-1.5.3/fim/slivers/__init__.py
+-rw-r--r--   0        0        0     3641 2023-02-02 01:41:56.410512 fabric_fim-1.5.3/fim/slivers/attached_components.py
+-rw-r--r--   0        0        0    13021 2023-02-02 01:41:56.411041 fabric_fim-1.5.3/fim/slivers/base_sliver.py
+-rw-r--r--   0        0        0    26010 2023-06-29 20:04:50.939407 fabric_fim-1.5.3/fim/slivers/capacities_labels.py
+-rw-r--r--   0        0        0    11537 2023-06-13 15:16:11.169736 fabric_fim-1.5.3/fim/slivers/component_catalog.py
+-rw-r--r--   0        0        0        1 2021-03-03 19:57:54.291739 fabric_fim-1.5.3/fim/slivers/data/__init__.py
+-rw-r--r--   0        0        0     1691 2023-05-10 14:54:24.202981 fabric_fim-1.5.3/fim/slivers/data/component_catalog.json
+-rw-r--r--   0        0        0    76943 2022-09-10 21:18:41.714675 fabric_fim-1.5.3/fim/slivers/data/instance_sizes.json
+-rw-r--r--   0        0        0    23524 2022-02-18 19:27:15.591229 fabric_fim-1.5.3/fim/slivers/delegations.py
+-rw-r--r--   0        0        0     3593 2022-02-18 19:27:15.591744 fabric_fim-1.5.3/fim/slivers/gateway.py
+-rw-r--r--   0        0        0      919 2021-06-29 20:04:13.972162 fabric_fim-1.5.3/fim/slivers/identifiers.py
+-rw-r--r--   0        0        0     3444 2022-02-18 19:27:15.592250 fabric_fim-1.5.3/fim/slivers/instance_catalog.py
+-rw-r--r--   0        0        0     3225 2023-02-02 01:41:56.413360 fabric_fim-1.5.3/fim/slivers/interface_info.py
+-rw-r--r--   0        0        0     2702 2021-09-22 14:46:40.423027 fabric_fim-1.5.3/fim/slivers/json.py
+-rw-r--r--   0        0        0     3869 2023-02-02 01:41:56.413720 fabric_fim-1.5.3/fim/slivers/json_data.py
+-rw-r--r--   0        0        0     5983 2023-02-02 01:41:56.414203 fabric_fim-1.5.3/fim/slivers/maintenance_mode.py
+-rw-r--r--   0        0        0     1566 2021-03-03 19:57:54.294274 fabric_fim-1.5.3/fim/slivers/network_attached_storage.py
+-rw-r--r--   0        0        0     3910 2023-02-02 01:41:56.414662 fabric_fim-1.5.3/fim/slivers/network_link.py
+-rw-r--r--   0        0        0    10283 2023-06-29 20:04:50.940050 fabric_fim-1.5.3/fim/slivers/network_node.py
+-rw-r--r--   0        0        0    22052 2023-06-29 20:04:50.940814 fabric_fim-1.5.3/fim/slivers/network_service.py
+-rw-r--r--   0        0        0     6795 2021-06-04 19:43:14.993329 fabric_fim-1.5.3/fim/slivers/path_info.py
+-rw-r--r--   0        0        0     3024 2022-02-18 19:27:15.594931 fabric_fim-1.5.3/fim/slivers/tags.py
+-rw-r--r--   0        0        0     2622 2023-02-02 01:41:56.416090 fabric_fim-1.5.3/fim/slivers/topology_diff.py
+-rw-r--r--   0        0        0     8706 2022-02-18 19:27:15.595505 fabric_fim-1.5.3/fim/user/README.md
+-rw-r--r--   0        0        0     1914 2023-02-02 01:41:56.417286 fabric_fim-1.5.3/fim/user/__init__.py
+-rw-r--r--   0        0        0    11730 2022-09-10 21:18:41.716394 fabric_fim-1.5.3/fim/user/component.py
+-rw-r--r--   0        0        0     5668 2022-09-10 21:18:41.716675 fabric_fim-1.5.3/fim/user/composite_node.py
+-rw-r--r--   0        0        0     7660 2023-02-02 01:41:56.418568 fabric_fim-1.5.3/fim/user/interface.py
+-rw-r--r--   0        0        0     8381 2022-09-10 21:18:41.717280 fabric_fim-1.5.3/fim/user/link.py
+-rw-r--r--   0        0        0     1219 2021-03-03 19:57:54.300001 fabric_fim-1.5.3/fim/user/measurement.py
+-rw-r--r--   0        0        0     9668 2023-04-05 18:48:29.319327 fabric_fim-1.5.3/fim/user/model_element.py
+-rw-r--r--   0        0        0    29219 2023-05-10 14:54:24.206616 fabric_fim-1.5.3/fim/user/network_service.py
+-rw-r--r--   0        0        0    22636 2023-02-14 21:58:39.970039 fabric_fim-1.5.3/fim/user/node.py
+-rw-r--r--   0        0        0    58158 2023-06-01 15:42:31.904936 fabric_fim-1.5.3/fim/user/topology.py
+-rw-r--r--   0        0        0        2 2023-06-29 20:04:50.942320 fabric_fim-1.5.3/fim/util/__init__.py
+-rw-r--r--   0        0        0    14680 2023-07-12 01:55:39.635415 fabric_fim-1.5.3/fim/util/fim_util.py
+-rw-r--r--   0        0        0      595 2021-03-13 20:40:37.643107 fabric_fim-1.5.3/fim/view_only_dict.py
+-rw-r--r--   0        0        0        0 2023-02-02 01:41:56.421372 fabric_fim-1.5.3/neo4j/data/.empty
+-rw-r--r--   0        0        0        0 2023-02-02 01:41:56.421489 fabric_fim-1.5.3/neo4j/imports/.empty
+-rw-r--r--   0        0        0      863 2023-06-29 20:04:50.944432 fabric_fim-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4632 2022-03-09 00:58:31.583145 fabric_fim-1.5.3/test/ad_topology_test.py
+-rw-r--r--   0        0        0     4834 2022-09-10 21:18:41.719406 fabric_fim-1.5.3/test/after.graphml
+-rw-r--r--   0        0        0    17550 2023-06-29 20:04:50.945459 fabric_fim-1.5.3/test/attribute_collector_test.py
+-rw-r--r--   0        0        0     4696 2022-09-10 21:18:41.719615 fabric_fim-1.5.3/test/before.graphml
+-rw-r--r--   0        0        0     2729 2022-09-10 21:18:41.719876 fabric_fim-1.5.3/test/catalog_test.py
+-rw-r--r--   0        0        0     4319 2022-02-18 19:27:15.602412 fabric_fim-1.5.3/test/delegation_label_test.py
+-rw-r--r--   0        0        0     1653 2023-02-02 01:41:56.423551 fabric_fim-1.5.3/test/maintenance_test.py
+-rw-r--r--   0        0        0    51613 2023-05-10 17:34:04.562843 fabric_fim-1.5.3/test/models/advertised_topo.graphml
+-rw-r--r--   0        0        0    49696 2023-05-10 17:34:04.565992 fabric_fim-1.5.3/test/models/graph-template.graphml
+-rw-r--r--   0        0        0    82994 2023-05-10 17:34:04.568753 fabric_fim-1.5.3/test/models/network-am-ad.graphml
+-rw-r--r--   0        0        0    57411 2023-05-10 17:34:04.571919 fabric_fim-1.5.3/test/models/site-2-am-1broker-ad.graphml
+-rw-r--r--   0        0        0    52887 2023-05-10 17:34:04.574274 fabric_fim-1.5.3/test/models/site-3-am-1broker-ad.graphml
+-rw-r--r--   0        0        0   131407 2023-05-10 17:34:04.575177 fabric_fim-1.5.3/test/models/site-am-2broker-ad.graphml
+-rw-r--r--   0        0        0    18708 2023-06-29 20:04:50.945949 fabric_fim-1.5.3/test/modify_test.py
+-rw-r--r--   0        0        0    13135 2021-05-23 19:50:30.753072 fabric_fim-1.5.3/test/networkxx_pg_disjoint_test.py
+-rw-r--r--   0        0        0    14091 2021-05-23 19:50:30.753595 fabric_fim-1.5.3/test/networkxx_pg_test.py
+-rw-r--r--   0        0        0     2572 2021-03-24 00:18:51.064667 fabric_fim-1.5.3/test/pluggable_test.py
+-rw-r--r--   0        0        0    42428 2023-06-29 20:04:50.947265 fabric_fim-1.5.3/test/slice_topology_test.py
+-rw-r--r--   0        0        0     1869 2022-04-27 22:22:19.322857 fabric_fim-1.5.3/test/sliver_json_test.py
+-rw-r--r--   0        0        0     6030 2023-06-29 20:04:50.948288 fabric_fim-1.5.3/test/sliver_test.py
+-rw-r--r--   0        0        0    97162 2023-02-02 01:41:56.427682 fabric_fim-1.5.3/test/substrate_topology_test.py
+-rw-r--r--   0        0        0      654 2022-02-18 19:27:15.604787 fabric_fim-1.5.3/test/test_load.py
+-rw-r--r--   0        0        0     2362 2022-02-18 19:27:15.605244 fabric_fim-1.5.3/test/tuple_test.py
+-rw-r--r--   0        0        0    15663 2023-06-15 15:19:01.186763 fabric_fim-1.5.3/test/zz_neo4j_pg_test.py
+-rw-r--r--   0        0        0    11890 1970-01-01 00:00:00.000000 fabric_fim-1.5.3/PKG-INFO
```

### Comparing `fabric_fim-1.5.2/.gitignore` & `fabric_fim-1.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/LICENSE` & `fabric_fim-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/README.md` & `fabric_fim-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/figs/fim-structure.png` & `fabric_fim-1.5.3/figs/fim-structure.png`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/README.md` & `fabric_fim-1.5.3/fim/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/authz/attribute_collector.py` & `fabric_fim-1.5.3/fim/authz/attribute_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/abc_property_graph.py` & `fabric_fim-1.5.3/fim/graph/abc_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/abc_property_graph_constants.py` & `fabric_fim-1.5.3/fim/graph/abc_property_graph_constants.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/data/graph_validation_rules.json` & `fabric_fim-1.5.3/fim/graph/data/graph_validation_rules.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/data/graph_validation_rules_neo4j_v4.json` & `fabric_fim-1.5.3/fim/graph/data/graph_validation_rules_neo4j_v4.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/data/label_types.json` & `fabric_fim-1.5.3/fim/graph/data/label_types.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/data/neo4j_indexes.json` & `fabric_fim-1.5.3/fim/graph/data/neo4j_indexes.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/graph_util.py` & `fabric_fim-1.5.3/fim/graph/graph_util.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/neo4j_property_graph.py` & `fabric_fim-1.5.3/fim/graph/neo4j_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/networkx_mixin.py` & `fabric_fim-1.5.3/fim/graph/networkx_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/networkx_property_graph.py` & `fabric_fim-1.5.3/fim/graph/networkx_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/networkx_property_graph_disjoint.py` & `fabric_fim-1.5.3/fim/graph/networkx_property_graph_disjoint.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/resources/README.md` & `fabric_fim-1.5.3/fim/graph/resources/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/resources/abc_adm.py` & `fabric_fim-1.5.3/fim/graph/resources/abc_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/resources/abc_arm.py` & `fabric_fim-1.5.3/fim/graph/resources/abc_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/resources/abc_bqm.py` & `fabric_fim-1.5.3/fim/graph/resources/abc_bqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/resources/abc_cbm.py` & `fabric_fim-1.5.3/fim/graph/resources/abc_cbm.py`

 * *Files 12% similar despite different names*

```diff
@@ -119,7 +119,31 @@
     def get_intersite_links(self) -> List[Tuple]:
         """
         Get a list of unique intersite links, and return a list of tuples
         (Source NodeID, Link NodeID, Sink NodeID, Source Site, Sink Site,
         Source CP NodeID, Sink CP NodeID).
         :return:
         """
+
+    @abstractmethod
+    def get_sites(self) -> List[str]:
+        """
+        Return a lexicographically sorted list of site names in CBM topology
+        """
+
+    @abstractmethod
+    def get_disconnected_sites(self) -> List[str]:
+        """
+        Return a lexicographically sorted list of site names that are disconnected in the CBM topology
+        """
+
+    @abstractmethod
+    def get_connected_sites(self) -> List[str]:
+        """
+        Return a lexicographically sorted list of site names that are connected in the CBM topology
+        """
+
+    @abstractmethod
+    def get_facility_ports(self) -> List[str]:
+        """
+        Return a lexicographically sorted list of names of facility ports in the CBM topology
+        """
```

### Comparing `fabric_fim-1.5.2/fim/graph/resources/neo4j_adm.py` & `fabric_fim-1.5.3/fim/graph/resources/neo4j_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/resources/neo4j_arm.py` & `fabric_fim-1.5.3/fim/graph/resources/neo4j_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/resources/neo4j_cbm.py` & `fabric_fim-1.5.3/fim/graph/resources/neo4j_cbm.py`

 * *Files 9% similar despite different names*

```diff
@@ -336,14 +336,58 @@
                 'm.Site as sink_site, cp1.NodeID as source_cp, cp2.NodeID as sink_cp'
         with self.driver.session() as session:
             val = session.run(query, graphId=self.graph_id).values()
         if val is None:
             return list()
         return val
 
+    def get_sites(self) -> List[str]:
+        query = 'match(na:GraphNode:NetworkNode {Type:"Switch", GraphID: $graphId}) return ' \
+                'collect(distinct na.Site) as allSites'
+        with self.driver.session() as session:
+            val = session.run(query, graphId=self.graph_id).single()
+        if val is None:
+            return list()
+        return sorted(val.value())
+
+    def get_disconnected_sites(self) -> List[str]:
+        query = 'match(na:GraphNode:NetworkNode {Type:"Switch", GraphID: $graphId}) with collect(na.Site) ' \
+                'as allSites match(n:GraphNode:NetworkNode {Type:"Switch", GraphID: $graphId}) ' \
+                '-[:has]- (ns1:GraphNode:NetworkService {Type:"MPLS", GraphID: $graphId}) -[:connects*1..4]- ' \
+                '(ns2:GraphNode:NetworkService {Type:"MPLS", GraphID: $graphId}) -[:has]- ' \
+                '(m:GraphNode:NetworkNode {Type:"Switch", GraphID: $graphId}) ' \
+                'with allSites, collect(distinct n.Site) as connectedSites ' \
+                'return [x in allSites where not x in connectedSites] as disconnectedSites'
+        with self.driver.session() as session:
+            val = session.run(query, graphId=self.graph_id).single()
+        if val is None:
+            return list()
+        return sorted(val.value())
+
+    def get_connected_sites(self) -> List[str]:
+        query = 'match(n:GraphNode:NetworkNode {Type:"Switch", GraphID: $graphId}) ' \
+                '-[:has]- (ns1:GraphNode:NetworkService {Type:"MPLS", GraphID: $graphId}) -[:connects*1..4]- ' \
+                '(ns2:GraphNode:NetworkService {Type:"MPLS", GraphID: $graphId}) -[:has]- ' \
+                '(m:GraphNode:NetworkNode {Type:"Switch", GraphID: $graphId}) ' \
+                'return collect(distinct n.Site) as connectedSites '
+        with self.driver.session() as session:
+            val = session.run(query, graphId=self.graph_id).single()
+        if val is None:
+            return list()
+        return sorted(val.value())
+
+    def get_facility_ports(self) -> List[str]:
+        query = 'match(n:GraphNode:NetworkNode {Type: "Facility", GraphID: $graphId}) return ' \
+                'collect(distinct n.Name) as allFPs'
+        with self.driver.session() as session:
+            val = session.run(query, graphId=self.graph_id).single()
+        if val is None:
+            return list()
+        return sorted(val.value())
+
 
 class Neo4jCBMFactory:
     """
     Help convert graphs between formats so long as they are rooted in Neo4jPropertyGraph
     """
     @staticmethod
     def create(graph: Neo4jPropertyGraph) -> Neo4jCBMGraph:
```

### Comparing `fabric_fim-1.5.2/fim/graph/resources/networkx_abqm.py` & `fabric_fim-1.5.3/fim/graph/resources/networkx_abqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/resources/networkx_adm.py` & `fabric_fim-1.5.3/fim/graph/resources/networkx_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/resources/networkx_arm.py` & `fabric_fim-1.5.3/fim/graph/resources/networkx_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/slices/abc_asm.py` & `fabric_fim-1.5.3/fim/graph/slices/abc_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/slices/neo4j_asm.py` & `fabric_fim-1.5.3/fim/graph/slices/neo4j_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/slices/networkx_asm.py` & `fabric_fim-1.5.3/fim/graph/slices/networkx_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/graph/typed_tuples.py` & `fabric_fim-1.5.3/fim/graph/typed_tuples.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/logging/fim_logger.py` & `fabric_fim-1.5.3/fim/logging/fim_logger.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/logging/log_collector.py` & `fabric_fim-1.5.3/fim/logging/log_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/pluggable.py` & `fabric_fim-1.5.3/fim/pluggable.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/attached_components.py` & `fabric_fim-1.5.3/fim/slivers/attached_components.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/base_sliver.py` & `fabric_fim-1.5.3/fim/slivers/base_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/capacities_labels.py` & `fabric_fim-1.5.3/fim/slivers/capacities_labels.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/component_catalog.py` & `fabric_fim-1.5.3/fim/slivers/component_catalog.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/data/component_catalog.json` & `fabric_fim-1.5.3/fim/slivers/data/component_catalog.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/data/instance_sizes.json` & `fabric_fim-1.5.3/fim/slivers/data/instance_sizes.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/delegations.py` & `fabric_fim-1.5.3/fim/slivers/delegations.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/gateway.py` & `fabric_fim-1.5.3/fim/slivers/gateway.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/identifiers.py` & `fabric_fim-1.5.3/fim/slivers/identifiers.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/instance_catalog.py` & `fabric_fim-1.5.3/fim/slivers/instance_catalog.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/interface_info.py` & `fabric_fim-1.5.3/fim/slivers/interface_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/json.py` & `fabric_fim-1.5.3/fim/slivers/json.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/json_data.py` & `fabric_fim-1.5.3/fim/slivers/json_data.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/maintenance_mode.py` & `fabric_fim-1.5.3/fim/slivers/maintenance_mode.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/network_attached_storage.py` & `fabric_fim-1.5.3/fim/slivers/network_attached_storage.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/network_link.py` & `fabric_fim-1.5.3/fim/slivers/network_link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/network_node.py` & `fabric_fim-1.5.3/fim/slivers/network_node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/network_service.py` & `fabric_fim-1.5.3/fim/slivers/network_service.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/path_info.py` & `fabric_fim-1.5.3/fim/slivers/path_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/tags.py` & `fabric_fim-1.5.3/fim/slivers/tags.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/slivers/topology_diff.py` & `fabric_fim-1.5.3/fim/slivers/topology_diff.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/user/README.md` & `fabric_fim-1.5.3/fim/user/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/user/__init__.py` & `fabric_fim-1.5.3/fim/user/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/user/component.py` & `fabric_fim-1.5.3/fim/user/component.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/user/composite_node.py` & `fabric_fim-1.5.3/fim/user/composite_node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/user/interface.py` & `fabric_fim-1.5.3/fim/user/interface.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/user/link.py` & `fabric_fim-1.5.3/fim/user/link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/user/measurement.py` & `fabric_fim-1.5.3/fim/user/measurement.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/user/model_element.py` & `fabric_fim-1.5.3/fim/user/model_element.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/user/network_service.py` & `fabric_fim-1.5.3/fim/user/network_service.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/user/node.py` & `fabric_fim-1.5.3/fim/user/node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/user/topology.py` & `fabric_fim-1.5.3/fim/user/topology.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/fim/util/fim_util.py` & `fabric_fim-1.5.3/fim/util/fim_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                                      import_dir=neo4j_config["import_dir"])
     if graph_id is None:
         neo4j_graph.delete_all_graphs()
     else:
         neo4j_graph.delete_graph(graph_id=graph_id)
 
 
-def merge_ads(*, neo4j_config, file_names, delete_arms, delete_adms):
+def merge_ads(*, neo4j_config, file_names, delete_arms, delete_adms, info=False):
     """
     Merge these advertisements together in the order provided
     :param neo4j_config:
     :param file_names: list of file names
     :return:
     """
     neo4j_graph_importer = Neo4jGraphImporter(url=neo4j_config["url"], user=neo4j_config["user"],
@@ -175,14 +175,19 @@
             logging.info(f'Deleting ARM {file_name}')
             arms[file_name].delete_graph()
         if delete_adms:
             logging.info(f'Deleting ADMs for {file_name}')
             for adm in site_adms.values():
                 adm.delete_graph()
     logging.info('Completed')
+    if info:
+        logging.info(f'List of sites in the model: {cbm.get_sites()}')
+        logging.info(f'List of connected sites in the model: {cbm.get_connected_sites()}')
+        logging.info(f'List of disconnected sites in the model: {cbm.get_disconnected_sites()}')
+        logging.info(f'List of facility ports in the model: {cbm.get_facility_ports()}')
 
 
 def save_graph(*, outfile, graph_id, neo4j_config):
     """
     Save indicated graph id into a file
     :param outfile:
     :param graph_id:
@@ -224,14 +229,16 @@
                         help="output GraphML file(s)")
     parser.add_argument("-g", "--graph", action="append",
                         help="identifier of the graph in the Neo4j database")
     parser.add_argument("-r", "--direct", action="store_true",
                         help="load file directly without validation or any manipulations")
     parser.add_argument("-d", "--debug", action="count",
                         help="turn on debugging")
+    parser.add_argument("-i", "--info", action="store_true",
+                        help="used with -m/--merge, provide information about merged CBM")
 
     args = parser.parse_args()
 
     if args.debug is None:
         logging.basicConfig(level=logging.INFO)
     elif args.debug >= 1:
         logging.basicConfig(level=logging.DEBUG)
@@ -275,15 +282,15 @@
     elif args.merge:
         if args.file is None or len(args.file) == 0:
             logging.error('Must specify at least one -f option', file=sys.stderr)
             sys.exit(-1)
         # merge specified files into a CBM
         try:
             merge_ads(neo4j_config=yaml_config["neo4j"], file_names=args.file,
-                      delete_arms=True, delete_adms=True)
+                      delete_arms=True, delete_adms=True, info=args.info)
         except Exception as e:
             logging.error(f"Unable to merge files {args.file} to Neo4j due to {e.args}", file=sys.stderr)
             traceback.print_exc(file=sys.stderr)
             sys.exit(-1)
     elif args.wipe:
         # wipe one graph or whole database
         delete_graphs(neo4j_config=yaml_config["neo4j"], graph_id=args.graph)
```

### Comparing `fabric_fim-1.5.2/fim/view_only_dict.py` & `fabric_fim-1.5.3/fim/view_only_dict.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/pyproject.toml` & `fabric_fim-1.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/ad_topology_test.py` & `fabric_fim-1.5.3/test/ad_topology_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/after.graphml` & `fabric_fim-1.5.3/test/after.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/attribute_collector_test.py` & `fabric_fim-1.5.3/test/attribute_collector_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/before.graphml` & `fabric_fim-1.5.3/test/before.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/catalog_test.py` & `fabric_fim-1.5.3/test/catalog_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/delegation_label_test.py` & `fabric_fim-1.5.3/test/delegation_label_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/maintenance_test.py` & `fabric_fim-1.5.3/test/maintenance_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/models/advertised_topo.graphml` & `fabric_fim-1.5.3/test/models/advertised_topo.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/models/graph-template.graphml` & `fabric_fim-1.5.3/test/models/graph-template.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/models/network-am-ad.graphml` & `fabric_fim-1.5.3/test/models/network-am-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/models/site-2-am-1broker-ad.graphml` & `fabric_fim-1.5.3/test/models/site-2-am-1broker-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/models/site-3-am-1broker-ad.graphml` & `fabric_fim-1.5.3/test/models/site-3-am-1broker-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/models/site-am-2broker-ad.graphml` & `fabric_fim-1.5.3/test/models/site-am-2broker-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/modify_test.py` & `fabric_fim-1.5.3/test/modify_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/networkxx_pg_disjoint_test.py` & `fabric_fim-1.5.3/test/networkxx_pg_disjoint_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/networkxx_pg_test.py` & `fabric_fim-1.5.3/test/networkxx_pg_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/pluggable_test.py` & `fabric_fim-1.5.3/test/pluggable_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/slice_topology_test.py` & `fabric_fim-1.5.3/test/slice_topology_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/sliver_json_test.py` & `fabric_fim-1.5.3/test/sliver_json_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/sliver_test.py` & `fabric_fim-1.5.3/test/sliver_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/substrate_topology_test.py` & `fabric_fim-1.5.3/test/substrate_topology_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/test_load.py` & `fabric_fim-1.5.3/test/test_load.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/tuple_test.py` & `fabric_fim-1.5.3/test/tuple_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/test/zz_neo4j_pg_test.py` & `fabric_fim-1.5.3/test/zz_neo4j_pg_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.2/PKG-INFO` & `fabric_fim-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric_fim
-Version: 1.5.2
+Version: 1.5.3
 Summary: FABRIC Information Model library and utilities
 Keywords: Neo4j
 Author-email: Ilya Baldin <ibaldin@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


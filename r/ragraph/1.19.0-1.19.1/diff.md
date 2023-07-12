# Comparing `tmp/ragraph-1.19.0.tar.gz` & `tmp/ragraph-1.19.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragraph-1.19.0.tar", max compression
+gzip compressed data, was "ragraph-1.19.1.tar", max compression
```

## Comparing `ragraph-1.19.0.tar` & `ragraph-1.19.1.tar`

### file list

```diff
@@ -1,151 +1,151 @@
--rw-r--r--   0        0        0    35400 2023-05-24 14:59:25.820630 ragraph-1.19.0/LICENSE.rst
--rw-r--r--   0        0        0     1781 2023-05-24 14:59:25.820630 ragraph-1.19.0/README.rst
--rw-r--r--   0        0        0     2325 2023-05-24 14:59:25.823630 ragraph-1.19.0/pyproject.toml
--rw-r--r--   0        0        0       72 2023-05-24 14:59:25.823630 ragraph-1.19.0/ragraph/__init__.py
--rw-r--r--   0        0        0      100 2023-05-24 14:59:25.823630 ragraph-1.19.0/ragraph/analysis/__init__.py
--rw-r--r--   0        0        0    19876 2023-05-24 14:59:25.823630 ragraph-1.19.0/ragraph/analysis/_classes.py
--rw-r--r--   0        0        0     7901 2023-05-24 14:59:25.823630 ragraph-1.19.0/ragraph/analysis/_utils.py
--rw-r--r--   0        0        0     1142 2023-05-24 14:59:25.823630 ragraph-1.19.0/ragraph/analysis/bus/__init__.py
--rw-r--r--   0        0        0     3743 2023-05-24 14:59:25.823630 ragraph-1.19.0/ragraph/analysis/bus/_gamma.py
--rw-r--r--   0        0        0     1613 2023-05-24 14:59:25.823630 ragraph-1.19.0/ragraph/analysis/cluster/__init__.py
--rw-r--r--   0        0        0    13777 2023-05-24 14:59:25.823630 ragraph-1.19.0/ragraph/analysis/cluster/_markov.py
--rw-r--r--   0        0        0     3438 2023-05-24 14:59:25.823630 ragraph-1.19.0/ragraph/analysis/cluster/_tarjan.py
--rw-r--r--   0        0        0      417 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/comparison/__init__.py
--rw-r--r--   0        0        0     2533 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/comparison/_delta.py
--rw-r--r--   0        0        0     6163 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/comparison/_sigma.py
--rw-r--r--   0        0        0     3518 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/comparison/utils.py
--rw-r--r--   0        0        0    19484 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/compatibility/__init__.py
--rw-r--r--   0        0        0     2729 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/compatibility/bdd.py
--rw-r--r--   0        0        0     1227 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/heuristics/__init__.py
--rw-r--r--   0        0        0     3368 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/heuristics/_johnson.py
--rw-r--r--   0        0        0     5157 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/heuristics/_markov_gamma.py
--rw-r--r--   0        0        0     1787 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/sequence/__init__.py
--rw-r--r--   0        0        0    10956 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/sequence/_axis.py
--rw-r--r--   0        0        0     5226 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/sequence/_genetic.py
--rw-r--r--   0        0        0     3010 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/sequence/_markov.py
--rw-r--r--   0        0        0      840 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/sequence/_name.py
--rw-r--r--   0        0        0     3750 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/sequence/_scc_tearing.py
--rw-r--r--   0        0        0     1713 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/sequence/_tarjan.py
--rw-r--r--   0        0        0     7133 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/sequence/metrics.py
--rw-r--r--   0        0        0     5256 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/sequence/utils.py
--rw-r--r--   0        0        0     1336 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/similarity/__init__.py
--rw-r--r--   0        0        0     3036 2023-05-24 14:59:25.824630 ragraph-1.19.0/ragraph/analysis/similarity/_jaccard.py
--rw-r--r--   0        0        0     9582 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/analysis/similarity/_similarity.py
--rw-r--r--   0        0        0     1824 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/analysis/similarity/utils.py
--rw-r--r--   0        0        0     9963 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/colors/__init__.py
--rw-r--r--   0        0        0     5320 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/colors/cubehelix.py
--rw-r--r--   0        0        0      774 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/colors/utils.py
--rw-r--r--   0        0        0     1663 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/__init__.py
--rw-r--r--   0        0        0      673 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/aircraft_engine/__init__.py
--rw-r--r--   0        0        0    28938 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv
--rw-r--r--   0        0        0      977 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv
--rw-r--r--   0        0        0     1035 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/architecture_integral/__init__.py
--rw-r--r--   0        0        0     1364 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/architecture_integral/architecture_integral_edges.csv
--rw-r--r--   0        0        0      352 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/architecture_integral/architecture_integral_nodes.csv
--rw-r--r--   0        0        0     1048 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/architecture_mix/__init__.py
--rw-r--r--   0        0        0     2264 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/architecture_mix/architecture_mix_edges.csv
--rw-r--r--   0        0        0      352 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/architecture_mix/architecture_mix_nodes.csv
--rw-r--r--   0        0        0     1043 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/architecture_modular/__init__.py
--rw-r--r--   0        0        0     2722 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/architecture_modular/architecture_modular_edges.csv
--rw-r--r--   0        0        0      351 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/architecture_modular/architecture_modular_nodes.csv
--rw-r--r--   0        0        0      813 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/climate_control/__init__.py
--rw-r--r--   0        0        0     5778 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/climate_control/climate_control_edges.csv
--rw-r--r--   0        0        0      632 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/climate_control/climate_control_nodes.csv
--rw-r--r--   0        0        0      374 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/climate_control_mg/__init__.py
--rw-r--r--   0        0        0     5778 2023-05-24 14:59:25.825630 ragraph-1.19.0/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv
--rw-r--r--   0        0        0     1441 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv
--rw-r--r--   0        0        0      460 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/compatibility/__init__.py
--rw-r--r--   0        0        0      564 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/compatibility/compatibility_edges.csv
--rw-r--r--   0        0        0       83 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/compatibility/compatibility_nodes.csv
--rw-r--r--   0        0        0      431 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/design/__init__.py
--rw-r--r--   0        0        0      872 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/design/design_edges.csv
--rw-r--r--   0        0        0      384 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/design/design_nodes.csv
--rw-r--r--   0        0        0      998 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/elevator175/__init__.py
--rw-r--r--   0        0        0   103961 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/elevator175/elevator175_edges.csv
--rw-r--r--   0        0        0     7255 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/elevator175/elevator175_nodes.csv
--rw-r--r--   0        0        0      995 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/elevator45/__init__.py
--rw-r--r--   0        0        0    29033 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/elevator45/elevator45_edges.csv
--rw-r--r--   0        0        0     1887 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/elevator45/elevator45_nodes.csv
--rw-r--r--   0        0        0     1148 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/esl/__init__.py
--rw-r--r--   0        0        0       75 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/esl/pump/__init__.py
--rw-r--r--   0        0        0     3523 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/esl/pump/pump.esl
--rw-r--r--   0        0        0     1868 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/ford_hood/__init__.py
--rw-r--r--   0        0        0    30483 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/ford_hood/ford_hood_edges.csv
--rw-r--r--   0        0        0     3339 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/ford_hood/ford_hood_nodes.csv
--rw-r--r--   0        0        0     1461 2023-05-24 14:59:25.826630 ragraph-1.19.0/ragraph/datasets/kodak3d/__init__.py
--rw-r--r--   0        0        0     6660 2023-05-24 14:59:25.827630 ragraph-1.19.0/ragraph/datasets/kodak3d/kodak3d_edges.csv
--rw-r--r--   0        0        0     1134 2023-05-24 14:59:25.827630 ragraph-1.19.0/ragraph/datasets/kodak3d/kodak3d_nodes.csv
--rw-r--r--   0        0        0      216 2023-05-24 14:59:25.827630 ragraph-1.19.0/ragraph/datasets/ledsip/__init__.py
--rw-r--r--   0        0        0   210027 2023-05-24 14:59:25.827630 ragraph-1.19.0/ragraph/datasets/ledsip/ledsip_edges.csv
--rw-r--r--   0        0        0    50840 2023-05-24 14:59:25.827630 ragraph-1.19.0/ragraph/datasets/ledsip/ledsip_nodes.csv
--rw-r--r--   0        0        0       74 2023-05-24 14:59:25.827630 ragraph-1.19.0/ragraph/datasets/localbus/__init__.py
--rw-r--r--   0        0        0      723 2023-05-24 14:59:25.827630 ragraph-1.19.0/ragraph/datasets/localbus/localbus_edges.csv
--rw-r--r--   0        0        0       27 2023-05-24 14:59:25.827630 ragraph-1.19.0/ragraph/datasets/localbus/localbus_nodes.csv
--rw-r--r--   0        0        0        0 2023-05-24 14:59:25.827630 ragraph-1.19.0/ragraph/datasets/mww_lock_aspect/__init__.py
--rw-r--r--   0        0        0    93289 2023-05-24 14:59:25.828630 ragraph-1.19.0/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_edges.csv
--rw-r--r--   0        0        0     9178 2023-05-24 14:59:25.828630 ragraph-1.19.0/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_nodes.csv
--rw-r--r--   0        0        0       83 2023-05-24 14:59:25.828630 ragraph-1.19.0/ragraph/datasets/mww_lock_eefde/__init__.py
--rw-r--r--   0        0        0   147721 2023-05-24 14:59:25.828630 ragraph-1.19.0/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_edges.csv
--rw-r--r--   0        0        0     1388 2023-05-24 14:59:25.828630 ragraph-1.19.0/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_nodes.csv
--rw-r--r--   0        0        0       83 2023-05-24 14:59:25.828630 ragraph-1.19.0/ragraph/datasets/mww_lock_hansweert/__init__.py
--rw-r--r--   0        0        0    54617 2023-05-24 14:59:25.828630 ragraph-1.19.0/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_edges.csv
--rw-r--r--   0        0        0     1144 2023-05-24 14:59:25.828630 ragraph-1.19.0/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_nodes.csv
--rw-r--r--   0        0        0       83 2023-05-24 14:59:25.828630 ragraph-1.19.0/ragraph/datasets/mww_lock_sambeek/__init__.py
--rw-r--r--   0        0        0    53667 2023-05-24 14:59:25.829630 ragraph-1.19.0/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_edges.csv
--rw-r--r--   0        0        0     1123 2023-05-24 14:59:25.829630 ragraph-1.19.0/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_nodes.csv
--rw-r--r--   0        0        0       83 2023-05-24 14:59:25.829630 ragraph-1.19.0/ragraph/datasets/mww_lock_sluis15/__init__.py
--rw-r--r--   0        0        0    54995 2023-05-24 14:59:25.829630 ragraph-1.19.0/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_edges.csv
--rw-r--r--   0        0        0     1054 2023-05-24 14:59:25.829630 ragraph-1.19.0/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_nodes.csv
--rw-r--r--   0        0        0        0 2023-05-24 14:59:25.829630 ragraph-1.19.0/ragraph/datasets/mww_lock_volkerak/__init__.py
--rw-r--r--   0        0        0    18120 2023-05-24 14:59:25.829630 ragraph-1.19.0/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_edges.csv
--rw-r--r--   0        0        0     1216 2023-05-24 14:59:25.829630 ragraph-1.19.0/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_nodes.csv
--rw-r--r--   0        0        0       76 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/overlap/__init__.py
--rw-r--r--   0        0        0      149 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/overlap/overlap_edges.csv
--rw-r--r--   0        0        0       15 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/overlap/overlap_nodes.csv
--rw-r--r--   0        0        0     3167 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/pathfinder/__init__.py
--rw-r--r--   0        0        0    17741 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/pathfinder/pathfinder_edges.csv
--rw-r--r--   0        0        0     1084 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/pathfinder/pathfinder_nodes.csv
--rw-r--r--   0        0        0      307 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/shaja8/__init__.py
--rw-r--r--   0        0        0      243 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/shaja8/shaja8_edges.csv
--rw-r--r--   0        0        0       21 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/shaja8/shaja8_nodes.csv
--rw-r--r--   0        0        0      224 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/similarity/__init__.py
--rw-r--r--   0        0        0      872 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/similarity/similarity_edges.csv
--rw-r--r--   0        0        0      360 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/similarity/similarity_nodes.csv
--rw-r--r--   0        0        0      253 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/tarjans8/__init__.py
--rw-r--r--   0        0        0      199 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/tarjans8/tarjans8_edges.csv
--rw-r--r--   0        0        0       21 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/tarjans8/tarjans8_nodes.csv
--rw-r--r--   0        0        0     1493 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/ucav/__init__.py
--rw-r--r--   0        0        0     5183 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/ucav/ucav_edges.csv
--rw-r--r--   0        0        0     1141 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/datasets/ucav/ucav_nodes.csv
--rw-r--r--   0        0        0     4372 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/edge.py
--rw-r--r--   0        0        0    23032 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/generic.py
--rw-r--r--   0        0        0    39432 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/graph.py
--rw-r--r--   0        0        0       80 2023-05-24 14:59:25.830630 ragraph-1.19.0/ragraph/io/__init__.py
--rw-r--r--   0        0        0    11755 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/io/archimate/__init__.py
--rw-r--r--   0        0        0    48350 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/io/archimate/archimate3_Model.xsd
--rw-r--r--   0        0        0      461 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/io/archimate/bare.xml
--rw-r--r--   0        0        0     8836 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/io/archimate/xml.xsd
--rw-r--r--   0        0        0     6745 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/io/canopy.py
--rw-r--r--   0        0        0    13730 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/io/csv.py
--rw-r--r--   0        0        0      229 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/io/esl.py
--rw-r--r--   0        0        0     5925 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/io/grip.py
--rw-r--r--   0        0        0     4146 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/io/json.py
--rw-r--r--   0        0        0     5081 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/io/matrix.py
--rw-r--r--   0        0        0     1819 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/io/xml/XMI-Canonical.xsd
--rw-r--r--   0        0        0     9246 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/io/xml/__init__.py
--rw-r--r--   0        0        0      358 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/io/xml/bare.xml
--rw-r--r--   0        0        0     4332 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/io/xml/ragraph.xsd
--rw-r--r--   0        0        0     1270 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/io/yaml.py
--rw-r--r--   0        0        0     7862 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/node.py
--rw-r--r--   0        0        0     4325 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/plot/__init__.py
--rw-r--r--   0        0        0      507 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/plot/components/__init__.py
--rw-r--r--   0        0        0     1178 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/plot/components/blank.py
--rw-r--r--   0        0        0     3822 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/plot/components/labels.py
--rw-r--r--   0        0        0     9115 2023-05-24 14:59:25.831630 ragraph-1.19.0/ragraph/plot/components/legend.py
--rw-r--r--   0        0        0    20779 2023-05-24 14:59:25.832630 ragraph-1.19.0/ragraph/plot/components/piemap.py
--rw-r--r--   0        0        0     6765 2023-05-24 14:59:25.832630 ragraph-1.19.0/ragraph/plot/components/tree.py
--rw-r--r--   0        0        0    28046 2023-05-24 14:59:25.832630 ragraph-1.19.0/ragraph/plot/generic.py
--rw-r--r--   0        0        0     9811 2023-05-24 14:59:25.832630 ragraph-1.19.0/ragraph/plot/svg.py
--rw-r--r--   0        0        0     9274 2023-05-24 14:59:25.832630 ragraph-1.19.0/ragraph/plot/utils.py
--rw-r--r--   0        0        0     3088 2023-05-24 14:59:25.832630 ragraph-1.19.0/ragraph/utils.py
--rw-r--r--   0        0        0     2884 1970-01-01 00:00:00.000000 ragraph-1.19.0/PKG-INFO
+-rw-r--r--   0        0        0    34753 2023-07-12 05:57:28.865613 ragraph-1.19.1/LICENSE-GPL
+-rw-r--r--   0        0        0     2144 2023-07-12 05:57:28.865613 ragraph-1.19.1/README.md
+-rw-r--r--   0        0        0     1970 2023-07-12 05:57:28.869613 ragraph-1.19.1/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-07-12 05:57:28.869613 ragraph-1.19.1/ragraph/__init__.py
+-rw-r--r--   0        0        0      138 2023-07-12 05:57:28.869613 ragraph-1.19.1/ragraph/analysis/__init__.py
+-rw-r--r--   0        0        0    19876 2023-07-12 05:57:28.870613 ragraph-1.19.1/ragraph/analysis/_classes.py
+-rw-r--r--   0        0        0     7950 2023-07-12 05:57:28.870613 ragraph-1.19.1/ragraph/analysis/_utils.py
+-rw-r--r--   0        0        0     1008 2023-07-12 05:57:28.870613 ragraph-1.19.1/ragraph/analysis/bus/__init__.py
+-rw-r--r--   0        0        0     4020 2023-07-12 05:57:28.870613 ragraph-1.19.1/ragraph/analysis/bus/_gamma.py
+-rw-r--r--   0        0        0     1376 2023-07-12 05:57:28.870613 ragraph-1.19.1/ragraph/analysis/cluster/__init__.py
+-rw-r--r--   0        0        0    13980 2023-07-12 05:57:28.870613 ragraph-1.19.1/ragraph/analysis/cluster/_markov.py
+-rw-r--r--   0        0        0     3470 2023-07-12 05:57:28.870613 ragraph-1.19.1/ragraph/analysis/cluster/_tarjan.py
+-rw-r--r--   0        0        0     1201 2023-07-12 05:57:28.870613 ragraph-1.19.1/ragraph/analysis/comparison/__init__.py
+-rw-r--r--   0        0        0     2540 2023-07-12 05:57:28.870613 ragraph-1.19.1/ragraph/analysis/comparison/_delta.py
+-rw-r--r--   0        0        0     6291 2023-07-12 05:57:28.870613 ragraph-1.19.1/ragraph/analysis/comparison/_sigma.py
+-rw-r--r--   0        0        0     3556 2023-07-12 05:57:28.870613 ragraph-1.19.1/ragraph/analysis/comparison/utils.py
+-rw-r--r--   0        0        0    20554 2023-07-12 05:57:28.870613 ragraph-1.19.1/ragraph/analysis/compatibility/__init__.py
+-rw-r--r--   0        0        0     2789 2023-07-12 05:57:28.870613 ragraph-1.19.1/ragraph/analysis/compatibility/bdd.py
+-rw-r--r--   0        0        0      649 2023-07-12 05:57:28.871613 ragraph-1.19.1/ragraph/analysis/heuristics/__init__.py
+-rw-r--r--   0        0        0     3351 2023-07-12 05:57:28.871613 ragraph-1.19.1/ragraph/analysis/heuristics/_johnson.py
+-rw-r--r--   0        0        0     5079 2023-07-12 05:57:28.871613 ragraph-1.19.1/ragraph/analysis/heuristics/_markov_gamma.py
+-rw-r--r--   0        0        0     2166 2023-07-12 05:57:28.871613 ragraph-1.19.1/ragraph/analysis/sequence/__init__.py
+-rw-r--r--   0        0        0    10933 2023-07-12 05:57:28.871613 ragraph-1.19.1/ragraph/analysis/sequence/_axis.py
+-rw-r--r--   0        0        0     5251 2023-07-12 05:57:28.871613 ragraph-1.19.1/ragraph/analysis/sequence/_genetic.py
+-rw-r--r--   0        0        0     3025 2023-07-12 05:57:28.871613 ragraph-1.19.1/ragraph/analysis/sequence/_markov.py
+-rw-r--r--   0        0        0      832 2023-07-12 05:57:28.871613 ragraph-1.19.1/ragraph/analysis/sequence/_name.py
+-rw-r--r--   0        0        0     3775 2023-07-12 05:57:28.871613 ragraph-1.19.1/ragraph/analysis/sequence/_scc_tearing.py
+-rw-r--r--   0        0        0     1727 2023-07-12 05:57:28.871613 ragraph-1.19.1/ragraph/analysis/sequence/_tarjan.py
+-rw-r--r--   0        0        0     7130 2023-07-12 05:57:28.871613 ragraph-1.19.1/ragraph/analysis/sequence/metrics.py
+-rw-r--r--   0        0        0     5245 2023-07-12 05:57:28.871613 ragraph-1.19.1/ragraph/analysis/sequence/utils.py
+-rw-r--r--   0        0        0     1460 2023-07-12 05:57:28.871613 ragraph-1.19.1/ragraph/analysis/similarity/__init__.py
+-rw-r--r--   0        0        0     3103 2023-07-12 05:57:28.871613 ragraph-1.19.1/ragraph/analysis/similarity/_jaccard.py
+-rw-r--r--   0        0        0     9922 2023-07-12 05:57:28.872613 ragraph-1.19.1/ragraph/analysis/similarity/_similarity.py
+-rw-r--r--   0        0        0     1826 2023-07-12 05:57:28.872613 ragraph-1.19.1/ragraph/analysis/similarity/utils.py
+-rw-r--r--   0        0        0    10265 2023-07-12 05:57:28.872613 ragraph-1.19.1/ragraph/colors/__init__.py
+-rw-r--r--   0        0        0     5447 2023-07-12 05:57:28.872613 ragraph-1.19.1/ragraph/colors/cubehelix.py
+-rw-r--r--   0        0        0      769 2023-07-12 05:57:28.872613 ragraph-1.19.1/ragraph/colors/utils.py
+-rw-r--r--   0        0        0     1589 2023-07-12 05:57:28.872613 ragraph-1.19.1/ragraph/datasets/__init__.py
+-rw-r--r--   0        0        0      679 2023-07-12 05:57:28.872613 ragraph-1.19.1/ragraph/datasets/aircraft_engine/__init__.py
+-rw-r--r--   0        0        0    28938 2023-07-12 05:57:28.872613 ragraph-1.19.1/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv
+-rw-r--r--   0        0        0      977 2023-07-12 05:57:28.872613 ragraph-1.19.1/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv
+-rw-r--r--   0        0        0     1073 2023-07-12 05:57:28.872613 ragraph-1.19.1/ragraph/datasets/architecture_integral/__init__.py
+-rw-r--r--   0        0        0     1364 2023-07-12 05:57:28.872613 ragraph-1.19.1/ragraph/datasets/architecture_integral/architecture_integral_edges.csv
+-rw-r--r--   0        0        0      352 2023-07-12 05:57:28.872613 ragraph-1.19.1/ragraph/datasets/architecture_integral/architecture_integral_nodes.csv
+-rw-r--r--   0        0        0     1083 2023-07-12 05:57:28.872613 ragraph-1.19.1/ragraph/datasets/architecture_mix/__init__.py
+-rw-r--r--   0        0        0     2264 2023-07-12 05:57:28.872613 ragraph-1.19.1/ragraph/datasets/architecture_mix/architecture_mix_edges.csv
+-rw-r--r--   0        0        0      352 2023-07-12 05:57:28.872613 ragraph-1.19.1/ragraph/datasets/architecture_mix/architecture_mix_nodes.csv
+-rw-r--r--   0        0        0     1079 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/architecture_modular/__init__.py
+-rw-r--r--   0        0        0     2722 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/architecture_modular/architecture_modular_edges.csv
+-rw-r--r--   0        0        0      351 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/architecture_modular/architecture_modular_nodes.csv
+-rw-r--r--   0        0        0      822 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/climate_control/__init__.py
+-rw-r--r--   0        0        0     5778 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/climate_control/climate_control_edges.csv
+-rw-r--r--   0        0        0      632 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/climate_control/climate_control_nodes.csv
+-rw-r--r--   0        0        0      423 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/climate_control_mg/__init__.py
+-rw-r--r--   0        0        0     5778 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv
+-rw-r--r--   0        0        0     1441 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv
+-rw-r--r--   0        0        0      443 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/compatibility/__init__.py
+-rw-r--r--   0        0        0      564 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/compatibility/compatibility_edges.csv
+-rw-r--r--   0        0        0       83 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/compatibility/compatibility_nodes.csv
+-rw-r--r--   0        0        0      469 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/design/__init__.py
+-rw-r--r--   0        0        0      872 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/design/design_edges.csv
+-rw-r--r--   0        0        0      384 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/design/design_nodes.csv
+-rw-r--r--   0        0        0     1008 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/elevator175/__init__.py
+-rw-r--r--   0        0        0   103961 2023-07-12 05:57:28.873613 ragraph-1.19.1/ragraph/datasets/elevator175/elevator175_edges.csv
+-rw-r--r--   0        0        0     7255 2023-07-12 05:57:28.874613 ragraph-1.19.1/ragraph/datasets/elevator175/elevator175_nodes.csv
+-rw-r--r--   0        0        0     1007 2023-07-12 05:57:28.874613 ragraph-1.19.1/ragraph/datasets/elevator45/__init__.py
+-rw-r--r--   0        0        0    29033 2023-07-12 05:57:28.874613 ragraph-1.19.1/ragraph/datasets/elevator45/elevator45_edges.csv
+-rw-r--r--   0        0        0     1887 2023-07-12 05:57:28.874613 ragraph-1.19.1/ragraph/datasets/elevator45/elevator45_nodes.csv
+-rw-r--r--   0        0        0     1197 2023-07-12 05:57:28.874613 ragraph-1.19.1/ragraph/datasets/esl/__init__.py
+-rw-r--r--   0        0        0       75 2023-07-12 05:57:28.874613 ragraph-1.19.1/ragraph/datasets/esl/pump/__init__.py
+-rw-r--r--   0        0        0     3523 2023-07-12 05:57:28.874613 ragraph-1.19.1/ragraph/datasets/esl/pump/pump.esl
+-rw-r--r--   0        0        0     1918 2023-07-12 05:57:28.874613 ragraph-1.19.1/ragraph/datasets/ford_hood/__init__.py
+-rw-r--r--   0        0        0    30483 2023-07-12 05:57:28.874613 ragraph-1.19.1/ragraph/datasets/ford_hood/ford_hood_edges.csv
+-rw-r--r--   0        0        0     3339 2023-07-12 05:57:28.874613 ragraph-1.19.1/ragraph/datasets/ford_hood/ford_hood_nodes.csv
+-rw-r--r--   0        0        0     1477 2023-07-12 05:57:28.874613 ragraph-1.19.1/ragraph/datasets/kodak3d/__init__.py
+-rw-r--r--   0        0        0     6660 2023-07-12 05:57:28.874613 ragraph-1.19.1/ragraph/datasets/kodak3d/kodak3d_edges.csv
+-rw-r--r--   0        0        0     1134 2023-07-12 05:57:28.874613 ragraph-1.19.1/ragraph/datasets/kodak3d/kodak3d_nodes.csv
+-rw-r--r--   0        0        0      202 2023-07-12 05:57:28.874613 ragraph-1.19.1/ragraph/datasets/ledsip/__init__.py
+-rw-r--r--   0        0        0   210027 2023-07-12 05:57:28.875613 ragraph-1.19.1/ragraph/datasets/ledsip/ledsip_edges.csv
+-rw-r--r--   0        0        0    50840 2023-07-12 05:57:28.875613 ragraph-1.19.1/ragraph/datasets/ledsip/ledsip_nodes.csv
+-rw-r--r--   0        0        0       75 2023-07-12 05:57:28.875613 ragraph-1.19.1/ragraph/datasets/localbus/__init__.py
+-rw-r--r--   0        0        0      723 2023-07-12 05:57:28.875613 ragraph-1.19.1/ragraph/datasets/localbus/localbus_edges.csv
+-rw-r--r--   0        0        0       27 2023-07-12 05:57:28.875613 ragraph-1.19.1/ragraph/datasets/localbus/localbus_nodes.csv
+-rw-r--r--   0        0        0       59 2023-07-12 05:57:28.875613 ragraph-1.19.1/ragraph/datasets/mww_lock_aspect/__init__.py
+-rw-r--r--   0        0        0    93289 2023-07-12 05:57:28.875613 ragraph-1.19.1/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_edges.csv
+-rw-r--r--   0        0        0     9178 2023-07-12 05:57:28.875613 ragraph-1.19.1/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_nodes.csv
+-rw-r--r--   0        0        0      136 2023-07-12 05:57:28.876613 ragraph-1.19.1/ragraph/datasets/mww_lock_eefde/__init__.py
+-rw-r--r--   0        0        0   147721 2023-07-12 05:57:28.876613 ragraph-1.19.1/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_edges.csv
+-rw-r--r--   0        0        0     1388 2023-07-12 05:57:28.876613 ragraph-1.19.1/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_nodes.csv
+-rw-r--r--   0        0        0      140 2023-07-12 05:57:28.876613 ragraph-1.19.1/ragraph/datasets/mww_lock_hansweert/__init__.py
+-rw-r--r--   0        0        0    54617 2023-07-12 05:57:28.876613 ragraph-1.19.1/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_edges.csv
+-rw-r--r--   0        0        0     1144 2023-07-12 05:57:28.876613 ragraph-1.19.1/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_nodes.csv
+-rw-r--r--   0        0        0      138 2023-07-12 05:57:28.876613 ragraph-1.19.1/ragraph/datasets/mww_lock_sambeek/__init__.py
+-rw-r--r--   0        0        0    53667 2023-07-12 05:57:28.877613 ragraph-1.19.1/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_edges.csv
+-rw-r--r--   0        0        0     1123 2023-07-12 05:57:28.877613 ragraph-1.19.1/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_nodes.csv
+-rw-r--r--   0        0        0      139 2023-07-12 05:57:28.877613 ragraph-1.19.1/ragraph/datasets/mww_lock_sluis15/__init__.py
+-rw-r--r--   0        0        0    54995 2023-07-12 05:57:28.877613 ragraph-1.19.1/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_edges.csv
+-rw-r--r--   0        0        0     1054 2023-07-12 05:57:28.877613 ragraph-1.19.1/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_nodes.csv
+-rw-r--r--   0        0        0       55 2023-07-12 05:57:28.877613 ragraph-1.19.1/ragraph/datasets/mww_lock_volkerak/__init__.py
+-rw-r--r--   0        0        0    18120 2023-07-12 05:57:28.877613 ragraph-1.19.1/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_edges.csv
+-rw-r--r--   0        0        0     1216 2023-07-12 05:57:28.877613 ragraph-1.19.1/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_nodes.csv
+-rw-r--r--   0        0        0       76 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/overlap/__init__.py
+-rw-r--r--   0        0        0      149 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/overlap/overlap_edges.csv
+-rw-r--r--   0        0        0       15 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/overlap/overlap_nodes.csv
+-rw-r--r--   0        0        0     2149 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/pathfinder/__init__.py
+-rw-r--r--   0        0        0    17741 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/pathfinder/pathfinder_edges.csv
+-rw-r--r--   0        0        0     1084 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/pathfinder/pathfinder_nodes.csv
+-rw-r--r--   0        0        0      353 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/shaja8/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/shaja8/shaja8_edges.csv
+-rw-r--r--   0        0        0       21 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/shaja8/shaja8_nodes.csv
+-rw-r--r--   0        0        0      255 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/similarity/__init__.py
+-rw-r--r--   0        0        0      872 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/similarity/similarity_edges.csv
+-rw-r--r--   0        0        0      360 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/similarity/similarity_nodes.csv
+-rw-r--r--   0        0        0      289 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/tarjans8/__init__.py
+-rw-r--r--   0        0        0      199 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/tarjans8/tarjans8_edges.csv
+-rw-r--r--   0        0        0       21 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/tarjans8/tarjans8_nodes.csv
+-rw-r--r--   0        0        0     1493 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/ucav/__init__.py
+-rw-r--r--   0        0        0     5183 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/ucav/ucav_edges.csv
+-rw-r--r--   0        0        0     1141 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/datasets/ucav/ucav_nodes.csv
+-rw-r--r--   0        0        0     4410 2023-07-12 05:57:28.878613 ragraph-1.19.1/ragraph/edge.py
+-rw-r--r--   0        0        0    23116 2023-07-12 05:57:28.879613 ragraph-1.19.1/ragraph/generic.py
+-rw-r--r--   0        0        0    39491 2023-07-12 05:57:28.879613 ragraph-1.19.1/ragraph/graph.py
+-rw-r--r--   0        0        0       76 2023-07-12 05:57:28.879613 ragraph-1.19.1/ragraph/io/__init__.py
+-rw-r--r--   0        0        0    11788 2023-07-12 05:57:28.879613 ragraph-1.19.1/ragraph/io/archimate/__init__.py
+-rw-r--r--   0        0        0    48350 2023-07-12 05:57:28.879613 ragraph-1.19.1/ragraph/io/archimate/archimate3_Model.xsd
+-rw-r--r--   0        0        0      461 2023-07-12 05:57:28.879613 ragraph-1.19.1/ragraph/io/archimate/bare.xml
+-rw-r--r--   0        0        0     8836 2023-07-12 05:57:28.879613 ragraph-1.19.1/ragraph/io/archimate/xml.xsd
+-rw-r--r--   0        0        0     6747 2023-07-12 05:57:28.879613 ragraph-1.19.1/ragraph/io/canopy.py
+-rw-r--r--   0        0        0    13762 2023-07-12 05:57:28.879613 ragraph-1.19.1/ragraph/io/csv.py
+-rw-r--r--   0        0        0      527 2023-07-12 05:57:28.879613 ragraph-1.19.1/ragraph/io/esl.py
+-rw-r--r--   0        0        0     5907 2023-07-12 05:57:28.880613 ragraph-1.19.1/ragraph/io/grip.py
+-rw-r--r--   0        0        0     4136 2023-07-12 05:57:28.880613 ragraph-1.19.1/ragraph/io/json.py
+-rw-r--r--   0        0        0     5150 2023-07-12 05:57:28.880613 ragraph-1.19.1/ragraph/io/matrix.py
+-rw-r--r--   0        0        0     1819 2023-07-12 05:57:28.880613 ragraph-1.19.1/ragraph/io/xml/XMI-Canonical.xsd
+-rw-r--r--   0        0        0     9259 2023-07-12 05:57:28.880613 ragraph-1.19.1/ragraph/io/xml/__init__.py
+-rw-r--r--   0        0        0      358 2023-07-12 05:57:28.880613 ragraph-1.19.1/ragraph/io/xml/bare.xml
+-rw-r--r--   0        0        0     4332 2023-07-12 05:57:28.880613 ragraph-1.19.1/ragraph/io/xml/ragraph.xsd
+-rw-r--r--   0        0        0     1269 2023-07-12 05:57:28.880613 ragraph-1.19.1/ragraph/io/yaml.py
+-rw-r--r--   0        0        0     7924 2023-07-12 05:57:28.880613 ragraph-1.19.1/ragraph/node.py
+-rw-r--r--   0        0        0     4327 2023-07-12 05:57:28.880613 ragraph-1.19.1/ragraph/plot/__init__.py
+-rw-r--r--   0        0        0      526 2023-07-12 05:57:28.880613 ragraph-1.19.1/ragraph/plot/components/__init__.py
+-rw-r--r--   0        0        0     1219 2023-07-12 05:57:28.880613 ragraph-1.19.1/ragraph/plot/components/blank.py
+-rw-r--r--   0        0        0     3818 2023-07-12 05:57:28.880613 ragraph-1.19.1/ragraph/plot/components/labels.py
+-rw-r--r--   0        0        0     9106 2023-07-12 05:57:28.880613 ragraph-1.19.1/ragraph/plot/components/legend.py
+-rw-r--r--   0        0        0    20583 2023-07-12 05:57:28.880613 ragraph-1.19.1/ragraph/plot/components/piemap.py
+-rw-r--r--   0        0        0     6794 2023-07-12 05:57:28.881613 ragraph-1.19.1/ragraph/plot/components/tree.py
+-rw-r--r--   0        0        0    28974 2023-07-12 05:57:28.881613 ragraph-1.19.1/ragraph/plot/generic.py
+-rw-r--r--   0        0        0    10320 2023-07-12 05:57:28.881613 ragraph-1.19.1/ragraph/plot/svg.py
+-rw-r--r--   0        0        0     9310 2023-07-12 05:57:28.881613 ragraph-1.19.1/ragraph/plot/utils.py
+-rw-r--r--   0        0        0     3169 2023-07-12 05:57:28.881613 ragraph-1.19.1/ragraph/utils.py
+-rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 ragraph-1.19.1/PKG-INFO
```

### Comparing `ragraph-1.19.0/LICENSE.rst` & `ragraph-1.19.1/LICENSE-GPL`

 * *Files 6% similar despite different names*

```diff
@@ -1,168 +1,166 @@
-GNU GENERAL PUBLIC LICENSE
-~~~~~~~~~~~~~~~~~~~~~~~~~~
+# GNU GENERAL PUBLIC LICENSE
 
 Version 3, 29 June 2007
 
-Copyright (C) 2007 Free Software Foundation, Inc. https://fsf.org/
+Copyright (C) 2007 Free Software Foundation, Inc.
+<https://fsf.org/>
 
 Everyone is permitted to copy and distribute verbatim copies of this
 license document, but changing it is not allowed.
 
-Preamble
-~~~~~~~~
+## Preamble
 
-The GNU General Public License is a free, copyleft license for software
-and other kinds of works.
+The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
 
-The licenses for most software and other practical works are designed to
-take away your freedom to share and change the works. By contrast, the
-GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users. We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors. You can apply it to
-your programs, too.
-
-When we speak of free software, we are referring to freedom, not price.
-Our General Public Licenses are designed to make sure that you have the
-freedom to distribute copies of free software (and charge for them if
-you wish), that you receive source code or can get it if you want it,
-that you can change the software or use pieces of it in new free
-programs, and that you know you can do these things.
-
-To protect your rights, we need to prevent others from denying you these
-rights or asking you to surrender the rights. Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-For example, if you distribute copies of such a program, whether gratis
-or for a fee, you must pass on to the recipients the same freedoms that
-you received. You must make sure that they, too, receive or can get the
-source code. And you must show them these terms so they know their
-rights.
-
-Developers that use the GNU GPL protect your rights with two steps: (1)
-assert copyright on the software, and (2) offer you this License giving
-you legal permission to copy, distribute and/or modify it.
+The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works. By contrast,
+the GNU General Public License is intended to guarantee your freedom
+to share and change all versions of a program--to make sure it remains
+free software for all its users. We, the Free Software Foundation, use
+the GNU General Public License for most of our software; it applies
+also to any other work released this way by its authors. You can apply
+it to your programs, too.
+
+When we speak of free software, we are referring to freedom, not
+price. Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights. Therefore, you
+have certain responsibilities if you distribute copies of the
+software, or if you modify it: responsibilities to respect the freedom
+of others.
+
+For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received. You must make sure that they, too, receive
+or can get the source code. And you must show them these terms so they
+know their rights.
+
+Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
 
 For the developers' and authors' protection, the GPL clearly explains
 that there is no warranty for this free software. For both users' and
 authors' sake, the GPL requires that modified versions be marked as
 changed, so that their problems will not be attributed erroneously to
 authors of previous versions.
 
 Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so. This is fundamentally incompatible with the aim of protecting
-users' freedom to change the software. The systematic pattern of such
-abuse occurs in the area of products for individuals to use, which is
-precisely where it is most unacceptable. Therefore, we have designed
-this version of the GPL to prohibit the practice for those products. If
-such problems arise substantially in other domains, we stand ready to
-extend this provision to those domains in future versions of the GPL, as
-needed to protect the freedom of users.
+modified versions of the software inside them, although the
+manufacturer can do so. This is fundamentally incompatible with the
+aim of protecting users' freedom to change the software. The
+systematic pattern of such abuse occurs in the area of products for
+individuals to use, which is precisely where it is most unacceptable.
+Therefore, we have designed this version of the GPL to prohibit the
+practice for those products. If such problems arise substantially in
+other domains, we stand ready to extend this provision to those
+domains in future versions of the GPL, as needed to protect the
+freedom of users.
 
 Finally, every program is threatened constantly by software patents.
 States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary. To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
+software on general-purpose computers, but in those that do, we wish
+to avoid the special danger that patents applied to a free program
+could make it effectively proprietary. To prevent this, the GPL
+assures that patents cannot be used to render the program non-free.
 
 The precise terms and conditions for copying, distribution and
 modification follow.
 
-TERMS AND CONDITIONS
-~~~~~~~~~~~~~~~~~~~~
+## TERMS AND CONDITIONS
 
-0. Definitions.
-^^^^^^^^^^^^^^^
+### 0. Definitions.
 
 "This License" refers to version 3 of the GNU General Public License.
 
-"Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
+"Copyright" also means copyright-like laws that apply to other kinds
+of works, such as semiconductor masks.
 
 "The Program" refers to any copyrightable work licensed under this
 License. Each licensee is addressed as "you". "Licensees" and
 "recipients" may be individuals or organizations.
 
 To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy. The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
+in a fashion requiring copyright permission, other than the making of
+an exact copy. The resulting work is called a "modified version" of
+the earlier work or a work "based on" the earlier work.
 
-A "covered work" means either the unmodified Program or a work based on
-the Program.
+A "covered work" means either the unmodified Program or a work based
+on the Program.
 
 To "propagate" a work means to do anything with it that, without
 permission, would make you directly or secondarily liable for
 infringement under applicable copyright law, except executing it on a
 computer or modifying a private copy. Propagation includes copying,
 distribution (with or without modification), making available to the
 public, and in some countries other activities as well.
 
 To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies. Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
+parties to make or receive copies. Mere interaction with a user
+through a computer network, with no transfer of a copy, is not
+conveying.
 
 An interactive user interface displays "Appropriate Legal Notices" to
-the extent that it includes a convenient and prominently visible feature
-that (1) displays an appropriate copyright notice, and (2) tells the
-user that there is no warranty for the work (except to the extent that
-warranties are provided), that licensees may convey the work under this
-License, and how to view a copy of this License. If the interface
-presents a list of user commands or options, such as a menu, a prominent
-item in the list meets this criterion.
+the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License. If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
 
-1. Source Code.
-^^^^^^^^^^^^^^^
+### 1. Source Code.
 
 The "source code" for a work means the preferred form of the work for
-making modifications to it. "Object code" means any non-source form of a
-work.
+making modifications to it. "Object code" means any non-source form of
+a work.
 
 A "Standard Interface" means an interface that either is an official
 standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that is
-widely used among developers working in that language.
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
 
 The "System Libraries" of an executable work include anything, other
 than the work as a whole, that (a) is included in the normal form of
 packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that Major
-Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form. A "Major
-Component", in this context, means a major essential component (kernel,
-window system, and so on) of the specific operating system (if any) on
-which the executable work runs, or a compiler used to produce the work,
-or an object code interpreter used to run it.
-
-The "Corresponding Source" for a work in object code form means all the
-source code needed to generate, install, and (for an executable work)
-run the object code and to modify the work, including scripts to control
-those activities. However, it does not include the work's System
-Libraries, or general-purpose tools or generally available free programs
-which are used unmodified in performing those activities but which are
-not part of the work. For example, Corresponding Source includes
-interface definition files associated with source files for the work,
-and the source code for shared libraries and dynamically linked
-subprograms that the work is specifically designed to require, such as
-by intimate data communication or control flow between those subprograms
-and other parts of the work.
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form. A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities. However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work. For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
 
 The Corresponding Source need not include anything that users can
 regenerate automatically from other parts of the Corresponding Source.
 
 The Corresponding Source for a work in source code form is that same
 work.
 
-2. Basic Permissions.
-^^^^^^^^^^^^^^^^^^^^^
+### 2. Basic Permissions.
 
 All rights granted under this License are granted for the term of
 copyright on the Program, and are irrevocable provided the stated
 conditions are met. This License explicitly affirms your unlimited
 permission to run the unmodified Program. The output from running a
 covered work is covered by this License only if the output, given its
 content, constitutes a covered work. This License acknowledges your
@@ -179,487 +177,463 @@
 control, on terms that prohibit them from making any copies of your
 copyrighted material outside their relationship with you.
 
 Conveying under any other circumstances is permitted solely under the
 conditions stated below. Sublicensing is not allowed; section 10 makes
 it unnecessary.
 
-3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### 3. Protecting Users' Legal Rights From Anti-Circumvention Law.
 
 No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article 11
-of the WIPO copyright treaty adopted on 20 December 1996, or similar
-laws prohibiting or restricting circumvention of such measures.
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
 
 When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to the
-covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
+circumvention of technological measures to the extent such
+circumvention is effected by exercising rights under this License with
+respect to the covered work, and you disclaim any intention to limit
+operation or modification of the work as a means of enforcing, against
+the work's users, your or third parties' legal rights to forbid
+circumvention of technological measures.
 
-4. Conveying Verbatim Copies.
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### 4. Conveying Verbatim Copies.
 
 You may convey verbatim copies of the Program's source code as you
 receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice; keep
-intact all notices stating that this License and any non-permissive
-terms added in accord with section 7 apply to the code; keep intact all
-notices of the absence of any warranty; and give all recipients a copy
-of this License along with the Program.
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
 
-You may charge any price or no price for each copy that you convey, and
-you may offer support or warranty protection for a fee.
+You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
 
-5. Conveying Modified Source Versions.
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### 5. Conveying Modified Source Versions.
 
 You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the terms
-of section 4, provided that you also meet all of these conditions:
-
-a) The work must carry prominent notices stating that you modified
-   it, and giving a relevant date.
-
-b) The work must carry prominent notices stating that it is released
-   under this License and any conditions added under section 7. This
-   requirement modifies the requirement in section 4 to "keep intact
-   all notices".
-
-c) You must license the entire work, as a whole, under this License
-   to anyone who comes into possession of a copy. This License will
-   therefore apply, along with any applicable section 7 additional
-   terms, to the whole of the work, and all its parts, regardless of
-   how they are packaged. This License gives no permission to license
-   the work in any other way, but it does not invalidate such
-   permission if you have separately received it.
-
-d) If the work has interactive user interfaces, each must display
-   Appropriate Legal Notices; however, if the Program has interactive
-   interfaces that do not display Appropriate Legal Notices, your
-   work need not make them do so.
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these
+conditions:
+
+- a) The work must carry prominent notices stating that you modified
+  it, and giving a relevant date.
+- b) The work must carry prominent notices stating that it is
+  released under this License and any conditions added under
+  section 7. This requirement modifies the requirement in section 4
+  to "keep intact all notices".
+- c) You must license the entire work, as a whole, under this
+  License to anyone who comes into possession of a copy. This
+  License will therefore apply, along with any applicable section 7
+  additional terms, to the whole of the work, and all its parts,
+  regardless of how they are packaged. This License gives no
+  permission to license the work in any other way, but it does not
+  invalidate such permission if you have separately received it.
+- d) If the work has interactive user interfaces, each must display
+  Appropriate Legal Notices; however, if the Program has interactive
+  interfaces that do not display Appropriate Legal Notices, your
+  work need not make them do so.
 
 A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work, and
-which are not combined with it such as to form a larger program, in or
-on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not used
-to limit the access or legal rights of the compilation's users beyond
-what the individual works permit. Inclusion of a covered work in an
-aggregate does not cause this License to apply to the other parts of the
-aggregate.
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit. Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
 
-6. Conveying Non-Source Forms.
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### 6. Conveying Non-Source Forms.
 
 You may convey a covered work in object code form under the terms of
 sections 4 and 5, provided that you also convey the machine-readable
 Corresponding Source under the terms of this License, in one of these
 ways:
 
-a) Convey the object code in, or embodied in, a physical product
-   (including a physical distribution medium), accompanied by the
-   Corresponding Source fixed on a durable physical medium
-   customarily used for software interchange.
-
-b) Convey the object code in, or embodied in, a physical product
-   (including a physical distribution medium), accompanied by a
-   written offer, valid for at least three years and valid for as
-   long as you offer spare parts or customer support for that product
-   model, to give anyone who possesses the object code either (1) a
-   copy of the Corresponding Source for all the software in the
-   product that is covered by this License, on a durable physical
-   medium customarily used for software interchange, for a price no
-   more than your reasonable cost of physically performing this
-   conveying of source, or (2) access to copy the Corresponding
-   Source from a network server at no charge.
-
-c) Convey individual copies of the object code with a copy of the
-   written offer to provide the Corresponding Source. This
-   alternative is allowed only occasionally and noncommercially, and
-   only if you received the object code with such an offer, in accord
-   with subsection 6b.
-
-d) Convey the object code by offering access from a designated place
-   (gratis or for a charge), and offer equivalent access to the
-   Corresponding Source in the same way through the same place at no
-   further charge. You need not require recipients to copy the
-   Corresponding Source along with the object code. If the place to
-   copy the object code is a network server, the Corresponding Source
-   may be on a different server (operated by you or a third party)
-   that supports equivalent copying facilities, provided you maintain
-   clear directions next to the object code saying where to find the
-   Corresponding Source. Regardless of what server hosts the
-   Corresponding Source, you remain obligated to ensure that it is
-   available for as long as needed to satisfy these requirements.
-
-e) Convey the object code using peer-to-peer transmission, provided
-   you inform other peers where the object code and Corresponding
-   Source of the work are being offered to the general public at no
-   charge under subsection 6d.
+- a) Convey the object code in, or embodied in, a physical product
+  (including a physical distribution medium), accompanied by the
+  Corresponding Source fixed on a durable physical medium
+  customarily used for software interchange.
+- b) Convey the object code in, or embodied in, a physical product
+  (including a physical distribution medium), accompanied by a
+  written offer, valid for at least three years and valid for as
+  long as you offer spare parts or customer support for that product
+  model, to give anyone who possesses the object code either (1) a
+  copy of the Corresponding Source for all the software in the
+  product that is covered by this License, on a durable physical
+  medium customarily used for software interchange, for a price no
+  more than your reasonable cost of physically performing this
+  conveying of source, or (2) access to copy the Corresponding
+  Source from a network server at no charge.
+- c) Convey individual copies of the object code with a copy of the
+  written offer to provide the Corresponding Source. This
+  alternative is allowed only occasionally and noncommercially, and
+  only if you received the object code with such an offer, in accord
+  with subsection 6b.
+- d) Convey the object code by offering access from a designated
+  place (gratis or for a charge), and offer equivalent access to the
+  Corresponding Source in the same way through the same place at no
+  further charge. You need not require recipients to copy the
+  Corresponding Source along with the object code. If the place to
+  copy the object code is a network server, the Corresponding Source
+  may be on a different server (operated by you or a third party)
+  that supports equivalent copying facilities, provided you maintain
+  clear directions next to the object code saying where to find the
+  Corresponding Source. Regardless of what server hosts the
+  Corresponding Source, you remain obligated to ensure that it is
+  available for as long as needed to satisfy these requirements.
+- e) Convey the object code using peer-to-peer transmission,
+  provided you inform other peers where the object code and
+  Corresponding Source of the work are being offered to the general
+  public at no charge under subsection 6d.
 
 A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be included
-in conveying the object code work.
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
 
 A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for
+tangible personal property which is normally used for personal,
+family, or household purposes, or (2) anything designed or sold for
 incorporation into a dwelling. In determining whether a product is a
-consumer product, doubtful cases shall be resolved in favor of coverage.
-For a particular product received by a particular user, "normally used"
-refers to a typical or common use of that class of product, regardless
-of the status of the particular user or of the way in which the
-particular user actually uses, or expects or is expected to use, the
-product. A product is a consumer product regardless of whether the
-product has substantial commercial, industrial or non-consumer uses,
-unless such uses represent the only significant mode of use of the
-product.
+consumer product, doubtful cases shall be resolved in favor of
+coverage. For a particular product received by a particular user,
+"normally used" refers to a typical or common use of that class of
+product, regardless of the status of the particular user or of the way
+in which the particular user actually uses, or expects or is expected
+to use, the product. A product is a consumer product regardless of
+whether the product has substantial commercial, industrial or
+non-consumer uses, unless such uses represent the only significant
+mode of use of the product.
 
 "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product
-from a modified version of its Corresponding Source. The information
-must suffice to ensure that the continued functioning of the modified
-object code is in no case prevented or interfered with solely because
-modification has been made.
+procedures, authorization keys, or other information required to
+install and execute modified versions of a covered work in that User
+Product from a modified version of its Corresponding Source. The
+information must suffice to ensure that the continued functioning of
+the modified object code is in no case prevented or interfered with
+solely because modification has been made.
 
 If you convey an object code work under this section in, or with, or
 specifically for use in, a User Product, and the conveying occurs as
 part of a transaction in which the right of possession and use of the
 User Product is transferred to the recipient in perpetuity or for a
 fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied by
-the Installation Information. But this requirement does not apply if
-neither you nor any third party retains the ability to install modified
-object code on the User Product (for example, the work has been
-installed in ROM).
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information. But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
 
 The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed. Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-Corresponding Source conveyed, and Installation Information provided, in
-accord with this section must be in a format that is publicly documented
-(and with an implementation available to the public in source code
-form), and must require no special password or key for unpacking,
-reading or copying.
+requirement to continue to provide support service, warranty, or
+updates for a work that has been modified or installed by the
+recipient, or for the User Product in which it has been modified or
+installed. Access to a network may be denied when the modification
+itself materially and adversely affects the operation of the network
+or violates the rules and protocols for communication across the
+network.
+
+Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
 
-7. Additional Terms.
-^^^^^^^^^^^^^^^^^^^^
+### 7. Additional Terms.
 
 "Additional permissions" are terms that supplement the terms of this
 License by making exceptions from one or more of its conditions.
 Additional permissions that are applicable to the entire Program shall
 be treated as though they were included in this License, to the extent
 that they are valid under applicable law. If additional permissions
 apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by this
-License without regard to the additional permissions.
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
 
-When you convey a copy of a covered work, you may at your option remove
-any additional permissions from that copy, or from any part of it.
-(Additional permissions may be written to require their own removal in
-certain cases when you modify the work.) You may place additional
-permissions on material, added by you to a covered work, for which you
-have or can give appropriate copyright permission.
+When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it. (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.) You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
 
 Notwithstanding any other provision of this License, for material you
 add to a covered work, you may (if authorized by the copyright holders
 of that material) supplement the terms of this License with terms:
 
-a) Disclaiming warranty or limiting liability differently from the
-   terms of sections 15 and 16 of this License; or
-
-b) Requiring preservation of specified reasonable legal notices or
-   author attributions in that material or in the Appropriate Legal
-   Notices displayed by works containing it; or
-
-c) Prohibiting misrepresentation of the origin of that material, or
-   requiring that modified versions of such material be marked in
-   reasonable ways as different from the original version; or
-
-d) Limiting the use for publicity purposes of names of licensors or
-   authors of the material; or
-
-e) Declining to grant rights under trademark law for use of some
-   trade names, trademarks, or service marks; or
-
-f) Requiring indemnification of licensors and authors of that
-   material by anyone who conveys the material (or modified versions
-   of it) with contractual assumptions of liability to the recipient,
-   for any liability that these contractual assumptions directly
-   impose on those licensors and authors.
+- a) Disclaiming warranty or limiting liability differently from the
+  terms of sections 15 and 16 of this License; or
+- b) Requiring preservation of specified reasonable legal notices or
+  author attributions in that material or in the Appropriate Legal
+  Notices displayed by works containing it; or
+- c) Prohibiting misrepresentation of the origin of that material,
+  or requiring that modified versions of such material be marked in
+  reasonable ways as different from the original version; or
+- d) Limiting the use for publicity purposes of names of licensors
+  or authors of the material; or
+- e) Declining to grant rights under trademark law for use of some
+  trade names, trademarks, or service marks; or
+- f) Requiring indemnification of licensors and authors of that
+  material by anyone who conveys the material (or modified versions
+  of it) with contractual assumptions of liability to the recipient,
+  for any liability that these contractual assumptions directly
+  impose on those licensors and authors.
 
 All other non-permissive additional terms are considered "further
 restrictions" within the meaning of section 10. If the Program as you
 received it, or any part of it, contains a notice stating that it is
 governed by this License along with a term that is a further
-restriction, you may remove that term. If a license document contains a
-further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms of
-that license document, provided that the further restriction does not
-survive such relicensing or conveying.
-
-If you add terms to a covered work in accord with this section, you must
-place, in the relevant source files, a statement of the additional terms
-that apply to those files, or a notice indicating where to find the
-applicable terms.
+restriction, you may remove that term. If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
 
 Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions; the above
-requirements apply either way.
+form of a separately written license, or stated as exceptions; the
+above requirements apply either way.
 
-8. Termination.
-^^^^^^^^^^^^^^^
+### 8. Termination.
 
 You may not propagate or modify a covered work except as expressly
 provided under this License. Any attempt otherwise to propagate or
 modify it is void, and will automatically terminate your rights under
 this License (including any patent licenses granted under the third
 paragraph of section 11).
 
 However, if you cease all violation of this License, then your license
 from a particular copyright holder is reinstated (a) provisionally,
-unless and until the copyright holder explicitly and finally terminates
-your license, and (b) permanently, if the copyright holder fails to
-notify you of the violation by some reasonable means prior to 60 days
-after the cessation.
-
-Moreover, your license from a particular copyright holder is reinstated
-permanently if the copyright holder notifies you of the violation by
-some reasonable means, this is the first time you have received notice
-of violation of this License (for any work) from that copyright holder,
-and you cure the violation prior to 30 days after your receipt of the
-notice.
+unless and until the copyright holder explicitly and finally
+terminates your license, and (b) permanently, if the copyright holder
+fails to notify you of the violation by some reasonable means prior to
+60 days after the cessation.
+
+Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
 
 Termination of your rights under this section does not terminate the
 licenses of parties who have received copies or rights from you under
 this License. If your rights have been terminated and not permanently
 reinstated, you do not qualify to receive new licenses for the same
 material under section 10.
 
-9. Acceptance Not Required for Having Copies.
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### 9. Acceptance Not Required for Having Copies.
 
-You are not required to accept this License in order to receive or run a
-copy of the Program. Ancillary propagation of a covered work occurring
-solely as a consequence of using peer-to-peer transmission to receive a
-copy likewise does not require acceptance. However, nothing other than
-this License grants you permission to propagate or modify any covered
-work. These actions infringe copyright if you do not accept this
-License. Therefore, by modifying or propagating a covered work, you
-indicate your acceptance of this License to do so.
+You are not required to accept this License in order to receive or run
+a copy of the Program. Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance. However,
+nothing other than this License grants you permission to propagate or
+modify any covered work. These actions infringe copyright if you do
+not accept this License. Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
 
-10. Automatic Licensing of Downstream Recipients.
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### 10. Automatic Licensing of Downstream Recipients.
 
 Each time you convey a covered work, the recipient automatically
 receives a license from the original licensors, to run, modify and
 propagate that work, subject to this License. You are not responsible
 for enforcing compliance by third parties with this License.
 
 An "entity transaction" is a transaction transferring control of an
 organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations. If propagation of a covered work
-results from an entity transaction, each party to that transaction who
-receives a copy of the work also receives whatever licenses to the work
-the party's predecessor in interest had or could give under the previous
-paragraph, plus a right to possession of the Corresponding Source of the
-work from the predecessor in interest, if the predecessor has it or can
-get it with reasonable efforts.
+organization, or merging organizations. If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
 
 You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License. For example, you may not
-impose a license fee, royalty, or other charge for exercise of rights
-granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that any
-patent claim is infringed by making, using, selling, offering for sale,
-or importing the Program or any portion of it.
+rights granted or affirmed under this License. For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
 
-11. Patents.
-^^^^^^^^^^^^
+### 11. Patents.
 
 A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based. The work
-thus licensed is called the contributor's "contributor version".
+License of the Program or a work on which the Program is based. The
+work thus licensed is called the contributor's "contributor version".
 
-A contributor's "essential patent claims" are all patent claims owned or
-controlled by the contributor, whether already acquired or hereafter
-acquired, that would be infringed by some manner, permitted by this
-License, of making, using, or selling its contributor version, but do
-not include claims that would be infringed only as a consequence of
-further modification of the contributor version. For purposes of this
-definition, "control" includes the right to grant patent sublicenses in
-a manner consistent with the requirements of this License.
+A contributor's "essential patent claims" are all patent claims owned
+or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version. For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
 
 Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to make,
-use, sell, offer for sale, import and otherwise run, modify and
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
 propagate the contents of its contributor version.
 
 In the following three paragraphs, a "patent license" is any express
 agreement or commitment, however denominated, not to enforce a patent
 (such as an express permission to practice a patent or covenant not to
 sue for patent infringement). To "grant" such a patent license to a
 party means to make such an agreement or commitment not to enforce a
 patent against the party.
 
-If you convey a covered work, knowingly relying on a patent license, and
-the Corresponding Source of the work is not available for anyone to
-copy, free of charge and under the terms of this License, through a
+If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
 publicly available network server or other readily accessible means,
 then you must either (1) cause the Corresponding Source to be so
 available, or (2) arrange to deprive yourself of the benefit of the
 patent license for this particular work, or (3) arrange, in a manner
 consistent with the requirements of this License, to extend the patent
 license to downstream recipients. "Knowingly relying" means you have
 actual knowledge that, but for the patent license, your conveying the
 covered work in a country, or your recipient's use of the covered work
 in a country, would infringe one or more identifiable patents in that
 country that you have reason to believe are valid.
 
 If, pursuant to or in connection with a single transaction or
 arrangement, you convey, or propagate by procuring conveyance of, a
 covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify or
-convey a specific copy of the covered work, then the patent license you
-grant is automatically extended to all recipients of the covered work
-and works based on it.
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
 
 A patent license is "discriminatory" if it does not include within the
 scope of its coverage, prohibits the exercise of, or is conditioned on
 the non-exercise of one or more of the rights that are specifically
-granted under this License. You may not convey a covered work if you are
-a party to an arrangement with a third party that is in the business of
-distributing software, under which you make payment to the third party
-based on the extent of your activity of conveying the work, and under
-which the third party grants, to any of the parties who would receive
-the covered work from you, a discriminatory patent license (a) in
-connection with copies of the covered work conveyed by you (or copies
-made from those copies), or (b) primarily for and in connection with
-specific products or compilations that contain the covered work, unless
-you entered into that arrangement, or that patent license was granted,
-prior to 28 March 2007.
-
-Nothing in this License shall be construed as excluding or limiting any
-implied license or other defenses to infringement that may otherwise be
-available to you under applicable patent law.
+granted under this License. You may not convey a covered work if you
+are a party to an arrangement with a third party that is in the
+business of distributing software, under which you make payment to the
+third party based on the extent of your activity of conveying the
+work, and under which the third party grants, to any of the parties
+who would receive the covered work from you, a discriminatory patent
+license (a) in connection with copies of the covered work conveyed by
+you (or copies made from those copies), or (b) primarily for and in
+connection with specific products or compilations that contain the
+covered work, unless you entered into that arrangement, or that patent
+license was granted, prior to 28 March 2007.
+
+Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
 
-12. No Surrender of Others' Freedom.
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### 12. No Surrender of Others' Freedom.
 
 If conditions are imposed on you (whether by court order, agreement or
 otherwise) that contradict the conditions of this License, they do not
 excuse you from the conditions of this License. If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you
-may not convey it at all. For example, if you agree to terms that
-obligate you to collect a royalty for further conveying from those to
-whom you convey the Program, the only way you could satisfy both those
-terms and this License would be to refrain entirely from conveying the
-Program.
-
-13. Use with the GNU Affero General Public License.
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-Notwithstanding any other provision of this License, you have permission
-to link or combine any covered work with a work licensed under version 3
-of the GNU Affero General Public License into a single combined work,
-and to convey the resulting work. The terms of this License will
-continue to apply to the part which is the covered work, but the special
-requirements of the GNU Affero General Public License, section 13,
-concerning interaction through a network will apply to the combination
-as such.
-
-14. Revised Versions of this License.
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time. Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
+covered work so as to satisfy simultaneously your obligations under
+this License and any other pertinent obligations, then as a
+consequence you may not convey it at all. For example, if you agree to
+terms that obligate you to collect a royalty for further conveying
+from those to whom you convey the Program, the only way you could
+satisfy both those terms and this License would be to refrain entirely
+from conveying the Program.
+
+### 13. Use with the GNU Affero General Public License.
+
+Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work. The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+### 14. Revised Versions of this License.
+
+The Free Software Foundation may publish revised and/or new versions
+of the GNU General Public License from time to time. Such new versions
+will be similar in spirit to the present version, but may differ in
+detail to address new problems or concerns.
 
 Each version is given a distinguishing version number. If the Program
 specifies that a certain numbered version of the GNU General Public
 License "or any later version" applies to it, you have the option of
-following the terms and conditions either of that numbered version or of
-any later version published by the Free Software Foundation. If the
+following the terms and conditions either of that numbered version or
+of any later version published by the Free Software Foundation. If the
 Program does not specify a version number of the GNU General Public
-License, you may choose any version ever published by the Free Software
-Foundation.
+License, you may choose any version ever published by the Free
+Software Foundation.
 
 If the Program specifies that a proxy can decide which future versions
 of the GNU General Public License can be used, that proxy's public
 statement of acceptance of a version permanently authorizes you to
 choose that version for the Program.
 
-Later license versions may give you additional or different permissions.
-However, no additional obligations are imposed on any author or
-copyright holder as a result of your choosing to follow a later version.
+Later license versions may give you additional or different
+permissions. However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
 
-15. Disclaimer of Warranty.
-^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### 15. Disclaimer of Warranty.
 
 THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
 APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
 HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT
 WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT
-LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
-PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF
-THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME
-THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND
+PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE
+DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR
+CORRECTION.
 
-16. Limitation of Liability.
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### 16. Limitation of Liability.
 
 IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
 WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR
 CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
 INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES
 ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT
-NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES
-SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE
-WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN
-ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
-
-17. Interpretation of Sections 15 and 16.
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-If the disclaimer of warranty and limitation of liability provided above
-cannot be given local legal effect according to their terms, reviewing
-courts shall apply local law that most closely approximates an absolute
-waiver of all civil liability in connection with the Program, unless a
-warranty or assumption of liability accompanies a copy of the Program in
-return for a fee.
+NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR
+LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM
+TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER
+PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
+
+### 17. Interpretation of Sections 15 and 16.
+
+If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
 
 END OF TERMS AND CONDITIONS
 
-How to Apply These Terms to Your New Programs
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+## How to Apply These Terms to Your New Programs
 
 If you develop a new program, and you want it to be of the greatest
 possible use to the public, the best way to achieve this is to make it
 free software which everyone can redistribute and change under these
 terms.
 
 To do so, attach the following notices to the program. It is safest to
 attach them to the start of each source file to most effectively state
 the exclusion of warranty; and each file should have at least the
 "copyright" line and a pointer to where the full notice is found.
 
-::
-
         <one line to give the program's name and a brief idea of what it does.>
         Copyright (C) <year>  <name of author>
 
         This program is free software: you can redistribute it and/or modify
         it under the terms of the GNU General Public License as published by
         the Free Software Foundation, either version 3 of the License, or
         (at your option) any later version.
@@ -668,35 +642,34 @@
         but WITHOUT ANY WARRANTY; without even the implied warranty of
         MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
         GNU General Public License for more details.
 
         You should have received a copy of the GNU General Public License
         along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-Also add information on how to contact you by electronic and paper mail.
-
-If the program does terminal interaction, make it output a short notice
-like this when it starts in an interactive mode:
+Also add information on how to contact you by electronic and paper
+mail.
 
-::
+If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
 
         <program>  Copyright (C) <year>  <name of author>
         This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
         This is free software, and you are welcome to redistribute it
         under certain conditions; type `show c' for details.
 
 The hypothetical commands \`show w' and \`show c' should show the
 appropriate parts of the General Public License. Of course, your
 program's commands might be different; for a GUI interface, you would
 use an "about box".
 
 You should also get your employer (if you work as a programmer) or
 school, if any, to sign a "copyright disclaimer" for the program, if
-necessary. For more information on this, and how to apply and follow the
-GNU GPL, see https://www.gnu.org/licenses/.
+necessary. For more information on this, and how to apply and follow
+the GNU GPL, see <https://www.gnu.org/licenses/>.
 
 The GNU General Public License does not permit incorporating your
 program into proprietary programs. If your program is a subroutine
 library, you may consider it more useful to permit linking proprietary
 applications with the library. If this is what you want to do, use the
 GNU Lesser General Public License instead of this License. But first,
-please read https://www.gnu.org/licenses/why-not-lgpl.html.
+please read <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `ragraph-1.19.0/pyproject.toml` & `ragraph-1.19.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ragraph"
-version = "1.19.0"
+version = "1.19.1"
 description = "Ratio graph handling in Python."
 authors = ["Ratio Innovations B.V. <info@ratio-case.nl>"]
 license = "GPL-3.0-or-later"
 documentation = "https://ragraph.ratio-case.nl"
-readme = "README.rst"
+readme = "README.md"
 repository = "https://gitlab.com/ratio-case-os/python/ragraph"
 homepage = "https://ragraph.ratio-case.nl"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 dd = { version = "^0.5" }
 lxml = { version = "^4" }
 numpy = { version = "^1" }
 plotly = { version = "^5" }
 "ruamel.yaml" = "^0.17"
 kaleido = { version = "0.2.1", optional = true }
-raesl = { version = "*", optional = true }
+raesl = { version = "^0", optional = true }
 ratio-genetic-py = "^0.3"
 
 [tool.poetry.extras]
 esl = ["raesl"]
 plot = ["kaleido"]
 all = ["kaleido", "raesl"]
 
@@ -37,34 +37,24 @@
 [tool.poetry.group.experiment.dependencies]
 jupyterlab = "^3"
 pandas = "^1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-cov = "*"
-pytest-doctestplus = "*"
-
-[tool.poetry.group.docs.dependencies]
-pydata-sphinx-theme = { version = "*" }
-pygments-csv-lexer = { version = "*" }
-Sphinx = { version = "*" }
-sphinx-autoapi = { version = "*" }
-sphinx-copybutton = { version = "*" }
-sphinx-prompt = { version = "*" }
-sphinxcontrib-bibtex = { version = "*" }
-sphinxemoji = { version = "*" }
+pytest-examples = "*"
 
 [tool.black]
 line-length = 100
 target-version = ["py39"]
 
 [tool.pytest.ini_options]
-addopts = "-s --cov --cov-report xml:./.pytest_cache/coverage.xml --cov-report term-missing --doctest-plus --doctest-rst --basetemp ./tests/.temp"
-testpaths = ["docs", "tests"]
-markers = ["slow"]
+addopts = "-s --cov --cov-report xml:./.pytest_cache/coverage.xml --cov-report term-missing --basetemp ./tests/.temp"
+testpaths = ["tests"]
+markers = ["slow", "format"]
 
 [tool.coverage.run]
 source = [
     "ragraph",
     "/usr/local/lib/python3.9/site-packages/ragraph",
     "/home/ratio/.local/lib/python3.9/site-packages/ragraph",
 ]
@@ -84,11 +74,11 @@
 [tool.raver]
 ref = "origin/main"
 changelog = "./docs/source/changelog.rst"
 
 [tool.ruff]
 line-length = 100
 select = [
-  "E",   # pycodestyle
-  "F",   # pyflakes
+    "E", # pycodestyle
+    "F", # pyflakes
 ]
 target-version = "py39"
```

### Comparing `ragraph-1.19.0/ragraph/analysis/_classes.py` & `ragraph-1.19.1/ragraph/analysis/_classes.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/analysis/_utils.py` & `ragraph-1.19.1/ragraph/analysis/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-"""Utility functions for managing the graph object during analysis."""
+"""# RaGraph analysis utilities
+
+Utility functions for managing the graph object during analysis.
+"""
 
 from copy import copy
 from typing import Iterable, List, Optional, Union
 
 from ragraph.graph import Graph
 from ragraph.node import Node
 
@@ -50,15 +53,15 @@
 
     Arguments:
         graph: Graph to check availability in.
         prefix: Node name prefix, will be appended by first available integer.
         lower: Lower bound for integer to append to name prefix.
 
     Returns:
-        First available node name not in :obj:`graph.node_dict`.
+        First available node name not in [`graph.node_dict`][ragraph.graph.Graph.node_dict].
     """
     available = False
     i = lower
     while not available:
         name = prefix + str(i)
         available = name not in graph.node_dict
         i += 1
@@ -99,30 +102,30 @@
 
     for i in new_parent_nodes:
         for j in new_parent_nodes:
             if i == j:
                 continue
             for child_edge_ij in graph.edges_between_all(i.children, j.children):
                 edge_ij = copy(child_edge_ij)
-                edge_ij.name = None
+                edge_ij.name = None  # type: ignore
                 edge_ij.source = i
                 edge_ij.target = j
                 graph.add_edge(edge_ij)
 
     for i in new_parent_nodes:
         for j in parent_sibling_nodes:
             for child_edge_ij in graph.edges_between_all(i.children, [j]):
                 edge_ij = copy(child_edge_ij)
-                edge_ij.name = None
+                edge_ij.name = None  # type: ignore
                 edge_ij.source = i
                 edge_ij.target = j
                 graph.add_edge(edge_ij)
             for child_edge_ji in graph.edges_between_all([j], i.children):
                 edge_ji = copy(child_edge_ji)
-                edge_ji.name = None
+                edge_ji.name = None  # type: ignore
                 edge_ji.source = j
                 edge_ji.target = i
                 graph.add_edge(edge_ji)
 
 
 def set_children(graph: Graph, parent: Node, children: List[Node]) -> None:
     """Safely set children of parent node.
@@ -165,37 +168,37 @@
     Note:
         The node is has its parent unset and is therefore removed from the parent's
         children. The parent may have just a single other child left, in which case
         that child node should replace the parent altogether. When it has more children,
         it is kept intact.
 
     Example:
-        Unsetting the parent of "a" in the following tree:
-
-        .. code-block::
+        Resetting the parent of "a" in the following tree:
 
-                   g
-               ____|____
-              |         |
-              e         f
-             _|_     ___|___
-            |   |   |   |   |
-            a   b   c   d   e
+        ```
+               g
+           ____|____
+          |         |
+          e         f
+         _|_     ___|___
+        |   |   |   |   |
+        a   b   c   d   e
+        ```
 
         leaves the following forest:
 
-        .. code-block::
-
-            a        g
-                 ____|____
-                |         |
-                b         f
-                       ___|___
-                      |   |   |
-                      c   d   e
+        ```
+        a        g
+             ____|____
+            |         |
+            b         f
+                   ___|___
+                  |   |   |
+                  c   d   e
+        ```
 
         in which "a" has become a root and "b" has become a child of "g" since "e" has
         been removed.
     """
     parent = node.parent
     if not parent:
         return
```

### Comparing `ragraph-1.19.0/ragraph/analysis/bus/__init__.py` & `ragraph-1.19.1/ragraph/analysis/bus/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,30 @@
-"""
-########################
-Bus detection algorithms
-########################
+"""# Bus detection algorithms
 
 Bus detection algorithms find bus nodes in graphs, also called "hubs" or "integrative
 components". Typical bus nodes have a high node degree or "centrality" score.
 
 All bus detection algorithms have the following arguments:
 
-* ``graph``: Graph to find bus nodes in.
-* ``root``: Root node to perform bus detection in.
-* ``leafs``: Optional list of leaf nodes to consider during the bus detection cycle. If
+- `graph`: Graph to find bus nodes in.
+- `root`: Root node to perform bus detection in.
+- `leafs`: Optional list of leaf nodes to consider during the bus detection cycle. If
   not supplied, the leaf node descendants of the root will be considered.
 
 They always return two lists of nodes:
 
-* Leaf nodes that have been marked as bus nodes
-* The remaining leaf nodes.
+- Leaf nodes that have been marked as bus nodes.
+- The remaining leaf nodes.
 
 They currently do **NOT** change anything in the graph in-place. That is up to the user.
 
-********************
-Available algorithms
-********************
+## Available algorithms
 
 The following algorithms are directly available after importing
-:obj:`ragraph.analysis.bus`:
+[`ragraph.analysis.bus`][ragraph.analysis.bus]:
 
-* :func:`gamma() <ragraph.analysis.bus.gamma.gamma_bus_detection>`: Gamma bus detection.
+- [`gamma`][ragraph.analysis.bus.gamma]: Gamma bus detection.
 """
-# flake8: noqa, ignore errors on unused imports here.
 
 from ragraph.analysis.bus._gamma import gamma_bus_detection as gamma
+
+__all__ = ["gamma"]
```

### Comparing `ragraph-1.19.0/ragraph/analysis/bus/_gamma.py` & `ragraph-1.19.1/ragraph/analysis/bus/_gamma.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-"""Gamma bus detection module.
+"""
+# Gamma bus detection
 
-Wilschut, T., Etman, L. F. P., Rooda, J. E., & Adan, I. J. B. F. (2017). Multilevel
- Flow-Based Markov Clustering for Design Structure Matrices. Journal of Mechanical
- Design, 139(12), 121402. https://doi.org/10.1115/1.4037626
+References:
+    Wilschut, T., Etman, L. F. P., Rooda, J. E., & Adan, I. J. B. F. (2017). Multilevel
+    Flow-Based Markov Clustering for Design Structure Matrices. Journal of Mechanical
+    Design, 139(12), 121402. [DOI: 10.1115/1.4037626](https://doi.org/10.1115/1.4037626)
 """
 
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
+
 from ragraph.analysis._classes import Bound, BusAnalysis, Parameter
 from ragraph.graph import Graph, Node
 
 gamma_params = {
     p.name: p
     for p in [
         Parameter(
@@ -43,18 +46,18 @@
     loops: bool = False,
     edge_weights: Optional[List[str]] = None,
     names: bool = False,
     gamma: float = gamma_params["gamma"].default,  # type: ignore
     safe: bool = True,
     **kwargs,
 ) -> Union[Tuple[List[Node], List[Node]], Tuple[List[str], List[str]]]:
-    """Detect bus nodes in an adjacency matrix.
+    """Detect bus nodes in a graph.
 
     Arguments:
-        matrix: Adjacency matrix.
+        graph: Graph to detect bus nodes in.
         root: Root node of this bus detection analysis.
         leafs: Optional list of nodes to consider leafs during this bus detection cycle.
         inherit: Whether edges between descendants of nodes should be taken into account
             (if applicable).
         loops: Whether self-loop edges should be taken into account (if applicable).
         gamma: Bus threshold w.r.t. median of nonzero node degrees.
         names: Whether to return node names or node instances.
@@ -62,14 +65,19 @@
     Returns:
         Bus leafs.
         Nonbus leafs.
 
     Note:
         Works by selecting node degree outliers by some factor gamma w.r.t. median of
         nonzero node degrees.
+
+    Reference:
+        Wilschut, T., Etman, L. F. P., Rooda, J. E., & Adan, I. J. B. F. (2017). Multilevel
+        Flow-Based Markov Clustering for Design Structure Matrices. Journal of Mechanical
+        Design, 139(12), 121402. https://doi.org/10.1115/1.4037626
     """
     matrix = graph.get_adjacency_matrix(
         nodes=leafs, inherit=inherit, loops=loops, only=edge_weights
     )
     assert isinstance(matrix, np.ndarray)
     assert leafs is not None
     dim = matrix.shape[0]
@@ -102,10 +110,7 @@
         bus_leafs = [leafs[i] for i in bus_idxs]
         nonbus_leafs = [leafs[i] for i in nonbus_idxs]
     else:
         bus_leafs = []
         nonbus_leafs = leafs
 
     return bus_leafs, nonbus_leafs
-
-
-assert gamma_analysis.method
```

### Comparing `ragraph-1.19.0/ragraph/analysis/cluster/_markov.py` & `ragraph-1.19.1/ragraph/analysis/cluster/_markov.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-"""Markov clustering module.
+"""
+# Markov clustering module
 
- Wilschut, T., Etman, L. F. P., Rooda, J. E., & Adan, I. J. B. F. (2017). Multilevel
- Flow-Based Markov Clustering for Design Structure Matrices. Journal of Mechanical
- Design, 139(12), 121402. https://doi.org/10.1115/1.4037626
+Reference:
+    Wilschut, T., Etman, L. F. P., Rooda, J. E., & Adan, I. J. B. F. (2017). Multilevel
+    Flow-Based Markov Clustering for Design Structure Matrices. Journal of Mechanical
+    Design, 139(12), 121402. [DOI: 10.1115/1.4037626](https://doi.org/10.1115/1.4037626)
 """
 
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 from numpy.linalg import LinAlgError
+
 from ragraph.analysis._classes import Bound, ClusterAnalysis, Parameter
 from ragraph.analysis._utils import create_parent
 from ragraph.graph import Graph, Node
 
 markov_params = {
     p.name: p
     for p in [
@@ -67,15 +70,15 @@
     description="Hierarchically cluster the graph in place using Hierarchical Markov "
     + "clustering.",
     parameters=markov_params,
 )
 
 
 @hierarchical_markov_analysis
-def hierarchical_markov_clustering(
+def hierarchical_markov(
     graph: Graph,
     root: Optional[Union[str, Node]] = None,
     leafs: Optional[Union[List[Node], List[str]]] = None,
     inherit: bool = True,
     loops: bool = False,
     edge_weights: Optional[List[str]] = None,
     alpha: int = markov_params["alpha"].default,  # type: ignore
@@ -84,21 +87,22 @@
     max_iter: int = markov_params["max_iter"].default,  # type: ignore
     symmetrize: bool = markov_params["symmetrize"].default,  # type: ignore
     inplace: bool = True,
     names: bool = False,
     safe: bool = True,
     **kwargs,
 ) -> Tuple[Graph, Union[List[Node], List[str]]]:
+    """docstring stub"""
     cluster_roots: List[Node] = [] if leafs is None else leafs  # type: ignore
     children: List[Node] = []
 
     while set(cluster_roots) != set(children) and len(cluster_roots) > 1:
         # Previous cluster_roots become children for new cluster level.
         children = cluster_roots
-        graph, cluster_roots = markov_clustering(
+        graph, cluster_roots = markov(
             graph,
             root=None,
             leafs=children,
             inherit=inherit,
             loops=loops,
             edge_weights=edge_weights,
             alpha=alpha,
@@ -115,15 +119,15 @@
     "Markov clustering",
     description="Cluster the graph in place using Markov Clustering.",
     parameters=markov_params,
 )
 
 
 @markov_analysis
-def markov_clustering(
+def markov(
     graph: Graph,
     root: Optional[Union[str, Node]] = None,
     leafs: Optional[Union[List[Node], List[str]]] = None,
     inherit: bool = True,
     loops: bool = False,
     edge_weights: Optional[List[str]] = None,
     alpha: int = markov_params["alpha"].default,  # type: ignore
@@ -132,14 +136,15 @@
     max_iter: int = markov_params["max_iter"].default,  # type: ignore
     symmetrize: bool = markov_params["symmetrize"],  # type: ignore
     inplace: bool = True,
     names: bool = False,
     safe: bool = True,
     **kwargs,
 ) -> Tuple[Graph, Union[List[Node], List[str]]]:
+    """docstring stub"""
     assert leafs is not None
     mat = graph.get_adjacency_matrix(leafs, inherit=inherit, loops=loops, only=edge_weights)
     assert isinstance(mat, np.ndarray)
     if symmetrize:
         mat = mat + mat.T  # Add transpose to get a guaranteed symmetrical matrix.
     tpm = calculate_tpm(mat, mu)
     if alpha > 1:  # Otherwise algorithm does nothing, then column max -> cluster ID.
@@ -324,28 +329,32 @@
         else:
             f_in = np.ones((self.dim + 1, 1))
             f_in[-1, 0] = 0
         return f_in
 
     @property
     def flow_vector(self) -> np.ndarray:
-        """Flow through every node if system is injected with :obj:`self.in_vector`."""
+        """Flow through every node if system is injected with
+        [`self.in_vector`][ragraph.analysis.cluster._markov.MarkovFlow.in_vector].
+        """
         return self.sensitivity_matrix @ self.in_vector
 
     @property
     def flow_matrix(self) -> np.ndarray:
-        """Flow over every edge if nodal flow equal :obj:`self.flow_vector`."""
+        """Flow over every edge if nodal flow equal
+        [`self.flow_vector`][ragraph.analysis.cluster._markov.MarkovFlow.flow_vector].
+        """
         return self.sink_matrix * self.flow_vector.T
 
 
 class MarkovRelative:
     """Markov relative influence and dependency calculations.
 
     Arguments:
-        matrix: Adjacency matrix (non-negative, IR/FAD convention).
+        adj: Adjacency matrix (non-negative, IR/FAD convention).
         mu: Evaporation constant (>1.0).
 
     Note:
         Solves specific cases of the Markov flow analysis where each node is injected
         with a flow of 1 to calculate the relative influence. The network is also
         reversed and injected again, which results in relative dependency.
     """
```

### Comparing `ragraph-1.19.0/ragraph/analysis/cluster/_tarjan.py` & `ragraph-1.19.1/ragraph/analysis/cluster/_tarjan.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,46 @@
-"""Tarjan's strongly connected components algorithm.
+"""
+# Tarjan's strongly connected components algorithm.
 
 Reference:
     Tarjan, R. (1972). Depth-First Search and Linear Graph Algorithms.
-        SIAM Journal on Computing, 1(2), 146-160. https://doi.org/10.1137/0201010
+    SIAM Journal on Computing, 1(2), 146-160.
+    [DOI: 10.1137/0201010] (https://doi.org/10.1137/0201010)
 """
 from textwrap import dedent
 from typing import Dict, List, Optional, Tuple, Union
 
 from ragraph.analysis._classes import ClusterAnalysis
 from ragraph.analysis._utils import create_parent
 from ragraph.graph import Graph
 from ragraph.node import Node
 
 tarjans_scc_analysis = ClusterAnalysis(
     "Tarjan's strongly connected components clustering algorithm.",
     description=dedent(
         """Clusters all strongly connected components (cycles) in a graph.
-        Ignores the :obj:`loops` and :obj:`edge_weights` parameters."""
+        Ignores the `loops` and `edge_weights` parameters."""
     ),
 )
 
 
 @tarjans_scc_analysis
-def tarjans_scc_clustering(
+def tarjans_scc(
     graph: Graph,
     root: Optional[Union[str, Node]] = None,
     leafs: Optional[Union[List[Node], List[str]]] = None,
     inherit: bool = True,
     loops: bool = False,
     edge_weights: Optional[List[str]] = None,
     inplace: bool = True,
     names: bool = False,
     safe: bool = True,
     **kwargs,
 ) -> Tuple[Graph, Union[List[Node], List[str]]]:
+    """docstring stub"""
     assert leafs is not None
     clusters = tarjans_scc_algorithm(graph, leafs, inherit)  # type: ignore
 
     cluster_roots = []
     for children in clusters:
         if len(children) > 1:
             parent = create_parent(graph, children)
```

### Comparing `ragraph-1.19.0/ragraph/analysis/comparison/_delta.py` & `ragraph-1.19.1/ragraph/analysis/comparison/_delta.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Delta analysis module."""
+"""# Delta analysis"""
 
 
 from typing import Type
 
 from ragraph.analysis.comparison.utils import (
     EdgeDescriptor,
     EdgeDescriptorLike,
@@ -32,16 +32,16 @@
         delta_a: Name for nodes and edges unique to the first graph.
         delta_b: Name for nodes and edges unique to the second graph.
         common: Name for the common nodes and edges occurring in both graphs.
 
     Note:
         Graphs are compared on leaf node level and compared by name only.
         Please provide appropriate input as such and look to
-        :obj:`~ragraph.graph.Graph.get_graph_slice` for example on how to obtain a subgraph to
-        your liking.
+        [`get_graph_slice`][ragraph.graph.Graph.get_graph_slice] for example on how to obtain a
+        subgraph to your liking.
     """
     graph = Graph(name="delta", kind="delta")
 
     # Compare leaf nodes by name. Set to unique A first and change to common if found again.
     nds_a = set(node_descriptor.from_node(n) for n in graph_a.leafs)
     nds_b = set(node_descriptor.from_node(n) for n in graph_b.leafs)
     for n in nds_a.difference(nds_b):
```

### Comparing `ragraph-1.19.0/ragraph/analysis/comparison/_sigma.py` & `ragraph-1.19.1/ragraph/analysis/comparison/_sigma.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Sigma analysis module. """
+"""# Sigma analysis"""
 
 import enum
 from copy import deepcopy
 from typing import Iterable
 
 from ragraph.edge import Edge
 from ragraph.generic import Metadata
@@ -26,15 +26,16 @@
         graphs: Graphs to sum and count edge occurrences in.
         mode: Whether to count absolute occurrence values or an average per graph.
         count_prefix: Which weight key (prefix) to store the occurrence values under. Also used as
             a prefix for label counts that are stored as weights using as well.
 
     Note:
         Summations are done over (leaf) node names. Edges in an input graph are aggregated first
-        using the :obj:`add_meta` method before being aggregated into the resulting graph.
+        using the [`add_meta` method][ragraph.analysis.comparison.add_meta]
+        before being aggregated into the resulting graph.
     """
     accumulator = Graph(name="sigma")
     num = 0
     for graph in graphs:
         # Override that first one's results because of default values for a Graph.
         add_graph(accumulator, graph, count_prefix, num == 0)
         num += 1
@@ -111,15 +112,16 @@
 
 
 def add_nodes(accumulator: Graph, item: Graph, count_prefix: str):
     """Add observed nodes in item to the accumulator in-place and keep track of an occurrence count.
 
     Based on node names.
 
-    Metadata for existing nodes is added using :obj:`add_meta`.
+    Metadata for existing nodes is added using
+    [`add_meta` method][ragraph.analysis.comparison.add_meta].
     """
     for n in item.leafs:
         try:
             add_meta(accumulator[n.name], n, count_prefix)
         except KeyError:
             node = Node(name=n.name)
             add_meta(node, n, count_prefix, is_first=True)
@@ -127,15 +129,16 @@
 
 
 def add_edges(accumulator: Graph, item: Graph, count_prefix: str):
     """Add observed edges in item to the accumulator in-place.
 
     Based on node names.
 
-    Metadata for existing nodes is added using :obj:`add_meta`.
+    Metadata for existing nodes is added using
+    [`add_meta` method][ragraph.analysis.comparison.add_meta].
     """
     for source_name, tgt_map in item.directed_edges.items():
         for target_name, item_edges in tgt_map.items():
             # Take a deepcopy of the list of edges in the item and aggregate those first.
             item_edges = deepcopy(item_edges)
             item_edge = item_edges.pop()
             for e in item_edges:
```

### Comparing `ragraph-1.19.0/ragraph/analysis/comparison/utils.py` & `ragraph-1.19.1/ragraph/analysis/comparison/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""# Comparison analysis utilities"""
 import enum
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import FrozenSet, Tuple
 
 from ragraph.edge import Edge
 from ragraph.generic import Metadata
```

### Comparing `ragraph-1.19.0/ragraph/analysis/compatibility/__init__.py` & `ragraph-1.19.1/ragraph/analysis/compatibility/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-"""Compatibility analysis between different variants for several functional elements."""
+"""# Compatibility analysis
+
+Calculate compatibility between different variants for several functional elements.
+"""
 
 from copy import deepcopy
 from itertools import combinations
 from math import prod
 from pathlib import Path
 from typing import Callable, Dict, Generator, Iterable, List, Optional, Tuple, Union
 
 from plotly import graph_objs as go
+
 from ragraph.analysis.compatibility.bdd import yield_feasible_configurations
 from ragraph.edge import Edge
 from ragraph.graph import Graph
 from ragraph.node import Node
 from ragraph.plot import generic, mdm
 
 try:  # pragma: no cover
@@ -202,15 +206,16 @@
             guard for whether compatibility checking is necessary when
             `interface_compatibility` is set.
         compatibility_method: A method accepting a Graph and two variant nodes to check
             whether the two given variants are compatible (by returning `True`).
         interface_compatibility: When set, the compatibility of two variants is only
             checked when they share an interface.
         score_method: A method accepting a tuple of variant nodes and
-            returning a single performance score. See :obj:`get_score_method`.
+            returning a single performance score. See
+            [`get_score_method`][ragraph.analysis.compatibility.get_score_method].
         constraints: Optional list of constraint nodes ("project scope") for which
             variants must be applicable in order to be taken into account.
         applicability_method: A method accepting a graph, a variant node and a
             constraint node that returns whether a variant is applicable when that
             constraint is set.
     """
 
@@ -230,33 +235,50 @@
         labels=generic.LabelsStyle(shorten=False),
     )
 
     def __init__(
         self,
         graph: Graph,
         variants: Dict[str, List[Node]],
-        interface_method: Callable[[Graph, Node, Node], bool] = None,
+        interface_method: Optional[Callable[[Graph, Node, Node], bool]] = None,
         compatibility_method: Callable[[Graph, Node, Node], bool] = get_compatibility_method(
             compatibility_kind="compatibility", incompatibility_kind=None
         ),
         interface_compatibility: bool = True,
         score_method: Callable[[Tuple[Node, ...]], float] = get_score_method(
             variant_agg="sum", config_agg="sum", weights=None
         ),
         constraints: Optional[List[Node]] = None,
         applicability_method: Callable[[Graph, Node, Node], bool] = get_applicability_method(
             applicability_kind="applicability", inapplicability_kind=None
         ),
     ):
         self.graph = graph
+        """Graph containing compatibility data between different variants."""
+
         self.interface_method = interface_method
+        """An optional method accepting a Graph and two variant nodes that returns whether the two
+        given variants have an interface. Acts as a guard for whether compatibility checking is
+        necessary when `interface_compatibility` is set."""
+
         self.compatibility_method = compatibility_method
+        """A method accepting a Graph and two variant nodes to check whether the two given variants
+        are compatible (by returning `True`)."""
+
         self.interface_compatibility = interface_compatibility
+        """When set, the compatibility of two variants is only checked when they share an interface.
+        """
+
         self.applicability_method = applicability_method
+        """A method accepting a graph, a variant node and a constraint node that returns whether a
+        variant is applicable when that constraint is set."""
+
         self.score_method = score_method
+        """A method accepting a tuple of variant nodes and returning a single performance score.
+        See [`get_score_method`][ragraph.analysis.compatibility.get_score_method]."""
 
         self._elements: List[str] = []
         self._element_nums: List[int] = []
         self._disabled_elements: List[str] = []
 
         self._constraints: List[Node] = [] if constraints is None else constraints
 
@@ -294,22 +316,22 @@
     def constraints(self, value: List[Node]):
         self._constraints = value
         self.variants = self._variants  # Re-trigger variants setter.
 
     @property
     def elements(self) -> List[str]:
         """Enabled elements with at least one applicable variant.
-        See :obj:`self.constraints` and :obj:`self.applicability_method`
+        See `self.constraints` and `self.applicability_method`.
         """
         return self._elements
 
     @property
     def disabled_elements(self) -> List[str]:
         """Disabled elements with no applicable variant.
-        See :obj:`self.constraints` and :obj:`self.applicability_method`
+        See `self.constraints` and `self.applicability_method`.
         """
         return self._disabled_elements
 
     @property
     def element_nums(self) -> List[int]:
         """Number of applicable variants per element."""
         return self._element_nums
@@ -317,28 +339,28 @@
     @property
     def variants_list(self) -> List[Node]:
         """Flat list of applicable variants sorted by (enabled) element."""
         return self._variants_list
 
     def is_applicable(self, variant: Node) -> bool:
         """Whether a variant is applicable to the currently set of constraints."""
-        if not self.constraints or not self.applicability_method:
-            return True
-        return all(
-            self.applicability_method(self.graph, variant, constraint)
-            for constraint in self.constraints
-        )
+        if self.constraints:
+            return all(
+                self.applicability_method(self.graph, variant, constraint)
+                for constraint in self.constraints
+            )
+        return True
 
     def has_interface(self, var1: Node, var2: Node) -> bool:
         """Whether two variants have an interface that needs a compatibility check."""
         return (self.interface_method is None) or self.interface_method(self.graph, var1, var2)
 
     def is_compatible(self, var1: Node, var2: Node) -> bool:
         """Whether the two given variants are compatible according to
-        :obj:`self.compatibility_method`
+        [`self.applicability_method`][ragraph.analysis.compatibility.CompatibilityAnalysis.applicability_method]
         """
 
         if self.interface_compatibility:
             return (
                 self.compatibility_method(self.graph, var1, var2)
                 if self.has_interface(var1, var2)
                 else True
```

### Comparing `ragraph-1.19.0/ragraph/analysis/compatibility/bdd.py` & `ragraph-1.19.1/ragraph/analysis/compatibility/bdd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-"""Binary Decision Diagram implementation of the compatibility problem."""
+"""# Binary Decision Diagram compatibility calculation
+
+Binary Decision Diagram (BDD) implementation of the compatibility problem.
+"""
 from typing import Generator, List, Tuple, Union
 
 import dd.autoref as _bdd
 import numpy as np
 
 
 def _yield_ranges(nums: List[int], start: int = 0) -> Generator[range, None, None]:
```

### Comparing `ragraph-1.19.0/ragraph/analysis/heuristics/_johnson.py` & `ragraph-1.19.1/ragraph/analysis/heuristics/_johnson.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""Donald B. Johnson's nested circuit finding algorithm."""
+"""# Donald B. Johnson's nested circuit finding algorithm"""
 from collections import defaultdict
 from typing import Dict, Generator, List, Optional, Set, Union
 
 from ragraph.analysis.cluster._tarjan import tarjans_scc_algorithm
 from ragraph.graph import Graph
 from ragraph.node import Node
 
 
-def circuit_finding_algorithm(
+def johnson(
     graph: Graph,
     nodes: Optional[List[Node]] = None,
     names: bool = False,
     inherit: bool = True,
     **kwargs,
 ) -> Generator[Union[List[str], List[Node]], None, None]:
     """Donald B. Johnson's nested circuit finding algorithm. A circuit is a cycle in a
```

### Comparing `ragraph-1.19.0/ragraph/analysis/heuristics/_markov_gamma.py` & `ragraph-1.19.1/ragraph/analysis/heuristics/_markov_gamma.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-"""Heuristic that combines Hierarchical Markov Clustering (HMC) with Gamma bus
-detection.
-"""
+"""# Hierarchical Markov Clustering (HMC) with Gamma bus detection."""
 from textwrap import dedent
 from typing import List, Optional, Tuple, Union
 
 from ragraph.analysis import _utils
 from ragraph.analysis._classes import ClusterAnalysis, Parameter
 from ragraph.analysis.bus._gamma import gamma_bus_detection, gamma_params
 from ragraph.analysis.cluster._markov import (
-    hierarchical_markov_clustering,
+    hierarchical_markov,
     markov_params,
 )
 from ragraph.graph import Graph, Node
 
 markov_gamma_params = {
     p.name: p
     for p in [
@@ -42,15 +40,15 @@
     """
     ),
     parameters=markov_gamma_params,
 )
 
 
 @markov_gamma_analysis
-def markov_gamma_clustering(
+def markov_gamma(
     graph: Graph,
     root: Optional[Union[str, Node]] = None,
     leafs: Optional[Union[List[Node], List[str]]] = None,
     inherit: bool = True,
     loops: bool = False,
     edge_weights: Optional[List[str]] = None,
     alpha: int = markov_gamma_params["alpha"].default,  # type: ignore
@@ -63,15 +61,15 @@
     inplace: bool = True,
     names: bool = False,
     safe: bool = True,
     **kwargs,
 ) -> Union[List[Node], Tuple[Graph, List[Node]]]:
     """Cluster a given graph hierarchically with buses on a local level or globally."""
     assert leafs is not None
-    graph, roots = hierarchical_markov_clustering(
+    graph, roots = hierarchical_markov(
         graph,
         root=root,
         leafs=leafs,
         inherit=inherit,
         loops=loops,
         alpha=alpha,
         beta=beta,
@@ -105,15 +103,15 @@
         # Bus detected!
         if bus_leafs:
             # Unset local hierarchy.
             _utils.clear_local_hierarchy(graph, local_leafs, [local_root])
             local_root.children = None
 
             # Recalculate the nonbus hierarchy.
-            graph, nonbus_roots = hierarchical_markov_clustering(
+            graph, nonbus_roots = hierarchical_markov(
                 graph,
                 alpha=alpha,
                 beta=beta,
                 mu=mu,
                 root=None,
                 leafs=nonbus_leafs,
                 inherit=inherit,
@@ -124,15 +122,15 @@
                 symmetrize=symmetrize,
                 names=False,
                 safe=False,
             )
             _utils.set_children(graph, local_root, nonbus_roots)
 
             # Recalculate the bus hierarchy.
-            graph, bus_roots = hierarchical_markov_clustering(
+            graph, bus_roots = hierarchical_markov(
                 graph,
                 alpha=alpha,
                 beta=beta,
                 mu=mu,
                 root=None,
                 leafs=bus_leafs,
                 inherit=inherit,
```

### Comparing `ragraph-1.19.0/ragraph/analysis/sequence/_axis.py` & `ragraph-1.19.1/ragraph/analysis/sequence/_axis.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,31 +19,29 @@
         else:
             return value
 
 
 axis_sequencing_analysis = SequenceAnalysis(
     "Plot axis sequencing. Get nodes in a plot-axis-ready order.",
     description=dedent(
-        """\
-        Order nodes for a typical display on matrix plot axis. They are sorted by:
+        """Order nodes for a typical display on matrix plot axis. They are sorted by:
           1. Node kinds in order of (supplied) occurrence.
           2. Top-down hierarchy.
           3. Optional: Bus-nodes before nonbus-nodes in w.r.t. siblings.
           4. Optional: Node width (e.g. size in terms of leaf nodes).
 
         Note:
             Axis ready means ordered by kind and buses nodes first where possible.
 
         Note:
-            :obj:`inherit`, :obj:`loops`, and :obj:`edge_weights` are ignored for this
-            analysis.
+            `inherit`, `loops`, and `edge_weights` are ignored for this analysis.
 
         Warning:
-            When supplying node kinds it's your own responsibility to make sure
-            that each node's kind actually is included in that node kind order.
+            When supplying node kinds it's your own responsibility to make sure that each node's
+            kind actually is included in that node kind order.
         """
     ),
     parameters={
         "kinds": Parameter(
             "kinds",
             Optional[List[str]],
             description="Optional order of node kinds.",
@@ -324,24 +322,25 @@
     elif sort_by_width:
         return -get_width(node, width_cache)
     else:
         return 0
 
 
 @axis_sequencing_analysis
-def axis_sequencing(
+def axis(
     graph: Graph,
     root: Optional[Union[str, Node]] = None,
     nodes: Optional[Union[List[Node], List[str]]] = None,
     kinds: Optional[List[str]] = None,
     sort_by_bus: bool = True,
     sort_by_width: bool = True,
     edge_weights: Optional[List[str]] = None,
     inherit: bool = True,
     loops: bool = False,
     inplace: bool = True,
     names: bool = False,
     safe: bool = True,
     **kwargs,
 ):
+    """docstring stub"""
     seq = get_axis_sequence(nodes, kinds, sort_by_bus, sort_by_width)  # type: ignore
     return graph, seq
```

### Comparing `ragraph-1.19.0/ragraph/analysis/sequence/_genetic.py` & `ragraph-1.19.1/ragraph/analysis/sequence/_genetic.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     edge_weights: Optional[List[str]] = None,
     loops: bool = False,
     inplace: bool = True,
     names: bool = False,
     safe: bool = True,
     **kwargs,
 ) -> Tuple[Graph, List[Node]]:
+    """docstring stub"""
     lineage = genetic_sequencing(
         graph,
         nodes,  # type: ignore
         n_chromosomes,  # type: ignore
         n_generations,  # type: ignore
         1,
         p_crossover,  # type: ignore
```

### Comparing `ragraph-1.19.0/ragraph/analysis/sequence/_markov.py` & `ragraph-1.19.1/ragraph/analysis/sequence/_markov.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Sorting algorithm based on the node dependency/influence in a Markov chain.
 """
 from textwrap import dedent
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
+
 from ragraph.analysis._classes import Bound, Parameter, SequenceAnalysis
 from ragraph.analysis.sequence.metrics import net_markov_flow_adjacency
 from ragraph.graph import Graph, Node
 
 markov_params = {
     p.name: p
     for p in [
@@ -55,15 +56,15 @@
     """
     ),
     parameters=markov_params,
 )
 
 
 @markov_sequencing_analysis
-def markov_sequencing(
+def markov(
     graph: Graph,
     root: Optional[Union[str, Node]] = None,
     nodes: Optional[Union[List[Node], List[str]]] = None,
     edge_weights: Optional[List[str]] = None,
     inf: float = markov_params["inf"].default,  # type: ignore
     dep: float = markov_params["dep"].default,  # type: ignore
     mu: float = markov_params["mu"].default,  # type: ignore
@@ -71,14 +72,15 @@
     inherit: bool = True,
     loops: bool = False,
     inplace: bool = True,
     names: bool = False,
     safe: bool = True,
     **kwargs,
 ) -> Tuple[Graph, List[Node]]:
+    """docstring stub"""
     assert nodes is not None
     adj = graph.get_adjacency_matrix(nodes=nodes, inherit=inherit, loops=loops, only=edge_weights)
     assert isinstance(adj, np.ndarray)
 
     # Obtain node penalty scores.
     penalties = net_markov_flow_adjacency(adj, inf=inf, dep=dep, mu=mu, scale=scale)
```

### Comparing `ragraph-1.19.0/ragraph/analysis/sequence/_name.py` & `ragraph-1.19.1/ragraph/analysis/sequence/_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ragraph.analysis._classes import SequenceAnalysis
 from ragraph.graph import Graph, Node
 
 sort_by_name_analysis = SequenceAnalysis("Sort by name")
 
 
 @sort_by_name_analysis
-def sort_by_name(
+def name(
     graph: Graph,
     root: Optional[Union[str, Node]] = None,
     nodes: Optional[Union[List[str], List[Node]]] = None,
     inherit: bool = True,
     loops: bool = False,
     edge_weights: Optional[List[str]] = None,
     inplace: bool = True,
```

### Comparing `ragraph-1.19.0/ragraph/analysis/sequence/_scc_tearing.py` & `ragraph-1.19.1/ragraph/analysis/sequence/_scc_tearing.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     loops: bool = False,
     edge_weights: Optional[List[str]] = None,
     inplace: bool = True,
     names: bool = False,
     safe: bool = True,
     **kwargs,
 ) -> Tuple[Graph, List[Node]]:
+    """docstring stub"""
     sequence = scc_tearing_algorithm(
         graph, nodes, inherit, loops, decision, decision_args  # type: ignore
     )
     seq = list(sequence)
 
     return graph, seq
```

### Comparing `ragraph-1.19.0/ragraph/analysis/sequence/_tarjan.py` & `ragraph-1.19.1/ragraph/analysis/sequence/_tarjan.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,26 +13,27 @@
     Note:
         Can only parse nodes which form a directed acyclic graph (DAG).
     """,
 )
 
 
 @tarjans_dfs_analysis
-def tarjans_dfs_sequencing(
+def tarjans_dfs(
     graph: Graph,
     root: Optional[Union[str, Node]] = None,
     nodes: Optional[Union[List[str], List[Node]]] = None,
     inherit: bool = True,
     loops: bool = False,
     edge_weights: Optional[List[str]] = None,
     inplace: bool = True,
     names: bool = False,
     safe: bool = True,
     **kwargs,
 ) -> Tuple[Graph, List[Node]]:
+    """docstring stub"""
     assert nodes
     out = []
     unmarked = [n for n in nodes if isinstance(n, Node)]
     state = {n: "todo" for n in nodes}
 
     targets_of: Dict[Node, List[Node]] = {
         source: [
```

### Comparing `ragraph-1.19.0/ragraph/analysis/sequence/metrics.py` & `ragraph-1.19.1/ragraph/analysis/sequence/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Sequence metrics."""
 
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
+
 from ragraph.graph import Graph
 from ragraph.node import Node
 
 
 def feedback_marks(mat: np.ndarray) -> Tuple[float, np.ndarray]:
     """Measure the sum of feedback marks in an adjacency matrix.
 
@@ -36,15 +37,15 @@
     Returns:
         Resulting metric.
         Cell contribution matrix.
 
     References:
         Gebala, D. A., & Eppinger, S. D. (1991). Methods for analyzing design
             procedures. ASME Design Technical Conferences (Design Theory and
-            Methodology), 227–233. Miami.
+            Methodology), 227-233. Miami.
     """
     dim = len(mat)
 
     dimtile = np.tile(np.arange(dim), (dim, 1))
     ddist = dimtile - dimtile.T
 
     contrib = np.triu(mat, 1) * ddist
@@ -137,15 +138,15 @@
         except when this crossing is a feedback mark in itself. Multiple lines from
         "above" in the matrix are summed, those from the right are **NOT** (treated as
         binary).
 
     References:
         McCulley, C., and Bloebaum, C. L., 1996, “A Genetic Tool for Optimal Design
             Sequencing in Complex Engineering Systems,” Struct. Optim., 12(2), pp.
-            186–201.
+            186-201.
     """
     # Treat binary matrix
     mat = (mat > 0) * 1.0
 
     # contrib_fb is upper triangularized
     total_fb, contrib_fb = feedback_marks(mat)
```

### Comparing `ragraph-1.19.0/ragraph/analysis/sequence/utils.py` & `ragraph-1.19.1/ragraph/analysis/sequence/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 """Sequencing utils."""
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
+
 from ragraph.analysis import logger
 from ragraph.analysis._classes import BranchsortAnalysis
 from ragraph.analysis.sequence.metrics import net_markov_flow_adjacency
 from ragraph.graph import Graph, Node
 
 branchsort_analysis = BranchsortAnalysis(
     "Branchsort analysis",
-    description="""\
-    Sequence all branches in a hierarchy using any sequencing algorithm. Returns the
-    graph, (sequenced) root nodes and sequenced leaf nodes.
+    description="""Sequence all branches in a hierarchy using any sequencing algorithm. Returns
+    the graph, (sequenced) root nodes and sequenced leaf nodes.
 
     Note:
-        Setting just the :obj:`root` argument will sort it's children (recursively if
-        you want). Setting :obj:`nodes` is like setting multiple roots.
-        Setting :obj:`leafs` treats the given nodes as leaf nodes, whose children will
-        not be reordered.
+        Setting just the `root` argument will sort it's children (recursively if you want). Setting
+        `nodes` is like setting multiple roots. Setting `leafs` treats the given nodes as leaf
+        nodes, whose children will not be reordered.
 
     Note:
-        It is assumed that all edges are already nicely instantiated for all their
-        parent components. E.g., your root node should have it's own incoming and
-        outgoing edges.
+        It is assumed that all edges are already nicely instantiated for all their parent
+        components. E.g., your root node should have it's own incoming and outgoing edges.
     """,
 )
 
 
 @branchsort_analysis
 def branchsort(
     graph: Graph,
@@ -39,14 +37,15 @@
     inherit: bool = True,
     loops: bool = False,
     inplace: bool = True,
     recurse: bool = True,
     names: bool = False,
     safe: bool = True,
 ) -> Tuple[Graph, List[Node], List[Node]]:
+    """docstring stub"""
     # Sort roots
     assert isinstance(algo_args, dict)
     graph, node_sequence = algo(
         graph=graph,
         root=None,
         nodes=nodes,
         inherit=inherit,
```

### Comparing `ragraph-1.19.0/ragraph/analysis/similarity/__init__.py` & `ragraph-1.19.1/ragraph/analysis/similarity/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 """
-###################
-Similarity analyses
-###################
-
-Graph similarity is often expressed as a metric, where nodes and edges are scanned for
-similar patterns, properties, or other aspects. There are three levels of equivalence,
-being structural, automorphic, or regular equivalence. Where each of the former implies
-all latter equivalences, respectively.
+# Similarity analyses
 
+Graph similarity is often expressed as a metric, where nodes and edges are scanned for similar
+patterns, properties, or other aspects. There are three levels of equivalence, being structural,
+automorphic, or regular equivalence. Where each of the former implies all latter equivalences,
+respectively.
 
-******************
-Available analyses
-******************
+## Available analyses
 
 The following algorithms are directly accessible after importing
-:obj:`ragraph.analysis.similarity`:
+[`ragraph.analysis.similarity`][ragraph.analysis.similarity]:
 
-* :obj:`jaccard_index`: Jaccard Similarity Index of two objects based on the number
-  properties they both possess divided by the number of properties either of them have.
-* :obj:`jaccard_matrix`: Jaccard Similarity Index between a set of objects stored in a
-  square matrix.
-
-.. note:: Both Jaccard methods require a callable that takes an object and returns a
-   list of booleans representing the possession of a property (the :obj:`on` argument).
-   Some examples are included in the :mod:`ragraph.analysis.similarity.utils` module,
-   like :func:`ragraph.analysis.similarity.utils.on_hasattrs`.
+* [`jaccard_index`][ragraph.analysis.similarity.jaccard_matrix]: Jaccard Similarity Index of two
+  objects based on the number properties they both possess divided by the number of properties
+  either of them have.
+* [`jaccard_matrix`][ragraph.analysis.similarity.jaccard_matrix]: Jaccard Similarity Index between a
+  set of objects stored in a square matrix.
+
+Note:
+    Both Jaccard methods require a callable that takes an object and returns a list of booleans
+    representing the possession of a property (the `on` argument). Some examples are included in the
+    [`ragraph.analysis.similarity.utils`][ragraph.analysis.similarity.utils] module, like
+    [`ragraph.analysis.similarity.utils.on_hasattrs`][ragraph.analysis.similarity.utils.on_hasattrs].
 """
-# flake8: noqa, ignore errors on unused imports here.
 
 from ragraph.analysis.similarity._jaccard import jaccard_index, jaccard_matrix
 from ragraph.analysis.similarity._similarity import SimilarityAnalysis
+
+__all__ = ["jaccard_index", "jaccard_matrix", "SimilarityAnalysis"]
```

### Comparing `ragraph-1.19.0/ragraph/analysis/similarity/_jaccard.py` & `ragraph-1.19.1/ragraph/analysis/similarity/_jaccard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-"""Jaccard Similarity Index.
+"""# Jaccard Similarity Index
 
-The index compares two objects, and is calculated as the size of the overlap in
-properties divided by total size of properties they posess.
+The index compares two objects, and is calculated as the size of the overlap in properties divided
+by total size of properties they possess.
 
-For examples on 'object description functions', please refer to
-:obj:`ragraph.analysis.similarity.utils`.
+For examples on 'object description functions', please refer to [`the similarity
+utilities`][ragraph.analysis.similarity.utils].
 
-References: Kosub, S. (2016). A note on the triangle inequality for the Jaccard
-    distance. Retrieved from https://arxiv.org/pdf/1612.02696.pdf Jaccard, P. (1901).
-    Étude comparative de la distribution florale dans une portion des Alpes et du Jura.
-    Bulletin de La Société Vaudoise Des Sciences Naturelles.
-    https://doi.org/10.5169/seals-266450
+References:
+    Kosub, S. (2016). A note on the triangle inequality for the Jaccard distance. Retrieved from
+    [arXiv.org](https://arxiv.org/pdf/1612.02696.pdf) Jaccard, P. (1901). Étude comparative de la
+    distribution florale dans une portion des Alpes et du Jura. Bulletin de La Société Vaudoise Des
+    Sciences Naturelles. [DOI: 10.5169/seals-266450](https://doi.org/10.5169/seals-266450)
 """
 
 from typing import Any, Callable, List
 
 import numpy as np
```

### Comparing `ragraph-1.19.0/ragraph/analysis/similarity/_similarity.py` & `ragraph-1.19.1/ragraph/analysis/similarity/_similarity.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+"""# Similarity analysis"""
 from typing import Any, Callable, List, Tuple
 
 import numpy as np
+
 from ragraph.analysis import cluster, similarity
 from ragraph.edge import Edge
 from ragraph.graph import Graph
 from ragraph.node import Node
 
 
 class SimilarityAnalysis:
@@ -212,64 +214,66 @@
                         weights=dict(similarity=mat[row][col]),
                     )
                 )
 
     def cluster_rows(
         self,
         algo: Callable[[Graph, Any], Tuple[List[Node]]] = cluster.markov,
-        **algo_args,
+        **algo_args: Any,
     ) -> None:
         """Cluster column nodes based on their similarity. Updates Graph in-place.
 
         Arguments:
-            algo: Clustering algorithm. Should take a graph as first argument and
-                cluster it in-place. Defaults to :obj:`cluster.markov`.
-            **algo_args: Algorithm arguments. See :obj:`cluster.markov` for sensible
-                defaults.
+            algo: Clustering algorithm. Should take a graph as first argument and cluster it
+                in-place. Defaults to [`cluster.markov`][ragraph.analysis.cluster.markov].
+            **algo_args: Algorithm arguments. See
+                [`cluster.markov`][ragraph.analysis.cluster.markov] for sensible defaults.
         """
         self._cluster(self.rows, algo, **algo_args)
 
     def cluster_cols(
         self,
         algo: Callable[[Graph, Any], Tuple[List[Node]]] = cluster.markov,
-        **algo_args,
+        **algo_args: Any,
     ) -> None:
         """Cluster column nodes based on their similarity. Updates Graph in-place.
 
         Arguments:
-            algo: Clustering algorithm. Should take a graph as first argument and
-                cluster it in-place. Defaults to :obj:`cluster.markov`.
-            **algo_args: Algorithm arguments. See :obj:`cluster.markov` for sensible
-                defaults.
+            algo: Clustering algorithm. Should take a graph as first argument and cluster it
+                in-place. Defaults to [`cluster.markov`][ragraph.analysis.cluster.markov].
+            **algo_args: Algorithm arguments. See
+                [`cluster.markov`][ragraph.analysis.cluster.markov] for sensible defaults.
         """
         self._cluster(self.cols, algo, **algo_args)
 
     def _cluster(
         self,
         leafs: List[Node],
         algo: Callable[[Graph, Any], Tuple[List[Node]]] = cluster.markov,
-        **algo_args,
+        **algo_args: Any,
     ) -> None:
         """Cluster column nodes based on their similarity. Updates Graph in-place.
 
         Arguments:
             leafs: List of row or column nodes to be clustered.
-            algo: Clustering algorithm. Should take a graph as first argument and
-                cluster it in-place. Defaults to :obj:`cluster.markov`.
-            **algo_args: Algorithm arguments. See :obj:`cluster.markov` for sensible
-                defaults.
+            algo: Clustering algorithm. Should take a graph as first argument and cluster it
+                in-place. Defaults to [`cluster.markov`][ragraph.analysis.cluster.markov].
+            **algo_args: Algorithm arguments. See
+                [`cluster.markov`][ragraph.analysis.cluster.markov] for sensible defaults.
         """
         algo(self.graph, leafs=leafs, **algo_args, inplace=True)  # type: ignore
 
     def row_mapping(self, row: Node) -> List[bool]:
-        """Boolean possession checklist for a row node w.r.t. :obj:`self.cols`."""
+        """Boolean possession checklist for a row node w.r.t.
+        [`self.cols`][ragraph.analysis.similarity.SimilarityAnalysis.cols]."""
         return [self.check_mapping(col, row) for col in self.cols]
 
     def col_mapping(self, col: Node) -> List[bool]:
-        """Boolean possession checklist for a column node w.r.t. :obj:`self.rows`."""
+        """Boolean possession checklist for a column node w.r.t.
+        [`self.rows`][ragraph.analysis.similarity.SimilarityAnalysis.rows]."""
         return [self.check_mapping(col, row) for row in self.rows]
 
     def check_mapping(self, col: Node, row: Node) -> bool:
         """Check whether a column node maps to a row node."""
         if len(self.graph.directed_edges[col.name][row.name]) > 0:
             return True
         else:
```

### Comparing `ragraph-1.19.0/ragraph/analysis/similarity/utils.py` & `ragraph-1.19.1/ragraph/analysis/similarity/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-"""Similarity utilities."""
+"""#Similarity analysis utilities"""
 from typing import Any, Callable, List
 
 
 def on_hasattrs(attrs: List[str]) -> Callable[[Any], List[bool]]:
-    """Get an object description function that checks whether an instance possesses
-    certain attributes. It does not check the values thereof!
+    """Get an object description function that checks whether an instance possesses certain
+    attributes. It does not check the values thereof!
 
     Arguments:
         attrs: List of attributes to check the existence of.
 
     Returns:
         Object description function indicating attribute possession.
     """
     return lambda obj: [hasattr(obj, attr) for attr in attrs]
 
 
 def on_checks(checks: List[Callable[[Any], bool]]) -> Callable[[Any], List[bool]]:
-    """Get an object description function that runs a predefined set of checks (which
-    should be in a fixed order) and returns their boolean results.
+    """Get an object description function that runs a predefined set of checks (which should be in a
+    fixed order) and returns their boolean results.
 
     Arguments:
         checks: Checks to perform.
 
     Returns:
         Object description function indicating check passings.
     """
     return lambda obj: [check(obj) for check in checks]
 
 
 def on_hasweights(weights: List[str], threshold: float = 0.0) -> Callable[[Any], List[bool]]:
-    """Check whether an objects has certain weights above a threshold in its weights
-    dictionary property.
+    """Check whether an objects has certain weights above a threshold in its weights dictionary
+    property.
 
     Arguments:
-        weights: Keys to the :obj:`obj.weights` dictionary to check.
+        weights: Keys to the `obj.weights` dictionary to check.
         threshold: Threshold to verify against.
 
     Returns:
         Object description function indicating weights exceeding a threshold.
     """
     return lambda obj: [obj.weights.get(w, 0.0) >= threshold for w in weights]
 
 
 def on_contains(contents: List[Any]) -> Callable[[Any], List[bool]]:
     """Check whether an object contains certain contents.
 
     Arguments:
-        contents: Contents to check for with ``lambda x: x in obj``.
+        contents: Contents to check for with `lambda x: x in obj`.
 
     Returns:
         Object description function indicating content presence.
     """
     return lambda obj: [content in obj for content in contents]
```

### Comparing `ragraph-1.19.0/ragraph/colors/__init__.py` & `ragraph-1.19.1/ragraph/colors/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-"""Colors and palettes for RaGraph plots.
+"""# RaGraph colors and palettes
 
 This module contains several convenient methods to obtain color palettes as lists of
 hex-coded colors. The defaults for categorical and continuous data are
-:obj:`get_categorical` and :obj:`get_continuous`, respectively.
+[`get_categorical`][ragraph.colors.get_categorical] and
+[`get_continuous`][ragraph.colors.get_continuous], respectively.
 
 Additional methods are included, most of which are based on the
-:obj:`~ragraph.colors.cubehelix` palette with certain preset options.
-:obj:`get_hue` is a great way to get a sequential color palette for any hue where the
-hue value corresponds to anything between red (1.0), green (2.0) or blue (3.0).
-
-In our plots, these colors are *not* interpolated. This opens up an easy way to
-visualize your colors in a discrete fashion, since you merely need to supply a list with
-less colors (e.g. the desired number of discrete steps).
+[`cubehelix palette`][ragraph.colors.cubehelix.cubehelix_palette] with certain preset options.
+[`get_hue`][ragraph.colors.get_hue] is a great way to get a sequential color palette for any hue
+where the hue value corresponds to anything between red (1.0), green (2.0) or blue (3.0).
+
+In our plots, these colors are *not* interpolated. This opens up an easy way to visualize your
+colors in a discrete fashion, since you merely need to supply a list with less colors (e.g. the
+desired number of discrete steps).
 """
 from typing import Any, Dict, List
 
 from ragraph.colors.cubehelix import cubehelix_palette
 
 
 def get_categorical(n_colors: int = 10, **kwargs) -> List[str]:
@@ -25,15 +26,15 @@
         n_colors: Number of colors to generate.
 
     Returns:
         A list of colors as hex codes.
 
     Note:
         Additional keyword arguments are passed on to
-        :obj:`ragraph.colors.cubehelix.cubehelix_palette`.
+        [`cubehelix_palette`][ragraph.colors.cubehelix.cubehelix_palette].
     """
     n_colors = max(n_colors, 1)
     base_light = 0.6
     if n_colors <= 10:
         dark = base_light
         light = base_light
     else:
@@ -61,15 +62,15 @@
         n_colors: Number of colors to generate.
 
     Returns:
         A list of colors as hex codes.
 
     Note:
         Additional keyword arguments are passed on to
-        :obj:`ragraph.colors.cubehelix.cubehelix_palette`.
+        [`cubehelix_palette`][ragraph.colors.cubehelix.cubehelix_palette].
     """
     n_colors = max(n_colors, 1)
     opts: Dict[str, Any] = dict(
         n_colors=n_colors,
         start=2.25,
         end=3.45,
         dark=0.2,
@@ -90,15 +91,15 @@
         hue: Hue for this sequential color palette.
 
     Returns:
         A list of colors as hex codes.
 
     Note:
         Additional keyword arguments are passed on to
-        :obj:`ragraph.colors.cubehelix.cubehelix_palette`.
+        [`cubehelix_palette`][ragraph.colors.cubehelix.cubehelix_palette].
     """
     n_colors = max(n_colors, 1)
     opts: Dict[str, Any] = dict(
         n_colors=n_colors,
         start=hue,
         end=hue,
         dark=0.25,
@@ -118,15 +119,15 @@
         n_colors: Number of colors to generate.
 
     Returns:
         A list of colors as hex codes.
 
     Note:
         Additional keyword arguments are passed on to
-        :obj:`ragraph.colors.cubehelix.cubehelix_palette`.
+        [`cubehelix_palette`][ragraph.colors.cubehelix.cubehelix_palette].
     """
     opts: Dict[str, Any] = dict(hue=0.15, n_colors=n_colors)
     opts.update(**kwargs)
     return get_hue(**opts)
 
 
 def get_red(n_colors: int = 256, **kwargs) -> List[str]:
@@ -136,15 +137,15 @@
         n_colors: Number of colors to generate.
 
     Returns:
         A list of colors as hex codes.
 
     Note:
         Additional keyword arguments are passed on to
-        :obj:`ragraph.colors.cubehelix.cubehelix_palette`.
+        [`cubehelix_palette`][ragraph.colors.cubehelix.cubehelix_palette].
     """
     opts: Dict[str, Any] = dict(hue=0.95, n_colors=n_colors)
     opts.update(**kwargs)
     return get_hue(**opts)
 
 
 def get_orange(n_colors: int = 256, **kwargs) -> List[str]:
@@ -154,15 +155,15 @@
         n_colors: Number of colors to generate.
 
     Returns:
         A list of colors as hex codes.
 
     Note:
         Additional keyword arguments are passed on to
-        :obj:`ragraph.colors.cubehelix.cubehelix_palette`.
+        [`cubehelix_palette`][ragraph.colors.cubehelix.cubehelix_palette].
     """
     opts: Dict[str, Any] = dict(hue=1.2, n_colors=n_colors)
     opts.update(**kwargs)
     return get_hue(**opts)
 
 
 def get_green(n_colors: int = 256, **kwargs) -> List[str]:
@@ -172,15 +173,15 @@
         n_colors: Number of colors to generate.
 
     Returns:
         A list of colors as hex codes.
 
     Note:
         Additional keyword arguments are passed on to
-        :obj:`ragraph.colors.cubehelix.cubehelix_palette`.
+        [`cubehelix_palette`][ragraph.colors.cubehelix.cubehelix_palette].
     """
     opts: Dict[str, Any] = dict(hue=1.8, n_colors=n_colors)
     opts.update(**kwargs)
     return get_hue(**opts)
 
 
 def get_cyan(n_colors: int = 256, **kwargs) -> List[str]:
@@ -190,15 +191,15 @@
         n_colors: Number of colors to generate.
 
     Returns:
         A list of colors as hex codes.
 
     Note:
         Additional keyword arguments are passed on to
-        :obj:`ragraph.colors.cubehelix.cubehelix_palette`.
+        [`cubehelix_palette`][ragraph.colors.cubehelix.cubehelix_palette].
     """
     opts: Dict[str, Any] = dict(hue=2.45, n_colors=n_colors)
     opts.update(**kwargs)
     return get_hue(**opts)
 
 
 def get_blue(n_colors: int = 256, **kwargs) -> List[str]:
@@ -208,15 +209,15 @@
         n_colors: Number of colors to generate.
 
     Returns:
         A list of colors as hex codes.
 
     Note:
         Additional keyword arguments are passed on to
-        :obj:`ragraph.colors.cubehelix.cubehelix_palette`.
+        [`cubehelix_palette`][ragraph.colors.cubehelix.cubehelix_palette].
     """
     opts: Dict[str, Any] = dict(hue=2.85, n_colors=n_colors)
     opts.update(**kwargs)
     return get_hue(**opts)
 
 
 def get_diverging_hues(
@@ -235,15 +236,15 @@
         midpoint: Fraction between [0.0, 1.0] where to put the midpoint.
 
     Returns:
         A list of colors as hex codes.
 
     Note:
         Additional keyword arguments are passed on to
-        :obj:`ragraph.colors.cubehelix.cubehelix_palette`.
+        [`cubehelix_palette`][ragraph.colors.cubehelix.cubehelix_palette].
     """
     if n_colors <= 1:
         return ["#ffffff"]
 
     midindex = round(midpoint * (n_colors - 1))
     lower = get_hue(hue=lower_hue, n_colors=midindex + 1, **kwargs)
     upper = get_hue(hue=upper_hue, n_colors=n_colors - midindex, **kwargs)
@@ -257,15 +258,15 @@
         n_colors: Number of colors to generate.
 
     Returns:
         A list of colors as hex codes.
 
     Note:
         Additional keyword arguments are passed on to
-        :obj:`ragraph.colors.cubehelix.cubehelix_palette`.
+        [`cubehelix_palette`][ragraph.colors.cubehelix.cubehelix_palette].
     """
     opts: Dict[str, Any] = dict(lower_hue=0.95, upper_hue=2.85, n_colors=n_colors)
     opts.update(kwargs)
     return get_diverging_hues(**opts)
 
 
 def get_diverging_orangecyan(n_colors: int = 257, **kwargs) -> List[str]:
@@ -275,15 +276,15 @@
         n_colors: Number of colors to generate.
 
     Returns:
         A list of colors as hex codes.
 
     Note:
         Additional keyword arguments are passed on to
-        :obj:`ragraph.colors.cubehelix.cubehelix_palette`.
+        [`cubehelix_palette`][ragraph.colors.cubehelix.cubehelix_palette].
     """
     opts: Dict[str, Any] = dict(lower_hue=1.2, upper_hue=2.45, n_colors=n_colors)
     opts.update(kwargs)
     return get_diverging_hues(**opts)
 
 
 def get_diverging_purplegreen(n_colors: int = 257, **kwargs) -> List[str]:
@@ -293,15 +294,15 @@
         n_colors: Number of colors to generate.
 
     Returns:
         A list of colors as hex codes.
 
     Note:
         Additional keyword arguments are passed on to
-        :obj:`ragraph.colors.cubehelix.cubehelix_palette`.
+        [`cubehelix_palette`][ragraph.colors.cubehelix.cubehelix_palette].
     """
     opts: Dict[str, Any] = dict(lower_hue=0.15, upper_hue=1.8, n_colors=n_colors)
     opts.update(kwargs)
     return get_diverging_hues(**opts)
 
 
 def get_colormaps(
```

### Comparing `ragraph-1.19.0/ragraph/colors/cubehelix.py` & `ragraph-1.19.1/ragraph/colors/cubehelix.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-"""Cubehelix color palette support.
+"""# Cubehelix color palette
 
-Green, D. A. (2011). A colour scheme for the display of astronomical intensity images.
-Bull. Astr. Soc. India. Retrieved from http://www.astro.caltech.edu/
+Reference:
+    Green, D. A. (2011). A colour scheme for the display of astronomical intensity images.
+    Bull. Astr. Soc. India. Retrieved from
+    [http://www.astro.caltech.edu/](http://www.astro.caltech.edu/).
 """
 
 from typing import List, Optional
 
 from ragraph.colors import utils
 
 try:
@@ -31,27 +33,27 @@
 
     Arguments:
         n_colors: Number of RGB colour pairs to generate.
         start: Starting color (Red: 1.0, Green: 2.0, Blue: 3.0).
         end: Final color (Red: 1.0, Green: 2.0, Blue: 3.0).
         dark: Lightness of the darkest value [0.0 - 1.0].
         light: Lightness of the lightest value [0.0 - 1.0].
-        gamma: Exponential factor applied to lightness to emphasize low intensity
-            values (< 1.0) or high intensity values (> 1.0).
-        rotations: Number of RGB rotations (1.0 means a full RGB rotation). Overrides
-            :obj:`end`. Otherwise calculated as `(end - start) / 3`.
-        categorical: Whether to shuffle the rotational space optimally for categorical
-            color palettes. Similar colors are positioned as far apart as possible.
+        gamma: Exponential factor applied to lightness to emphasize low intensity values (< 1.0) or
+            high intensity values (> 1.0).
+        rotations: Number of RGB rotations (1.0 means a full RGB rotation). Overrides `end`.
+            Otherwise calculated as `(end - start) / 3`.
+        categorical: Whether to shuffle the rotational space optimally for categorical color
+            palettes. Similar colors are positioned as far apart as possible.
 
     Returns:
         Color palette as a list of hex codes.
 
     Reference:
-        Green, D. A. (2011). A colour scheme for the display of astronomical intensity
-        images. Bull. Astr. Soc. India. Retrieved from http://www.astro.caltech.edu/
+        Green, D. A. (2011). A colour scheme for the display of astronomical intensity images. Bull.
+        Astr. Soc. India. Retrieved from http://www.astro.caltech.edu/
     """
     if HAVE_NUMPY:
         method = _cubehelix_numpy
     else:
         method = _cubehelix_pure_python
 
     n_colors = max(n_colors, 1)
@@ -80,15 +82,15 @@
     dark: float = 0.2,
     light: float = 0.85,
     gamma: float = 1.0,
     saturation: float = 1.2,
     rotations: Optional[float] = None,
     categorical: bool = False,
 ) -> List[List[float]]:
-    """See :obj:`cubehelix_palette`."""
+    """See [`cubehelix_palette`][ragraph.colors.cubehelix.cubehelix_palette]."""
     n_colors = max(n_colors, 1)
 
     if rotations is None:
         rotations = (end - start) / 3
 
     start = start / 3
 
@@ -120,15 +122,15 @@
     dark: float = 0.2,
     light: float = 0.85,
     gamma: float = 1.0,
     saturation: float = 1.2,
     rotations: Optional[float] = None,
     categorical: bool = False,
 ) -> List[List[float]]:
-    """See :obj:`cubehelix_palette`."""
+    """See [`cubehelix_palette`][ragraph.colors.cubehelix.cubehelix_palette]."""
     import math
 
     if rotations is None:
         rotations = (end - start) / 3
 
     start = start / 3
```

### Comparing `ragraph-1.19.0/ragraph/colors/utils.py` & `ragraph-1.19.1/ragraph/colors/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Color utility methods."""
+"""# Color utilities"""
 from typing import Tuple
 
 
 def rgb1_to_rgb(r: float, g: float, b: float) -> Tuple[int, int, int]:
     """Convert [0.0-1.0] scaled RGB to [0-255]."""
     return round(r * 255), round(g * 255), round(b * 255)
```

### Comparing `ragraph-1.19.0/ragraph/datasets/__init__.py` & `ragraph-1.19.1/ragraph/datasets/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""Datasets module. Contains various graph datasets (see :obj:`enum()`, :obj:`get()`,
-and :obj:`info`).
-"""
+"""# RaGraph built-in datasets"""
 
 import importlib
 from pathlib import Path
 from typing import List
 
 from ragraph.graph import Graph
 from ragraph.io.csv import from_csv
```

### Comparing `ragraph-1.19.0/ragraph/datasets/aircraft_engine/__init__.py` & `ragraph-1.19.1/ragraph/datasets/aircraft_engine/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""Pratt & Whitney Aircraft Engine
+"""# Pratt & Whitney Aircraft Engine
 
-A directed graph describing the Pratt & Whitney PW4098 commercial high bypass-ratio
-turbofan engine. The graph describes a combination of the actual hardware dependencies
-of the engine and those of the development teams involved with them. It is a weighted
-and directed graph featuring 60 elements, four of which are sometimes left out as they
-represent the integration teams and no individual hardware components. Weak and strong
-dependencies are distinguished using weights of 1 and 2, respectively.
+A directed graph describing the Pratt & Whitney PW4098 commercial high bypass-ratio turbofan engine.
+The graph describes a combination of the actual hardware dependencies of the engine and those of the
+development teams involved with them. It is a weighted and directed graph featuring 60 elements,
+four of which are sometimes left out as they represent the integration teams and no individual
+hardware components. Weak and strong dependencies are distinguished using weights of 1 and 2,
+respectively.
 
 Reference:
-Rowles, C. M. (1999). System integration analysis of a large commercial aircraft engine.
+    Rowles, C. M. (1999). System integration analysis of a large commercial aircraft engine.
 """
 
 edge_weights = ["adjacency"]
```

### Comparing `ragraph-1.19.0/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv` & `ragraph-1.19.1/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/architecture_integral/__init__.py` & `ragraph-1.19.1/ragraph/datasets/architecture_integral/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-"""Graph describing a design problem using objects that need to be designed based on
+"""# Integral architecture example
+
+Graph describing a design problem using objects that need to be designed based on
 certain aspects. It is part of a set of three design problem graphs, each ideally solved
 with a different approach -- being a modular, **integral** or mixed architecture.
 
 This particular graph describes a design problem which is ideally solved using a
 **integral object architecture**. That the architecture consists vertically integrated
 modules. That is, each module in one domain integrates with only one (or very few) in
 the next and there is no crossover (mixing and matching across domains like with a
 modular approach). This means that interfaces between modules in different domains are
 relatively few. A module's design solution should be applicable to every member.
 
 Nodes are of kind "object" or "aspect_1", "aspect_2", and "aspect_3". The numbers
 represent different aspect domains. An "incidence" kind edge from an object to an aspect
-means that it posesses that aspect.
+means that it possesses that aspect.
 
-Authors: Tim Wilschut and Tiemen Schuijbroek, October 2019.
+Authors:
+    Tim Wilschut and Tiemen Schuijbroek, October 2019.
 """
```

### Comparing `ragraph-1.19.0/ragraph/datasets/architecture_integral/architecture_integral_edges.csv` & `ragraph-1.19.1/ragraph/datasets/architecture_integral/architecture_integral_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/architecture_mix/__init__.py` & `ragraph-1.19.1/ragraph/datasets/architecture_modular/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-"""Graph describing a design problem using objects that need to be designed based on
-certain aspects. It is part of a set of three design problem graphs, each ideally solved
-with a different approach -- being a modular, integral or **mixed architecture**.
+"""# Modular architecture example
 
-This particular graph describes a design problem which is ideally solved using a **mixed
-object architecture**. That means that the objects are best put into modules with some,
-but little interfaces across domains with limited crossover (mixing and matching like
-with a modular approach). Each module should be designed based on all aspects that the
-objects members posess combined, while taking into account the shared dependencies with
-other domains. A module's design solution should be applicable to every member.
+Graph describing a design problem using objects that need to be designed based on certain aspects.
+It is part of a set of three design problem graphs, each ideally solved with a different approach --
+being a **modular**, integral or mixed architecture.
 
-Nodes are of kind "object" or "aspect_1", "aspect_2", and "aspect_3". The numbers
-represent different aspect domains. An "incidence" kind edge from an object to an aspect
-means that it posesses that aspect.
+This particular graph describes a design problem which is ideally solved using a **modular object
+architecture**. That means that the objects are best put into modules. Modules on different aspect
+domains can then be mixed and matched so achieve a solution for it's combined members. Each module
+should be designed based on all aspects that the objects members posess combined, while taking into
+account the shared dependencies with other domains. A module's design solution should be applicable
+to every member.
 
-Authors: Tim Wilschut and Tiemen Schuijbroek, October 2019.
+Nodes are of kind "object" or "aspect_1", "aspect_2", and "aspect_3". The numbers represent
+different aspect domains. An "incidence" kind edge from an object to an aspect means that it
+posesses that aspect.
+
+Authors:
+    Tim Wilschut and Tiemen Schuijbroek, October 2019.
 """
```

### Comparing `ragraph-1.19.0/ragraph/datasets/architecture_mix/architecture_mix_edges.csv` & `ragraph-1.19.1/ragraph/datasets/architecture_mix/architecture_mix_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/architecture_modular/__init__.py` & `ragraph-1.19.1/ragraph/datasets/architecture_mix/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-"""Graph describing a design problem using objects that need to be designed based on
-certain aspects. It is part of a set of three design problem graphs, each ideally solved
-with a different approach -- being a **modular**, integral or mixed architecture.
+"""# Mixed architecture example
 
-This particular graph describes a design problem which is ideally solved using a
-**modular object architecture**. That means that the objects are best put into modules.
-Modules on different aspect domains can then be mixed and matched so achieve a solution
-for it's combined members. Each module should be designed based on all aspects that the
-objects members posess combined, while taking into account the shared dependencies with
-other domains. A module's design solution should be applicable to every member.
+Graph describing a design problem using objects that need to be designed based on certain aspects.
+It is part of a set of three design problem graphs, each ideally solved with a different approach --
+being a modular, integral or **mixed architecture**.
 
-Nodes are of kind "object" or "aspect_1", "aspect_2", and "aspect_3". The numbers
-represent different aspect domains. An "incidence" kind edge from an object to an aspect
-means that it posesses that aspect.
+This particular graph describes a design problem which is ideally solved using a **mixed object
+architecture**. That means that the objects are best put into modules with some, but little
+interfaces across domains with limited crossover (mixing and matching like with a modular approach).
+Each module should be designed based on all aspects that the objects members possess combined, while
+taking into account the shared dependencies with other domains. A module's design solution should be
+applicable to every member.
 
-Authors: Tim Wilschut and Tiemen Schuijbroek, October 2019.
+Nodes are of kind "object" or "aspect_1", "aspect_2", and "aspect_3". The numbers represent
+different aspect domains. An "incidence" kind edge from an object to an aspect means that it
+posesses that aspect.
+
+Authors:
+    Tim Wilschut and Tiemen Schuijbroek, October 2019.
 """
```

### Comparing `ragraph-1.19.0/ragraph/datasets/architecture_modular/architecture_modular_edges.csv` & `ragraph-1.19.1/ragraph/datasets/architecture_modular/architecture_modular_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/climate_control/climate_control_edges.csv` & `ragraph-1.19.1/ragraph/datasets/climate_control/climate_control_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/climate_control/climate_control_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/climate_control/climate_control_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv` & `ragraph-1.19.1/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/compatibility/compatibility_edges.csv` & `ragraph-1.19.1/ragraph/datasets/compatibility/compatibility_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/design/design_edges.csv` & `ragraph-1.19.1/ragraph/datasets/design/design_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/elevator175/__init__.py` & `ragraph-1.19.1/ragraph/datasets/elevator175/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-"""Elevator system decomposed into 175 components.
+"""# Elevator system decomposed into 175 components
 
-The Complex Elevator System is described using an undirected graph with multiple
-dependency types. It describes a machine-room-less elevator called the 'Kone MonoSpace'.
-It is designed for low- to midrise buildings and uses permanent-magnet electric motors.
-The five defined edge types are spatial, material, mechanical energy, electrical energy
-and information. It was published in a variation of 175 elements and a less granular
-variation of 45 elements. The less granular variation collapses a set of pre-defined
-modules and therefore contains less detail of the system.
+The Complex Elevator System is described using an undirected graph with multiple dependency types.
+It describes a machine-room-less elevator called the 'Kone MonoSpace'. It is designed for low- to
+midrise buildings and uses permanent-magnet electric motors. The five defined edge types are
+spatial, material, mechanical energy, electrical energy and information. It was published in a
+variation of 175 elements and a less granular variation of 45 elements. The less granular variation
+collapses a set of pre-defined modules and therefore contains less detail of the system.
 
 Reference:
-Niutanen, V., Hölttä-otto, K., Rahardjo, A., & Stowe, H. M. (2017). Complex Elevator
-System DSM - Case for a DSM Design Sprint. In 19th International dependency and
-structure modeling conference, DSM 2017.
+    Niutanen, V., Hölttä-otto, K., Rahardjo, A., & Stowe, H. M. (2017). Complex Elevator System DSM
+    - Case for a DSM Design Sprint. In 19th International dependency and structure modeling
+    conference, DSM 2017.
 """
 
 edge_weights = [
     "spatial",
     "material",
     "information",
     "mechanical energy",
```

### Comparing `ragraph-1.19.0/ragraph/datasets/elevator175/elevator175_edges.csv` & `ragraph-1.19.1/ragraph/datasets/elevator175/elevator175_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/elevator175/elevator175_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/elevator175/elevator175_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/elevator45/__init__.py` & `ragraph-1.19.1/ragraph/datasets/elevator45/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-"""Elevator system decomposed into 45 components.
+"""# Elevator system decomposed into 45 components
 
-The Complex Elevator System is described using an undirected graph with multiple
-dependency types. It describes a machine-room-less elevator called the 'Kone MonoSpace'.
-It is designed for low- to midrise buildings and uses permanent-magnet electric motors.
-The five defined edge types are spatial, material, mechanical energy, electrical energy
-and information. It was published in a variation of 175 elements and a less granular
-variation of 45 elements. The less granular variation collapses a set of pre-defined
-modules and therefore contains less detail of the system.
+The Complex Elevator System is described using an undirected graph with multiple dependency types.
+It describes a machine-room-less elevator called the 'Kone MonoSpace'. It is designed for low- to
+midrise buildings and uses permanent-magnet electric motors. The five defined edge types are
+spatial, material, mechanical energy, electrical energy and information. It was published in a
+variation of 175 elements and a less granular variation of 45 elements. The less granular variation
+collapses a set of pre-defined modules and therefore contains less detail of the system.
 
 Reference:
-Niutanen, V., Hölttä-otto, K., Rahardjo, A., & Stowe, H. M. (2017). Complex Elevator
-System DSM - Case for a DSM Design Sprint. In 19th International dependency and
-structure modeling conference, DSM 2017.
+    Niutanen, V., Hölttä-otto, K., Rahardjo, A., & Stowe, H. M. (2017). Complex Elevator System DSM
+    - Case for a DSM Design Sprint. In 19th International dependency and structure modeling
+    conference, DSM 2017.
 """
 
 edge_weights = [
     "spatial",
     "material",
     "information",
     "mechanical energy",
```

### Comparing `ragraph-1.19.0/ragraph/datasets/elevator45/elevator45_edges.csv` & `ragraph-1.19.1/ragraph/datasets/elevator45/elevator45_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/elevator45/elevator45_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/elevator45/elevator45_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/esl/__init__.py` & `ragraph-1.19.1/ragraph/datasets/esl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""# Elephant Specification Language datasets"""
 import importlib
 from pathlib import Path
 from typing import List
 
 HERE = Path(__file__).parent
```

### Comparing `ragraph-1.19.0/ragraph/datasets/esl/pump/pump.esl` & `ragraph-1.19.1/ragraph/datasets/esl/pump/pump.esl`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/ford_hood/__init__.py` & `ragraph-1.19.1/ragraph/datasets/ford_hood/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 """Ford Motor Company Hood Development Process.
 
-This DSM application was made to test the effectiveness of a DSM analysis to improve a
-highly developed iterative design process in terms of:
+This DSM application was made to test the effectiveness of a DSM analysis to improve a highly
+developed iterative design process in terms of:
 
 - Reduction of product development lead time
 - Reduction of product development lead-time variation
 
-
-As it is a process DSM, the nodes represent tasks in the design process. The edges
-represent dependencies between them. Each task in the design process was assigned a task
-volatility value, which is an indication of the probability of rework.
-
+As it is a process DSM, the nodes represent tasks in the design process. The edges represent
+dependencies between them. Each task in the design process was assigned a task volatility value,
+which is an indication of the probability of rework.
 
 Node (task) weights:
 
 - EC(i) and EC(r) represent the initial and rework costs
 - ED(i) and ED(r) represent the initial and rework durations
 - Information variability (likelihood of input changing)
 
 
 Edge weights:
 
-- volatility: an indication of the probability of rework when the dependent task is
-  executed without properly waiting for its input to finish. It's value was determined
-  using the information variability of the source (depended on) task and the sensitivity
-  of the target (dependent) task.
-
-
-References:
-Browning, Tyson R., and Steven D. Eppinger. 2002, November. Modeling Impacts of Process
-Architecture on Cost and Schedule Risk in Product Development. IEEE Transactions on
-Engineering Management 49 (4):428-442.
-Krishnan, Viswanathan, Steven D. Eppinger, and Daniel E. Whitney. 1997, April.
-A Model-Based Framework to Overlap Product Development Activities.
-Management Science 43 (4):437-451.
-Yassine, Ali A., Daniel E. Whitney, and Tony P. Zambito. 2001. Assessment of Rework
-Probabilities for Simulating Product Development Processes Using the Design Structure
-Matrix (DSM). ASME Design Engineering Technical Conferences, DTM-21693.
+- volatility: an indication of the probability of rework when the dependent task is executed without
+  properly waiting for its input to finish. It's value was determined using the information
+  variability of the source (depended on) task and the sensitivity of the target (dependent) task.
+
+Reference:
+    Browning, Tyson R., and Steven D. Eppinger. 2002, November. Modeling Impacts of Process
+    Architecture on Cost and Schedule Risk in Product Development. IEEE Transactions on Engineering
+    Management 49 (4):428-442.
+
+Reference:
+    Krishnan, Viswanathan, Steven D. Eppinger, and Daniel E. Whitney. 1997, April. A Model-Based
+    Framework to Overlap Product Development Activities. Management Science 43 (4):437-451.
+
+Reference:
+    Yassine, Ali A., Daniel E. Whitney, and Tony P. Zambito. 2001. Assessment of Rework
+    Probabilities for Simulating Product Development Processes Using the Design Structure Matrix
+    (DSM). ASME Design Engineering Technical Conferences, DTM-21693.
 """
 
 
 node_weights = [
     "EC(i) ($000)",
     "EC(r) ($000)",
     "ED(i) (days)",
```

### Comparing `ragraph-1.19.0/ragraph/datasets/ford_hood/ford_hood_edges.csv` & `ragraph-1.19.1/ragraph/datasets/ford_hood/ford_hood_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/ford_hood/ford_hood_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/ford_hood/ford_hood_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/kodak3d/__init__.py` & `ragraph-1.19.1/ragraph/datasets/kodak3d/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Kodak Single-Use Camera product commonality dataset.
+"""# Kodak Single-Use Camera product commonality
 
 This DSM dataset was actually proposed as a "3D DSM" as it was featured in the reference
 papers in a 3D layered fashion. Relationships between components in a product family for
 different family members were shown in a 3D layered fashion. Common interfaces and
 unique interfaces were color coded accordingly for three family members: The "Fun
 Saver", "Outdoor", and "Plus Digital" single-use cameras.
 
@@ -12,22 +12,24 @@
 
 Edges indicate an interface between components, which is therefore modeled using an
 "adjacency" edge weight. Once again, they are labeled with the camera typename when that
 dependency occurs in the corresponding camera type.
 
 Available labels for nodes or edges:
 
-    - Fun Saver
-    - Outdoor
-    - Plus Digital
-
-References:
-Alizon, Fabrice. 2009, February. Module-Based Design Management-Synerg'. Symposium on
-Product Family & Product Platform Design, Helsinki University of Technology (TKK),
-Helsinki, Finland.
-Alizon, Fabrice, Seung K. Moon, Steven B. Shooter, and Timothy W. Simpson. 2007,
-September 4--7. Three Dimensional Design Structure Matrix-DSM3D. ASME Design Engineering
-Technical Conferences, DETCZ007-34510, Las Vegas, NV, pp. 941-948.
+- Fun Saver
+- Outdoor
+- Plus Digital
+
+Reference:
+    Alizon, Fabrice. 2009, February. Module-Based Design Management-Synerg'. Symposium on
+    Product Family & Product Platform Design, Helsinki University of Technology (TKK),
+    Helsinki, Finland.
+
+Reference:
+    Alizon, Fabrice, Seung K. Moon, Steven B. Shooter, and Timothy W. Simpson. 2007,
+    September 4--7. Three Dimensional Design Structure Matrix-DSM3D. ASME Design Engineering
+    Technical Conferences, DETCZ007-34510, Las Vegas, NV, pp. 941-948.
 """
 
 
 edge_weights = ["adjacency"]
```

### Comparing `ragraph-1.19.0/ragraph/datasets/kodak3d/kodak3d_edges.csv` & `ragraph-1.19.1/ragraph/datasets/kodak3d/kodak3d_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/kodak3d/kodak3d_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/kodak3d/kodak3d_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/ledsip/ledsip_edges.csv` & `ragraph-1.19.1/ragraph/datasets/ledsip/ledsip_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/ledsip/ledsip_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/ledsip/ledsip_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/localbus/localbus_edges.csv` & `ragraph-1.19.1/ragraph/datasets/localbus/localbus_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_edges.csv` & `ragraph-1.19.1/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_edges.csv` & `ragraph-1.19.1/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_edges.csv` & `ragraph-1.19.1/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_edges.csv` & `ragraph-1.19.1/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_edges.csv` & `ragraph-1.19.1/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_edges.csv` & `ragraph-1.19.1/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/pathfinder/__init__.py` & `ragraph-1.19.1/ragraph/datasets/pathfinder/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-"""NASA Mars Pathfinder Technology Risk DSM.
+"""# NASA Mars Pathfinder Technology Risk DSM
 
 The technology risk DSM (TR-DSM) helps to identify where most of the design effort
 should go if one wants to mitigate technological failures and improve robustness of a
 system. All components of a system are assigned with a technology risk factor,
 which indicates the probability of failure, unprovenness, or uncertainty in design.
 The technology risk factor at NASA is loosely defined as the inverse of the technology
 readiness level:
 
-
-+-----+--------------------------------------------------------------------------------------+-----+
-| TRF | NASA TRL Definition                                                                  | TRL |
-+=====+======================================================================================+=====+
+| TRF | NASA Technology Readiness Level Definition                                           | TRL |
+|-----|--------------------------------------------------------------------------------------|-----|
 |  1  | Actual system "flight proven" through successful mission operations                  |  9  |
-+-----+--------------------------------------------------------------------------------------+-----+
 |  2  | Actual system completed and "flight qualified" through test and demonstration        |  8  |
-+-----+--------------------------------------------------------------------------------------+-----+
 |  2  | System prototype in a space environment                                              |  7  |
-+-----+--------------------------------------------------------------------------------------+-----+
 |  3  | System/subsystem model or prototype demonstration in a relevant environment          |  6  |
-+-----+--------------------------------------------------------------------------------------+-----+
 |  4  | Component and/or breadboard validation in relevant environment                       |  5  |
-+-----+--------------------------------------------------------------------------------------+-----+
 |  4  | Component and/or breadboard validation in laboratory environment                     |  4  |
-+-----+--------------------------------------------------------------------------------------+-----+
 |  5  | Analytical and experimental critical function and/or characteristic proof-of-concept |  3  |
-+-----+--------------------------------------------------------------------------------------+-----+
 |  5  | Technology concept and/or application formulated                                     |  2  |
-+-----+--------------------------------------------------------------------------------------+-----+
 |  5  | Basic principles observed and reported                                               |  1  |
-+-----+--------------------------------------------------------------------------------------+-----+
 
 
 The dataset includes both an adjacency value as if the DSM were a regular product DSM
 with interface strength values and the technology risk value which is computed using:
 
     TR = TRF-source * TRF-target * adjacency
 
 Reference:
     Brady, Timothy K. 2002. Utilization of Dependency Structure Matrix Analysis to
     Assess Complex Project Designs. Proceedings of ASME Design Engineering Technical
     Conferences, no. DETCZ002/DTM-34031, Montreal, Canada.
-"""  # noqa
+"""
 
 node_weights = ["technology risk factor"]
 edge_weights = ["adjacency", "technology risk"]
```

### Comparing `ragraph-1.19.0/ragraph/datasets/pathfinder/pathfinder_edges.csv` & `ragraph-1.19.1/ragraph/datasets/pathfinder/pathfinder_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/pathfinder/pathfinder_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/pathfinder/pathfinder_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/similarity/similarity_edges.csv` & `ragraph-1.19.1/ragraph/datasets/similarity/similarity_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/ucav/__init__.py` & `ragraph-1.19.1/ragraph/datasets/ucav/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""UCAV (unmanned combat aerial vehicle) preliminary design process graph.
+"""# UCAV (unmanned combat aerial vehicle) preliminary design process.
 
 The graph contains 14 preliminary design activities. Each phase consists of an initial
 activity to define design several disciplines-such as aerodynamics, propulsion,
 stability and control (S&C), distribute a design configuration (a design concept
 proposed to satisfy the DR&O). Then, requirements and objectives (DR&O), followed by a
 couple of activities to create and mechanical and electrical, weights, and performance -
 each evaluate the configuration from their own perspective.
@@ -13,16 +13,16 @@
 probability and rework impact annotations.
 
 When an activity is performed before all activities with edges to that activity has been
 succesfully executed, there is a rework probability that the activity needs to be
 redone, the impact then indicates the percentage that needs to be redone and the
 improvement curve decreases this in successive iterations.
 
-Reference: Eppinger, S. D., & Browning, T. R. (2012). Design Structure Matrix - Methods
-and Applications.
+Reference:
+    Eppinger, S. D., & Browning, T. R. (2012). Design Structure Matrix - Methods and Applications.
 """
 
 node_weights = [
     "min_duration",
     "mean_duration",
     "max_duration",
     "min_cost",
```

### Comparing `ragraph-1.19.0/ragraph/datasets/ucav/ucav_edges.csv` & `ragraph-1.19.1/ragraph/datasets/ucav/ucav_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/datasets/ucav/ucav_nodes.csv` & `ragraph-1.19.1/ragraph/datasets/ucav/ucav_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/edge.py` & `ragraph-1.19.1/ragraph/edge.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Edge module. Contains Edge class definitions."""
+"""# Edge class module"""
 
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
 
 from ragraph.generic import Annotations, Metadata
 from ragraph.node import Node
 
 
 class Edge(Metadata):
-    """Edge between a source :obj:`Node` and a target :obj:`Node`.
+    """Edge between a source [`Node`][ragraph.node.Node] and a target [`Node`][ragraph.node.Node].
 
     Arguments:
-        source: Source :obj:`Node` of this edge.
-        target: Target :obj:`Node` of this edge.
+        source: Source [`Node`][ragraph.node.Node] of this edge.
+        target: Target [`Node`][ragraph.node.Node] of this edge.
         name: Instance name. Given a UUID if none provided.
         kind: Kind or main category of this instance.
         labels: Labels categorizing this instance.
         weights: Dictionary of weights attached to this instance.
         annotations: Miscellaneous properties of this instance.
         uuid: Fixed UUID if desired, generated when left set to None.
     """
```

### Comparing `ragraph-1.19.0/ragraph/generic.py` & `ragraph-1.19.1/ragraph/generic.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,32 +11,33 @@
 
 
 class MappingValidationError(Exception):
     pass
 
 
 def field(fget: Callable):
-    """A :obj:`Mapping` field is a property that utilizes the :obj:`Mapping`'s data.
+    """A [`Mapping`][ragraph.generic.Mapping] `field` is a property that utilizes the
+    [`Mapping`][ragraph.generic.Mapping]'s data.
 
     Use it like the ``@property`` decorator and leave the function body blank (or pass):
 
     By inspecting the wrapped method's name we derive the property's key.
 
-    Getting data from the mapping is done by retrieving the key from the set values.
-    If that key is not found, an attempt is made on the defaults.
-    An error is thrown when the key is neither to be found in the data or defaults.
-
-    Setting data checks for nested :obj:`Mapping` keys to update those and otherwise
-    defaults to simply storing the value. Updating a nested :obj:`Mapping` field only
-    updates the keys that are provided.
+    Getting data from the mapping is done by retrieving the key from the set values. If that key is
+    not found, an attempt is made on the defaults. An error is thrown when the key is neither to be
+    found in the data or defaults.
+
+    Setting data checks for nested [`Mapping`][ragraph.generic.Mapping] keys to update those and
+    otherwise defaults to simply storing the value. Updating a nested
+    [`Mapping`][ragraph.generic.Mapping] field only updates the keys that are provided.
 
     Deleting data pops the key from the set values, but does not remove any defaults.
 
     Note:
-        The method contents of a :obj:`Mapping` :obj:`field` are ignored.
+        The method contents of a [`Mapping`][ragraph.generic.Mapping] `field` are ignored.
     """
     key = fget.__name__
 
     def getter(self):
         """Get a mapping value."""
         if key in self._data:
             return self._data[key]
@@ -77,47 +78,50 @@
 
 class Mapping:
     """A dictionary like object that with property-based access fields.
 
     It's possible to include allowed keys, default values, and optional validators for
     certain keys/properties of a derived class.
 
-    .. doctest::
-
-        >>> from ragraph.generic import Mapping, field
-        >>> def check_int(value):
-        ...     assert value == 1
-        ...
-        >>> class MyMap(Mapping):
-        ...     _protected = True
-        ...     _defaults = dict(myfield=1)
-        ...     _validators = dict(myfield=check_int)
-        ...     @field
-        ...     def myfield(self) -> int:
-        ...         '''My field's docstring'''
-        ...
-        >>> m = MyMap(myfield=3)
-        >>> assert m.myfield == 3,            "This should return our set value."
-        >>> assert m.myfield == m['myfield'], "A mapping works like a dictionary."
-        >>> del(m.myfield)                   # This deletes our override.
-        >>> m.validate()                     # Checks whether myfield == 1.
+    ```py
+    from ragraph.generic import Mapping, field
+    def check_int(value):
+        assert value == 1
+
+    class MyMap(Mapping):
+        _protected = True
+        _defaults = dict(myfield=1)
+        _validators = dict(myfield=check_int)
+        @field
+        def myfield(self) -> int:
+            '''My field's docstring'''
+
+    m = MyMap(myfield=3)
+    assert m.myfield == 3,            "This should return our set value."
+    assert m.myfield == m['myfield'], "A mapping works like a dictionary."
+    del(m.myfield)                    # This deletes our override.
+    m.validate()                      # Checks whether myfield == 1.
+    ```
     """
 
     _protected = False
-    """Setting public properties is restricted to those in :obj:`self.keys`."""
+    """Setting public properties is restricted to those in
+    [`self.keys`][ragraph.generic.Mapping.keys].
+    """
 
     _defaults: Dict[str, Any] = dict()
     """Default values for included keys."""
 
     _keys: Optional[Set[str]] = None
     """Set of always allowed keys to set."""
 
     _validators: Dict[str, Callable] = dict()
-    """Validators for included keys. Used when calling :obj:`self.validate`.
-    Also see :obj:`self._post_validation`."""
+    """Validators for included keys. Used when calling
+    [`self.validate`][ragraph.generic.Mapping.validate].
+    Also see [`self._post_validation`][ragraph.generic.Mapping._post_validation]."""
 
     def __init__(self, *args, **kwargs):
         # The internal storage dictionary.
         self._data: Dict[str, Any] = dict()
 
         # Update the mapping with args and kwargs.
         self.update(*args, **kwargs)
@@ -145,15 +149,14 @@
         """Get an attribute with a fallback value if it isn't found."""
         return getattr(self, key, fallback)
 
     def __setattr__(self, key: str, value: Any) -> None:
         """Set an attribute : `self.key = value`.
 
         Private properties are left untouched, public properties need permission.
-        See :obj:`self._check_allowed`.
         """
         if not key.startswith("_"):
             keys = set() if self._keys is None else self._keys
             keys = keys.union(self.keys())
             if key not in keys:
                 if self._protected:
                     raise KeyError(f"Key or property '{key}' is not allowed. Only '{keys}'.")
@@ -168,19 +171,18 @@
 
         super().__setattr__(key, value)
 
     def __setitem__(self, key: str, value: Any) -> None:
         """Set an attribute via a dictionary accessor: `self['key'] = value`.
 
         Private properties are left untouched, public properties need permission.
-        See :obj:`self._check_allowed`.
         """
         setattr(self, key, value)
 
-    def update(self, *args, **kwargs) -> None:
+    def update(self, *args: Dict[str, Any], **kwargs: Any) -> None:
         """Update multiple keys at once.
 
         Arguments:
             args: Dictionaries of key value pairs to update the set data with.
             kwargs: Keyword arguments to update the set data with.
         """
         for arg in args:
@@ -243,15 +245,15 @@
 
         Useful when a derived class needs to cross-validate certain keys instead of just
         a dedicated method per key.
         """
         pass
 
     def as_dict(self) -> Dict[str, Any]:
-        """Return a copy as a dictionary with all submappings as dictionaries, too."""
+        """Return a copy as a dictionary with all sub-mappings as dictionaries, too."""
         m = self._defaults.copy()
         m.update(self._data)
         for key, value in m.items():
             if isinstance(value, Mapping):
                 m[key] = value.as_dict()
         return deepcopy(m)
 
@@ -264,15 +266,15 @@
 
 class Bound:
     """Numerical lower or upper bound for a value. Use with comparison operators.
 
     Arguments:
         value: Numerical bound value.
         inclusive: Whether the bound is inclusive.
-        report: Whether to report an "error", "warn" or nothing (``None``) on
+        report: Whether to report an "error", "warn" or nothing (`None`) on
             bound violations.
     """
 
     def __init__(
         self,
         value: Union[int, float],
         inclusive: bool = True,
@@ -365,20 +367,20 @@
         )
 
 
 class Metadata:
     """Metadata for graph elements.
 
     Arguments:
-        name: Instance name. Set to a copy of the UUID if :obj:`None` provided.
+        name: Instance name. Set to a copy of the UUID if `None` provided.
         kind: Kind or main category of this instance.
         labels: Labels categorizing this instance.
         weights: Dictionary of weights attached to this instance.
         annotations: Miscellaneous properties of this instance.
-        uuid: UUID of this instance, generated when :obj:`None` provided.
+        uuid: UUID of this instance, generated when `None` provided.
     """
 
     def __init__(
         self,
         name: Optional[str] = None,
         kind: Optional[str] = None,
         labels: Optional[List[str]] = None,
@@ -478,23 +480,23 @@
         else:
             self._weights = dict(value)
 
     @property
     def weight(self) -> Union[int, float]:
         """Cumulative weight of this instance (read-only).
 
-        Returns the sum of :obj:`self.weights`.
+        Returns the sum of [`self.weights`][ragraph.generic.Metadata.weights].
         """
         return sum(self._weights.values())
 
     @property
     def annotations(self) -> Annotations:
         """Annotations of this instance.
 
-        Defaults to an empty :obj:`Annotations` instance.
+        Defaults to an empty [`Annotations`][ragraph.generic.Annotations] instance.
         """
         return self._annotations
 
     @annotations.setter
     def annotations(self, value: Optional[Union[Annotations, Dict[str, Any]]]):
         if value is None:
             self._annotations = Annotations()
@@ -661,15 +663,15 @@
         self.labels = labels
         self.weights = weights
         self.weight_domains = weight_domains
         self.annotations = annotations
 
     def as_dict(self) -> Dict[str, Any]:
         """Serializable dictionary representation."""
-        result = dict(
+        result: Dict[str, Any] = dict(
             kinds=sorted(self.kinds),
             labels=sorted(self.labels),
             weights=sorted(self.weights),
             weight_domains={k: v.as_dict() for k, v in self.weight_domains.items()},
             annotations=sorted(self.annotations),
         )
         if self.uuids is not None:
```

### Comparing `ragraph-1.19.0/ragraph/graph.py` & `ragraph-1.19.1/ragraph/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""Graph module. Contains Graph class definitions.
+"""# Graph class module
 
-The :obj:`Graph` class is the core of this package. It is the internal storage
+The [`Graph`][ragraph.graph.Graph] class is the core of this package. It is the internal storage
 format that facilitates all conversions. These class definitions are designed to
 accommodate a wide range of graph formats.
 """
 from collections import OrderedDict, defaultdict
 from copy import deepcopy
 from typing import (
     Any,
@@ -33,15 +33,16 @@
 
 
 class ConsistencyError(Exception):
     pass
 
 
 class Graph(Metadata):
-    """Graph of :obj:`Node` objects and :obj:`Edge` objects between them.
+    """Graph of [`Node`][ragraph.node.Node] objects and [`Edge`][ragraph.edge.Edge] objects between
+    them.
 
     Arguments:
         nodes: Iterable of graph nodes.
         edges: Iterable of graph edges.
         add_parents: Recursively add parent nodes of the provided nodes.
         add_children: Recursively add child nodes of the provided nodes.
         name: Instance name. Given a UUID if none provided.
@@ -311,16 +312,15 @@
     def add_edge(self, edge: Edge):
         """Add a new edge to the graph. Source and target need to exist in the graph.
 
         Arguments:
             edge: Edge to add.
 
         Raises:
-            A ValueError if the source or target doesn't exist or the edge instance
-            already does.
+            ValueError: if the source or target doesn't exist or the edge instance already does.
         """
         source = edge.source.name
         target = edge.target.name
         if source not in self.node_dict:
             raise ValueError("Source node %r does not exist in graph." % edge.source)
         if target not in self.node_dict:
             raise ValueError("Target node %r does not exist in graph." % edge.target)
@@ -464,16 +464,16 @@
         target: Union[str, Node],
         inherit: bool = False,
         loops: bool = True,
     ) -> Generator[Edge, None, None]:
         """Yield edges between source and target node.
 
         Arguments:
-            sources: Source nodes.
-            targets: Target nodes.
+            source: Source node.
+            target: Target node.
             inherit: Whether to include edges between descendants of given nodes.
             loops: Whether to include self-loop edges.
         """
         if source == target and not loops:
             return
         source_node = source if isinstance(source, Node) else self._nodes[source]
         target_node = target if isinstance(target, Node) else self._nodes[target]
@@ -558,15 +558,15 @@
             edge_kinds: The kind of edges to be selected.
             depth: The maximum depth of node to be selected.
             selection_mode: The selection mode. Either 'dependent' or 'independent'.
 
         Note:
             The selection mode argument determines how nodes of different kinds are
             selected. If the selection mode is set to 'dependent', the first node kind
-            in the :obj:`node_kinds` list is considered to be the 'lead node kind'.
+            in the `node_kinds` list is considered to be the 'lead node kind'.
             Nodes of different kind than the lead node kind, are only selected if they
             have a dependency with at least one of the selected nodes of the lead node
             kind. If the selection mode is set to 'independent' this dependency
             condition is dropped.
         """
         nkinds = node_kinds or self.node_kinds
         ekinds = edge_kinds or self.edge_kinds
@@ -605,15 +605,15 @@
             edge_kinds: The kind of edges to be selected.
             depth: The maximum depth of node to be selected.
             selection_mode: The selection mode. Either 'dependent' or 'independent'.
 
         Note:
             The selection mode argument determines how nodes of different kinds are
             selected. If the selection mode is set to 'dependent', the first node kind
-            in the :obj:`node_kinds` list is considered to be the 'lead node kind'.
+            in the `node_kinds` list is considered to be the 'lead node kind'.
             Nodes of different kind than the lead node kind, are only selected if they
             have a dependency with at least one of the selected nodes of the lead node
             kind. If the selection mode is set to 'independent' this dependency
             condition is dropped.
         """
 
         nodes = self.get_node_selection(
@@ -656,15 +656,15 @@
     ) -> Union["np.ndarray", List[List[float]]]:
         """Convert graph data into a numerical adjacency matrix.
 
         Arguments:
             nodes: Optional list of nodes for which to get the adjacency matrix.
             inherit: Whether to count weights between children of the given nodes.
             loops: Whether to calculate self-loops from a node to itself.
-            only: Optional subset of edge weights to consider. See :obj:`Edge` for
+            only: Optional subset of edge weights to consider. See [`Edge`][ragraph.edge.Edge] for
                 default edge weight implementation.
 
         Returns:
             Adjacency matrix as a 2D numpy array if numpy is present. Otherwise it will
             return a 2D nested list.
         """
         from ragraph.io.matrix import to_matrix
@@ -678,20 +678,19 @@
         inherit: bool = False,
         loops: bool = False,
         only: Optional[List[str]] = None,
     ) -> Union["np.ndarray", List[List[float]]]:
         """Convert graph data into a numerical mapping matrix.
 
         Arguments:
-            graph: Graph to fetch data from.
             rows: Nodes representing the matrix rows.
             cols: Nodes representing the matrix columns if different from the rows.
             inherit: Whether to count weights between children of the given nodes.
             loops: Whether to calculate self-loops from a node to itself.
-            only: Optional subset of edge weights to consider. See :obj:`Edge` for
+            only: Optional subset of edge weights to consider. See [`Edge`][ragraph.edge.Edge] for
                 default edge weight implementation.
 
         Returns:
             Adjacency matrix as a 2D numpy array if numpy is present. Otherwise it will
             return a 2D nested list.
         """
         from ragraph.io.matrix import to_matrix
@@ -699,15 +698,15 @@
         return to_matrix(self, rows=rows, cols=cols, inherit=inherit, loops=loops, only=only)
 
     def get_ascii_art(
         self,
         nodes: Optional[List[Node]] = None,
         edge: str = "X",
         diag: str = "\u25A0",
-        show: bool = True,
+        show: bool = False,
     ) -> Optional[str]:
         """Get a unicode ASCII art representation of a binary adjacency matrix for a
         given set of nodes.
 
         Arguments:
             nodes: Nodes to include in the art.
             edge: Mark to use when there's an edge between nodes. (X by default)
@@ -804,15 +803,15 @@
 
         Arguments:
             raise_error: Whether to raise an error instead of returning a bool.
 
         Returns:
             Whether nodes aren't their own ancestor/descendant and if all their children
             and parents exist in the graph. Raises an error for inconsistencies if
-            :obj:`raise_error` is set to `True`.
+            `raise_error` is set to `True`.
         """
         consistent = True
 
         try:
             for node in self.node_list:
                 a = node
                 while a.parent:
@@ -859,20 +858,21 @@
             if raise_error:
                 raise e
 
         return consistent
 
 
 class GraphView(Graph):
-    """A view on a :obj:`Graph` object. It works exactly like the :obj:`Graph` object,
-    except for that the nodes and edges are filtered according to the view function.
+    """A view on a [`Graph`][ragraph.graph.Graph] object. It works exactly like the
+    [`Graph`][ragraph.graph.Graph] object, except for that the nodes and edges are filtered
+    according to the view function.
 
     Arguments:
         graph: Graph to provide a view on.
-        view_func: View function that filters the :obj:`Graph`'s nodes and edges.
+        view_func: View function that filters the [`Graph`][ragraph.graph.Graph]'s nodes and edges.
         view_kwargs: Optional arguments to pass to the view function.
     """
 
     def __init__(
         self,
         graph: Graph,
         view_func: Optional[
@@ -924,15 +924,15 @@
             [Any],
             Tuple[
                 Union[Iterable[Node], Dict[str, Node]],
                 Union[Iterable[Edge], Dict[str, Edge]],
             ],
         ]
     ]:
-        """View function that filters the :obj:`Graph`'s nodes and edges."""
+        """View function that filters the [`Graph`][ragraph.graph.Graph]'s nodes and edges."""
         return self._view_func
 
     @view_func.setter
     def view_func(
         self,
         value: Optional[
             Callable[
```

### Comparing `ragraph-1.19.0/ragraph/io/archimate/__init__.py` & `ragraph-1.19.1/ragraph/io/archimate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 import shutil
 from pathlib import Path
 from typing import Any, Dict, Generator, Optional, Union
 
 from lxml import etree
 from lxml.builder import ElementMaker
+
 from ragraph.edge import Edge
 from ragraph.graph import Graph
 from ragraph.io.xml import _get_xmi_id
 from ragraph.node import Node
 
 here = Path(__file__).parent
 schema_doc = etree.parse(str(here / "archimate3_Model.xsd"))
@@ -288,24 +289,25 @@
 ) -> str:
     """Encode Graph to an Archimate model XML element.
 
     Arguments:
         graph: Graph to convert to XML.
         path: Optional file path to write XML to.
         elem: Optional object to append the Graph to.
-        tostring_args: Optional argument overrides to :obj:`lxml.etree.tostring()`.
+        tostring_args: Optional argument overrides to
+            [`lxml.etree.tostring`][lxml.etree.tostring].
         bundle_schemas: When exporting to a file, bundle the .xsd schemas.
 
     Returns:
         XML element.
 
     Note:
         For both nodes and edges we use the following:
-        The annotations.archimate["type"] determines the type (and therefore layer).
-        The annotations.archimate["documentation"] populates the documentation field.
+        The `annotations.archimate["type"]` determines the type (and therefore layer).
+        The `annotations.archimate["documentation"]` populates the documentation field.
         Refer to https://www.opengroup.org/xsd/archimate/ and the XSD scheme for all
         possible XML element types.
     """
     if elem is None:
         parser = etree.XMLParser(remove_blank_text=True)
         doc = etree.parse(str(here / "bare.xml"), parser)
         root = doc.getroot()
```

### Comparing `ragraph-1.19.0/ragraph/io/archimate/archimate3_Model.xsd` & `ragraph-1.19.1/ragraph/io/archimate/archimate3_Model.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/io/archimate/xml.xsd` & `ragraph-1.19.1/ragraph/io/archimate/xml.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/io/canopy.py` & `ragraph-1.19.1/ragraph/io/canopy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Canopy by Ratio CASE format support."""
+"""# Canopy by Ratio CASE format support"""
 
 import json
 import re
 from pathlib import Path
 from typing import Any, Dict, Generator, List, Optional, Union
 from uuid import UUID
 
@@ -28,15 +28,15 @@
         path: Path of the file to load.
 
     Returns:
         Graph objects contained in Canopy data formats being either a graph, tab,
         session, or workspace export of Canopy.
 
     Raises:
-        InconsistencyError if graph is inconsistent.
+        InconsistencyError: if graph is inconsistent.
     """
     data = json.loads(Path(path).read_text())
     schema = _match_schema(data.get("$schema", ""))
     if schema == "workspace":
         graphs = list(_decode_workspace(data))
     elif schema == "session":
         graphs = list(_decode_session(data))
```

### Comparing `ragraph-1.19.0/ragraph/io/csv.py` & `ragraph-1.19.1/ragraph/io/csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""CSV format support."""
+"""# CSV format support"""
 
 import csv
 import warnings
 from collections import OrderedDict
 from pathlib import Path
-from typing import Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from ragraph.generic import Annotations
 from ragraph.graph import Edge, Graph, Node
 
 NODE_COLUMNS = ["name", "uuid", "kind", "labels", "parent", "children", "is_bus"]
 EDGE_COLUMNS = ["source", "target", "name", "uuid", "kind", "labels"]
 
@@ -16,16 +16,16 @@
 def from_csv(
     nodes_path: Optional[Union[str, Path]] = None,
     edges_path: Optional[Union[str, Path]] = None,
     csv_delimiter: str = ";",
     iter_delimiter: str = ";",
     node_weights: Optional[List[str]] = None,
     edge_weights: Optional[List[str]] = None,
-    **graph_kwargs,
-):
+    **graph_kwargs: Any,
+) -> Graph:
     """Convert CSV files to a graph.
 
     Nodes file (optional) requires at least a `name` column. Optional special
     property columns are `kind`, `labels`, `parent`, `children` and `is_bus`.
 
     Edges file requires at least a `source` and `target` column. Optional special
     property columns are `kind` and `labels`.
@@ -35,23 +35,21 @@
     Arguments:
         nodes_path: Path of optional nodes CSV file.
         edges_path: Path of edges CSV file.
         csv_delimiter: Delimiter of CSV file.
         iter_delimiter: Iterable delimiter (i.e. for children names list).
         node_weights: Columns to interpret as node weights.
         edge_weights: Columns to interpret as edge weights.
-
-    Keyword arguments:
-        Optional :obj:`Graph` arguments when instantiating.
+        **graph_kwargs: Optional [`Graph`][ragraph.graph.Graph] arguments when instantiating.
 
     Returns:
         Graph object.
 
     Raises:
-        InconsistencyError if graph is inconsistent.
+        InconsistencyError: if graph is inconsistent.
     """
     graph = Graph(**graph_kwargs)
 
     if not nodes_path and not edges_path:
         return graph
 
     if not node_weights:
@@ -181,15 +179,15 @@
     return node_dict
 
 
 def _derive_nodes(edges_path: Union[str, Path], csv_delimiter: str) -> Dict[str, Node]:
     """Derive nodes from edges CSV file.
 
     Arguments:
-        edge_path: Path to edges CSV file.
+        edges_path: Path to edges CSV file.
         csv_delimiter: CSV delimiter.
 
     Returns:
         Node dictionary (name, node).
     """
 
     with Path(edges_path).open(newline="") as f:
```

### Comparing `ragraph-1.19.0/ragraph/io/grip.py` & `ragraph-1.19.1/ragraph/io/grip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Capability to import GRIP data exports."""
+"""# GRIP format support"""
 from pathlib import Path
 from typing import Union
 from uuid import UUID
 
 from lxml import etree
 
 from ragraph.edge import Edge
```

### Comparing `ragraph-1.19.0/ragraph/io/json.py` & `ragraph-1.19.1/ragraph/io/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""JSON encoding/decoding support."""
+"""# JSON format support"""
 import json
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 from uuid import UUID
 
 from ragraph.edge import Edge
 from ragraph.generic import Annotations
```

### Comparing `ragraph-1.19.0/ragraph/io/matrix.py` & `ragraph-1.19.1/ragraph/io/matrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""Adjacency and mapping matrices support."""
+"""# Adjacency and mapping matrices support"""
 
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from ragraph.edge import Edge
 from ragraph.graph import Graph
 from ragraph.node import Node
 
 try:
     import numpy as np
@@ -15,26 +15,26 @@
 
 def from_matrix(
     matrix: Union["np.ndarray", List[List[int]], List[List[float]]],
     rows: Optional[Union[List[Node], List[str]]] = None,
     cols: Optional[Union[List[Node], List[str]]] = None,
     weight_label: str = "default",
     empty: Optional[Union[int, float]] = 0.0,
-    **graph_args,
+    **graph_args: Dict[str, Any],
 ) -> Graph:
     """Create a graph from an adjacency or mapping matrix.
 
     Arguments:
         matrix: Matrix to convert into a graph.
         rows: Nodes or node labels corresponding to the rows of the matrix.
         cols: Nodes or node labels corresponding to the columns of the matrix. If none
             are provided, the row labels are re-used.
         weight_label: Weight label to use for matrix values.
         empty: Cell value to be considered "empty", e.g. no edge should be created.
-        **graph_args: Additional arguments to :obj:`Graph` constructor.
+        **graph_args: Additional arguments to [`Graph`][ragraph.graph.Graph] constructor.
 
     Returns:
         Graph object.
 
     Note:
         If no row labels are provided, they are generated in a "node#" format.
         If no column labels are provided, they are assumed to be equal to the rows.
@@ -74,15 +74,15 @@
         if matrix[row][col] != empty
     ]
     graph.edges = edges
     return graph
 
 
 def to_matrix(
-    graph,
+    graph: Graph,
     rows: Optional[Union[List[Node], List[str]]] = None,
     cols: Optional[Union[List[Node], List[str]]] = None,
     inherit: bool = False,
     loops: bool = False,
     only: Optional[List[str]] = None,
 ) -> Union[np.ndarray, List[List[float]]]:
     """Convert graph data into a directed numerical adjacency or mapping matrix.
@@ -90,19 +90,19 @@
     Arguments:
         graph: Graph to fetch data from.
         rows: Nodes representing the matrix rows.
         cols: Nodes representing the matrix columns if different from the rows.
         inherit: Whether to count weights between children of the given nodes.
         loops: Whether to calculate self-loops from a node to itself.
         only: Optional subset of edge weights to consider. See
-            :obj:`ragraph.edge.Edge` for default edge weight implementation.
+            [`ragraph.edge.Edge`][ragraph.edge.Edge] for default edge weight implementation.
 
     Returns:
-        Adjacency matrix as a 2D numpy array if numpy is present. Otherwise it will
-        return a 2D nested list.
+        Adjacency matrix as a 2D numpy array if numpy is present. Otherwise it will return a 2D
+        nested list.
 
     Note:
         Note that the matrix is directed! Columns are inputs to rows.
     """
     if rows is None:
         rows = graph.leafs
     else:
```

### Comparing `ragraph-1.19.0/ragraph/io/xml/XMI-Canonical.xsd` & `ragraph-1.19.1/ragraph/io/xml/XMI-Canonical.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/io/xml/__init__.py` & `ragraph-1.19.1/ragraph/io/xml/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,15 +134,16 @@
 ) -> str:
     """Encode Graph to an XML element.
 
     Arguments:
         graph: Graph to convert to XML.
         path: Optional file path to write XML to.
         elem: Optional object to append the Graph to.
-        tostring_args: Optional argument overrides to :obj:`lxml.etree.tostring()`.
+        tostring_args: Optional argument overrides to
+            [`lxml.etree.tostring`][lxml.etree.tostring].
         bundle_schemas: When exporting to a file, bundle the .xsd schemas.
 
     Returns:
         XML element.
     """
 
     if elem is None:
@@ -261,16 +262,16 @@
         elem: XML Element.
         validate: Whether to validate the XML input.
 
     Returns:
         Graph object.
 
     Note:
-        You should only provide one of :obj:`path`, :obj:`enc`, or :obj:`elem`,
-        which are handled in that order of precedence.
+        You should only provide one of `path`, `enc`, or `elem`, which are handled in that order of
+        precedence.
     """
     # Parse input XML.
     if path is not None:
         elem = etree.parse(str(Path(path))).getroot()
     elif enc is not None:
         elem = etree.fromstring(enc)
     elif elem is not None:
```

### Comparing `ragraph-1.19.0/ragraph/io/xml/ragraph.xsd` & `ragraph-1.19.1/ragraph/io/xml/ragraph.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.19.0/ragraph/io/yaml.py` & `ragraph-1.19.1/ragraph/io/yaml.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""YAML dump/load module."""
+"""# YAML format support"""
 from pathlib import Path
 from typing import Optional, Union
 
 from ragraph.graph import Graph
 from ragraph.io.json import graph_from_json_dict
 
 try:
```

### Comparing `ragraph-1.19.0/ragraph/node.py` & `ragraph-1.19.1/ragraph/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Node module. Contains Node class definitions."""
+"""# Node class module"""
 
 from typing import Any, Dict, Generator, Iterable, List, Optional, Union
 from uuid import UUID
 
 from ragraph.generic import Annotations, Metadata
 
 
@@ -181,30 +181,32 @@
             name: Name as str.
             parent: Parent name (not Node) as str.
             children: Children names (not Nodes) as str.
             is_bus: is_bus as bool.
             kind: Kind as str.
             labels: Labels as a list of strings.
             weights: Weights as dict.
-            annotations: Annotations as per :obj:`ragraph.generic.Mapping.as_dict()`.
+            annotations: Annotations as per
+                [`ragraph.generic.Mapping.as_dict`][ragraph.generic.Mapping.as_dict].
         """
         return self.as_dict(use_uuid=True)
 
     def as_dict(self, use_uuid: bool = False) -> Dict[str, Any]:
         """Return a copy as a (serializable) dictionary.
 
         Returns:
             name: Name as str.
             parent: Parent name or UUID (not Node) as str.
             children: Children names (not Nodes) as str.
             is_bus: is_bus as bool.
             kind: Kind as str.
             labels: Labels as a list of strings.
             weights: Weights as dict.
-            annotations: Annotations as per :obj:`ragraph.generic.Mapping.as_dict()`.
+            annotations: Annotations as per
+                [`ragraph.generic.Mapping.as_dict`][ragraph.generic.Mapping.as_dict].
             uuid: UUID as str if toggled.
         """
         if use_uuid:
             return dict(
                 name=self.name,
                 parent=None if self.parent is None else str(self.parent.uuid),
                 children=[str(n.uuid) for n in self.children],
```

### Comparing `ragraph-1.19.0/ragraph/plot/__init__.py` & `ragraph-1.19.1/ragraph/plot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-"""RaGraph plotting module."""
+"""# RaGraph plotting module"""
 from typing import Any, Dict, Iterable, List, Optional
 
 from plotly import graph_objects as go
+
 from ragraph.edge import Edge
 from ragraph.graph import Graph
 from ragraph.node import Node
 from ragraph.plot.generic import Style
 
 
 def dsm(
```

### Comparing `ragraph-1.19.0/ragraph/plot/components/blank.py` & `ragraph-1.19.1/ragraph/plot/components/blank.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+"""# Blank plot component"""
+
 import plotly.graph_objs as go
+
 from ragraph.plot.generic import Component, Style
 
 
 class Blank(Component):
-    """Blank plot component
+    """Blank plot component.
 
     Arguments:
         style: Plot style mapping.
     """
 
-    def __init__(self, style=Style()):
+    def __init__(self, style: Style = Style()):
         trace = go.Scatter(
             x=[0.5 * style.xstep],
             y=[0.5 * style.ystep],
             mode="markers",
             marker=dict(
                 line=dict(
                     color="#FFFFFF",
```

### Comparing `ragraph-1.19.0/ragraph/plot/components/labels.py` & `ragraph-1.19.1/ragraph/plot/components/labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""Re-usable labels list plot component."""
+"""# Labels list plot component"""
 from copy import deepcopy
 from typing import List
 
 from ragraph.node import Node
 from ragraph.plot.generic import Component, Style
 
 
 class Labels(Component):
-    """Labels plot component.
+    """Labels list plot component.
 
     Arguments:
         leafs: List of leaf nodes.
         style: Plot style mapping.
     """
 
     def __init__(self, leafs: List[Node], style: Style = Style()):
```

### Comparing `ragraph-1.19.0/ragraph/plot/components/legend.py` & `ragraph-1.19.1/ragraph/plot/components/legend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-"""Re-usable legend plot components."""
+"""# Legend plot component"""
 
 from collections import defaultdict
 from copy import deepcopy
 from typing import List
 
 import plotly.graph_objs as go
+
 from ragraph.edge import Edge
 from ragraph.plot.generic import Component, Style
 
 
 class Legend(Component):
     """Legend component.
```

### Comparing `ragraph-1.19.0/ragraph/plot/components/piemap.py` & `ragraph-1.19.1/ragraph/plot/components/piemap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Re-usable mapping plot component.
+"""# Piechart mapping matrix plot component
 
 The mapping plot is a matrix of pie-charts, indicating the edges between leaf nodes.
 
 The nodes are identically placed from left-to-right as well as top-to-bottom. This
 results in a diagonal (from top-left to bottom-right) of 'self loops', which are
 commonly used to indicate "the nodes themselves".
 
@@ -34,16 +34,14 @@
     This map, or matrix, of pie-charts display the edges between leaf nodes.
 
     Arguments:
         rows: The nodes to be placed on the rows of the matrix.
         cols: The columns to be placed on the columns of the matrix.
         edges: Edges to be displayed between leaf nodes.
         style: Plot style option mapping.
-        rows: The nodes to be placed on the rows of the matrix.
-        cols: The columns to be placed on the columns of the matrix.
 
     Note:
         The pie-charts can represent a number of things, including edge weights, edge
         labels as well as other metrics. The node hierarchy is included using squares
         drawn around the diagonal.
 
         Furthermore, bus nodes have their respective row and column in a shaded
@@ -511,29 +509,26 @@
             customdata=[customdata],
         )
     ]
 
     return traces, shapes
 
 
-def _get_hierarchy_shapes(leafs: List[Node], style: Style):
+def _get_hierarchy_shapes(leafs: List[Node], style: Style) -> List[Dict[str, Any]]:
     """Get hierarchy shapes for the mapping plot component.
 
     Arguments:
       leafs: List of leaf nodes.
       style: Style of the tree to be plotted.
 
     Returns:
-        Processed ancestor nodes.
-        Tree depth.
-        Dictionary of node to x position of tree nodes.
-        Dictionary of node to y position of tree nodes.
+        Hierarchy shapes as SVG mappings converted to dictionaries.
     """
 
-    shapes = []
+    shapes: List[Dict[str, Any]] = []
 
     # Plot geometrics
     x_step, y_step = style.xstep, style.ystep
     tree_depth = max([node.depth for node in leafs])
     dim = len(leafs)
 
     # Compute leaf node positions.
@@ -638,8 +633,7 @@
         # Horizontal line.
         shapes.append(svg.get_line(x0=0, x1=dim, y0=y, y1=y, line=line).as_dict())
 
         # Vertical line.
         shapes.append(svg.get_line(x0=i, x1=i, y0=0, y1=dim, line=line).as_dict())
 
     return shapes
-    return shapes
```

### Comparing `ragraph-1.19.0/ragraph/plot/components/tree.py` & `ragraph-1.19.1/ragraph/plot/components/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-"""Re-usable hierarchy tree plot component.
+"""# Hierarchy tree plot component
 
-This module contains the :obj:`~get_tree` method which produces a
-:obj:`~ragraph.plot.generic.Component` for the hierarchy tree of a vertical
-list of leaf nodes up to their roots which are put on their left.
+This module contains the [`Tree` component][ragraph.plot.components.tree.Tree] which produces a
+[`Component`][ragraph.plot.generic.Component] for the hierarchy tree of a vertical list of leaf
+nodes up to their roots which are put on their left.
 """
 from collections import OrderedDict
 from copy import deepcopy
 from typing import Any, Dict, List, Set, Tuple, Union
 
 import plotly.graph_objs as go
+
 from ragraph.node import Node
 from ragraph.plot import svg
 from ragraph.plot.generic import Component, Style
 
 
 class Tree(Component):
     """Hierarchy tree plot component of leaf nodes up to their roots.
@@ -189,15 +190,15 @@
 ) -> List[svg.SVG]:
     """Draw a line with a curved 90 degree angle from a parent to a child in the tree.
 
     Arguments:
         x0: x starting coordinate of the line.
         y0: y starting coordinate of the line.
         x1: x ending coordinate of the line.
-        x2: y ending coordinate of the line.
+        y1: y ending coordinate of the line.
         style: Plot style mapping.
 
     Returns:
        List of SVG shape mappings of the different line sections.
     """
     linestyle = style.tree.line
     curve_delta = min(0.1, abs(y0 - y1))
```

### Comparing `ragraph-1.19.0/ragraph/plot/generic.py` & `ragraph-1.19.1/ragraph/plot/generic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""RaGraph generic plotting classes such as :obj:`Component` and :obj:`Style`."""
+"""# RaGraph generic plotting classes"""
 from copy import deepcopy
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from plotly import graph_objs as go
 from plotly.basedatatypes import BaseTraceType
 
 from ragraph import colors
@@ -93,23 +93,23 @@
             for k, v in yaxis.items():
                 setattr(_yaxis, k, v)
             yaxis = _yaxis
 
         super().__init__(line=line, xaxis=xaxis, yaxis=yaxis)
 
     @field
-    def line(self) -> svg.Line:
+    def line(self) -> svg.Line:  # type: ignore
         """Line style mapping for hierarchy tree lines."""
 
     @field
-    def xaxis(self) -> go.layout.XAxis:
+    def xaxis(self) -> go.layout.XAxis:  # type: ignore
         """Plotly X-axis settings."""
 
     @field
-    def yaxis(self) -> go.layout.YAxis:
+    def yaxis(self) -> go.layout.YAxis:  # type: ignore
         """Plotly Y-axis settings."""
 
 
 class LabelsStyle(Mapping):
     """Labels plot component style mapping.
 
     Arguments:
@@ -179,81 +179,80 @@
             shorten=shorten,
             textorientation=textorientation,
             xaxis=xaxis,
             yaxis=yaxis,
         )
 
     @field
-    def fontcolor(self) -> str:
+    def fontcolor(self) -> str:  # type: ignore
         """Font color used for labels."""
 
     @field
-    def fontfamily(self) -> str:
+    def fontfamily(self) -> str:  # type: ignore
         """Font family used for labels."""
 
     @field
-    def fontsize(self) -> int:
+    def fontsize(self) -> int:  # type: ignore
         """Fontsize used for labels."""
 
     @field
-    def fontaspectratio(self) -> float:
+    def fontaspectratio(self) -> float:  # type: ignore
         """Font width per fontsize ratio."""
 
     @field
-    def shorten(self) -> Union[bool, Callable[[str], str]]:
+    def shorten(self) -> Union[bool, Callable[[str], str]]:  # type: ignore
         """Label shortening toggle or function. When set to `True` everything after
         the last dot '.' is kept.
         """
 
     @field
-    def textorientation(self) -> float:
+    def textorientation(self) -> float:  # type: ignore
         """Orientation of text."""
 
     @field
-    def xaxis(self) -> go.layout.XAxis:
+    def xaxis(self) -> go.layout.XAxis:  # type: ignore
         """Plotly X-axis settings."""
 
     @field
-    def yaxis(self) -> go.layout.YAxis:
+    def yaxis(self) -> go.layout.YAxis:  # type: ignore
         """Plotly Y-axis settings."""
 
 
 class PieMapStyle(Mapping):
     """Piechart map's plot component style mapping.
 
     Arguments:
         busarea: Bus area SVG mapping. Used for styling the bus area.
         display: What to display. One of 'kinds', 'labels', 'weight labels', 'weights'.
-        fields: The fields to plot (the selection of kinds, labels, or weights).
-            Leave set to `None` to display all the available fields automatically.
+        fields: The fields to plot (the selection of kinds, labels, or weights). Leave set to `None`
+            to display all the available fields automatically.
         gridline: Grid line options mapping.
-        highlight_col_annotation: Annotation that signals what columns should be
-            highlighted. Value should be True-ish.
+        highlight_col_annotation: Annotation that signals what columns should be highlighted.
+            Value should be True-ish.
         highlight_col_color: Default color to use for column highlights.
-        highlight_row_annotation: Annotation that signals what rows should be
-            highlighted. Value should be True-ish.
+        highlight_row_annotation: Annotation that signals what rows should be highlighted.
+            Value should be True-ish.
         highlight_row_color: Default color to use for row highlights.
         inherit: Whether to display edges between descendants of the axis nodes.
         kindline: Node kind separation lines options mapping.
         mode: How to divide the pie-charts per category: 'equal' or 'relative'.
             'equal' divides the piechart evenly.
             'relative' divides the piechart according to category value.
         radius: The piechart radius between 0.0 and 0.5.
-        scale_weight: Edge weight label that should contain values between 0.0 and 1.0
-            to scale the radius with.
+        scale_weight: Edge weight label that should contain values between 0.0 and 1.0 to scale the
+            radius with.
         customhoverkeys: List of keys for information to be displayed on hover.
         xaxis: Plotly X-axis settings.
         yaxis: Plotly Y-axis settings.
 
     Note:
-        The :obj:`display` argument determines what is going to be plotted as piecharts
-        in the plot area. The :obj:`fields` argument is a filter on the possible
-        values for that display mode. The :obj:`mode` argument then tunes how the wedges
-        that make up the piecharts should be distributed. Most of the time, 'equal'
-        gives the most predictable and clear results.
+        The `display` argument determines what is going to be plotted as piecharts in the plot area.
+        The `fields` argument is a filter on the possible values for that display mode. The `mode`
+        argument then tunes how the wedges that make up the piecharts should be distributed. Most of
+        the time, 'equal' gives the most predictable and clear results.
     """
 
     _defaults = dict(
         busarea=svg.SVG(fillcolor="rgba(150,150,150,0.2)", line=svg.Line(width=0), layer="below"),
         clusterline=svg.Line(width=2, color="gray", dash="solid"),
         display="kinds",
         fields=None,
@@ -336,86 +335,86 @@
             scale_weight=scale_weight,
             customhoverkeys=customhoverkeys,
             xaxis=xaxis,
             yaxis=yaxis,
         )
 
     @field
-    def busarea(self) -> svg.SVG:
+    def busarea(self) -> svg.SVG:  # type: ignore
         """Bus area SVG mapping. Used for styling the bus area."""
 
     @field
-    def display(self) -> str:
+    def display(self) -> str:  # type: ignore
         """What to display. One of 'kinds', 'labels', 'weight labels', 'weights'."""
 
     @field
-    def fields(self) -> List[str]:
+    def fields(self) -> List[str]:  # type: ignore
         """The fields to plot (the selection of kinds, labels, or weights). Leave set
         to `None` to display all the available fields automatically.
         """
 
     @field
-    def gridline(self) -> svg.Line:
+    def gridline(self) -> svg.Line:  # type: ignore
         """Grid line style."""
 
     @field
-    def highlight_col_annotation(self) -> Optional[str]:
+    def highlight_col_annotation(self) -> Optional[str]:  # type: ignore
         """Annotation that signals what columns should be highlighted.
         Value should be True-ish.
         """
 
     @field
-    def highlight_col_color(self) -> Optional[str]:
+    def highlight_col_color(self) -> Optional[str]:  # type: ignore
         """Default color to use for column highlights."""
 
     @field
-    def highlight_row_annotation(self) -> Optional[str]:
+    def highlight_row_annotation(self) -> Optional[str]:  # type: ignore
         """Annotation that signals what rows should be highlighted.
         Value should be True-ish.
         """
 
     @field
-    def highlight_row_color(self) -> Optional[str]:
+    def highlight_row_color(self) -> Optional[str]:  # type: ignore
         """Default color to use for row highlights."""
 
     @field
-    def inherit(self) -> bool:
+    def inherit(self) -> bool:  # type: ignore
         """Whether to display edges between descendants of the axis nodes."""
 
     @field
-    def kindline(self) -> svg.Line:
+    def kindline(self) -> svg.Line:  # type: ignore
         """Node kind separation lines options mapping."""
 
     @field
-    def mode(self) -> str:
+    def mode(self) -> str:  # type: ignore
         """How to divide the piecharts per field. Either 'equal' or 'relative'.
         'equal' divides the piecharts evenly.
         'relative' divides the piechart according to field value.
         """
 
     @field
-    def radius(self) -> float:
+    def radius(self) -> float:  # type: ignore
         """The piechart radius between 0.0 and 0.5."""
 
     @field
-    def scale_weight(self) -> str:
+    def scale_weight(self) -> str:  # type: ignore
         """Edge weight label that should contain values between 0.0 and 1.0 to scale the
         radius with.
         """
 
     @field
-    def customhoverkeys(self) -> List[str]:
+    def customhoverkeys(self) -> List[str]:  # type: ignore
         """Custom keys for information to be displayed on hover."""
 
     @field
-    def xaxis(self) -> go.layout.XAxis:
+    def xaxis(self) -> go.layout.XAxis:  # type: ignore
         """Plotly X-axis settings."""
 
     @field
-    def yaxis(self) -> go.layout.YAxis:
+    def yaxis(self) -> go.layout.YAxis:  # type: ignore
         """Plotly Y-axis settings."""
 
 
 class FieldPalette(Mapping):
     """Palettes for a field in a plot.
 
     Argument:
@@ -432,31 +431,31 @@
         self,
         categorical: Optional[Union[str, List[str]]] = None,
         continuous: Optional[List[str]] = None,
     ):
         super().__init__(self, categorical=categorical, continuous=continuous)
 
     @field
-    def categorical(self) -> Optional[str]:
+    def categorical(self) -> Optional[str]:  # type: ignore
         """Categorical color for this field."""
 
     @field
-    def continuous(self) -> Optional[List[str]]:
+    def continuous(self) -> Optional[List[str]]:  # type: ignore
         """Continuous (numeric) data color palette for this field."""
 
 
 class Palettes(Mapping):
     """Plot palettes mapping.
 
     Arguments:
         categorical: Categorical data color palette.
         continuous: Continuous (numeric) data color palette.
         fields: Palette override dictionary per display field.
-        domains: Value domains to interpolate palettes between per field as a tuple
-            of (lower, upper) bounds. Only used for continuous fields.
+        domains: Value domains to interpolate palettes between per field as a tuple of
+            (lower, upper) bounds. Only used for continuous fields.
     """
 
     _defaults = dict(
         categorical=colors.get_categorical(),
         continuous=colors.get_continuous(),
         fields=dict(),
         domains=dict(),
@@ -539,27 +538,27 @@
         step = (upper - lower) / (len(palette) - 1)
         idx = int((value - lower) // step)
 
         idx = min(max(idx, 0), len(palette) - 1)
         return palette[idx]
 
     @field
-    def categorical(self) -> List[str]:
+    def categorical(self) -> List[str]:  # type: ignore
         """Categorical data color palette."""
 
     @field
-    def continuous(self) -> List[str]:
+    def continuous(self) -> List[str]:  # type: ignore
         """Continuous (numeric) data color palette."""
 
     @field
-    def fields(self) -> Dict[str, Union[str, List[str], FieldPalette]]:
+    def fields(self) -> Dict[str, Union[str, List[str], FieldPalette]]:  # type: ignore
         """Palette override dictionary per display field."""
 
     @field
-    def domains(self) -> Dict[str, Tuple[float, float]]:
+    def domains(self) -> Dict[str, Tuple[float, float]]:  # type: ignore
         """Value domains to interpolate palettes between per field as a tuple of
         (lower, upper), bounds. Only used for continuous fields.
         """
 
 
 class LegendStyle(Mapping):
     """Legend plot component style mapping.
@@ -633,44 +632,44 @@
             height=height,
             n_ticks=n_ticks,
             xaxis=xaxis,
             yaxis=yaxis,
         )
 
     @field
-    def fontcolor(self) -> str:
+    def fontcolor(self) -> str:  # type: ignore
         """Font color used for labels."""
 
     @field
-    def fontfamily(self) -> str:
+    def fontfamily(self) -> str:  # type: ignore
         """Font family used for labels."""
 
     @field
-    def fontsize(self) -> int:
+    def fontsize(self) -> int:  # type: ignore
         """Fontsize used for labels."""
 
     @field
-    def fontaspectratio(self) -> float:
+    def fontaspectratio(self) -> float:  # type: ignore
         """Font width per fontsize ratio."""
 
     @field
-    def height(self) -> int:
+    def height(self) -> int:  # type: ignore
         """Height of the swatch plot in number of box sizes when plotting a
         numerical legend."""
 
     @field
-    def n_ticks(self) -> int:
+    def n_ticks(self) -> int:  # type: ignore
         """Number of ticks in the swatch plot when plotting a numerical legend."""
 
     @field
-    def xaxis(self) -> go.layout.XAxis:
+    def xaxis(self) -> go.layout.XAxis:  # type: ignore
         """Plotly X-axis settings."""
 
     @field
-    def yaxis(self) -> go.layout.YAxis:
+    def yaxis(self) -> go.layout.YAxis:  # type: ignore
         """Plotly Y-axis settings."""
 
 
 class Style(Mapping):
     """RaGraph plot style mapping.
 
     Arguments:
@@ -753,68 +752,68 @@
             show_legend=show_legend,
             row_col_numbers=row_col_numbers,
             xstep=xstep,
             ystep=ystep,
         )
 
     @field
-    def boxsize(self) -> int:
+    def boxsize(self) -> int:  # type: ignore
         """Size in pixels per row or column."""
 
     @field
-    def config(self) -> Dict[str, Any]:
+    def config(self) -> Dict[str, Any]:  # type: ignore
         """Plotly Figure.show() config."""
 
     @field
-    def highlight_annotation(self) -> Optional[str]:
+    def highlight_annotation(self) -> Optional[str]:  # type: ignore
         """Annotation key of instances that should be highlighted.
         Value should be True-ish. Set key to `None` to disable."""
 
     @field
-    def highlight_color(self) -> str:
+    def highlight_color(self) -> str:  # type: ignore
         """Default color to use for highlights."""
 
     @field
-    def labels(self) -> LabelsStyle:
+    def labels(self) -> LabelsStyle:  # type: ignore
         """Labels plot style."""
 
     @field
-    def layout(self) -> go.Layout:
+    def layout(self) -> go.Layout:  # type: ignore
         """Layout options."""
 
     @field
-    def palettes(self) -> Palettes:
+    def palettes(self) -> Palettes:  # type: ignore
         """Plot palettes options."""
 
     @field
-    def piemap(self) -> PieMapStyle:
+    def piemap(self) -> PieMapStyle:  # type: ignore
         """Piechart map plot style."""
 
     @field
-    def tree(self) -> TreeStyle:
+    def tree(self) -> TreeStyle:  # type: ignore
         """Tree plot style."""
 
     @field
-    def legend(self) -> LegendStyle:
+    def legend(self) -> LegendStyle:  # type: ignore
         """Legend plot style."""
 
     @field
-    def show_legend(self) -> bool:
+    def show_legend(self) -> bool:  # type: ignore
         """Boolean to display a legend."""
 
     @field
-    def row_col_numbers(self) -> bool:
+    def row_col_numbers(self) -> bool:  # type: ignore
         """Boolean to display row and column numbers."""
 
     @field
-    def xstep(self) -> float:
+    def xstep(self) -> float:  # type: ignore
         """Axis increment per row or column in plots (usually 1)."""
 
     @field
-    def ystep(self) -> float:
+    def ystep(self) -> float:  # type: ignore
         """Axis increment per row or column in plots (usually 1)."""
 
 
 class Component(Mapping):
     """Plot component. The basic building block to create compound Plotly figures with.
 
     Arguments:
@@ -865,39 +864,39 @@
             shapes=shapes,
             annotations=annotations,
             xaxis=xaxis,
             yaxis=yaxis,
         )
 
     @field
-    def width(self) -> float:
+    def width(self) -> float:  # type: ignore
         """Width in pixels."""
 
     @field
-    def height(self) -> float:
+    def height(self) -> float:  # type: ignore
         """Height in pixels."""
 
     @field
-    def traces(self) -> List[BaseTraceType]:
+    def traces(self) -> List[BaseTraceType]:  # type: ignore
         """Traces to plot in this domain."""
 
     @field
-    def shapes(self) -> List[Dict[str, Any]]:
+    def shapes(self) -> List[Dict[str, Any]]:  # type: ignore
         """SVG shapes from this component."""
 
     @field
-    def annotations(self) -> List[Dict[str, Any]]:
+    def annotations(self) -> List[Dict[str, Any]]:  # type: ignore
         """Annotations from this component."""
 
     @field
-    def xaxis(self) -> go.layout.XAxis:
+    def xaxis(self) -> go.layout.XAxis:  # type: ignore
         """Plotly X-axis options."""
 
     @field
-    def yaxis(self) -> go.layout.YAxis:
+    def yaxis(self) -> go.layout.YAxis:  # type: ignore
         """Plotly Y-axis options."""
 
     def get_figure(self, style: Style = Style(), show: bool = True) -> Optional[go.Figure]:
         """Get a Plotly figure of this component alone."""
         from ragraph.plot.utils import get_subplots, process_fig
 
         fig = get_subplots([[self]], style=style)
```

### Comparing `ragraph-1.19.0/ragraph/plot/svg.py` & `ragraph-1.19.1/ragraph/plot/svg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-"""SVG shape methods.
+"""# SVG shapes
 
-This module contains two base classes, being the :obj:`Line` options for SVG shapes and
-a SVG mapping for the shapes themselves. You will also find several methods to obtain
-several basic shapes conveniently.
+This module contains two base classes, being the [`Line`][ragraph.plot.svg.Line] options for SVG
+shapes and an [`SVG`][ragraph.plot.svg.SVG] mapping for the shapes themselves. You will also find
+several methods to obtain several basic shapes conveniently.
 """
 from math import cos, pi, sin
 from typing import Any, Dict, Optional, Union
 
 from ragraph.generic import Mapping, field
 
 
@@ -26,23 +26,23 @@
         color: Optional[str] = None,
         width: Optional[int] = None,
         dash: Optional[str] = None,
     ):
         super().__init__(color=color, width=width, dash=dash)
 
     @field
-    def color(self) -> str:
+    def color(self) -> str:  # type: ignore
         """Line color."""
 
     @field
-    def width(self) -> int:
+    def width(self) -> int:  # type: ignore
         """Line width in pixels."""
 
     @field
-    def dash(self) -> str:
+    def dash(self) -> str:  # type: ignore
         """Dash style of the line."""
 
 
 class SVG(Mapping):
     """SVG shape mapping.
 
     Arguments:
@@ -55,19 +55,19 @@
         x0: Starting x position.
         x1: Ending x position.
         yref: y coordinate axis. 'paper' or 'y', 'y1', 'y2', etc.
         ysizemode: 'scaled' or 'pixel'. Relative or absolute sizing w.r.t. axis.
         yanchor: If sizemode is set to 'pixel', reference on axis to anchor shape to.
         y0: Starting y position.
         y1: Ending y position.
-        path: For shapetype 'path', a valid SVG path, with data values as coordinates
-         when referencing axis and absolute pixels with respect to anchors when the
-         'pixel' sizemode is set.
+        path: For shapetype 'path', a valid SVG path, with data values as coordinates when
+            referencing axis and absolute pixels with respect to anchors when the 'pixel' sizemode
+            is set.
         opacity: The opacity between 0.0 and 1.0.
-        line: Line mapping options. See :obj:`Line`.
+        line: Line mapping options. See [`Line`][ragraph.plot.svg.Line].
         fillcolor: Interior shape color.
         fillrule: Determines which regions of complex paths constitute the interior.
             One of "evenodd" or "nonzero".
         editable: Whether the shape could be activated for edit or not.
         name: Only used with templates.
         templateitemname: Used to refer to a named item in this array in the template.
     """
@@ -141,192 +141,185 @@
             fillrule=fillrule,
             editable=editable,
             name=name,
             templateitemname=templateitemname,
         )
 
     @field
-    def visible(self) -> bool:
+    def visible(self) -> bool:  # type: ignore
         """Toggles shape visibility."""
 
     @field
-    def type(self) -> str:
+    def type(self) -> str:  # type: ignore
         """One of 'circle', 'rect', 'path' or 'line'."""
 
     @field
-    def layer(self) -> str:
+    def layer(self) -> str:  # type: ignore
         """'above' draws shape above traces, 'below' under them."""
 
     @field
-    def xref(self) -> str:
+    def xref(self) -> str:  # type: ignore
         """x coordinate axis. 'paper' or 'x', 'x1', 'x2', etc."""
 
     @field
-    def xsizemode(self) -> str:
+    def xsizemode(self) -> str:  # type: ignore
         """'scaled' or 'pixel'. Relative or absolute sizing w.r.t. axis."""
 
     @field
-    def xanchor(self) -> str:
+    def xanchor(self) -> str:  # type: ignore
         """If sizemode is set to 'pixel', reference on axis to anchor shape to."""
 
     @field
-    def x0(self) -> float:
+    def x0(self) -> float:  # type: ignore
         """Starting x position."""
 
     @field
-    def x1(self) -> float:
+    def x1(self) -> float:  # type: ignore
         """Ending x position."""
 
     @field
-    def yref(self) -> str:
+    def yref(self) -> str:  # type: ignore
         """y coordinate axis. 'paper' or 'y', 'y1', 'y2', etc."""
 
     @field
-    def ysizemode(self) -> str:
+    def ysizemode(self) -> str:  # type: ignore
         """'scaled' or 'pixel'. Relative or absolute sizing w.r.t. axis."""
 
     @field
-    def yanchor(self) -> str:
+    def yanchor(self) -> str:  # type: ignore
         """If sizemode is set to 'pixel', reference on axis to anchor shape to."""
 
     @field
-    def y0(self) -> float:
+    def y0(self) -> float:  # type: ignore
         """Starting y position."""
 
     @field
-    def y1(self) -> float:
+    def y1(self) -> float:  # type: ignore
         """Ending y position."""
 
     @field
-    def path(self) -> str:
-        """For shapetype 'path', a valid SVG path, with data values as coordinates when
-        referencing axis and absolute pixels with respect to anchors when the 'pixel'
-        sizemode is set.
+    def path(self) -> str:  # type: ignore
+        """For shapetype 'path', a valid SVG path, with data values as coordinates when referencing
+        axis and absolute pixels with respect to anchors when the 'pixel' sizemode is set.
         """
 
     @field
-    def opacity(self) -> float:
+    def opacity(self) -> float:  # type: ignore
         """The opacity between 0.0 and 1.0."""
 
     @field
-    def line(self) -> Line:
-        """Line mapping options. See :obj:`Line`."""
+    def line(self) -> Line:  # type: ignore
+        """Line mapping options. See [`Line`][ragraph.plot.svg.Line]."""
 
     @field
-    def fillcolor(self) -> str:
+    def fillcolor(self) -> str:  # type: ignore
         """Interior shape color."""
 
     @field
-    def fillrule(self) -> str:
+    def fillrule(self) -> str:  # type: ignore
         """Determines which regions of complex paths constitute the interior.
         One of 'evenodd' or 'nonzero'.
         """
 
     @field
-    def editable(self) -> bool:
+    def editable(self) -> bool:  # type: ignore
         """Whether the shape could be activated for edit or not."""
 
     @field
-    def name(self) -> str:
+    def name(self) -> str:  # type: ignore
         """Only used with templates."""
 
     @field
-    def templateitemname(self) -> str:
+    def templateitemname(self) -> str:  # type: ignore
         """Used to refer to a named item in this array in the template."""
 
 
 def get_line(
     x0: float,
     x1: float,
     y0: float,
     y1: float,
-    **kwargs,
+    **kwargs: Any,
 ) -> SVG:
     """Get straight line SVG mapping.
 
     Arguments:
         x0: Starting x position.
         x1: Ending x position.
         y0: Starting y position.
         y1: Ending y position.
-
-    Keyword arguments:
-        Overrides for the :obj:`SVG` object.
+        **kwargs: Overrides for the [`SVG`][ragraph.plot.svg.SVG] object.
 
     Returns:
         SVG shape mapping.
     """
     return SVG(type="line", x0=x0, x1=x1, y0=y0, y1=y1, **kwargs)
 
 
 def get_curvedline(
     x0: float,
     x1: float,
     x2: float,
     y0: float,
     y1: float,
     y2: float,
-    **kwargs,
+    **kwargs: Any,
 ) -> SVG:
     """Get curved line (quadratic Bezier) SVG mapping.
 
     Arguments:
         x0: Starting x position.
         x1: Control point x position.
         x2: Ending x position.
         y0: Starting y position.
         y1: Control point y position.
         y2: Ending y position.
-
-    Keyword arguments:
-        Overrides for the :obj:`SVG` object.
+        **kwargs: Overrides for the [`SVG`][ragraph.plot.svg.SVG] object.
 
     Returns:
         Quadratic Bezier SVG shape mapping.
     """
     path = f"M {x0} {y0} Q {x1} {y1} {x2} {y2}"
     return SVG(type="path", path=path, **kwargs)
 
 
 def get_rectangle(
     x0: float,
     x1: float,
     y0: float,
     y1: float,
-    **kwargs,
+    **kwargs: Any,
 ) -> SVG:
     """Get a rectangle SVG mapping.
 
     Arguments:
         x0: Starting x position.
         x1: Ending x position.
         y0: Starting y position.
         y1: Ending y position.
-
-    Keyword arguments:
-        Overrides for the :obj:`SVG` object.
+        **kwargs: Overrides for the [`SVG`][ragraph.plot.svg.SVG] object.
 
     Returns:
         SVG shape mapping.
     """
     return SVG(type="rect", x0=x0, x1=x1, y0=y0, y1=y1, **kwargs)
 
 
-def get_wedge(x: float, y: float, r: float, start_angle: float, end_angle: float, **kwargs) -> SVG:
+def get_wedge(
+    x: float, y: float, r: float, start_angle: float, end_angle: float, **kwargs: Any
+) -> SVG:
     """Get a wedge SVG mapping.
 
     Arguments:
         x: x position of the wedge center.
         y: y position of the wedge center.
         r: radius of the wedge.
         start_angle: Starting angle (radians) of the wedge.
         end_angle: Ending angle (radians) of the wedge.
-
-    Keyword arguments:
-        Overrides for the :obj:`SVG` object.
+        **kwargs: Overrides for the [`SVG`][ragraph.plot.svg.SVG] object.
 
     Returns:
         SVG shape mapping.
     """
     segments = ["M {} {}".format(x, y)]
     xa = x + round(r * cos(start_angle), 3)
     xb = y + round(r * sin(start_angle), 3)
```

### Comparing `ragraph-1.19.0/ragraph/plot/utils.py` & `ragraph-1.19.1/ragraph/plot/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """RaGraph plot utilities."""
-from typing import Dict, List, Optional, Union
+from typing import Dict, Iterable, List, Optional, Union
 
 from plotly import graph_objects as go
 from plotly.subplots import make_subplots
+
 from ragraph.analysis.sequence._axis import get_axis_sequence  # noqa
 from ragraph.edge import Edge
 from ragraph.node import Node
 from ragraph.plot.components.blank import Blank
 from ragraph.plot.components.labels import Labels
 from ragraph.plot.components.legend import Legend
 from ragraph.plot.components.piemap import PieMap
 from ragraph.plot.components.tree import Tree
 from ragraph.plot.generic import Component, Style
 
 
-def get_subplots(components: List[List[Optional[Component]]], style=Style()) -> go.Figure:
-    """Get a subplots :obj:`plotly.graph_objects.Figure` the given
+def get_subplots(components: List[List[Optional[Component]]], style: Style = Style()) -> go.Figure:
+    """Get a subplots [`plotly.graph_objects.Figure`][plotly.graph_objects.Figure] for the given
+    components list of lists.
 
     Arguments:
-        components: Components to be laid out as subplots based on their width and
-            height properties.
-
-    Keyword arguments:
-        Passed on to :obj:`plotly.subplots.make_subplots`.
+        components: Components to be laid out as subplots based on their width and height
+            properties.
+        style: Style options.
     """
     rows = len(components)
 
     components_t = list(zip(*components))  # Transpose helper matrix.
     cols = len(components_t)
 
     min_x_ranges = [
@@ -133,15 +133,15 @@
         }
     )
 
     return fig
 
 
 def process_fig(fig: go.Figure, style: Style = Style(), show: bool = True) -> Optional[go.Figure]:
-    """Show figure with config if :obj:`show` is set, otherwise return figure unchanged.
+    """Show figure with config if `show` is set, otherwise return figure unchanged.
 
     Arguments:
         fig: Plotly figure.
         style: Style containing additional config.
         show: Whether to show the figure inline.
     """
     if show:
@@ -267,22 +267,20 @@
     if col_num_row:
         grid.append(col_num_row)
     grid.append(piemap_row)
 
     return grid
 
 
-def get_swatchplot(*args, **kwargs: Dict[str, List[str]]) -> go.Figure:
+def get_swatchplot(*args: Iterable[List[str]], **kwargs: Dict[str, List[str]]) -> go.Figure:
     """Swatch plot of colormaps.
 
     Arguments:
-        Hex coded color lists.
-
-    Keyword arguments:
-        Names to hex coded color lists.
+        *args: Hex coded color lists.
+        **kwargs: Names to hex coded color lists.
 
     Returns:
         Plotly figure.
     """
     colormaps = kwargs
     for i, colormap in enumerate(args):
         colormaps[str(i)] = colormap
```

### Comparing `ragraph-1.19.0/ragraph/utils.py` & `ragraph-1.19.1/ragraph/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""Graph handling utilities module."""
-from typing import Generator, List, Set
+"""# Graph handling utilities"""
+from typing import TYPE_CHECKING, Generator, List, Set
 
-from ragraph.node import Node
+if TYPE_CHECKING:
+    from ragraph.graph import Graph
+    from ragraph.node import Node
 
 
 def select_nodes(
-    graph, node_kinds: List[str], edge_kinds: List[str], depth: int, selection_mode: str
-) -> List[Node]:
+    graph: "Graph", node_kinds: List[str], edge_kinds: List[str], depth: int, selection_mode: str
+) -> List["Node"]:
     """Select specific nodes from this graph in a structured order.
 
     Arguments:
         graph: Graph to fetch data from.
         node_kinds: The kind of nodes to be selected.
         edge_kinds: The kind of edges to be selected.
         depth: The maximum depth of node to be selected.
         selection_mode: The selection mode. Either 'dependent' or 'independent'.
 
     Note:
         The selection mode argument determines how nodes of different kinds are
         selected. If the selection mode is set to 'dependent', the first node kind
-        in the :obj:`node_kinds` list is considered to be the 'lead node kind'.
+        in the `node_kinds` list is considered to be the 'lead node kind'.
         Nodes of different kind than the lead node kind, are only selected if they
         have a dependency with at least one of the selected nodes of the lead node
         kind. If the selection mode is set to 'independent' this dependency
         condition is dropped.
     """
     node_kinds = node_kinds or graph.node_kinds
 
@@ -55,30 +57,30 @@
     dependent_nodes = [
         n for n in candidate_nodes if is_dependent(graph, lead_nodes, n, edge_kindset)
     ]
 
     return lead_nodes + dependent_nodes
 
 
-def get_up_to_depth(roots: List[Node], depth: int) -> Generator[Node, None, None]:
+def get_up_to_depth(roots: List["Node"], depth: int) -> Generator["Node", None, None]:
     """Get nodes up to a certain depth with bus nodes at the start of child lists."""
     for node in roots:
         if node.is_leaf or node.depth == depth:
             yield node
             continue
 
         children = sorted(node.children, key=lambda n: n.is_bus, reverse=True)
 
         if node.depth == depth - 1:
             yield from children
         else:
             yield from get_up_to_depth(children, depth)
 
 
-def is_dependent(graph, lead_nodes: List[Node], node: Node, edge_kinds=Set[str]) -> bool:
+def is_dependent(graph, lead_nodes: List["Node"], node: "Node", edge_kinds=Set[str]) -> bool:
     """Check if a node is dependent on the lead node kind.
 
     E.g. an edge of the allowed kinds exists to or from the lead nodes.
     """
     return any(
         True for e in graph.edges_between_all(lead_nodes, [node]) if e.kind in edge_kinds
     ) or any(True for e in graph.edges_between_all([node], lead_nodes) if e.kind in edge_kinds)
```

### Comparing `ragraph-1.19.0/PKG-INFO` & `ragraph-1.19.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragraph
-Version: 1.19.0
+Version: 1.19.1
 Summary: Ratio graph handling in Python.
 Home-page: https://ragraph.ratio-case.nl
 License: GPL-3.0-or-later
 Author: Ratio Innovations B.V.
 Author-email: info@ratio-case.nl
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -16,78 +16,64 @@
 Provides-Extra: esl
 Provides-Extra: plot
 Requires-Dist: dd (>=0.5,<0.6)
 Requires-Dist: kaleido (==0.2.1) ; extra == "plot" or extra == "all"
 Requires-Dist: lxml (>=4,<5)
 Requires-Dist: numpy (>=1,<2)
 Requires-Dist: plotly (>=5,<6)
-Requires-Dist: raesl ; extra == "esl" or extra == "all"
+Requires-Dist: raesl (>=0,<1) ; extra == "esl" or extra == "all"
 Requires-Dist: ratio-genetic-py (>=0.3,<0.4)
 Requires-Dist: ruamel.yaml (>=0.17,<0.18)
 Project-URL: Documentation, https://ragraph.ratio-case.nl
 Project-URL: Repository, https://gitlab.com/ratio-case-os/python/ragraph
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
-#######
-RaGraph
-#######
+# RaGraph
 
-RaGraph is a package to create, manipulate, and analyze graphs consisting of nodes and
-edges. Nodes usually represent (hierarchies of) objects and edges the dependencies or
-relationships between them.
+RaGraph is a package to create, manipulate, and analyze graphs consisting of nodes and edges. Nodes
+usually represent (hierarchies of) objects and edges the dependencies or relationships between them.
 
-These graphs, or networks if you will, lend themselves well to applied analyses like
-clustering and sequencing, as well as analyses involving the calculation of various
-insightful metrics.
+These graphs, or networks if you will, lend themselves well to applied analyses like clustering and
+sequencing, as well as analyses involving the calculation of various insightful metrics.
 
+## User documentation
 
-**********
-Quickstart
-**********
+For all user-facing documentation, please head over to our beautiful documentation over at
+[https://ragraph.ratio-case.nl](https://ragraph.ratio-case.nl)!
 
-Installation
-============
+## Development installation
 
-RaGraph can be installed using ``pip install ragraph[all]`` for any Python version >=3.9. Or,
-for Poetry managed projects, use ``poetry add ragraph -E all`` to add it as a dependency.
+This project is packaged using [poetry](https://python-poetry.org/). Packaging information as well
+as dependencies are stored in [pyproject.toml](./pyproject.toml).
 
+Installing the project and its development dependencies can be done using `poetry install -E all`.
 
-Using RaGraph
-=============
+### Tests
 
-RaGraph's primary use is working with Graph objects that contain Nodes and Eges between
-Nodes. See the `usage documentation <https://ragraph.ratio-case.nl/usage/index.html>`_
-for more info!
+Tests can be run using `poetry run pytest`.
 
-***************
-Developer guide
-***************
+### Linting
 
-Python packaging information
-============================
+Linting config is included in [pyproject.toml](./pyproject.toml) for both Black and Ruff.
 
-This project is packaged using `poetry <https://python-poetry.org/>`_. Packaging
-information as well as dependencies are stored in `pyproject.toml <./pyproject.toml>`_.
+## Contributions and license
 
-Installing the project and its development dependencies can be done using ``poetry install -E all``.
+To get contributing, feel free to fork, pick up an issue or file your own and get going for your
+first merge! We'll be more than happy to help.
 
-Versioning
-==========
+For contribution instructions, head over to the [open-source GitLab
+repository](https://gitlab.com/ratio-case-os/python/ragraph)!
 
-This project uses `semantic versioning <https://semver.org>`_. Version increments are
-checked using `Raver <https://raver.ratio-case.nl>`_.
+All code snippets in the tutorial and how-to guide sections of the package documentation are free to
+use.
 
-Changelog
-=========
+If you find any documentation worthwhile citing, please do so with a proper reference to our
+documentation!
 
-Changelog format as described by https://keepachangelog.com/ has been adopted and can be reviewed `on this page <https://ragraph.ratio-case.nl/changelog.html>`.
-
-Tests
-=====
-
-Tests can be run using ``poetry run pytest``.
-
-Linting
-=======
-
-Linting config is included in `pyproject.toml <./pyproject.toml>`_ for both Black and Ruff.
+RaGraph is licensed following a dual licensing model. In short, we want to provide anyone that
+wishes to use our published software under the GNU GPLv3 to do so freely and without any further
+limitation. The GNU GPLv3 is a strong copyleft license that promotes the distribution of free,
+open-source software. In that spirit, it requires dependent pieces of software to follow the same
+route. This might be too restrictive for some. To accommodate users with specific requirements
+regarding licenses, we offer a proprietary license. The terms can be discussed by reaching out to
+Ratio.
```


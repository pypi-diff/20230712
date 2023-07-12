# Comparing `tmp/genomehubs-2.7.6.tar.gz` & `tmp/genomehubs-2.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomehubs-2.7.6.tar", last modified: Fri Jun 30 15:58:29 2023, max compression
+gzip compressed data, was "genomehubs-2.7.7.tar", last modified: Wed Jul 12 15:59:54 2023, max compression
```

## Comparing `genomehubs-2.7.6.tar` & `genomehubs-2.7.7.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.432419 genomehubs-2.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-30 15:57:45.000000 genomehubs-2.7.6/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 15:57:45.000000 genomehubs-2.7.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-30 15:57:45.000000 genomehubs-2.7.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-30 15:57:45.000000 genomehubs-2.7.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-30 15:57:45.000000 genomehubs-2.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-30 15:57:45.000000 genomehubs-2.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-30 15:58:29.432419 genomehubs-2.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-30 15:57:45.000000 genomehubs-2.7.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-30 15:57:45.000000 genomehubs-2.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-30 15:58:29.432419 genomehubs-2.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-30 15:57:45.000000 genomehubs-2.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.416419 genomehubs-2.7.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.420419 genomehubs-2.7.6/src/genomehubs/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.420419 genomehubs-2.7.6/src/genomehubs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/config/dist.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/genomehubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.424419 genomehubs-2.7.6/src/genomehubs/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/btk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/busco.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/es_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    34397 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/gbif.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    35765 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    37857 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/taxon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/wikidata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/lib/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.428419 genomehubs-2.7.6/src/genomehubs/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/ATTR_assembly.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/ATTR_btk.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/ATTR_busco.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/ATTR_feature.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/ATTR_sample.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/ATTR_window_stats.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/TAXON_assembly.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/analysis.json
--rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/assembly.json
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/assembly.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/btk.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/busco.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/busco_feature.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/feature.json
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/file.json
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/identifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/organelle.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/sample.types.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.432419 genomehubs-2.7.6/src/genomehubs/templates/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/analysis_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/analysis_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/assembly_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/assembly_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/attribute_types_by_group.json
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/attribute_values_by_taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/attributes_by_keyword_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/attributes_identifiers_by_keyword_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/attributes_names_by_keyword_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/file_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/file_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/max_nested_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/max_nested_value_by_key_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/max_nested_value_by_type.json
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/search_by_taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_attributes_by_taxon_id.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_any_name.json
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_name.json
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_specific_name.json
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_names.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_names_by_root.json
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/taxonomy_node_by_taxon_id.json
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/scripts/value_by_type_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/taxon.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/taxonomy.json
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/wikidata.names.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/window_full.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-30 15:57:45.000000 genomehubs-2.7.6/src/genomehubs/templates/window_stats.types.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:58:29.420419 genomehubs-2.7.6/src/genomehubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-30 15:58:29.000000 genomehubs-2.7.6/src/genomehubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-30 15:58:29.000000 genomehubs-2.7.6/src/genomehubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:58:29.000000 genomehubs-2.7.6/src/genomehubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-30 15:58:29.000000 genomehubs-2.7.6/src/genomehubs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-30 15:58:29.000000 genomehubs-2.7.6/src/genomehubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 15:58:29.000000 genomehubs-2.7.6/src/genomehubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:59:54.904430 genomehubs-2.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-12 15:59:23.000000 genomehubs-2.7.7/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-12 15:59:23.000000 genomehubs-2.7.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-12 15:59:23.000000 genomehubs-2.7.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-12 15:59:23.000000 genomehubs-2.7.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-12 15:59:23.000000 genomehubs-2.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 15:59:23.000000 genomehubs-2.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-12 15:59:54.904430 genomehubs-2.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-12 15:59:23.000000 genomehubs-2.7.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-12 15:59:23.000000 genomehubs-2.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-12 15:59:54.908431 genomehubs-2.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-07-12 15:59:23.000000 genomehubs-2.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:59:54.892431 genomehubs-2.7.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:59:54.896431 genomehubs-2.7.7/src/genomehubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:59:54.896431 genomehubs-2.7.7/src/genomehubs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/config/dist.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/genomehubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:59:54.900431 genomehubs-2.7.7/src/genomehubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/btk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/busco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/es_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34397 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/gbif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36878 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37857 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/taxon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/wikidata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/lib/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:59:54.900431 genomehubs-2.7.7/src/genomehubs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    89855 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/ATTR_ancestral_unit.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/ATTR_assembly.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/ATTR_btk.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/ATTR_busco.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/ATTR_feature.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/ATTR_sample.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/ATTR_window_stats.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/TAXON_assembly.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/analysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/assembly.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/assembly.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/attributes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/btk.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/busco.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/busco_feature.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/identifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/organelle.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/sample.types.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:59:54.904430 genomehubs-2.7.7/src/genomehubs/templates/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/analysis_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/analysis_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/assembly_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/assembly_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/attribute_types_by_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/attribute_values_by_taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/attributes_by_keyword_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/attributes_identifiers_by_keyword_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/attributes_names_by_keyword_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/file_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/file_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/max_nested_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/max_nested_value_by_key_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/max_nested_value_by_type.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/search_by_taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_attributes_by_taxon_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_by_any_name.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_by_name.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_by_specific_name.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_names_by_root.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/taxonomy_node_by_taxon_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/scripts/value_by_type_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/taxon.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/taxonomy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/wikidata.names.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/window_full.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-12 15:59:23.000000 genomehubs-2.7.7/src/genomehubs/templates/window_stats.types.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:59:54.896431 genomehubs-2.7.7/src/genomehubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-12 15:59:54.000000 genomehubs-2.7.7/src/genomehubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-12 15:59:54.000000 genomehubs-2.7.7/src/genomehubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:59:54.000000 genomehubs-2.7.7/src/genomehubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-12 15:59:54.000000 genomehubs-2.7.7/src/genomehubs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-12 15:59:54.000000 genomehubs-2.7.7/src/genomehubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 15:59:54.000000 genomehubs-2.7.7/src/genomehubs.egg-info/top_level.txt
```

### Comparing `genomehubs-2.7.6/CONTRIBUTING.rst` & `genomehubs-2.7.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/LICENSE` & `genomehubs-2.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/PKG-INFO` & `genomehubs-2.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomehubs
-Version: 2.7.6
+Version: 2.7.7
 Summary: GenomeHubs
 Home-page: https://github.com/genomehubs/genomehubs
 Author: genomehubs
 Author-email: genomehubs@genomehubs.org
 Project-URL: Bug Reports, https://github.com/genomehubs/genomehubs/issues
 Project-URL: Source, https://github.com/genomehubs/genomehubs
 Keywords: bioinformatics
```

### Comparing `genomehubs-2.7.6/README.rst` & `genomehubs-2.7.7/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     :alt: Install with Conda
     :target: https://anaconda.org/tolkit/genomehubs
 
 .. |platforms| image:: https://anaconda.org/tolkit/genomehubs/badges/platforms.svg
     :alt: Conda platforms
     :target: https://anaconda.org/tolkit/genomehubs
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/genomehubs/genomehubs/2.7.6.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/genomehubs/genomehubs/2.7.7.svg
     :alt: Commits since latest release
-    :target: https://github.com/genomehubs/genomehubs/compare/2.7.6...main
+    :target: https://github.com/genomehubs/genomehubs/compare/2.7.7...main
 
 .. |license| image:: https://anaconda.org/tolkit/genomehubs/badges/license.svg
     :alt: MIT License
     :target: https://anaconda.org/tolkit/genomehubs
 
 .. end-badges
```

### Comparing `genomehubs-2.7.6/setup.cfg` & `genomehubs-2.7.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/setup.py` & `genomehubs-2.7.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="genomehubs",  # Required
-    version="2.7.6",
+    version="2.7.7",
     description="GenomeHubs",  # Optional
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
```

### Comparing `genomehubs-2.7.6/src/genomehubs/config/dist.config.yaml` & `genomehubs-2.7.7/src/genomehubs/config/dist.config.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/genomehubs.py` & `genomehubs-2.7.7/src/genomehubs/genomehubs.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/attributes.py` & `genomehubs-2.7.7/src/genomehubs/lib/attributes.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/btk.py` & `genomehubs-2.7.7/src/genomehubs/lib/btk.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/busco.py` & `genomehubs-2.7.7/src/genomehubs/lib/busco.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/config.py` & `genomehubs-2.7.7/src/genomehubs/lib/config.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/directory.py` & `genomehubs-2.7.7/src/genomehubs/lib/directory.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/es_functions.py` & `genomehubs-2.7.7/src/genomehubs/lib/es_functions.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/files.py` & `genomehubs-2.7.7/src/genomehubs/lib/files.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/fill.py` & `genomehubs-2.7.7/src/genomehubs/lib/fill.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/gbif.py` & `genomehubs-2.7.7/src/genomehubs/lib/gbif.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/geo.py` & `genomehubs-2.7.7/src/genomehubs/lib/geo.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/hub.py` & `genomehubs-2.7.7/src/genomehubs/lib/hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,17 @@
 from operator import sub
 from operator import truediv
 from pathlib import Path
 
 from tolkein import tofile
 from tolkein import tolog
 
-from .es_functions import query_flexible_template
-
 LOGGER = tolog.logger(__name__)
-MIN_INTEGER = -(2 ** 31)
-MAX_INTEGER = 2 ** 31 - 1
+MIN_INTEGER = -(2**31)
+MAX_INTEGER = 2**31 - 1
 DATE = re.compile(r"^[12]\d{3}-[01]\d-[0123]\d$")
 
 
 def setup(opts):
     """Set up directory for this GenomeHubs instance and handle reset."""
     Path(opts["hub-path"]).mkdir(parents=True, exist_ok=True)
     return True
@@ -342,26 +340,57 @@
         if operator in operators:
             try:
                 return operators[operator](calculate(left), calculate(right))
             except TypeError:
                 return None
 
 
+def attribute_value_query(es, index, opts=None):
+    """Run attribute value query."""
+    query = {
+        "bool": {
+            "filter": [
+                {"match": {opts["id_field"]: opts["primary_id"]}},
+                {
+                    "nested": {
+                        "path": "attributes",
+                        "query": {
+                            "bool": {
+                                "filter": [
+                                    {"match": {"attributes.key": opts["attribute"]}}
+                                ]
+                            }
+                        },
+                        "inner_hits": {
+                            "_source": False,
+                            "name": "%s_values" % opts["attribute"],
+                            "docvalue_fields": [
+                                "attributes.key",
+                                "attributes.%s_value" % opts["value_type"],
+                            ],
+                        },
+                    }
+                },
+            ]
+        }
+    }
+    return es.search(index=index, body={"query": query, "_source": False})
+
+
 def lookup_attribute_value(identifier, attribute, shared_values):
     """Lookup an indexed attribute value."""
     value_type = shared_values["_types"]["attributes"][attribute]["type"]
     opts = {
         "id_field": f'{shared_values["_index_type"]}_id',
         "primary_id": identifier,
         "attribute": attribute,
         "value_type": value_type,
     }
-    res = query_flexible_template(
+    res = attribute_value_query(
         shared_values["_es"],
-        "attribute_value_by_primary_id",
         shared_values["_index"],
         opts,
     )
     hits = res["hits"]["hits"]
     try:
         if len(hits) == 1:
             inner_hits = hits[0]["inner_hits"][f"{attribute}_values"]["hits"]["hits"]
@@ -634,22 +663,21 @@
                 else:
                     existing.append({"key": entry["key"], "values": arr})
                     indices[entry["key"]] = index
                     index += 1
                 del entry["key"]
                 arr.append(entry)
             else:
-                existing.append(
-                    {
-                        **entry,
-                        "count": 1,
-                        # "aggregation_method": "unique",
-                        # "aggregation_source": "direct",
-                    }
-                )
+                mod_entry = {**entry, "count": 1}
+                if "keyword_value" in entry:
+                    if isinstance(mod_entry["keyword_value"], list):
+                        mod_entry["length"] = len(mod_entry["keyword_value"])
+                    else:
+                        mod_entry["length"] = 1
+                existing.append(mod_entry)
 
 
 def strip_comments(data, types):
     """Strip comment lines from a file stream."""
     comment_chars = {"#"}
     if "file" in types and "comment" in types["file"]:
         comment_chars.update(set(types["file"]["comment"]))
@@ -1004,15 +1032,15 @@
         for key, new_key in matched_keys.items():
             if new_key != key:
                 item[new_key] = item[key]
                 del item[key]
     elif isinstance(item, list):
         item = [do_replace(value, arr) for value in item]
     elif isinstance(item, str):
-        for (query, replace) in arr:
+        for query, replace in arr:
             new_item = item.replace(query, str(replace))
             if new_item != item:
                 item = new_item
     return item
 
 
 def deep_replace(obj, arr):
```

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/index.py` & `genomehubs-2.7.7/src/genomehubs/lib/index.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/init.py` & `genomehubs-2.7.7/src/genomehubs/lib/init.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/ncbi.py` & `genomehubs-2.7.7/src/genomehubs/lib/ncbi.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/parse.py` & `genomehubs-2.7.7/src/genomehubs/lib/parse.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/run.py` & `genomehubs-2.7.7/src/genomehubs/lib/run.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/sample.py` & `genomehubs-2.7.7/src/genomehubs/lib/sample.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/search.py` & `genomehubs-2.7.7/src/genomehubs/lib/search.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/taxon.py` & `genomehubs-2.7.7/src/genomehubs/lib/taxon.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/taxonomy.py` & `genomehubs-2.7.7/src/genomehubs/lib/taxonomy.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/test.py` & `genomehubs-2.7.7/src/genomehubs/lib/test.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/validate.py` & `genomehubs-2.7.7/src/genomehubs/lib/validate.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/wikidata.py` & `genomehubs-2.7.7/src/genomehubs/lib/wikidata.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/lib/window.py` & `genomehubs-2.7.7/src/genomehubs/lib/window.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/ATTR_assembly.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/ATTR_assembly.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/ATTR_btk.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/ATTR_btk.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/ATTR_busco.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/ATTR_busco.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/ATTR_feature.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/ATTR_feature.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/ATTR_sample.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/ATTR_sample.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/ATTR_window_stats.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/ATTR_window_stats.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/TAXON_assembly.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/TAXON_assembly.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/analysis.json` & `genomehubs-2.7.7/src/genomehubs/templates/analysis.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/assembly.json` & `genomehubs-2.7.7/src/genomehubs/templates/assembly.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999879436728395%*

 * *Differences: {"'mappings'": "{'properties': {'attributes': {'properties': {'length': OrderedDict([('type', "*

 * *               "'integer'), ('meta', OrderedDict([('description', 'Number of values in "*

 * *               "list')]))])}}}}"}*

```diff
@@ -142,14 +142,20 @@
                         "ignore_above": 64,
                         "meta": {
                             "description": "Value of type keyword (including ontology terms)"
                         },
                         "normalizer": "lowercase",
                         "type": "keyword"
                     },
+                    "length": {
+                        "meta": {
+                            "description": "Number of values in list"
+                        },
+                        "type": "integer"
+                    },
                     "long_value": {
                         "meta": {
                             "description": "Value of type long"
                         },
                         "type": "long"
                     },
                     "max": {
```

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/assembly.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/assembly.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/attributes.json` & `genomehubs-2.7.7/src/genomehubs/templates/attributes.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/btk.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/btk.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/busco.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/busco.types.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,17 @@
   order:
     - <<lineage>>_odb10_complete
     - <<lineage>>_odb10_fragmented
     - <<lineage>>_odb10_missing
   separator: ","
   source_url_stub: https://blobtoolkit.genomehubs.org
   source: BlobToolKit
+  summary: list
   type: keyword
+  default_summary: length
   taxon_summary: ordered_list
   taxon_traverse: ordered_list
   taxon_traverse_direction: up
   taxon_traverse_limit: <<lineage>>
   taxon_display_level: 2
 taxonomy:
   taxon_id:
```

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/busco_feature.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/busco_feature.types.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 file:
   format: tsv
   header: true
   name: <<accession>>.<<lineage>>.full_table.tsv.gz
   needs:
     - ATTR_busco.types.yaml
+    - ATTR_ancestral_unit.types.yaml
     - <<accession>>.window_stats.types.yaml
   source: BlobToolKit
   source_url: https://blobtoolkit.genomehubs.org/view/dataset/<<blobtoolkit_id>>
 analysis:
   analysis_id: busco5-<<lineage>>-<<accession>>
   assembly_id: <<accession>>
   taxon_id: "<<taxon_id>>"
@@ -60,10 +61,9 @@
     header: buscoId
   busco_status:
     header: status
   busco_score:
     header: score
   analysis_name:
     default: BUSCO_<<lineage>>
-  # ancestral_unit:
-  #   index: 0
-  # include merian/nigon translation
+  ancestral_unit:
+    header: buscoId
```

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/feature.json` & `genomehubs-2.7.7/src/genomehubs/templates/feature.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/file.json` & `genomehubs-2.7.7/src/genomehubs/templates/file.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/identifiers.json` & `genomehubs-2.7.7/src/genomehubs/templates/identifiers.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/organelle.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/organelle.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/sample.json` & `genomehubs-2.7.7/src/genomehubs/templates/sample.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/sample.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/sample.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/assembly_lookup.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/assembly_lookup.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/assembly_suggest.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/assembly_suggest.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/attribute_values_by_taxon.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/attribute_values_by_taxon.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/max_nested_value_by_type.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/max_nested_value_by_type.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_any_name.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_by_any_name.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_lineage.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_name.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_by_name.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_by_specific_name.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_by_specific_name.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_lookup.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_lookup.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/taxon_suggest.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/taxon_suggest.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/scripts/value_by_type_by_lineage.json` & `genomehubs-2.7.7/src/genomehubs/templates/scripts/value_by_type_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/taxon.json` & `genomehubs-2.7.7/src/genomehubs/templates/taxon.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/taxon.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/taxon.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/taxonomy.json` & `genomehubs-2.7.7/src/genomehubs/templates/taxonomy.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/window_full.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/window_full.types.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 features:
   assembly_id: <<accession>>
   feature_id:
     header: sequence
   primary_type: <<level>>
 taxonomy:
   taxon_id: <<taxon_id>>
+identifiers:
+  genbank_accession:
+    header: sequence
+  assigned_name:
+    header: assigned_name
 attributes:
   sequence_id:
     header: sequence
   feature_type:
     default:
       - <<level>>
       - toplevel
```

### Comparing `genomehubs-2.7.6/src/genomehubs/templates/window_stats.types.yaml` & `genomehubs-2.7.7/src/genomehubs/templates/window_stats.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.6/src/genomehubs.egg-info/PKG-INFO` & `genomehubs-2.7.7/src/genomehubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomehubs
-Version: 2.7.6
+Version: 2.7.7
 Summary: GenomeHubs
 Home-page: https://github.com/genomehubs/genomehubs
 Author: genomehubs
 Author-email: genomehubs@genomehubs.org
 Project-URL: Bug Reports, https://github.com/genomehubs/genomehubs/issues
 Project-URL: Source, https://github.com/genomehubs/genomehubs
 Keywords: bioinformatics
```

### Comparing `genomehubs-2.7.6/src/genomehubs.egg-info/SOURCES.txt` & `genomehubs-2.7.7/src/genomehubs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 src/genomehubs/lib/taxon.py
 src/genomehubs/lib/taxonomy.py
 src/genomehubs/lib/test.py
 src/genomehubs/lib/validate.py
 src/genomehubs/lib/version.py
 src/genomehubs/lib/wikidata.py
 src/genomehubs/lib/window.py
+src/genomehubs/templates/ATTR_ancestral_unit.types.yaml
 src/genomehubs/templates/ATTR_assembly.types.yaml
 src/genomehubs/templates/ATTR_btk.types.yaml
 src/genomehubs/templates/ATTR_busco.types.yaml
 src/genomehubs/templates/ATTR_feature.types.yaml
 src/genomehubs/templates/ATTR_sample.types.yaml
 src/genomehubs/templates/ATTR_window_stats.types.yaml
 src/genomehubs/templates/TAXON_assembly.types.yaml
```


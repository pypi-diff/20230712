# Comparing `tmp/Marl-Factory-Grid-0.0.9.tar.gz` & `tmp/Marl-Factory-Grid-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Marl-Factory-Grid-0.0.9.tar", last modified: Wed Jun 21 09:40:11 2023, max compression
+gzip compressed data, was "Marl-Factory-Grid-0.1.1.tar", last modified: Wed Jul 12 14:00:26 2023, max compression
```

## Comparing `Marl-Factory-Grid-0.0.9.tar` & `Marl-Factory-Grid-0.1.1.tar`

### file list

```diff
@@ -1,167 +1,188 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4376 2023-06-21 09:40:11.000000 Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6209 2023-06-21 09:40:11.000000 Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 09:40:11.000000 Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 09:40:11.000000 Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 09:40:11.000000 Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4376 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3673 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/_quickstart/
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/_quickstart/all_test_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/images/
--rw-rw-rw-   0 root         (0) root         (0)   303396 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/images/Hooks_FIKS.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/marl_factory_grid/
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8710 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/base_ac.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/example_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/iac.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/mappo.py
--rw-rw-rw-   0 root         (0) root         (0)     7763 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/memory.py
--rw-rw-rw-   0 root         (0) root         (0)     4784 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/networks.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/seac.py
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/snac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/
--rw-rw-rw-   0 root         (0) root         (0)     5337 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/TSP_base_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/TSP_dirt_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/TSP_item_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/TSP_target_agent.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/random_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2687 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/default_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2633 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8521 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/adversary.png
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/agent.png
--rw-rw-rw-   0 root         (0) root         (0)    18857 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/agent_collision.png
--rw-rw-rw-   0 root         (0) root         (0)     1631 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/idle.png
--rw-rw-rw-   0 root         (0) root         (0)     1599 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/invalid.png
--rw-rw-rw-   0 root         (0) root         (0)     5933 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/move.png
--rw-rw-rw-   0 root         (0) root         (0)     5717 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/valid.png
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/wall.png
--rw-rw-rw-   0 root         (0) root         (0)     2766 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2380 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2175 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/entity.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3320 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/object.py
--rw-rw-rw-   0 root         (0) root         (0)     1240 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/util.py
--rw-rw-rw-   0 root         (0) root         (0)     3123 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/wall_floor.py
--rw-rw-rw-   0 root         (0) root         (0)     6943 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/agents.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/env_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     2056 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/global_entities.py
--rw-rw-rw-   0 root         (0) root         (0)     2910 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     3902 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/objects.py
--rw-rw-rw-   0 root         (0) root         (0)     2399 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/wall_n_floors.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     2537 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/logging/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2244 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/logging/envmonitor.py
--rw-rw-rw-   0 root         (0) root         (0)     5474 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/logging/recorder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/_template/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/_template/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/_template/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/_template/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1103 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2426 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     2135 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1319 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    39296 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/dirtpiles.png
--rw-rw-rw-   0 root         (0) root         (0)     1180 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)     2611 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/rule_done_on_all_clean.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/rule_respawn.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/rule_smear_on_move.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      948 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/destinations.png
--rw-rw-rw-   0 root         (0) root         (0)     1813 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     3728 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/door_closed.png
--rw-rw-rw-   0 root         (0) root         (0)     4224 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/door_open.png
--rw-rw-rw-   0 root         (0) root         (0)     2740 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/rule_door_auto_close.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/assets/
--rw-rw-rw-   0 root         (0) root         (0)     6610 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/assets/charge_pod.png
--rw-rw-rw-   0 root         (0) root         (0)     2318 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/assets/dropofflocations.png
--rw-rw-rw-   0 root         (0) root         (0)     3102 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/assets/items.png
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2074 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)     3173 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     3153 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/levels/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/levels/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1511 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/levels/large.txt
--rw-rw-rw-   0 root         (0) root         (0)     5827 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/levels/large_qquad.txt
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/levels/rooms.txt
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/levels/shelves.txt
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/levels/simple.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1898 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/marl_factory_grid/plotting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/plotting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8652 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/plotting/compare_runs.py
--rw-rw-rw-   0 root         (0) root         (0)     2967 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/plotting/plotting.py
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/quickstart.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5309 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/config_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    10888 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/level_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    12499 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/observation_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/render.py
--rw-rw-rw-   0 root         (0) root         (0)     5765 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/renderer.py
--rw-rw-rw-   0 root         (0) root         (0)     1114 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/results.py
--rw-rw-rw-   0 root         (0) root         (0)     3625 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/states.py
--rw-rw-rw-   0 root         (0) root         (0)     5673 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/tools.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/utility_classes.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.689568 Marl-Factory-Grid-0.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.677569 Marl-Factory-Grid-0.1.1/Marl_Factory_Grid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-07-12 14:00:26.000000 Marl-Factory-Grid-0.1.1/Marl_Factory_Grid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7002 2023-07-12 14:00:26.000000 Marl-Factory-Grid-0.1.1/Marl_Factory_Grid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 14:00:26.000000 Marl-Factory-Grid-0.1.1/Marl_Factory_Grid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 14:00:26.000000 Marl-Factory-Grid-0.1.1/Marl_Factory_Grid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-12 14:00:26.000000 Marl-Factory-Grid-0.1.1/Marl_Factory_Grid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-07-12 14:00:26.689568 Marl-Factory-Grid-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3673 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.677569 Marl-Factory-Grid-0.1.1/_quickstart/
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/_quickstart/all_test_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.677569 Marl-Factory-Grid-0.1.1/images/
+-rw-rw-rw-   0 root         (0) root         (0)   303396 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/images/Hooks_FIKS.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.677569 Marl-Factory-Grid-0.1.1/marl_factory_grid/
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.677569 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.677569 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8710 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/base_ac.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/example_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/iac.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/mappo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7763 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/memory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4784 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/networks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/seac.py
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/snac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.681568 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/static/
+-rw-rw-rw-   0 root         (0) root         (0)     3705 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/static/TSP_base_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/static/TSP_dirt_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/static/TSP_item_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/static/TSP_target_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/static/random_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/static/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2687 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.681568 Marl-Factory-Grid-0.1.1/marl_factory_grid/configs/
+-rw-rw-rw-   0 root         (0) root         (0)     1582 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/configs/default_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      762 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/configs/two_rooms_one_door.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.681568 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.681568 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.681568 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/agent/
+-rw-rw-rw-   0 root         (0) root         (0)     8521 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/agent/adversary.png
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/agent/agent.png
+-rw-rw-rw-   0 root         (0) root         (0)    18857 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/agent/agent_collision.png
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/agent/idle.png
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/agent/invalid.png
+-rw-rw-rw-   0 root         (0) root         (0)     5933 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/agent/move.png
+-rw-rw-rw-   0 root         (0) root         (0)     5717 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/agent/valid.png
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/wall.png
+-rw-rw-rw-   0 root         (0) root         (0)     2672 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.681568 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/entity/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/entity/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2659 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/entity/agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2315 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/entity/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)      399 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/entity/mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/entity/object.py
+-rw-rw-rw-   0 root         (0) root         (0)     1232 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/entity/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3060 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/entity/wall_floor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7447 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.681568 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/agents.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/env_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2210 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/global_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     3053 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2467 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1594 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/wall_n_floors.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     2949 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.681568 Marl-Factory-Grid-0.1.1/marl_factory_grid/logging/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/logging/envmonitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5474 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/logging/recorder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.681568 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.681568 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/_template/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/_template/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/_template/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/_template/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.681568 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/batteries/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/batteries/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/batteries/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/batteries/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2426 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/batteries/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/batteries/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/batteries/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     2134 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/batteries/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.685568 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1319 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      150 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    39296 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/dirtpiles.png
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)     2601 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/rule_done_on_all_clean.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/rule_respawn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/rule_smear_on_move.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.685568 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/destinations/
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/destinations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/destinations/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/destinations/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/destinations/destinations.png
+-rw-rw-rw-   0 root         (0) root         (0)     2574 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/destinations/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/destinations/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/destinations/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     3737 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/destinations/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.685568 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      699 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/door_closed.png
+-rw-rw-rw-   0 root         (0) root         (0)     4224 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/door_open.png
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/rule_door_auto_close.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.685568 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/factory/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/factory/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      972 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/factory/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.685568 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.685568 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/assets/
+-rw-rw-rw-   0 root         (0) root         (0)     6610 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/assets/charge_pod.png
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/assets/dropofflocations.png
+-rw-rw-rw-   0 root         (0) root         (0)     3102 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/assets/items.png
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2374 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)     2780 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     3144 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.685568 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/levels/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/levels/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1511 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/levels/large.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5827 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/levels/large_qquad.txt
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/levels/rooms.txt
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/levels/shelves.txt
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/levels/simple.txt
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/levels/two_rooms.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.685568 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/machines/
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/machines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/machines/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/machines/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2128 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/machines/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/machines/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     8729 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/machines/machine.png
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/machines/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/machines/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.689568 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/maintenance/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/maintenance/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/maintenance/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3600 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/maintenance/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/maintenance/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)    22988 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/maintenance/maintainer.png
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/maintenance/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/maintenance/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.689568 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/zones/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/zones/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      150 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/zones/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      733 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/zones/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/zones/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/zones/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.689568 Marl-Factory-Grid-0.1.1/marl_factory_grid/plotting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/plotting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8652 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/plotting/compare_runs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2967 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/plotting/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/quickstart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:00:26.689568 Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5864 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/config_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    10666 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2733 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/level_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    11989 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/observation_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/render.py
+-rw-rw-rw-   0 root         (0) root         (0)     5681 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/results.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/states.py
+-rw-rw-rw-   0 root         (0) root         (0)     5719 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/utility_classes.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 14:00:26.689568 Marl-Factory-Grid-0.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-07-12 14:00:19.000000 Marl-Factory-Grid-0.1.1/setup.py
```

### Comparing `Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/PKG-INFO` & `Marl-Factory-Grid-0.1.1/Marl_Factory_Grid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Marl-Factory-Grid
-Version: 0.0.9
+Version: 0.1.1
 Summary: A framework to research MARL agents in various setings.
 Home-page: https://github.com/illiumst/marl-factory-grid/import
 Author: Steffen Illium
 Author-email: steffen.illium@ifi.lmu.de
 License: MIT
 Keywords: artificial intelligence,pytorch,multiagent reinforcement learning,simulation,emergence,gymnasium,environment,deepdiff,natsort
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/SOURCES.txt` & `Marl-Factory-Grid-0.1.1/Marl_Factory_Grid.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 Marl_Factory_Grid.egg-info/SOURCES.txt
 Marl_Factory_Grid.egg-info/dependency_links.txt
 Marl_Factory_Grid.egg-info/requires.txt
 Marl_Factory_Grid.egg-info/top_level.txt
 _quickstart/all_test_config.yaml
 images/Hooks_FIKS.png
 marl_factory_grid/__init__.py
-marl_factory_grid/default_config.yaml
 marl_factory_grid/quickstart.py
 marl_factory_grid/algorithms/__init__.py
 marl_factory_grid/algorithms/utils.py
 marl_factory_grid/algorithms/marl/__init__.py
 marl_factory_grid/algorithms/marl/base_ac.py
 marl_factory_grid/algorithms/marl/example_config.yaml
 marl_factory_grid/algorithms/marl/iac.py
@@ -25,23 +24,24 @@
 marl_factory_grid/algorithms/marl/snac.py
 marl_factory_grid/algorithms/static/TSP_base_agent.py
 marl_factory_grid/algorithms/static/TSP_dirt_agent.py
 marl_factory_grid/algorithms/static/TSP_item_agent.py
 marl_factory_grid/algorithms/static/TSP_target_agent.py
 marl_factory_grid/algorithms/static/__init__.py
 marl_factory_grid/algorithms/static/random_agent.py
+marl_factory_grid/algorithms/static/utils.py
+marl_factory_grid/configs/default_config.yaml
+marl_factory_grid/configs/two_rooms_one_door.yaml
 marl_factory_grid/environment/__init__.py
 marl_factory_grid/environment/actions.py
 marl_factory_grid/environment/constants.py
 marl_factory_grid/environment/factory.py
 marl_factory_grid/environment/rewards.py
 marl_factory_grid/environment/rules.py
-marl_factory_grid/environment/assets/__init__.py
 marl_factory_grid/environment/assets/wall.png
-marl_factory_grid/environment/assets/agent/__init__.py
 marl_factory_grid/environment/assets/agent/adversary.png
 marl_factory_grid/environment/assets/agent/agent.png
 marl_factory_grid/environment/assets/agent/agent_collision.png
 marl_factory_grid/environment/assets/agent/idle.png
 marl_factory_grid/environment/assets/agent/invalid.png
 marl_factory_grid/environment/assets/agent/move.png
 marl_factory_grid/environment/assets/agent/valid.png
@@ -97,14 +97,16 @@
 marl_factory_grid/modules/doors/constants.py
 marl_factory_grid/modules/doors/door_closed.png
 marl_factory_grid/modules/doors/door_open.png
 marl_factory_grid/modules/doors/entitites.py
 marl_factory_grid/modules/doors/groups.py
 marl_factory_grid/modules/doors/rewards.py
 marl_factory_grid/modules/doors/rule_door_auto_close.py
+marl_factory_grid/modules/factory/__init__.py
+marl_factory_grid/modules/factory/rules.py
 marl_factory_grid/modules/items/__init__.py
 marl_factory_grid/modules/items/actions.py
 marl_factory_grid/modules/items/constants.py
 marl_factory_grid/modules/items/entitites.py
 marl_factory_grid/modules/items/groups.py
 marl_factory_grid/modules/items/rewards.py
 marl_factory_grid/modules/items/rules.py
@@ -113,20 +115,35 @@
 marl_factory_grid/modules/items/assets/items.png
 marl_factory_grid/modules/levels/__init__.py
 marl_factory_grid/modules/levels/large.txt
 marl_factory_grid/modules/levels/large_qquad.txt
 marl_factory_grid/modules/levels/rooms.txt
 marl_factory_grid/modules/levels/shelves.txt
 marl_factory_grid/modules/levels/simple.txt
+marl_factory_grid/modules/levels/two_rooms.txt
 marl_factory_grid/modules/machines/__init__.py
+marl_factory_grid/modules/machines/actions.py
 marl_factory_grid/modules/machines/constants.py
 marl_factory_grid/modules/machines/entitites.py
 marl_factory_grid/modules/machines/groups.py
+marl_factory_grid/modules/machines/machine.png
 marl_factory_grid/modules/machines/rewards.py
 marl_factory_grid/modules/machines/rules.py
+marl_factory_grid/modules/maintenance/__init__.py
+marl_factory_grid/modules/maintenance/constants.py
+marl_factory_grid/modules/maintenance/entities.py
+marl_factory_grid/modules/maintenance/groups.py
+marl_factory_grid/modules/maintenance/maintainer.png
+marl_factory_grid/modules/maintenance/rewards.py
+marl_factory_grid/modules/maintenance/rules.py
+marl_factory_grid/modules/zones/__init__.py
+marl_factory_grid/modules/zones/constants.py
+marl_factory_grid/modules/zones/entitites.py
+marl_factory_grid/modules/zones/groups.py
+marl_factory_grid/modules/zones/rules.py
 marl_factory_grid/plotting/__init__.py
 marl_factory_grid/plotting/compare_runs.py
 marl_factory_grid/plotting/plotting.py
 marl_factory_grid/utils/__init__.py
 marl_factory_grid/utils/config_parser.py
 marl_factory_grid/utils/helpers.py
 marl_factory_grid/utils/level_parser.py
```

### Comparing `Marl-Factory-Grid-0.0.9/PKG-INFO` & `Marl-Factory-Grid-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Marl-Factory-Grid
-Version: 0.0.9
+Version: 0.1.1
 Summary: A framework to research MARL agents in various setings.
 Home-page: https://github.com/illiumst/marl-factory-grid/import
 Author: Steffen Illium
 Author-email: steffen.illium@ifi.lmu.de
 License: MIT
 Keywords: artificial intelligence,pytorch,multiagent reinforcement learning,simulation,emergence,gymnasium,environment,deepdiff,natsort
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Marl-Factory-Grid-0.0.9/README.md` & `Marl-Factory-Grid-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/_quickstart/all_test_config.yaml` & `Marl-Factory-Grid-0.1.1/_quickstart/all_test_config.yaml`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/images/Hooks_FIKS.png` & `Marl-Factory-Grid-0.1.1/images/Hooks_FIKS.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/base_ac.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/base_ac.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/example_config.yaml` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/example_config.yaml`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/iac.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/iac.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/mappo.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/mappo.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/memory.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/memory.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/networks.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/networks.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/seac.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/seac.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/snac.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/marl/snac.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/TSP_dirt_agent.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/static/TSP_dirt_agent.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/TSP_item_agent.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/static/TSP_item_agent.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/TSP_target_agent.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/static/TSP_target_agent.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/utils.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/algorithms/utils.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/actions.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,7 +94,9 @@
     def __init__(self, *args, **kwargs):
         super().__init__(c.NORTHWEST, *args, **kwargs)
 
 
 Move4 = [North, East, South, West]
 # noinspection PyTypeChecker
 Move8 = Move4 + [NorthEast, SouthEast, SouthWest, NorthWest]
+
+ALL_BASEACTIONS = Move8 + [Noop]
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/adversary.png` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/agent/adversary.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/agent.png` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/agent/agent.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/agent_collision.png` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/agent/agent_collision.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/idle.png` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/agent/idle.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/invalid.png` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/agent/invalid.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/move.png` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/agent/move.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/valid.png` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/agent/valid.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/wall.png` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/assets/wall.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/constants.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # Names
 DANGER_ZONE             = 'x'                   # Dange Zone tile _identifier for resolving the string based map files.
 DEFAULTS                = 'Defaults'
 SELF                    = 'Self'
 PLACEHOLDER             = 'Placeholder'
 FLOOR                   = 'Floor'               # Identifier of Floor-objects and groups (groups).
-FLOORS                  = 'Floors'               # Identifier of Floor-objects and groups (groups).
+FLOORS                  = 'Floors'              # Identifier of Floor-objects and groups (groups).
 WALL                    = 'Wall'                # Identifier of Wall-objects and groups (groups).
 WALLS                   = 'Walls'               # Identifier of Wall-objects and groups (groups).
 LEVEL                   = 'Level'               # Identifier of Level-objects and groups (groups).
 AGENT                   = 'Agent'               # Identifier of Agent-objects and groups (groups).
-AGENTS                  = 'Agents'              # Identifier of Agent-objects and groups (groups).
 OTHERS                  = 'Other'
 COMBINED                = 'Combined'
-GLOBAL_POSITION         = 'GLOBAL_POSITION'     # Identifier of the global position slice
-
+GLOBALPOSITIONS        = 'GlobalPositions'     # Identifier of the global position slice
 
 # Attributes
-IS_BLOCKING_LIGHT       = 'is_blocking_light'
-HAS_POSITION            = 'has_position'
+IS_BLOCKING_LIGHT       = 'var_is_blocking_light'
+HAS_POSITION            = 'var_has_position'
 HAS_NO_POSITION         = 'has_no_position'
 ALL                     = 'All'
 
 # Symbols (Read from map-files)
 SYMBOL_WALL             = '#'
 SYMBOL_FLOOR            = '-'
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/agent.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/entity/agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,51 @@
 from typing import List, Union
 
-from marl_factory_grid.environment import constants as c
 from marl_factory_grid.environment.actions import Action
 from marl_factory_grid.environment.entity.entity import Entity
 from marl_factory_grid.utils.render import RenderEntity
 from marl_factory_grid.utils import renderer
 from marl_factory_grid.utils.helpers import is_move
 from marl_factory_grid.utils.results import ActionResult, Result
 
+from marl_factory_grid.environment import constants as c
+
 
 class Agent(Entity):
 
     @property
+    def var_is_blocking_light(self):
+        return False
+
+    @property
+    def var_can_move(self):
+        return True
+
+    @property
+    def var_is_blocking_pos(self):
+        return False
+
+    @property
+    def var_has_position(self):
+        return True
+
+    @property
     def obs_tag(self):
         return self.name
 
     @property
     def actions(self):
         return self._actions
 
     @property
     def observations(self):
         return self._observations
 
     @property
-    def can_collide(self):
+    def var_can_collide(self):
         return True
 
     def step_result(self):
         pass
 
     @property
     def collection(self):
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/entity.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/entity/entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import abc
 
-from marl_factory_grid.environment import constants as c
-from marl_factory_grid.environment.entity.object import EnvObject
-from marl_factory_grid.utils.render import RenderEntity
+from .. import constants as c
+from .object import EnvObject
+from ...utils.render import RenderEntity
+from ...utils.results import ActionResult
 
 
 class Entity(EnvObject, abc.ABC):
     """Full Env Entity that lives on the environment Grid. Doors, Items, DirtPile etc..."""
 
     @property
-    def has_position(self):
+    def state(self):
+        return self._status or ActionResult(entity=self, identifier=c.NOOP, validity=c.VALID, reward=0)
+
+    @property
+    def var_has_position(self):
         return self.pos != c.VALUE_NO_POS
 
     @property
     def x(self):
         return self.pos[0]
 
     @property
@@ -60,20 +65,21 @@
                 for observer in self.observers:
                     observer.notify_change_pos(self)
             return valid
         return not_same_tile
 
     def __init__(self, tile, **kwargs):
         super().__init__(**kwargs)
+        self._status = None
         self._tile = tile
         tile.enter(self)
 
     def summarize_state(self) -> dict:
         return dict(name=str(self.name), x=int(self.x), y=int(self.y),
-                    tile=str(self.tile.name), can_collide=bool(self.can_collide))
+                    tile=str(self.tile.name), can_collide=bool(self.var_can_collide))
 
     @abc.abstractmethod
     def render(self):
         return RenderEntity(self.__class__.__name__.lower(), self.pos)
 
     def __repr__(self):
         return super(Entity, self).__repr__() + f'(@{self.pos})'
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/object.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/entity/object.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,27 +17,31 @@
     def observers(self):
         return self._observers
 
     @property
     def name(self):
         if self._str_ident is not None:
             return f'{self.__class__.__name__}[{self._str_ident}]'
-        return f'{self.__class__.__name__}#{self.identifier_int}'
+        return f'{self.__class__.__name__}#{self.u_int}'
 
     @property
     def identifier(self):
         if self._str_ident is not None:
             return self._str_ident
         else:
             return self.name
 
+    def reset_uid(self):
+        self._u_idx = defaultdict(lambda: 0)
+        return True
+
     def __init__(self, str_ident: Union[str, None] = None, **kwargs):
         self._observers = []
         self._str_ident = str_ident
-        self.identifier_int = self._identify_and_count_up()
+        self.u_int = self._identify_and_count_up()
         self._collection = None
 
         if kwargs:
             print(f'Following kwargs were passed, but ignored: {kwargs}')
 
     def __repr__(self):
         return f'{self.name}'
@@ -74,45 +78,45 @@
     def obs_tag(self):
         try:
             return self._collection.name or self.name
         except AttributeError:
             return self.name
 
     @property
-    def is_blocking_light(self):
+    def var_is_blocking_light(self):
         try:
-            return self._collection.is_blocking_light or False
+            return self._collection.var_is_blocking_light or False
         except AttributeError:
             return False
 
     @property
-    def can_move(self):
+    def var_can_move(self):
         try:
-            return self._collection.can_move or False
+            return self._collection.var_can_move or False
         except AttributeError:
             return False
 
     @property
-    def is_blocking_pos(self):
+    def var_is_blocking_pos(self):
         try:
-            return self._collection.is_blocking_pos or False
+            return self._collection.var_is_blocking_pos or False
         except AttributeError:
             return False
 
     @property
-    def has_position(self):
+    def var_has_position(self):
         try:
-            return self._collection.has_position or False
+            return self._collection.var_has_position or False
         except AttributeError:
             return False
 
     @property
-    def can_collide(self):
+    def var_can_collide(self):
         try:
-            return self._collection.can_collide or False
+            return self._collection.var_can_collide or False
         except AttributeError:
             return False
 
     @property
     def encoding(self):
         return c.VALUE_OCCUPIED_CELL
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/util.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/entity/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 class GlobalPosition(BoundEntityMixin, EnvObject):
 
     @property
     def encoding(self):
         if self._normalized:
-            return tuple(np.divide(self._bound_entity.pos, self._level_shape))
+            return tuple(np.divide(self._bound_entity.pos, self._shape))
         else:
             return self.bound_entity.pos
 
-    def __init__(self, *args, normalized: bool = True, **kwargs):
+    def __init__(self, level_shape, *args, normalized: bool = True, **kwargs):
         super(GlobalPosition, self).__init__(*args, **kwargs)
-        self._level_shape = math.sqrt(self.size)
         self._normalized = normalized
+        self._shape = level_shape
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/wall_floor.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/entity/wall_floor.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,38 +7,34 @@
 from marl_factory_grid.utils.render import RenderEntity
 from marl_factory_grid.utils import helpers as h
 
 
 class Floor(EnvObject):
 
     @property
-    def has_position(self):
+    def var_has_position(self):
         return True
 
     @property
-    def can_collide(self):
+    def var_can_collide(self):
         return False
 
     @property
-    def can_move(self):
+    def var_can_move(self):
         return False
 
     @property
-    def is_blocking_pos(self):
+    def var_is_blocking_pos(self):
         return False
 
     @property
-    def is_blocking_light(self):
+    def var_is_blocking_light(self):
         return False
 
     @property
-    def neighboring_floor_pos(self):
-        return [x.pos for x in self.neighboring_floor]
-
-    @property
     def neighboring_floor(self):
         if self._neighboring_floor:
             pass
         else:
             self._neighboring_floor = [x for x in [self._collection.by_pos(np.add(self.pos, pos))
                                                    for pos in h.POS_MASK.reshape(-1, 2)
                                                    if not np.all(pos == [0, 0])]
@@ -47,15 +43,15 @@
 
     @property
     def encoding(self):
         return c.VALUE_OCCUPIED_CELL
 
     @property
     def guests_that_can_collide(self):
-        return [x for x in self.guests if x.can_collide]
+        return [x for x in self.guests if x.var_can_collide]
 
     @property
     def guests(self):
         return self._guests.values()
 
     @property
     def x(self):
@@ -63,15 +59,15 @@
 
     @property
     def y(self):
         return self.pos[1]
 
     @property
     def is_blocked(self):
-        return any([x.is_blocking_pos for x in self.guests])
+        return any([x.var_is_blocking_pos for x in self.guests])
 
     def __init__(self, pos, **kwargs):
         super(Floor, self).__init__(**kwargs)
         self._guests = dict()
         self.pos = tuple(pos)
         self._neighboring_floor: List[Floor] = list()
         self._blocked_by = None
@@ -82,15 +78,15 @@
     def is_empty(self):
         return not len(self._guests)
 
     def is_occupied(self):
         return bool(len(self._guests))
 
     def enter(self, guest):
-        if (guest.name not in self._guests and not self.is_blocked) and not (guest.is_blocking_pos and self.is_occupied()):
+        if (guest.name not in self._guests and not self.is_blocked) and not (guest.var_is_blocking_pos and self.is_occupied()):
             self._guests.update({guest.name: guest})
             return c.VALID
         else:
             return c.NOT_VALID
 
     def leave(self, guest):
         try:
@@ -108,24 +104,24 @@
     def render(self):
         return None
 
 
 class Wall(Floor):
 
     @property
-    def can_collide(self):
+    def var_can_collide(self):
         return True
 
     @property
     def encoding(self):
         return c.VALUE_OCCUPIED_CELL
 
     def render(self):
         return RenderEntity(c.WALL, self.pos)
 
     @property
-    def is_blocking_pos(self):
+    def var_is_blocking_pos(self):
         return True
 
     @property
-    def is_blocking_light(self):
+    def var_is_blocking_light(self):
         return True
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/factory.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import marl_factory_grid.environment.constants as c
 
 from marl_factory_grid.utils.states import Gamestate
 
 REC_TAC = 'rec_'
 
 
-class BaseFactory(gym.Env):
+class Factory(gym.Env):
 
     @property
     def action_space(self):
         return self.state[c.AGENT].action_space
 
     @property
     def named_action_space(self):
@@ -48,19 +48,23 @@
     def summarize_header(self):
         summary_dict = self._summarize_state(stateless_entities=True)
         return summary_dict
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
-    def __init__(self, config_file: Union[str, PathLike]):
+    def __init__(self, config_file: Union[str, PathLike], custom_modules_path: Union[None, PathLike] = None,
+                 custom_level_path: Union[None, PathLike] = None):
         self._config_file = config_file
-        self.conf = FactoryConfigParser(self._config_file)
+        self.conf = FactoryConfigParser(self._config_file, custom_modules_path)
         # Attribute Assignment
-        self.level_filepath = Path(__file__).parent.parent / h.LEVELS_DIR / f'{self.conf.level_name}.txt'
+        if custom_level_path is not None:
+            self.level_filepath = Path(custom_level_path)
+        else:
+            self.level_filepath = Path(__file__).parent.parent / h.LEVELS_DIR / f'{self.conf.level_name}.txt'
         self._renderer = None  # expensive - don't use; unless required !
 
         parsed_entities = self.conf.load_entities()
         self.map = LevelParser(self.level_filepath, parsed_entities, self.conf.pomdp_r)
 
         # Init for later usage:
         self.state: Gamestate
@@ -70,31 +74,38 @@
         # TODO: Reset ---> document this
         self.reset()
 
     def __getitem__(self, item):
         return self.state.entities[item]
 
     def reset(self) -> (dict, dict):
+        if hasattr(self, 'state'):
+            for entity_group in self.state.entities:
+                try:
+                    entity_group[0].reset_uid()
+                except (AttributeError, TypeError):
+                    pass
+
         self.state = None
 
         # Init entity:
         entities = self.map.do_init()
 
-        # Grab all rules:
+        # Grab all )rules:
         rules = self.conf.load_rules()
 
         # Agents
         # noinspection PyAttributeOutsideInit
         self.state = Gamestate(entities, rules, self.conf.env_seed)
 
         agents = self.conf.load_agents(self.map.size, self[c.FLOOR].empty_tiles)
         self.state.entities.add_item({c.AGENT: agents})
 
         # All is set up, trigger additional init (after agent entity spawn etc)
-        self.state.rules.do_all_init(self.state)
+        self.state.rules.do_all_init(self.state, self.map)
 
         # Observations
         # noinspection PyAttributeOutsideInit
         self.obs_builder = OBSBuilder(self.map.level_shape, self.state, self.map.pomdp_r)
         return self.obs_builder.refresh_and_build_for_all(self.state)
 
     def step(self, actions):
@@ -140,15 +151,15 @@
                 assert isinstance(info.value, (float, int))
                 combined_info_dict[info.identifier] += info.value
 
         # Check Done Rule Results
         try:
             done_reason = next(x for x in done_check_results if x.validity)
             done = True
-            self.state.print(f'Env done, Reason: {done_reason.name}.')
+            self.state.print(f'Env done, Reason: {done_reason.identifier}.')
         except StopIteration:
             done = False
 
         if self.conf.individual_rewards:
             global_rewards = rewards['global']
             del rewards['global']
             reward = [rewards[agent.name] for agent in self.state[c.AGENT]]
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/agents.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/agents.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from marl_factory_grid.environment.entity.agent import Agent
 from marl_factory_grid.environment.groups.env_objects import EnvObjects
 from marl_factory_grid.environment.groups.mixins import PositionMixin
-from marl_factory_grid.environment.entity.agent import Agent
 
 
 class Agents(PositionMixin, EnvObjects):
     _entity = Agent
     is_blocking_light = False
     can_move = True
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/env_objects.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/env_objects.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from marl_factory_grid.environment.groups.objects import Objects
 from marl_factory_grid.environment.entity.object import EnvObject
 
 
 class EnvObjects(Objects):
 
     _entity = EnvObject
-    is_blocking_light: bool = False
-    can_collide: bool = False
-    has_position: bool = False
-    can_move: bool = False
+    var_is_blocking_light: bool = False
+    var_can_collide: bool = False
+    var_has_position: bool = False
+    var_can_move: bool = False
 
     @property
     def encodings(self):
         return [x.encoding for x in self]
 
     def __init__(self, size, *args, **kwargs):
         super(EnvObjects, self).__init__(*args, **kwargs)
         self.size = size
 
     def add_item(self, item: EnvObject):
-        assert self.has_position or (len(self) <= self.size)
+        assert self.var_has_position or (len(self) <= self.size)
         super(EnvObjects, self).add_item(item)
         return self
 
     def summarize_states(self):
         return [entity.summarize_state() for entity in self.values()]
 
     def delete_env_object(self, env_object: EnvObject):
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/global_entities.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/global_entities.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,25 +37,31 @@
         assert_str = 'This group of entity has already been added!'
         assert not any([key for key in item.keys() if key in self.keys()]), assert_str
         self._data.update(item)
         for val in item.values():
             val.add_observer(self)
         return self
 
+    def __contains__(self, item):
+        return item in self._data
+
     def __delitem__(self, name):
         assert_str = 'This group of entity does not exist in this collection!'
         assert any([key for key in name.keys() if key in self.keys()]), assert_str
         self[name]._observers.delete(self)
         for entity in self[name]:
             entity.del_observer(self)
         return super(Entities, self).__delitem__(name)
 
     @property
     def obs_pairs(self):
-        return [y for x in self for y in x.obs_pairs]
+        try:
+            return [y for x in self for y in x.obs_pairs]
+        except AttributeError:
+            print('OhOh (debug me)')
 
     def by_pos(self, pos: (int, int)):
         return self.pos_dict[pos]
         # found_entities = [y for y in (x.by_pos(pos) for x in self.values() if hasattr(x, 'by_pos')) if y is not None]
         # return found_entities
 
     @property
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/mixins.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/mixins.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-from marl_factory_grid.environment import constants as c
+from typing import List
 
+from marl_factory_grid.environment import constants as c
 from marl_factory_grid.environment.entity.entity import Entity
+from marl_factory_grid.environment.entity.wall_floor import Floor
 
 
-# noinspection PyUnresolvedReferences,PyTypeChecker,PyArgumentList
 class PositionMixin:
 
     _entity = Entity
-    is_blocking_light: bool = True
-    can_collide: bool = True
-    has_position: bool = True
+    var_is_blocking_light: bool = True
+    var_can_collide: bool = True
+    var_has_position: bool = True
+
+    def spawn(self, tiles: List[Floor]):
+        self.add_items([self._entity(tile) for tile in tiles])
 
     def render(self):
         return [y for y in [x.render() for x in self] if y is not None]
 
     @classmethod
     def from_tiles(cls, tiles, *args, entity_kwargs=None, **kwargs):
         collection = cls(*args, **kwargs)
@@ -74,19 +78,19 @@
         return c.VALID
 
     def belongs_to_entity(self, entity):
         return self._bound_entity == entity
 
 
 # noinspection PyUnresolvedReferences,PyTypeChecker
-class HasBoundedMixin:
+class HasBoundMixin:
 
     @property
-    def obs_names(self):
-        return [x.name for x in self]
+    def obs_pairs(self):
+        return [(x.name, x) for x in self]
 
     def by_entity(self, entity):
         try:
             return next((x for x in self if x.belongs_to_entity(entity)))
         except StopIteration:
             return None
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/objects.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/objects.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections import defaultdict
 from typing import List
 
 import numpy as np
 
 from marl_factory_grid.environment.entity.object import Object
+import marl_factory_grid.environment.constants as c
 
 
 class Objects:
     _entity = Object
 
     @property
     def observers(self):
@@ -32,29 +33,30 @@
 
     @property
     def name(self):
         return f'{self.__class__.__name__}'
 
     def __init__(self, *args, **kwargs):
         self._data = defaultdict(lambda: None)
-        self._observers = list()
+        self._observers = [self]
         self.pos_dict = defaultdict(list)
 
     def __len__(self):
         return len(self._data)
 
     def __iter__(self):
         return iter(self.values())
 
     def add_item(self, item: _entity):
         assert_str = f'All item names have to be of type {self._entity}, but were {item.__class__}.,'
         assert isinstance(item, self._entity), assert_str
         assert self._data[item.name] is None, f'{item.name} allready exists!!!'
         self._data.update({item.name: item})
         item.set_collection(self)
+        # self.notify_add_entity(item)
         for observer in self.observers:
             observer.notify_add_entity(item)
         return self
 
     # noinspection PyUnresolvedReferences
     def del_observer(self, observer):
         self.observers.remove(observer)
@@ -91,16 +93,14 @@
 
     def _get_index(self, item):
         try:
             return next(i for i, v in enumerate(self._data.values()) if v == item)
         except StopIteration:
             return None
 
-
-
     def __getitem__(self, item):
         if isinstance(item, (int, np.int64, np.int32)):
             if item < 0:
                 item = len(self._data) - abs(item)
             try:
                 return next(v for i, v in enumerate(self._data.values()) if i == item)
             except StopIteration:
@@ -112,20 +112,29 @@
         except TypeError:
             print('Ups')
             raise TypeError
 
     def __repr__(self):
         return f'{self.__class__.__name__}[{dict(self._data)}]'
 
+    def spawn(self, n: int):
+        self.add_items([self._entity() for _ in range(n)])
+        return c.VALID
+
+    def despawn(self, items: List[Object]):
+        items = [items] if isinstance(items, Object) else items
+        for item in items:
+            del self[item]
+
     def notify_change_pos(self, entity: object):
         try:
             self.pos_dict[entity.last_pos].remove(entity)
         except (ValueError, AttributeError):
             pass
-        if entity.has_position:
+        if entity.var_has_position:
             try:
                 self.pos_dict[entity.pos].append(entity)
             except (ValueError, AttributeError):
                 pass
 
     def notify_del_entity(self, entity: Object):
         try:
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/utils.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import List, Union
 
 import numpy as np
 
+from marl_factory_grid.environment.entity.util import GlobalPosition
 from marl_factory_grid.environment.groups.env_objects import EnvObjects
+from marl_factory_grid.environment.groups.mixins import PositionMixin, HasBoundMixin
 from marl_factory_grid.environment.groups.objects import Objects
-from marl_factory_grid.environment.groups.mixins import HasBoundedMixin, PositionMixin
-from marl_factory_grid.environment.entity.util import GlobalPosition
+from marl_factory_grid.modules.zones import Zone
 from marl_factory_grid.utils import helpers as h
 from marl_factory_grid.environment import constants as c
 
 
 class Combined(PositionMixin, EnvObjects):
 
     @property
@@ -30,25 +31,27 @@
         return self.name
 
     @property
     def obs_pairs(self):
         return [(name, None) for name in self.names]
 
 
-class GlobalPositions(HasBoundedMixin, EnvObjects):
+class GlobalPositions(HasBoundMixin, EnvObjects):
 
     _entity = GlobalPosition
     is_blocking_light = False,
     can_collide = False
 
     def __init__(self, *args, **kwargs):
         super(GlobalPositions, self).__init__(*args, **kwargs)
 
 
-class Zones(Objects):
+class ZonesOLD(Objects):
+
+    _entity = Zone
 
     @property
     def accounting_zones(self):
         return [self[idx] for idx, name in self.items() if name != c.DANGER_ZONE]
 
     def __init__(self, parsed_level):
         raise NotImplementedError('This needs a Rework')
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/wall_n_floors.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/groups/wall_n_floors.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     def from_tiles(cls, tiles, *args, **kwargs):
         raise RuntimeError()
 
 
 class Floors(Walls):
     _entity = Floor
     symbol = c.SYMBOL_FLOOR
-    is_blocking_light: bool = False
-    can_collide: bool = False
+    var_is_blocking_light: bool = False
+    var_can_collide: bool = False
 
     def __init__(self, *args, **kwargs):
         super(Floors, self).__init__(*args, **kwargs)
         self._value = c.VALUE_FREE_CELL
 
     @property
     def occupied_tiles(self):
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/rules.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/environment/rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     def __init__(self):
         pass
 
     def __repr__(self):
         return f'{self.name}'
 
-    def on_init(self, state):
+    def on_init(self, state, lvl_map):
         return []
 
     def on_reset(self):
         return []
 
     def tick_pre_step(self, state) -> List[TickResult]:
         return []
@@ -38,23 +38,37 @@
 
 class MaxStepsReached(Rule):
 
     def __init__(self, max_steps: int = 500):
         super().__init__()
         self.max_steps = max_steps
 
-    def on_init(self, state):
+    def on_init(self, state, lvl_map):
         pass
 
     def on_check_done(self, state):
         if self.max_steps <= state.curr_step:
             return [DoneResult(validity=c.VALID, identifier=self.name, reward=0)]
         return [DoneResult(validity=c.NOT_VALID, identifier=self.name, reward=0)]
 
 
+class AssignGlobalPositions(Rule):
+
+    def __init__(self):
+        super().__init__()
+
+    def on_init(self, state, lvl_map):
+        from marl_factory_grid.environment.entity.util import GlobalPosition
+        for agent in state[c.AGENT]:
+            gp = GlobalPosition(lvl_map.level_shape)
+            gp.bind_to(agent)
+            state[c.GLOBALPOSITIONS].add_item(gp)
+        return []
+
+
 class Collision(Rule):
 
     def __init__(self, done_at_collisions: bool = False):
         super().__init__()
         self.done_at_collisions = done_at_collisions
         self.curr_done = False
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/logging/envmonitor.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/logging/envmonitor.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/logging/recorder.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/logging/recorder.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/_template/rules.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/_template/rules.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class TemplateRule(Rule):
 
     def __init__(self, *args, **kwargs):
         super(TemplateRule, self).__init__(*args, **kwargs)
 
-    def on_init(self, state):
+    def on_init(self, state, lvl_map):
         pass
 
     def tick_pre_step(self, state) -> List[TickResult]:
         pass
 
     def tick_step(self, state) -> List[TickResult]:
         pass
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/actions.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/batteries/actions.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/constants.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/batteries/constants.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/entitites.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/batteries/entitites.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/groups.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/batteries/groups.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 from marl_factory_grid.environment.groups.env_objects import EnvObjects
-from marl_factory_grid.environment.groups.mixins import PositionMixin, HasBoundedMixin
+from marl_factory_grid.environment.groups.mixins import PositionMixin, HasBoundMixin
 from marl_factory_grid.modules.batteries.entitites import ChargePod, Battery
 
 
-class Batteries(HasBoundedMixin, EnvObjects):
+class Batteries(HasBoundMixin, EnvObjects):
 
     _entity = Battery
     is_blocking_light: bool = False
     can_collide: bool = False
 
     @property
     def obs_tag(self):
         return self.__class__.__name__
 
-    @property
-    def obs_pairs(self):
-        return [(x.name, x) for x in self]
-
     def __init__(self, *args, **kwargs):
         super(Batteries, self).__init__(*args, **kwargs)
 
-    def spawn_batteries(self, agents, initial_charge_level):
+    def spawn(self, agents, initial_charge_level):
         batteries = [self._entity(initial_charge_level, agent) for _, agent in enumerate(agents)]
         self.add_items(batteries)
 
-
 class ChargePods(PositionMixin, EnvObjects):
 
     _entity = ChargePod
 
     def __init__(self, *args, **kwargs):
         super(ChargePods, self).__init__(*args, **kwargs)
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/rules.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/batteries/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 class Btry(Rule):
 
     def __init__(self, initial_charge: float = 0.8, per_action_costs: Union[dict, float] = 0.02):
         super().__init__()
         self.per_action_costs = per_action_costs
         self.initial_charge = initial_charge
 
-    def on_init(self, state):
-        state[b.BATTERIES].spawn_batteries(state[c.AGENT], self.initial_charge)
+    def on_init(self, state, lvl_map):
+        state[b.BATTERIES].spawn(state[c.AGENT], self.initial_charge)
 
     def tick_pre_step(self, state) -> List[TickResult]:
         pass
 
     def tick_step(self, state) -> List[TickResult]:
         # Decharge
         batteries = state[b.BATTERIES]
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/actions.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/actions.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/dirtpiles.png` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/dirtpiles.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/entitites.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/entitites.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,30 @@
 from marl_factory_grid.utils.render import RenderEntity
 from marl_factory_grid.modules.clean_up import constants as d
 
 
 class DirtPile(Entity):
 
     @property
+    def var_can_collide(self):
+        return False
+
+    @property
+    def var_can_move(self):
+        return False
+
+    @property
+    def var_is_blocking_light(self):
+        return False
+
+    @property
+    def var_has_position(self):
+        return True
+
+    @property
     def amount(self):
         return self._amount
 
     @property
     def encoding(self):
         # Edit this if you want items to be drawn in the ops differntly
         return self._amount
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/groups.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/groups.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.clean_amount = clean_amount
         self.initial_amount = initial_amount
         self.initial_dirt_ratio = initial_dirt_ratio
         self.dirt_spawn_r_var = dirt_spawn_r_var
         self.max_global_amount = max_global_amount
         self.max_local_amount = max_local_amount
 
-    def spawn_dirt(self, then_dirty_tiles, amount) -> bool:
+    def spawn(self, then_dirty_tiles, amount) -> bool:
         if isinstance(then_dirty_tiles, Floor):
             then_dirty_tiles = [then_dirty_tiles]
         for tile in then_dirty_tiles:
             if not self.amount > self.max_global_amount:
                 if dirt := self.by_pos(tile.pos):
                     new_value = dirt.amount + amount
                     dirt.set_new_amount(new_value)
@@ -53,12 +53,12 @@
                                  isinstance(next(y for y in x.guests), DirtPile))
                          ]
         state.rng.shuffle(free_for_dirt)
 
         var = self.dirt_spawn_r_var
         new_spawn = abs(self.initial_dirt_ratio + (state.rng.uniform(-var, var) if initial_spawn else 0))
         n_dirt_tiles = max(0, int(new_spawn * len(free_for_dirt)))
-        return self.spawn_dirt(free_for_dirt[:n_dirt_tiles], self.initial_amount)
+        return self.spawn(free_for_dirt[:n_dirt_tiles], self.initial_amount)
 
     def __repr__(self):
         s = super(DirtPiles, self).__repr__()
         return f'{s[:-1]}, {self.amount})'
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/rule_done_on_all_clean.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/rule_done_on_all_clean.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/rule_respawn.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/rule_respawn.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class DirtRespawnRule(Rule):
 
     def __init__(self, spawn_freq=15):
         super().__init__()
         self.spawn_freq = spawn_freq
         self._next_dirt_spawn = spawn_freq
 
-    def on_init(self, state) -> str:
+    def on_init(self, state, lvl_map) -> str:
         state[d.DIRT].trigger_dirt_spawn(state, initial_spawn=True)
         return f'Initial Dirt was spawned on: {[x.pos for x in state[d.DIRT]]}'
 
     def tick_step(self, state):
         if self._next_dirt_spawn < 0:
             pass  # No DirtPile Spawn
         elif not self._next_dirt_spawn:
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/rule_smear_on_move.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/clean_up/rule_smear_on_move.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 
     def tick_post_step(self, state):
         results = list()
         for entity in state.moving_entites:
             if is_move(entity.state.identifier) and entity.state.validity == c.VALID:
                 if old_pos_dirt := state[d.DIRT].by_pos(entity.last_pos):
                     if smeared_dirt := round(old_pos_dirt.amount * self.smear_amount, 2):
-                        if state[d.DIRT].spawn_dirt(entity.tile, amount=smeared_dirt):
+                        if state[d.DIRT].spawn(entity.tile, amount=smeared_dirt):
                             results.append(TickResult(identifier=self.name, entity=entity,
                                                       reward=0, validity=c.VALID))
         return results
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/actions.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/destinations/actions.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 class DestAction(Action):
 
     def __init__(self):
         super().__init__(d.DESTINATION)
 
     def do(self, entity, state) -> Union[None, ActionResult]:
-        if destination := state[d.DESTINATION].by_pos(entity.pos):
+        dest_entities = d.DESTINATION if d.DESTINATION in state else d.BOUNDDESTINATION
+        assert dest_entities
+        if destination := state[dest_entities].by_pos(entity.pos):
             valid = destination.do_wait_action(entity)
             state.print(f'{entity.name} just waited at {entity.pos}')
         else:
             valid = c.NOT_VALID
             state.print(f'{entity.name} just tried to do_wait_action do_wait_action at {entity.pos} but failed')
         return ActionResult(entity=entity, identifier=self._identifier, validity=valid,
                             reward=r.WAIT_VALID if valid else r.WAIT_FAIL)
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/destinations.png` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/destinations/destinations.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/groups.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/destinations/groups.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from marl_factory_grid.environment.groups.env_objects import EnvObjects
-from marl_factory_grid.environment.groups.mixins import PositionMixin
-from marl_factory_grid.modules.destinations.entitites import Destination
+from marl_factory_grid.environment.groups.mixins import PositionMixin, HasBoundMixin
+from marl_factory_grid.modules.destinations.entitites import Destination, BoundDestination
 
 
 class Destinations(PositionMixin, EnvObjects):
 
     _entity = Destination
     is_blocking_light: bool = False
     can_collide: bool = False
@@ -12,14 +12,22 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def __repr__(self):
         return super(Destinations, self).__repr__()
 
 
+class BoundDestinations(HasBoundMixin, Destinations):
+
+    _entity = BoundDestination
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+
 class ReachedDestinations(Destinations):
     _entity = Destination
     is_blocking_light = False
     can_collide = False
 
     def __init__(self, *args, **kwargs):
         super(ReachedDestinations, self).__init__(*args, **kwargs)
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/rules.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/destinations/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     def __init__(self, spawn_frequency: int = 5, n_dests: int = 1,
                  spawn_mode: str = d.MODE_GROUPED):
         super(DestinationSpawn, self).__init__()
         self.spawn_frequency = spawn_frequency
         self.n_dests = n_dests
         self.spawn_mode = spawn_mode
 
-    def on_init(self, state):
+    def on_init(self, state, lvl_map):
         # noinspection PyAttributeOutsideInit
         self._dest_spawn_timer = self.spawn_frequency
         self.trigger_destination_spawn(self.n_dests, state)
         pass
 
     def tick_pre_step(self, state) -> List[TickResult]:
         pass
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/actions.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Union
 
 from marl_factory_grid.environment.actions import Action
-from marl_factory_grid.utils.results import ActionResult
-
 from marl_factory_grid.modules.doors import constants as d, rewards as r
 from marl_factory_grid.environment import constants as c
+from marl_factory_grid.utils.results import ActionResult
 
 
 class DoorUse(Action):
 
     def __init__(self):
         super().__init__(d.ACTION_DOOR_USE)
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/constants.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Names / Identifiers
-DOOR                    = 'Door'   # Identifier of Single-Door Entities.
-DOORS                   = 'Doors'  # Identifier of Door-objects and groups (groups).
+DOOR                    = 'Door'                # Identifier of Single-Door Entities.
+DOORS                   = 'Doors'               # Identifier of Door-objects and groups (groups).
 
 # Symbols (in map)
 SYMBOL_DOOR             = 'D'                   # Door _identifier for resolving the string based map files.
 
 # Values
-VALUE_ACCESS_INDICATOR  = 1 / 3  # Access-door-Cell value used in observation
-VALUE_OPEN_DOOR         = 2 / 3  # Open-door-Cell value used in observation
-VALUE_CLOSED_DOOR       = 3 / 3  # Closed-door-Cell value used in observation
+VALUE_ACCESS_INDICATOR  = 0.2222                # Access-door-Cell value used in observation
+VALUE_OPEN_DOOR         = 0.4444                # Open-door-Cell value used in observation
+VALUE_CLOSED_DOOR       = 0.6666                # Closed-door-Cell value used in observation
 
 # States
 STATE_CLOSED            = 'closed'              # Identifier to compare door-is-closed state
 STATE_OPEN              = 'open'                # Identifier to compare door-is-open state
 
 # Actions
-ACTION_DOOR_USE         = 'use_door'
+ACTION_DOOR_USE         = 'use_door'            # Identifier for door-action
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/door_closed.png` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/door_closed.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/door_open.png` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/door_open.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/entitites.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/entitites.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,66 +18,68 @@
         super().__init__(*args, **kwargs)
         self.__delattr__('move')
 
 
 class Door(Entity):
 
     @property
-    def is_blocking_pos(self):
+    def var_is_blocking_pos(self):
         return False if self.is_open else True
 
     @property
-    def is_blocking_light(self):
+    def var_is_blocking_light(self):
         return False if self.is_open else True
 
     @property
-    def can_collide(self):
+    def var_can_collide(self):
         return False if self.is_open else True
 
     @property
     def encoding(self):
         return d.VALUE_CLOSED_DOOR if self.is_closed else d.VALUE_OPEN_DOOR
 
     @property
     def str_state(self):
         return 'open' if self.is_open else 'closed'
 
     def __init__(self, *args, closed_on_init=True, auto_close_interval=10, indicate_area=False, **kwargs):
-        self._state = d.STATE_CLOSED
+        self._status = d.STATE_CLOSED
         super(Door, self).__init__(*args, **kwargs)
         self.auto_close_interval = auto_close_interval
         self.time_to_close = 0
         if not closed_on_init:
             self._open()
+        else:
+            self._close()
         if indicate_area:
             self._collection.add_items([DoorIndicator(x) for x in self.tile.neighboring_floor])
 
     def summarize_state(self):
         state_dict = super().summarize_state()
         state_dict.update(state=str(self.str_state), time_to_close=int(self.time_to_close))
         return state_dict
 
     @property
     def is_closed(self):
-        return self._state == d.STATE_CLOSED
+        return self._status == d.STATE_CLOSED
 
     @property
     def is_open(self):
-        return self._state == d.STATE_OPEN
+        return self._status == d.STATE_OPEN
 
     @property
     def status(self):
-        return self._state
+        return self._status
 
     def render(self):
         name, state = 'door_open' if self.is_open else 'door_closed', 'blank'
-        return RenderEntity(name, self.pos, 1, 'none', state, self.identifier_int + 1)
+        return RenderEntity(name, self.pos, 1, 'none', state, self.u_int + 1)
 
     def use(self):
-        if self._state == d.STATE_OPEN:
+        if self._status == d.STATE_OPEN:
             self._close()
         else:
             self._open()
         return c.VALID
 
     def tick(self):
         if self.is_open and len(self.tile) == 1 and self.time_to_close:
@@ -86,12 +88,12 @@
         elif self.is_open and not self.time_to_close and len(self.tile) == 1:
             self.use()
             return c.VALID
         else:
             return c.NOT_VALID
 
     def _open(self):
-        self._state = d.STATE_OPEN
+        self._status = d.STATE_OPEN
         self.time_to_close = self.auto_close_interval
 
     def _close(self):
-        self._state = d.STATE_CLOSED
+        self._status = d.STATE_CLOSED
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/groups.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/groups.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,19 +10,13 @@
 
     symbol = d.SYMBOL_DOOR
     _entity = Door
 
     def __init__(self, *args, **kwargs):
         super(Doors, self).__init__(*args, can_collide=True, **kwargs)
 
-    def get_near_position(self, position: (int, int)) -> Union[None, Door]:
-        try:
-            return next(door for door in self if position in door.tile.neighboring_floor_pos)
-        except StopIteration:
-            return None
-
     def tick_doors(self):
         result_dict = dict()
         for door in self:
             did_tick = door.tick()
             result_dict.update({door.name: did_tick})
         return result_dict
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/rule_door_auto_close.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/doors/rule_door_auto_close.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/actions.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/actions.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/assets/charge_pod.png` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/assets/charge_pod.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/assets/dropofflocations.png` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/assets/dropofflocations.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/assets/items.png` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/assets/items.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/entitites.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/entitites.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from marl_factory_grid.environment import constants as c
 from marl_factory_grid.utils.render import RenderEntity
 from marl_factory_grid.modules.items import constants as i
 
 
 class Item(Entity):
 
+    var_can_collide = False
+
     def render(self):
         return RenderEntity(i.ITEM, self.tile.pos) if self.pos != c.VALUE_NO_POS else None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._auto_despawn = -1
 
@@ -34,14 +36,30 @@
         super_summarization = super(Item, self).summarize_state()
         super_summarization.update(dict(auto_despawn=self.auto_despawn))
         return super_summarization
 
 
 class DropOffLocation(Entity):
 
+    @property
+    def var_can_collide(self):
+        return False
+
+    @property
+    def var_can_move(self):
+        return False
+
+    @property
+    def var_is_blocking_light(self):
+        return False
+
+    @property
+    def var_has_position(self):
+        return True
+
     def render(self):
         return RenderEntity(i.DROP_OFF, self.tile.pos)
 
     @property
     def encoding(self):
         return i.SYMBOL_DROP_OFF
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/groups.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/groups.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 from typing import List
 
 from marl_factory_grid.environment.groups.env_objects import EnvObjects
 from marl_factory_grid.environment.groups.objects import Objects
-from marl_factory_grid.environment.groups.mixins import PositionMixin, IsBoundMixin, HasBoundedMixin
+from marl_factory_grid.environment.groups.mixins import PositionMixin, IsBoundMixin, HasBoundMixin
 from marl_factory_grid.environment.entity.wall_floor import Floor
 from marl_factory_grid.environment.entity.agent import Agent
 from marl_factory_grid.modules.items.entitites import Item, DropOffLocation
 
 
 class Items(PositionMixin, EnvObjects):
 
     _entity = Item
     is_blocking_light: bool = False
     can_collide: bool = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def spawn_items(self, tiles: List[Floor]):
-        items = [self._entity(tile) for tile in tiles]
-        self.add_items(items)
-
-    def despawn_items(self, items: List[Item]):
-        items = [items] if isinstance(items, Item) else items
-        for item in items:
-            del self[item]
-
 
 class Inventory(IsBoundMixin, EnvObjects):
 
     _accepted_objects = Item
 
     @property
     def obs_tag(self):
@@ -51,30 +42,26 @@
         self.delete_env_object(item_to_pop)
         return item_to_pop
 
     def set_collection(self, collection):
         self._collection = collection
 
 
-class Inventories(HasBoundedMixin, Objects):
+class Inventories(HasBoundMixin, Objects):
 
     _entity = Inventory
-    can_move = False
-
-    @property
-    def obs_pairs(self):
-        return [(x.name, x) for x in self]
+    var_can_move = False
 
     def __init__(self, size, *args, **kwargs):
         super(Inventories, self).__init__(*args, **kwargs)
         self.size = size
         self._obs = None
         self._lazy_eval_transforms = []
 
-    def spawn_inventories(self, agents):
+    def spawn(self, agents):
         inventories = [self._entity(agent, self.size,)
                        for _, agent in enumerate(agents)]
         self.add_items(inventories)
 
     def idx_by_entity(self, entity):
         try:
             return next((idx for idx, inv in enumerate(self) if inv.belongs_to_entity(entity)))
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/rules.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/items/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         super().__init__()
         self.spawn_frequency = spawn_frequency
         self._next_item_spawn = spawn_frequency
         self.n_items = n_items
         self.max_dropoff_storage_size = max_dropoff_storage_size
         self.n_locations = n_locations
 
-    def on_init(self, state):
+    def on_init(self, state, lvl_map):
         self.trigger_drop_off_location_spawn(state)
         self._next_item_spawn = self.spawn_frequency
         self.trigger_inventory_spawn(state)
         self.trigger_item_spawn(state)
 
     def tick_step(self, state):
         for item in list(state[i.ITEM].values()):
@@ -38,25 +38,25 @@
         else:
             self._next_item_spawn = max(0, self._next_item_spawn - 1)
         return []
 
     def trigger_item_spawn(self, state):
         if item_to_spawns := max(0, (self.n_items - len(state[i.ITEM]))):
             empty_tiles = state[c.FLOOR].empty_tiles[:item_to_spawns]
-            state[i.ITEM].spawn_items(empty_tiles)
+            state[i.ITEM].spawn(empty_tiles)
             self._next_item_spawn = self.spawn_frequency
             state.print(f'{item_to_spawns} new items have been spawned; next spawn in {self._next_item_spawn}')
             return len(empty_tiles)
         else:
             state.print('No Items are spawning, limit is reached.')
             return 0
 
     @staticmethod
     def trigger_inventory_spawn(state):
-        state[i.INVENTORY].spawn_inventories(state[c.AGENT])
+        state[i.INVENTORY].spawn(state[c.AGENT])
 
     def tick_post_step(self, state) -> List[TickResult]:
         for item in list(state[i.ITEM].values()):
             if item.auto_despawn >= 1:
                 item.set_auto_despawn(item.auto_despawn-1)
             elif not item.auto_despawn:
                 state[i.ITEM].delete_env_object(item)
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/entitites.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/machines/entitites.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,69 @@
 from marl_factory_grid.environment.entity.entity import Entity
 from marl_factory_grid.utils.render import RenderEntity
 from marl_factory_grid.environment import constants as c
 from marl_factory_grid.utils.results import TickResult
-from marl_factory_grid.modules.machines import constants as m, rewards as r
+
+from . import constants as m
 
 
 class Machine(Entity):
 
     @property
+    def var_can_collide(self):
+        return False
+
+    @property
+    def var_can_move(self):
+        return False
+
+    @property
+    def var_is_blocking_light(self):
+        return False
+
+    @property
+    def var_has_position(self):
+        return True
+
+    @property
     def encoding(self):
-        return self._encodings[self.state]
+        return self._encodings[self.status]
 
     def __init__(self, *args, work_interval: int = 10, pause_interval: int = 15, **kwargs):
         super(Machine, self).__init__(*args, **kwargs)
         self._intervals = dict({m.STATE_IDLE: pause_interval, m.STATE_WORK: work_interval})
         self._encodings = dict({m.STATE_IDLE: pause_interval, m.STATE_WORK: work_interval})
 
-        self.state = m.STATE_IDLE
+        self.status = m.STATE_IDLE
         self.health = 100
         self._counter = 0
-        self.__delattr__('move')
 
     def maintain(self):
-        if self.state == m.STATE_WORK:
+        if self.status == m.STATE_WORK:
             return c.NOT_VALID
         if self.health <= 98:
             self.health = 100
             return c.VALID
         else:
             return c.NOT_VALID
 
     def tick(self):
-        if self.state == m.STATE_MAINTAIN and any([c.AGENT in x.name for x in self.tile.guests]):
-            return TickResult(self.name, c.VALID, r.NONE, self)
-        elif self.state == m.STATE_MAINTAIN and not any([c.AGENT in x.name for x in self.tile.guests]):
-            self.state = m.STATE_WORK
+        if self.status == m.STATE_MAINTAIN and any([c.AGENT in x.name for x in self.tile.guests]):
+            return TickResult(identifier=self.name, validity=c.VALID, reward=0, entity=self)
+        elif self.status == m.STATE_MAINTAIN and not any([c.AGENT in x.name for x in self.tile.guests]):
+            self.status = m.STATE_WORK
             self.reset_counter()
             return None
         elif self._counter:
             self._counter -= 1
             self.health -= 1
             return None
         else:
-            self.state = m.STATE_WORK if self.state == m.STATE_IDLE else m.STATE_IDLE
+            self.status = m.STATE_WORK if self.status == m.STATE_IDLE else m.STATE_IDLE
             self.reset_counter()
             return None
 
     def reset_counter(self):
-        self._counter = self._intervals[self.state]
+        self._counter = self._intervals[self.status]
 
     def render(self):
         return RenderEntity(m.MACHINE, self.pos)
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/rules.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/modules/machines/rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,22 +8,28 @@
 
 class MachineRule(Rule):
 
     def __init__(self, n_machines: int = 2):
         super(MachineRule, self).__init__()
         self.n_machines = n_machines
 
-    def on_init(self, state):
+    def on_init(self, state, lvl_map):
         empty_tiles = state[c.FLOOR].empty_tiles[:self.n_machines]
         state[m.MACHINES].add_items(Machine(tile) for tile in empty_tiles)
 
     def tick_pre_step(self, state) -> List[TickResult]:
         pass
 
     def tick_step(self, state) -> List[TickResult]:
         pass
 
     def tick_post_step(self, state) -> List[TickResult]:
         pass
 
     def on_check_done(self, state) -> List[DoneResult]:
         pass
+
+
+class DoneOnBreakRule(Rule):
+
+    def on_check_done(self, state) -> List[DoneResult]:
+        pass
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/plotting/compare_runs.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/plotting/compare_runs.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/plotting/plotting.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/quickstart.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/quickstart.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 
 
 def init():
     print('Retrieving available options...')
     ce = ConfigExplainer()
     cwd = Path(os.getcwd())
     ce.save_all(cwd / 'full_config.yaml')
-    template_path = Path(__file__) / 'marl_factory_grid' / 'modules' / '_template'
+    template_path = Path(__file__).parent / 'modules' / '_template'
     print(f'Available config options saved to: {(cwd / "full_config.yaml").resolve()}')
     print('-----------------------------')
     print(f'Copying Templates....')
     shutil.copytree(template_path, cwd)
-    print(f'Templates copied to {template_path.resolve()}')
+    print(f'Templates copied to {cwd}"/"{template_path.name}')
     print(':wave:')
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/config_parser.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/config_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 
 class FactoryConfigParser(object):
 
     default_entites = []
     default_rules = ['MaxStepsReached', 'Collision']
     default_actions = [c.MOVE8, c.NOOP]
-    default_observations = [c.WALLS, c.AGENTS]
+    default_observations = [c.WALLS, c.AGENT]
 
     def __init__(self, config_path, custom_modules_path: Union[None, PathLike] = None):
         self.config_path = Path(config_path)
-        self.custom_modules_path = Path(config_path) if custom_modules_path is not None else custom_modules_path
+        self.custom_modules_path = Path(custom_modules_path) if custom_modules_path is not None else custom_modules_path
         self.config = yaml.safe_load(self.config_path.open())
         self.do_record = False
 
     def __getattr__(self, item):
         return self['General'][item]
 
     def _get_sub_list(self, primary_key: str, sub_key: str):
@@ -65,20 +65,28 @@
         entities = []
         if c.DEFAULTS in self.entities:
             entities.extend(self.default_entites)
         entities.extend(x for x in self.entities if x != c.DEFAULTS)
 
         for entity in entities:
             try:
-                folder_path = MODULE_PATH if entity not in self.default_entites else DEFAULT_PATH
-                folder_path = (Path(__file__) / '..' / '..' / '..' / folder_path)
-                entity_class = locate_and_import_class(entity, folder_path)
-            except AttributeError:
-                folder_path = self.custom_modules_path
+                folder_path = Path(__file__).parent.parent / DEFAULT_PATH
                 entity_class = locate_and_import_class(entity, folder_path)
+            except AttributeError as e1:
+                try:
+                    folder_path = Path(__file__).parent.parent / MODULE_PATH
+                    entity_class = locate_and_import_class(entity, folder_path)
+                except AttributeError as e2:
+                    try:
+                        folder_path = self.custom_modules_path
+                        entity_class = locate_and_import_class(entity, folder_path)
+                    except AttributeError as e3:
+                        ents = [y for x in [e1.argss[1], e2.argss[1], e3.argss[1]] for y in x]
+                        raise AttributeError(e1.argss[0], e2.argss[0], e3.argss[0], 'Possible Entitys are>:', str(ents))
+
             entity_kwargs = self.entities.get(entity, {})
             entity_symbol = entity_class.symbol if hasattr(entity_class, 'symbol') else None
             entity_classes.update({entity: {'class': entity_class, 'kwargs': entity_kwargs, 'symbol': entity_symbol}})
         return entity_classes
 
     def load_agents(self, size, free_tiles):
         agents = Agents(size)
@@ -88,15 +96,15 @@
             actions = list()
             if c.DEFAULTS in self.agents[name]['Actions']:
                 actions.extend(self.default_actions)
             actions.extend(x for x in self.agents[name]['Actions'] if x != c.DEFAULTS)
             parsed_actions = list()
             for action in actions:
                 folder_path = MODULE_PATH if action not in base_env_actions else DEFAULT_PATH
-                folder_path = (Path(__file__) / '..' / '..' / '..' / folder_path)
+                folder_path = Path(__file__).parent.parent / folder_path
                 try:
                     class_or_classes = locate_and_import_class(action, folder_path)
                 except AttributeError:
                     class_or_classes = locate_and_import_class(action, self.custom_modules_path)
                 try:
                     parsed_actions.extend(class_or_classes)
                 except TypeError:
@@ -120,16 +128,19 @@
         if c.DEFAULTS in self.rules:
             for rule in self.default_rules:
                 if rule not in rules:
                     rules.append(rule)
         rules.extend(x for x in self.rules if x != c.DEFAULTS)
 
         for rule in rules:
-            folder_path = MODULE_PATH if rule not in self.default_rules else DEFAULT_PATH
-            folder_path = (Path(__file__) / '..' / '..' / '..' / folder_path)
             try:
+                folder_path = (Path(__file__).parent.parent / DEFAULT_PATH)
                 rule_class = locate_and_import_class(rule, folder_path)
             except AttributeError:
-                rule_class = locate_and_import_class(rule, self.custom_modules_path)
+                try:
+                    folder_path = (Path(__file__).parent.parent / MODULE_PATH)
+                    rule_class = locate_and_import_class(rule, folder_path)
+                except AttributeError:
+                    rule_class = locate_and_import_class(rule, self.custom_modules_path)
             rule_kwargs = self.rules.get(rule, {})
             rules_classes.update({rule: {'class': rule_class, 'kwargs': rule_kwargs}})
         return rules_classes
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/helpers.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
     :return: Binary numpy array
     :rtype: np.typing._array_like.ArrayLike
     """
 
     grid = np.array(level)
     binary_grid = np.zeros(grid.shape, dtype=np.int8)
-    binary_grid[grid == symbol] = c.VALUE_OCCUPIED_CELL
+    binary_grid[grid == str(symbol)] = c.VALUE_OCCUPIED_CELL
     return binary_grid
 
 
 def is_move(action_name: str):
     return action_name in MOVEMAP.keys()
 
 
@@ -218,22 +218,19 @@
     # possible_package_path = folder_path / '__init__.py'
     # package = str(possible_package_path) if possible_package_path.exists() else None
     all_found_modules = list()
     package_pos = next(idx for idx, x in enumerate(Path(__file__).resolve().parts) if x == 'marl_factory_grid')
     for module_path in module_paths:
         module_parts = [x.replace('.py', '') for idx, x in enumerate(module_path.parts) if idx >= package_pos]
         mod = importlib.import_module('.'.join(module_parts))
-        all_found_modules.extend([x for x in dir(mod) if not(x.startswith('__') or len(x) < 2 or x.isupper())
-                                  and x not in ['Entity',  'NamedTuple', 'List', 'Rule', 'Union', 'random', 'Floor'
-                                                'TickResult', 'ActionResult', 'Action', 'Agent', 'deque',
-                                                'BoundEntityMixin', 'RenderEntity', 'TemplateRule', 'defaultdict',
-                                                'is_move', 'Objects', 'PositionMixin', 'IsBoundMixin', 'EnvObject',
-                                                'EnvObjects', 'Dict', 'locate_and_import_class', 'yaml', 'Any',
-                                                'inspect']])
+        all_found_modules.extend([x for x in dir(mod) if (not(x.startswith('__') or len(x) <= 2) and x.istitle())
+                                  and x not in ['Entity',  'NamedTuple', 'List', 'Rule', 'Union', 'Floor'
+                                                'TickResult', 'ActionResult', 'Action', 'Agent', 'BoundEntityMixin',
+                                                'RenderEntity', 'TemplateRule', 'Objects', 'PositionMixin',
+                                                'IsBoundMixin', 'EnvObject', 'EnvObjects', 'Dict', 'Any'
+                                                ]])
         try:
             model_class = mod.__getattribute__(class_name)
             return model_class
         except AttributeError:
             continue
-    raise AttributeError(f'Class "{class_name}" was not found!!!"\n'
-                         f'Check the {folder_path.name} name.\n'
-                         f'Possible Options are:\n{set(all_found_modules)}')
+    raise AttributeError(f'Class "{class_name}" was not found in "{folder_path.name}"', list(set(all_found_modules)))
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/level_parser.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/level_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,36 +20,45 @@
         self.pomdp_r = pomdp_r
         self.e_p_dict = entity_parse_dict
         self._parsed_level = h.parse_level(Path(level_file_path))
         level_array = h.one_hot_level(self._parsed_level, c.SYMBOL_WALL)
         self.level_shape = level_array.shape
         self.size = self.pomdp_r**2 if self.pomdp_r else np.prod(self.level_shape)
 
+    def get_coordinates_for_symbol(self, symbol, negate=False):
+        level_array = h.one_hot_level(self._parsed_level, symbol)
+        if negate:
+            return np.argwhere(level_array != c.VALUE_OCCUPIED_CELL)
+        else:
+            return np.argwhere(level_array == c.VALUE_OCCUPIED_CELL)
+
     def do_init(self):
         entities = Entities()
         # Walls
-        level_array = h.one_hot_level(self._parsed_level, c.SYMBOL_WALL)
-
-        walls = Walls.from_coordinates(np.argwhere(level_array == c.VALUE_OCCUPIED_CELL), self.size)
+        walls = Walls.from_coordinates(self.get_coordinates_for_symbol(c.SYMBOL_WALL), self.size)
         entities.add_items({c.WALL: walls})
 
         # Floor
-        floor = Floors.from_coordinates(np.argwhere(level_array == c.VALUE_FREE_CELL), self.size)
+        floor = Floors.from_coordinates(self.get_coordinates_for_symbol(c.SYMBOL_WALL, negate=True), self.size)
         entities.add_items({c.FLOOR: floor})
 
         # All other
         for es_name in self.e_p_dict:
             e_class, e_kwargs = self.e_p_dict[es_name]['class'], self.e_p_dict[es_name]['kwargs']
 
-            if hasattr(e_class, 'symbol'):
-                level_array = h.one_hot_level(self._parsed_level, symbol=e_class.symbol)
-                if np.any(level_array):
-                    e = e_class.from_coordinates(np.argwhere(level_array == c.VALUE_OCCUPIED_CELL).tolist(),
-                                                 entities[c.FLOOR], self.size, entity_kwargs=e_kwargs
-                                                 )
-                else:
-                    raise ValueError(f'No {e_class} (Symbol: {e_class.symbol}) could be found!\n'
-                                     f'Check your level file!')
+            if hasattr(e_class, 'symbol') and e_class.symbol is not None:
+                symbols = e_class.symbol
+                if isinstance(symbols, (str, int, float)):
+                    symbols = [symbols]
+                for symbol in symbols:
+                    level_array = h.one_hot_level(self._parsed_level, symbol=symbol)
+                    if np.any(level_array):
+                        e = e_class.from_coordinates(np.argwhere(level_array == c.VALUE_OCCUPIED_CELL).tolist(),
+                                                     entities[c.FLOOR], self.size, entity_kwargs=e_kwargs
+                                                     )
+                    else:
+                        raise ValueError(f'No {e_class} (Symbol: {e_class.symbol}) could be found!\n'
+                                         f'Check your level file!')
             else:
                 e = e_class(self.size, **e_kwargs)
             entities.add_items({e.name: e})
         return entities
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/observation_builder.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/observation_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 from collections import defaultdict
 from itertools import product
 from typing import Dict, List
 
 import numpy as np
 from numba import njit
 
+from marl_factory_grid.environment import constants as c
 from marl_factory_grid.environment.groups.utils import Combined
 from marl_factory_grid.utils.states import Gamestate
 
-from marl_factory_grid.environment import constants as c
-
 
 class OBSBuilder(object):
 
     default_obs = [c.WALLS, c.OTHERS]
 
     @property
     def pomdp_d(self):
@@ -107,18 +106,18 @@
                         try:
                             e = self.all_obs[f'{l_name}({agent.name})']
                         except KeyError:
                             try:
                                 e = next(x for x in self.all_obs if l_name in x and agent.name in x)
                             except StopIteration:
                                 raise KeyError(
-                                    f'Check typing!\n{l_name} could not be found in:\n{dict(self.all_obs).keys()}')
+                                    f'Check typing! {l_name} could not be found in: {list(dict(self.all_obs).keys())}')
 
                     try:
-                        positional = e.has_position
+                        positional = e.var_has_position
                     except AttributeError:
                         positional = False
                     if positional:
                         # Seems to be not visible, so just skip it
                         # obs[idx] = np.zeros((self.pomdp_d, self.pomdp_d))
                         # All good
                         pass
@@ -168,15 +167,15 @@
                     else:
                         names.append(val)
                 combined = Combined(names, self.pomdp_r, identifier=agent.name)
                 self.all_obs[combined.name] = combined
                 obs_layers.append(combined.name)
             elif obs_str == c.OTHERS:
                 obs_layers.extend([x for x in self.all_obs if x != agent.name and x.startswith(f'{c.AGENT}[')])
-            elif obs_str == c.AGENTS:
+            elif obs_str == c.AGENT:
                 obs_layers.extend([x for x in self.all_obs if x.startswith(f'{c.AGENT}[')])
             else:
                 obs_layers.append(obs_str)
         self.obs_layers[agent.name] = obs_layers
         self.curr_lightmaps[agent.name] = np.zeros((self.pomdp_d or self.level_shape[0],
                                                     self.pomdp_d or self.level_shape[1]
                                                     ))
@@ -201,15 +200,15 @@
             [[math.cos(theta), -math.sin(theta)],
              [math.sin(theta), math.cos(theta)]] for theta in thetas
         ]
         rot_M = np.stack(rot_M, 0)
         rot_M = np.unique(np.round(rot_M @ north), axis=0)
         return rot_M.astype(int)
 
-    def ray_block_cache(self, cache_dict, key, callback, ents):
+    def ray_block_cache(self, cache_dict, key, callback):
         if key not in cache_dict:
             cache_dict[key] = callback()
         return cache_dict[key]
 
     def visible_entities(self, entities):
         visible = list()
         cache_blocking = {}
@@ -218,32 +217,21 @@
             rx, ry = ray[0]
             for x, y in ray:
                 cx, cy = x - rx, y - ry
 
                 entities_hit = entities.pos_dict[(x, y)]
                 hits = self.ray_block_cache(cache_blocking,
                                             (x, y),
-                                            lambda: any(e.is_blocking_light for e in entities_hit),
-                                            entities)
-
-                try:
-                    d = next(x for x in entities_hit if 'Door' in x.name)
-                    if d.pos in entities.pos_dict.keys():
-                        if d.is_closed and not entities.pos_dict[d.pos]:
-                            print()
-                except StopIteration:
-                    pass
+                                            lambda: any(True for e in entities_hit if e.var_is_blocking_light))
 
-                diag_hits = any([
+                diag_hits = all([
                     self.ray_block_cache(
                         cache_blocking,
                         key,
-                        # lambda: all(False for e in entities.pos_dict[key] if not e.is_blocking_light),
-                        lambda: any(e.is_blocking_light for e in entities.pos_dict[key]),
-                                            entities)
+                        lambda: all(False for e in entities.pos_dict[key] if not e.var_is_blocking_light))
                     for key in ((x, y-cy), (x-cx, y))
                 ]) if (cx != 0 and cy != 0) else False
 
                 visible += entities_hit if not diag_hits else []
                 if hits or diag_hits:
                     break
                 rx, ry = x, y
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/renderer.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,32 +23,32 @@
 SCALE: str = 'scale'
 
 
 class Renderer:
     BG_COLOR = (178, 190, 195)         # (99, 110, 114)
     WHITE = (223, 230, 233)            # (200, 200, 200)
     AGENT_VIEW_COLOR = (9, 132, 227)
-    ASSETS = Path(__file__).parent.parent / 'assets'
-    MODULE_ASSETS = Path(__file__).parent.parent.parent / 'modules'
+    ASSETS = Path(__file__).parent.parent
 
     def __init__(self, lvl_shape: Tuple[int, int] = (16, 16),
                  lvl_padded_shape: Union[Tuple[int, int], None] = None,
                  cell_size: int = 40, fps: int = 7,
                  grid_lines: bool = True, view_radius: int = 2):
+        # TODO: Customn_assets paths
         self.grid_h, self.grid_w = lvl_shape
         self.lvl_padded_shape = lvl_padded_shape if lvl_padded_shape is not None else lvl_shape
         self.cell_size = cell_size
         self.fps = fps
         self.grid_lines = grid_lines
         self.view_radius = view_radius
         pygame.init()
         self.screen_size = (self.grid_w*cell_size, self.grid_h*cell_size)
         self.screen = pygame.display.set_mode(self.screen_size)
         self.clock = pygame.time.Clock()
-        assets = list(self.ASSETS.rglob('*.png')) + list(self.MODULE_ASSETS.rglob('*.png'))
+        assets = list(self.ASSETS.rglob('*.png'))
         self.assets = {path.stem: self.load_asset(str(path), 1) for path in assets}
         self.fill_bg()
 
         now = time.time()
         self.font = pygame.font.Font(None, 20)
         self.font.set_bold(True)
         print('Loading System font with pygame.font.Font took', time.time() - now)
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/results.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/results.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from typing import Union
 from dataclasses import dataclass
 
-from marl_factory_grid.environment.entity.entity import Entity
-
 TYPE_VALUE  = 'value'
 TYPE_REWARD = 'reward'
 types = [TYPE_VALUE, TYPE_REWARD]
 
 @dataclass
 class InfoObject:
     identifier: str
@@ -16,15 +14,15 @@
 
 @dataclass
 class Result:
     identifier: str
     validity: bool
     reward: Union[float, None] = None
     value: Union[float, None] = None
-    entity: Union[Entity, None] = None
+    entity: None = None
 
     def get_infos(self):
         n = self.entity.name if self.entity is not None else "Global"
         return [InfoObject(identifier=f'{n}_{self.identifier}_{t}',
                            val_type=t, value=self.__getattribute__(t)) for t in types
                 if self.__getattribute__(t) is not None]
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/states.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/states.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import List, Dict
 
 import numpy as np
 
+
+from marl_factory_grid.environment import constants as c
 from marl_factory_grid.environment.entity.wall_floor import Floor
 from marl_factory_grid.environment.rules import Rule
 from marl_factory_grid.utils.results import Result
-from marl_factory_grid.environment import constants as c
 
 
 class StepRules:
     def __init__(self, *args):
         if args:
             self.rules = list(args)
         else:
@@ -22,17 +23,17 @@
         return iter(self.rules)
 
     def append(self, item):
         assert isinstance(item, Rule)
         self.rules.append(item)
         return True
 
-    def do_all_init(self, state):
+    def do_all_init(self, state, lvl_map):
         for rule in self.rules:
-            if rule_init_printline := rule.on_init(state):
+            if rule_init_printline := rule.on_init(state, lvl_map):
                 state.print(rule_init_printline)
         return c.VALID
 
     def tick_step_all(self, state):
         results = list()
         for rule in self.rules:
             if tick_step_result := rule.tick_step(state):
@@ -54,15 +55,15 @@
         return results
 
 
 class Gamestate(object):
 
     @property
     def moving_entites(self):
-        return [y for x in self.entities for y in x if x.can_move]
+        return [y for x in self.entities for y in x if x.var_can_move]
 
     def __init__(self, entitites, rules: Dict[str, dict], env_seed=69, verbose=False):
         self.entities = entitites
         self.NO_POS_TILE = Floor(c.VALUE_NO_POS)
         self.curr_step = 0
         self.curr_actions = None
         self.verbose = verbose
@@ -71,14 +72,17 @@
 
     def __getitem__(self, item):
         return self.entities[item]
 
     def __iter__(self):
         return iter(e for e in self.entities.values())
 
+    def __contains__(self, item):
+        return item in self.entities
+
     def __repr__(self):
         return f'{self.__class__.__name__}({len(self.entities)} Entitites @ Step {self.curr_step})'
 
     def tick(self, actions) -> List[Result]:
         results = list()
         self.curr_step += 1
 
@@ -103,10 +107,10 @@
         for rule in self.rules:
             if on_check_done_result := rule.on_check_done(self):
                 results.extend(on_check_done_result)
         return results
 
     def get_all_tiles_with_collisions(self) -> List[Floor]:
         tiles = [self[c.FLOOR].by_pos(pos) for pos, e in self.entities.pos_dict.items()
-                 if sum([x.can_collide for x in e]) > 1]
+                 if sum([x.var_can_collide for x in e]) > 1]
         # tiles = [x for x in self[c.FLOOR] if len(x.guests_that_can_collide) > 1]
         return tiles
```

### Comparing `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/tools.py` & `Marl-Factory-Grid-0.1.1/marl_factory_grid/utils/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ACTION       = 'Action'
 GENERAL      = 'General'
 ENTITIES     = 'Objects'
 OBSERVATIONS = 'Observations'
 RULES        = 'Rule'
 ASSETS       = 'Assets'
-EXCLUDED     = ['identifier', 'args', 'kwargs', 'Move',
+EXCLUDED     = ['identifier', 'args', 'kwargs', 'Move', 'Floor', 'Agent', 'GlobalPositions', 'Walls',
                 'TemplateRule', 'Entities', 'EnvObjects', 'Zones', ]
 
 
 class ConfigExplainer:
 
     def __init__(self, custom_path: Union[None, PathLike] = None):
         self.base_path = Path(__file__).parent.parent.resolve()
```

### Comparing `Marl-Factory-Grid-0.0.9/setup.py` & `Marl-Factory-Grid-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='Marl-Factory-Grid',
-      version='0.0.9',
+      version='0.1.1',
       description='A framework to research MARL agents in various setings.',
       author='Steffen Illium',
       author_email='steffen.illium@ifi.lmu.de',
       url='https://github.com/illiumst/marl-factory-grid/import',
       license='MIT',
       keywords=[
             'artificial intelligence',
```


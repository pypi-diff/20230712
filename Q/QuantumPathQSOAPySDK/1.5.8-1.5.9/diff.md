# Comparing `tmp/QuantumPathQSOAPySDK-1.5.8.tar.gz` & `tmp/QuantumPathQSOAPySDK-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantumPathQSOAPySDK-1.5.8.tar", last modified: Mon Jul  3 09:00:51 2023, max compression
+gzip compressed data, was "QuantumPathQSOAPySDK-1.5.9.tar", last modified: Wed Jul 12 10:57:04 2023, max compression
```

## Comparing `QuantumPathQSOAPySDK-1.5.8.tar` & `QuantumPathQSOAPySDK-1.5.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 09:00:51.069873 QuantumPathQSOAPySDK-1.5.8/
--rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.8/MANIFEST.in
--rw-rw-rw-   0        0        0      928 2023-07-03 09:00:51.068875 QuantumPathQSOAPySDK-1.5.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-03 09:00:50.965752 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/
--rw-rw-rw-   0        0        0    43350 2023-06-30 11:31:19.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/QSOAPlatform.py
--rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:00:50.981108 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/
--rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:00:50.989089 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/annealing/
--rw-rw-rw-   0        0        0     7907 2023-06-26 09:01:38.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
--rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
--rw-rw-rw-   0        0        0    28762 2023-06-27 08:12:21.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/annealing/components.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:00:50.995072 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/flow/
--rw-rw-rw-   0        0        0     4848 2023-06-26 09:03:51.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
--rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/flow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:00:50.999061 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/gates/
--rw-rw-rw-   0        0        0    53330 2023-06-27 11:39:45.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
--rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/gates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:00:51.020012 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/
--rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/Application.py
--rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/Asset.py
--rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/AssetManagementData.py
--rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
--rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/DeviceItem.py
--rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/Execution.py
--rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/FlowItem.py
--rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
--rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/SolutionItem.py
--rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:00:51.030001 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/
--rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/__init__.py
--rw-rw-rw-   0        0        0     9869 2023-07-03 08:57:31.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
--rw-rw-rw-   0        0        0    10579 2023-07-03 08:57:37.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
--rw-rw-rw-   0        0        0     4296 2023-07-03 08:57:44.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:00:51.040950 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/
--rw-rw-rw-   0        0        0     3682 2023-07-03 08:31:52.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/Context.py
--rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/Exception.py
--rw-rw-rw-   0        0        0      160 2023-06-22 10:01:20.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/__init__.py
--rw-rw-rw-   0        0        0     1605 2023-06-30 10:05:23.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/apiConnection.py
--rw-rw-rw-   0        0        0     3571 2023-06-30 12:03:18.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/checker.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:00:50.980112 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/
--rw-rw-rw-   0        0        0      928 2023-07-03 09:00:50.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2085 2023-07-03 09:00:50.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 09:00:50.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-03 09:00:50.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-03 09:00:50.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 09:00:51.069873 QuantumPathQSOAPySDK-1.5.8/setup.cfg
--rw-rw-rw-   0        0        0      973 2023-07-03 09:00:42.000000 QuantumPathQSOAPySDK-1.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:00:51.042943 QuantumPathQSOAPySDK-1.5.8/test/
--rw-rw-rw-   0        0        0       83 2023-07-03 08:57:13.000000 QuantumPathQSOAPySDK-1.5.8/test/test.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:00:51.053915 QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/__init__.py
--rw-rw-rw-   0        0        0     4995 2023-07-03 08:37:49.000000 QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_ContextMethods.py
--rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_DynamicMethods.py
--rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_QSOAPlatform.py
--rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_SecurityMethods.py
--rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_StaticMethods.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:00:51.066880 QuantumPathQSOAPySDK-1.5.8/test/test_circuit/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5.8/test/test_circuit/__init__.py
--rw-rw-rw-   0        0        0   130207 2023-06-27 08:11:21.000000 QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitAnnealing.py
--rw-rw-rw-   0        0        0     8004 2023-06-26 10:45:48.000000 QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitFlow.py
--rw-rw-rw-   0        0        0     7331 2023-06-26 10:46:07.000000 QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitGates.py
--rw-rw-rw-   0        0        0   153999 2023-06-27 11:33:39.000000 QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitGates_gates1.py
--rw-rw-rw-   0        0        0    41572 2023-06-27 11:33:49.000000 QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitGates_gates2.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:57:04.842326 QuantumPathQSOAPySDK-1.5.9/
+-rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      928 2023-07-12 10:57:04.840323 QuantumPathQSOAPySDK-1.5.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 10:57:04.652890 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/
+-rw-rw-rw-   0        0        0    43350 2023-06-30 11:31:19.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/QSOAPlatform.py
+-rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:57:04.694635 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/
+-rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:57:04.704769 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/annealing/
+-rw-rw-rw-   0        0        0     7907 2023-06-26 09:01:38.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
+-rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
+-rw-rw-rw-   0        0        0    28762 2023-06-27 08:12:21.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/annealing/components.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:57:04.709750 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/flow/
+-rw-rw-rw-   0        0        0     4848 2023-06-26 09:03:51.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
+-rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/flow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:57:04.717316 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/gates/
+-rw-rw-rw-   0        0        0    53330 2023-06-27 11:39:45.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
+-rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/gates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:57:04.755222 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/
+-rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/Application.py
+-rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/Asset.py
+-rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/AssetManagementData.py
+-rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
+-rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/DeviceItem.py
+-rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/Execution.py
+-rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/FlowItem.py
+-rw-rw-rw-   0        0        0     2613 2023-07-12 10:45:13.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
+-rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/SolutionItem.py
+-rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:57:04.771187 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/qsoa/
+-rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/qsoa/__init__.py
+-rw-rw-rw-   0        0        0     9869 2023-07-03 08:57:31.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
+-rw-rw-rw-   0        0        0    10579 2023-07-03 08:57:37.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
+-rw-rw-rw-   0        0        0     4296 2023-07-03 08:57:44.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:57:04.788134 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/utils/
+-rw-rw-rw-   0        0        0     3682 2023-07-03 08:31:52.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/utils/Context.py
+-rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/utils/Exception.py
+-rw-rw-rw-   0        0        0      160 2023-06-22 10:01:20.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/utils/__init__.py
+-rw-rw-rw-   0        0        0     1605 2023-06-30 10:05:23.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/utils/apiConnection.py
+-rw-rw-rw-   0        0        0     3571 2023-06-30 12:03:18.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/utils/checker.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:57:04.690790 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK.egg-info/
+-rw-rw-rw-   0        0        0      928 2023-07-12 10:57:04.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2085 2023-07-12 10:57:04.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 10:57:04.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-12 10:57:04.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-12 10:57:04.000000 QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 10:57:04.844310 QuantumPathQSOAPySDK-1.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      973 2023-07-12 10:56:25.000000 QuantumPathQSOAPySDK-1.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:57:04.791194 QuantumPathQSOAPySDK-1.5.9/test/
+-rw-rw-rw-   0        0        0       83 2023-07-03 08:57:13.000000 QuantumPathQSOAPySDK-1.5.9/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:57:04.810580 QuantumPathQSOAPySDK-1.5.9/test/test_QSOAPlatform/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5.9/test/test_QSOAPlatform/__init__.py
+-rw-rw-rw-   0        0        0     4995 2023-07-03 08:37:49.000000 QuantumPathQSOAPySDK-1.5.9/test/test_QSOAPlatform/test_ContextMethods.py
+-rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5.9/test/test_QSOAPlatform/test_DynamicMethods.py
+-rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5.9/test/test_QSOAPlatform/test_QSOAPlatform.py
+-rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5.9/test/test_QSOAPlatform/test_SecurityMethods.py
+-rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5.9/test/test_QSOAPlatform/test_StaticMethods.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:57:04.837002 QuantumPathQSOAPySDK-1.5.9/test/test_circuit/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5.9/test/test_circuit/__init__.py
+-rw-rw-rw-   0        0        0   130207 2023-06-27 08:11:21.000000 QuantumPathQSOAPySDK-1.5.9/test/test_circuit/test_CircuitAnnealing.py
+-rw-rw-rw-   0        0        0     8004 2023-06-26 10:45:48.000000 QuantumPathQSOAPySDK-1.5.9/test/test_circuit/test_CircuitFlow.py
+-rw-rw-rw-   0        0        0     7331 2023-06-26 10:46:07.000000 QuantumPathQSOAPySDK-1.5.9/test/test_circuit/test_CircuitGates.py
+-rw-rw-rw-   0        0        0   153999 2023-06-27 11:33:39.000000 QuantumPathQSOAPySDK-1.5.9/test/test_circuit/test_CircuitGates_gates1.py
+-rw-rw-rw-   0        0        0    41572 2023-06-27 11:33:49.000000 QuantumPathQSOAPySDK-1.5.9/test/test_circuit/test_CircuitGates_gates2.py
```

### Comparing `QuantumPathQSOAPySDK-1.5.8/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5.8
+Version: 1.5.9
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/QSOAPlatform.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/annealing/components.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/annealing/components.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/Application.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/Application.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/Asset.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/Asset.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/AssetManagementData.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/AssetManagementData.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/AssetManagementResult.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/AssetManagementResult.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/DeviceItem.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/DeviceItem.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/Execution.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/Execution.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     def getDeviceTypeName(self) -> str:
         return self.__deviceTypeName
         
     def getResultHistogram(self) -> str:
         return self.__resultHistogram
 
-    def getExecutionDate(self) -> float:
+    def getExecutionDate(self) -> str:
         return self.__executionDate
 
     def getDurationMinutes(self) -> float:
         return self.__durationMinutes
 
     def getResultType(self) -> str:
         return self.__resultType
```

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/__init__.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/qsoa/__init__.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/connectionPoints.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/qsoa/connectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/Context.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/utils/Context.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/Exception.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/utils/Exception.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/apiConnection.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/utils/apiConnection.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/checker.py` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK/utils/checker.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5.8
+Version: 1.5.9
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/SOURCES.txt` & `QuantumPathQSOAPySDK-1.5.9/QuantumPathQSOAPySDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/setup.py` & `QuantumPathQSOAPySDK-1.5.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   'Intended Audience :: Developers',
   'Intended Audience :: Education',
   'Intended Audience :: Information Technology'
 ]
 
 setup(
   name='QuantumPathQSOAPySDK',
-  version='1.5.8',
+  version='1.5.9',
   description='QuantumPath qSOA Python SDK',
   long_description=open('README.md').read(),
   long_description_content_type = 'text/markdown',
   url='https://core.quantumpath.app/',
   author='QuantumPath',
   classifiers=classifiers,
   keywords='quantum, quantumpath, qSOA, sdk, quantum applications, quantum software',
```

### Comparing `QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_ContextMethods.py` & `QuantumPathQSOAPySDK-1.5.9/test/test_QSOAPlatform/test_ContextMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_DynamicMethods.py` & `QuantumPathQSOAPySDK-1.5.9/test/test_QSOAPlatform/test_DynamicMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.9/test/test_QSOAPlatform/test_QSOAPlatform.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_SecurityMethods.py` & `QuantumPathQSOAPySDK-1.5.9/test/test_QSOAPlatform/test_SecurityMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_StaticMethods.py` & `QuantumPathQSOAPySDK-1.5.9/test/test_QSOAPlatform/test_StaticMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.9/test/test_circuit/test_CircuitAnnealing.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.9/test/test_circuit/test_CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.9/test/test_circuit/test_CircuitGates.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitGates_gates1.py` & `QuantumPathQSOAPySDK-1.5.9/test/test_circuit/test_CircuitGates_gates1.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitGates_gates2.py` & `QuantumPathQSOAPySDK-1.5.9/test/test_circuit/test_CircuitGates_gates2.py`

 * *Files identical despite different names*


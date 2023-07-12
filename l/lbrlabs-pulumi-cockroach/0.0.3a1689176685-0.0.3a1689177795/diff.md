# Comparing `tmp/lbrlabs_pulumi_cockroach-0.0.3a1689176685.tar.gz` & `tmp/lbrlabs_pulumi_cockroach-0.0.3a1689177795.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbrlabs_pulumi_cockroach-0.0.3a1689176685.tar", last modified: Wed Jul 12 15:49:44 2023, max compression
+gzip compressed data, was "dist/lbrlabs_pulumi_cockroach-0.0.3a1689177795.tar", last modified: Wed Jul 12 16:08:42 2023, max compression
```

## Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685.tar` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:44.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-12 15:49:44.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:44.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23444 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/allow_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/ca_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/cmek.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:44.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/finalize_version_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/get_cluster_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/get_cockroach_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/get_connection_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/get_person_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    20051 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/log_export_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/metric_export_cloudwatch_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/metric_export_datadog_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    27888 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/private_endpoint_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/private_endpoint_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/sql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/user_role_grants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:44.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-12 15:49:44.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-12 15:49:44.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:49:44.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:49:44.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 15:49:44.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 15:49:44.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:49:44.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-12 15:49:43.000000 lbrlabs_pulumi_cockroach-0.0.3a1689176685/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23444 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/ca_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18469 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/cmek.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/finalize_version_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/get_cluster_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/get_cockroach_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/get_connection_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/get_person_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21794 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/log_export_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/metric_export_cloudwatch_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/metric_export_datadog_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27888 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/private_endpoint_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/private_endpoint_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/sql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/user_role_grants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-12 16:08:42.000000 lbrlabs_pulumi_cockroach-0.0.3a1689177795/setup.py
```

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/PKG-INFO` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbrlabs_pulumi_cockroach
-Version: 0.0.3a1689176685
+Version: 0.0.3a1689177795
 Summary: A Pulumi package to create and managed cockroach db resources in Pulumi programs.
 Home-page: https://lbrlabs.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/lbrlabs/pulumi-cockroach
 Description: 
         # Cockroach Resource Provider
```

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/README.md` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/README.md`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/__init__.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/__init__.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/_inputs.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/_inputs.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/_utilities.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/_utilities.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/allow_list.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/allow_list.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/ca_cert.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/finalize_version_upgrade.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,170 +5,177 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['CaCertArgs', 'CaCert']
+__all__ = ['FinalizeVersionUpgradeArgs', 'FinalizeVersionUpgrade']
 
 @pulumi.input_type
-class CaCertArgs:
+class FinalizeVersionUpgradeArgs:
     def __init__(__self__, *,
-                 x509_pem_cert: pulumi.Input[str]):
+                 cluster_id: pulumi.Input[str],
+                 cockroach_version: pulumi.Input[str]):
         """
-        The set of arguments for constructing a CaCert resource.
-        :param pulumi.Input[str] x509_pem_cert: X509 certificate in PEM format
+        The set of arguments for constructing a FinalizeVersionUpgrade resource.
+        :param pulumi.Input[str] cluster_id: Cluster ID
         """
-        pulumi.set(__self__, "x509_pem_cert", x509_pem_cert)
+        pulumi.set(__self__, "cluster_id", cluster_id)
+        pulumi.set(__self__, "cockroach_version", cockroach_version)
 
     @property
-    @pulumi.getter(name="x509PemCert")
-    def x509_pem_cert(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> pulumi.Input[str]:
         """
-        X509 certificate in PEM format
+        Cluster ID
         """
-        return pulumi.get(self, "x509_pem_cert")
+        return pulumi.get(self, "cluster_id")
 
-    @x509_pem_cert.setter
-    def x509_pem_cert(self, value: pulumi.Input[str]):
-        pulumi.set(self, "x509_pem_cert", value)
+    @cluster_id.setter
+    def cluster_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "cluster_id", value)
+
+    @property
+    @pulumi.getter(name="cockroachVersion")
+    def cockroach_version(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "cockroach_version")
+
+    @cockroach_version.setter
+    def cockroach_version(self, value: pulumi.Input[str]):
+        pulumi.set(self, "cockroach_version", value)
 
 
 @pulumi.input_type
-class _CaCertState:
+class _FinalizeVersionUpgradeState:
     def __init__(__self__, *,
-                 status: Optional[pulumi.Input[str]] = None,
-                 x509_pem_cert: Optional[pulumi.Input[str]] = None):
+                 cluster_id: Optional[pulumi.Input[str]] = None,
+                 cockroach_version: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering CaCert resources.
-        :param pulumi.Input[str] status: Status of client CA certs on a cluster
-        :param pulumi.Input[str] x509_pem_cert: X509 certificate in PEM format
+        Input properties used for looking up and filtering FinalizeVersionUpgrade resources.
+        :param pulumi.Input[str] cluster_id: Cluster ID
         """
-        if status is not None:
-            pulumi.set(__self__, "status", status)
-        if x509_pem_cert is not None:
-            pulumi.set(__self__, "x509_pem_cert", x509_pem_cert)
+        if cluster_id is not None:
+            pulumi.set(__self__, "cluster_id", cluster_id)
+        if cockroach_version is not None:
+            pulumi.set(__self__, "cockroach_version", cockroach_version)
 
     @property
-    @pulumi.getter
-    def status(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Status of client CA certs on a cluster
+        Cluster ID
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "cluster_id")
 
-    @status.setter
-    def status(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "status", value)
+    @cluster_id.setter
+    def cluster_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cluster_id", value)
 
     @property
-    @pulumi.getter(name="x509PemCert")
-    def x509_pem_cert(self) -> Optional[pulumi.Input[str]]:
-        """
-        X509 certificate in PEM format
-        """
-        return pulumi.get(self, "x509_pem_cert")
+    @pulumi.getter(name="cockroachVersion")
+    def cockroach_version(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "cockroach_version")
 
-    @x509_pem_cert.setter
-    def x509_pem_cert(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "x509_pem_cert", value)
+    @cockroach_version.setter
+    def cockroach_version(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cockroach_version", value)
 
 
-class CaCert(pulumi.CustomResource):
+class FinalizeVersionUpgrade(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 x509_pem_cert: Optional[pulumi.Input[str]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
+                 cockroach_version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Manages client CA certs.
+        Utility resource that represents the one-time action of finalizing a cluster's pending CockroachDB version upgrade.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] x509_pem_cert: X509 certificate in PEM format
+        :param pulumi.Input[str] cluster_id: Cluster ID
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: CaCertArgs,
+                 args: FinalizeVersionUpgradeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Manages client CA certs.
+        Utility resource that represents the one-time action of finalizing a cluster's pending CockroachDB version upgrade.
 
         :param str resource_name: The name of the resource.
-        :param CaCertArgs args: The arguments to use to populate this resource's properties.
+        :param FinalizeVersionUpgradeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(CaCertArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(FinalizeVersionUpgradeArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 x509_pem_cert: Optional[pulumi.Input[str]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
+                 cockroach_version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = CaCertArgs.__new__(CaCertArgs)
+            __props__ = FinalizeVersionUpgradeArgs.__new__(FinalizeVersionUpgradeArgs)
 
-            if x509_pem_cert is None and not opts.urn:
-                raise TypeError("Missing required property 'x509_pem_cert'")
-            __props__.__dict__["x509_pem_cert"] = x509_pem_cert
-            __props__.__dict__["status"] = None
-        super(CaCert, __self__).__init__(
-            'cockroach:index/caCert:CaCert',
+            if cluster_id is None and not opts.urn:
+                raise TypeError("Missing required property 'cluster_id'")
+            __props__.__dict__["cluster_id"] = cluster_id
+            if cockroach_version is None and not opts.urn:
+                raise TypeError("Missing required property 'cockroach_version'")
+            __props__.__dict__["cockroach_version"] = cockroach_version
+        super(FinalizeVersionUpgrade, __self__).__init__(
+            'cockroach:index/finalizeVersionUpgrade:FinalizeVersionUpgrade',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            status: Optional[pulumi.Input[str]] = None,
-            x509_pem_cert: Optional[pulumi.Input[str]] = None) -> 'CaCert':
+            cluster_id: Optional[pulumi.Input[str]] = None,
+            cockroach_version: Optional[pulumi.Input[str]] = None) -> 'FinalizeVersionUpgrade':
         """
-        Get an existing CaCert resource's state with the given name, id, and optional extra
+        Get an existing FinalizeVersionUpgrade resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] status: Status of client CA certs on a cluster
-        :param pulumi.Input[str] x509_pem_cert: X509 certificate in PEM format
+        :param pulumi.Input[str] cluster_id: Cluster ID
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _CaCertState.__new__(_CaCertState)
+        __props__ = _FinalizeVersionUpgradeState.__new__(_FinalizeVersionUpgradeState)
 
-        __props__.__dict__["status"] = status
-        __props__.__dict__["x509_pem_cert"] = x509_pem_cert
-        return CaCert(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["cluster_id"] = cluster_id
+        __props__.__dict__["cockroach_version"] = cockroach_version
+        return FinalizeVersionUpgrade(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def status(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> pulumi.Output[str]:
         """
-        Status of client CA certs on a cluster
+        Cluster ID
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "cluster_id")
 
     @property
-    @pulumi.getter(name="x509PemCert")
-    def x509_pem_cert(self) -> pulumi.Output[str]:
-        """
-        X509 certificate in PEM format
-        """
-        return pulumi.get(self, "x509_pem_cert")
+    @pulumi.getter(name="cockroachVersion")
+    def cockroach_version(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "cockroach_version")
```

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/cluster.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,32 +95,36 @@
 
 
 @pulumi.input_type
 class _ClusterState:
     def __init__(__self__, *,
                  account_id: Optional[pulumi.Input[str]] = None,
                  cloud_provider: Optional[pulumi.Input[str]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  cockroach_version: Optional[pulumi.Input[str]] = None,
                  creator_id: Optional[pulumi.Input[str]] = None,
                  dedicated: Optional[pulumi.Input['ClusterDedicatedArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  operation_status: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[str]] = None,
                  regions: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterRegionArgs']]]] = None,
                  serverless: Optional[pulumi.Input['ClusterServerlessArgs']] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  upgrade_status: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Cluster resources.
+        :param pulumi.Input[str] cluster_id: The ID of this resource.
         :param pulumi.Input[str] name: Name of cluster
         """
         if account_id is not None:
             pulumi.set(__self__, "account_id", account_id)
         if cloud_provider is not None:
             pulumi.set(__self__, "cloud_provider", cloud_provider)
+        if cluster_id is not None:
+            pulumi.set(__self__, "cluster_id", cluster_id)
         if cockroach_version is not None:
             pulumi.set(__self__, "cockroach_version", cockroach_version)
         if creator_id is not None:
             pulumi.set(__self__, "creator_id", creator_id)
         if dedicated is not None:
             pulumi.set(__self__, "dedicated", dedicated)
         if name is not None:
@@ -153,14 +157,26 @@
         return pulumi.get(self, "cloud_provider")
 
     @cloud_provider.setter
     def cloud_provider(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cloud_provider", value)
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ID of this resource.
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @cluster_id.setter
+    def cluster_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cluster_id", value)
+
+    @property
     @pulumi.getter(name="cockroachVersion")
     def cockroach_version(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "cockroach_version")
 
     @cockroach_version.setter
     def cockroach_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cockroach_version", value)
@@ -317,14 +333,15 @@
                 raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             if regions is None and not opts.urn:
                 raise TypeError("Missing required property 'regions'")
             __props__.__dict__["regions"] = regions
             __props__.__dict__["serverless"] = serverless
             __props__.__dict__["account_id"] = None
+            __props__.__dict__["cluster_id"] = None
             __props__.__dict__["creator_id"] = None
             __props__.__dict__["operation_status"] = None
             __props__.__dict__["plan"] = None
             __props__.__dict__["state"] = None
             __props__.__dict__["upgrade_status"] = None
         super(Cluster, __self__).__init__(
             'cockroach:index/cluster:Cluster',
@@ -334,14 +351,15 @@
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             account_id: Optional[pulumi.Input[str]] = None,
             cloud_provider: Optional[pulumi.Input[str]] = None,
+            cluster_id: Optional[pulumi.Input[str]] = None,
             cockroach_version: Optional[pulumi.Input[str]] = None,
             creator_id: Optional[pulumi.Input[str]] = None,
             dedicated: Optional[pulumi.Input[pulumi.InputType['ClusterDedicatedArgs']]] = None,
             name: Optional[pulumi.Input[str]] = None,
             operation_status: Optional[pulumi.Input[str]] = None,
             plan: Optional[pulumi.Input[str]] = None,
             regions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterRegionArgs']]]]] = None,
@@ -351,22 +369,24 @@
         """
         Get an existing Cluster resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] cluster_id: The ID of this resource.
         :param pulumi.Input[str] name: Name of cluster
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ClusterState.__new__(_ClusterState)
 
         __props__.__dict__["account_id"] = account_id
         __props__.__dict__["cloud_provider"] = cloud_provider
+        __props__.__dict__["cluster_id"] = cluster_id
         __props__.__dict__["cockroach_version"] = cockroach_version
         __props__.__dict__["creator_id"] = creator_id
         __props__.__dict__["dedicated"] = dedicated
         __props__.__dict__["name"] = name
         __props__.__dict__["operation_status"] = operation_status
         __props__.__dict__["plan"] = plan
         __props__.__dict__["regions"] = regions
@@ -382,14 +402,22 @@
 
     @property
     @pulumi.getter(name="cloudProvider")
     def cloud_provider(self) -> pulumi.Output[str]:
         return pulumi.get(self, "cloud_provider")
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> pulumi.Output[str]:
+        """
+        The ID of this resource.
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @property
     @pulumi.getter(name="cockroachVersion")
     def cockroach_version(self) -> pulumi.Output[str]:
         return pulumi.get(self, "cockroach_version")
 
     @property
     @pulumi.getter(name="creatorId")
     def creator_id(self) -> pulumi.Output[str]:
```

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/cmek.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/cmek.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,29 +12,44 @@
 from ._inputs import *
 
 __all__ = ['CmekArgs', 'Cmek']
 
 @pulumi.input_type
 class CmekArgs:
     def __init__(__self__, *,
+                 cluster_id: pulumi.Input[str],
                  regions: pulumi.Input[Sequence[pulumi.Input['CmekRegionArgs']]],
                  additional_regions: Optional[pulumi.Input[Sequence[pulumi.Input['CmekAdditionalRegionArgs']]]] = None,
                  status: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Cmek resource.
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[Sequence[pulumi.Input['CmekAdditionalRegionArgs']]] additional_regions: Once CMEK is enabled for a cluster, no new regions can be added to the cluster resource, since they need encryption key info stored in the CMEK resource. New regions can be added and maintained here instead.
         :param pulumi.Input[str] status: Aggregated status of the cluster's encryption key(s)
         """
+        pulumi.set(__self__, "cluster_id", cluster_id)
         pulumi.set(__self__, "regions", regions)
         if additional_regions is not None:
             pulumi.set(__self__, "additional_regions", additional_regions)
         if status is not None:
             pulumi.set(__self__, "status", status)
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> pulumi.Input[str]:
+        """
+        Cluster ID
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @cluster_id.setter
+    def cluster_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "cluster_id", value)
+
+    @property
     @pulumi.getter
     def regions(self) -> pulumi.Input[Sequence[pulumi.Input['CmekRegionArgs']]]:
         return pulumi.get(self, "regions")
 
     @regions.setter
     def regions(self, value: pulumi.Input[Sequence[pulumi.Input['CmekRegionArgs']]]):
         pulumi.set(self, "regions", value)
@@ -64,23 +79,27 @@
         pulumi.set(self, "status", value)
 
 
 @pulumi.input_type
 class _CmekState:
     def __init__(__self__, *,
                  additional_regions: Optional[pulumi.Input[Sequence[pulumi.Input['CmekAdditionalRegionArgs']]]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  regions: Optional[pulumi.Input[Sequence[pulumi.Input['CmekRegionArgs']]]] = None,
                  status: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Cmek resources.
         :param pulumi.Input[Sequence[pulumi.Input['CmekAdditionalRegionArgs']]] additional_regions: Once CMEK is enabled for a cluster, no new regions can be added to the cluster resource, since they need encryption key info stored in the CMEK resource. New regions can be added and maintained here instead.
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[str] status: Aggregated status of the cluster's encryption key(s)
         """
         if additional_regions is not None:
             pulumi.set(__self__, "additional_regions", additional_regions)
+        if cluster_id is not None:
+            pulumi.set(__self__, "cluster_id", cluster_id)
         if regions is not None:
             pulumi.set(__self__, "regions", regions)
         if status is not None:
             pulumi.set(__self__, "status", status)
 
     @property
     @pulumi.getter(name="additionalRegions")
@@ -91,14 +110,26 @@
         return pulumi.get(self, "additional_regions")
 
     @additional_regions.setter
     def additional_regions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CmekAdditionalRegionArgs']]]]):
         pulumi.set(self, "additional_regions", value)
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        Cluster ID
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @cluster_id.setter
+    def cluster_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cluster_id", value)
+
+    @property
     @pulumi.getter
     def regions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CmekRegionArgs']]]]:
         return pulumi.get(self, "regions")
 
     @regions.setter
     def regions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CmekRegionArgs']]]]):
         pulumi.set(self, "regions", value)
@@ -118,23 +149,25 @@
 
 class Cmek(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  additional_regions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CmekAdditionalRegionArgs']]]]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  regions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CmekRegionArgs']]]]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Customer-managed encryption keys (CMEK) resource for a single cluster
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CmekAdditionalRegionArgs']]]] additional_regions: Once CMEK is enabled for a cluster, no new regions can be added to the cluster resource, since they need encryption key info stored in the CMEK resource. New regions can be added and maintained here instead.
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[str] status: Aggregated status of the cluster's encryption key(s)
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: CmekArgs,
@@ -154,26 +187,30 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  additional_regions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CmekAdditionalRegionArgs']]]]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  regions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CmekRegionArgs']]]]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = CmekArgs.__new__(CmekArgs)
 
             __props__.__dict__["additional_regions"] = additional_regions
+            if cluster_id is None and not opts.urn:
+                raise TypeError("Missing required property 'cluster_id'")
+            __props__.__dict__["cluster_id"] = cluster_id
             if regions is None and not opts.urn:
                 raise TypeError("Missing required property 'regions'")
             __props__.__dict__["regions"] = regions
             __props__.__dict__["status"] = status
         super(Cmek, __self__).__init__(
             'cockroach:index/cmek:Cmek',
             resource_name,
@@ -181,44 +218,55 @@
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             additional_regions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CmekAdditionalRegionArgs']]]]] = None,
+            cluster_id: Optional[pulumi.Input[str]] = None,
             regions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CmekRegionArgs']]]]] = None,
             status: Optional[pulumi.Input[str]] = None) -> 'Cmek':
         """
         Get an existing Cmek resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CmekAdditionalRegionArgs']]]] additional_regions: Once CMEK is enabled for a cluster, no new regions can be added to the cluster resource, since they need encryption key info stored in the CMEK resource. New regions can be added and maintained here instead.
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[str] status: Aggregated status of the cluster's encryption key(s)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _CmekState.__new__(_CmekState)
 
         __props__.__dict__["additional_regions"] = additional_regions
+        __props__.__dict__["cluster_id"] = cluster_id
         __props__.__dict__["regions"] = regions
         __props__.__dict__["status"] = status
         return Cmek(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="additionalRegions")
     def additional_regions(self) -> pulumi.Output[Optional[Sequence['outputs.CmekAdditionalRegion']]]:
         """
         Once CMEK is enabled for a cluster, no new regions can be added to the cluster resource, since they need encryption key info stored in the CMEK resource. New regions can be added and maintained here instead.
         """
         return pulumi.get(self, "additional_regions")
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> pulumi.Output[str]:
+        """
+        Cluster ID
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @property
     @pulumi.getter
     def regions(self) -> pulumi.Output[Sequence['outputs.CmekRegion']]:
         return pulumi.get(self, "regions")
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Output[str]:
```

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/config/vars.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/config/vars.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/database.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/database.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/get_cluster_cert.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/get_cluster_cert.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/get_cockroach_cluster.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/get_cockroach_cluster.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/get_connection_string.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/get_connection_string.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/get_organization.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/get_organization.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/get_person_user.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/get_person_user.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/log_export_config.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/log_export_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,28 +13,31 @@
 
 __all__ = ['LogExportConfigArgs', 'LogExportConfig']
 
 @pulumi.input_type
 class LogExportConfigArgs:
     def __init__(__self__, *,
                  auth_principal: pulumi.Input[str],
+                 cluster_id: pulumi.Input[str],
                  log_name: pulumi.Input[str],
                  type: pulumi.Input[str],
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input['LogExportConfigGroupArgs']]]] = None,
                  redact: Optional[pulumi.Input[bool]] = None,
                  region: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a LogExportConfig resource.
         :param pulumi.Input[str] auth_principal: Either the AWS Role ARN that identifies a role that the cluster account can assume to write to CloudWatch or the GCP Project ID that the cluster service account has permissions to write to for cloud logging
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[str] log_name: An identifier for the logs in the customer's log sink
         :param pulumi.Input[str] type: The cloud selection that we're exporting to along with the cloud logging platform. Possible values are `GCP_CLOUD_LOGGING` or `AWS_CLOUDWATCH`
         :param pulumi.Input[bool] redact: Controls whether logs are redacted before forwarding to customer sinks
         :param pulumi.Input[str] region: Controls whether all logs are sent to a specific region in the customer sink
         """
         pulumi.set(__self__, "auth_principal", auth_principal)
+        pulumi.set(__self__, "cluster_id", cluster_id)
         pulumi.set(__self__, "log_name", log_name)
         pulumi.set(__self__, "type", type)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if redact is not None:
             pulumi.set(__self__, "redact", redact)
         if region is not None:
@@ -49,14 +52,26 @@
         return pulumi.get(self, "auth_principal")
 
     @auth_principal.setter
     def auth_principal(self, value: pulumi.Input[str]):
         pulumi.set(self, "auth_principal", value)
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> pulumi.Input[str]:
+        """
+        Cluster ID
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @cluster_id.setter
+    def cluster_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "cluster_id", value)
+
+    @property
     @pulumi.getter(name="logName")
     def log_name(self) -> pulumi.Input[str]:
         """
         An identifier for the logs in the customer's log sink
         """
         return pulumi.get(self, "log_name")
 
@@ -110,33 +125,37 @@
         pulumi.set(self, "region", value)
 
 
 @pulumi.input_type
 class _LogExportConfigState:
     def __init__(__self__, *,
                  auth_principal: Optional[pulumi.Input[str]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  created_at: Optional[pulumi.Input[str]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input['LogExportConfigGroupArgs']]]] = None,
                  log_name: Optional[pulumi.Input[str]] = None,
                  redact: Optional[pulumi.Input[bool]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  updated_at: Optional[pulumi.Input[str]] = None,
                  user_message: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering LogExportConfig resources.
         :param pulumi.Input[str] auth_principal: Either the AWS Role ARN that identifies a role that the cluster account can assume to write to CloudWatch or the GCP Project ID that the cluster service account has permissions to write to for cloud logging
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[str] log_name: An identifier for the logs in the customer's log sink
         :param pulumi.Input[bool] redact: Controls whether logs are redacted before forwarding to customer sinks
         :param pulumi.Input[str] region: Controls whether all logs are sent to a specific region in the customer sink
         :param pulumi.Input[str] type: The cloud selection that we're exporting to along with the cloud logging platform. Possible values are `GCP_CLOUD_LOGGING` or `AWS_CLOUDWATCH`
         """
         if auth_principal is not None:
             pulumi.set(__self__, "auth_principal", auth_principal)
+        if cluster_id is not None:
+            pulumi.set(__self__, "cluster_id", cluster_id)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if log_name is not None:
             pulumi.set(__self__, "log_name", log_name)
         if redact is not None:
@@ -161,14 +180,26 @@
         return pulumi.get(self, "auth_principal")
 
     @auth_principal.setter
     def auth_principal(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "auth_principal", value)
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        Cluster ID
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @cluster_id.setter
+    def cluster_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cluster_id", value)
+
+    @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "created_at")
 
     @created_at.setter
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
@@ -260,26 +291,28 @@
 
 class LogExportConfig(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  auth_principal: Optional[pulumi.Input[str]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LogExportConfigGroupArgs']]]]] = None,
                  log_name: Optional[pulumi.Input[str]] = None,
                  redact: Optional[pulumi.Input[bool]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Log Export Config Resource
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] auth_principal: Either the AWS Role ARN that identifies a role that the cluster account can assume to write to CloudWatch or the GCP Project ID that the cluster service account has permissions to write to for cloud logging
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[str] log_name: An identifier for the logs in the customer's log sink
         :param pulumi.Input[bool] redact: Controls whether logs are redacted before forwarding to customer sinks
         :param pulumi.Input[str] region: Controls whether all logs are sent to a specific region in the customer sink
         :param pulumi.Input[str] type: The cloud selection that we're exporting to along with the cloud logging platform. Possible values are `GCP_CLOUD_LOGGING` or `AWS_CLOUDWATCH`
         """
         ...
     @overload
@@ -302,14 +335,15 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  auth_principal: Optional[pulumi.Input[str]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LogExportConfigGroupArgs']]]]] = None,
                  log_name: Optional[pulumi.Input[str]] = None,
                  redact: Optional[pulumi.Input[bool]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
@@ -319,14 +353,17 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = LogExportConfigArgs.__new__(LogExportConfigArgs)
 
             if auth_principal is None and not opts.urn:
                 raise TypeError("Missing required property 'auth_principal'")
             __props__.__dict__["auth_principal"] = auth_principal
+            if cluster_id is None and not opts.urn:
+                raise TypeError("Missing required property 'cluster_id'")
+            __props__.__dict__["cluster_id"] = cluster_id
             __props__.__dict__["groups"] = groups
             if log_name is None and not opts.urn:
                 raise TypeError("Missing required property 'log_name'")
             __props__.__dict__["log_name"] = log_name
             __props__.__dict__["redact"] = redact
             __props__.__dict__["region"] = region
             if type is None and not opts.urn:
@@ -343,14 +380,15 @@
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             auth_principal: Optional[pulumi.Input[str]] = None,
+            cluster_id: Optional[pulumi.Input[str]] = None,
             created_at: Optional[pulumi.Input[str]] = None,
             groups: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LogExportConfigGroupArgs']]]]] = None,
             log_name: Optional[pulumi.Input[str]] = None,
             redact: Optional[pulumi.Input[bool]] = None,
             region: Optional[pulumi.Input[str]] = None,
             status: Optional[pulumi.Input[str]] = None,
             type: Optional[pulumi.Input[str]] = None,
@@ -360,24 +398,26 @@
         Get an existing LogExportConfig resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] auth_principal: Either the AWS Role ARN that identifies a role that the cluster account can assume to write to CloudWatch or the GCP Project ID that the cluster service account has permissions to write to for cloud logging
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[str] log_name: An identifier for the logs in the customer's log sink
         :param pulumi.Input[bool] redact: Controls whether logs are redacted before forwarding to customer sinks
         :param pulumi.Input[str] region: Controls whether all logs are sent to a specific region in the customer sink
         :param pulumi.Input[str] type: The cloud selection that we're exporting to along with the cloud logging platform. Possible values are `GCP_CLOUD_LOGGING` or `AWS_CLOUDWATCH`
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _LogExportConfigState.__new__(_LogExportConfigState)
 
         __props__.__dict__["auth_principal"] = auth_principal
+        __props__.__dict__["cluster_id"] = cluster_id
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["groups"] = groups
         __props__.__dict__["log_name"] = log_name
         __props__.__dict__["redact"] = redact
         __props__.__dict__["region"] = region
         __props__.__dict__["status"] = status
         __props__.__dict__["type"] = type
@@ -390,14 +430,22 @@
     def auth_principal(self) -> pulumi.Output[str]:
         """
         Either the AWS Role ARN that identifies a role that the cluster account can assume to write to CloudWatch or the GCP Project ID that the cluster service account has permissions to write to for cloud logging
         """
         return pulumi.get(self, "auth_principal")
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> pulumi.Output[str]:
+        """
+        Cluster ID
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[str]:
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter
     def groups(self) -> pulumi.Output[Optional[Sequence['outputs.LogExportConfigGroup']]]:
```

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/maintenance_window.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/maintenance_window.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,25 +10,40 @@
 from . import _utilities
 
 __all__ = ['MaintenanceWindowArgs', 'MaintenanceWindow']
 
 @pulumi.input_type
 class MaintenanceWindowArgs:
     def __init__(__self__, *,
+                 cluster_id: pulumi.Input[str],
                  offset_duration: pulumi.Input[int],
                  window_duration: pulumi.Input[int]):
         """
         The set of arguments for constructing a MaintenanceWindow resource.
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[int] offset_duration: The offset duration is the duration in seconds from the beginning of each Monday (UTC) after which the maintenance window starts.
         :param pulumi.Input[int] window_duration: The window duration is the duration in seconds that the maintenance window will remain active for after it starts.
         """
+        pulumi.set(__self__, "cluster_id", cluster_id)
         pulumi.set(__self__, "offset_duration", offset_duration)
         pulumi.set(__self__, "window_duration", window_duration)
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> pulumi.Input[str]:
+        """
+        Cluster ID
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @cluster_id.setter
+    def cluster_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "cluster_id", value)
+
+    @property
     @pulumi.getter(name="offsetDuration")
     def offset_duration(self) -> pulumi.Input[int]:
         """
         The offset duration is the duration in seconds from the beginning of each Monday (UTC) after which the maintenance window starts.
         """
         return pulumi.get(self, "offset_duration")
 
@@ -48,27 +63,43 @@
     def window_duration(self, value: pulumi.Input[int]):
         pulumi.set(self, "window_duration", value)
 
 
 @pulumi.input_type
 class _MaintenanceWindowState:
     def __init__(__self__, *,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  offset_duration: Optional[pulumi.Input[int]] = None,
                  window_duration: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering MaintenanceWindow resources.
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[int] offset_duration: The offset duration is the duration in seconds from the beginning of each Monday (UTC) after which the maintenance window starts.
         :param pulumi.Input[int] window_duration: The window duration is the duration in seconds that the maintenance window will remain active for after it starts.
         """
+        if cluster_id is not None:
+            pulumi.set(__self__, "cluster_id", cluster_id)
         if offset_duration is not None:
             pulumi.set(__self__, "offset_duration", offset_duration)
         if window_duration is not None:
             pulumi.set(__self__, "window_duration", window_duration)
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        Cluster ID
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @cluster_id.setter
+    def cluster_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cluster_id", value)
+
+    @property
     @pulumi.getter(name="offsetDuration")
     def offset_duration(self) -> Optional[pulumi.Input[int]]:
         """
         The offset duration is the duration in seconds from the beginning of each Monday (UTC) after which the maintenance window starts.
         """
         return pulumi.get(self, "offset_duration")
 
@@ -90,22 +121,24 @@
 
 
 class MaintenanceWindow(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  offset_duration: Optional[pulumi.Input[int]] = None,
                  window_duration: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Maintenance window resource for a cluster.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[int] offset_duration: The offset duration is the duration in seconds from the beginning of each Monday (UTC) after which the maintenance window starts.
         :param pulumi.Input[int] window_duration: The window duration is the duration in seconds that the maintenance window will remain active for after it starts.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -125,25 +158,29 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  offset_duration: Optional[pulumi.Input[int]] = None,
                  window_duration: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = MaintenanceWindowArgs.__new__(MaintenanceWindowArgs)
 
+            if cluster_id is None and not opts.urn:
+                raise TypeError("Missing required property 'cluster_id'")
+            __props__.__dict__["cluster_id"] = cluster_id
             if offset_duration is None and not opts.urn:
                 raise TypeError("Missing required property 'offset_duration'")
             __props__.__dict__["offset_duration"] = offset_duration
             if window_duration is None and not opts.urn:
                 raise TypeError("Missing required property 'window_duration'")
             __props__.__dict__["window_duration"] = window_duration
         super(MaintenanceWindow, __self__).__init__(
@@ -152,35 +189,46 @@
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            cluster_id: Optional[pulumi.Input[str]] = None,
             offset_duration: Optional[pulumi.Input[int]] = None,
             window_duration: Optional[pulumi.Input[int]] = None) -> 'MaintenanceWindow':
         """
         Get an existing MaintenanceWindow resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[int] offset_duration: The offset duration is the duration in seconds from the beginning of each Monday (UTC) after which the maintenance window starts.
         :param pulumi.Input[int] window_duration: The window duration is the duration in seconds that the maintenance window will remain active for after it starts.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _MaintenanceWindowState.__new__(_MaintenanceWindowState)
 
+        __props__.__dict__["cluster_id"] = cluster_id
         __props__.__dict__["offset_duration"] = offset_duration
         __props__.__dict__["window_duration"] = window_duration
         return MaintenanceWindow(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> pulumi.Output[str]:
+        """
+        Cluster ID
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @property
     @pulumi.getter(name="offsetDuration")
     def offset_duration(self) -> pulumi.Output[int]:
         """
         The offset duration is the duration in seconds from the beginning of each Monday (UTC) after which the maintenance window starts.
         """
         return pulumi.get(self, "offset_duration")
```

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/metric_export_cloudwatch_config.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/metric_export_cloudwatch_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,30 +10,45 @@
 from . import _utilities
 
 __all__ = ['MetricExportCloudwatchConfigArgs', 'MetricExportCloudwatchConfig']
 
 @pulumi.input_type
 class MetricExportCloudwatchConfigArgs:
     def __init__(__self__, *,
+                 cluster_id: pulumi.Input[str],
                  role_arn: pulumi.Input[str],
                  log_group_name: Optional[pulumi.Input[str]] = None,
                  target_region: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a MetricExportCloudwatchConfig resource.
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[str] role_arn: The IAM role used to upload metric segments to the target AWS account.
         :param pulumi.Input[str] log_group_name: The customized AWS CloudWatch log group name.
         :param pulumi.Input[str] target_region: The specific AWS region that the metrics will be exported to.
         """
+        pulumi.set(__self__, "cluster_id", cluster_id)
         pulumi.set(__self__, "role_arn", role_arn)
         if log_group_name is not None:
             pulumi.set(__self__, "log_group_name", log_group_name)
         if target_region is not None:
             pulumi.set(__self__, "target_region", target_region)
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> pulumi.Input[str]:
+        """
+        Cluster ID
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @cluster_id.setter
+    def cluster_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "cluster_id", value)
+
+    @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> pulumi.Input[str]:
         """
         The IAM role used to upload metric segments to the target AWS account.
         """
         return pulumi.get(self, "role_arn")
 
@@ -65,37 +80,53 @@
     def target_region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "target_region", value)
 
 
 @pulumi.input_type
 class _MetricExportCloudwatchConfigState:
     def __init__(__self__, *,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  log_group_name: Optional[pulumi.Input[str]] = None,
                  role_arn: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  target_region: Optional[pulumi.Input[str]] = None,
                  user_message: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering MetricExportCloudwatchConfig resources.
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[str] log_group_name: The customized AWS CloudWatch log group name.
         :param pulumi.Input[str] role_arn: The IAM role used to upload metric segments to the target AWS account.
         :param pulumi.Input[str] target_region: The specific AWS region that the metrics will be exported to.
         """
+        if cluster_id is not None:
+            pulumi.set(__self__, "cluster_id", cluster_id)
         if log_group_name is not None:
             pulumi.set(__self__, "log_group_name", log_group_name)
         if role_arn is not None:
             pulumi.set(__self__, "role_arn", role_arn)
         if status is not None:
             pulumi.set(__self__, "status", status)
         if target_region is not None:
             pulumi.set(__self__, "target_region", target_region)
         if user_message is not None:
             pulumi.set(__self__, "user_message", user_message)
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        Cluster ID
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @cluster_id.setter
+    def cluster_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cluster_id", value)
+
+    @property
     @pulumi.getter(name="logGroupName")
     def log_group_name(self) -> Optional[pulumi.Input[str]]:
         """
         The customized AWS CloudWatch log group name.
         """
         return pulumi.get(self, "log_group_name")
 
@@ -147,23 +178,25 @@
 
 
 class MetricExportCloudwatchConfig(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  log_group_name: Optional[pulumi.Input[str]] = None,
                  role_arn: Optional[pulumi.Input[str]] = None,
                  target_region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Metric Export CloudWatch Config Resource
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[str] log_group_name: The customized AWS CloudWatch log group name.
         :param pulumi.Input[str] role_arn: The IAM role used to upload metric segments to the target AWS account.
         :param pulumi.Input[str] target_region: The specific AWS region that the metrics will be exported to.
         """
         ...
     @overload
     def __init__(__self__,
@@ -184,26 +217,30 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  log_group_name: Optional[pulumi.Input[str]] = None,
                  role_arn: Optional[pulumi.Input[str]] = None,
                  target_region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = MetricExportCloudwatchConfigArgs.__new__(MetricExportCloudwatchConfigArgs)
 
+            if cluster_id is None and not opts.urn:
+                raise TypeError("Missing required property 'cluster_id'")
+            __props__.__dict__["cluster_id"] = cluster_id
             __props__.__dict__["log_group_name"] = log_group_name
             if role_arn is None and not opts.urn:
                 raise TypeError("Missing required property 'role_arn'")
             __props__.__dict__["role_arn"] = role_arn
             __props__.__dict__["target_region"] = target_region
             __props__.__dict__["status"] = None
             __props__.__dict__["user_message"] = None
@@ -213,42 +250,53 @@
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            cluster_id: Optional[pulumi.Input[str]] = None,
             log_group_name: Optional[pulumi.Input[str]] = None,
             role_arn: Optional[pulumi.Input[str]] = None,
             status: Optional[pulumi.Input[str]] = None,
             target_region: Optional[pulumi.Input[str]] = None,
             user_message: Optional[pulumi.Input[str]] = None) -> 'MetricExportCloudwatchConfig':
         """
         Get an existing MetricExportCloudwatchConfig resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[str] log_group_name: The customized AWS CloudWatch log group name.
         :param pulumi.Input[str] role_arn: The IAM role used to upload metric segments to the target AWS account.
         :param pulumi.Input[str] target_region: The specific AWS region that the metrics will be exported to.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _MetricExportCloudwatchConfigState.__new__(_MetricExportCloudwatchConfigState)
 
+        __props__.__dict__["cluster_id"] = cluster_id
         __props__.__dict__["log_group_name"] = log_group_name
         __props__.__dict__["role_arn"] = role_arn
         __props__.__dict__["status"] = status
         __props__.__dict__["target_region"] = target_region
         __props__.__dict__["user_message"] = user_message
         return MetricExportCloudwatchConfig(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> pulumi.Output[str]:
+        """
+        Cluster ID
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @property
     @pulumi.getter(name="logGroupName")
     def log_group_name(self) -> pulumi.Output[str]:
         """
         The customized AWS CloudWatch log group name.
         """
         return pulumi.get(self, "log_group_name")
```

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/metric_export_datadog_config.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/metric_export_datadog_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,21 +11,24 @@
 
 __all__ = ['MetricExportDatadogConfigArgs', 'MetricExportDatadogConfig']
 
 @pulumi.input_type
 class MetricExportDatadogConfigArgs:
     def __init__(__self__, *,
                  api_key: pulumi.Input[str],
+                 cluster_id: pulumi.Input[str],
                  site: pulumi.Input[str]):
         """
         The set of arguments for constructing a MetricExportDatadogConfig resource.
         :param pulumi.Input[str] api_key: A Datadog API key
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[str] site: The Datadog region to export to
         """
         pulumi.set(__self__, "api_key", api_key)
+        pulumi.set(__self__, "cluster_id", cluster_id)
         pulumi.set(__self__, "site", site)
 
     @property
     @pulumi.getter(name="apiKey")
     def api_key(self) -> pulumi.Input[str]:
         """
         A Datadog API key
@@ -33,14 +36,26 @@
         return pulumi.get(self, "api_key")
 
     @api_key.setter
     def api_key(self, value: pulumi.Input[str]):
         pulumi.set(self, "api_key", value)
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> pulumi.Input[str]:
+        """
+        Cluster ID
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @cluster_id.setter
+    def cluster_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "cluster_id", value)
+
+    @property
     @pulumi.getter
     def site(self) -> pulumi.Input[str]:
         """
         The Datadog region to export to
         """
         return pulumi.get(self, "site")
 
@@ -49,24 +64,28 @@
         pulumi.set(self, "site", value)
 
 
 @pulumi.input_type
 class _MetricExportDatadogConfigState:
     def __init__(__self__, *,
                  api_key: Optional[pulumi.Input[str]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  site: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  user_message: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering MetricExportDatadogConfig resources.
         :param pulumi.Input[str] api_key: A Datadog API key
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[str] site: The Datadog region to export to
         """
         if api_key is not None:
             pulumi.set(__self__, "api_key", api_key)
+        if cluster_id is not None:
+            pulumi.set(__self__, "cluster_id", cluster_id)
         if site is not None:
             pulumi.set(__self__, "site", site)
         if status is not None:
             pulumi.set(__self__, "status", status)
         if user_message is not None:
             pulumi.set(__self__, "user_message", user_message)
 
@@ -79,14 +98,26 @@
         return pulumi.get(self, "api_key")
 
     @api_key.setter
     def api_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "api_key", value)
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        Cluster ID
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @cluster_id.setter
+    def cluster_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cluster_id", value)
+
+    @property
     @pulumi.getter
     def site(self) -> Optional[pulumi.Input[str]]:
         """
         The Datadog region to export to
         """
         return pulumi.get(self, "site")
 
@@ -115,22 +146,24 @@
 
 class MetricExportDatadogConfig(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  api_key: Optional[pulumi.Input[str]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  site: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Metric Export Datadog Config Resource
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] api_key: A Datadog API key
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[str] site: The Datadog region to export to
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: MetricExportDatadogConfigArgs,
@@ -150,27 +183,31 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  api_key: Optional[pulumi.Input[str]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  site: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = MetricExportDatadogConfigArgs.__new__(MetricExportDatadogConfigArgs)
 
             if api_key is None and not opts.urn:
                 raise TypeError("Missing required property 'api_key'")
             __props__.__dict__["api_key"] = None if api_key is None else pulumi.Output.secret(api_key)
+            if cluster_id is None and not opts.urn:
+                raise TypeError("Missing required property 'cluster_id'")
+            __props__.__dict__["cluster_id"] = cluster_id
             if site is None and not opts.urn:
                 raise TypeError("Missing required property 'site'")
             __props__.__dict__["site"] = site
             __props__.__dict__["status"] = None
             __props__.__dict__["user_message"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["apiKey"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
@@ -181,46 +218,57 @@
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             api_key: Optional[pulumi.Input[str]] = None,
+            cluster_id: Optional[pulumi.Input[str]] = None,
             site: Optional[pulumi.Input[str]] = None,
             status: Optional[pulumi.Input[str]] = None,
             user_message: Optional[pulumi.Input[str]] = None) -> 'MetricExportDatadogConfig':
         """
         Get an existing MetricExportDatadogConfig resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] api_key: A Datadog API key
+        :param pulumi.Input[str] cluster_id: Cluster ID
         :param pulumi.Input[str] site: The Datadog region to export to
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _MetricExportDatadogConfigState.__new__(_MetricExportDatadogConfigState)
 
         __props__.__dict__["api_key"] = api_key
+        __props__.__dict__["cluster_id"] = cluster_id
         __props__.__dict__["site"] = site
         __props__.__dict__["status"] = status
         __props__.__dict__["user_message"] = user_message
         return MetricExportDatadogConfig(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="apiKey")
     def api_key(self) -> pulumi.Output[str]:
         """
         A Datadog API key
         """
         return pulumi.get(self, "api_key")
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> pulumi.Output[str]:
+        """
+        Cluster ID
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @property
     @pulumi.getter
     def site(self) -> pulumi.Output[str]:
         """
         The Datadog region to export to
         """
         return pulumi.get(self, "site")
```

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/outputs.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/outputs.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/private_endpoint_connection.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/private_endpoint_connection.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/private_endpoint_services.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/private_endpoint_services.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/provider.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/provider.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/sql_user.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/sql_user.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach/user_role_grants.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach/user_role_grants.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach.egg-info/PKG-INFO` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbrlabs-pulumi-cockroach
-Version: 0.0.3a1689176685
+Version: 0.0.3a1689177795
 Summary: A Pulumi package to create and managed cockroach db resources in Pulumi programs.
 Home-page: https://lbrlabs.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/lbrlabs/pulumi-cockroach
 Description: 
         # Cockroach Resource Provider
```

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/lbrlabs_pulumi_cockroach.egg-info/SOURCES.txt` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/lbrlabs_pulumi_cockroach.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.3a1689176685/setup.py` & `lbrlabs_pulumi_cockroach-0.0.3a1689177795/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.3a1689176685"
-PLUGIN_VERSION = "0.0.3-alpha.1689176685+15c411bb"
+VERSION = "0.0.3a1689177795"
+PLUGIN_VERSION = "0.0.3-alpha.1689177795+5beb4e6c"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'cockroach', PLUGIN_VERSION, '--server', 'github://api.github.com/lbrlabs'])
         except OSError as error:
```


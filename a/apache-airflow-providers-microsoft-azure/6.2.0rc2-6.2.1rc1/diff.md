# Comparing `tmp/apache-airflow-providers-microsoft-azure-6.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-microsoft-azure-6.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-microsoft-azure-6.2.0rc2.tar", last modified: Thu Jul  6 04:51:05 2023, max compression
+gzip compressed data, was "apache-airflow-providers-microsoft-azure-6.2.1rc1.tar", last modified: Wed Jul 12 19:13:31 2023, max compression
```

## Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2.tar` & `apache-airflow-providers-microsoft-azure-6.2.1rc1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:05.200615 apache-airflow-providers-microsoft-azure-6.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:51:03.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6595 2023-07-06 04:51:05.201209 apache-airflow-providers-microsoft-azure-6.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4854 2023-07-06 04:51:03.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:04.986815 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:04.987949 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:04.989041 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:05.033417 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/
--rw-r--r--   0 root         (0) root         (0)     1540 2023-07-05 18:52:15.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:05.042218 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/example_dag/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-04 06:09:02.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/example_dag/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1900 2023-07-04 06:09:02.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/example_dag/example_cosmos_document_sensor.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-07-04 06:09:02.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/example_dag/example_wasb_sensors.py
--rw-r--r--   0 root         (0) root         (0)    17240 2023-07-06 04:51:03.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:05.086395 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8759 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/adx.py
--rw-r--r--   0 root         (0) root         (0)    10984 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/asb.py
--rw-r--r--   0 root         (0) root         (0)     4785 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/base_azure.py
--rw-r--r--   0 root         (0) root         (0)    15302 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/batch.py
--rw-r--r--   0 root         (0) root         (0)     6183 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/container_instance.py
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/container_registry.py
--rw-r--r--   0 root         (0) root         (0)     4062 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/container_volume.py
--rw-r--r--   0 root         (0) root         (0)    14177 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/cosmos.py
--rw-r--r--   0 root         (0) root         (0)    44145 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/data_factory.py
--rw-r--r--   0 root         (0) root         (0)    22133 2023-06-28 06:26:40.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/data_lake.py
--rw-r--r--   0 root         (0) root         (0)    13004 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/fileshare.py
--rw-r--r--   0 root         (0) root         (0)     7320 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/synapse.py
--rw-r--r--   0 root         (0) root         (0)    29041 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:05.092474 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10038 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/log/wasb_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:05.123257 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3789 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/adls.py
--rw-r--r--   0 root         (0) root         (0)     3032 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/adx.py
--rw-r--r--   0 root         (0) root         (0)    29255 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/asb.py
--rw-r--r--   0 root         (0) root         (0)    16254 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)    15968 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/container_instances.py
--rw-r--r--   0 root         (0) root         (0)     2782 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/cosmos.py
--rw-r--r--   0 root         (0) root         (0)    12525 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     4422 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/synapse.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:05.129058 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7891 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/secrets/key_vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:05.140698 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2637 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/sensors/cosmos.py
--rw-r--r--   0 root         (0) root         (0)     5896 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/sensors/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     8065 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/sensors/wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:05.164717 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4641 2023-06-17 16:45:00.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     4817 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/transfers/local_to_adls.py
--rw-r--r--   0 root         (0) root         (0)     2936 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
--rw-r--r--   0 root         (0) root         (0)     4475 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
--rw-r--r--   0 root         (0) root         (0)     8202 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:05.174119 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11197 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/triggers/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     7382 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/triggers/wasb.py
--rw-r--r--   0 root         (0) root         (0)     2821 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:05.198349 apache-airflow-providers-microsoft-azure-6.2.0rc2/apache_airflow_providers_microsoft_azure.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6595 2023-07-06 04:51:04.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3152 2023-07-06 04:51:04.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:04.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/apache_airflow_providers_microsoft_azure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-07-06 04:51:04.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/apache_airflow_providers_microsoft_azure.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:04.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/apache_airflow_providers_microsoft_azure.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      609 2023-07-06 04:51:04.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/apache_airflow_providers_microsoft_azure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:51:04.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/apache_airflow_providers_microsoft_azure.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2465 2023-07-06 04:51:05.203609 apache-airflow-providers-microsoft-azure-6.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1874 2023-07-06 04:51:03.000000 apache-airflow-providers-microsoft-azure-6.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.581397 apache-airflow-providers-microsoft-azure-6.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-12 19:13:30.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6595 2023-07-12 19:13:31.581936 apache-airflow-providers-microsoft-azure-6.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4854 2023-07-12 19:13:30.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.377077 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.378193 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.379220 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.423358 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-12 19:08:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.432138 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/example_dag/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-04 06:09:02.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/example_dag/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-07-04 06:09:02.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/example_dag/example_cosmos_document_sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-07-04 06:09:02.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/example_dag/example_wasb_sensors.py
+-rw-r--r--   0 root         (0) root         (0)    17536 2023-07-12 19:13:30.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.473019 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8759 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/adx.py
+-rw-r--r--   0 root         (0) root         (0)    10984 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/asb.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/base_azure.py
+-rw-r--r--   0 root         (0) root         (0)    15302 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/batch.py
+-rw-r--r--   0 root         (0) root         (0)     6183 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/container_instance.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/container_registry.py
+-rw-r--r--   0 root         (0) root         (0)     4062 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/container_volume.py
+-rw-r--r--   0 root         (0) root         (0)    14177 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)    44145 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)    22133 2023-06-28 06:26:40.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/data_lake.py
+-rw-r--r--   0 root         (0) root         (0)    13004 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/fileshare.py
+-rw-r--r--   0 root         (0) root         (0)     7320 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/synapse.py
+-rw-r--r--   0 root         (0) root         (0)    29495 2023-07-12 17:52:12.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.478925 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.507784 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/adls.py
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/adx.py
+-rw-r--r--   0 root         (0) root         (0)    29255 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/asb.py
+-rw-r--r--   0 root         (0) root         (0)    16254 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)    15968 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/container_instances.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)    12525 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/synapse.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.513580 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7891 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/secrets/key_vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.524663 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)     5896 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     8065 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.541506 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2023-07-09 14:40:47.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     4817 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
+-rw-r--r--   0 root         (0) root         (0)     4475 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
+-rw-r--r--   0 root         (0) root         (0)     8202 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.550009 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11197 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/triggers/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7382 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/triggers/wasb.py
+-rw-r--r--   0 root         (0) root         (0)     2821 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.578400 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6595 2023-07-12 19:13:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-07-12 19:13:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-12 19:13:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      609 2023-07-12 19:13:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:13:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2465 2023-07-12 19:13:31.583989 apache-airflow-providers-microsoft-azure-6.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-07-12 19:13:30.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/LICENSE` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/MANIFEST.in` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/PKG-INFO` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-azure
-Version: 6.2.0rc2
+Version: 6.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-azure package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -69,28 +69,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``6.2.0rc2``
+Release: ``6.2.1rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.azure`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.azure`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -142,8 +142,8 @@
 ====================================================================================================  ==========
 `apache-airflow-providers-google <https://airflow.apache.org/docs/apache-airflow-providers-google>`_  ``google``
 `apache-airflow-providers-oracle <https://airflow.apache.org/docs/apache-airflow-providers-oracle>`_  ``oracle``
 `apache-airflow-providers-sftp <https://airflow.apache.org/docs/apache-airflow-providers-sftp>`_      ``sftp``
 ====================================================================================================  ==========
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/README.rst` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``6.2.0rc2``
+Release: ``6.2.1rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.azure`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.azure`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -105,8 +105,8 @@
 ====================================================================================================  ==========
 `apache-airflow-providers-google <https://airflow.apache.org/docs/apache-airflow-providers-google>`_  ``google``
 `apache-airflow-providers-oracle <https://airflow.apache.org/docs/apache-airflow-providers-oracle>`_  ``oracle``
 `apache-airflow-providers-sftp <https://airflow.apache.org/docs/apache-airflow-providers-sftp>`_      ``sftp``
 ====================================================================================================  ==========
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "6.2.0"
+__version__ = "6.2.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/example_dag/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/example_dag/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/example_dag/example_cosmos_document_sensor.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/example_dag/example_cosmos_document_sensor.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/example_dag/example_wasb_sensors.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/example_dag/example_wasb_sensors.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/get_provider_info.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-microsoft-azure",
         "name": "Microsoft Azure",
         "description": "`Microsoft Azure <https://azure.microsoft.com/>`__\n",
         "suspended": False,
         "versions": [
+            "6.2.1",
             "6.2.0",
             "6.1.2",
             "6.1.1",
             "6.1.0",
             "6.0.0",
             "5.3.1",
             "5.3.0",
@@ -305,23 +306,28 @@
                 "target-integration-name": "Microsoft Azure Blob Storage",
                 "how-to-guide": "/docs/apache-airflow-providers-microsoft-azure/transfer/local_to_wasb.rst",
                 "python-module": "airflow.providers.microsoft.azure.transfers.local_to_wasb",
             },
             {
                 "source-integration-name": "Microsoft Azure Blob Storage",
                 "target-integration-name": "Google Cloud Storage (GCS)",
-                "how-to-guide": "/docs/apache-airflow-providers-microsoft-azure/transfer/azure_blob_to_gcs.rst",
                 "python-module": "airflow.providers.microsoft.azure.transfers.azure_blob_to_gcs",
             },
             {
                 "source-integration-name": "SSH File Transfer Protocol (SFTP)",
                 "target-integration-name": "Microsoft Azure Blob Storage",
                 "how-to-guide": "/docs/apache-airflow-providers-microsoft-azure/transfer/sftp_to_wasb.rst",
                 "python-module": "airflow.providers.microsoft.azure.transfers.sftp_to_wasb",
             },
+            {
+                "source-integration-name": "Microsoft Azure Blob Storage",
+                "target-integration-name": "Google Cloud Storage (GCS)",
+                "how-to-guide": "/docs/apache-airflow-providers-microsoft-azure/transfer/azure_blob_to_gcs.rst",
+                "python-module": "airflow.providers.microsoft.azure.transfers.azure_blob_to_gcs",
+            },
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.microsoft.azure.hooks.base_azure.AzureBaseHook",
                 "connection-type": "azure",
             },
             {
```

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/adx.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/adx.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/asb.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/asb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/base_azure.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/base_azure.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/batch.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/container_instance.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/container_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/container_registry.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/container_registry.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/container_volume.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/container_volume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/data_lake.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/data_lake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/fileshare.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/fileshare.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/synapse.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/synapse.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/hooks/wasb.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/wasb.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,21 +206,27 @@
             return BlobServiceClient(account_url=account_url, credential=shared_access_key, **extra)
 
         sas_token = self._get_field(extra, "sas_token")
         if sas_token:
             if sas_token.startswith("https"):
                 return BlobServiceClient(account_url=sas_token, **extra)
             else:
-                return BlobServiceClient(account_url=f"{account_url}/{sas_token}", **extra)
+                if not account_url.startswith("https://"):
+                    # TODO: require url in the host field in the next major version?
+                    account_url = f"https://{conn.login}.blob.core.windows.net"
+                return BlobServiceClient(account_url=f"{account_url.rstrip('/')}/{sas_token}", **extra)
 
         # Fall back to old auth (password) or use managed identity if not provided.
         credential = conn.password
         if not credential:
             credential = DefaultAzureCredential()
             self.log.info("Using DefaultAzureCredential as credential")
+        if not account_url.startswith("https://"):
+            # TODO: require url in the host field in the next major version?
+            account_url = f"https://{conn.login}.blob.core.windows.net/"
         return BlobServiceClient(
             account_url=account_url,
             credential=credential,
             **extra,
         )
 
     def _get_container_client(self, container_name: str) -> ContainerClient:
@@ -683,18 +689,18 @@
             begin with the specified prefix.
         :param include: specifies one or more additional datasets to include in the
             response. Options include: ``snapshots``, ``metadata``, ``uncommittedblobs``,
             ``copy`, ``deleted``.
         :param delimiter: filters objects based on the delimiter (for e.g '.csv')
         """
         container = self._get_container_client(container_name)
-        blob_list = []
+        blob_list: list[BlobProperties] = []
         blobs = container.walk_blobs(name_starts_with=prefix, include=include, delimiter=delimiter, **kwargs)
         async for blob in blobs:
-            blob_list.append(blob.name)
+            blob_list.append(blob)
         return blob_list
 
     async def check_for_prefix_async(self, container_name: str, prefix: str, **kwargs: Any) -> bool:
         """
         Check if a prefix exists on Azure Blob storage.
 
         :param container_name: Name of the container.
```

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/log/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/log/wasb_task_handler.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/adls.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/adls.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/adx.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/adx.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/asb.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/asb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/batch.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/container_instances.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/container_instances.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/synapse.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/synapse.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/secrets/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/secrets/key_vault.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/secrets/key_vault.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/sensors/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/sensors/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/sensors/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/sensors/wasb.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/transfers/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/transfers/local_to_adls.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/transfers/local_to_wasb.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/triggers/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/triggers/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/triggers/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/triggers/wasb.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/triggers/wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/airflow/providers/microsoft/azure/utils.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/utils.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-azure
-Version: 6.2.0rc2
+Version: 6.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-azure package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -69,28 +69,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``6.2.0rc2``
+Release: ``6.2.1rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.azure`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.azure`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -142,8 +142,8 @@
 ====================================================================================================  ==========
 `apache-airflow-providers-google <https://airflow.apache.org/docs/apache-airflow-providers-google>`_  ``google``
 `apache-airflow-providers-oracle <https://airflow.apache.org/docs/apache-airflow-providers-oracle>`_  ``oracle``
 `apache-airflow-providers-sftp <https://airflow.apache.org/docs/apache-airflow-providers-sftp>`_      ``sftp``
 ====================================================================================================  ==========
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/apache_airflow_providers_microsoft_azure.egg-info/requires.txt` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/pyproject.toml` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/setup.cfg` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.1/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.1/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -70,10 +70,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.microsoft.azure.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.microsoft.azure
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-microsoft-azure-6.2.0rc2/setup.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-microsoft-azure package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "6.2.0"
+version = "6.2.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-microsoft-azure setup."""
     setup(
         version=version,
         extras_require={
```


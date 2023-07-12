# Comparing `tmp/apache-airflow-providers-cncf-kubernetes-7.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-cncf-kubernetes-7.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-cncf-kubernetes-7.2.0rc2.tar", last modified: Thu Jul  6 04:50:31 2023, max compression
+gzip compressed data, was "apache-airflow-providers-cncf-kubernetes-7.3.0rc1.tar", last modified: Wed Jul 12 19:13:20 2023, max compression
```

## Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2.tar` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:31.044342 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1156 2023-07-06 04:50:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4637 2023-07-06 04:50:31.044953 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2963 2023-07-06 04:50:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.896052 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.897373 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.898543 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.955705 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/
--rw-r--r--   0 root         (0) root         (0)     1540 2023-07-05 18:48:19.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.961583 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/backcompat/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/backcompat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.968046 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6178 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     4483 2023-07-06 04:50:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.974522 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23125 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.991405 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    40772 2023-07-05 07:19:39.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/pod.py
--rw-r--r--   0 root         (0) root         (0)     3827 2023-06-08 05:42:54.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/resource.py
--rw-r--r--   0 root         (0) root         (0)     6484 2023-06-28 06:26:40.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
--rw-r--r--   0 root         (0) root         (0)     3345 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.997085 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5226 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:31.005609 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1152 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    11941 2023-06-30 08:49:17.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/triggers/pod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:31.017562 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/
--rw-r--r--   0 root         (0) root         (0)      863 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5176 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/delete_from.py
--rw-r--r--   0 root         (0) root         (0)    24797 2023-07-01 06:49:42.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/pod_manager.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:31.041692 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4637 2023-07-06 04:50:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1893 2023-07-06 04:50:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-07-06 04:50:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      117 2023-07-06 04:50:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2082 2023-07-06 04:50:31.046894 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1692 2023-07-06 04:50:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.421423 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-07-12 19:13:19.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4637 2023-07-12 19:13:20.422013 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-07-12 19:13:19.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.285314 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.286510 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.287650 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.338150 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-12 19:08:31.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.343829 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.349520 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     4504 2023-07-12 19:13:19.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.355146 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23125 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.370152 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    40898 2023-07-12 12:42:21.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
+-rw-r--r--   0 root         (0) root         (0)     3827 2023-06-08 05:42:54.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py
+-rw-r--r--   0 root         (0) root         (0)     6484 2023-06-28 06:26:40.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.375749 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.384149 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    11511 2023-07-12 12:42:21.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.395876 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/
+-rw-r--r--   0 root         (0) root         (0)      863 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5176 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
+-rw-r--r--   0 root         (0) root         (0)    28931 2023-07-09 14:40:47.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.418731 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4637 2023-07-12 19:13:20.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-07-12 19:13:20.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:20.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-12 19:13:20.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:20.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      117 2023-07-12 19:13:20.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:13:20.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-07-12 19:13:20.423922 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-12 19:13:19.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/LICENSE` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/MANIFEST.in` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 7.2.0rc2
+Version: 7.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -66,28 +66,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.2.0rc2``
+Release: ``7.3.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -105,8 +105,8 @@
 ``asgiref``             ``>=3.5.2``
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=21.7.0,<24``
 ``kubernetes_asyncio``  ``>=18.20.1,<25``
 ======================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/README.rst` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.2.0rc2``
+Release: ``7.3.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -71,8 +71,8 @@
 ``asgiref``             ``>=3.5.2``
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=21.7.0,<24``
 ``kubernetes_asyncio``  ``>=18.20.1,<25``
 ======================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "7.2.0"
+__version__ = "7.3.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/backcompat/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/decorators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/decorators/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/get_provider_info.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-cncf-kubernetes",
         "name": "Kubernetes",
         "description": "`Kubernetes <https://kubernetes.io/>`__\n",
         "suspended": False,
         "versions": [
+            "7.3.0",
             "7.2.0",
             "7.1.0",
             "7.0.0",
             "6.1.0",
             "6.0.0",
             "5.3.0",
             "5.2.2",
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/hooks/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/hooks/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import re
 import secrets
 import string
 import warnings
 from collections.abc import Container
 from contextlib import AbstractContextManager
 from functools import cached_property
-from typing import TYPE_CHECKING, Any, Sequence
+from typing import TYPE_CHECKING, Any, Iterable, Sequence
 
 from kubernetes.client import CoreV1Api, models as k8s
 from slugify import slugify
 from urllib3.exceptions import HTTPError
 
 from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning, AirflowSkipException
@@ -58,14 +58,15 @@
     PodLaunchFailedException,
     PodManager,
     PodOperatorHookProtocol,
     PodPhase,
     get_container_termination_message,
 )
 from airflow.settings import pod_mutation_hook
+from airflow.typing_compat import Literal
 from airflow.utils import yaml
 from airflow.utils.helpers import prune_dict, validate_key
 from airflow.utils.timezone import utcnow
 from airflow.version import version as airflow_version
 
 if TYPE_CHECKING:
     import jinja2
@@ -174,14 +175,18 @@
     :param cluster_context: context that points to kubernetes cluster.
         Ignored when in_cluster is True. If None, current-context is used.
     :param reattach_on_restart: if the worker dies while the pod is running, reattach and monitor
         during the next try. If False, always create a new pod for each try.
     :param labels: labels to apply to the Pod. (templated)
     :param startup_timeout_seconds: timeout in seconds to startup the pod.
     :param get_logs: get the stdout of the base container as logs of the tasks.
+    :param container_logs: list of containers whose logs will be published to stdout
+        Takes a sequence of containers, a single container name or True. If True,
+        all the containers logs are published. Works in conjunction with get_logs param.
+        The default value is the base container.
     :param image_pull_policy: Specify a policy to cache or always pull an image.
     :param annotations: non-identifying metadata you can attach to the Pod.
         Can be a large range of data, and can include characters
         that are not permitted by labels.
     :param container_resources: resources for the launched pod. (templated)
     :param affinity: affinity scheduling rules for the launched pod.
     :param config_file: The path to the Kubernetes config file. (templated)
@@ -274,14 +279,15 @@
         secrets: list[Secret] | None = None,
         in_cluster: bool | None = None,
         cluster_context: str | None = None,
         labels: dict | None = None,
         reattach_on_restart: bool = True,
         startup_timeout_seconds: int = 120,
         get_logs: bool = True,
+        container_logs: Iterable[str] | str | Literal[True] = BASE_CONTAINER_NAME,
         image_pull_policy: str | None = None,
         annotations: dict | None = None,
         container_resources: k8s.V1ResourceRequirements | None = None,
         affinity: k8s.V1Affinity | None = None,
         config_file: str | None = None,
         node_selector: dict | None = None,
         image_pull_secrets: list[k8s.V1LocalObjectReference] | None = None,
@@ -346,14 +352,19 @@
         self.volume_mounts = [convert_volume_mount(v) for v in volume_mounts] if volume_mounts else []
         self.volumes = [convert_volume(volume) for volume in volumes] if volumes else []
         self.secrets = secrets or []
         self.in_cluster = in_cluster
         self.cluster_context = cluster_context
         self.reattach_on_restart = reattach_on_restart
         self.get_logs = get_logs
+        self.container_logs = container_logs
+        if self.container_logs == KubernetesPodOperator.BASE_CONTAINER_NAME:
+            self.container_logs = (
+                base_container_name if base_container_name else KubernetesPodOperator.BASE_CONTAINER_NAME
+            )
         self.image_pull_policy = image_pull_policy
         self.node_selector = node_selector or {}
         self.annotations = annotations or {}
         self.affinity = convert_affinity(affinity) if affinity else {}
         self.container_resources = container_resources
         self.config_file = config_file
         self.image_pull_secrets = convert_image_pull_secrets(image_pull_secrets) if image_pull_secrets else []
@@ -568,19 +579,18 @@
             ti.xcom_push(key="pod_namespace", value=self.pod.metadata.namespace)
 
             # get remote pod for use in cleanup methods
             self.remote_pod = self.find_pod(self.pod.metadata.namespace, context=context)
             self.await_pod_start(pod=self.pod)
 
             if self.get_logs:
-                self.pod_manager.fetch_container_logs(
+                self.pod_manager.fetch_requested_container_logs(
                     pod=self.pod,
-                    container_name=self.base_container_name,
-                    follow=True,
-                    post_termination_timeout=self.POST_TERMINATION_TIMEOUT,
+                    container_logs=self.container_logs,
+                    follow_logs=True,
                 )
             else:
                 self.pod_manager.await_container_completion(
                     pod=self.pod, container_name=self.base_container_name
                 )
 
             if self.do_xcom_push:
@@ -622,23 +632,19 @@
                 on_finish_action=self.on_finish_action.value,
             ),
             method_name="execute_complete",
         )
 
     def execute_complete(self, context: Context, event: dict, **kwargs):
         pod = None
-        remote_pod = None
         try:
             pod = self.hook.get_pod(
                 event["name"],
                 event["namespace"],
             )
-            # It is done to coincide with the current implementation of the general logic of the cleanup
-            # method. If it's going to be remade in future then it must be changed
-            remote_pod = pod
             if event["status"] in ("error", "failed", "timeout"):
                 # fetch some logs when pod is failed
                 if self.get_logs:
                     self.write_logs(pod)
                 raise AirflowException(event["message"])
             elif event["status"] == "success":
                 ti = context["ti"]
@@ -647,24 +653,21 @@
 
                 # fetch some logs when pod is executed successfully
                 if self.get_logs:
                     self.write_logs(pod)
 
                 if self.do_xcom_push:
                     xcom_sidecar_output = self.extract_xcom(pod=pod)
-                    pod = self.pod_manager.await_pod_completion(pod)
-                    # It is done to coincide with the current implementation of the general logic of
-                    # the cleanup method. If it's going to be remade in future then it must be changed
-                    remote_pod = pod
                     return xcom_sidecar_output
         finally:
-            if pod is not None and remote_pod is not None:
+            pod = self.pod_manager.await_pod_completion(pod)
+            if pod is not None:
                 self.post_complete_action(
                     pod=pod,
-                    remote_pod=remote_pod,
+                    remote_pod=pod,
                 )
 
     def write_logs(self, pod: k8s.V1Pod):
         try:
             logs = self.pod_manager.read_pod_logs(
                 pod=pod,
                 container_name=self.base_container_name,
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/resource.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/sensors/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/triggers/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/triggers/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,31 +150,23 @@
                 pod_status = pod.status.phase
                 self.log.debug("Pod %s status: %s", self.pod_name, pod_status)
 
                 container_state = self.define_container_state(pod)
                 self.log.debug("Container %s status: %s", self.base_container_name, container_state)
 
                 if container_state == ContainerState.TERMINATED:
-                    if pod_status not in PodPhase.terminal_states:
-                        self.log.info(
-                            "Pod %s is still running. Sleeping for %s seconds.",
-                            self.pod_name,
-                            self.poll_interval,
-                        )
-                        await asyncio.sleep(self.poll_interval)
-                    else:
-                        yield TriggerEvent(
-                            {
-                                "name": self.pod_name,
-                                "namespace": self.pod_namespace,
-                                "status": "success",
-                                "message": "All containers inside pod have started successfully.",
-                            }
-                        )
-                        return
+                    yield TriggerEvent(
+                        {
+                            "name": self.pod_name,
+                            "namespace": self.pod_namespace,
+                            "status": "success",
+                            "message": "All containers inside pod have started successfully.",
+                        }
+                    )
+                    return
                 elif self.should_wait(pod_phase=pod_status, container_state=container_state):
                     self.log.info("Container is not completed and still working.")
 
                     if pod_status == PodPhase.PENDING and container_state == ContainerState.UNDEFINED:
                         delta = datetime.now(tz=pytz.UTC) - self.trigger_start_time
                         if delta.total_seconds() >= self.startup_timeout:
                             message = (
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/delete_from.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/pod_manager.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 import enum
 import json
 import logging
 import math
 import time
 import warnings
+from collections.abc import Iterable
 from contextlib import closing, suppress
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from typing import TYPE_CHECKING, Generator, cast
 
 import pendulum
 import tenacity
@@ -39,15 +40,15 @@
 from pendulum.parsing.exceptions import ParserError
 from tenacity import before_log
 from urllib3.exceptions import HTTPError as BaseHTTPError
 from urllib3.response import HTTPResponse
 
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.kubernetes.pod_generator import PodDefaults
-from airflow.typing_compat import Protocol
+from airflow.typing_compat import Literal, Protocol
 from airflow.utils.log.logging_mixin import LoggingMixin
 from airflow.utils.timezone import utcnow
 
 if TYPE_CHECKING:
     from kubernetes.client.models.core_v1_event_list import CoreV1EventList
 
 
@@ -121,14 +122,26 @@
     """
     container_status = get_container_status(pod, container_name)
     if not container_status:
         return False
     return container_status.state.running is not None
 
 
+def container_is_completed(pod: V1Pod, container_name: str) -> bool:
+    """
+    Examines V1Pod ``pod`` to determine whether ``container_name`` is completed.
+
+    If that container is present and completed, returns True.  Returns False otherwise.
+    """
+    container_status = get_container_status(pod, container_name)
+    if not container_status:
+        return False
+    return container_status.state.terminated is not None
+
+
 def container_is_terminated(pod: V1Pod, container_name: str) -> bool:
     """
     Examines V1Pod ``pod`` to determine whether ``container_name`` is terminated.
 
     If that container is present and terminated, returns True.  Returns False otherwise.
     """
     container_statuses = pod.status.container_statuses if pod and pod.status else None
@@ -375,19 +388,20 @@
                     ),
                     follow=follow,
                     post_termination_timeout=termination_timeout,
                 )
                 for raw_line in logs:
                     line = raw_line.decode("utf-8", errors="backslashreplace")
                     timestamp, message = self.parse_log_line(line)
-                    self.log.info(message)
+                    self.log.info("[%s] %s", container_name, message)
             except BaseHTTPError as e:
                 self.log.warning(
-                    "Reading of logs interrupted with error %r; will retry. "
+                    "Reading of logs interrupted for container %r with error %r; will retry. "
                     "Set log level to DEBUG for traceback.",
+                    container_name,
                     e,
                 )
                 self.log.debug(
                     "Traceback for interrupted logs read for pod %r",
                     pod.metadata.name,
                     exc_info=True,
                 )
@@ -409,22 +423,87 @@
                 self.log.warning(
                     "Pod %s log read interrupted but container %s still running",
                     pod.metadata.name,
                     container_name,
                 )
                 time.sleep(1)
 
+    def fetch_requested_container_logs(
+        self, pod: V1Pod, container_logs: Iterable[str] | str | Literal[True], follow_logs=False
+    ) -> list[PodLoggingStatus]:
+        """
+        Follow the logs of containers in the specified pod and publish it to airflow logging.
+
+        Returns when all the containers exit.
+        """
+        pod_logging_statuses = []
+        all_containers = self.get_container_names(pod)
+        if len(all_containers) == 0:
+            self.log.error("Could not retrieve containers for the pod: %s", pod.metadata.name)
+        else:
+            if isinstance(container_logs, str):
+                # fetch logs only for requested container if only one container is provided
+                if container_logs in all_containers:
+                    status = self.fetch_container_logs(
+                        pod=pod, container_name=container_logs, follow=follow_logs
+                    )
+                    pod_logging_statuses.append(status)
+                else:
+                    self.log.error(
+                        "container %s whose logs were requested not found in the pod %s",
+                        container_logs,
+                        pod.metadata.name,
+                    )
+            elif isinstance(container_logs, bool):
+                # if True is provided, get logs for all the containers
+                if container_logs is True:
+                    for container_name in all_containers:
+                        status = self.fetch_container_logs(
+                            pod=pod, container_name=container_name, follow=follow_logs
+                        )
+                        pod_logging_statuses.append(status)
+                else:
+                    self.log.error(
+                        "False is not a valid value for container_logs",
+                    )
+            else:
+                # if a sequence of containers are provided, iterate for every container in the pod
+                if isinstance(container_logs, Iterable):
+                    for container in container_logs:
+                        if container in all_containers:
+                            status = self.fetch_container_logs(
+                                pod=pod, container_name=container, follow=follow_logs
+                            )
+                            pod_logging_statuses.append(status)
+                        else:
+                            self.log.error(
+                                "Container %s whose logs were requests not found in the pod %s",
+                                container,
+                                pod.metadata.name,
+                            )
+                else:
+                    self.log.error(
+                        "Invalid type %s specified for container names input parameter", type(container_logs)
+                    )
+
+        return pod_logging_statuses
+
     def await_container_completion(self, pod: V1Pod, container_name: str) -> None:
         """
         Waits for the given container in the given pod to be completed.
 
         :param pod: pod spec that will be monitored
         :param container_name: name of the container within the pod to monitor
         """
-        while not self.container_is_terminated(pod=pod, container_name=container_name):
+        while True:
+            remote_pod = self.read_pod(pod)
+            terminated = container_is_completed(remote_pod, container_name)
+            if terminated:
+                break
+            self.log.info("Waiting for container '%s' state to be completed", container_name)
             time.sleep(1)
 
     def await_pod_completion(self, pod: V1Pod) -> V1Pod:
         """
         Monitors a pod and returns the final state.
 
         :param pod: pod spec that will be monitored
@@ -510,14 +589,24 @@
             pod=pod,
             pod_manager=self,
             container_name=container_name,
             post_termination_timeout=post_termination_timeout,
         )
 
     @tenacity.retry(stop=tenacity.stop_after_attempt(3), wait=tenacity.wait_exponential(), reraise=True)
+    def get_container_names(self, pod: V1Pod) -> list[str]:
+        """Return container names from the POD except for the airflow-xcom-sidecar container."""
+        pod_info = self.read_pod(pod)
+        return [
+            container_spec.name
+            for container_spec in pod_info.spec.containers
+            if container_spec.name != PodDefaults.SIDECAR_CONTAINER_NAME
+        ]
+
+    @tenacity.retry(stop=tenacity.stop_after_attempt(3), wait=tenacity.wait_exponential(), reraise=True)
     def read_pod_events(self, pod: V1Pod) -> CoreV1EventList:
         """Reads events from the POD."""
         try:
             return self._client.list_namespaced_event(
                 namespace=pod.metadata.namespace, field_selector=f"involvedObject.name={pod.metadata.name}"
             )
         except BaseHTTPError as e:
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 7.2.0rc2
+Version: 7.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -66,28 +66,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.2.0rc2``
+Release: ``7.3.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -105,8 +105,8 @@
 ``asgiref``             ``>=3.5.2``
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=21.7.0,<24``
 ``kubernetes_asyncio``  ``>=18.20.1,<25``
 ======================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/pyproject.toml` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/setup.cfg` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -57,10 +57,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.cncf.kubernetes.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.cncf.kubernetes
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/setup.py` & `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-cncf-kubernetes package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "7.2.0"
+version = "7.3.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-cncf-kubernetes setup."""
     setup(
         version=version,
         extras_require={},
```


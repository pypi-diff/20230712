# Comparing `tmp/aws-embedded-metrics-3.1.0.tar.gz` & `tmp/aws-embedded-metrics-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aws-embedded-metrics-3.1.0.tar", last modified: Wed Jan 25 00:30:25 2023, max compression
+gzip compressed data, was "dist/aws-embedded-metrics-3.1.1.tar", last modified: Wed Jul 12 20:13:17 2023, max compression
```

## Comparing `aws-embedded-metrics-3.1.0.tar` & `aws-embedded-metrics-3.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/
--rw-rw-r--   0 root         (0) root         (0)    10142 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       72 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13470 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    12767 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/
--rw-rw-r--   0 root         (0) root         (0)      886 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/config/
--rw-rw-r--   0 root         (0) root         (0)      945 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1512 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/config/configuration.py
--rw-rw-r--   0 root         (0) root         (0)     2192 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/config/environment_configuration_provider.py
--rw-rw-r--   0 root         (0) root         (0)      900 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/environment/
--rw-rw-r--   0 root         (0) root         (0)     1613 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/environment/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1627 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/environment/default_environment.py
--rw-rw-r--   0 root         (0) root         (0)     4777 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/environment/ec2_environment.py
--rw-rw-r--   0 root         (0) root         (0)     3111 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/environment/environment_detector.py
--rw-rw-r--   0 root         (0) root         (0)     2025 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/environment/lambda_environment.py
--rw-rw-r--   0 root         (0) root         (0)     1580 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/environment/local_environment.py
--rw-rw-r--   0 root         (0) root         (0)     1370 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/logger/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/logger/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1046 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/logger/metric.py
--rw-rw-r--   0 root         (0) root         (0)     7024 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/logger/metrics_context.py
--rw-rw-r--   0 root         (0) root         (0)     4679 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/logger/metrics_logger.py
--rw-rw-r--   0 root         (0) root         (0)      985 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/logger/metrics_logger_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/metric_scope/
--rw-rw-r--   0 root         (0) root         (0)     1762 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/metric_scope/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/serializers/
--rw-rw-r--   0 root         (0) root         (0)      888 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/serializers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4599 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/serializers/log_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/sinks/
--rw-rw-r--   0 root         (0) root         (0)     1211 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/sinks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2905 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/sinks/agent_sink.py
--rw-rw-r--   0 root         (0) root         (0)     1246 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/sinks/stdout_sink.py
--rw-rw-r--   0 root         (0) root         (0)     3553 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/sinks/tcp_client.py
--rw-rw-r--   0 root         (0) root         (0)     1135 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/sinks/udp_client.py
--rw-rw-r--   0 root         (0) root         (0)      359 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/storage_resolution.py
--rw-rw-r--   0 root         (0) root         (0)     1169 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/unit.py
--rw-rw-r--   0 root         (0) root         (0)      667 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/utils.py
--rw-rw-r--   0 root         (0) root         (0)     5072 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13470 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1541 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/aws_embedded_metrics.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       79 2023-01-25 00:30:25.000000 aws-embedded-metrics-3.1.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      974 2023-01-24 22:22:26.000000 aws-embedded-metrics-3.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 20:13:17.000000 aws-embedded-metrics-3.1.1/
+-rw-rw-r--   0 root         (0) root         (0)    10142 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       72 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13611 2023-07-12 20:13:17.000000 aws-embedded-metrics-3.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    12908 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 20:13:17.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/
+-rw-rw-r--   0 root         (0) root         (0)      886 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 20:13:17.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/config/
+-rw-rw-r--   0 root         (0) root         (0)      945 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1512 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/config/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     2192 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/config/environment_configuration_provider.py
+-rw-rw-r--   0 root         (0) root         (0)      900 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 20:13:17.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/environment/
+-rw-rw-r--   0 root         (0) root         (0)     1613 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/environment/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1627 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/environment/default_environment.py
+-rw-rw-r--   0 root         (0) root         (0)     4777 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/environment/ec2_environment.py
+-rw-rw-r--   0 root         (0) root         (0)     3111 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/environment/environment_detector.py
+-rw-rw-r--   0 root         (0) root         (0)     2025 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/environment/lambda_environment.py
+-rw-rw-r--   0 root         (0) root         (0)     1580 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/environment/local_environment.py
+-rw-rw-r--   0 root         (0) root         (0)     1370 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 20:13:17.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/logger/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/logger/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1046 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/logger/metric.py
+-rw-rw-r--   0 root         (0) root         (0)     7024 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/logger/metrics_context.py
+-rw-rw-r--   0 root         (0) root         (0)     4679 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/logger/metrics_logger.py
+-rw-rw-r--   0 root         (0) root         (0)      985 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/logger/metrics_logger_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 20:13:17.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/metric_scope/
+-rw-rw-r--   0 root         (0) root         (0)     1762 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/metric_scope/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 20:13:17.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/serializers/
+-rw-rw-r--   0 root         (0) root         (0)      888 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/serializers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4931 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/serializers/log_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 20:13:17.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/sinks/
+-rw-rw-r--   0 root         (0) root         (0)     1211 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/sinks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2905 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/sinks/agent_sink.py
+-rw-rw-r--   0 root         (0) root         (0)     1246 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/sinks/stdout_sink.py
+-rw-rw-r--   0 root         (0) root         (0)     3553 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/sinks/tcp_client.py
+-rw-rw-r--   0 root         (0) root         (0)     1135 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/sinks/udp_client.py
+-rw-rw-r--   0 root         (0) root         (0)      359 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/storage_resolution.py
+-rw-rw-r--   0 root         (0) root         (0)     1169 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/unit.py
+-rw-rw-r--   0 root         (0) root         (0)      667 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     5072 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 20:13:17.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13611 2023-07-12 20:13:16.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-07-12 20:13:17.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 20:13:16.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 20:13:16.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-12 20:13:16.000000 aws-embedded-metrics-3.1.1/aws_embedded_metrics.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       79 2023-07-12 20:13:17.000000 aws-embedded-metrics-3.1.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      974 2023-07-11 20:06:26.000000 aws-embedded-metrics-3.1.1/setup.py
```

### Comparing `aws-embedded-metrics-3.1.0/LICENSE` & `aws-embedded-metrics-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/PKG-INFO` & `aws-embedded-metrics-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-embedded-metrics
-Version: 3.1.0
+Version: 3.1.1
 Summary: AWS Embedded Metrics Package
 Home-page: https://github.com/awslabs/aws-embedded-metrics-python
 Author: Amazon Web Services
 Author-email: jarnance@amazon.com
 License: UNKNOWN
 Keywords: aws logs metrics emf
 Platform: UNKNOWN
@@ -35,14 +35,15 @@
 
 ## Use Cases
 
 - **Generate custom metrics across compute environments**
 
   - Easily generate custom metrics from Lambda functions without requiring custom batching code, making blocking network requests or relying on 3rd party software.
   - Other compute environments (EC2, On-prem, ECS, EKS, and other container environments) are supported by installing the [CloudWatch Agent](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Embedded_Metric_Format_Generation_CloudWatch_Agent.html).
+  	- Examples can be found in [examples/README.md](examples/README.md)
 
 - **Linking metrics to high cardinality context**
 
   Using the Embedded Metric Format, you will be able to visualize and alarm on custom metrics, but also retain the original, detailed and high-cardinality context which is queryable using [CloudWatch Logs Insights](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/AnalyzingLogData.html). For example, the library automatically injects environment metadata such as Lambda Function version, EC2 instance and image ids into the structured log event data.
 
 ## Installation
 
@@ -52,14 +53,15 @@
 
 ## Usage
 
 To get a metric logger, you can decorate your function with a `metric_scope`:
 
 ```py
 from aws_embedded_metrics import metric_scope
+from aws_embedded_metrics.storage_resolution import StorageResolution
 
 @metric_scope
 def my_handler(metrics):
     metrics.put_dimensions({"Foo": "Bar"})
     metrics.put_metric("ProcessingLatency", 100, "Milliseconds", StorageResolution.STANDARD)
     metrics.put_metric("Memory.HeapUsed", 1600424.0, "Bytes", StorageResolution.HIGH)
     metrics.set_property("AccountId", "123456789012")
```

### Comparing `aws-embedded-metrics-3.1.0/README.md` & `aws-embedded-metrics-3.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 ## Use Cases
 
 - **Generate custom metrics across compute environments**
 
   - Easily generate custom metrics from Lambda functions without requiring custom batching code, making blocking network requests or relying on 3rd party software.
   - Other compute environments (EC2, On-prem, ECS, EKS, and other container environments) are supported by installing the [CloudWatch Agent](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Embedded_Metric_Format_Generation_CloudWatch_Agent.html).
+  	- Examples can be found in [examples/README.md](examples/README.md)
 
 - **Linking metrics to high cardinality context**
 
   Using the Embedded Metric Format, you will be able to visualize and alarm on custom metrics, but also retain the original, detailed and high-cardinality context which is queryable using [CloudWatch Logs Insights](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/AnalyzingLogData.html). For example, the library automatically injects environment metadata such as Lambda Function version, EC2 instance and image ids into the structured log event data.
 
 ## Installation
 
@@ -31,14 +32,15 @@
 
 ## Usage
 
 To get a metric logger, you can decorate your function with a `metric_scope`:
 
 ```py
 from aws_embedded_metrics import metric_scope
+from aws_embedded_metrics.storage_resolution import StorageResolution
 
 @metric_scope
 def my_handler(metrics):
     metrics.put_dimensions({"Foo": "Bar"})
     metrics.put_metric("ProcessingLatency", 100, "Milliseconds", StorageResolution.STANDARD)
     metrics.put_metric("Memory.HeapUsed", 1600424.0, "Bytes", StorageResolution.HIGH)
     metrics.set_property("AccountId", "123456789012")
```

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/__init__.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/config/__init__.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/config/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/config/configuration.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/config/configuration.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/config/environment_configuration_provider.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/config/environment_configuration_provider.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/constants.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/constants.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/environment/__init__.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/environment/default_environment.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/environment/default_environment.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/environment/ec2_environment.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/environment/ec2_environment.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/environment/environment_detector.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/environment/environment_detector.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/environment/lambda_environment.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/environment/lambda_environment.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/environment/local_environment.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/environment/local_environment.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/exceptions.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/logger/metric.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/logger/metric.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/logger/metrics_context.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/logger/metrics_context.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/logger/metrics_logger.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/logger/metrics_logger.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/logger/metrics_logger_factory.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/logger/metrics_logger_factory.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/metric_scope/__init__.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/metric_scope/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/serializers/__init__.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/serializers/log_serializer.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/serializers/log_serializer.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,34 +63,40 @@
         num_metrics_in_current_body = 0
 
         # Track if any given metric has data remaining to be serialized
         remaining_data = True
 
         # Track batch number to know where to slice metric data
         i = 0
-
+        complete_metrics = set()
         while remaining_data:
             remaining_data = False
             current_body = create_body()
 
             for metric_name, metric in context.metrics.items():
+                # ensure we don't add duplicates of metrics we already completed
+                if metric_name in complete_metrics:
+                    continue
 
                 if len(metric.values) == 1:
                     current_body[metric_name] = metric.values[0]
+                    complete_metrics.add(metric_name)
                 else:
                     # Slice metric data as each batch cannot contain more than
                     # MAX_DATAPOINTS_PER_METRIC entries for a given metric
                     start_index = i * MAX_DATAPOINTS_PER_METRIC
                     end_index = (i + 1) * MAX_DATAPOINTS_PER_METRIC
                     current_body[metric_name] = metric.values[start_index:end_index]
 
                     # Make sure to consume remaining values if we sliced before the end
                     # of the metric value list
                     if len(metric.values) > end_index:
                         remaining_data = True
+                    else:
+                        complete_metrics.add(metric_name)
 
                 metric_body = {"Name": metric_name, "Unit": metric.unit}
                 if metric.storage_resolution == StorageResolution.HIGH:
                     metric_body["StorageResolution"] = metric.storage_resolution.value  # type: ignore
                 if not config.disable_metric_extraction:
                     current_body["_aws"]["CloudWatchMetrics"][0]["Metrics"].append(metric_body)
                 num_metrics_in_current_body += 1
```

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/sinks/__init__.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/sinks/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/sinks/agent_sink.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/sinks/agent_sink.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/sinks/stdout_sink.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/sinks/stdout_sink.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/sinks/tcp_client.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/sinks/tcp_client.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/sinks/udp_client.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/sinks/udp_client.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/unit.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/unit.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/utils.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics/validator.py` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics/validator.py`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics.egg-info/PKG-INFO` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-embedded-metrics
-Version: 3.1.0
+Version: 3.1.1
 Summary: AWS Embedded Metrics Package
 Home-page: https://github.com/awslabs/aws-embedded-metrics-python
 Author: Amazon Web Services
 Author-email: jarnance@amazon.com
 License: UNKNOWN
 Keywords: aws logs metrics emf
 Platform: UNKNOWN
@@ -35,14 +35,15 @@
 
 ## Use Cases
 
 - **Generate custom metrics across compute environments**
 
   - Easily generate custom metrics from Lambda functions without requiring custom batching code, making blocking network requests or relying on 3rd party software.
   - Other compute environments (EC2, On-prem, ECS, EKS, and other container environments) are supported by installing the [CloudWatch Agent](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Embedded_Metric_Format_Generation_CloudWatch_Agent.html).
+  	- Examples can be found in [examples/README.md](examples/README.md)
 
 - **Linking metrics to high cardinality context**
 
   Using the Embedded Metric Format, you will be able to visualize and alarm on custom metrics, but also retain the original, detailed and high-cardinality context which is queryable using [CloudWatch Logs Insights](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/AnalyzingLogData.html). For example, the library automatically injects environment metadata such as Lambda Function version, EC2 instance and image ids into the structured log event data.
 
 ## Installation
 
@@ -52,14 +53,15 @@
 
 ## Usage
 
 To get a metric logger, you can decorate your function with a `metric_scope`:
 
 ```py
 from aws_embedded_metrics import metric_scope
+from aws_embedded_metrics.storage_resolution import StorageResolution
 
 @metric_scope
 def my_handler(metrics):
     metrics.put_dimensions({"Foo": "Bar"})
     metrics.put_metric("ProcessingLatency", 100, "Milliseconds", StorageResolution.STANDARD)
     metrics.put_metric("Memory.HeapUsed", 1600424.0, "Bytes", StorageResolution.HIGH)
     metrics.set_property("AccountId", "123456789012")
```

### Comparing `aws-embedded-metrics-3.1.0/aws_embedded_metrics.egg-info/SOURCES.txt` & `aws-embedded-metrics-3.1.1/aws_embedded_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-embedded-metrics-3.1.0/setup.py` & `aws-embedded-metrics-3.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="aws-embedded-metrics",
-    version="3.1.0",
+    version="3.1.1",
     author="Amazon Web Services",
     author_email="jarnance@amazon.com",
     description="AWS Embedded Metrics Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="aws logs metrics emf",
     url="https://github.com/awslabs/aws-embedded-metrics-python",
```


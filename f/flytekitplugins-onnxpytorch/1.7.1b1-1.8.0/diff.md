# Comparing `tmp/flytekitplugins-onnxpytorch-1.7.1b1.tar.gz` & `tmp/flytekitplugins-onnxpytorch-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-onnxpytorch-1.7.1b1.tar", last modified: Tue Jun 27 22:00:58 2023, max compression
+gzip compressed data, was "flytekitplugins-onnxpytorch-1.8.0.tar", last modified: Tue Jul 11 22:07:22 2023, max compression
```

## Comparing `flytekitplugins-onnxpytorch-1.7.1b1.tar` & `flytekitplugins-onnxpytorch-1.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:58.320716 flytekitplugins-onnxpytorch-1.7.1b1/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-27 22:00:58.320716 flytekitplugins-onnxpytorch-1.7.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-27 22:00:35.000000 flytekitplugins-onnxpytorch-1.7.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:58.320716 flytekitplugins-onnxpytorch-1.7.1b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:58.320716 flytekitplugins-onnxpytorch-1.7.1b1/flytekitplugins/onnxpytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-27 22:00:35.000000 flytekitplugins-onnxpytorch-1.7.1b1/flytekitplugins/onnxpytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-27 22:00:35.000000 flytekitplugins-onnxpytorch-1.7.1b1/flytekitplugins/onnxpytorch/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:58.320716 flytekitplugins-onnxpytorch-1.7.1b1/flytekitplugins_onnxpytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-27 22:00:58.000000 flytekitplugins-onnxpytorch-1.7.1b1/flytekitplugins_onnxpytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-27 22:00:58.000000 flytekitplugins-onnxpytorch-1.7.1b1/flytekitplugins_onnxpytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:00:58.000000 flytekitplugins-onnxpytorch-1.7.1b1/flytekitplugins_onnxpytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:58.000000 flytekitplugins-onnxpytorch-1.7.1b1/flytekitplugins_onnxpytorch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 22:00:58.000000 flytekitplugins-onnxpytorch-1.7.1b1/flytekitplugins_onnxpytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:58.000000 flytekitplugins-onnxpytorch-1.7.1b1/flytekitplugins_onnxpytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 22:00:58.320716 flytekitplugins-onnxpytorch-1.7.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-27 22:00:50.000000 flytekitplugins-onnxpytorch-1.7.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:22.415733 flytekitplugins-onnxpytorch-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-11 22:07:22.415733 flytekitplugins-onnxpytorch-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-11 22:06:52.000000 flytekitplugins-onnxpytorch-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:22.415733 flytekitplugins-onnxpytorch-1.8.0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:22.415733 flytekitplugins-onnxpytorch-1.8.0/flytekitplugins/onnxpytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-11 22:06:52.000000 flytekitplugins-onnxpytorch-1.8.0/flytekitplugins/onnxpytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-07-11 22:06:52.000000 flytekitplugins-onnxpytorch-1.8.0/flytekitplugins/onnxpytorch/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:22.415733 flytekitplugins-onnxpytorch-1.8.0/flytekitplugins_onnxpytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-11 22:07:22.000000 flytekitplugins-onnxpytorch-1.8.0/flytekitplugins_onnxpytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-11 22:07:22.000000 flytekitplugins-onnxpytorch-1.8.0/flytekitplugins_onnxpytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:07:22.000000 flytekitplugins-onnxpytorch-1.8.0/flytekitplugins_onnxpytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:22.000000 flytekitplugins-onnxpytorch-1.8.0/flytekitplugins_onnxpytorch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 22:07:22.000000 flytekitplugins-onnxpytorch-1.8.0/flytekitplugins_onnxpytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:22.000000 flytekitplugins-onnxpytorch-1.8.0/flytekitplugins_onnxpytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 22:07:22.415733 flytekitplugins-onnxpytorch-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-11 22:07:11.000000 flytekitplugins-onnxpytorch-1.8.0/setup.py
```

### Comparing `flytekitplugins-onnxpytorch-1.7.1b1/PKG-INFO` & `flytekitplugins-onnxpytorch-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxpytorch
-Version: 1.7.1b1
+Version: 1.8.0
 Summary: ONNX PyTorch Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxpytorch-1.7.1b1/flytekitplugins/onnxpytorch/schema.py` & `flytekitplugins-onnxpytorch-1.8.0/flytekitplugins/onnxpytorch/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-onnxpytorch-1.7.1b1/flytekitplugins_onnxpytorch.egg-info/PKG-INFO` & `flytekitplugins-onnxpytorch-1.8.0/flytekitplugins_onnxpytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxpytorch
-Version: 1.7.1b1
+Version: 1.8.0
 Summary: ONNX PyTorch Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxpytorch-1.7.1b1/setup.py` & `flytekitplugins-onnxpytorch-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "onnxpytorch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "torch>=1.11.0"]
 
-__version__ = "1.7.1b1"
+__version__ = "1.8.0"
 
 setup(
     name=f"flytekitplugins-{PLUGIN_NAME}",
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="ONNX PyTorch Plugin for Flytekit",
```


# Comparing `tmp/onnc-bench-4.2.0.tar.gz` & `tmp/onnc-bench-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onnc-bench-4.2.0.tar", last modified: Wed Jun  7 18:50:13 2023, max compression
+gzip compressed data, was "onnc-bench-4.3.0.tar", last modified: Wed Jul 12 05:14:26 2023, max compression
```

## Comparing `onnc-bench-4.2.0.tar` & `onnc-bench-4.3.0.tar`

### file list

```diff
@@ -1,80 +1,84 @@
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      991 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/PKG-INFO
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      725 2023-05-22 10:00:39.000000 onnc-bench-4.2.0/README.md
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/
--rwxrwxr-x   0 fuji      (1010) fuji      (1010)      863 2023-02-07 10:13:51.000000 onnc-bench-4.2.0/onnc/__init__.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/bench/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      794 2023-06-07 18:50:12.000000 onnc-bench-4.2.0/onnc/bench/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1213 2023-06-01 09:39:05.000000 onnc-bench-4.2.0/onnc/bench/config.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/bench/core/
--rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-05-19 06:51:56.000000 onnc-bench-4.2.0/onnc/bench/core/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)       92 2022-05-19 06:51:56.000000 onnc-bench-4.2.0/onnc/bench/core/benchmark.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      515 2022-07-05 06:10:59.000000 onnc-bench-4.2.0/onnc/bench/core/common.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/bench/core/compiler/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1811 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/compiler/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1838 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/compiler/builder.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     3886 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/compiler/nnuxe.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2129 2022-09-22 04:18:54.000000 onnc-bench-4.2.0/onnc/bench/core/compiler/nnuxe_docker.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)    11856 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/compiler/onnc_saas.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1009 2022-07-05 06:10:59.000000 onnc-bench-4.2.0/onnc/bench/core/compiler/saas_config.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      574 2022-07-12 05:47:39.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     3048 2022-10-27 02:52:35.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/dataset.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     7431 2023-05-17 08:52:59.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/identifier.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      661 2022-05-19 06:51:56.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/layout.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2220 2022-10-19 15:48:12.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/operation.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1456 2022-10-25 08:05:07.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/preprocessor.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     8188 2023-05-17 08:46:00.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/serializer.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2419 2022-05-19 06:51:56.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/transformer.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     4005 2023-05-22 10:27:59.000000 onnc-bench-4.2.0/onnc/bench/core/deployment.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/bench/core/evaluator/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      697 2022-05-19 06:51:56.000000 onnc-bench-4.2.0/onnc/bench/core/evaluator/__init__.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/bench/core/model/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1122 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/model/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     3759 2023-06-01 11:15:50.000000 onnc-bench-4.2.0/onnc/bench/core/model/dtype_map.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     9880 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/model/identifier.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)    15409 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/model/meta.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     4573 2023-05-17 08:09:57.000000 onnc-bench-4.2.0/onnc/bench/core/model/model.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     6772 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/model/serializer.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      577 2022-05-19 06:51:56.000000 onnc-bench-4.2.0/onnc/bench/core/model/transformer.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     7347 2023-05-17 08:56:50.000000 onnc-bench-4.2.0/onnc/bench/core/modelpackage.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     6253 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/project.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      279 2022-07-28 03:03:26.000000 onnc-bench-4.2.0/onnc/bench/utils.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      295 2022-07-28 03:03:26.000000 onnc-bench-4.2.0/onnc/forest/__init__.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/core/
--rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.2.0/onnc/forest/core/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      748 2022-09-21 03:34:59.000000 onnc-bench-4.2.0/onnc/forest/core/binding_helper.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1667 2022-09-19 02:11:04.000000 onnc-bench-4.2.0/onnc/forest/core/options.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     4244 2022-10-21 04:37:40.000000 onnc-bench-4.2.0/onnc/forest/core/runtime.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/proxies/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1754 2022-09-19 02:11:04.000000 onnc-bench-4.2.0/onnc/forest/proxies/__init__.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/proxies/zerorpc/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2022-09-19 02:11:04.000000 onnc-bench-4.2.0/onnc/forest/proxies/zerorpc/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2294 2022-09-19 02:11:04.000000 onnc-bench-4.2.0/onnc/forest/proxies/zerorpc/runtime.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2388 2022-09-19 02:11:04.000000 onnc-bench-4.2.0/onnc/forest/proxies/zerorpc/runtime_server.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      482 2022-09-19 02:11:04.000000 onnc-bench-4.2.0/onnc/forest/proxies/zerorpc/utils.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/runtimes/
--rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.2.0/onnc/forest/runtimes/__init__.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/runtimes/onnx/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-02-07 10:13:51.000000 onnc-bench-4.2.0/onnc/forest/runtimes/onnx/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2069 2022-10-25 08:05:07.000000 onnc-bench-4.2.0/onnc/forest/runtimes/onnx/runtime.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/runtimes/openvino/
--rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.2.0/onnc/forest/runtimes/openvino/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     4819 2023-05-19 03:28:04.000000 onnc-bench-4.2.0/onnc/forest/runtimes/openvino/runtime.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     6455 2022-07-05 06:10:59.000000 onnc-bench-4.2.0/onnc/forest/runtimes/openvino/utils.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/runtimes/tensorrt/
--rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.2.0/onnc/forest/runtimes/tensorrt/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     3623 2022-10-25 08:05:07.000000 onnc-bench-4.2.0/onnc/forest/runtimes/tensorrt/runtime.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2930 2022-07-26 09:00:19.000000 onnc-bench-4.2.0/onnc/forest/runtimes/tensorrt/utils.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/utils/
--rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.2.0/onnc/forest/utils/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      510 2022-07-05 06:10:59.000000 onnc-bench-4.2.0/onnc/forest/utils/load_img.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc_bench.egg-info/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      991 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc_bench.egg-info/PKG-INFO
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1985 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc_bench.egg-info/SOURCES.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        1 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc_bench.egg-info/dependency_links.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      291 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc_bench.egg-info/requires.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        5 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc_bench.egg-info/top_level.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)       38 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/setup.cfg
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1324 2023-06-07 18:50:12.000000 onnc-bench-4.2.0/setup.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.455508 onnc-bench-4.3.0/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1070 2023-07-12 05:14:26.455508 onnc-bench-4.3.0/PKG-INFO
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      784 2023-07-05 02:46:47.000000 onnc-bench-4.3.0/README.md
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.447508 onnc-bench-4.3.0/onnc/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)      863 2023-02-07 10:13:51.000000 onnc-bench-4.3.0/onnc/__init__.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/bench/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      794 2023-07-12 05:14:26.000000 onnc-bench-4.3.0/onnc/bench/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1213 2023-06-01 09:39:05.000000 onnc-bench-4.3.0/onnc/bench/config.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/bench/core/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-05-19 06:51:56.000000 onnc-bench-4.3.0/onnc/bench/core/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       92 2022-05-19 06:51:56.000000 onnc-bench-4.3.0/onnc/bench/core/benchmark.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      515 2022-07-05 06:10:59.000000 onnc-bench-4.3.0/onnc/bench/core/common.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/bench/core/compiler/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1811 2023-07-06 03:40:40.000000 onnc-bench-4.3.0/onnc/bench/core/compiler/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1843 2023-07-06 03:49:30.000000 onnc-bench-4.3.0/onnc/bench/core/compiler/builder.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4319 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/onnc/bench/core/compiler/nnuxe.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2129 2022-09-22 04:18:54.000000 onnc-bench-4.3.0/onnc/bench/core/compiler/nnuxe_docker.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)    11826 2023-06-20 04:57:49.000000 onnc-bench-4.3.0/onnc/bench/core/compiler/onnc_saas.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1009 2022-07-05 06:10:59.000000 onnc-bench-4.3.0/onnc/bench/core/compiler/saas_config.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/bench/core/dataset/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       51 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/onnc/bench/core/dataset/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3072 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/bench/core/dataset/dataset.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      661 2022-05-19 06:51:56.000000 onnc-bench-4.3.0/onnc/bench/core/dataset/layout.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2220 2022-10-19 15:48:12.000000 onnc-bench-4.3.0/onnc/bench/core/dataset/operation.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1508 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/bench/core/dataset/preprocessor.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     8208 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/bench/core/dataset/serializer.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2419 2022-05-19 06:51:56.000000 onnc-bench-4.3.0/onnc/bench/core/dataset/transformer.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4005 2023-05-22 10:27:59.000000 onnc-bench-4.3.0/onnc/bench/core/deployment.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/bench/core/evaluator/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      697 2022-05-19 06:51:56.000000 onnc-bench-4.3.0/onnc/bench/core/evaluator/__init__.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/bench/core/model/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/onnc/bench/core/model/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3912 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/bench/core/model/model.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     6987 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/bench/core/model/serializer.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      577 2022-05-19 06:51:56.000000 onnc-bench-4.3.0/onnc/bench/core/model/transformer.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     7409 2023-07-12 04:29:20.000000 onnc-bench-4.3.0/onnc/bench/core/modelpackage.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     6963 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/bench/project.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      279 2022-07-28 03:03:26.000000 onnc-bench-4.3.0/onnc/bench/utils.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/forest/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      295 2022-07-28 03:03:26.000000 onnc-bench-4.3.0/onnc/forest/__init__.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/forest/core/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.3.0/onnc/forest/core/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      748 2022-09-21 03:34:59.000000 onnc-bench-4.3.0/onnc/forest/core/binding_helper.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1618 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/forest/core/options.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4144 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/onnc/forest/core/runtime.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/forest/proxies/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1663 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/onnc/forest/proxies/__init__.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/forest/proxies/zerorpc/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2022-09-19 02:11:04.000000 onnc-bench-4.3.0/onnc/forest/proxies/zerorpc/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2066 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/onnc/forest/proxies/zerorpc/runtime.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2334 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/onnc/forest/proxies/zerorpc/runtime_server.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      482 2022-09-19 02:11:04.000000 onnc-bench-4.3.0/onnc/forest/proxies/zerorpc/utils.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/forest/runtimes/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.3.0/onnc/forest/runtimes/__init__.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/forest/runtimes/onnx/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-02-07 10:13:51.000000 onnc-bench-4.3.0/onnc/forest/runtimes/onnx/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2072 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/forest/runtimes/onnx/runtime.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/forest/runtimes/openvino/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.3.0/onnc/forest/runtimes/openvino/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4823 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/forest/runtimes/openvino/runtime.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     6455 2022-07-05 06:10:59.000000 onnc-bench-4.3.0/onnc/forest/runtimes/openvino/utils.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.455508 onnc-bench-4.3.0/onnc/forest/runtimes/tensorrt/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.3.0/onnc/forest/runtimes/tensorrt/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3627 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/forest/runtimes/tensorrt/runtime.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2930 2022-07-26 09:00:19.000000 onnc-bench-4.3.0/onnc/forest/runtimes/tensorrt/utils.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.455508 onnc-bench-4.3.0/onnc/forest/utils/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.3.0/onnc/forest/utils/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      510 2022-07-05 06:10:59.000000 onnc-bench-4.3.0/onnc/forest/utils/load_img.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.455508 onnc-bench-4.3.0/onnc_bench.egg-info/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1070 2023-07-12 05:14:26.000000 onnc-bench-4.3.0/onnc_bench.egg-info/PKG-INFO
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2052 2023-07-12 05:14:26.000000 onnc-bench-4.3.0/onnc_bench.egg-info/SOURCES.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        1 2023-07-12 05:14:26.000000 onnc-bench-4.3.0/onnc_bench.egg-info/dependency_links.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      211 2023-07-12 05:14:26.000000 onnc-bench-4.3.0/onnc_bench.egg-info/requires.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        5 2023-07-12 05:14:26.000000 onnc-bench-4.3.0/onnc_bench.egg-info/top_level.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       38 2023-07-12 05:14:26.455508 onnc-bench-4.3.0/setup.cfg
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1278 2023-07-12 05:14:26.000000 onnc-bench-4.3.0/setup.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.455508 onnc-bench-4.3.0/tests/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      721 2023-06-07 17:45:11.000000 onnc-bench-4.3.0/tests/test_core_compiler.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2207 2022-10-25 06:18:30.000000 onnc-bench-4.3.0/tests/test_core_dataset_operation.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4576 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/tests/test_core_model.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3379 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/tests/test_core_modelpackage.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3936 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/tests/test_onnc_saas_builder.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      398 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/tests/test_options_factory.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3389 2022-09-19 02:11:04.000000 onnc-bench-4.3.0/tests/test_runtime.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `onnc-bench-4.2.0/PKG-INFO` & `onnc-bench-4.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: onnc-bench
-Version: 4.2.0
+Version: 4.3.0
 Summary: ONNC-bench is a Python wrapper of ONNC
 Home-page: https://www.skymizer.com
 Author: The Skymizer Team
 Author-email: hello@skymizer.com
 License: Apache License 2.0
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # ONNC-bench
 
 ONNC-bench is a Python wrapper of ONNC
 
 ## Installation
 
+### Developer install
+```
+python3 -m pip install -e .
+```
+
 ### Using pip
 
 ```
 pip install onnc-bench
 ```
 
 ## Python API Example
@@ -42,7 +48,9 @@
 
 # Save the compiled model
 deployment = project.save('./output')
 
 ```
 
 Please Check https://docs-tinyonnc.skymizer.com/index.html for the full documents.
+
+
```

### Comparing `onnc-bench-4.2.0/README.md` & `onnc-bench-4.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # ONNC-bench
 
 ONNC-bench is a Python wrapper of ONNC
 
 ## Installation
 
+### Developer install
+```
+python3 -m pip install -e .
+```
+
 ### Using pip
 
 ```
 pip install onnc-bench
 ```
 
 ## Python API Example
```

### Comparing `onnc-bench-4.2.0/onnc/__init__.py` & `onnc-bench-4.3.0/onnc/__init__.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.2.0/onnc/bench/__init__.py` & `onnc-bench-4.3.0/onnc/bench/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,8 +24,8 @@
              level="INFO")
 
 sentry_sdk.init(
     "https://da9cdf5759874504940714a91657de21@o304393.ingest.sentry.io/5901378",
     traces_sample_rate=1.0)
 fpath = os.path.dirname(os.path.abspath(__file__))
 
-__version__= "4.2.0"
+__version__= "4.3.0"
```

### Comparing `onnc-bench-4.2.0/onnc/bench/config.py` & `onnc-bench-4.3.0/onnc/bench/config.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.2.0/onnc/bench/core/common.py` & `onnc-bench-4.3.0/onnc/bench/core/common.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.2.0/onnc/bench/core/compiler/__init__.py` & `onnc-bench-4.3.0/onnc/bench/core/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.2.0/onnc/bench/core/compiler/builder.py` & `onnc-bench-4.3.0/onnc/bench/core/compiler/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         pass
 
     @abstractmethod
     def save(self, output: Path) -> Union[Dict, Deployment]:
         pass
 
     @property
-    def supported_devices(self) -> Dict:
+    def supported_devices(self) -> List[str]:
         pass
 
     def get_device_id(self, target):
         if target in self.supported_devices:
             return target
         else:
             logger.error(f'`{target}` is not a supported device/format.')
```

### Comparing `onnc-bench-4.2.0/onnc/bench/core/compiler/nnuxe.py` & `onnc-bench-4.3.0/onnc/bench/core/compiler/nnuxe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,52 @@
 from pathlib import Path
 from typing import Dict, Union, List
+from typing_extensions import Literal
 from pathlib import Path
 import os
 import json
 import shutil
+import logging
 
 from loguru import logger
 from onnc.bench.core.deployment import Deployment
 from .builder import IBuilder
 from onnc.bench.core.common import get_tmp_path
 from . import Compilation
-from onnc.bench.core.model.model import Model
-from onnc.bench.core.dataset.dataset import Dataset
 
 
 def spinning_cursor():
     while True:
         for cursor in '|/-\\':
             yield cursor
 
 
 class NNUXEBuilder(IBuilder):
     BUILDER_NAME = "NNUXEBuilder"
 
     def __init__(self):
         self._compilations: Dict[int, Compilation] = {}
         self.output_path: str = ""
+        self._builder_log_level = 'DEBUG'
+
+    def set_builder_log_level(self, level: Literal['DEBUG', 'INFO', 'WARN',
+                                                   'ERROR', 'CRITICAL']):
+        if level not in ('DEBUG', 'INFO', 'WARN', 'ERROR', 'CRITICAL'):
+            return self._builder_log_level
+        self._builder_log_level = self._builder_log_level
+        if level == "DEBUG":
+            self._builder_log_level = logging.DEBUG
+        elif level == "INFO":
+            self._builder_log_level = logging.INFO
+        elif level == "WARN":
+            self._builder_log_level = logging.WARN
+        elif level == "ERROR":
+            self._builder_log_level = logging.ERROR
+        elif level == "CRITICAL":
+            self._builder_log_level = logging.CRITICAL
 
     def _compile(self,
                  model_name,
                  model_path: str,
                  sample_path: str,
                  params_path: str,
                  output_path: str,
@@ -39,39 +56,35 @@
         from nnuxe.core.report import CompileReport
         report = CompileReport()
         nnuxe_compile(model_path,
                       sample_path,
                       params_path,
                       os.path.join(output_path, model_name),
                       report,
-                      local_nnuxe=local_nnuxe)
+                      local_nnuxe=local_nnuxe,
+                      log_level=self._builder_log_level)
         return report
 
     def build(self, target: str, converter_params={}) -> Dict:
 
-        compilation_list = []
-
+        output_path = get_tmp_path()
+        os.makedirs(output_path, exist_ok=True)
 
         # Upload files and create compilation
-        for iternal_cid in self._compilations:
+        res = {}
+
+        for idx, iternal_cid in enumerate(self._compilations):
             params = {}
             compilation = self._compilations[iternal_cid]
             params["target"] = target
             params["model_meta"] = compilation.model_meta
             params["sample_meta"] = compilation.sample_meta
             params["converter_params"] = converter_params
-            compilation_list.append(
-                (compilation.model_path, compilation.sample_path, params))
-        output_path = get_tmp_path()
-        os.makedirs(output_path, exist_ok=True)
-        res = {}
-        for idx, compi in enumerate(compilation_list):
-            model_path = compi[0]
-            sample_path = compi[1]
-            params = compi[2]
+            model_path = compilation.model_path
+            sample_path = compilation.sample_path
             params_path = get_tmp_path()
             open(params_path, 'w').write(json.dumps(params))
             report = self._compile(f'model_{idx}', model_path, sample_path,
                                    params_path, output_path)
             res[f'model_{idx}'] = report
             report.dump_json(
                 os.path.join(output_path, f'model_{idx}', "report.json"))
@@ -86,29 +99,36 @@
 
     def save(self, output: Path) -> Deployment:
         shutil.rmtree(output, ignore_errors=True)
         shutil.copytree(self.output_path, output)
         return Deployment(output)
 
     @property
-    def supported_devices(self) -> Dict:
-        devices = {
-            'CMSIS-NN': 'CMSIS-NN',
-            'ANDES-LIBNN': 'ANDES-LIBNN',
-            'NVDLA-NV-SMALL': 'NVDLA-NV-SMALL',
-            'NVDLA-NV-LARGE': 'NVDLA-NV-LARGE',
-            'NVDLA-NV-FULL': 'NVDLA-NV-FULL',
-            'CMSIS-NN-DEFAULT': 'CMSIS-NN-DEFAULT',
-            'NVDLA-NV-SMALL-DEFAULT': 'NVDLA-NV-SMALL-DEFAULT',
-            'NVDLA-NV-LARGE-DEFAULT': 'NVDLA-NV-LARGE-DEFAULT',
-            'NVDLA-NV-FULL-DEFAULT': 'NVDLA-NV-FULL-DEFAULT',
-            'NVIDIA-TENSORRT-FP32': 'NVIDIA-TENSORRT-FP32',
-            'NVIDIA-TENSORRT-FP16': 'NVIDIA-TENSORRT-FP16',
-            'NVIDIA-TENSORRT-INT8': 'NVIDIA-TENSORRT-INT8',
-            'RELAYIR': 'RELAYIR',
-            "INTEL-OPENVINO-CPU-FP32": "INTEL-OPENVINO-CPU-FP32",
-            "FIXED_ONNX": "FIXED_ONNX",
-            "ONNX": "ONNX",
-            "ONNC-IN2O3": "ONNC-IN2O3",
-            "GenericONNC": "GenericONNC"
-        }
-        return devices
+    def supported_devices(self) -> List[str]:
+        return [
+            'CMSIS-NN',
+            'ANDES-LIBNN',
+            'NVDLA-NV-SMALL',
+            'NVDLA-NV-LARGE',
+            'NVDLA-NV-FULL',
+            'CMSIS-NN-DEFAULT',
+            'NVDLA-NV-SMALL-DEFAULT',
+            'NVDLA-NV-LARGE-DEFAULT',
+            'NVDLA-NV-FULL-DEFAULT',
+            'NVIDIA-TENSORRT-FP32',
+            'NVIDIA-TENSORRT-FP16',
+            'NVIDIA-TENSORRT-INT8',
+            'RELAYIR',
+            "INTEL-OPENVINO-CPU-FP32",
+            "ONNC-IN2O3",
+            "GenericONNC",
+            "PTH",
+            "TORCH_SCRIPT",
+            "SAVED_MODEL",
+            "ONNX",
+            "FIXED_ONNX",
+            "PB",
+            "TFLITE",
+            "H5",
+            "OPENVINO",
+            "CAFFE_DIR",
+        ]
```

### Comparing `onnc-bench-4.2.0/onnc/bench/core/compiler/nnuxe_docker.py` & `onnc-bench-4.3.0/onnc/bench/core/compiler/nnuxe_docker.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.2.0/onnc/bench/core/compiler/onnc_saas.py` & `onnc-bench-4.3.0/onnc/bench/core/compiler/onnc_saas.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,11 +343,10 @@
                 deployment = Deployment(None, {}, [])
 
                 return deployment
 
         return deployment
 
     @property
-    def supported_devices(self) -> Dict:
+    def supported_devices(self) -> List[str]:
         sr = self.saas_list_devices()
-        devices = {x['name']: x['id'] for x in sr.data}
-        return devices
+        return [x['name'] for x in sr.data]
```

### Comparing `onnc-bench-4.2.0/onnc/bench/core/compiler/saas_config.py` & `onnc-bench-4.3.0/onnc/bench/core/compiler/saas_config.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.2.0/onnc/bench/core/dataset/dataset.py` & `onnc-bench-4.3.0/onnc/bench/core/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from loguru import logger
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .layout import DataLayout
 
 from ..common import get_class_name
-from . import DatasetFormat
+from pydlmeta.identifier.types import DatasetFormat
 
 
 class Dataset:
 
     def __init__(self,
                  raw_dataset: Union[Iterable, Iterable[Path], object],
                  format: DatasetFormat = DatasetFormat.NON_SPECIFIED):
```

### Comparing `onnc-bench-4.2.0/onnc/bench/core/dataset/layout.py` & `onnc-bench-4.3.0/onnc/bench/core/dataset/layout.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.2.0/onnc/bench/core/dataset/operation.py` & `onnc-bench-4.3.0/onnc/bench/core/dataset/operation.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.2.0/onnc/bench/core/dataset/preprocessor.py` & `onnc-bench-4.3.0/onnc/bench/core/dataset/preprocessor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 from typing import Callable, Dict, List, Type
-import types
 
-from .identifier import identify, DatasetFormat
+from pydlmeta.identifier.dataset import identify, DatasetFormat
 from .transform import DatasetTransformer
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .dataset import Dataset
 
 
@@ -17,17 +16,18 @@
     @classmethod
     def is_me(cls, dataset: Dataset) -> bool:
         return identify(dataset) == cls.FORMAT
 
     def transform(self, dataset: Type[Dataset]):
         pass
 
-    def set_preprocessor(self, func: Callable, args: List = [],
+    def set_preprocessor(self,
+                         func: Callable,
+                         args: List = [],
                          kwargs: Dict = {}) -> None:
-
         """Set the transform func as given callback
 
         Args:
             func (Callable): preprocessor function, the output of the this
                              function has to be the preprocessed dataset.
             args (List): args for the preprocessor function, use `__DATASET__`
                          to indicate the dataset argument position
```

### Comparing `onnc-bench-4.2.0/onnc/bench/core/dataset/serializer.py` & `onnc-bench-4.3.0/onnc/bench/core/dataset/serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Union, List
 from abc import abstractmethod
 from pathlib import Path
 import shutil
 import numpy as np
 from loguru import logger
 
-from .identifier import DatasetFormat, identify
+from pydlmeta.identifier.dataset import DatasetFormat, identify
 from ..common import get_tmp_path
 from .transformer import DatasetTransformer
 from .dataset import Dataset
 
 
 class SerializerRegistry(type):
 
@@ -25,15 +25,15 @@
 
 class Serializer(DatasetTransformer, metaclass=SerializerRegistry):
 
     FORMAT: Union[None, DatasetFormat] = None
 
     @classmethod
     def is_me(cls, dataset: Dataset) -> bool:
-        return identify(dataset) == cls.FORMAT
+        return identify(dataset.src) == cls.FORMAT
 
     @abstractmethod
     def transform(self, dataset: Dataset) -> Dataset:
         pass
 
     def serialize(self, dataset: Dataset, dest: Path) -> Dataset:
         self.add_param('dest', dest)  # type: ignore[attr-defined]
```

### Comparing `onnc-bench-4.2.0/onnc/bench/core/dataset/transformer.py` & `onnc-bench-4.3.0/onnc/bench/core/dataset/transformer.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.2.0/onnc/bench/core/deployment.py` & `onnc-bench-4.3.0/onnc/bench/core/deployment.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.2.0/onnc/bench/core/evaluator/__init__.py` & `onnc-bench-4.3.0/onnc/bench/core/evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.2.0/onnc/bench/core/model/model.py` & `onnc-bench-4.3.0/onnc/bench/core/model/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,53 @@
 from typing import Union, Tuple, Any, List, Type, Dict, Optional
 from dataclasses import dataclass
 from pathlib import Path
 from collections import OrderedDict
 from loguru import logger
 from enum import Enum, auto
 
-from . import ModelFormat, ModelDataType
+from pydlmeta.identifier.types import ModelFormat, ModelDataType
 from ..common import get_class_name
 
 
 @dataclass
 class Tensor:
     name: str
     shape: Union[None, Tuple[int, ...]] = None
-    dtype: Union[None, ModelDataType] = None
+    dtype: ModelDataType = ModelDataType.NON_SPECIFIED
 
     def dump(self) -> Dict:
-        return {
-            "name":
-                self.name,
-            "shape":
-                self.shape,
-            "type":
-                self.dtype.name
-                if isinstance(self.dtype, ModelDataType) else None
-        }
-
-
-class SrcType(Enum):
-    OBJ = auto()
-    FILE = auto()
-    DIR = auto()
+        _dtype =  ModelDataType.NON_SPECIFIED
+        if self.dtype:
+            _dtype = self.dtype
+        return {"name": self.name, "shape": self.shape, "type": _dtype.name}
 
 
 class Model():
 
     def __init__(self,
                  src: Union[str, Path, object],
                  format=ModelFormat.NON_SPECIFIED,
-                 inputs: List[Union[List, Tuple, Tensor]] = None,
-                 outputs: List[Union[List, Tuple, Tensor]] = None,
+                 inputs: List[Tensor] = None,
+                 outputs: List[Tensor] = None,
                  batch_dim=0):
         """
         Do not put identify_format in Model. Make sure
         (MVC) control and model are separated.
         """
         if not inputs:
             inputs = []
         if not outputs:
             outputs = []
         if isinstance(src, str):
             self.src = Path(src)
         else:
             self.src = src
-        self.inputs: List[Tensor] = inputs
-        self.outputs: List = outputs
+        self.inputs = inputs
+        self.outputs = outputs
         self.format = format
         self.batch_dim: int = batch_dim
 
         self._name: str
         if isinstance(src, str):
             self._name = Path(src).stem
         elif isinstance(src, Path):
@@ -66,34 +55,14 @@
         else:
             self._name = str(type(object))
 
     @property
     def name(self) -> str:
         return self._name
 
-    def get_src_type(self) -> SrcType:
-        """
-          Return type of self.src
-          Return None if self.src is not a valid path
-        """
-
-        if isinstance(self.src, str):
-            path = Path(self.src)
-        elif isinstance(self.src, Path):
-            path = self.src
-        else:
-            return SrcType.OBJ
-
-        if path.is_dir():
-            return SrcType.DIR
-        elif path.is_file():
-            return SrcType.FILE
-        else:
-            return None
-
     def set_name(self, _name: str):
         self._name = _name
 
     def set_batch_dim(self, _batch_dim: Optional[int]):
         if _batch_dim is not None:
             assert _batch_dim >= 0
         self.batch_dim = _batch_dim
```

### Comparing `onnc-bench-4.2.0/onnc/bench/core/model/serializer.py` & `onnc-bench-4.3.0/onnc/bench/core/model/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from pathlib import Path
 from abc import abstractmethod
 import shutil
 from loguru import logger
 
 from .transformer import ModelTransformer
 from .model import Model
-from . import ModelFormat
-from .identifier import identify
+from pydlmeta.identifier.types import ModelFormat
+from pydlmeta.identifier.model  import identify
 from ..common import get_tmp_path
 
 
 class SerializerRegistry(type):
 
     REGISTRY: List = []
 
@@ -24,15 +24,15 @@
 
 class Serializer(ModelTransformer, metaclass=SerializerRegistry):
 
     FORMAT = None
 
     @classmethod
     def is_me(cls, model: Model) -> bool:
-        return identify(model) == cls.FORMAT
+        return identify(model.src) == cls.FORMAT
 
     @abstractmethod
     def transform(self, model: Model) -> Model:
         raise NotImplementedError("`transform` has to be implemented")
 
     def serialize(self, model: Model, dest: Path) -> Model:
         self.add_param('dest', dest)  # type: ignore[attr-defined]
@@ -140,14 +140,24 @@
 
 
 class TFLITE(FileSerializer):
 
     FORMAT = ModelFormat.TFLITE
 
 
+class OpenvinoIRDir(DirSerializer):
+
+    FORMAT = ModelFormat.OPENVINO_IRDIR
+
+
+class ZippedOpenvinoIRDir(FileSerializer):
+
+    FORMAT = ModelFormat.ZIPPED_OPENVINO_IRDIR
+
+
 class SavedModel(DirSerializer):
 
     FORMAT = ModelFormat.SAVED_MODEL
 
 
 class ZippedSavedModel(FileSerializer):
```

### Comparing `onnc-bench-4.2.0/onnc/bench/core/model/transformer.py` & `onnc-bench-4.3.0/onnc/bench/core/model/transformer.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.2.0/onnc/bench/core/modelpackage.py` & `onnc-bench-4.3.0/onnc/bench/core/modelpackage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from typing import Dict, List, Union, Type, Iterable, Any, Tuple, Optional
 from pathlib import Path
 
 from loguru import logger
 
-from .dataset.dataset import Dataset
-from .dataset.transformer import DatasetTransformer
+from .common import get_tmp_path
+
 from .evaluator import Evaluator
 from .evaluator import Metric
 
-from .dataset import serializer as dataset_serializer
-from .dataset import DatasetFormat
-from .dataset import identifier as dataset_identifier
 from .dataset.dataset import Dataset
+from .dataset.transformer import DatasetTransformer
+from .dataset import serializer as dataset_serializer
 
 from .model import serializer as model_serializer
-from .model import ModelFormat, ModelDataType
-from .model import PYTORCH_MODEL_FORMATS
-from .model import identifier as model_identifier
+
 from .model.model import Model, Tensor
 from .model.transformer import ModelTransformer
 
-from .common import get_tmp_path
+from pydlmeta.identifier.dataset import identify as identify_dataset
+from pydlmeta.identifier.model import identify as identify_model
+from pydlmeta.identifier.types import ModelFormat, DatasetFormat, ModelDataType, PYTORCH_MODEL_FORMATS
 
 
 class ModelPackage:
     """Contain all data and controllers
 
     Data include: model and dataset
     Controllers include: evaluators, model_transformer and dataset_transformer
@@ -59,37 +58,39 @@
     def __encapsulate_model(self, model: Union[str, Path], model_format,
                             model_inputs, model_outputs, batch_dim) -> Model:
         """
         Do not put these code in Model.__init__(). Make sure
         (MVC) control and model are separated.
         """
 
-        from .model.meta import retrieve_model_metadata
+        from pydlmeta.meta import retrieve_model_metadata
 
         def inputs_outputs_to_tensors(data: List[Union[List, Tuple, Tensor]]):
             res = []
             for i in data:
                 if isinstance(i, list) or isinstance(i, tuple):
                     assert len(i) > 0
                     name = i[0]
                     shape = i[1] if len(i) >= 2 else tuple()
                     dtype = i[2] if len(i) >= 3 else ModelDataType.NON_SPECIFIED
+                    if not dtype:
+                        dtype = ModelDataType.NON_SPECIFIED
                     tensor = Tensor(name, shape, dtype)
                 elif isinstance(i, Tensor):
                     tensor = i
                 res.append(tensor)
             return res
 
         res_model = Model(model, batch_dim=batch_dim)
         if model_format == ModelFormat.NON_SPECIFIED:
-            res_model.format = model_identifier.identify(res_model)
+            res_model.format = identify_model(res_model.src)
         else:
             res_model.format = model_format
 
-        meta = retrieve_model_metadata(res_model)
+        meta = retrieve_model_metadata(res_model.src)
         meta_input_names = set([x.name for x in meta.inputs])
         meta_output_names = set([x.name for x in meta.outputs])
         if len(model_inputs) == 0:
             if res_model.format in PYTORCH_MODEL_FORMATS:
                 logger.error("Please specify model_inputs in "
                              "Project.add(model, model_inputs="
                              "[[input_name, shape, type]])."
@@ -120,15 +121,15 @@
             res_model.reset_outputs(tensors)
         return res_model
 
     def __encapsulate_dataset(self, dataset: Union[str, Path],
                               format: DatasetFormat) -> Dataset:
         dataset = Dataset(dataset, format)
         if format == DatasetFormat.NON_SPECIFIED:
-            dataset.format = dataset_identifier.identify(dataset)
+            dataset.format = identify_dataset(dataset.src)
         return dataset
 
     def serialize(
             self,
             model_path: Union[str, Path, None] = None,
             dataset_path: Union[str, Path,
                                 None] = None) -> Tuple[Model, Dataset]:
```

### Comparing `onnc-bench-4.2.0/onnc/bench/project.py` & `onnc-bench-4.3.0/onnc/bench/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from pathlib import Path
 from typing import Dict, Union, List, Tuple, Optional
+from typing_extensions import Literal
 import os
 import json
 import shutil
 
 from loguru import logger
 
 from .core.modelpackage import ModelPackage
 from .core.dataset.dataset import Dataset
 
-from .core.model import ModelFormat, TF_MODEL_FORMATS, ModelDataType
+from pydlmeta.identifier.types import ModelFormat, DatasetFormat
 from .core.model.model import Tensor
 
-from .core.dataset import DatasetFormat
-
 from .core.compiler.onnc_saas import ONNCSaaSBuilder
 # from .core.compiler.nnuxe import NNUXEBuilder
 # from .config import api_protocol, api_url, api_port
 from .core.common import get_tmp_path, get_temp_base
 
 from .config import default_builder, default_builder_params
-from onnc.bench.core.model.model import Model
 
 
 def login(api_key: str, password: str = ""):
     os.environ['ONNC_API_USER'] = api_key
     os.environ['ONNC_API_PASSWD'] = password
 
 
@@ -44,14 +42,18 @@
             self.builder.saas_login(*get_api_key())
             proj_info_sr = self.builder.saas_get_project_id_by_name(name)
             if len(proj_info_sr.data) == 0:
                 self.builder.saas_create_project(name)
 
             logger.info(f"ProjectID: {self.builder._project_id}")
 
+    def set_builder_log_level(self, level: Literal['DEBUG', 'INFO', 'WARN',
+                                                   'ERROR', 'CRITICAL']):
+        pass
+
     def add_model(
             self,
             model: Union[object, str, Path],
             samples: Union[object, str, Path, Dataset, None] = None,
             model_format: ModelFormat = ModelFormat.NON_SPECIFIED,
             sample_format: DatasetFormat = DatasetFormat.NON_SPECIFIED,
             # [name: str, shape:Tuple, dtype:ModelDataType]
@@ -98,14 +100,29 @@
             A list of input tensor(s), which include(s) 3 fields:
                 1. name: str
                 2. shape(optional): Union[List, Tuple]
                 3. dtype(optional): onnc.bench.core.model.ModelDataType
 
 
         """
+
+        def _check_io_type(x):
+            if not isinstance(x, (list, tuple)):
+                raise TypeError(
+                    f"model_inputs and model_outputs should be a list or tuple, got {type(x)}"
+                )
+            if len(x) == 0:
+                return
+            if not isinstance(x[0], (list, tuple, Tensor)):
+                raise TypeError(
+                    f"model_inputs and model_outputs should be a list "
+                    f"or tuple of list or tuple or a Tensor, got {type(x[0])}")
+
+        _check_io_type(model_inputs)
+        _check_io_type(model_outputs)
         model_package = ModelPackage(model, samples, model_format,
                                      sample_format, model_inputs, model_outputs,
                                      batch_dim)
         serialized_model, serialized_dataset = model_package.serialize()
 
         model_id = self.builder.prepare_model(serialized_model,
                                               serialized_dataset,
```

### Comparing `onnc-bench-4.2.0/onnc/forest/core/binding_helper.py` & `onnc-bench-4.3.0/onnc/forest/core/binding_helper.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.2.0/onnc/forest/core/options.py` & `onnc-bench-4.3.0/onnc/forest/core/options.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from dataclasses import dataclass, field
 import abc, typing
 from typing import List, Union
 from pathlib import Path
 
-from onnc.bench.core.model.identifier import identify
-from onnc.bench.core.model import ModelFormat
+from pydlmeta.identifier.model import identify
 from onnc.bench.core.model.model import Model
 
 
 @dataclass
 class RuntimeSettings:
     pass
 
@@ -35,15 +34,15 @@
         self.loadable = loadable
         self.__change_cls(loadable)
 
     def encapsulate(self, options):
         self._encapsulation.append(options)
 
     def __change_cls(self, loadable):
-        format_ = identify(loadable)
+        format_ = identify(loadable.src)
 
         for opt_cls in OptionsRegistry.REGISTRY:
             if opt_cls.is_me(format_):
                 """
                  The entire Options class is substituded by the derived class
                  after calling self.__class__ = opt_cls. Thus, the followeing
                  self.__init__ will call derived class's init
```

### Comparing `onnc-bench-4.2.0/onnc/forest/core/runtime.py` & `onnc-bench-4.3.0/onnc/forest/core/runtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from abc import ABC, abstractmethod
-from onnc.bench.core.model.identifier import identify
-from onnc.bench.core.model.model import Model
 from onnc.forest.core.options import Options
 
 from typing import Union, List
 
 
 class Runtime:
     """
```

### Comparing `onnc-bench-4.2.0/onnc/forest/proxies/__init__.py` & `onnc-bench-4.3.0/onnc/forest/proxies/zerorpc/runtime.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,63 @@
 from typing import List
-from importlib import import_module
 from dataclasses import dataclass
-from onnc.forest.core.runtime import AbstractRuntimeImplementation
+
+import zerorpc
+import pickle
+
 from onnc.forest.core.options import Options, RuntimeSettings
-from onnc.forest.core.runtime import make_runtime
 
 from onnc.bench.core.model.model import Model
-from onnc.bench.core.model import ModelFormat
-import time
+from onnc.forest.proxies import RuntimeProxy
+from onnc.forest.proxies.zerorpc.utils import np_to_bytes, np_from_bytes
+
 
 @dataclass
-class ProxySettings(RuntimeSettings):
-    pass
+class ZeroRPCSettings(RuntimeSettings):
+    protocol = 'tcp'
+    host = '127.0.0.1'
+    port = 20000
 
 
-class ProxyOptions(Options):
+class ZeroRPCOptions(Options):
 
     def __init__(self, loadable):
-        self.settings: ProxySettings = ProxySettings()
+        self.settings: ZeroRPCSettings = ZeroRPCSettings()
         self.devices: List = []
         self.loadable: Model = loadable
         self._encapsulation: List = []
 
     @staticmethod
     def is_me(format) -> bool:
-        return False # This runtime should be used manually
+        return False  # This runtime should be used manually
 
 
-class RuntimeProxy(AbstractRuntimeImplementation):
+class ZeroRPCProxy(RuntimeProxy):
 
-    def __init__(self, options):
-        self.options = options
-        self._options_ = self.options._encapsulation[0]        
-        self._runtime_ = make_runtime(self._options_)
+    @staticmethod
+    def is_me(options: Options) -> bool:
+        return isinstance(options, ZeroRPCOptions)
+
+    def __init__(self):
+        pass
 
     def launch(self, options: Options):
-        self._runtime_.launch(self._options_)
+        self._runtime_ = zerorpc.Client()
+        self._runtime_.connect(
+            f"{options.settings.protocol}://{options.settings.host}:{options.settings.port}"
+        )
+        self.options = options
+        self._runtime_.init(pickle.dumps(options))
+
+        options = pickle.dumps(options)
+        self._runtime_.launch(options)
 
     def load(self, options: Options):
-        self._runtime_.load(self._options_)
+        options = pickle.dumps(options)
+        self._runtime_.load(options)
 
     def bind_input(self, *args, **kwargs):
         self._runtime_.bind_input(*args, **kwargs)
 
     def bind_output(self, *args, **kwargs):
         self._runtime_.bind_output(*args, **kwargs)
 
@@ -52,15 +67,14 @@
     def bind_all_outputs(self):
         self._runtime_.bind_all_outputs()
 
     def materialize(self):
         self._runtime_.materialize()
 
     def write(self, data):
-        self._runtime_.write(data)
+        self._runtime_.write(np_to_bytes(data))
 
     def run(self):
-        self._runtime_.run()
+        self._runtime_.rpcrun()
 
     def read(self):
-        self._runtime_.read()
-
+        return np_from_bytes(self._runtime_.read())
```

### Comparing `onnc-bench-4.2.0/onnc/forest/proxies/zerorpc/runtime.py` & `onnc-bench-4.3.0/onnc/forest/proxies/zerorpc/runtime_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,58 @@
+import time
 from typing import List
 from importlib import import_module
 from dataclasses import dataclass
-from onnc.forest.core.runtime import AbstractRuntimeImplementation
+import pickle
 
 import zerorpc
-import numpy as np
-import time
-import pickle
 
 from onnc.forest.core.options import Options, RuntimeSettings
 from onnc.forest.core.runtime import make_runtime
 
 from onnc.bench.core.model.model import Model
-from onnc.bench.core.model import ModelFormat
+from onnc.forest.core.runtime import make_runtime
 from onnc.forest.proxies import RuntimeProxy
 from onnc.forest.proxies.zerorpc.utils import np_to_bytes, np_from_bytes
 
 
 @dataclass
-class ZeroRPCSettings(RuntimeSettings):
+class ZeroRPCServerSettings(RuntimeSettings):
     protocol = 'tcp'
-    host = '127.0.0.1'
+    host = '0.0.0.0'
     port = 20000
 
 
-class ZeroRPCOptions(Options):
-
+class ZeroRPCServerOptions(Options):
     def __init__(self, loadable):
-        self.settings: ZeroRPCSettings = ZeroRPCSettings()
+        self.settings: ZeroRPCServerSettings = ZeroRPCServerSettings()
         self.devices: List = []
         self.loadable: Model = loadable
         self._encapsulation: List = []
 
     @staticmethod
     def is_me(format) -> bool:
         return False # This runtime should be used manually
 
 
-class ZeroRPCProxy(RuntimeProxy):
-    @staticmethod
-    def is_me(options: Options) -> bool:
-        return isinstance(options, ZeroRPCOptions)
-
-    def __init__(self):
+class ZeroRPCServerProxy(RuntimeProxy):
+    def __init__(self, options):
         pass
 
-    def launch(self, options: Options):
-        self._runtime_ = zerorpc.Client()
-        self._runtime_.connect(f"{options.settings.protocol}://{options.settings.host}:{options.settings.port}")     
+    def init(self, options):
+        options = pickle.loads(options)
         self.options = options
-        self._runtime_.init(pickle.dumps(options))
-                
-        options = pickle.dumps(options)
-        self._runtime_.launch(options)
+        self._options_ = self.options._encapsulation[0]
+        self._runtime_ = make_runtime(self._options_)
+
+    def launch(self, options: Options):
+        self._runtime_.launch(self._options_)
 
     def load(self, options: Options):
-        options = pickle.dumps(options)
-        self._runtime_.load(options)
+        self._runtime_.load(self._options_)
 
     def bind_input(self, *args, **kwargs):
         self._runtime_.bind_input(*args, **kwargs)
 
     def bind_output(self, *args, **kwargs):
         self._runtime_.bind_output(*args, **kwargs)
 
@@ -70,15 +62,24 @@
     def bind_all_outputs(self):
         self._runtime_.bind_all_outputs()
 
     def materialize(self):
         self._runtime_.materialize()
 
     def write(self, data):
-        self._runtime_.write(np_to_bytes(data))
+        data = np_from_bytes(data)
+        self._runtime_.write(data)
+
+    def rpcrun(self):
+        self._runtime_.run()
 
     def run(self):
-        self._runtime_.rpcrun()
+        raise Exception('ZeroRPC cannot use `run` as method name')
 
     def read(self):
-        return np_from_bytes(self._runtime_.read())
+        return np_to_bytes(self._runtime_.read())
 
+if __name__ == "__main__":
+    opt = ZeroRPCServerOptions(None)
+    s = zerorpc.Server(ZeroRPCServerProxy(opt))
+    s.bind(f"{opt.settings.protocol}://{opt.settings.host}:{opt.settings.port}")
+    s.run()
```

### Comparing `onnc-bench-4.2.0/onnc/forest/runtimes/onnx/runtime.py` & `onnc-bench-4.3.0/onnc/forest/runtimes/onnx/runtime.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import List
 from importlib import import_module
 from dataclasses import dataclass
 from onnc.forest.core.runtime import AbstractRuntimeImplementation
 
 from onnc.forest.core.options import Options, RuntimeSettings
 from onnc.bench.core.model.model import Model
-from onnc.bench.core.model import ModelFormat
-
+from pydlmeta.identifier.types import ModelFormat
 
 @dataclass
 class ONNXSettings(RuntimeSettings):
     ep_list = ['CPUExecutionProvider']
     intra_op_num_threads = 0
```

### Comparing `onnc-bench-4.2.0/onnc/forest/runtimes/openvino/runtime.py` & `onnc-bench-4.3.0/onnc/forest/runtimes/openvino/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 import copy
 from importlib import import_module
 from onnc.forest.core.runtime import AbstractRuntimeImplementation
 
 from onnc.forest.core.options import Options, RuntimeSettings
-from onnc.bench.core.model import ModelFormat
+from pydlmeta.identifier.types import ModelFormat
 
 
 @dataclass
 class OpenvinoSettings(RuntimeSettings):
     pass
```

### Comparing `onnc-bench-4.2.0/onnc/forest/runtimes/openvino/utils.py` & `onnc-bench-4.3.0/onnc/forest/runtimes/openvino/utils.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.2.0/onnc/forest/runtimes/tensorrt/runtime.py` & `onnc-bench-4.3.0/onnc/forest/runtimes/tensorrt/runtime.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass, field
 from typing import List
 import numpy as np
 from importlib import import_module
 
 from onnc.forest.core.runtime import AbstractRuntimeImplementation
 from onnc.forest.core.options import Options, RuntimeSettings
-from onnc.bench.core.model import ModelFormat
+from pydlmeta.identifier.types import ModelFormat
 
 
 @dataclass
 class TensorRTSettings(RuntimeSettings):
     pass
```

### Comparing `onnc-bench-4.2.0/onnc/forest/runtimes/tensorrt/utils.py` & `onnc-bench-4.3.0/onnc/forest/runtimes/tensorrt/utils.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.2.0/onnc_bench.egg-info/PKG-INFO` & `onnc-bench-4.3.0/onnc_bench.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: onnc-bench
-Version: 4.2.0
+Version: 4.3.0
 Summary: ONNC-bench is a Python wrapper of ONNC
 Home-page: https://www.skymizer.com
 Author: The Skymizer Team
 Author-email: hello@skymizer.com
 License: Apache License 2.0
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # ONNC-bench
 
 ONNC-bench is a Python wrapper of ONNC
 
 ## Installation
 
+### Developer install
+```
+python3 -m pip install -e .
+```
+
 ### Using pip
 
 ```
 pip install onnc-bench
 ```
 
 ## Python API Example
@@ -42,7 +48,9 @@
 
 # Save the compiled model
 deployment = project.save('./output')
 
 ```
 
 Please Check https://docs-tinyonnc.skymizer.com/index.html for the full documents.
+
+
```

### Comparing `onnc-bench-4.2.0/onnc_bench.egg-info/SOURCES.txt` & `onnc-bench-4.3.0/onnc_bench.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -14,25 +14,21 @@
 onnc/bench/core/compiler/builder.py
 onnc/bench/core/compiler/nnuxe.py
 onnc/bench/core/compiler/nnuxe_docker.py
 onnc/bench/core/compiler/onnc_saas.py
 onnc/bench/core/compiler/saas_config.py
 onnc/bench/core/dataset/__init__.py
 onnc/bench/core/dataset/dataset.py
-onnc/bench/core/dataset/identifier.py
 onnc/bench/core/dataset/layout.py
 onnc/bench/core/dataset/operation.py
 onnc/bench/core/dataset/preprocessor.py
 onnc/bench/core/dataset/serializer.py
 onnc/bench/core/dataset/transformer.py
 onnc/bench/core/evaluator/__init__.py
 onnc/bench/core/model/__init__.py
-onnc/bench/core/model/dtype_map.py
-onnc/bench/core/model/identifier.py
-onnc/bench/core/model/meta.py
 onnc/bench/core/model/model.py
 onnc/bench/core/model/serializer.py
 onnc/bench/core/model/transformer.py
 onnc/forest/__init__.py
 onnc/forest/core/__init__.py
 onnc/forest/core/binding_helper.py
 onnc/forest/core/options.py
@@ -53,8 +49,15 @@
 onnc/forest/runtimes/tensorrt/utils.py
 onnc/forest/utils/__init__.py
 onnc/forest/utils/load_img.py
 onnc_bench.egg-info/PKG-INFO
 onnc_bench.egg-info/SOURCES.txt
 onnc_bench.egg-info/dependency_links.txt
 onnc_bench.egg-info/requires.txt
-onnc_bench.egg-info/top_level.txt
+onnc_bench.egg-info/top_level.txt
+tests/test_core_compiler.py
+tests/test_core_dataset_operation.py
+tests/test_core_model.py
+tests/test_core_modelpackage.py
+tests/test_onnc_saas_builder.py
+tests/test_options_factory.py
+tests/test_runtime.py
```

### Comparing `onnc-bench-4.2.0/setup.py` & `onnc-bench-4.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,23 +18,22 @@
         for i in range(len(requirements)):
             if "{CWD}" in requirements[i]:
                 requirements[i] = requirements[i].replace("{CWD}", os.getcwd())
     return [r for r in requirements if r and r[0] != '#']
 
 
 # This call to setup() does all the work
-setup(name="onnc-bench",
-      version="4.2.0",
-      description="ONNC-bench is a Python wrapper of ONNC",
-      long_description=README,
-      long_description_content_type="text/markdown",
-      url="https://www.skymizer.com",
-      author="The Skymizer Team",
-      author_email="hello@skymizer.com",
-      license="Apache License 2.0",
-      packages=find_packages(),
-      package_data={"onnc": ["*"]},
-      data_files=[],
-      install_requires=[
-          "requests", "numpy", "onnx", "loguru",
-          "sentry-sdk", "packaging"] + load_req("requirements.txt")
-)
+setup(
+    name="onnc-bench",
+    version="4.3.0",
+    description="ONNC-bench is a Python wrapper of ONNC",
+    long_description=README,
+    long_description_content_type="text/markdown",
+    url="https://www.skymizer.com",
+    author="The Skymizer Team",
+    author_email="hello@skymizer.com",
+    license="Apache License 2.0",
+    packages=find_packages(),
+    package_data={"onnc": ["*"]},
+    data_files=[],
+    install_requires=["requests", "onnx", "loguru", "sentry-sdk", "packaging"] +
+    load_req("requirements.txt"))
```


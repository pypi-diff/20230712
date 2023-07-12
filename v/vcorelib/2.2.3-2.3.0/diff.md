# Comparing `tmp/vcorelib-2.2.3.tar.gz` & `tmp/vcorelib-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcorelib-2.2.3.tar", last modified: Tue Jul 11 20:24:11 2023, max compression
+gzip compressed data, was "vcorelib-2.3.0.tar", last modified: Wed Jul 12 21:07:02 2023, max compression
```

## Comparing `vcorelib-2.2.3.tar` & `vcorelib-2.3.0.tar`

### file list

```diff
@@ -1,102 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.373852 vcorelib-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 20:22:37.000000 vcorelib-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-11 20:24:11.373852 vcorelib-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-11 20:22:37.000000 vcorelib-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-11 20:22:37.000000 vcorelib-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:24:11.373852 vcorelib-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-11 20:22:37.000000 vcorelib-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.357851 vcorelib-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-11 20:22:37.000000 vcorelib-2.2.3/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-11 20:22:37.000000 vcorelib-2.2.3/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-11 20:22:37.000000 vcorelib-2.2.3/tests/test_namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.361852 vcorelib-2.2.3/vcorelib/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.361852 vcorelib-2.2.3/vcorelib/args/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/args/newline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.361852 vcorelib-2.2.3/vcorelib/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/asyncio/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/asyncio/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.361852 vcorelib-2.2.3/vcorelib/dict/
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/dict/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/dict/codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/dict/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/dict/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.361852 vcorelib-2.2.3/vcorelib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/graph/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/graph/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.365851 vcorelib-2.2.3/vcorelib/io/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/io/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.365851 vcorelib-2.2.3/vcorelib/io/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/io/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/io/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/io/arbiter/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/io/arbiter/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.365851 vcorelib-2.2.3/vcorelib/io/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/io/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/io/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/io/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/io/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/io/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/io/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.365851 vcorelib-2.2.3/vcorelib/math/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.365851 vcorelib-2.2.3/vcorelib/math/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/math/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/math/analysis/average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/math/analysis/buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.369851 vcorelib-2.2.3/vcorelib/math/analysis/rate/
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/math/analysis/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/math/analysis/rate/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/math/analysis/weighted.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/math/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/math/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.369851 vcorelib-2.2.3/vcorelib/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/paths/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/paths/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/paths/info_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.369851 vcorelib-2.2.3/vcorelib/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.369851 vcorelib-2.2.3/vcorelib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/schemas/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/schemas/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.369851 vcorelib-2.2.3/vcorelib/script/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.369851 vcorelib-2.2.3/vcorelib/target/
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/target/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/target/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/target/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.369851 vcorelib-2.2.3/vcorelib/task/
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.369851 vcorelib-2.2.3/vcorelib/task/dict/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/task/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/task/dict/melder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/task/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.369851 vcorelib-2.2.3/vcorelib/task/subprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/task/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/task/subprocess/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.369851 vcorelib-2.2.3/vcorelib/task/time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/task/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-11 20:22:37.000000 vcorelib-2.2.3/vcorelib/task/time/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:11.361852 vcorelib-2.2.3/vcorelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-11 20:24:11.000000 vcorelib-2.2.3/vcorelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-11 20:24:11.000000 vcorelib-2.2.3/vcorelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:24:11.000000 vcorelib-2.2.3/vcorelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 20:24:11.000000 vcorelib-2.2.3/vcorelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 20:24:11.000000 vcorelib-2.2.3/vcorelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.163618 vcorelib-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-12 21:05:45.000000 vcorelib-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-12 21:07:02.163618 vcorelib-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-12 21:05:45.000000 vcorelib-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-12 21:05:45.000000 vcorelib-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 21:07:02.163618 vcorelib-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-12 21:05:45.000000 vcorelib-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.151618 vcorelib-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-12 21:05:45.000000 vcorelib-2.3.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-12 21:05:45.000000 vcorelib-2.3.0/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-12 21:05:45.000000 vcorelib-2.3.0/tests/test_namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.155618 vcorelib-2.3.0/vcorelib/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.155618 vcorelib-2.3.0/vcorelib/args/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/args/newline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.155618 vcorelib-2.3.0/vcorelib/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/asyncio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/asyncio/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.155618 vcorelib-2.3.0/vcorelib/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/dict/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/dict/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/dict/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/dict/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.155618 vcorelib-2.3.0/vcorelib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/graph/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/graph/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.155618 vcorelib-2.3.0/vcorelib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/io/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.159618 vcorelib-2.3.0/vcorelib/io/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/io/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/io/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/io/arbiter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/io/arbiter/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.159618 vcorelib-2.3.0/vcorelib/io/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/io/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/io/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/io/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/io/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/io/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/io/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.159618 vcorelib-2.3.0/vcorelib/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.159618 vcorelib-2.3.0/vcorelib/math/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/math/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/math/analysis/average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/math/analysis/buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.159618 vcorelib-2.3.0/vcorelib/math/analysis/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/math/analysis/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/math/analysis/rate/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/math/analysis/weighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/math/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/math/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.159618 vcorelib-2.3.0/vcorelib/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/paths/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/paths/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/paths/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/paths/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/paths/info_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.159618 vcorelib-2.3.0/vcorelib/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.159618 vcorelib-2.3.0/vcorelib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/schemas/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/schemas/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.159618 vcorelib-2.3.0/vcorelib/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.159618 vcorelib-2.3.0/vcorelib/target/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/target/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/target/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/target/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.159618 vcorelib-2.3.0/vcorelib/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.159618 vcorelib-2.3.0/vcorelib/task/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/task/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/task/dict/melder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/task/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.159618 vcorelib-2.3.0/vcorelib/task/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/task/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/task/subprocess/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.163618 vcorelib-2.3.0/vcorelib/task/time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/task/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-12 21:05:45.000000 vcorelib-2.3.0/vcorelib/task/time/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:07:02.155618 vcorelib-2.3.0/vcorelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-12 21:07:02.000000 vcorelib-2.3.0/vcorelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-12 21:07:02.000000 vcorelib-2.3.0/vcorelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:07:02.000000 vcorelib-2.3.0/vcorelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-12 21:07:02.000000 vcorelib-2.3.0/vcorelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 21:07:02.000000 vcorelib-2.3.0/vcorelib.egg-info/top_level.txt
```

### Comparing `vcorelib-2.2.3/LICENSE` & `vcorelib-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/PKG-INFO` & `vcorelib-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 2.2.3
+Version: 2.3.0
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=f6114ec2f47f68cb9c8196b8c0c35bf4
+    hash=08dfba51dc98120d47088a5ec810ec88
     =====================================
 -->
 
-# vcorelib ([2.2.3](https://pypi.org/project/vcorelib/))
+# vcorelib ([2.3.0](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-2.2.3/README.md` & `vcorelib-2.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=f6114ec2f47f68cb9c8196b8c0c35bf4
+    hash=08dfba51dc98120d47088a5ec810ec88
     =====================================
 -->
 
-# vcorelib ([2.2.3](https://pypi.org/project/vcorelib/))
+# vcorelib ([2.3.0](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-2.2.3/pyproject.toml` & `vcorelib-2.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vcorelib"
-version = "2.2.3"
+version = "2.3.0"
 description = "A collection of core Python utilities."
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `vcorelib-2.2.3/setup.py` & `vcorelib-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/tests/test_logging.py` & `vcorelib-2.3.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/tests/test_names.py` & `vcorelib-2.3.0/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/tests/test_namespace.py` & `vcorelib-2.3.0/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/args/__init__.py` & `vcorelib-2.3.0/vcorelib/args/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/args/newline.py` & `vcorelib-2.3.0/vcorelib/args/newline.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/asyncio/__init__.py` & `vcorelib-2.3.0/vcorelib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/asyncio/cli.py` & `vcorelib-2.3.0/vcorelib/asyncio/cli.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/asyncio/subprocess.py` & `vcorelib-2.3.0/vcorelib/asyncio/subprocess.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/dict/__init__.py` & `vcorelib-2.3.0/vcorelib/dict/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/dict/cache.py` & `vcorelib-2.3.0/vcorelib/dict/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/dict/codec.py` & `vcorelib-2.3.0/vcorelib/dict/codec.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/dict/config.py` & `vcorelib-2.3.0/vcorelib/dict/config.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/dict/env.py` & `vcorelib-2.3.0/vcorelib/dict/env.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/graph/__init__.py` & `vcorelib-2.3.0/vcorelib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/graph/abc.py` & `vcorelib-2.3.0/vcorelib/graph/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/graph/edge.py` & `vcorelib-2.3.0/vcorelib/graph/edge.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/graph/node.py` & `vcorelib-2.3.0/vcorelib/graph/node.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/graph/port.py` & `vcorelib-2.3.0/vcorelib/graph/port.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/io/__init__.py` & `vcorelib-2.3.0/vcorelib/io/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/io/abc.py` & `vcorelib-2.3.0/vcorelib/io/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/io/arbiter/base.py` & `vcorelib-2.3.0/vcorelib/io/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/io/arbiter/context.py` & `vcorelib-2.3.0/vcorelib/io/arbiter/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/io/arbiter/directory.py` & `vcorelib-2.3.0/vcorelib/io/arbiter/directory.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/io/archive/__init__.py` & `vcorelib-2.3.0/vcorelib/io/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/io/cache.py` & `vcorelib-2.3.0/vcorelib/io/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/io/decode.py` & `vcorelib-2.3.0/vcorelib/io/decode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/io/encode.py` & `vcorelib-2.3.0/vcorelib/io/encode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/io/mapping.py` & `vcorelib-2.3.0/vcorelib/io/mapping.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/io/types.py` & `vcorelib-2.3.0/vcorelib/io/types.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/logging.py` & `vcorelib-2.3.0/vcorelib/logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/math/__init__.py` & `vcorelib-2.3.0/vcorelib/math/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/math/analysis/__init__.py` & `vcorelib-2.3.0/vcorelib/math/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/math/analysis/average.py` & `vcorelib-2.3.0/vcorelib/math/analysis/average.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/math/analysis/buffer.py` & `vcorelib-2.3.0/vcorelib/math/analysis/buffer.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/math/analysis/rate/__init__.py` & `vcorelib-2.3.0/vcorelib/math/analysis/rate/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/math/analysis/rate/limiter.py` & `vcorelib-2.3.0/vcorelib/math/analysis/rate/limiter.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/math/analysis/weighted.py` & `vcorelib-2.3.0/vcorelib/math/analysis/weighted.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/math/time.py` & `vcorelib-2.3.0/vcorelib/math/time.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/math/unit.py` & `vcorelib-2.3.0/vcorelib/math/unit.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/names.py` & `vcorelib-2.3.0/vcorelib/names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/namespace.py` & `vcorelib-2.3.0/vcorelib/namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/paths/context.py` & `vcorelib-2.3.0/vcorelib/paths/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/paths/info.py` & `vcorelib-2.3.0/vcorelib/paths/info.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/paths/info_cache.py` & `vcorelib-2.3.0/vcorelib/paths/info_cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/platform/__init__.py` & `vcorelib-2.3.0/vcorelib/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/schemas/__init__.py` & `vcorelib-2.3.0/vcorelib/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/schemas/base.py` & `vcorelib-2.3.0/vcorelib/schemas/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/schemas/json.py` & `vcorelib-2.3.0/vcorelib/schemas/json.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/schemas/mixins.py` & `vcorelib-2.3.0/vcorelib/schemas/mixins.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/script/__init__.py` & `vcorelib-2.3.0/vcorelib/script/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/target/__init__.py` & `vcorelib-2.3.0/vcorelib/target/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/target/evaluation.py` & `vcorelib-2.3.0/vcorelib/target/evaluation.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/target/expression.py` & `vcorelib-2.3.0/vcorelib/target/expression.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/target/resolver.py` & `vcorelib-2.3.0/vcorelib/target/resolver.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/task/__init__.py` & `vcorelib-2.3.0/vcorelib/task/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/task/dict/melder.py` & `vcorelib-2.3.0/vcorelib/task/dict/melder.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/task/manager.py` & `vcorelib-2.3.0/vcorelib/task/manager.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib/task/subprocess/run.py` & `vcorelib-2.3.0/vcorelib/task/subprocess/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 A task definition for wrapping subprocess's 'run' method.
 """
 
 # built-in
 from asyncio.subprocess import PIPE as _PIPE
 from asyncio.subprocess import Process as _Process
+from pathlib import Path as _Path
 from sys import executable as _executable
+from typing import List as _List
 
 # internal
 from vcorelib.asyncio.cli import (
     create_subprocess_shell_log,
     handle_process_cancel,
 )
 from vcorelib.asyncio.subprocess import create_subprocess_exec_log
@@ -32,15 +34,15 @@
     """
     A class for creating asyncio subprocesses and logging what gets created.
     """
 
     async def subprocess_exec(
         self,
         program: str,
-        *caller_args,
+        *caller_args: str,
         args: str = "",
         separator: str = "::",
         stdout: int = None,
         stderr: int = None,
         **kwargs,
     ) -> _Process:
         """
@@ -55,42 +57,46 @@
             stderr=stderr,
             **kwargs,
         )
 
     async def exec(
         self,
         program: str,
-        *caller_args,
+        *caller_args: str,
         args: str = "",
         separator: str = "::",
         stdout: int = None,
         stderr: int = None,
         **kwargs,
     ) -> bool:
         """Execute a command and return whether or not it succeeded."""
 
-        proc, _, __ = await handle_process_cancel(
-            await self.subprocess_exec(
-                program,
-                *caller_args,
-                args=args,
-                separator=separator,
-                stdout=stdout,
-                stderr=stderr,
-                **kwargs,
-            ),
-            self.name,
-            self.log,
-        )
-        return proc.returncode == 0
+        try:
+            proc, _, __ = await handle_process_cancel(
+                await self.subprocess_exec(
+                    program,
+                    *caller_args,
+                    args=args,
+                    separator=separator,
+                    stdout=stdout,
+                    stderr=stderr,
+                    **kwargs,
+                ),
+                self.name,
+                self.log,
+            )
+            return proc.returncode == 0
+        except FileNotFoundError as exc:
+            self.log.exception("Couldn't run command:", exc_info=exc)
+            return False
 
     async def subprocess_shell(
         self,
         cmd: str,
-        *caller_args,
+        *caller_args: str,
         args: str = "",
         joiner: str = " ",
         separator: str = "::",
         stdout: int = None,
         stderr: int = None,
         **kwargs,
     ) -> _Process:
@@ -108,15 +114,15 @@
             stderr=stderr,
             **kwargs,
         )
 
     async def shell(
         self,
         cmd: str,
-        *caller_args,
+        *caller_args: str,
         args: str = "",
         joiner: str = " ",
         separator: str = "::",
         stdout: int = None,
         stderr: int = None,
         **kwargs,
     ) -> bool:
@@ -134,14 +140,29 @@
                 **kwargs,
             ),
             self.name,
             self.log,
         )
         return proc.returncode == 0
 
+    async def shell_cmd_in_dir(
+        self,
+        path: _Path,
+        cmd: _List[str],
+        joiner: str = " ",
+        cd: str = "cd",
+        **kwargs,
+    ) -> bool:
+        """Run a shell command in a specific directory."""
+
+        path.mkdir(exist_ok=True)
+        return await self.shell(
+            f'( {cd} "{path}"; {joiner.join(cmd)} )', **kwargs
+        )
+
 
 class SubprocessExec(SubprocessLogMixin):
     """A task wrapping a subprocess."""
 
     async def run(
         self,
         inbox: _Inbox,
```

### Comparing `vcorelib-2.2.3/vcorelib/task/time/sleep.py` & `vcorelib-2.3.0/vcorelib/task/time/sleep.py`

 * *Files identical despite different names*

### Comparing `vcorelib-2.2.3/vcorelib.egg-info/PKG-INFO` & `vcorelib-2.3.0/vcorelib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 2.2.3
+Version: 2.3.0
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=f6114ec2f47f68cb9c8196b8c0c35bf4
+    hash=08dfba51dc98120d47088a5ec810ec88
     =====================================
 -->
 
-# vcorelib ([2.2.3](https://pypi.org/project/vcorelib/))
+# vcorelib ([2.3.0](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-2.2.3/vcorelib.egg-info/SOURCES.txt` & `vcorelib-2.3.0/vcorelib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,17 @@
 vcorelib/math/analysis/__init__.py
 vcorelib/math/analysis/average.py
 vcorelib/math/analysis/buffer.py
 vcorelib/math/analysis/weighted.py
 vcorelib/math/analysis/rate/__init__.py
 vcorelib/math/analysis/rate/limiter.py
 vcorelib/paths/__init__.py
+vcorelib/paths/base.py
 vcorelib/paths/context.py
+vcorelib/paths/hashing.py
 vcorelib/paths/info.py
 vcorelib/paths/info_cache.py
 vcorelib/platform/__init__.py
 vcorelib/schemas/__init__.py
 vcorelib/schemas/base.py
 vcorelib/schemas/json.py
 vcorelib/schemas/mixins.py
```


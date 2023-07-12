# Comparing `tmp/audiofile-1.2.1.tar.gz` & `tmp/audiofile-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiofile-1.2.1.tar", last modified: Mon Feb 13 12:00:27 2023, max compression
+gzip compressed data, was "audiofile-1.3.0.tar", last modified: Wed Jul 12 09:01:32 2023, max compression
```

## Comparing `audiofile-1.2.1.tar` & `audiofile-1.3.0.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:00:27.439556 audiofile-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:00:27.431556 audiofile-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:00:27.435556 audiofile-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-02-13 11:59:37.000000 audiofile-1.2.1/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-13 11:59:37.000000 audiofile-1.2.1/.github/workflows/flake8.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-02-13 11:59:37.000000 audiofile-1.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-02-13 11:59:37.000000 audiofile-1.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-13 11:59:37.000000 audiofile-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-13 11:59:37.000000 audiofile-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-02-13 11:59:37.000000 audiofile-1.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-02-13 11:59:37.000000 audiofile-1.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-02-13 11:59:37.000000 audiofile-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-02-13 12:00:27.439556 audiofile-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-02-13 11:59:37.000000 audiofile-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:00:27.435556 audiofile-1.2.1/audiofile/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-13 11:59:37.000000 audiofile-1.2.1/audiofile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:00:27.435556 audiofile-1.2.1/audiofile/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 11:59:37.000000 audiofile-1.2.1/audiofile/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-02-13 11:59:37.000000 audiofile-1.2.1/audiofile/core/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-02-13 11:59:37.000000 audiofile-1.2.1/audiofile/core/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-02-13 11:59:37.000000 audiofile-1.2.1/audiofile/core/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    16696 2023-02-13 11:59:37.000000 audiofile-1.2.1/audiofile/core/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-02-13 11:59:37.000000 audiofile-1.2.1/audiofile/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:00:27.435556 audiofile-1.2.1/audiofile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-02-13 12:00:27.000000 audiofile-1.2.1/audiofile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-02-13 12:00:27.000000 audiofile-1.2.1/audiofile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 12:00:27.000000 audiofile-1.2.1/audiofile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 12:00:27.000000 audiofile-1.2.1/audiofile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-13 12:00:27.000000 audiofile-1.2.1/audiofile.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:00:27.435556 audiofile-1.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:00:27.431556 audiofile-1.2.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:00:27.435556 audiofile-1.2.1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/_templates/autosummary/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:00:27.435556 audiofile-1.2.1/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/api-src/audiofile.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:00:27.435556 audiofile-1.2.1/docs/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/benchmark_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/benchmark_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/generate_audio.sh
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/install_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/requirements.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:00:27.439556 audiofile-1.2.1/docs/benchmark/results/
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/results/benchmark_info_flac.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/results/benchmark_info_mp3.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/results/benchmark_info_mp4.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/results/benchmark_info_ogg.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/results/benchmark_info_wav.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/results/benchmark_mp3-mp4_info.png
--rw-r--r--   0 runner    (1001) docker     (123)    24157 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/results/benchmark_mp3-mp4_read.png
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/results/benchmark_read_flac.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/results/benchmark_read_mp3.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/results/benchmark_read_mp4.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/results/benchmark_read_ogg.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/results/benchmark_read_wav.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/results/benchmark_wav-flac-ogg_info.png
--rw-r--r--   0 runner    (1001) docker     (123)    28211 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/results/benchmark_wav-flac-ogg_read.png
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-02-13 11:59:37.000000 audiofile-1.2.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-13 11:59:37.000000 audiofile-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-02-13 12:00:27.439556 audiofile-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-13 11:59:37.000000 audiofile-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:00:27.439556 audiofile-1.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 12:00:27.439556 audiofile-1.2.1/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-02-13 11:59:37.000000 audiofile-1.2.1/tests/assets/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   137099 2023-02-13 11:59:37.000000 audiofile-1.2.1/tests/assets/gs-16b-1c-44100hz.aac
--rw-r--r--   0 runner    (1001) docker     (123)   649912 2023-02-13 11:59:37.000000 audiofile-1.2.1/tests/assets/gs-16b-1c-44100hz.m4a
--rw-r--r--   0 runner    (1001) docker     (123)   131566 2023-02-13 11:59:37.000000 audiofile-1.2.1/tests/assets/gs-16b-1c-44100hz.opus
--rw-r--r--   0 runner    (1001) docker     (123)    25350 2023-02-13 11:59:37.000000 audiofile-1.2.1/tests/assets/gs-16b-1c-8000hz.amr
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-13 11:59:37.000000 audiofile-1.2.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    41192 2023-02-13 11:59:37.000000 audiofile-1.2.1/tests/test_audiofile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:01:32.893301 audiofile-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-12 09:00:20.000000 audiofile-1.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:01:32.873301 audiofile-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:01:32.877301 audiofile-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-12 09:00:20.000000 audiofile-1.3.0/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-12 09:00:20.000000 audiofile-1.3.0/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-12 09:00:20.000000 audiofile-1.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-12 09:00:20.000000 audiofile-1.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-12 09:00:20.000000 audiofile-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-12 09:00:20.000000 audiofile-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-12 09:00:20.000000 audiofile-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-12 09:00:20.000000 audiofile-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-12 09:00:20.000000 audiofile-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-12 09:01:32.893301 audiofile-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-12 09:00:20.000000 audiofile-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:01:32.877301 audiofile-1.3.0/audiofile/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-12 09:00:20.000000 audiofile-1.3.0/audiofile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:01:32.881301 audiofile-1.3.0/audiofile/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:00:20.000000 audiofile-1.3.0/audiofile/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-12 09:00:20.000000 audiofile-1.3.0/audiofile/core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-12 09:00:20.000000 audiofile-1.3.0/audiofile/core/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-07-12 09:00:20.000000 audiofile-1.3.0/audiofile/core/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17370 2023-07-12 09:00:20.000000 audiofile-1.3.0/audiofile/core/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-12 09:00:20.000000 audiofile-1.3.0/audiofile/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:01:32.877301 audiofile-1.3.0/audiofile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-12 09:01:32.000000 audiofile-1.3.0/audiofile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-12 09:01:32.000000 audiofile-1.3.0/audiofile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:01:32.000000 audiofile-1.3.0/audiofile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:01:32.000000 audiofile-1.3.0/audiofile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-12 09:01:32.000000 audiofile-1.3.0/audiofile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:01:32.881301 audiofile-1.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:01:32.873301 audiofile-1.3.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:01:32.881301 audiofile-1.3.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/_templates/autosummary/function.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:01:32.881301 audiofile-1.3.0/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/api-src/audiofile.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:01:32.885301 audiofile-1.3.0/docs/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/benchmark_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/benchmark_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/generate_audio.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/install_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/requirements.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:01:32.889301 audiofile-1.3.0/docs/benchmark/results/
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/results/benchmark_info_flac.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/results/benchmark_info_mp3.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/results/benchmark_info_mp4.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/results/benchmark_info_ogg.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/results/benchmark_info_wav.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/results/benchmark_mp3-mp4_info.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24157 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/results/benchmark_mp3-mp4_read.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/results/benchmark_read_flac.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/results/benchmark_read_mp3.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/results/benchmark_read_mp4.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/results/benchmark_read_ogg.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/results/benchmark_read_wav.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/results/benchmark_wav-flac-ogg_info.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28211 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/results/benchmark_wav-flac-ogg_read.png
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-12 09:00:20.000000 audiofile-1.3.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-12 09:00:20.000000 audiofile-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 09:00:20.000000 audiofile-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:01:32.893301 audiofile-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:01:32.889301 audiofile-1.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:01:32.893301 audiofile-1.3.0/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-12 09:00:20.000000 audiofile-1.3.0/tests/assets/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   137099 2023-07-12 09:00:20.000000 audiofile-1.3.0/tests/assets/gs-16b-1c-44100hz.aac
+-rw-r--r--   0 runner    (1001) docker     (123)   649912 2023-07-12 09:00:20.000000 audiofile-1.3.0/tests/assets/gs-16b-1c-44100hz.m4a
+-rw-r--r--   0 runner    (1001) docker     (123)   131566 2023-07-12 09:00:20.000000 audiofile-1.3.0/tests/assets/gs-16b-1c-44100hz.opus
+-rw-r--r--   0 runner    (1001) docker     (123)    25350 2023-07-12 09:00:20.000000 audiofile-1.3.0/tests/assets/gs-16b-1c-8000hz.amr
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-12 09:00:20.000000 audiofile-1.3.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    43751 2023-07-12 09:00:20.000000 audiofile-1.3.0/tests/test_audiofile.py
```

### Comparing `audiofile-1.2.1/.github/workflows/doc.yml` & `audiofile-1.3.0/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/.github/workflows/publish.yml` & `audiofile-1.3.0/.github/workflows/publish.yml`

 * *Files 7% similar despite different names*

```diff
@@ -19,22 +19,22 @@
     - name: Prepare Ubuntu
       run: |
         sudo apt-get update
         sudo apt-get install -y sox libsox-fmt-mp3 ffmpeg mediainfo
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install setuptools wheel twine
+        pip install build twine virtualenv
     # PyPI package
     - name: Build and publish
       env:
         TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
         TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
       run: |
-        python setup.py sdist bdist_wheel
+        python -m build
         python -m twine upload dist/*
     # Docuemntation
     - name: Install doc dependencies
       run: |
         pip install -r requirements.txt
         pip install -r docs/requirements.txt
     - name: Build documentation
```

### Comparing `audiofile-1.2.1/.github/workflows/test.yml` & `audiofile-1.3.0/.github/workflows/test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -6,39 +6,37 @@
   pull_request:
     branches: [ main ]
 
 jobs:
   build:
 
     # Make sure .bashrc is read by shell for micromamba,
-    # see https://github.com/mamba-org/provision-with-micromamba#important
+    # see https://github.com/mamba-org/setup-micromamba#about-login-shells
     defaults:
       run:
         shell: bash -l {0}
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ ubuntu-latest, macOS-latest, windows-latest ]
-        python-version: [ '3.7', '3.8', '3.9', '3.10', '3.11' ]
+        python-version: [ '3.8', '3.9', '3.10', '3.11' ]
         sox: [ sox, no-sox ]  # sox binary present or not
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }} with Micromamba
-      uses: mamba-org/provision-with-micromamba@main
+      uses: mamba-org/setup-micromamba@v1
       with:
-        cache-env: true
-        environment-file: false
+        cache-environment: true
         environment-name: venv
-        extra-specs: |
+        create-args: >-
           pip
           python=${{ matrix.python-version }}
-        channels: conda-forge
 
     - name: Activate Python virtual environment
       run: micromamba activate venv
 
     - name: Install sox with Micromamba
       run: micromamba install sox
       if: matrix.sox == 'sox'
```

### Comparing `audiofile-1.2.1/CHANGELOG.rst` & `audiofile-1.3.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,29 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.3.0 (2023-07-12)
+--------------------------
+
+* Changed: evenly round ``offset``
+  and ``duration``
+  after converting to samples
+  in ``audiofile.read()``
+  and ``audiofile.convert_to_wav()``
+  for SND files
+* Fix: ``offset``
+  and ``duration``
+  now behave the same
+  independent of the incoming file format
+
+
 Version 1.2.1 (2023-02-13)
 --------------------------
 
 * Fixed: missing ``pytest`` requirement
   in ``docs/requirements.txt``
```

### Comparing `audiofile-1.2.1/CONTRIBUTING.rst` & `audiofile-1.3.0/CONTRIBUTING.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,112 +1,121 @@
 Contributing
 ============
 
-If you would like to add new functionality fell free to create a
-`pull request`_.
-If you find errors, omissions, inconsistencies or other things that need
-improvement, please create an issue_.
-Contributions are always welcome!
+Everyone is invited to contribute to this project.
+Feel free to create a `pull request`_ .
+If you find errors,
+omissions,
+inconsistencies,
+or other things
+that need improvement,
+please create an issue_.
 
-.. _issue: https://github.com/audeering/audiofile/issues/new
-.. _pull request: https://github.com/audeering/audiofile/compare
+.. _issue: https://github.com/audeering/audiofile/issues/new/
+.. _pull request: https://github.com/audeering/audiofile/compare/
 
 
 Development Installation
 ------------------------
 
-Instead of pip-installing the latest release from PyPI_, you should get the
-newest development version from Github_::
+Instead of pip-installing the latest release from PyPI_,
+you should get the newest development version from Github_::
 
    git clone https://github.com/audeering/audiofile/
    cd audiofile
-   # Create virtual environment, e.g.
-   # virtualenv --python=/usr/bin/python3 --no-site-packages _env
-   # source _env/bin/activate
-   python setup.py develop
-
-.. _PyPI: https://pypi.org/project/audiofile/
-.. _Github: https://github.com/audeering/audiofile/
+   # Create virtual environment for this project
+   # e.g.
+   # virtualenv --python="python3"  $HOME/.envs/audiofile
+   # source $HOME/.envs/audiofile/bin/activate
+   pip install -r requirements.txt
 
-This way, your installation always stays up-to-date, even if you pull new
-changes from the Github_ repository.
 
-If you prefer, you can also replace the last command with::
+This way,
+your installation always stays up-to-date,
+even if you pull new changes from the Github repository.
 
-   pip install -r requirements.txt
+.. _PyPI: https://pypi.org/project/audiofile/
+.. _Github: https://github.com/audeering/audiofile/
 
 
 Coding Convention
 -----------------
 
 We follow the PEP8_ convention for Python code
-and check for correct syntax with flake8_.
-Exceptions are defined under the ``[flake8]`` section
-in :file:`setup.cfg`.
+and check for correct syntax with ruff_.
+In addition,
+we check for common spelling errors with codespell_.
+Both tools and possible exceptions
+are defined in :file:`pyproject.toml`.
 
 The checks are executed in the CI using `pre-commit`_.
 You can enable those checks locally by executing::
 
     pip install pre-commit  # consider system wide installation
     pre-commit install
     pre-commit run --all-files
 
-Afterwards flake8_ is executed
+Afterwards ruff_ and codespell_ are executed
 every time you create a commit.
 
-You can also install flake8_
+You can also install ruff_ and codespell_
 and call it directly::
 
-    pip install flake8  # consider system wide installation
-    flake8
+    pip install ruff codespell  # consider system wide installation
+    ruff check .
+    codespell
 
 It can be restricted to specific folders::
 
-    flake8 audfoo/ tests/
+    ruff check audfoo/ tests/
+    codespell audfoo/ tests/
+
 
+.. _codespell: https://github.com/codespell-project/codespell/
 .. _PEP8: http://www.python.org/dev/peps/pep-0008/
-.. _flake8: https://flake8.pycqa.org/en/latest/index.html
 .. _pre-commit: https://pre-commit.com
+.. _ruff: https://beta.ruff.rs
 
 
 Building the Documentation
 --------------------------
 
-If you make changes to the documentation, you can re-create the HTML pages
-using Sphinx_.
+If you make changes to the documentation,
+you can re-create the HTML pages using Sphinx_.
 You can install it and a few other necessary packages with::
 
    pip install -r docs/requirements.txt
 
 To create the HTML pages, use::
 
-   python setup.py build_sphinx
+   python -m sphinx docs/ build/sphinx/html -b html
 
-The generated files will be available in the directory ``build/sphinx/html/``.
+The generated files will be available
+in the directory :file:`build/sphinx/html/`.
 
 It is also possible to automatically check if all links are still valid::
 
-   python setup.py build_sphinx -b linkcheck
+   python -m sphinx docs/ build/sphinx/html -b linkcheck
 
-.. _Sphinx: http://sphinx-doc.org/
+.. _Sphinx: http://sphinx-doc.org
 
 
 Running the Tests
 -----------------
 
 You'll need pytest_ for that.
 It can be installed with::
 
    pip install -r tests/requirements.txt
 
 To execute the tests, simply run::
 
    python -m pytest
 
-.. _pytest: https://pytest.org/
+.. _pytest: https://pytest.org
 
 
 Creating a New Release
 ----------------------
 
 New releases are made using the following steps:
```

### Comparing `audiofile-1.2.1/LICENSE` & `audiofile-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/README.rst` & `audiofile-1.3.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -41,19 +41,19 @@
 .. _sox: http://sox.sourceforge.net/
 .. _virtualenv: https://virtualenv.pypa.io/
 .. _soundfile: https://pysoundfile.readthedocs.io/
 
 .. |tests| image:: https://github.com/audeering/audiofile/workflows/Test/badge.svg
     :target: https://github.com/audeering/audiofile/actions?query=workflow%3ATest
     :alt: Test status
-.. |coverage| image:: https://codecov.io/gh/audeering/audiofile/branch/master/graph/badge.svg?token=LVF0621BKR
+.. |coverage| image:: https://codecov.io/gh/audeering/audiofile/branch/main/graph/badge.svg?token=LVF0621BKR
     :target: https://codecov.io/gh/audeering/audiofile/
     :alt: code coverage
 .. |docs| image:: https://img.shields.io/pypi/v/audiofile?label=docs
     :target: https://audeering.github.io/audiofile/
     :alt: audiofile's documentation
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/audiofile.svg
     :target: https://pypi.org/project/audiofile/
     :alt: audiofile's supported Python versions
 .. |license| image:: https://img.shields.io/badge/license-MIT-green.svg
-    :target: https://github.com/audeering/audiofile/blob/master/LICENSE
+    :target: https://github.com/audeering/audiofile/blob/main/LICENSE
     :alt: audiofile's MIT license
```

### Comparing `audiofile-1.2.1/audiofile/core/conftest.py` & `audiofile-1.3.0/audiofile/core/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 
 import numpy as np
 import pytest
 
 import audeer
+
 import audiofile
 
 
 np.random.seed(1)
 
 
 @pytest.fixture(scope='session', autouse=True)
```

### Comparing `audiofile-1.2.1/audiofile/core/convert.py` & `audiofile-1.3.0/audiofile/core/convert.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import subprocess
 
-from audiofile.core.utils import (
-    binary_missing_error,
-    broken_file_error,
-    run_ffmpeg,
-    run_sox,
-)
+from audiofile.core.utils import binary_missing_error
+from audiofile.core.utils import broken_file_error
+from audiofile.core.utils import run_ffmpeg
+from audiofile.core.utils import run_sox
 
 
 def convert(
         infile: str,
         outfile: str,
         offset: float = 0,
         duration: float = None,
```

### Comparing `audiofile-1.2.1/audiofile/core/info.py` & `audiofile-1.3.0/audiofile/core/info.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,19 @@
 import typing
 
 import soundfile
 
 import audeer
 
 from audiofile.core.io import convert_to_wav
-from audiofile.core.utils import (
-    binary_missing_error,
-    broken_file_error,
-    file_extension,
-    run,
-    SNDFORMATS,
-)
+from audiofile.core.utils import SNDFORMATS
+from audiofile.core.utils import binary_missing_error
+from audiofile.core.utils import broken_file_error
+from audiofile.core.utils import file_extension
+from audiofile.core.utils import run
 
 
 def bit_depth(file: str) -> typing.Optional[int]:
     r"""Bit depth of audio file.
 
     For lossy audio files,
     ``None`` is returned as they have a varying bit depth.
```

### Comparing `audiofile-1.2.1/audiofile/core/io.py` & `audiofile-1.3.0/audiofile/core/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 import tempfile
 import typing
 
 import numpy as np
 import soundfile
 
 import audeer
+import audmath
 
 from audiofile.core.convert import convert
-from audiofile.core.utils import (
-    duration_in_seconds,
-    file_extension,
-    MAX_CHANNELS,
-    SNDFORMATS,
-)
+from audiofile.core.utils import MAX_CHANNELS
+from audiofile.core.utils import SNDFORMATS
+from audiofile.core.utils import duration_in_seconds
+from audiofile.core.utils import file_extension
 
 
 def convert_to_wav(
         infile: str,
         outfile: str = None,
         offset: typing.Union[float, int, str, np.timedelta64] = None,
         duration: typing.Union[float, int, str, np.timedelta64] = None,
@@ -49,14 +48,18 @@
     for ``offset=None``.
     If the signal is shorter than the requested ``duration`` and/or ``offset``
     only the part of the signal overlapping with the requested signal
     is returned,
     e.g. for a file containing the signal ``[0, 1, 2]``,
     ``duration=2``, ``offset=-4`` will return ``[0]``.
 
+    ``duration`` and ``offset``
+    are evenly rounded
+    after conversion to samples.
+
     It then uses :func:`soundfile.write` to write the WAV file,
     which limits the number of supported channels to 65535.
 
     Args:
         infile: audio/video file name
         outfile: WAV file name.
             If ``None`` same path as ``infile``
@@ -149,14 +152,18 @@
     for ``offset=None``.
     If the signal is shorter than the requested ``duration`` and/or ``offset``
     only the part of the signal overlapping with the requested signal
     is returned,
     e.g. for a file containing the signal ``[0, 1, 2]``,
     ``duration=2``, ``offset=-4`` will return ``[0]``.
 
+    ``duration`` and ``offset``
+    are evenly rounded
+    after conversion to samples.
+
     Args:
         file: file name of input audio file
         duration: return only the specified duration
         offset: start reading at offset
         always_2d: if ``True`` it always returns a two-dimensional signal
             even for mono sound files
         dtype: data type of returned signal,
@@ -363,59 +370,71 @@
             duration = -signal_duration
         else:
             orig_offset = offset
             offset = max([0, signal_duration + offset + duration])
             duration = min([-duration, signal_duration + orig_offset])
             duration = max([0, duration])
 
-    if offset is None:
-        offset = 0
-
-    # Return immediately if duration == 0
+    # Convert to samples
+    #
+    # Handle duration first
+    # and returned immediately
+    # if duration == 0
+    if duration is not None and duration != 0:
+        duration = audmath.samples(duration, sampling_rate)
     if duration == 0:
         from audiofile.core.info import channels as get_channels
         channels = get_channels(file)
         if channels > 1 or always_2d:
             signal = np.zeros((channels, 0))
         else:
             signal = np.zeros((0,))
         return signal, sampling_rate
+    if offset is not None and offset != 0:
+        offset = audmath.samples(offset, sampling_rate)
+    else:
+        offset = 0
 
     tmpdir = None
     if file_extension(file) not in SNDFORMATS:
         # Convert file formats not recognized by soundfile to WAV first.
         #
         # NOTE: this is faster than loading them with librosa directly.
-        # In addition, librosa seems to have an issue with the precission of
+        # In addition, librosa seems to have an issue with the precision of
         # the returned magnitude
         # (https://github.com/librosa/librosa/issues/811).
         #
         # It might be the case that MP3 files will be supported by soundfile in
         # the future as well. For a discussion on MP3 support in the underlying
         # libsndfile see https://github.com/erikd/libsndfile/issues/258.
         with tempfile.TemporaryDirectory(prefix='audiofile') as tmpdir:
             tmpfile = os.path.join(tmpdir, 'tmp.wav')
+            # offset and duration have to be given in seconds
+            if offset != 0:
+                offset /= sampling_rate
+            if duration is not None and duration != 0:
+                duration /= sampling_rate
             convert(file, tmpfile, offset, duration)
             signal, sampling_rate = soundfile.read(
                 tmpfile,
                 dtype=dtype,
                 always_2d=always_2d,
                 **kwargs,
             )
     else:
-        if offset is not None and offset != 0:
-            offset = np.ceil(offset * sampling_rate)  # samples
-        if duration is not None and duration != 0:
-            duration = int(
-                np.ceil(duration * sampling_rate) + offset
-            )  # samples
+        start = offset
+        # duration == 0 is handled further above with immediate return
+        if duration is not None:
+            stop = duration + start
+        else:
+            stop = None
         signal, sampling_rate = soundfile.read(
             file,
-            start=int(offset),
-            stop=duration,
+            start=start,
+            stop=stop,
             dtype=dtype,
             always_2d=always_2d,
             **kwargs,
         )
     # [samples, channels] => [channels, samples]
     signal = signal.T
     return signal, sampling_rate
```

### Comparing `audiofile-1.2.1/audiofile/core/utils.py` & `audiofile-1.3.0/audiofile/core/utils.py`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/audiofile.egg-info/SOURCES.txt` & `audiofile-1.3.0/audiofile.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+.flake8
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 README.rst
+pyproject.toml
 requirements.txt
-setup.cfg
-setup.py
 .github/workflows/doc.yml
-.github/workflows/flake8.yml
+.github/workflows/linter.yml
 .github/workflows/publish.yml
 .github/workflows/test.yml
 audiofile/__init__.py
 audiofile.egg-info/PKG-INFO
 audiofile.egg-info/SOURCES.txt
 audiofile.egg-info/dependency_links.txt
 audiofile.egg-info/requires.txt
```

### Comparing `audiofile-1.2.1/docs/_templates/autosummary/class.rst` & `audiofile-1.3.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/benchmark_info.py` & `audiofile-1.3.0/docs/benchmark/benchmark_info.py`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/benchmark_read.py` & `audiofile-1.3.0/docs/benchmark/benchmark_read.py`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/install_dependencies.sh` & `audiofile-1.3.0/docs/benchmark/install_dependencies.sh`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 fi
 ENV_DIR="${HOME}/.envs/audiofile-benchmark"
 rm -rf ${ENV_DIR}
 virtualenv --python=python3.8 ${ENV_DIR}
 source ${ENV_DIR}/bin/activate
 pip install --upgrade pip
 
-# Enfore rebuolding of wheels
+# Enforce rebuilding of wheels
 pip cache purge
 
 # Fix numpy header include for aubio
 pip install "numpy==1.21.6"
 mkdir -p ${ENV_DIR}/include/
 ln -sf ${ENV_DIR}lib/python3.8/site-packages/numpy/core/include/numpy ${ENV_DIR}/include/
```

### Comparing `audiofile-1.2.1/docs/benchmark/loaders.py` & `audiofile-1.3.0/docs/benchmark/loaders.py`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/plot.py` & `audiofile-1.3.0/docs/benchmark/plot.py`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/requirements.txt.lock` & `audiofile-1.3.0/docs/benchmark/requirements.txt.lock`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/results/benchmark_info_flac.pickle` & `audiofile-1.3.0/docs/benchmark/results/benchmark_info_flac.pickle`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/results/benchmark_info_mp3.pickle` & `audiofile-1.3.0/docs/benchmark/results/benchmark_info_mp3.pickle`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/results/benchmark_info_mp4.pickle` & `audiofile-1.3.0/docs/benchmark/results/benchmark_info_mp4.pickle`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/results/benchmark_info_ogg.pickle` & `audiofile-1.3.0/docs/benchmark/results/benchmark_info_ogg.pickle`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/results/benchmark_info_wav.pickle` & `audiofile-1.3.0/docs/benchmark/results/benchmark_info_wav.pickle`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/results/benchmark_mp3-mp4_info.png` & `audiofile-1.3.0/docs/benchmark/results/benchmark_mp3-mp4_info.png`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/results/benchmark_mp3-mp4_read.png` & `audiofile-1.3.0/docs/benchmark/results/benchmark_mp3-mp4_read.png`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/results/benchmark_read_flac.pickle` & `audiofile-1.3.0/docs/benchmark/results/benchmark_read_flac.pickle`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/results/benchmark_read_mp3.pickle` & `audiofile-1.3.0/docs/benchmark/results/benchmark_read_mp3.pickle`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/results/benchmark_read_mp4.pickle` & `audiofile-1.3.0/docs/benchmark/results/benchmark_read_mp4.pickle`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/results/benchmark_read_ogg.pickle` & `audiofile-1.3.0/docs/benchmark/results/benchmark_read_ogg.pickle`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/results/benchmark_read_wav.pickle` & `audiofile-1.3.0/docs/benchmark/results/benchmark_read_wav.pickle`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/results/benchmark_wav-flac-ogg_info.png` & `audiofile-1.3.0/docs/benchmark/results/benchmark_wav-flac-ogg_info.png`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/results/benchmark_wav-flac-ogg_read.png` & `audiofile-1.3.0/docs/benchmark/results/benchmark_wav-flac-ogg_read.png`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark/utils.py` & `audiofile-1.3.0/docs/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/benchmark.rst` & `audiofile-1.3.0/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/conf.py` & `audiofile-1.3.0/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-import configparser
 from datetime import datetime
-import shutil
 import os
+import shutil
+
+import toml
 
 import audeer
+
 from audiofile.core.conftest import create_audio_files
 
 
-config = configparser.ConfigParser()
-config.read(os.path.join('..', 'setup.cfg'))
+config = toml.load(audeer.path('..', 'pyproject.toml'))
 
 
 # Project -----------------------------------------------------------------
 
-project = config['metadata']['name']
+project = config['project']['name']
 copyright = f'2018-{datetime.now().year} audEERING GmbH'
-author = config['metadata']['author']
+author = ', '.join(
+    author['name'] for author in config['project']['authors']
+)
 version = audeer.git_repo_version()
 title = 'Documentation'
 
 
 # General -----------------------------------------------------------------
 
 master_doc = 'index'
```

### Comparing `audiofile-1.2.1/docs/installation.rst` & `audiofile-1.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/docs/usage.rst` & `audiofile-1.3.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/tests/assets/gs-16b-1c-44100hz.aac` & `audiofile-1.3.0/tests/assets/gs-16b-1c-44100hz.aac`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/tests/assets/gs-16b-1c-44100hz.m4a` & `audiofile-1.3.0/tests/assets/gs-16b-1c-44100hz.m4a`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/tests/assets/gs-16b-1c-44100hz.opus` & `audiofile-1.3.0/tests/assets/gs-16b-1c-44100hz.opus`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/tests/assets/gs-16b-1c-8000hz.amr` & `audiofile-1.3.0/tests/assets/gs-16b-1c-8000hz.amr`

 * *Files identical despite different names*

### Comparing `audiofile-1.2.1/tests/test_audiofile.py` & `audiofile-1.3.0/tests/test_audiofile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,41 @@
-from __future__ import division
 import os
 import re
 import subprocess
 
-import pytest
 import numpy as np
 from numpy.testing import assert_allclose
 import pandas as pd
+import pytest
 import soundfile
 
 import audeer
+
 import audiofile as af
 
 
 SCRIPT_DIR = os.path.dirname(os.path.realpath(__file__))
 ASSETS_DIR = os.path.join(SCRIPT_DIR, 'assets')
 
 
+@pytest.fixture(scope='module')
+def audio_file(tmpdir_factory, request):
+    """Fixture to generate audio file.
+
+    Provide ``(signal, sampling_rate)``
+    as parameter to this fixture.
+
+    """
+    file = str(tmpdir_factory.mktemp('audio').join('file.wav'))
+    signal, sampling_rate = request.param
+    af.write(file, signal, sampling_rate)
+
+    yield file
+
+
 @pytest.fixture(scope='function')
 def empty_file(tmpdir, request):
     """Fixture to generate empty audio files.
 
     The request parameter allows to select the file extension.
 
     """
@@ -435,15 +450,15 @@
         duration = duration - 2 * offset
         sig, fs = af.read(
             file,
             offset=offset,
             duration=duration,
             always_2d=always_2d,
         )
-        assert _samples(sig) == int(np.ceil(duration * sampling_rate))
+        assert _samples(sig) == round(duration * sampling_rate)
 
 
 @pytest.mark.parametrize('magnitude', [0.01, 0.1, 1])
 @pytest.mark.parametrize('normalize', [False, True])
 @pytest.mark.parametrize('bit_depth', [16, 24, 32])
 @pytest.mark.parametrize('sampling_rate', [44100])
 def test_magnitude(tmpdir, magnitude, normalize, bit_depth, sampling_rate):
@@ -561,14 +576,24 @@
             precision = 1
             sloppy_duration = round(af.duration(file, sloppy=True), precision)
             header_duration = round(header_duration, precision)
             assert sloppy_duration == header_duration
         assert af.bit_depth(file) is None
 
 
+@pytest.mark.parametrize(
+    'audio_file',
+    [
+        (
+            np.array([[.0, .0, .1, .1, .2, .2]], dtype=np.float32),
+            2,  # Hz
+        ),
+    ],
+    indirect=True,
+)
 # The following test assumes a signal of 3s length,
 # containing 0 during the first second,
 # 1 during the second second,
 # 2 during the third second.
 @pytest.mark.parametrize(
     'offset, duration, expected',
     [
@@ -1125,23 +1150,22 @@
         ('-4', '-8', [[.0, .0]]),
         ('-5', '-8', [[.0]]),
         ('-6', '-8', [[]]),
         ('-7', '-8', [[]]),
         ('-8', '-8', [[]]),
     ]
 )
-def test_read_duration_and_offset(tmpdir, offset, duration, expected):
-    # Prepare signals
-    sampling_rate = 2
-    signal = np.array([[.0, .0, .1, .1, .2, .2]], dtype=np.float32)
-    file = str(tmpdir.join('signal.wav'))
-    af.write(file, signal, sampling_rate)
-    assert af.duration(file) == 3.0
+def test_read_duration_and_offset(audio_file, offset, duration, expected):
     # Read with provided duration/offset
-    signal, _ = af.read(file, offset=offset, duration=duration, always_2d=True)
+    signal, _ = af.read(
+        audio_file,
+        offset=offset,
+        duration=duration,
+        always_2d=True,
+    )
     np.testing.assert_allclose(
         signal,
         np.array(expected, dtype=np.float32),
         rtol=1e-03,
     )
 
 
@@ -1205,14 +1229,101 @@
         assert_allclose(
             _duration(sig, sampling_rate),
             af.duration(file) - offset_s,
             rtol=0,
             atol=tolerance('duration', sampling_rate),
         )
 
+        # Duration that results in empty signal
+        duration = 0.000001
+        sig, fs = af.read(file, duration=duration)
+        np.testing.assert_array_equal(
+            sig,
+            np.array([], np.float32),
+        )
+
+
+@pytest.mark.parametrize(
+    'audio_file',
+    [
+        (
+            np.array(
+                [[.0, .1, .2, .3, .4, .5, .6, .7, .8, .9]],
+                dtype=np.float32,
+            ),
+            10,  # Hz
+        ),
+    ],
+    indirect=True,
+)
+@pytest.mark.parametrize(
+    # offset and duration need to be given in seconds
+    'offset, duration, expected',
+    [
+        (0.1, 0.1, [.1]),
+        (0.1, 0.03, []),
+        (0.1, 0.15, [.1, .2]),
+        (0.1, 0.19, [.1, .2]),
+        (0.049, 0.19, [.0, .1]),
+        (0.15, 0.15, [.2, .3]),
+    ]
+)
+def test_read_duration_and_offset_rounding(
+        tmpdir,
+        audio_file,
+        offset,
+        duration,
+        expected,
+):
+
+    # Prepare signals
+
+    # Ensure that the rounding from duration to samples
+    # is done as expected
+    # and in the same way
+    # when reading with sox or ffmpeg
+
+    # soundfile
+    signal, _ = af.read(audio_file, offset=offset, duration=duration)
+    np.testing.assert_allclose(
+        signal,
+        np.array(expected, dtype=np.float32),
+        rtol=1e-03,
+    )
+
+    if len(expected) == 0:
+        # duration of 0 is handled inside af.read()
+        # even when duration is only 0 after rounding
+        # as ffmpeg cannot handle those cases
+        return 0
+
+    # sox
+    convert_file = str(tmpdir.join('signal-sox.wav'))
+    try:
+        af.core.utils.run_sox(audio_file, convert_file, offset, duration)
+        signal, _ = af.read(convert_file)
+        np.testing.assert_allclose(
+            signal,
+            np.array(expected, dtype=np.float32),
+            rtol=1e-03,
+        )
+    except FileNotFoundError:
+        # When testing without an installation of sox
+        pass
+
+    # ffmpeg
+    convert_file = str(tmpdir.join('signal-ffmpeg.wav'))
+    af.core.utils.run_ffmpeg(audio_file, convert_file, offset, duration)
+    signal, _ = af.read(convert_file)
+    np.testing.assert_allclose(
+        signal,
+        np.array(expected, dtype=np.float32),
+        rtol=1e-03,
+    )
+
 
 def test_write_errors():
 
     sampling_rate = 44100
 
     # Call with unallowed bit depths
     expected_error = '"bit_depth" has to be one of'
```


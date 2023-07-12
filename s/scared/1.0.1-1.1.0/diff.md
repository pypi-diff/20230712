# Comparing `tmp/scared-1.0.1.tar.gz` & `tmp/scared-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scared-1.0.1.tar", last modified: Wed Jan 25 15:32:22 2023, max compression
+gzip compressed data, was "scared-1.1.0.tar", last modified: Wed Jul 12 09:49:05 2023, max compression
```

## Comparing `scared-1.0.1.tar` & `scared-1.1.0.tar`

### file list

```diff
@@ -1,104 +1,120 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.675820 scared-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)      391 2022-10-21 13:53:41.000000 scared-1.0.1/AUTHORS.md
--rw-rw-rw-   0 root         (0) root         (0)    34506 2022-10-21 13:53:41.000000 scared-1.0.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       52 2022-10-21 13:53:41.000000 scared-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4499 2023-01-25 15:32:22.675820 scared-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3244 2023-01-24 17:26:49.000000 scared-1.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       80 2022-10-21 13:53:41.000000 scared-1.0.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.675820 scared-1.0.1/scared/
--rw-rw-rw-   0 root         (0) root         (0)     2120 2022-10-21 13:53:41.000000 scared-1.0.1/scared/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      802 2022-10-21 13:53:41.000000 scared-1.0.1/scared/_utils.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-01-25 15:32:22.675820 scared-1.0.1/scared/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.575819 scared-1.0.1/scared/aes/
--rw-rw-rw-   0 root         (0) root         (0)       88 2022-10-21 13:53:41.000000 scared-1.0.1/scared/aes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    32993 2022-10-21 13:53:41.000000 scared-1.0.1/scared/aes/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.575819 scared-1.0.1/scared/aes/selection_functions/
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-10-21 13:53:41.000000 scared-1.0.1/scared/aes/selection_functions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3385 2022-10-21 13:53:41.000000 scared-1.0.1/scared/aes/selection_functions/decrypt.py
--rw-rw-rw-   0 root         (0) root         (0)     6109 2022-10-21 13:53:41.000000 scared-1.0.1/scared/aes/selection_functions/encrypt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.575819 scared-1.0.1/scared/analysis/
--rw-rw-rw-   0 root         (0) root         (0)      440 2022-10-21 13:53:41.000000 scared-1.0.1/scared/analysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2964 2022-10-21 13:53:41.000000 scared-1.0.1/scared/analysis/_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    11595 2022-10-21 13:53:41.000000 scared-1.0.1/scared/analysis/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6987 2022-10-21 13:53:41.000000 scared-1.0.1/scared/analysis/template.py
--rw-rw-rw-   0 root         (0) root         (0)     9822 2023-01-20 13:58:14.000000 scared-1.0.1/scared/container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.575819 scared-1.0.1/scared/des/
--rw-rw-rw-   0 root         (0) root         (0)       88 2022-10-21 13:53:41.000000 scared-1.0.1/scared/des/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    41581 2022-10-21 13:53:41.000000 scared-1.0.1/scared/des/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.575819 scared-1.0.1/scared/des/selection_functions/
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-10-21 13:53:41.000000 scared-1.0.1/scared/des/selection_functions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5336 2022-10-21 13:53:41.000000 scared-1.0.1/scared/des/selection_functions/decrypt.py
--rw-rw-rw-   0 root         (0) root         (0)     9345 2022-10-21 13:53:41.000000 scared-1.0.1/scared/des/selection_functions/encrypt.py
--rw-rw-rw-   0 root         (0) root         (0)     2705 2022-10-21 13:53:41.000000 scared-1.0.1/scared/discriminants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.575819 scared-1.0.1/scared/distinguishers/
--rw-rw-rw-   0 root         (0) root         (0)      823 2022-10-21 13:53:41.000000 scared-1.0.1/scared/distinguishers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4945 2022-11-04 21:26:19.000000 scared-1.0.1/scared/distinguishers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4426 2022-10-21 13:53:41.000000 scared-1.0.1/scared/distinguishers/cpa.py
--rw-rw-rw-   0 root         (0) root         (0)     3149 2022-10-21 13:53:41.000000 scared-1.0.1/scared/distinguishers/dpa.py
--rw-rw-rw-   0 root         (0) root         (0)     4952 2022-11-04 21:26:19.000000 scared-1.0.1/scared/distinguishers/mia.py
--rw-rw-rw-   0 root         (0) root         (0)    11666 2022-11-04 21:26:19.000000 scared-1.0.1/scared/distinguishers/partitioned.py
--rw-rw-rw-   0 root         (0) root         (0)     4637 2022-10-21 13:53:41.000000 scared-1.0.1/scared/distinguishers/template.py
--rw-rw-rw-   0 root         (0) root         (0)     7332 2022-10-21 13:53:41.000000 scared-1.0.1/scared/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.575819 scared-1.0.1/scared/preprocesses/
--rw-rw-rw-   0 root         (0) root         (0)      239 2022-10-21 13:53:41.000000 scared-1.0.1/scared/preprocesses/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2302 2022-10-21 13:53:41.000000 scared-1.0.1/scared/preprocesses/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4854 2022-10-21 13:53:41.000000 scared-1.0.1/scared/preprocesses/first_order.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.579819 scared-1.0.1/scared/preprocesses/high_order/
--rw-rw-rw-   0 root         (0) root         (0)      189 2022-10-21 13:53:41.000000 scared-1.0.1/scared/preprocesses/high_order/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4555 2022-10-21 13:53:41.000000 scared-1.0.1/scared/preprocesses/high_order/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7010 2022-10-21 13:53:41.000000 scared-1.0.1/scared/preprocesses/high_order/standard.py
--rw-rw-rw-   0 root         (0) root         (0)     8826 2022-10-21 13:53:41.000000 scared-1.0.1/scared/preprocesses/high_order/time_freq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.579819 scared-1.0.1/scared/selection_functions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2022-10-21 13:53:41.000000 scared-1.0.1/scared/selection_functions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7508 2022-10-21 13:53:41.000000 scared-1.0.1/scared/selection_functions/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.579819 scared-1.0.1/scared/signal_processing/
--rwxrwxrwx   0 root         (0) root         (0)      466 2022-10-21 13:53:41.000000 scared-1.0.1/scared/signal_processing/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3396 2022-10-21 13:53:41.000000 scared-1.0.1/scared/signal_processing/base.py
--rwxrwxrwx   0 root         (0) root         (0)     4731 2022-10-21 13:53:41.000000 scared-1.0.1/scared/signal_processing/filters.py
--rwxrwxrwx   0 root         (0) root         (0)     1937 2022-10-21 13:53:41.000000 scared-1.0.1/scared/signal_processing/frequency_analysis.py
--rwxrwxrwx   0 root         (0) root         (0)     6585 2022-10-21 13:53:41.000000 scared-1.0.1/scared/signal_processing/moving_operators.py
--rwxrwxrwx   0 root         (0) root         (0)     4751 2022-10-21 13:53:41.000000 scared-1.0.1/scared/signal_processing/pattern_detection.py
--rwxrwxrwx   0 root         (0) root         (0)     7697 2022-10-21 13:53:41.000000 scared-1.0.1/scared/signal_processing/peaks_detection.py
--rwxrwxrwx   0 root         (0) root         (0)     7903 2022-10-21 13:53:41.000000 scared-1.0.1/scared/synchronization.py
--rw-rw-rw-   0 root         (0) root         (0)     9154 2023-01-19 13:29:02.000000 scared-1.0.1/scared/ttest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.575819 scared-1.0.1/scared.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4499 2023-01-25 15:32:22.000000 scared-1.0.1/scared.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2870 2023-01-25 15:32:22.000000 scared-1.0.1/scared.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-25 15:32:22.000000 scared-1.0.1/scared.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-25 15:32:22.000000 scared-1.0.1/scared.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      131 2023-01-25 15:32:22.000000 scared-1.0.1/scared.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-01-25 15:32:22.000000 scared-1.0.1/scared.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1544 2023-01-25 15:32:22.675820 scared-1.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      645 2022-10-21 13:53:41.000000 scared-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.559819 scared-1.0.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.599819 scared-1.0.1/tests/distinguishers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-21 13:53:41.000000 scared-1.0.1/tests/distinguishers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13933 2022-10-21 13:53:41.000000 scared-1.0.1/tests/distinguishers/test_distinguishers.py
--rw-rw-rw-   0 root         (0) root         (0)     9056 2022-11-04 21:26:19.000000 scared-1.0.1/tests/distinguishers/test_mia_distinguishers.py
--rw-rw-rw-   0 root         (0) root         (0)    14203 2022-11-04 21:26:19.000000 scared-1.0.1/tests/distinguishers/test_partitioned_distinguishers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.603819 scared-1.0.1/tests/end_to_end/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-21 13:53:41.000000 scared-1.0.1/tests/end_to_end/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2022-10-21 13:53:41.000000 scared-1.0.1/tests/end_to_end/test_e2e_anova.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2022-10-21 13:53:41.000000 scared-1.0.1/tests/end_to_end/test_e2e_cpa.py
--rw-rw-rw-   0 root         (0) root         (0)     1028 2022-10-21 13:53:41.000000 scared-1.0.1/tests/end_to_end/test_e2e_dpa.py
--rw-rw-rw-   0 root         (0) root         (0)      754 2023-01-19 13:29:02.000000 scared-1.0.1/tests/end_to_end/test_e2e_mia.py
--rw-rw-rw-   0 root         (0) root         (0)      642 2022-10-21 13:53:41.000000 scared-1.0.1/tests/end_to_end/test_e2e_nicv.py
--rw-rw-rw-   0 root         (0) root         (0)      762 2022-10-21 13:53:41.000000 scared-1.0.1/tests/end_to_end/test_e2e_snr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.663820 scared-1.0.1/tests/preprocesses/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-21 13:53:41.000000 scared-1.0.1/tests/preprocesses/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3344 2022-10-21 13:53:41.000000 scared-1.0.1/tests/preprocesses/test_preprocess_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     7982 2022-10-21 13:53:41.000000 scared-1.0.1/tests/preprocesses/test_preprocesses_absolute_difference_combination.py
--rw-rw-rw-   0 root         (0) root         (0)     7903 2022-10-21 13:53:41.000000 scared-1.0.1/tests/preprocesses/test_preprocesses_centered_product.py
--rw-rw-rw-   0 root         (0) root         (0)     7199 2022-10-21 13:53:41.000000 scared-1.0.1/tests/preprocesses/test_preprocesses_difference_combination.py
--rw-rw-rw-   0 root         (0) root         (0)     7301 2022-10-21 13:53:41.000000 scared-1.0.1/tests/preprocesses/test_preprocesses_product_combination.py
--rw-rw-rw-   0 root         (0) root         (0)     6547 2022-10-21 13:53:41.000000 scared-1.0.1/tests/preprocesses/test_preprocesses_simple.py
--rw-rw-rw-   0 root         (0) root         (0)     9116 2022-10-21 13:53:41.000000 scared-1.0.1/tests/preprocesses/test_preprocesses_timefreq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 15:32:22.675820 scared-1.0.1/tests/signal_processing/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-10-21 13:53:41.000000 scared-1.0.1/tests/signal_processing/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4196 2022-10-21 13:53:41.000000 scared-1.0.1/tests/signal_processing/test_base.py
--rwxrwxrwx   0 root         (0) root         (0)     8664 2022-10-21 13:53:41.000000 scared-1.0.1/tests/signal_processing/test_filters.py
--rwxrwxrwx   0 root         (0) root         (0)     2585 2022-10-21 13:53:41.000000 scared-1.0.1/tests/signal_processing/test_frequency_analysis.py
--rwxrwxrwx   0 root         (0) root         (0)    14078 2022-10-21 13:53:41.000000 scared-1.0.1/tests/signal_processing/test_moving_operators.py
--rwxrwxrwx   0 root         (0) root         (0)     7703 2022-10-21 13:53:41.000000 scared-1.0.1/tests/signal_processing/test_pattern_detection.py
--rwxrwxrwx   0 root         (0) root         (0)    15670 2022-10-21 13:53:41.000000 scared-1.0.1/tests/signal_processing/test_peaks_detection.py
--rw-rw-rw-   0 root         (0) root         (0)    81295 2022-10-21 13:53:41.000000 scared-1.0.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.236833 scared-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-12 09:27:01.000000 scared-1.1.0/AUTHORS.md
+-rw-rw-rw-   0 root         (0) root         (0)    34506 2023-07-12 09:27:01.000000 scared-1.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-12 09:27:01.000000 scared-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4501 2023-07-12 09:49:05.236833 scared-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3244 2023-07-12 09:27:01.000000 scared-1.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-12 09:27:01.000000 scared-1.1.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.236833 scared-1.1.0/scared/
+-rw-rw-rw-   0 root         (0) root         (0)     2120 2023-07-12 09:27:01.000000 scared-1.1.0/scared/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-07-12 09:27:01.000000 scared-1.1.0/scared/_utils.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-07-12 09:49:05.236833 scared-1.1.0/scared/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.228833 scared-1.1.0/scared/aes/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-12 09:27:01.000000 scared-1.1.0/scared/aes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32993 2023-07-12 09:27:01.000000 scared-1.1.0/scared/aes/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.228833 scared-1.1.0/scared/aes/selection_functions/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-07-12 09:27:01.000000 scared-1.1.0/scared/aes/selection_functions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3385 2023-07-12 09:27:01.000000 scared-1.1.0/scared/aes/selection_functions/decrypt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6109 2023-07-12 09:27:01.000000 scared-1.1.0/scared/aes/selection_functions/encrypt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.228833 scared-1.1.0/scared/analysis/
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-07-12 09:27:01.000000 scared-1.1.0/scared/analysis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2964 2023-07-12 09:27:01.000000 scared-1.1.0/scared/analysis/_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    11595 2023-07-12 09:27:01.000000 scared-1.1.0/scared/analysis/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6987 2023-07-12 09:27:01.000000 scared-1.1.0/scared/analysis/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     9822 2023-07-12 09:27:01.000000 scared-1.1.0/scared/container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.228833 scared-1.1.0/scared/des/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-12 09:27:01.000000 scared-1.1.0/scared/des/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    41581 2023-07-12 09:27:01.000000 scared-1.1.0/scared/des/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.228833 scared-1.1.0/scared/des/selection_functions/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-07-12 09:27:01.000000 scared-1.1.0/scared/des/selection_functions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5336 2023-07-12 09:27:01.000000 scared-1.1.0/scared/des/selection_functions/decrypt.py
+-rw-rw-rw-   0 root         (0) root         (0)     9345 2023-07-12 09:27:01.000000 scared-1.1.0/scared/des/selection_functions/encrypt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2705 2023-07-12 09:27:01.000000 scared-1.1.0/scared/discriminants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.228833 scared-1.1.0/scared/distinguishers/
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-07-12 09:27:01.000000 scared-1.1.0/scared/distinguishers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4945 2023-07-12 09:27:01.000000 scared-1.1.0/scared/distinguishers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4426 2023-07-12 09:27:01.000000 scared-1.1.0/scared/distinguishers/cpa.py
+-rw-rw-rw-   0 root         (0) root         (0)     3149 2023-07-12 09:27:01.000000 scared-1.1.0/scared/distinguishers/dpa.py
+-rw-rw-rw-   0 root         (0) root         (0)     4952 2023-07-12 09:27:01.000000 scared-1.1.0/scared/distinguishers/mia.py
+-rw-rw-rw-   0 root         (0) root         (0)    11666 2023-07-12 09:27:01.000000 scared-1.1.0/scared/distinguishers/partitioned.py
+-rw-rw-rw-   0 root         (0) root         (0)     4637 2023-07-12 09:27:01.000000 scared-1.1.0/scared/distinguishers/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     7332 2023-07-12 09:27:01.000000 scared-1.1.0/scared/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.228833 scared-1.1.0/scared/preprocesses/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-12 09:27:01.000000 scared-1.1.0/scared/preprocesses/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2302 2023-07-12 09:27:01.000000 scared-1.1.0/scared/preprocesses/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4854 2023-07-12 09:27:01.000000 scared-1.1.0/scared/preprocesses/first_order.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.232833 scared-1.1.0/scared/preprocesses/high_order/
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-07-12 09:27:01.000000 scared-1.1.0/scared/preprocesses/high_order/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4555 2023-07-12 09:27:01.000000 scared-1.1.0/scared/preprocesses/high_order/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7010 2023-07-12 09:27:01.000000 scared-1.1.0/scared/preprocesses/high_order/standard.py
+-rw-rw-rw-   0 root         (0) root         (0)     8826 2023-07-12 09:27:01.000000 scared-1.1.0/scared/preprocesses/high_order/time_freq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.232833 scared-1.1.0/scared/selection_functions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-12 09:27:01.000000 scared-1.1.0/scared/selection_functions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7508 2023-07-12 09:27:01.000000 scared-1.1.0/scared/selection_functions/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.232833 scared-1.1.0/scared/signal_processing/
+-rwxrwxrwx   0 root         (0) root         (0)      466 2023-07-12 09:27:01.000000 scared-1.1.0/scared/signal_processing/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3396 2023-07-12 09:27:01.000000 scared-1.1.0/scared/signal_processing/base.py
+-rwxrwxrwx   0 root         (0) root         (0)     4731 2023-07-12 09:27:01.000000 scared-1.1.0/scared/signal_processing/filters.py
+-rwxrwxrwx   0 root         (0) root         (0)     1937 2023-07-12 09:27:01.000000 scared-1.1.0/scared/signal_processing/frequency_analysis.py
+-rwxrwxrwx   0 root         (0) root         (0)     6585 2023-07-12 09:27:01.000000 scared-1.1.0/scared/signal_processing/moving_operators.py
+-rwxrwxrwx   0 root         (0) root         (0)     4751 2023-07-12 09:27:01.000000 scared-1.1.0/scared/signal_processing/pattern_detection.py
+-rwxrwxrwx   0 root         (0) root         (0)     7697 2023-07-12 09:27:01.000000 scared-1.1.0/scared/signal_processing/peaks_detection.py
+-rwxrwxrwx   0 root         (0) root         (0)     7903 2023-07-12 09:27:01.000000 scared-1.1.0/scared/synchronization.py
+-rw-rw-rw-   0 root         (0) root         (0)     9154 2023-07-12 09:27:01.000000 scared-1.1.0/scared/ttest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.228833 scared-1.1.0/scared.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4501 2023-07-12 09:49:05.000000 scared-1.1.0/scared.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3302 2023-07-12 09:49:05.000000 scared-1.1.0/scared.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 09:49:05.000000 scared-1.1.0/scared.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 09:49:05.000000 scared-1.1.0/scared.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-12 09:49:05.000000 scared-1.1.0/scared.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 09:49:05.000000 scared-1.1.0/scared.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1546 2023-07-12 09:49:05.236833 scared-1.1.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      645 2023-07-12 09:27:01.000000 scared-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.232833 scared-1.1.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.232833 scared-1.1.0/tests/distinguishers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 09:49:01.000000 scared-1.1.0/tests/distinguishers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13933 2023-07-12 09:27:01.000000 scared-1.1.0/tests/distinguishers/test_distinguishers.py
+-rw-rw-rw-   0 root         (0) root         (0)     9056 2023-07-12 09:27:01.000000 scared-1.1.0/tests/distinguishers/test_mia_distinguishers.py
+-rw-rw-rw-   0 root         (0) root         (0)    14203 2023-07-12 09:27:01.000000 scared-1.1.0/tests/distinguishers/test_partitioned_distinguishers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.236833 scared-1.1.0/tests/end_to_end/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 09:49:01.000000 scared-1.1.0/tests/end_to_end/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-12 09:27:01.000000 scared-1.1.0/tests/end_to_end/test_e2e_anova.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-07-12 09:27:01.000000 scared-1.1.0/tests/end_to_end/test_e2e_cpa.py
+-rw-rw-rw-   0 root         (0) root         (0)     1028 2023-07-12 09:27:01.000000 scared-1.1.0/tests/end_to_end/test_e2e_dpa.py
+-rw-rw-rw-   0 root         (0) root         (0)      754 2023-07-12 09:27:01.000000 scared-1.1.0/tests/end_to_end/test_e2e_mia.py
+-rw-rw-rw-   0 root         (0) root         (0)      642 2023-07-12 09:27:01.000000 scared-1.1.0/tests/end_to_end/test_e2e_nicv.py
+-rw-rw-rw-   0 root         (0) root         (0)      762 2023-07-12 09:27:01.000000 scared-1.1.0/tests/end_to_end/test_e2e_snr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.236833 scared-1.1.0/tests/preprocesses/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 09:49:01.000000 scared-1.1.0/tests/preprocesses/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3344 2023-07-12 09:27:01.000000 scared-1.1.0/tests/preprocesses/test_preprocess_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     7982 2023-07-12 09:27:01.000000 scared-1.1.0/tests/preprocesses/test_preprocesses_absolute_difference_combination.py
+-rw-rw-rw-   0 root         (0) root         (0)     7903 2023-07-12 09:27:01.000000 scared-1.1.0/tests/preprocesses/test_preprocesses_centered_product.py
+-rw-rw-rw-   0 root         (0) root         (0)     7199 2023-07-12 09:27:01.000000 scared-1.1.0/tests/preprocesses/test_preprocesses_difference_combination.py
+-rw-rw-rw-   0 root         (0) root         (0)     7301 2023-07-12 09:27:01.000000 scared-1.1.0/tests/preprocesses/test_preprocesses_product_combination.py
+-rw-rw-rw-   0 root         (0) root         (0)     6547 2023-07-12 09:27:01.000000 scared-1.1.0/tests/preprocesses/test_preprocesses_simple.py
+-rw-rw-rw-   0 root         (0) root         (0)     9116 2023-07-12 09:27:01.000000 scared-1.1.0/tests/preprocesses/test_preprocesses_timefreq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:49:05.236833 scared-1.1.0/tests/signal_processing/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-07-12 09:49:01.000000 scared-1.1.0/tests/signal_processing/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4196 2023-07-12 09:27:01.000000 scared-1.1.0/tests/signal_processing/test_base.py
+-rwxrwxrwx   0 root         (0) root         (0)     8664 2023-07-12 09:27:01.000000 scared-1.1.0/tests/signal_processing/test_filters.py
+-rwxrwxrwx   0 root         (0) root         (0)     2585 2023-07-12 09:27:01.000000 scared-1.1.0/tests/signal_processing/test_frequency_analysis.py
+-rwxrwxrwx   0 root         (0) root         (0)    14078 2023-07-12 09:27:01.000000 scared-1.1.0/tests/signal_processing/test_moving_operators.py
+-rwxrwxrwx   0 root         (0) root         (0)     7703 2023-07-12 09:27:01.000000 scared-1.1.0/tests/signal_processing/test_pattern_detection.py
+-rwxrwxrwx   0 root         (0) root         (0)    15670 2023-07-12 09:27:01.000000 scared-1.1.0/tests/signal_processing/test_peaks_detection.py
+-rw-rw-rw-   0 root         (0) root         (0)    29168 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_aes.py
+-rw-rw-rw-   0 root         (0) root         (0)    19344 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_aes_selection_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    19223 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_attacks_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    13660 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_container.py
+-rw-rw-rw-   0 root         (0) root         (0)    35237 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_des.py
+-rw-rw-rw-   0 root         (0) root         (0)    33970 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_des_selection_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2032 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_discriminants.py
+-rw-rw-rw-   0 root         (0) root         (0)     9802 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     8540 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_reverses_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    12396 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_selection_function.py
+-rwxrwxrwx   0 root         (0) root         (0)    11836 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_synchronization.py
+-rw-rw-rw-   0 root         (0) root         (0)    20890 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_template_attack.py
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_traces.py
+-rw-rw-rw-   0 root         (0) root         (0)    11965 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_ttest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1871 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_ttest_container.py
+-rw-rw-rw-   0 root         (0) root         (0)     3625 2023-07-12 09:27:01.000000 scared-1.1.0/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    81295 2023-07-12 09:27:01.000000 scared-1.1.0/versioneer.py
```

### Comparing `scared-1.0.1/LICENSE` & `scared-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/PKG-INFO` & `scared-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: scared
-Version: 1.0.1
+Version: 1.1.0
 Summary: scared is a side-channel analysis framework.
 Home-page: https://gitlab.com/eshard/scared
 Author: eshard
 Author-email: scared@eshard.com
 Project-URL: eShard, https://www.eshard.com
 Project-URL: Documentation, https://eshard.gitlab.io/scared
 Project-URL: Issues, https://gitlab.com/eshard/scared/issues
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Jupyter
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.0<3.11
+Requires-Python: <3.12,>=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # SCAred
```

### Comparing `scared-1.0.1/README.md` & `scared-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/__init__.py` & `scared-1.1.0/scared/__init__.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/_utils.py` & `scared-1.1.0/scared/_utils.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/aes/base.py` & `scared-1.1.0/scared/aes/base.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/aes/selection_functions/decrypt.py` & `scared-1.1.0/scared/aes/selection_functions/decrypt.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/aes/selection_functions/encrypt.py` & `scared-1.1.0/scared/aes/selection_functions/encrypt.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/analysis/_analysis.py` & `scared-1.1.0/scared/analysis/_analysis.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/analysis/base.py` & `scared-1.1.0/scared/analysis/base.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/analysis/template.py` & `scared-1.1.0/scared/analysis/template.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/container.py` & `scared-1.1.0/scared/container.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/des/base.py` & `scared-1.1.0/scared/des/base.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/des/selection_functions/decrypt.py` & `scared-1.1.0/scared/des/selection_functions/decrypt.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/des/selection_functions/encrypt.py` & `scared-1.1.0/scared/des/selection_functions/encrypt.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/discriminants.py` & `scared-1.1.0/scared/discriminants.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/distinguishers/__init__.py` & `scared-1.1.0/scared/distinguishers/__init__.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/distinguishers/base.py` & `scared-1.1.0/scared/distinguishers/base.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/distinguishers/cpa.py` & `scared-1.1.0/scared/distinguishers/cpa.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/distinguishers/dpa.py` & `scared-1.1.0/scared/distinguishers/dpa.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/distinguishers/mia.py` & `scared-1.1.0/scared/distinguishers/mia.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/distinguishers/partitioned.py` & `scared-1.1.0/scared/distinguishers/partitioned.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/distinguishers/template.py` & `scared-1.1.0/scared/distinguishers/template.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/models.py` & `scared-1.1.0/scared/models.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/preprocesses/_base.py` & `scared-1.1.0/scared/preprocesses/_base.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/preprocesses/first_order.py` & `scared-1.1.0/scared/preprocesses/first_order.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/preprocesses/high_order/_base.py` & `scared-1.1.0/scared/preprocesses/high_order/_base.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/preprocesses/high_order/standard.py` & `scared-1.1.0/scared/preprocesses/high_order/standard.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/preprocesses/high_order/time_freq.py` & `scared-1.1.0/scared/preprocesses/high_order/time_freq.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/selection_functions/base.py` & `scared-1.1.0/scared/selection_functions/base.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/signal_processing/base.py` & `scared-1.1.0/scared/signal_processing/base.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/signal_processing/filters.py` & `scared-1.1.0/scared/signal_processing/filters.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/signal_processing/frequency_analysis.py` & `scared-1.1.0/scared/signal_processing/frequency_analysis.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/signal_processing/moving_operators.py` & `scared-1.1.0/scared/signal_processing/moving_operators.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/signal_processing/pattern_detection.py` & `scared-1.1.0/scared/signal_processing/pattern_detection.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/signal_processing/peaks_detection.py` & `scared-1.1.0/scared/signal_processing/peaks_detection.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/synchronization.py` & `scared-1.1.0/scared/synchronization.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared/ttest.py` & `scared-1.1.0/scared/ttest.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/scared.egg-info/PKG-INFO` & `scared-1.1.0/scared.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: scared
-Version: 1.0.1
+Version: 1.1.0
 Summary: scared is a side-channel analysis framework.
 Home-page: https://gitlab.com/eshard/scared
 Author: eshard
 Author-email: scared@eshard.com
 Project-URL: eShard, https://www.eshard.com
 Project-URL: Documentation, https://eshard.gitlab.io/scared
 Project-URL: Issues, https://gitlab.com/eshard/scared/issues
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Jupyter
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.0<3.11
+Requires-Python: <3.12,>=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # SCAred
```

### Comparing `scared-1.0.1/scared.egg-info/SOURCES.txt` & `scared-1.1.0/scared.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -53,14 +53,30 @@
 scared/signal_processing/__init__.py
 scared/signal_processing/base.py
 scared/signal_processing/filters.py
 scared/signal_processing/frequency_analysis.py
 scared/signal_processing/moving_operators.py
 scared/signal_processing/pattern_detection.py
 scared/signal_processing/peaks_detection.py
+tests/test_aes.py
+tests/test_aes_selection_functions.py
+tests/test_attacks_analysis.py
+tests/test_container.py
+tests/test_des.py
+tests/test_des_selection_functions.py
+tests/test_discriminants.py
+tests/test_models.py
+tests/test_reverses_analysis.py
+tests/test_selection_function.py
+tests/test_synchronization.py
+tests/test_template_attack.py
+tests/test_traces.py
+tests/test_ttest.py
+tests/test_ttest_container.py
+tests/test_utils.py
 tests/distinguishers/__init__.py
 tests/distinguishers/test_distinguishers.py
 tests/distinguishers/test_mia_distinguishers.py
 tests/distinguishers/test_partitioned_distinguishers.py
 tests/end_to_end/__init__.py
 tests/end_to_end/test_e2e_anova.py
 tests/end_to_end/test_e2e_cpa.py
```

### Comparing `scared-1.0.1/setup.cfg` & `scared-1.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 long_description_content_type = text/markdown
 url = https://gitlab.com/eshard/scared
 project_urls = 
 	eShard=https://www.eshard.com
 	Documentation=https://eshard.gitlab.io/scared
 	Issues=https://gitlab.com/eshard/scared/issues
 classifiers = 
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Framework :: Jupyter
 	Framework :: IPython
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	Intended Audience :: Science/Research
@@ -28,15 +28,15 @@
 	Topic :: Software Development
 	Operating System :: OS Independent
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
-python_requires = >=3.7.0<3.11
+python_requires = >=3.7.0,<3.12
 install_requires = 
 	numba
 	numpy >=1.20.3
 	estraces
 	psutil
 	scipy
 test_suite = tests
```

### Comparing `scared-1.0.1/setup.py` & `scared-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/distinguishers/test_distinguishers.py` & `scared-1.1.0/tests/distinguishers/test_distinguishers.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/distinguishers/test_mia_distinguishers.py` & `scared-1.1.0/tests/distinguishers/test_mia_distinguishers.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/distinguishers/test_partitioned_distinguishers.py` & `scared-1.1.0/tests/distinguishers/test_partitioned_distinguishers.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/end_to_end/test_e2e_anova.py` & `scared-1.1.0/tests/end_to_end/test_e2e_anova.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/end_to_end/test_e2e_cpa.py` & `scared-1.1.0/tests/end_to_end/test_e2e_cpa.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/end_to_end/test_e2e_dpa.py` & `scared-1.1.0/tests/end_to_end/test_e2e_dpa.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/end_to_end/test_e2e_mia.py` & `scared-1.1.0/tests/end_to_end/test_e2e_mia.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/end_to_end/test_e2e_nicv.py` & `scared-1.1.0/tests/end_to_end/test_e2e_nicv.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/end_to_end/test_e2e_snr.py` & `scared-1.1.0/tests/end_to_end/test_e2e_snr.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/preprocesses/test_preprocess_decorator.py` & `scared-1.1.0/tests/preprocesses/test_preprocess_decorator.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/preprocesses/test_preprocesses_absolute_difference_combination.py` & `scared-1.1.0/tests/preprocesses/test_preprocesses_absolute_difference_combination.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/preprocesses/test_preprocesses_centered_product.py` & `scared-1.1.0/tests/preprocesses/test_preprocesses_centered_product.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/preprocesses/test_preprocesses_difference_combination.py` & `scared-1.1.0/tests/preprocesses/test_preprocesses_difference_combination.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/preprocesses/test_preprocesses_product_combination.py` & `scared-1.1.0/tests/preprocesses/test_preprocesses_product_combination.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/preprocesses/test_preprocesses_simple.py` & `scared-1.1.0/tests/preprocesses/test_preprocesses_simple.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/preprocesses/test_preprocesses_timefreq.py` & `scared-1.1.0/tests/preprocesses/test_preprocesses_timefreq.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/signal_processing/test_base.py` & `scared-1.1.0/tests/signal_processing/test_base.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/signal_processing/test_filters.py` & `scared-1.1.0/tests/signal_processing/test_filters.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/signal_processing/test_frequency_analysis.py` & `scared-1.1.0/tests/signal_processing/test_frequency_analysis.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/signal_processing/test_moving_operators.py` & `scared-1.1.0/tests/signal_processing/test_moving_operators.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/signal_processing/test_pattern_detection.py` & `scared-1.1.0/tests/signal_processing/test_pattern_detection.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/tests/signal_processing/test_peaks_detection.py` & `scared-1.1.0/tests/signal_processing/test_peaks_detection.py`

 * *Files identical despite different names*

### Comparing `scared-1.0.1/versioneer.py` & `scared-1.1.0/versioneer.py`

 * *Files identical despite different names*


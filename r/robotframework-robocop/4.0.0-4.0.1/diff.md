# Comparing `tmp/robotframework-robocop-4.0.0.tar.gz` & `tmp/robotframework-robocop-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-robocop-4.0.0.tar", last modified: Sun Jul  9 18:38:53 2023, max compression
+gzip compressed data, was "robotframework-robocop-4.0.1.tar", last modified: Wed Jul 12 12:49:04 2023, max compression
```

## Comparing `robotframework-robocop-4.0.0.tar` & `robotframework-robocop-4.0.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:38:53.237940 robotframework-robocop-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-07-09 18:38:53.237940 robotframework-robocop-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:38:53.233940 robotframework-robocop-4.0.0/robocop/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:38:53.233940 robotframework-robocop-4.0.0/robocop/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17812 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/duplications.py
--rw-r--r--   0 runner    (1001) docker     (123)    25343 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    29873 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/lengths.py
--rw-r--r--   0 runner    (1001) docker     (123)    51778 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    47251 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/naming.py
--rw-r--r--   0 runner    (1001) docker     (123)    34167 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    25154 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:38:53.233940 robotframework-robocop-4.0.0/robocop/reports/
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/compare_runs_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/file_stats_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/json_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/return_status_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/robocop_version_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/rules_by_id_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/rules_by_severity_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/sarif_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/time_taken_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/timestamp_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:38:53.233940 robotframework-robocop-4.0.0/robocop/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/utils/disablers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/utils/file_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/utils/run_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/utils/version_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:38:53.237940 robotframework-robocop-4.0.0/robotframework_robocop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-07-09 18:38:53.000000 robotframework-robocop-4.0.0/robotframework_robocop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-09 18:38:53.000000 robotframework-robocop-4.0.0/robotframework_robocop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:38:53.000000 robotframework-robocop-4.0.0/robotframework_robocop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 18:38:53.000000 robotframework-robocop-4.0.0/robotframework_robocop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-09 18:38:53.000000 robotframework-robocop-4.0.0/robotframework_robocop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 18:38:53.000000 robotframework-robocop-4.0.0/robotframework_robocop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:38:53.237940 robotframework-robocop-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:49:04.265009 robotframework-robocop-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-07-12 12:49:04.265009 robotframework-robocop-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:49:04.257009 robotframework-robocop-4.0.1/robocop/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:49:04.261009 robotframework-robocop-4.0.1/robocop/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/checkers/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/checkers/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17812 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/checkers/duplications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25343 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/checkers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29873 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/checkers/lengths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51778 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/checkers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/checkers/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34167 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/checkers/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/checkers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25154 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:49:04.261009 robotframework-robocop-4.0.1/robocop/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/reports/compare_runs_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/reports/file_stats_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/reports/json_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/reports/return_status_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/reports/robocop_version_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/reports/rules_by_id_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/reports/rules_by_severity_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/reports/sarif_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/reports/time_taken_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/reports/timestamp_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:49:04.265009 robotframework-robocop-4.0.1/robocop/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/utils/disablers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/utils/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/utils/run_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/utils/version_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/robocop/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:49:04.265009 robotframework-robocop-4.0.1/robotframework_robocop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-07-12 12:49:04.000000 robotframework-robocop-4.0.1/robotframework_robocop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-12 12:49:04.000000 robotframework-robocop-4.0.1/robotframework_robocop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:49:04.000000 robotframework-robocop-4.0.1/robotframework_robocop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 12:49:04.000000 robotframework-robocop-4.0.1/robotframework_robocop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-12 12:49:04.000000 robotframework-robocop-4.0.1/robotframework_robocop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 12:49:04.000000 robotframework-robocop-4.0.1/robotframework_robocop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:49:04.265009 robotframework-robocop-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-12 12:48:53.000000 robotframework-robocop-4.0.1/setup.py
```

### Comparing `robotframework-robocop-4.0.0/LICENSE` & `robotframework-robocop-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/PKG-INFO` & `robotframework-robocop-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 4.0.0
+Version: 4.0.1
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
```

### Comparing `robotframework-robocop-4.0.0/README.md` & `robotframework-robocop-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/checkers/__init__.py` & `robotframework-robocop-4.0.1/robocop/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/checkers/comments.py` & `robotframework-robocop-4.0.1/robocop/checkers/comments.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/checkers/documentation.py` & `robotframework-robocop-4.0.1/robocop/checkers/documentation.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/checkers/duplications.py` & `robotframework-robocop-4.0.1/robocop/checkers/duplications.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/checkers/errors.py` & `robotframework-robocop-4.0.1/robocop/checkers/errors.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/checkers/lengths.py` & `robotframework-robocop-4.0.1/robocop/checkers/lengths.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/checkers/misc.py` & `robotframework-robocop-4.0.1/robocop/checkers/misc.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/checkers/naming.py` & `robotframework-robocop-4.0.1/robocop/checkers/naming.py`

 * *Files 1% similar despite different names*

```diff
@@ -1096,33 +1096,36 @@
         and ads a list of all detected variations of this variable in the node as a value,
         then it checks if similar variable was found.
         """
         for child in node.body:
             # read arguments from Keywords
             if isinstance(child, Arguments):
                 for token in child.get_tokens(Token.ARGUMENT):
-                    name, *_ = token.value.split("=", maxsplit=1)
-                    self.assigned_variables[normalize_robot_var_name(name)].append(name.strip())
+                    variable_match = search_variable(token.value, ignore_errors=True)
+                    name = variable_match.name
+                    normalized = normalize_robot_name(variable_match.base)
+                    self.assigned_variables[normalized].append(name)
 
     def find_similar_variables(self, tokens, node):
         for token in tokens:
-            name, *_ = token.value.split("=", maxsplit=1)
-            normalized_token = normalize_robot_var_name(name)
-            if normalized_token in self.assigned_variables and name not in self.assigned_variables[normalized_token]:
+            variable_match = search_variable(token.value, ignore_errors=True)
+            name = variable_match.name
+            normalized = normalize_robot_name(variable_match.base)
+            if normalized in self.assigned_variables and name not in self.assigned_variables[normalized]:
                 self.report(
                     "possible-variable-overwriting",
                     variable_name=name,
                     block_name=self.parent_name,
                     block_type=self.parent_type,
                     node=node,
                     lineno=token.lineno,
                     col=token.col_offset + 1,
                     end_col=token.end_col_offset + 1,
                 )
-            self.assigned_variables[normalized_token].append(name.strip())
+            self.assigned_variables[normalized].append(name)
 
 
 class DeprecatedStatementChecker(VisitorChecker):
     """Checker for deprecated statements."""
 
     reports = ("deprecated-statement", "deprecated-with-name", "deprecated-singular-header")
     deprecated_keywords = {
```

### Comparing `robotframework-robocop-4.0.0/robocop/checkers/spacing.py` & `robotframework-robocop-4.0.1/robocop/checkers/spacing.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/checkers/tags.py` & `robotframework-robocop-4.0.1/robocop/checkers/tags.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/config.py` & `robotframework-robocop-4.0.1/robocop/config.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/exceptions.py` & `robotframework-robocop-4.0.1/robocop/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/files.py` & `robotframework-robocop-4.0.1/robocop/files.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/reports/__init__.py` & `robotframework-robocop-4.0.1/robocop/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/reports/compare_runs_report.py` & `robotframework-robocop-4.0.1/robocop/reports/compare_runs_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/reports/file_stats_report.py` & `robotframework-robocop-4.0.1/robocop/reports/file_stats_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/reports/json_report.py` & `robotframework-robocop-4.0.1/robocop/reports/json_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/reports/return_status_report.py` & `robotframework-robocop-4.0.1/robocop/reports/return_status_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/reports/robocop_version_report.py` & `robotframework-robocop-4.0.1/robocop/reports/robocop_version_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/reports/rules_by_id_report.py` & `robotframework-robocop-4.0.1/robocop/reports/rules_by_id_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/reports/rules_by_severity_report.py` & `robotframework-robocop-4.0.1/robocop/reports/rules_by_severity_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/reports/sarif_report.py` & `robotframework-robocop-4.0.1/robocop/reports/sarif_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/reports/time_taken_report.py` & `robotframework-robocop-4.0.1/robocop/reports/time_taken_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/reports/timestamp_report.py` & `robotframework-robocop-4.0.1/robocop/reports/timestamp_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/rules.py` & `robotframework-robocop-4.0.1/robocop/rules.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/run.py` & `robotframework-robocop-4.0.1/robocop/run.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/utils/__init__.py` & `robotframework-robocop-4.0.1/robocop/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/utils/disablers.py` & `robotframework-robocop-4.0.1/robocop/utils/disablers.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/utils/file_types.py` & `robotframework-robocop-4.0.1/robocop/utils/file_types.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/utils/misc.py` & `robotframework-robocop-4.0.1/robocop/utils/misc.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/utils/run_keywords.py` & `robotframework-robocop-4.0.1/robocop/utils/run_keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robocop/utils/version_matching.py` & `robotframework-robocop-4.0.1/robocop/utils/version_matching.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/robotframework_robocop.egg-info/PKG-INFO` & `robotframework-robocop-4.0.1/robotframework_robocop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 4.0.0
+Version: 4.0.1
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
```

### Comparing `robotframework-robocop-4.0.0/robotframework_robocop.egg-info/SOURCES.txt` & `robotframework-robocop-4.0.1/robotframework_robocop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-4.0.0/setup.py` & `robotframework-robocop-4.0.1/setup.py`

 * *Files identical despite different names*


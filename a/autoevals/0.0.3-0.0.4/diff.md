# Comparing `tmp/autoevals-0.0.3.tar.gz` & `tmp/autoevals-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoevals-0.0.3.tar", last modified: Tue Jul 11 21:46:29 2023, max compression
+gzip compressed data, was "autoevals-0.0.4.tar", last modified: Wed Jul 12 04:49:31 2023, max compression
```

## Comparing `autoevals-0.0.3.tar` & `autoevals-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,33 @@
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-11 21:46:29.564885 autoevals-0.0.3/
--rw-r--r--   0 ankur      (501) staff       (20)     1072 2023-07-11 17:08:28.000000 autoevals-0.0.3/LICENSE
--rw-r--r--   0 ankur      (501) staff       (20)     5639 2023-07-11 21:46:29.564764 autoevals-0.0.3/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)     5122 2023-07-11 21:46:08.000000 autoevals-0.0.3/README.md
--rw-r--r--   0 ankur      (501) staff       (20)       31 2023-07-11 06:26:06.000000 autoevals-0.0.3/pyproject.toml
--rw-r--r--   0 ankur      (501) staff       (20)       38 2023-07-11 21:46:29.564921 autoevals-0.0.3/setup.cfg
--rw-r--r--   0 ankur      (501) staff       (20)     1559 2023-07-11 18:47:47.000000 autoevals-0.0.3/setup.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-11 21:46:29.561179 autoevals-0.0.3/src/
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-11 21:46:29.564034 autoevals-0.0.3/src/autoevals/
--rw-r--r--   0 ankur      (501) staff       (20)       61 2023-07-11 06:26:29.000000 autoevals-0.0.3/src/autoevals/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)     1561 2023-07-11 21:00:52.000000 autoevals-0.0.3/src/autoevals/base.py
--rw-r--r--   0 ankur      (501) staff       (20)     6102 2023-07-11 21:05:09.000000 autoevals-0.0.3/src/autoevals/llm.py
--rw-r--r--   0 ankur      (501) staff       (20)      568 2023-07-11 21:01:18.000000 autoevals-0.0.3/src/autoevals/string.py
--rw-r--r--   0 ankur      (501) staff       (20)     4780 2023-07-11 20:58:26.000000 autoevals-0.0.3/src/autoevals/test_llm.py
--rw-r--r--   0 ankur      (501) staff       (20)      546 2023-07-11 20:10:50.000000 autoevals-0.0.3/src/autoevals/test_string.py
--rw-r--r--   0 ankur      (501) staff       (20)      307 2023-07-11 06:26:29.000000 autoevals-0.0.3/src/autoevals/util.py
--rw-r--r--   0 ankur      (501) staff       (20)       18 2023-07-11 21:46:19.000000 autoevals-0.0.3/src/autoevals/version.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-11 21:46:29.564601 autoevals-0.0.3/src/autoevals.egg-info/
--rw-r--r--   0 ankur      (501) staff       (20)     5639 2023-07-11 21:46:29.000000 autoevals-0.0.3/src/autoevals.egg-info/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      420 2023-07-11 21:46:29.000000 autoevals-0.0.3/src/autoevals.egg-info/SOURCES.txt
--rw-r--r--   0 ankur      (501) staff       (20)        1 2023-07-11 21:46:29.000000 autoevals-0.0.3/src/autoevals.egg-info/dependency_links.txt
--rw-r--r--   0 ankur      (501) staff       (20)      268 2023-07-11 21:46:29.000000 autoevals-0.0.3/src/autoevals.egg-info/requires.txt
--rw-r--r--   0 ankur      (501) staff       (20)       10 2023-07-11 21:46:29.000000 autoevals-0.0.3/src/autoevals.egg-info/top_level.txt
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-12 04:49:31.275469 autoevals-0.0.4/
+-rw-r--r--   0 ankur      (501) staff       (20)     1072 2023-07-11 17:08:28.000000 autoevals-0.0.4/LICENSE
+-rw-r--r--   0 ankur      (501) staff       (20)     5639 2023-07-12 04:49:31.275309 autoevals-0.0.4/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)     5122 2023-07-11 21:46:08.000000 autoevals-0.0.4/README.md
+-rw-r--r--   0 ankur      (501) staff       (20)       31 2023-07-11 06:26:06.000000 autoevals-0.0.4/pyproject.toml
+-rw-r--r--   0 ankur      (501) staff       (20)       38 2023-07-12 04:49:31.275510 autoevals-0.0.4/setup.cfg
+-rw-r--r--   0 ankur      (501) staff       (20)     1611 2023-07-12 04:49:11.000000 autoevals-0.0.4/setup.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-12 04:49:31.269596 autoevals-0.0.4/src/
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-12 04:49:31.272539 autoevals-0.0.4/src/autoevals/
+-rw-r--r--   0 ankur      (501) staff       (20)       61 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1561 2023-07-11 21:00:52.000000 autoevals-0.0.4/src/autoevals/base.py
+-rw-r--r--   0 ankur      (501) staff       (20)     6102 2023-07-11 21:05:09.000000 autoevals-0.0.4/src/autoevals/llm.py
+-rw-r--r--   0 ankur      (501) staff       (20)      568 2023-07-11 21:01:18.000000 autoevals-0.0.4/src/autoevals/string.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-12 04:49:31.275056 autoevals-0.0.4/src/autoevals/templates/
+-rw-r--r--   0 ankur      (501) staff       (20)      355 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/battle.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      312 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/closed_q_a.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)     1121 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/factuality.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      107 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/humor.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      636 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/possible.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      109 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/security.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)     1076 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/sql.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      356 2023-07-11 17:44:18.000000 autoevals-0.0.4/src/autoevals/templates/summary.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      683 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/translation.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)     4780 2023-07-11 20:58:26.000000 autoevals-0.0.4/src/autoevals/test_llm.py
+-rw-r--r--   0 ankur      (501) staff       (20)      546 2023-07-11 20:10:50.000000 autoevals-0.0.4/src/autoevals/test_string.py
+-rw-r--r--   0 ankur      (501) staff       (20)      307 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/util.py
+-rw-r--r--   0 ankur      (501) staff       (20)       18 2023-07-12 04:49:20.000000 autoevals-0.0.4/src/autoevals/version.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-12 04:49:31.273150 autoevals-0.0.4/src/autoevals.egg-info/
+-rw-r--r--   0 ankur      (501) staff       (20)     5639 2023-07-12 04:49:31.000000 autoevals-0.0.4/src/autoevals.egg-info/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      758 2023-07-12 04:49:31.000000 autoevals-0.0.4/src/autoevals.egg-info/SOURCES.txt
+-rw-r--r--   0 ankur      (501) staff       (20)        1 2023-07-12 04:49:31.000000 autoevals-0.0.4/src/autoevals.egg-info/dependency_links.txt
+-rw-r--r--   0 ankur      (501) staff       (20)      268 2023-07-12 04:49:31.000000 autoevals-0.0.4/src/autoevals.egg-info/requires.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       10 2023-07-12 04:49:31.000000 autoevals-0.0.4/src/autoevals.egg-info/top_level.txt
```

### Comparing `autoevals-0.0.3/LICENSE` & `autoevals-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.3/PKG-INFO` & `autoevals-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoevals
-Version: 0.0.3
+Version: 0.0.4
 Summary: Universal library for evaluating AI models
 Home-page: https://www.braintrustdata.com
 Author: BrainTrust
 Author-email: info@braintrustdata.com
 Project-URL: Bug Tracker, https://github.com/braintrustdata/autoevals
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `autoevals-0.0.3/README.md` & `autoevals-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.3/setup.py` & `autoevals-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,13 +44,16 @@
         "Bug Tracker": "https://github.com/braintrustdata/autoevals",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
+    package_data={
+        '': ['**/*.yaml']
+    },
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.9.0",
     entry_points={},
     install_requires=install_requires,
     extras_require=extras_require,
 )
```

### Comparing `autoevals-0.0.3/src/autoevals/base.py` & `autoevals-0.0.4/src/autoevals/base.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.3/src/autoevals/llm.py` & `autoevals-0.0.4/src/autoevals/llm.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.3/src/autoevals/string.py` & `autoevals-0.0.4/src/autoevals/string.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.3/src/autoevals/test_llm.py` & `autoevals-0.0.4/src/autoevals/test_llm.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.3/src/autoevals/test_string.py` & `autoevals-0.0.4/src/autoevals/test_string.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.3/src/autoevals.egg-info/PKG-INFO` & `autoevals-0.0.4/src/autoevals.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoevals
-Version: 0.0.3
+Version: 0.0.4
 Summary: Universal library for evaluating AI models
 Home-page: https://www.braintrustdata.com
 Author: BrainTrust
 Author-email: info@braintrustdata.com
 Project-URL: Bug Tracker, https://github.com/braintrustdata/autoevals
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```


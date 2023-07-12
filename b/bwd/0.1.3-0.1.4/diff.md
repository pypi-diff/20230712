# Comparing `tmp/bwd-0.1.3.tar.gz` & `tmp/bwd-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwd-0.1.3.tar", max compression
+gzip compressed data, was "bwd-0.1.4.tar", max compression
```

## Comparing `bwd-0.1.3.tar` & `bwd-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11324 2022-05-16 23:53:33.526725 bwd-0.1.3/LICENSE
--rw-r--r--   0        0        0     3782 2023-07-11 11:09:37.228356 bwd-0.1.3/README.md
--rw-r--r--   0        0        0     1058 2023-07-11 22:41:28.533767 bwd-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      522 2023-07-11 16:15:32.214386 bwd-0.1.3/src/bwd/__init__.py
--rw-r--r--   0        0        0     3904 2023-07-11 16:30:15.723201 bwd-0.1.3/src/bwd/bwd.py
--rw-r--r--   0        0        0     3802 2023-07-11 16:34:33.329397 bwd-0.1.3/src/bwd/bwd_random.py
--rw-r--r--   0        0        0       50 2023-07-11 15:15:49.096589 bwd-0.1.3/src/bwd/exceptions.py
--rw-r--r--   0        0        0     4918 2023-07-11 22:40:32.491803 bwd-0.1.3/src/bwd/multi_bwd.py
--rw-r--r--   0        0        0     1486 2023-07-11 16:16:49.055803 bwd-0.1.3/src/bwd/online.py
--rw-r--r--   0        0        0      898 2023-07-11 22:37:09.227768 bwd-0.1.3/src/bwd/serialization.py
--rw-r--r--   0        0        0     4542 1970-01-01 00:00:00.000000 bwd-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11324 2022-05-16 23:53:33.526725 bwd-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3759 2023-07-12 13:43:00.852399 bwd-0.1.4/README.md
+-rw-r--r--   0        0        0     1057 2023-07-12 13:43:39.254986 bwd-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      522 2023-07-11 16:15:32.214386 bwd-0.1.4/src/bwd/__init__.py
+-rw-r--r--   0        0        0     3904 2023-07-11 16:30:15.723201 bwd-0.1.4/src/bwd/bwd.py
+-rw-r--r--   0        0        0     3802 2023-07-11 16:34:33.329397 bwd-0.1.4/src/bwd/bwd_random.py
+-rw-r--r--   0        0        0       50 2023-07-11 15:15:49.096589 bwd-0.1.4/src/bwd/exceptions.py
+-rw-r--r--   0        0        0     4918 2023-07-11 22:40:32.491803 bwd-0.1.4/src/bwd/multi_bwd.py
+-rw-r--r--   0        0        0     1486 2023-07-11 16:16:49.055803 bwd-0.1.4/src/bwd/online.py
+-rw-r--r--   0        0        0      898 2023-07-11 22:37:09.227768 bwd-0.1.4/src/bwd/serialization.py
+-rw-r--r--   0        0        0     4569 1970-01-01 00:00:00.000000 bwd-0.1.4/PKG-INFO
```

### Comparing `bwd-0.1.3/LICENSE` & `bwd-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bwd-0.1.3/README.md` & `bwd-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 imbalance_bwd = np.array([[0] * d])
 imbalance_rand = np.array([[0] * d])
 
 increment_imbalance = lambda imba, a, x: np.concatenate([imba, imba[-1:, :] + (2 * a - 1) * x])
 
 for x in X:
     # Assign with BWD
-    a_bwd = balancer.assign_next(np.concatenate([[1], x]))
+    a_bwd = balancer.assign_next(x)
     imbalance_bwd = increment_imbalance(imbalance_bwd, a_bwd, x)
     A_bwd.append(a_bwd)
     # Assign with Bernoulli randomization
     a_rand = rng.binomial(n = 1, p = 0.5, size = 1).item()
     imbalance_rand = increment_imbalance(imbalance_rand, a_rand, x)
     A_rand.append(a_rand)
```

### Comparing `bwd-0.1.3/pyproject.toml` & `bwd-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "bwd"
-version = "0.1.3"
+version = "0.1.4"
 description = "A clean implementation of the Balancing Walk Design for online experimental design from Arbour, Dimmery, Mai and Rao (2022)"
 authors = ["Drew Dimmery <drew.dimmery@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://ddimmery.github.io/balancer-package/"
 repository = "https://github.com/ddimmery/balancer-package"
 keywords = ["causal inference", "experimentation", "ab testing"]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
+python = ">=3.9,<4.0"
 numpy = "^1.22.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 black = "^22.3.0"
 jupyter = "^1.0.0"
 mkdocs = "^1.3.0"
```

### Comparing `bwd-0.1.3/src/bwd/__init__.py` & `bwd-0.1.4/src/bwd/__init__.py`

 * *Files identical despite different names*

### Comparing `bwd-0.1.3/src/bwd/bwd.py` & `bwd-0.1.4/src/bwd/bwd.py`

 * *Files identical despite different names*

### Comparing `bwd-0.1.3/src/bwd/bwd_random.py` & `bwd-0.1.4/src/bwd/bwd_random.py`

 * *Files identical despite different names*

### Comparing `bwd-0.1.3/src/bwd/multi_bwd.py` & `bwd-0.1.4/src/bwd/multi_bwd.py`

 * *Files identical despite different names*

### Comparing `bwd-0.1.3/src/bwd/online.py` & `bwd-0.1.4/src/bwd/online.py`

 * *Files identical despite different names*

### Comparing `bwd-0.1.3/src/bwd/serialization.py` & `bwd-0.1.4/src/bwd/serialization.py`

 * *Files identical despite different names*

### Comparing `bwd-0.1.3/PKG-INFO` & `bwd-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: bwd
-Version: 0.1.3
+Version: 0.1.4
 Summary: A clean implementation of the Balancing Walk Design for online experimental design from Arbour, Dimmery, Mai and Rao (2022)
 Home-page: https://ddimmery.github.io/balancer-package/
 License: Apache-2.0
 Keywords: causal inference,experimentation,ab testing
 Author: Drew Dimmery
 Author-email: drew.dimmery@gmail.com
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Project-URL: Repository, https://github.com/ddimmery/balancer-package
 Description-Content-Type: text/markdown
 
 # Balancing Walk Design
 
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)
@@ -62,15 +63,15 @@
 imbalance_bwd = np.array([[0] * d])
 imbalance_rand = np.array([[0] * d])
 
 increment_imbalance = lambda imba, a, x: np.concatenate([imba, imba[-1:, :] + (2 * a - 1) * x])
 
 for x in X:
     # Assign with BWD
-    a_bwd = balancer.assign_next(np.concatenate([[1], x]))
+    a_bwd = balancer.assign_next(x)
     imbalance_bwd = increment_imbalance(imbalance_bwd, a_bwd, x)
     A_bwd.append(a_bwd)
     # Assign with Bernoulli randomization
     a_rand = rng.binomial(n = 1, p = 0.5, size = 1).item()
     imbalance_rand = increment_imbalance(imbalance_rand, a_rand, x)
     A_rand.append(a_rand)
```


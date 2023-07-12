# Comparing `tmp/easylaser-0.1.1.tar.gz` & `tmp/easylaser-0.1.2.tar.gz`

## Comparing `easylaser-0.1.1.tar` & `easylaser-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 easylaser-0.1.1/Distribution.md
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 easylaser-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/__init__.py
--rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/align.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/get_model.py
--rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/laser.py
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/embed/embed.py
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/embed/encoder.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/embed/laserLstmEncoder.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/embed/laserTransformerEncoder.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/embed/multiGpuEncoder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/lib/__init__.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/lib/constants.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/lib/text_processing.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 easylaser-0.1.1/test/fake_data.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 easylaser-0.1.1/test/test_laser.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 easylaser-0.1.1/.gitignore
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 easylaser-0.1.1/LICENSE
--rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 easylaser-0.1.1/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 easylaser-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 easylaser-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 easylaser-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/__init__.py
+-rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/align.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/get_model.py
+-rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/laser.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/embed/embed.py
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/embed/encoder.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/embed/laserLstmEncoder.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/embed/laserTransformerEncoder.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/embed/multiGpuEncoder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/lib/__init__.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/lib/constants.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/lib/text_processing.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 easylaser-0.1.2/test/fake_data.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 easylaser-0.1.2/test/test_laser.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 easylaser-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 easylaser-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 easylaser-0.1.2/README.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 easylaser-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 easylaser-0.1.2/PKG-INFO
```

### Comparing `easylaser-0.1.1/easylaser/align.py` & `easylaser-0.1.2/easylaser/align.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         indices = np.zeros((nbex, 1), dtype=np.int32)
         for i in range(nbex):
             indices[i] = Idx_xy[i, best[i]]
     return indices, scores
 
 
 def get_best_neighbors(lang0_embeddings, lang1_embeddings, scoring_method="ratio"):
-    # cohere embeddings are in float64 but faiss needs float32
+    k = min(len(lang0_embeddings), 4)
     indices, scores = score_knn(
         lang0_embeddings,
         lang1_embeddings,
         4,
         scoring_method,
     )
     return indices.flatten().tolist(), scores.max(axis=1)
```

### Comparing `easylaser-0.1.1/easylaser/get_model.py` & `easylaser-0.1.2/easylaser/get_model.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.1/easylaser/laser.py` & `easylaser-0.1.2/easylaser/laser.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.1/easylaser/embed/embed.py` & `easylaser-0.1.2/easylaser/embed/embed.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.1/easylaser/embed/encoder.py` & `easylaser-0.1.2/easylaser/embed/encoder.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.1/easylaser/embed/laserLstmEncoder.py` & `easylaser-0.1.2/easylaser/embed/laserLstmEncoder.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.1/easylaser/embed/laserTransformerEncoder.py` & `easylaser-0.1.2/easylaser/embed/laserTransformerEncoder.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.1/easylaser/embed/multiGpuEncoder.py` & `easylaser-0.1.2/easylaser/embed/multiGpuEncoder.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.1/easylaser/lib/constants.py` & `easylaser-0.1.2/easylaser/lib/constants.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.1/easylaser/lib/text_processing.py` & `easylaser-0.1.2/easylaser/lib/text_processing.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.1/test/fake_data.py` & `easylaser-0.1.2/test/fake_data.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.1/test/test_laser.py` & `easylaser-0.1.2/test/test_laser.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.1/LICENSE` & `easylaser-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.1/README.md` & `easylaser-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.1/pyproject.toml` & `easylaser-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "easylaser"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Lingua Custodia", email="it@linguacustodia.com" },
 ]
 description = "An easy to use interface to LASER"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `easylaser-0.1.1/PKG-INFO` & `easylaser-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easylaser
-Version: 0.1.1
+Version: 0.1.2
 Summary: An easy to use interface to LASER
 Author-email: Lingua Custodia <it@linguacustodia.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```


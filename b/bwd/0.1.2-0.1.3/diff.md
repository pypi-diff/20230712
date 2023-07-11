# Comparing `tmp/bwd-0.1.2.tar.gz` & `tmp/bwd-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwd-0.1.2.tar", max compression
+gzip compressed data, was "bwd-0.1.3.tar", max compression
```

## Comparing `bwd-0.1.2.tar` & `bwd-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0    11324 2022-05-16 23:53:33.526725 bwd-0.1.2/LICENSE
--rw-r--r--   0        0        0     3782 2023-07-11 11:09:37.228356 bwd-0.1.2/README.md
--rw-r--r--   0        0        0     1058 2023-07-11 11:08:55.903459 bwd-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      495 2022-05-17 20:40:56.204982 bwd-0.1.2/src/bwd/__init__.py
--rw-r--r--   0        0        0     4204 2023-07-10 21:49:37.009554 bwd-0.1.2/src/bwd/bwd.py
--rw-r--r--   0        0        0     4107 2023-07-10 21:48:49.286458 bwd-0.1.2/src/bwd/bwd_random.py
--rw-r--r--   0        0        0     4745 2023-07-10 21:51:11.360429 bwd-0.1.2/src/bwd/multi_bwd.py
--rw-r--r--   0        0        0     4542 1970-01-01 00:00:00.000000 bwd-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11324 2022-05-16 23:53:33.526725 bwd-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3782 2023-07-11 11:09:37.228356 bwd-0.1.3/README.md
+-rw-r--r--   0        0        0     1058 2023-07-11 22:41:28.533767 bwd-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      522 2023-07-11 16:15:32.214386 bwd-0.1.3/src/bwd/__init__.py
+-rw-r--r--   0        0        0     3904 2023-07-11 16:30:15.723201 bwd-0.1.3/src/bwd/bwd.py
+-rw-r--r--   0        0        0     3802 2023-07-11 16:34:33.329397 bwd-0.1.3/src/bwd/bwd_random.py
+-rw-r--r--   0        0        0       50 2023-07-11 15:15:49.096589 bwd-0.1.3/src/bwd/exceptions.py
+-rw-r--r--   0        0        0     4918 2023-07-11 22:40:32.491803 bwd-0.1.3/src/bwd/multi_bwd.py
+-rw-r--r--   0        0        0     1486 2023-07-11 16:16:49.055803 bwd-0.1.3/src/bwd/online.py
+-rw-r--r--   0        0        0      898 2023-07-11 22:37:09.227768 bwd-0.1.3/src/bwd/serialization.py
+-rw-r--r--   0        0        0     4542 1970-01-01 00:00:00.000000 bwd-0.1.3/PKG-INFO
```

### Comparing `bwd-0.1.2/LICENSE` & `bwd-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bwd-0.1.2/README.md` & `bwd-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bwd-0.1.2/pyproject.toml` & `bwd-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bwd"
-version = "0.1.2"
+version = "0.1.3"
 description = "A clean implementation of the Balancing Walk Design for online experimental design from Arbour, Dimmery, Mai and Rao (2022)"
 authors = ["Drew Dimmery <drew.dimmery@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://ddimmery.github.io/balancer-package/"
 repository = "https://github.com/ddimmery/balancer-package"
 keywords = ["causal inference", "experimentation", "ab testing"]
```

### Comparing `bwd-0.1.2/src/bwd/bwd.py` & `bwd-0.1.3/src/bwd/bwd.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,14 +58,16 @@
 
     def assign_next(self, x: np.ndarray) -> np.ndarray:
         """Assign treatment to the next point
 
         Args:
             x: covariate profile of unit to assign treatment
         """
+        if self.intercept:
+            x = np.concatenate(([1], x))
         dot = x @ self.w_i
         if abs(dot) > self.alpha:
             self.w_i = np.zeros((self.D,))
             self.set_alpha(self.N - self.iterations)
             dot = x @ self.w_i
 
         p_i = self.q * (1 - self.phi * dot / self.alpha)
@@ -86,37 +88,24 @@
         This assigns units to treatment in the offline setting in which all covariate
         profiles are available prior to assignment. The algorithm assigns as if units
         were still only observed in a stream.
 
         Args:
             X: array of size n × d of covariate profiles
         """
-        if self.intercept:
-            X = np.hstack((X, np.ones((X.shape[0], 1))))
         return np.array([self.assign_next(X[i, :]) for i in range(X.shape[0])])
+    
+    @property
+    def definition(self):
+        return {
+            "N": self.N, "D": self.D, "delta": self.delta, "q": self.q,
+            "intercept": self.intercept, "phi": self.phi
+        }
+    
+    @property
+    def state(self):
+        return {"w_i": self.w_i, "iterations": self.iterations}
+    
+    def update_state(self, w_i, iterations):
+        self.w_i = np.array(w_i)
+        self.iterations = iterations
 
-    def serialize(self):
-        attribs = {}
-        for a in SERIALIZED_ATTRIBUTES:
-            attribs[a] = getattr(self, a)
-        return json.dumps(attribs)
-
-    def to_json(self):
-        return self.serialize()
-
-    @classmethod
-    def deserialize(cls, str):
-        x = json.loads(str)
-        if not isinstance(x, dict):
-            raise ValueError("The deserialized object is not a dictionary.")
-
-        pars = {}
-        state = {}
-        for k in SERIALIZED_ATTRIBUTES:
-            if k in x.keys():
-                pars[k] = x[k]
-            else:
-                state[k] = x[k]
-        obj = cls(**pars)
-        for k, v in state.items():
-            setattr(obj, k, v)
-        return obj
```

### Comparing `bwd-0.1.2/src/bwd/bwd_random.py` & `bwd-0.1.3/src/bwd/bwd_random.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 
     def assign_next(self, x: np.ndarray) -> np.ndarray:
         """Assign treatment to the next point
 
         Args:
             x: covariate profile of unit to assign treatment
         """
+        if self.intercept:
+            x = np.concatenate(([1], x))
         dot = x @ self.w_i
         if abs(dot) > self.alpha:
             self.w_i = np.zeros((self.D,))
             self.set_alpha(self.N - self.iterations)
             dot = 0.0
 
         p_i = self.q * (1 - self.phi * dot / self.alpha)
@@ -85,37 +87,23 @@
         This assigns units to treatment in the offline setting in which all covariate
         profiles are available prior to assignment. The algorithm assigns as if units
         were still only observed in a stream.
 
         Args:
             X: array of size n × d of covariate profiles
         """
-        if self.intercept:
-            X = np.hstack((X, np.ones((X.shape[0], 1))))
         return np.array([self.assign_next(X[i, :]) for i in range(X.shape[0])])
 
-    def serialize(self):
-        attribs = {}
-        for a in SERIALIZED_ATTRIBUTES:
-            attribs[a] = getattr(self, a)
-        return json.dumps(attribs)
-
-    def to_json(self):
-        return self.serialize()
-
-    @classmethod
-    def deserialize(cls, str):
-        x = json.loads(str)
-        if not isinstance(x, dict):
-            raise ValueError("The deserialized object is not a dictionary.")
-
-        pars = {}
-        state = {}
-        for k in SERIALIZED_ATTRIBUTES:
-            if k in x.keys():
-                pars[k] = x[k]
-            else:
-                state[k] = x[k]
-        obj = cls(**pars)
-        for k, v in state.items():
-            setattr(obj, k, v)
-        return obj
+    @property
+    def definition(self):
+        return {
+            "N": self.N, "D": self.D, "delta": self.delta, "q": self.q,
+            "intercept": self.intercept, "phi": self.phi
+        }
+    
+    @property
+    def state(self):
+        return {"w_i": self.w_i, "iterations": self.iterations}
+    
+    def update_state(self, w_i, iterations):
+        self.w_i = np.array(w_i)
+        self.iterations = iterations
```

### Comparing `bwd-0.1.2/src/bwd/multi_bwd.py` & `bwd-0.1.3/src/bwd/multi_bwd.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,14 +30,20 @@
             D: dimension of the data
             delta: probability of failure
             q: Target marginal probability of treatment
             intercept: Whether an intercept term be added to covariate profiles
             phi: Robustness parameter. A value of 1 focuses entirely on balance, while a value
                 approaching zero does pure randomization.
         """
+        self.N = N
+        self.D = D
+        self.delta = delta
+        self.intercept = intercept
+        self.phi = phi
+
         if isinstance(q, float):
             q = q if q < 0.5 else 1 - q
             self.qs = [1 - q, q]
             self.classes = [0, 1]
         elif isinstance(q, Iterable):
             self.qs = [pr / sum(q) for pr in q]
             self.classes = [i for i, q in enumerate(self.qs)]
@@ -104,20 +110,23 @@
         This assigns units to treatment in the offline setting in which all covariate
         profiles are available prior to assignment. The algorithm assigns as if units
         were still only observed in a stream.
 
         Args:
             X: array of size n × d of covariate profiles
         """
-        if self.intercept:
-            X = np.hstack((X, np.ones((X.shape[0], 1))))
         return np.array([self.assign_next(X[i, :]) for i in range(X.shape[0])])
     
-    def serialize(self):
-        raise NotImplementedError("Serialization is not yet implemented for MultiBWD.")
-
-    def to_json(self):
-        raise NotImplementedError("Serialization is not yet implemented for MultiBWD.")
-
-    @classmethod
-    def deserialize(cls, str):
-        raise NotImplementedError("Serialization is not yet implemented for MultiBWD.")
+    @property
+    def definition(self):
+        return {
+            "N": self.N, "D": self.D, "delta": self.delta, "q": self.qs,
+            "intercept": self.intercept, "phi": self.phi
+        }
+    
+    @property
+    def state(self):
+        return {idx: node.state for idx, node in enumerate(self.nodes) if isinstance(node, BWD)}
+    
+    def update_state(self, **node_state_dict):
+        for node, state in node_state_dict.items():
+            self.nodes[int(node)].update_state(**state)
```

### Comparing `bwd-0.1.2/PKG-INFO` & `bwd-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwd
-Version: 0.1.2
+Version: 0.1.3
 Summary: A clean implementation of the Balancing Walk Design for online experimental design from Arbour, Dimmery, Mai and Rao (2022)
 Home-page: https://ddimmery.github.io/balancer-package/
 License: Apache-2.0
 Keywords: causal inference,experimentation,ab testing
 Author: Drew Dimmery
 Author-email: drew.dimmery@gmail.com
 Requires-Python: >=3.9,<3.11
```


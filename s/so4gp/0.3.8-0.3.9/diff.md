# Comparing `tmp/so4gp-0.3.8.tar.gz` & `tmp/so4gp-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so4gp-0.3.8.tar", last modified: Thu Oct 27 09:13:56 2022, max compression
+gzip compressed data, was "so4gp-0.3.9.tar", last modified: Wed Jul 12 15:06:13 2023, max compression
```

## Comparing `so4gp-0.3.8.tar` & `so4gp-0.3.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 owuorjnr   (501) staff       (20)        0 2022-10-27 09:13:56.228195 so4gp-0.3.8/
--rw-r--r--   0 owuorjnr   (501) staff       (20)     1078 2022-03-01 09:38:23.000000 so4gp-0.3.8/LICENSE
--rw-r--r--   0 owuorjnr   (501) staff       (20)    10724 2022-10-27 09:13:56.228530 so4gp-0.3.8/PKG-INFO
--rw-r--r--   0 owuorjnr   (501) staff       (20)     9784 2022-10-14 11:47:54.000000 so4gp-0.3.8/README.md
--rw-r--r--   0 owuorjnr   (501) staff       (20)      133 2022-03-01 09:38:23.000000 so4gp-0.3.8/pyproject.toml
--rw-r--r--   0 owuorjnr   (501) staff       (20)     1116 2022-10-27 09:13:56.229864 so4gp-0.3.8/setup.cfg
-drwxr-xr-x   0 owuorjnr   (501) staff       (20)        0 2022-10-27 09:13:56.206000 so4gp-0.3.8/src/
-drwxr-xr-x   0 owuorjnr   (501) staff       (20)        0 2022-10-27 09:13:56.215172 so4gp-0.3.8/src/so4gp/
--rw-r--r--   0 owuorjnr   (501) staff       (20)      504 2022-10-19 17:57:50.000000 so4gp-0.3.8/src/so4gp/__init__.py
--rw-r--r--   0 owuorjnr   (501) staff       (20)   119213 2022-10-27 08:59:24.000000 so4gp-0.3.8/src/so4gp/so4gp.py
-drwxr-xr-x   0 owuorjnr   (501) staff       (20)        0 2022-10-27 09:13:56.226930 so4gp-0.3.8/src/so4gp.egg-info/
--rw-r--r--   0 owuorjnr   (501) staff       (20)    10724 2022-10-27 09:13:56.000000 so4gp-0.3.8/src/so4gp.egg-info/PKG-INFO
--rw-r--r--   0 owuorjnr   (501) staff       (20)      247 2022-10-27 09:13:56.000000 so4gp-0.3.8/src/so4gp.egg-info/SOURCES.txt
--rw-r--r--   0 owuorjnr   (501) staff       (20)        1 2022-10-27 09:13:56.000000 so4gp-0.3.8/src/so4gp.egg-info/dependency_links.txt
--rw-r--r--   0 owuorjnr   (501) staff       (20)       67 2022-10-27 09:13:56.000000 so4gp-0.3.8/src/so4gp.egg-info/requires.txt
--rw-r--r--   0 owuorjnr   (501) staff       (20)        6 2022-10-27 09:13:56.000000 so4gp-0.3.8/src/so4gp.egg-info/top_level.txt
+drwxr-xr-x   0 owuorjnr   (501) staff       (20)        0 2023-07-12 15:06:13.512179 so4gp-0.3.9/
+-rw-r--r--   0 owuorjnr   (501) staff       (20)     1078 2022-03-01 09:38:23.000000 so4gp-0.3.9/LICENSE
+-rw-r--r--   0 owuorjnr   (501) staff       (20)    10724 2023-07-12 15:06:13.512538 so4gp-0.3.9/PKG-INFO
+-rw-r--r--   0 owuorjnr   (501) staff       (20)     9784 2022-10-14 11:47:54.000000 so4gp-0.3.9/README.md
+-rw-r--r--   0 owuorjnr   (501) staff       (20)      133 2022-03-01 09:38:23.000000 so4gp-0.3.9/pyproject.toml
+-rw-r--r--   0 owuorjnr   (501) staff       (20)     1116 2023-07-12 15:06:13.513748 so4gp-0.3.9/setup.cfg
+drwxr-xr-x   0 owuorjnr   (501) staff       (20)        0 2023-07-12 15:06:13.493185 so4gp-0.3.9/src/
+drwxr-xr-x   0 owuorjnr   (501) staff       (20)        0 2023-07-12 15:06:13.501299 so4gp-0.3.9/src/so4gp/
+-rw-r--r--   0 owuorjnr   (501) staff       (20)      504 2022-10-19 17:57:50.000000 so4gp-0.3.9/src/so4gp/__init__.py
+-rw-r--r--   0 owuorjnr   (501) staff       (20)   119233 2023-07-12 14:23:55.000000 so4gp-0.3.9/src/so4gp/so4gp.py
+drwxr-xr-x   0 owuorjnr   (501) staff       (20)        0 2023-07-12 15:06:13.511203 so4gp-0.3.9/src/so4gp.egg-info/
+-rw-r--r--   0 owuorjnr   (501) staff       (20)    10724 2023-07-12 15:06:13.000000 so4gp-0.3.9/src/so4gp.egg-info/PKG-INFO
+-rw-r--r--   0 owuorjnr   (501) staff       (20)      247 2023-07-12 15:06:13.000000 so4gp-0.3.9/src/so4gp.egg-info/SOURCES.txt
+-rw-r--r--   0 owuorjnr   (501) staff       (20)        1 2023-07-12 15:06:13.000000 so4gp-0.3.9/src/so4gp.egg-info/dependency_links.txt
+-rw-r--r--   0 owuorjnr   (501) staff       (20)       67 2023-07-12 15:06:13.000000 so4gp-0.3.9/src/so4gp.egg-info/requires.txt
+-rw-r--r--   0 owuorjnr   (501) staff       (20)        6 2023-07-12 15:06:13.000000 so4gp-0.3.9/src/so4gp.egg-info/top_level.txt
```

### Comparing `so4gp-0.3.8/LICENSE` & `so4gp-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `so4gp-0.3.8/PKG-INFO` & `so4gp-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so4gp
-Version: 0.3.8
+Version: 0.3.9
 Summary: Some optimization algorithms for mining gradual patterns.
 Home-page: https://github.com/owuordickson/sogp_pypi
 Author: Dickson Owuor
 Author-email: owuordickson@ieee.org
 License: MIT
 Project-URL: Documentation, http://sogp-pypi.readthedocs.io/
 Project-URL: Tracker, https://github.com/owuordickson/sogp_pypi/issues
```

### Comparing `so4gp-0.3.8/README.md` & `so4gp-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `so4gp-0.3.8/setup.cfg` & `so4gp-0.3.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = so4gp
-version = 0.3.8
+version = 0.3.9
 author = Dickson Owuor
 author_email = owuordickson@ieee.org
 description = Some optimization algorithms for mining gradual patterns.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/owuordickson/sogp_pypi
 project_urls =
```

### Comparing `so4gp-0.3.8/src/so4gp/so4gp.py` & `so4gp-0.3.9/src/so4gp/so4gp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1255,14 +1255,17 @@
     The class NumericSS has the following functions:
         decode_gp: decodes a GP from a numeric position
         cost_function: computes the fitness of a GP
         apply_bound: applies minimum and maximum values
 
     """
 
+    def __init__(self):
+        pass
+
     @staticmethod
     def decode_gp(attr_keys, position):
         """Description
 
         Decodes a numeric value (position) into a GP
 
         :param attr_keys: list of attribute keys
@@ -1737,21 +1740,20 @@
             """:type gradual_items: np.ndarray"""
             """:type cum_wins: np.ndarray"""
             """:type net_win_mat: np.ndarray"""
             """:type ij: np.ndarray"""
             self.win_mat = np.array([])
             """:type win_mat: np.ndarray"""
         else:
-            self.gradual_items, self.win_mat, self.cum_wins, self.net_win_mat, self.nodes_mat, self.ij = \
-                self._construct_all_matrices()
+            self.gradual_items, self.win_mat, self.cum_wins, self.net_win_mat, self.ij = self._construct_all_matrices()
             """:type gradual_items: np.ndarray"""
             """:type win_mat: np.ndarray"""
             """:type cum_wins: np.ndarray"""
             """:type net_win_mat: np.ndarray"""
-            """:type nodes_mat: np.ndarray"""
+            # """:type nodes_mat: np.ndarray"""
             """:type ij: np.ndarray"""
 
     def _construct_matrices(self, e):
         """Description
 
         Generates all the gradual items and, constructs: (1) net-win matrix, (2) cumulative wins, (3) pairwise objects.
 
@@ -1840,35 +1842,36 @@
 
         # 2. Variable declarations
         attr_data = self.data.T  # Feature data objects
         lst_gis = []  # List of GIs
         s_mat = []  # S-Matrix (made up of S-Vectors)
         w_mat = []  # win matrix
         cum_wins = []  # Cumulative wins
-        nodes_mat = []  # FP nodes matrix
+        # nodes_mat = []  # FP nodes matrix
 
         # 3. Construct S matrix from data set
         for col in np.nditer(self.attr_cols):
             # Feature data objects
             col_data = np.array(attr_data[col], dtype=np.float)  # Feature data objects
 
             # Cumulative Wins: for estimation of score-vector
             temp_cum_wins = np.where(col_data[pair_ij[:, 0]] < col_data[pair_ij[:, 1]], 1,
                                      np.where(col_data[pair_ij[:, 0]] > col_data[pair_ij[:, 1]], -1, 0))
 
             # S-vector
             s_vec = np.zeros((n,), dtype=np.int32)
-            nodes_vec = [[set(), set()]] * n
+            # nodes_vec = [[set(), set()]] * n
             for w in [1, -1]:
                 positions = np.flatnonzero(temp_cum_wins == w)
                 i, counts_i = np.unique(pair_ij[positions, 0], return_counts=True)
                 j, counts_j = np.unique(pair_ij[positions, 1], return_counts=True)
                 s_vec[i] += w * counts_i  # i wins/loses (1/-1)
                 s_vec[j] += -w * counts_j  # j loses/wins (1/-1)
 
+                """
                 if w == 1:
                     for node_i in i:
                         nodes_j = j[np.where(j > node_i)]
                         tmp = nodes_vec[node_i][0].union(set(nodes_j))
                         nodes_vec[node_i] = [tmp, nodes_vec[node_i][1]]
 
                     for node_j in j:
@@ -1884,34 +1887,34 @@
                     for node_j in j:
                         nodes_i = i[np.where(i < node_j)]
                         tmp = nodes_vec[node_j][0].union(set(nodes_i))
                         nodes_vec[node_j] = [tmp, nodes_vec[node_j][1]]
 
             # print('positions: ' + str(positions) + '; i: ' + str(i) + '; j: ' + str(j) + '; counts: ' + str(counts_i))
             #    print(nodes_vec)
-            # print("\n")
+            # print("\n")"""
 
             # Normalize S-vector
             if np.count_nonzero(s_vec) > 0:
                 w_mat.append(np.copy(s_vec))
-                nodes_mat.append(nodes_vec)
+                # nodes_mat.append(nodes_vec)
 
                 s_vec[s_vec > 0] = 1  # Normalize net wins
                 s_vec[s_vec < 0] = -1  # Normalize net loses
 
                 lst_gis.append(GI(col, '+'))
                 cum_wins.append(temp_cum_wins)
                 s_mat.append(s_vec)
 
                 lst_gis.append(GI(col, '-'))
                 cum_wins.append(-temp_cum_wins)
                 s_mat.append(-s_vec)
 
         # print(np.array(nodes_mat))
-        return np.array(lst_gis), np.array(w_mat), np.array(cum_wins), np.array(s_mat), np.array(nodes_mat), pair_ij
+        return np.array(lst_gis), np.array(w_mat), np.array(cum_wins), np.array(s_mat), pair_ij
 
     def _infer_gps(self, clusters):
         """Description
 
         A function that infers GPs from clusters of gradual items.
 
         :param clusters: [required] groups of gradual items clustered through K-MEANS algorithm
@@ -1969,15 +1972,15 @@
         arr_ij = self.ij
 
         # Construct a win-matrix
         temp_vec = np.zeros(shape=(n,))
         pair_count = arr_ij.shape[0]
 
         # Compute score vector
-        for k in range(self.max_iteration):
+        for _ in range(self.max_iteration):
             if np.count_nonzero(score_vector == 0) > 1:
                 break
             else:
                 for pr in range(pair_count):
                     pr_val = c_wins[pr]
                     i = arr_ij[pr][0]
                     j = arr_ij[pr][1]
@@ -2499,16 +2502,16 @@
                     z = 0
                     while z < (len(self.gradual_patterns) - 1):
                         if set(self.gradual_patterns[z].get_pattern()).issubset(set(gi_tuple)):
                             del self.gradual_patterns[z]
                         else:
                             z = z + 1
 
-                    gp = GP()
-                    """:type gp: GP"""
+                    gp = ExtGP()
+                    """:type gp: ExtGP"""
                     for obj in valid_bins[i][0]:
                         gi = GI(obj[0], obj[1].decode())
                         """:type gi: GI"""
                         gp.add_gradual_item(gi)
                     gp.set_support(sup)
                     self.gradual_patterns.append(gp)
                     str_winner_gps.append(gp.print(self.titles))
```

### Comparing `so4gp-0.3.8/src/so4gp.egg-info/PKG-INFO` & `so4gp-0.3.9/src/so4gp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so4gp
-Version: 0.3.8
+Version: 0.3.9
 Summary: Some optimization algorithms for mining gradual patterns.
 Home-page: https://github.com/owuordickson/sogp_pypi
 Author: Dickson Owuor
 Author-email: owuordickson@ieee.org
 License: MIT
 Project-URL: Documentation, http://sogp-pypi.readthedocs.io/
 Project-URL: Tracker, https://github.com/owuordickson/sogp_pypi/issues
```


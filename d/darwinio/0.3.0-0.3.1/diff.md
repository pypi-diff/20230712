# Comparing `tmp/darwinio-0.3.0.tar.gz` & `tmp/darwinio-0.3.1.tar.gz`

## Comparing `darwinio-0.3.0.tar` & `darwinio-0.3.1.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rwxr-xr-x   0        0        0     1873 2020-02-02 00:00:00.000000 darwinio-0.3.0/CONTRIBUTING.md
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 darwinio-0.3.0/requirements.txt
--rwxr-xr-x   0        0        0      562 2020-02-02 00:00:00.000000 darwinio-0.3.0/todo.org
--rwxr-xr-x   0        0        0     5915 2020-02-02 00:00:00.000000 darwinio-0.3.0/documentation/characteristics.ods
--rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 darwinio-0.3.0/documentation/doc.md
--rwxr-xr-x   0        0        0    86371 2020-02-02 00:00:00.000000 darwinio-0.3.0/documentation/doc.pdf
--rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 darwinio-0.3.0/documentation/earlystages.md
--rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 darwinio-0.3.0/documentation/implementation.md
--rwxr-xr-x   0        0        0     3062 2020-02-02 00:00:00.000000 darwinio-0.3.0/documentation/graphical_interface/empty_window.png
--rwxr-xr-x   0        0        0    11317 2020-02-02 00:00:00.000000 darwinio-0.3.0/documentation/graphical_interface/main_game.png
--rwxr-xr-x   0        0        0     7816 2020-02-02 00:00:00.000000 darwinio-0.3.0/documentation/graphical_interface/starting_window.png
--rwxr-xr-x   0        0        0    71751 2020-02-02 00:00:00.000000 darwinio-0.3.0/documentation/screenshot/main_game_play.png
--rwxr-xr-x   0        0        0    23470 2020-02-02 00:00:00.000000 darwinio-0.3.0/documentation/screenshot/titlescreen.png
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/__init__.py
--rwxr-xr-x   0        0        0     3879 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/__main__.py
--rwxr-xr-x   0        0        0     5467 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/brain.py
--rwxr-xr-x   0        0        0     2438 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/constants.py
--rwxr-xr-x   0        0        0    16167 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/distribution.py
--rwxr-xr-x   0        0        0     2728 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/genome.py
--rwxr-xr-x   0        0        0    20286 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/graphical_sim.py
--rwxr-xr-x   0        0        0     3645 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/organism.py
--rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/text_sim.py
--rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/archaebacteria_halophile.png
--rwxr-xr-x   0        0        0     3805 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/archaebacteria_methanogen.png
--rwxr-xr-x   0        0        0     3712 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/archaebacteria_thermoacidophile.png
--rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/eubacteria_BGA.png
--rwxr-xr-x   0        0        0     4533 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/eubacteria_mycoplasma.png
--rwxr-xr-x   0        0        0     5241 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/eubacteroa_chemosynthetic.png
--rwxr-xr-x   0        0        0     4269 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/fungi-ascomycetes.png
--rwxr-xr-x   0        0        0     4427 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/fungi-basidiomycetes.png
--rwxr-xr-x   0        0        0     3117 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/fungi-deuteromycetes.png
--rwxr-xr-x   0        0        0    11139 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/fungi-phycomycetes.png
--rwxr-xr-x   0        0        0     4609 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/metaphyta-algae.png
--rwxr-xr-x   0        0        0     6760 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/metaphyta-angiospermae.png
--rwxr-xr-x   0        0        0     4285 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/metaphyta-bryophyta.png
--rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/metaphyta-gymnospermae.png
--rwxr-xr-x   0        0        0     3474 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/metaphyta-pterdiophyta.png
--rwxr-xr-x   0        0        0     4270 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/protista_dinoflagellate.png
--rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/protista_euglena.png
--rwxr-xr-x   0        0        0     3734 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/protista_protozoan.png
--rwxr-xr-x   0        0        0     6104 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/protista_slimemould.png
--rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/art/theme.json
--rwxr-xr-x   0        0        0  4128852 2020-02-02 00:00:00.000000 darwinio-0.3.0/src/darwinio/assets/audio/Darwinio.mp3
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 darwinio-0.3.0/.gitignore
--rwxr-xr-x   0        0        0    34915 2020-02-02 00:00:00.000000 darwinio-0.3.0/LICENSE.md
--rwxr-xr-x   0        0        0     2497 2020-02-02 00:00:00.000000 darwinio-0.3.0/README.md
--rwxr-xr-x   0        0        0      853 2020-02-02 00:00:00.000000 darwinio-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 darwinio-0.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1873 2020-02-02 00:00:00.000000 darwinio-0.3.1/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0   441990 2020-02-02 00:00:00.000000 darwinio-0.3.1/keke
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 darwinio-0.3.1/requirements.txt
+-rwxr-xr-x   0        0        0      562 2020-02-02 00:00:00.000000 darwinio-0.3.1/todo.org
+-rwxr-xr-x   0        0        0     5915 2020-02-02 00:00:00.000000 darwinio-0.3.1/documentation/characteristics.ods
+-rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 darwinio-0.3.1/documentation/doc.md
+-rwxr-xr-x   0        0        0    86371 2020-02-02 00:00:00.000000 darwinio-0.3.1/documentation/doc.pdf
+-rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 darwinio-0.3.1/documentation/earlystages.md
+-rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 darwinio-0.3.1/documentation/implementation.md
+-rwxr-xr-x   0        0        0     3062 2020-02-02 00:00:00.000000 darwinio-0.3.1/documentation/graphical_interface/empty_window.png
+-rwxr-xr-x   0        0        0    11317 2020-02-02 00:00:00.000000 darwinio-0.3.1/documentation/graphical_interface/main_game.png
+-rwxr-xr-x   0        0        0     7816 2020-02-02 00:00:00.000000 darwinio-0.3.1/documentation/graphical_interface/starting_window.png
+-rwxr-xr-x   0        0        0    71751 2020-02-02 00:00:00.000000 darwinio-0.3.1/documentation/screenshot/main_game_play.png
+-rwxr-xr-x   0        0        0    23470 2020-02-02 00:00:00.000000 darwinio-0.3.1/documentation/screenshot/titlescreen.png
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/__init__.py
+-rwxr-xr-x   0        0        0     3879 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/__main__.py
+-rwxr-xr-x   0        0        0     5460 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/brain.py
+-rwxr-xr-x   0        0        0     2438 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/constants.py
+-rwxr-xr-x   0        0        0    15208 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/distribution.py
+-rwxr-xr-x   0        0        0     2728 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/genome.py
+-rwxr-xr-x   0        0        0    20286 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/graphical_sim.py
+-rwxr-xr-x   0        0        0     3645 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/organism.py
+-rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/text_sim.py
+-rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/archaebacteria_halophile.png
+-rwxr-xr-x   0        0        0     3805 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/archaebacteria_methanogen.png
+-rwxr-xr-x   0        0        0     3712 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/archaebacteria_thermoacidophile.png
+-rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/eubacteria_BGA.png
+-rwxr-xr-x   0        0        0     4533 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/eubacteria_mycoplasma.png
+-rwxr-xr-x   0        0        0     5241 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/eubacteroa_chemosynthetic.png
+-rwxr-xr-x   0        0        0     4269 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/fungi-ascomycetes.png
+-rwxr-xr-x   0        0        0     4427 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/fungi-basidiomycetes.png
+-rwxr-xr-x   0        0        0     3117 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/fungi-deuteromycetes.png
+-rwxr-xr-x   0        0        0    11139 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/fungi-phycomycetes.png
+-rwxr-xr-x   0        0        0     4609 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/metaphyta-algae.png
+-rwxr-xr-x   0        0        0     6760 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/metaphyta-angiospermae.png
+-rwxr-xr-x   0        0        0     4285 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/metaphyta-bryophyta.png
+-rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/metaphyta-gymnospermae.png
+-rwxr-xr-x   0        0        0     3474 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/metaphyta-pterdiophyta.png
+-rwxr-xr-x   0        0        0     4270 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/protista_dinoflagellate.png
+-rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/protista_euglena.png
+-rwxr-xr-x   0        0        0     3734 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/protista_protozoan.png
+-rwxr-xr-x   0        0        0     6104 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/protista_slimemould.png
+-rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/art/theme.json
+-rwxr-xr-x   0        0        0  4128852 2020-02-02 00:00:00.000000 darwinio-0.3.1/src/darwinio/assets/audio/Darwinio.mp3
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 darwinio-0.3.1/.gitignore
+-rwxr-xr-x   0        0        0    34915 2020-02-02 00:00:00.000000 darwinio-0.3.1/LICENSE.md
+-rwxr-xr-x   0        0        0     2497 2020-02-02 00:00:00.000000 darwinio-0.3.1/README.md
+-rwxr-xr-x   0        0        0      853 2020-02-02 00:00:00.000000 darwinio-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 darwinio-0.3.1/PKG-INFO
```

### Comparing `darwinio-0.3.0/CONTRIBUTING.md` & `darwinio-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/todo.org` & `darwinio-0.3.1/todo.org`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/documentation/characteristics.ods` & `darwinio-0.3.1/documentation/characteristics.ods`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/documentation/doc.md` & `darwinio-0.3.1/documentation/doc.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/documentation/doc.pdf` & `darwinio-0.3.1/documentation/doc.pdf`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/documentation/earlystages.md` & `darwinio-0.3.1/documentation/earlystages.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/documentation/implementation.md` & `darwinio-0.3.1/documentation/implementation.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/documentation/graphical_interface/empty_window.png` & `darwinio-0.3.1/documentation/graphical_interface/empty_window.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/documentation/graphical_interface/main_game.png` & `darwinio-0.3.1/documentation/graphical_interface/main_game.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/documentation/graphical_interface/starting_window.png` & `darwinio-0.3.1/documentation/graphical_interface/starting_window.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/documentation/screenshot/main_game_play.png` & `darwinio-0.3.1/documentation/screenshot/main_game_play.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/documentation/screenshot/titlescreen.png` & `darwinio-0.3.1/documentation/screenshot/titlescreen.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/__main__.py` & `darwinio-0.3.1/src/darwinio/__main__.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/brain.py` & `darwinio-0.3.1/src/darwinio/brain.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,16 +124,16 @@
             neural_network[next_layer_index] = list(next_layer_values)
 
         return np.array(neural_network[-1])
 
 
 def normalize(arr: np.ndarray) -> np.ndarray:
     """Normalize the Numpy Array."""
-    magnitude: np.floating = np.linalg.norm(arr)
-    return np.nan_to_num(arr / magnitude)
+    magnitude: np.floating = np.linalg.norm(arr) + 1e-16
+    return arr / magnitude
 
 
 def create_weights(
     genome_array: np.ndarray, neural_structure: np.ndarray
 ) -> np.ndarray:
     """Creates the weights for the neural network based on the genome and
     neural structure.
```

### Comparing `darwinio-0.3.0/src/darwinio/constants.py` & `darwinio-0.3.1/src/darwinio/constants.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/distribution.py` & `darwinio-0.3.1/src/darwinio/distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -428,50 +428,31 @@
     -----
     np.ndarray: An array of coordinates of the points that lie on the line
     between the two given points.(inclusive of point1 and point2)
 
     Note:
     -----
     The function calculates the coordinates of the points that lie on the line
-    between the two input points, and returns an array of these coordinates.
-    The function first determines the slope and intercept of the line
-    connecting the two input points. If the line is vertical, the function
-    returns an array of points with the same x coordinate and a range of y
-    coordinates. Otherwise, the function calculates the coordinates of the
-    points on the line using the slope and intercept, and returns an array of
-    these coordinates. The returned array is sorted by distance from the first
-    input point.
+    between the two input points, and returns an array of these coordinates. We
+    first get the number of possible points integer points. And then finds such
+    points such that they are linearly placed. And then combines them.
     """
 
     x1, y1 = np.array(point_1).astype(int)
     x2, y2 = np.array(point_2).astype(int)
 
-    # Calculate the slope of the line
-    if x1 == x2:
-        # Handle the special case where the line is vertical
-        x_coords: np.ndarray = np.full(abs(y2 - y1) + 1, x1)
-        y_coords: np.ndarray = np.arange(min(y1, y2), max(y1, y2) + 1)
-    else:
-        slope: int = (y2 - y1) // (x2 - x1)
-        intercept: int = y1 - slope * x1
-
-        # Calculate the coordinates of the points on the line
-        x_coords: np.ndarray = np.arange(min(x1, x2), max(x1, x2) + 1)
-        y_coords: np.ndarray = np.around(slope * x_coords + intercept)
+    Dy: int = y2 - y1
+    Dx: int = x2 - x1
+    no_of_points: int = np.gcd(Dy, Dx) + 1
+
+    x_coords: np.ndarray = np.linspace(x1, x2, no_of_points, dtype=int)
+    y_coords: np.ndarray = np.linspace(y1, y2, no_of_points, dtype=int)
 
     # Combine the x and y coordinates into a single array
     points: np.ndarray = np.column_stack((x_coords, y_coords))
 
-    # Remove duplicate points
-    points: np.ndarray = np.unique(points, axis=0)
-
-    # Sort the points by distance from the first input point
-    distances: np.ndarray = np.linalg.norm(points - point_1, axis=1)
-    sorted_indices: np.ndarray = np.argsort(distances)
-    points: np.ndarray = points[sorted_indices]
-
-    return points.astype(int)
+    return points
 
 
 def get_integer_neighbors(value: int, radius: int) -> np.ndarray:
     """Get integers around a particular integer."""
     return np.arange(value - radius, value + radius + 1)
```

### Comparing `darwinio-0.3.0/src/darwinio/genome.py` & `darwinio-0.3.1/src/darwinio/genome.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/graphical_sim.py` & `darwinio-0.3.1/src/darwinio/graphical_sim.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/organism.py` & `darwinio-0.3.1/src/darwinio/organism.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/text_sim.py` & `darwinio-0.3.1/src/darwinio/text_sim.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/archaebacteria_halophile.png` & `darwinio-0.3.1/src/darwinio/assets/art/archaebacteria_halophile.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/archaebacteria_methanogen.png` & `darwinio-0.3.1/src/darwinio/assets/art/archaebacteria_methanogen.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/archaebacteria_thermoacidophile.png` & `darwinio-0.3.1/src/darwinio/assets/art/archaebacteria_thermoacidophile.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/eubacteria_BGA.png` & `darwinio-0.3.1/src/darwinio/assets/art/eubacteria_BGA.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/eubacteria_mycoplasma.png` & `darwinio-0.3.1/src/darwinio/assets/art/eubacteria_mycoplasma.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/eubacteroa_chemosynthetic.png` & `darwinio-0.3.1/src/darwinio/assets/art/eubacteroa_chemosynthetic.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/fungi-ascomycetes.png` & `darwinio-0.3.1/src/darwinio/assets/art/fungi-ascomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/fungi-basidiomycetes.png` & `darwinio-0.3.1/src/darwinio/assets/art/fungi-basidiomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/fungi-deuteromycetes.png` & `darwinio-0.3.1/src/darwinio/assets/art/fungi-deuteromycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/fungi-phycomycetes.png` & `darwinio-0.3.1/src/darwinio/assets/art/fungi-phycomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/metaphyta-algae.png` & `darwinio-0.3.1/src/darwinio/assets/art/metaphyta-algae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/metaphyta-angiospermae.png` & `darwinio-0.3.1/src/darwinio/assets/art/metaphyta-angiospermae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/metaphyta-bryophyta.png` & `darwinio-0.3.1/src/darwinio/assets/art/metaphyta-bryophyta.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/metaphyta-gymnospermae.png` & `darwinio-0.3.1/src/darwinio/assets/art/metaphyta-gymnospermae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/metaphyta-pterdiophyta.png` & `darwinio-0.3.1/src/darwinio/assets/art/metaphyta-pterdiophyta.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/protista_dinoflagellate.png` & `darwinio-0.3.1/src/darwinio/assets/art/protista_dinoflagellate.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/protista_euglena.png` & `darwinio-0.3.1/src/darwinio/assets/art/protista_euglena.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/protista_protozoan.png` & `darwinio-0.3.1/src/darwinio/assets/art/protista_protozoan.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/protista_slimemould.png` & `darwinio-0.3.1/src/darwinio/assets/art/protista_slimemould.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/art/theme.json` & `darwinio-0.3.1/src/darwinio/assets/art/theme.json`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/src/darwinio/assets/audio/Darwinio.mp3` & `darwinio-0.3.1/src/darwinio/assets/audio/Darwinio.mp3`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/LICENSE.md` & `darwinio-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/README.md` & `darwinio-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.3.0/pyproject.toml` & `darwinio-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [tool.hatch.build]
 exclude = [
   "*.wav",
 ]
 
 [project]
 name = "darwinio"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Tushar Maharana", email="tusharhero@sdf.org" },
   { name="Mihir Nallagonda", email="adhikshithamihir@gmail.com" },
 ]
 description = "An evolution simulator"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `darwinio-0.3.0/PKG-INFO` & `darwinio-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darwinio
-Version: 0.3.0
+Version: 0.3.1
 Summary: An evolution simulator
 Project-URL: Homepage, https://github.com/tusharhero/darwinio
 Project-URL: Bug Tracker, https://github.com/tusharhero/darwinio/issues
 Author-email: Tushar Maharana <tusharhero@sdf.org>, Mihir Nallagonda <adhikshithamihir@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/brickblock-0.1.0.tar.gz` & `tmp/brickblock-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brickblock-0.1.0.tar", max compression
+gzip compressed data, was "brickblock-0.1.1.tar", max compression
```

## Comparing `brickblock-0.1.0.tar` & `brickblock-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35823 2023-07-11 16:43:32.128481 brickblock-0.1.0/LICENSE
--rw-r--r--   0        0        0     2411 2023-07-12 12:12:42.050834 brickblock-0.1.0/README.md
--rw-r--r--   0        0        0       30 2023-07-12 12:12:23.190399 brickblock-0.1.0/brickblock/__init__.py
--rw-r--r--   0        0        0    17417 2023-07-12 12:12:23.182553 brickblock-0.1.0/brickblock/space.py
--rw-r--r--   0        0        0      446 2023-07-12 12:12:23.177749 brickblock-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 brickblock-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-07-11 16:43:32.128481 brickblock-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2419 2023-07-12 12:20:04.956839 brickblock-0.1.1/README.md
+-rw-r--r--   0        0        0       30 2023-07-12 12:12:23.190399 brickblock-0.1.1/brickblock/__init__.py
+-rw-r--r--   0        0        0    17417 2023-07-12 12:12:23.182553 brickblock-0.1.1/brickblock/space.py
+-rw-r--r--   0        0        0      446 2023-07-12 12:23:28.976727 brickblock-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2989 1970-01-01 00:00:00.000000 brickblock-0.1.1/PKG-INFO
```

### Comparing `brickblock-0.1.0/LICENSE` & `brickblock-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brickblock-0.1.0/README.md` & `brickblock-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,34 @@
-# Sterling: A fun visualisation library for those that like boxes
+Metadata-Version: 2.1
+Name: brickblock
+Version: 0.1.1
+Summary: A fun visualisation library for those that like boxes
+Author: Daniel Soutar
+Author-email: danielsoutar144@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
+Requires-Dist: numpy (>=1.25.1,<2.0.0)
+Requires-Dist: pytest (>=7.4.0,<8.0.0)
+Description-Content-Type: text/markdown
+
+# Brickblock: A fun visualisation library for those that like boxes
 
 This is a small library that uses blocks in matplotlib's visually appealing 3D extension - and aims to be the 'seaborn of matplotlib-3D', if you will.
 
 ## Core abstractions
 
-At the centre of Sterling is the `Space`. A `Space` contains objects, and when a user wants a visualisation, they render the current state of the `Space` - the rendered state is known as a `Scene`.
+At the centre of BrickBlock is the `Space`. A `Space` contains objects, and when a user wants a visualisation, they render the current state of the `Space` - the rendered state is known as a `Scene`.
 
-Currently there is one object used for composing visualisations in Sterling: the `Cube`. `Cube` objects can be added into the `Space` with a degree of control over their visual presentation: transparency, colour, line widths.
+Currently there is one object used for composing visualisations in BrickBlock: the `Cube`. `Cube` objects can be added into the `Space` with a degree of control over their visual presentation: transparency, colour, line widths.
 
-Sterling also supports `Transition`s and `Transform`s:
+BrickBlock also supports `Transition`s and `Transform`s:
 
 * A `Transform` is simply any change to the space like adding one or more `Cube` objects. It does not produce a `Scene`. These are useful when you are just iteratively building up to a complex `Scene`.
 * A `Transition`, by contrast, is a transform between two `Scene`s. These are useful for generating sequences of `Scene`s - the `Space` will keep track of its state over time, as well as which states are `Scene`s. A `Transition` can be defined by one or more `Transform`s.
 
 Having these abstractions allows programmers to create animated visualisations like GIFs. You define a `Space`, using `Transform`s and `Transition`s to evolve the state, and the `Scene` objects are persisted to enable sequences of images for use in GIFs.
 
 ```python
@@ -40,7 +56,8 @@
 fig, ax = bb.render(s)
 # Or take a snapshot to indicate that this is a scene...
 state_history = bb.snapshot(s)
 # Do more stuff...
 # And then when you're ready, generate a GIF-like output...
 gif_filename = bb.stream(s, "gif", path_to_file))
 ```
+
```

### Comparing `brickblock-0.1.0/brickblock/space.py` & `brickblock-0.1.1/brickblock/space.py`

 * *Files identical despite different names*

### Comparing `brickblock-0.1.0/PKG-INFO` & `brickblock-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,18 @@
-Metadata-Version: 2.1
-Name: brickblock
-Version: 0.1.0
-Summary: A fun visualisation library for those that like boxes
-Author: Daniel Soutar
-Author-email: danielsoutar144@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
-Requires-Dist: numpy (>=1.25.1,<2.0.0)
-Requires-Dist: pytest (>=7.4.0,<8.0.0)
-Description-Content-Type: text/markdown
-
-# Sterling: A fun visualisation library for those that like boxes
+# Brickblock: A fun visualisation library for those that like boxes
 
 This is a small library that uses blocks in matplotlib's visually appealing 3D extension - and aims to be the 'seaborn of matplotlib-3D', if you will.
 
 ## Core abstractions
 
-At the centre of Sterling is the `Space`. A `Space` contains objects, and when a user wants a visualisation, they render the current state of the `Space` - the rendered state is known as a `Scene`.
+At the centre of BrickBlock is the `Space`. A `Space` contains objects, and when a user wants a visualisation, they render the current state of the `Space` - the rendered state is known as a `Scene`.
 
-Currently there is one object used for composing visualisations in Sterling: the `Cube`. `Cube` objects can be added into the `Space` with a degree of control over their visual presentation: transparency, colour, line widths.
+Currently there is one object used for composing visualisations in BrickBlock: the `Cube`. `Cube` objects can be added into the `Space` with a degree of control over their visual presentation: transparency, colour, line widths.
 
-Sterling also supports `Transition`s and `Transform`s:
+BrickBlock also supports `Transition`s and `Transform`s:
 
 * A `Transform` is simply any change to the space like adding one or more `Cube` objects. It does not produce a `Scene`. These are useful when you are just iteratively building up to a complex `Scene`.
 * A `Transition`, by contrast, is a transform between two `Scene`s. These are useful for generating sequences of `Scene`s - the `Space` will keep track of its state over time, as well as which states are `Scene`s. A `Transition` can be defined by one or more `Transform`s.
 
 Having these abstractions allows programmers to create animated visualisations like GIFs. You define a `Space`, using `Transform`s and `Transition`s to evolve the state, and the `Scene` objects are persisted to enable sequences of images for use in GIFs.
 
 ```python
@@ -56,8 +40,7 @@
 fig, ax = bb.render(s)
 # Or take a snapshot to indicate that this is a scene...
 state_history = bb.snapshot(s)
 # Do more stuff...
 # And then when you're ready, generate a GIF-like output...
 gif_filename = bb.stream(s, "gif", path_to_file))
 ```
-
```


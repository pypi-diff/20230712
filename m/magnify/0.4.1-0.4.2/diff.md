# Comparing `tmp/magnify-0.4.1.tar.gz` & `tmp/magnify-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnify-0.4.1.tar", max compression
+gzip compressed data, was "magnify-0.4.2.tar", max compression
```

## Comparing `magnify-0.4.1.tar` & `magnify-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.4.1/README.md
--rw-r--r--   0        0        0     1631 2023-07-11 23:24:24.576990 magnify-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      243 2023-07-11 23:24:31.489126 magnify-0.4.1/src/magnify/__init__.py
--rw-r--r--   0        0        0     3692 2023-07-11 23:24:08.976685 magnify-0.4.1/src/magnify/filter.py
--rw-r--r--   0        0        0    26165 2023-07-11 19:47:47.845868 magnify-0.4.1/src/magnify/find.py
--rw-r--r--   0        0        0     7516 2023-07-07 19:57:46.832323 magnify-0.4.1/src/magnify/identify.py
--rw-r--r--   0        0        0     1278 2023-07-07 22:23:16.867076 magnify-0.4.1/src/magnify/pipeline.py
--rw-r--r--   0        0        0      318 2023-07-07 19:04:45.491234 magnify-0.4.1/src/magnify/plot/__init__.py
--rw-r--r--   0        0        0     2345 2023-07-07 19:04:45.527235 magnify-0.4.1/src/magnify/plot/image.py
--rw-r--r--   0        0        0     1856 2023-07-07 19:04:45.511235 magnify-0.4.1/src/magnify/plot/ndplot.py
--rw-r--r--   0        0        0     2501 2023-07-07 19:04:45.551236 magnify-0.4.1/src/magnify/plot/relation.py
--rw-r--r--   0        0        0      694 2023-07-07 19:04:45.503235 magnify-0.4.1/src/magnify/plot/style.py
--rw-r--r--   0        0        0      445 2023-07-07 23:40:28.478446 magnify-0.4.1/src/magnify/postprocess.py
--rw-r--r--   0        0        0     1180 2023-07-07 19:09:00.448530 magnify-0.4.1/src/magnify/preprocess.py
--rw-r--r--   0        0        0    14930 2023-07-11 23:23:45.940234 magnify-0.4.1/src/magnify/reader.py
--rw-r--r--   0        0        0     2926 2023-07-07 23:43:18.929994 magnify-0.4.1/src/magnify/registry.py
--rw-r--r--   0        0        0     1077 2023-05-23 23:12:37.145369 magnify-0.4.1/src/magnify/stitch.py
--rw-r--r--   0        0        0     2639 2023-07-07 19:50:21.414864 magnify-0.4.1/src/magnify/utils.py
--rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 magnify-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.4.2/README.md
+-rw-r--r--   0        0        0     1631 2023-07-11 23:37:15.500967 magnify-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-07-11 23:37:20.385082 magnify-0.4.2/src/magnify/__init__.py
+-rw-r--r--   0        0        0     3692 2023-07-11 23:24:08.976685 magnify-0.4.2/src/magnify/filter.py
+-rw-r--r--   0        0        0    26135 2023-07-11 23:36:11.587453 magnify-0.4.2/src/magnify/find.py
+-rw-r--r--   0        0        0     7516 2023-07-07 19:57:46.832323 magnify-0.4.2/src/magnify/identify.py
+-rw-r--r--   0        0        0     1278 2023-07-07 22:23:16.867076 magnify-0.4.2/src/magnify/pipeline.py
+-rw-r--r--   0        0        0      318 2023-07-07 19:04:45.491234 magnify-0.4.2/src/magnify/plot/__init__.py
+-rw-r--r--   0        0        0     2345 2023-07-07 19:04:45.527235 magnify-0.4.2/src/magnify/plot/image.py
+-rw-r--r--   0        0        0     1856 2023-07-07 19:04:45.511235 magnify-0.4.2/src/magnify/plot/ndplot.py
+-rw-r--r--   0        0        0     2501 2023-07-07 19:04:45.551236 magnify-0.4.2/src/magnify/plot/relation.py
+-rw-r--r--   0        0        0      694 2023-07-07 19:04:45.503235 magnify-0.4.2/src/magnify/plot/style.py
+-rw-r--r--   0        0        0      446 2023-07-11 23:37:04.000697 magnify-0.4.2/src/magnify/postprocess.py
+-rw-r--r--   0        0        0     1180 2023-07-07 19:09:00.448530 magnify-0.4.2/src/magnify/preprocess.py
+-rw-r--r--   0        0        0    14930 2023-07-11 23:23:45.940234 magnify-0.4.2/src/magnify/reader.py
+-rw-r--r--   0        0        0     2926 2023-07-07 23:43:18.929994 magnify-0.4.2/src/magnify/registry.py
+-rw-r--r--   0        0        0     1077 2023-05-23 23:12:37.145369 magnify-0.4.2/src/magnify/stitch.py
+-rw-r--r--   0        0        0     2639 2023-07-07 19:50:21.414864 magnify-0.4.2/src/magnify/utils.py
+-rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 magnify-0.4.2/PKG-INFO
```

### Comparing `magnify-0.4.1/pyproject.toml` & `magnify-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnify"
-version = "0.4.1"
+version = "0.4.2"
 description = "A microscopy image processing toolkit."
 authors = ["Karl Krauth <karl.krauth@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 opencv-python = [
```

### Comparing `magnify-0.4.1/src/magnify/filter.py` & `magnify-0.4.2/src/magnify/filter.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.1/src/magnify/find.py` & `magnify-0.4.2/src/magnify/find.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,20 +36,20 @@
         self.col_dist = col_dist
         self.min_button_radius = min_button_radius
         self.max_button_radius = max_button_radius
         self.cluster_penalty = cluster_penalty
         self.roi_length = roi_length
         self.progress_bar = progress_bar
         self.search_timesteps = utils.to_list(search_timestep)
-        if search_channel is None:
-            self.search_channels = assay.channel
-        else:
-            self.search_channels = utils.to_list(search_channel)
+        self.search_channels = utils.to_list(search_channel)
 
     def __call__(self, assay: xr.Dataset) -> xr.Dataset:
+        if not self.search_channels:
+            self.search_channels = assay.channel
+
         num_rows, num_cols = assay.tag.shape
 
         # Store all channels and timesteps for each marker in one chunk and set marker row/col
         # sizes so each chunk ends up being at least 10MB.
         chunk_bytes = 1e7
         # Don't take into account dtype size since fg/bg bool arrays should also be 10MB.
         mark_bytes = assay.dims["channel"] * assay.dims["time"] * self.roi_length**2
@@ -379,20 +379,20 @@
         max_bead_radius: int = 25,
         roi_length: int = 61,
         search_channel: str | list[str] | None = None,
     ):
         self.min_bead_radius = min_bead_radius
         self.max_bead_radius = max_bead_radius
         self.roi_length = roi_length
-        if search_channel is None:
-            self.search_channels = assay.channel
-        else:
-            self.search_channels = utils.to_list(search_channel)
+        self.search_channels = utils.to_list(search_channel)
 
     def __call__(self, assay: xr.Dataset) -> xr.Dataset:
+        if not self.search_channels:
+            self.search_channels = assay.channel
+
         centers = np.empty((0, 2))
         labels = np.zeros((assay.sizes["im_y"], assay.sizes["im_x"]), dtype=int)
         for t in assay.time:
             for search_channel in self.search_channels:
                 image = utils.to_uint8(assay.image.sel(channel=search_channel, time=t).to_numpy())
                 # Find a mask of all bright spots.
                 mask = cv.adaptiveThreshold(
```

### Comparing `magnify-0.4.1/src/magnify/identify.py` & `magnify-0.4.2/src/magnify/identify.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.1/src/magnify/pipeline.py` & `magnify-0.4.2/src/magnify/pipeline.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.1/src/magnify/plot/image.py` & `magnify-0.4.2/src/magnify/plot/image.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.1/src/magnify/plot/ndplot.py` & `magnify-0.4.2/src/magnify/plot/ndplot.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.1/src/magnify/plot/relation.py` & `magnify-0.4.2/src/magnify/plot/relation.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.1/src/magnify/plot/style.py` & `magnify-0.4.2/src/magnify/plot/style.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.1/src/magnify/preprocess.py` & `magnify-0.4.2/src/magnify/preprocess.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.1/src/magnify/reader.py` & `magnify-0.4.2/src/magnify/reader.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.1/src/magnify/registry.py` & `magnify-0.4.2/src/magnify/registry.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.1/src/magnify/stitch.py` & `magnify-0.4.2/src/magnify/stitch.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.1/src/magnify/utils.py` & `magnify-0.4.2/src/magnify/utils.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.1/PKG-INFO` & `magnify-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnify
-Version: 0.4.1
+Version: 0.4.2
 Summary: A microscopy image processing toolkit.
 Author: Karl Krauth
 Author-email: karl.krauth@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


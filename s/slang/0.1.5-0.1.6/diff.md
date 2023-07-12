# Comparing `tmp/slang-0.1.5.tar.gz` & `tmp/slang-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slang-0.1.5.tar", last modified: Wed Dec  7 20:34:14 2022, max compression
+gzip compressed data, was "slang-0.1.6.tar", last modified: Wed Jul 12 00:22:02 2023, max compression
```

## Comparing `slang-0.1.5.tar` & `slang-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 20:34:14.518911 slang-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-07 20:33:27.000000 slang-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26532 2022-12-07 20:34:14.518911 slang-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23367 2022-12-07 20:33:27.000000 slang-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      677 2022-12-07 20:34:14.522910 slang-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-07 20:33:27.000000 slang-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 20:34:14.518911 slang-0.1.5/slang/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2022-12-07 20:34:11.000000 slang-0.1.5/slang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20493 2022-12-07 20:33:27.000000 slang-0.1.5/slang/chunkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2022-12-07 20:33:27.000000 slang-0.1.5/slang/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2022-12-07 20:34:11.000000 slang-0.1.5/slang/featurizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 20:34:14.518911 slang-0.1.5/slang/scrap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 20:33:27.000000 slang-0.1.5/slang/scrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2022-12-07 20:33:27.000000 slang-0.1.5/slang/scrap/learning_pipeline_01.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2022-12-07 20:33:27.000000 slang-0.1.5/slang/scrap/scrap_01.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2022-12-07 20:33:27.000000 slang-0.1.5/slang/scrap/the_apis_i_wish_for.py
--rw-r--r--   0 runner    (1001) docker     (123)    28484 2022-12-07 20:33:27.000000 slang-0.1.5/slang/snip_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12062 2022-12-07 20:33:27.000000 slang-0.1.5/slang/snippers.py
--rw-r--r--   0 runner    (1001) docker     (123)    42173 2022-12-07 20:34:12.000000 slang-0.1.5/slang/spectrop.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2022-12-07 20:33:27.000000 slang-0.1.5/slang/stypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2022-12-07 20:33:27.000000 slang-0.1.5/slang/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    15935 2022-12-07 20:33:27.000000 slang-0.1.5/slang/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    50015 2022-12-07 20:33:27.000000 slang-0.1.5/slang/util_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 20:34:14.518911 slang-0.1.5/slang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26532 2022-12-07 20:34:14.000000 slang-0.1.5/slang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      518 2022-12-07 20:34:14.000000 slang-0.1.5/slang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 20:34:14.000000 slang-0.1.5/slang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 20:34:14.000000 slang-0.1.5/slang.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-07 20:34:14.000000 slang-0.1.5/slang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-07 20:34:14.000000 slang-0.1.5/slang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:22:02.631711 slang-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 00:20:45.000000 slang-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26532 2023-07-12 00:22:02.631711 slang-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23367 2023-07-12 00:20:45.000000 slang-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-12 00:22:02.631711 slang-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-12 00:20:45.000000 slang-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:22:02.627711 slang-0.1.6/slang/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-12 00:20:45.000000 slang-0.1.6/slang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20493 2023-07-12 00:20:45.000000 slang-0.1.6/slang/chunkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-07-12 00:20:45.000000 slang-0.1.6/slang/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-07-12 00:20:45.000000 slang-0.1.6/slang/featurizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:22:02.631711 slang-0.1.6/slang/scrap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 00:20:45.000000 slang-0.1.6/slang/scrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-12 00:20:45.000000 slang-0.1.6/slang/scrap/learning_pipeline_01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-12 00:20:45.000000 slang-0.1.6/slang/scrap/scrap_01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-12 00:20:45.000000 slang-0.1.6/slang/scrap/the_apis_i_wish_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28484 2023-07-12 00:20:45.000000 slang-0.1.6/slang/snip_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-07-12 00:20:45.000000 slang-0.1.6/slang/snippers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42204 2023-07-12 00:20:45.000000 slang-0.1.6/slang/spectrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-12 00:20:45.000000 slang-0.1.6/slang/stypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-12 00:20:45.000000 slang-0.1.6/slang/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15935 2023-07-12 00:20:45.000000 slang-0.1.6/slang/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50015 2023-07-12 00:20:45.000000 slang-0.1.6/slang/util_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:22:02.627711 slang-0.1.6/slang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26532 2023-07-12 00:22:02.000000 slang-0.1.6/slang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-12 00:22:02.000000 slang-0.1.6/slang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 00:22:02.000000 slang-0.1.6/slang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 00:22:02.000000 slang-0.1.6/slang.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 00:22:02.000000 slang-0.1.6/slang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 00:22:02.000000 slang-0.1.6/slang.egg-info/top_level.txt
```

### Comparing `slang-0.1.5/LICENSE` & `slang-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `slang-0.1.5/PKG-INFO` & `slang-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slang
-Version: 0.1.5
+Version: 0.1.6
 Summary: A structural approach to signal ML
 Home-page: https://github.com/otosense/slang
 License: mit
 Description: - [Slang: Light weight tools to build signal languages](#slang--light-weight-tools-to-build-signal-languages)
           * [A story to paint the horizon](#a-story-to-paint-the-horizon)
           * [Okay, but what does a pipeline look like in slang](#okay--but-what-does-a-pipeline-look-like-in-slang)
         - [Sound Language](#sound-language)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: slang Version: 0.1.5 Summary: A structural approach
+Metadata-Version: 2.1 Name: slang Version: 0.1.6 Summary: A structural approach
 to signal ML Home-page: https://github.com/otosense/slang License: mit
 Description: - [Slang: Light weight tools to build signal languages](#slang--
 light-weight-tools-to-build-signal-languages) * [A story to paint the horizon]
 (#a-story-to-paint-the-horizon) * [Okay, but what does a pipeline look like in
 slang](#okay--but-what-does-a-pipeline-look-like-in-slang) - [Sound Language]
 (#sound-language) - [Structural and Syntactical Pattern Recognition]
 (#structural-and-syntactical-pattern-recognition) - [Semantic Structure]
```

### Comparing `slang-0.1.5/README.md` & `slang-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `slang-0.1.5/setup.cfg` & `slang-0.1.6/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.1.5
+version = 0.1.6
 description = A structural approach to signal ML
 license = mit
 description_file = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 keywords = 
 	sound recognition
```

### Comparing `slang-0.1.5/slang/__init__.py` & `slang-0.1.6/slang/__init__.py`

 * *Files identical despite different names*

### Comparing `slang-0.1.5/slang/chunkers.py` & `slang-0.1.6/slang/chunkers.py`

 * *Files identical despite different names*

### Comparing `slang-0.1.5/slang/core.py` & `slang-0.1.6/slang/core.py`

 * *Files identical despite different names*

### Comparing `slang-0.1.5/slang/featurizers.py` & `slang-0.1.6/slang/featurizers.py`

 * *Files identical despite different names*

### Comparing `slang-0.1.5/slang/snip_stats.py` & `slang-0.1.6/slang/snip_stats.py`

 * *Files identical despite different names*

### Comparing `slang-0.1.5/slang/snippers.py` & `slang-0.1.6/slang/snippers.py`

 * *Files identical despite different names*

### Comparing `slang-0.1.5/slang/spectrop.py` & `slang-0.1.6/slang/spectrop.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
         else:
             _assert_spectrum_and_chk_size_match(spectrum_size, chk_size)
     return spectrum_size
 
 
 @dataclass
 class Projector:
-    scalings_: np.ndarray = DFLT_SCALINGS
+    scalings_: np.ndarray = field(default_factory=lambda: DFLT_SCALINGS)
     mat_mult: Callable = DFLT_MATRIX_MULTI
 
     def transform(self, X):
         # return projection(self.scalings_, ascertain_array(X))
         return reducing_proj(self.scalings_, ascertain_array(X), mat_mult=self.mat_mult)
 
     def to_jdict(self):
```

### Comparing `slang-0.1.5/slang/stypes.py` & `slang-0.1.6/slang/stypes.py`

 * *Files identical despite different names*

### Comparing `slang-0.1.5/slang/tools.py` & `slang-0.1.6/slang/tools.py`

 * *Files identical despite different names*

### Comparing `slang-0.1.5/slang/util.py` & `slang-0.1.6/slang/util.py`

 * *Files identical despite different names*

### Comparing `slang-0.1.5/slang/util_data.py` & `slang-0.1.6/slang/util_data.py`

 * *Files identical despite different names*

### Comparing `slang-0.1.5/slang.egg-info/PKG-INFO` & `slang-0.1.6/slang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slang
-Version: 0.1.5
+Version: 0.1.6
 Summary: A structural approach to signal ML
 Home-page: https://github.com/otosense/slang
 License: mit
 Description: - [Slang: Light weight tools to build signal languages](#slang--light-weight-tools-to-build-signal-languages)
           * [A story to paint the horizon](#a-story-to-paint-the-horizon)
           * [Okay, but what does a pipeline look like in slang](#okay--but-what-does-a-pipeline-look-like-in-slang)
         - [Sound Language](#sound-language)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: slang Version: 0.1.5 Summary: A structural approach
+Metadata-Version: 2.1 Name: slang Version: 0.1.6 Summary: A structural approach
 to signal ML Home-page: https://github.com/otosense/slang License: mit
 Description: - [Slang: Light weight tools to build signal languages](#slang--
 light-weight-tools-to-build-signal-languages) * [A story to paint the horizon]
 (#a-story-to-paint-the-horizon) * [Okay, but what does a pipeline look like in
 slang](#okay--but-what-does-a-pipeline-look-like-in-slang) - [Sound Language]
 (#sound-language) - [Structural and Syntactical Pattern Recognition]
 (#structural-and-syntactical-pattern-recognition) - [Semantic Structure]
```

### Comparing `slang-0.1.5/slang.egg-info/SOURCES.txt` & `slang-0.1.6/slang.egg-info/SOURCES.txt`

 * *Files identical despite different names*


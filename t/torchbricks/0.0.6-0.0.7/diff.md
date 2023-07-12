# Comparing `tmp/torchbricks-0.0.6.tar.gz` & `tmp/torchbricks-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbricks-0.0.6.tar", last modified: Wed Jul 12 05:46:31 2023, max compression
+gzip compressed data, was "torchbricks-0.0.7.tar", last modified: Wed Jul 12 13:17:35 2023, max compression
```

## Comparing `torchbricks-0.0.6.tar` & `torchbricks-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:46:31.208448 torchbricks-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-12 05:46:15.000000 torchbricks-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 05:46:15.000000 torchbricks-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-07-12 05:46:31.208448 torchbricks-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18338 2023-07-12 05:46:15.000000 torchbricks-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-12 05:46:15.000000 torchbricks-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 05:46:31.208448 torchbricks-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:46:31.204448 torchbricks-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:46:31.208448 torchbricks-0.0.6/src/torchbricks/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 05:46:15.000000 torchbricks-0.0.6/src/torchbricks/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 05:46:15.000000 torchbricks-0.0.6/src/torchbricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-12 05:46:15.000000 torchbricks-0.0.6/src/torchbricks/bag_of_bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-07-12 05:46:15.000000 torchbricks-0.0.6/src/torchbricks/bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-12 05:46:15.000000 torchbricks-0.0.6/src/torchbricks/bricks_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-12 05:46:15.000000 torchbricks-0.0.6/src/torchbricks/custom_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:46:31.208448 torchbricks-0.0.6/src/torchbricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-07-12 05:46:31.000000 torchbricks-0.0.6/src/torchbricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-12 05:46:31.000000 torchbricks-0.0.6/src/torchbricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 05:46:31.000000 torchbricks-0.0.6/src/torchbricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 05:46:31.000000 torchbricks-0.0.6/src/torchbricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 05:46:31.000000 torchbricks-0.0.6/src/torchbricks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:46:31.208448 torchbricks-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 05:46:15.000000 torchbricks-0.0.6/tests/test_bag_of_bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-07-12 05:46:15.000000 torchbricks-0.0.6/tests/test_bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-07-12 05:46:15.000000 torchbricks-0.0.6/tests/test_bricks_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:17:35.753691 torchbricks-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-12 13:17:20.000000 torchbricks-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 13:17:20.000000 torchbricks-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-07-12 13:17:35.753691 torchbricks-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18487 2023-07-12 13:17:20.000000 torchbricks-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-12 13:17:20.000000 torchbricks-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:17:35.753691 torchbricks-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:17:35.749691 torchbricks-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:17:35.749691 torchbricks-0.0.7/src/torchbricks/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 13:17:20.000000 torchbricks-0.0.7/src/torchbricks/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 13:17:20.000000 torchbricks-0.0.7/src/torchbricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-12 13:17:20.000000 torchbricks-0.0.7/src/torchbricks/bag_of_bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-07-12 13:17:20.000000 torchbricks-0.0.7/src/torchbricks/bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-12 13:17:20.000000 torchbricks-0.0.7/src/torchbricks/bricks_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-12 13:17:20.000000 torchbricks-0.0.7/src/torchbricks/custom_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:17:35.753691 torchbricks-0.0.7/src/torchbricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-07-12 13:17:35.000000 torchbricks-0.0.7/src/torchbricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-12 13:17:35.000000 torchbricks-0.0.7/src/torchbricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:17:35.000000 torchbricks-0.0.7/src/torchbricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 13:17:35.000000 torchbricks-0.0.7/src/torchbricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 13:17:35.000000 torchbricks-0.0.7/src/torchbricks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:17:35.753691 torchbricks-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 13:17:20.000000 torchbricks-0.0.7/tests/test_bag_of_bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-07-12 13:17:20.000000 torchbricks-0.0.7/tests/test_bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-07-12 13:17:20.000000 torchbricks-0.0.7/tests/test_bricks_helper.py
```

### Comparing `torchbricks-0.0.6/LICENSE` & `torchbricks-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.6/PKG-INFO` & `torchbricks-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbricks
-Version: 0.0.6
+Version: 0.0.7
 Summary: Decoupled and modular approach to building multi-task ML models
 Author-email: Peter Hviid Christianse <PeterHviidChristiansen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Peter Christiansen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -121,16 +121,17 @@
 
 All modules are added as entries in a regular dictionary and for each module, we provide a name (dictionary key) and 
 input and output names. The number of input and output names should match the actually number of input and outputs 
 for each function. 
 
 Each module is wrapped inside a brick - here either `BrickTrainable` and `BrickNotTrainable`.
 
-The `preprocessor` uses a `raw` input tensor and passes the `processed` tensor to the `backbone`. The backbone returns 
-the `embedding` tensor and passes it to the `head` determining both `logits` and `softmaxed` tensors. 
+The `bricks`-dictionary describe how data is passed between bricks: The `preprocessor` uses a `raw` input tensor and passes the
+`processed` tensor to the `backbone`. The backbone returns the `embedding` tensor and passes it to the `head` determining 
+both `logits` and `softmaxed` tensors. 
 
 Bricks are then passed to a `BrickCollection` for executing bricks. The brick collection accepts a dictionary with required inputs and
 returns a dictionary with both intermediated and resulting tensors. 
 
 ```python
 brick_collection = BrickCollection(bricks)
 batch_images = torch.rand((2, 3, 100, 200))
@@ -376,14 +377,15 @@
 - [x] Update README.md to match the new bricks. 
   - [x] Start with basic bricks example. 
   - [x] Use loss-function to show that stage decided on what is being executed. 
   - [x] Introduce metrics by it-self in another example
 - [x] Ensure that all examples in the `README.md` are working with easy to use modules. 
 - [x] Add typeguard
 - [x] Allow a brick to receive all named_inputs and add a test for it.
+- [x] Fix the release process. It should be as simple as running `make release`.
 - [ ] Add onnx export example to the README.md
 - [ ] Make DAG like functionality to check if a inputs and outputs works for all model stages.
 - [ ] Use pymy, pyright or pyre to do static code checks. 
 - [ ] Decide: Add stage as an internal state and not in the forward pass:
   - Minor Pros: Tracing (to get onnx model) requires only torch.Tensors only as input - we avoid making an adapter class. 
   - Minor Cons: State gets hidden away - implicit instead of explicit.
   - Minor Pros: Similar to eval/training
```

### Comparing `torchbricks-0.0.6/README.md` & `torchbricks-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,16 +85,17 @@
 
 All modules are added as entries in a regular dictionary and for each module, we provide a name (dictionary key) and 
 input and output names. The number of input and output names should match the actually number of input and outputs 
 for each function. 
 
 Each module is wrapped inside a brick - here either `BrickTrainable` and `BrickNotTrainable`.
 
-The `preprocessor` uses a `raw` input tensor and passes the `processed` tensor to the `backbone`. The backbone returns 
-the `embedding` tensor and passes it to the `head` determining both `logits` and `softmaxed` tensors. 
+The `bricks`-dictionary describe how data is passed between bricks: The `preprocessor` uses a `raw` input tensor and passes the
+`processed` tensor to the `backbone`. The backbone returns the `embedding` tensor and passes it to the `head` determining 
+both `logits` and `softmaxed` tensors. 
 
 Bricks are then passed to a `BrickCollection` for executing bricks. The brick collection accepts a dictionary with required inputs and
 returns a dictionary with both intermediated and resulting tensors. 
 
 ```python
 brick_collection = BrickCollection(bricks)
 batch_images = torch.rand((2, 3, 100, 200))
@@ -340,14 +341,15 @@
 - [x] Update README.md to match the new bricks. 
   - [x] Start with basic bricks example. 
   - [x] Use loss-function to show that stage decided on what is being executed. 
   - [x] Introduce metrics by it-self in another example
 - [x] Ensure that all examples in the `README.md` are working with easy to use modules. 
 - [x] Add typeguard
 - [x] Allow a brick to receive all named_inputs and add a test for it.
+- [x] Fix the release process. It should be as simple as running `make release`.
 - [ ] Add onnx export example to the README.md
 - [ ] Make DAG like functionality to check if a inputs and outputs works for all model stages.
 - [ ] Use pymy, pyright or pyre to do static code checks. 
 - [ ] Decide: Add stage as an internal state and not in the forward pass:
   - Minor Pros: Tracing (to get onnx model) requires only torch.Tensors only as input - we avoid making an adapter class. 
   - Minor Cons: State gets hidden away - implicit instead of explicit.
   - Minor Pros: Similar to eval/training
```

### Comparing `torchbricks-0.0.6/pyproject.toml` & `torchbricks-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [tool.ruff]
 line-length = 140
 select = ["C4", "E", "F","B", "I", "W", "RUF"]
 
 [project]
 name = "torchbricks"
-version = "0.0.6"
+version = "0.0.7"
 description = "Decoupled and modular approach to building multi-task ML models"
 readme = "README.md"
 authors = [{ name = "Peter Hviid Christianse", email = "PeterHviidChristiansen@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -27,15 +27,15 @@
 requires-python = ">=3.7"
 
 [project.urls]
 Homepage = "https://github.com/PeteHeine/torchbricks"
 
 # bumpver update --patch | --minor | --major --dry
 [tool.bumpver]
-current_version = "0.0.6"
+current_version = "0.0.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]  # Specify all files containging version-numbers
```

### Comparing `torchbricks-0.0.6/src/torchbricks/bag_of_bricks.py` & `torchbricks-0.0.7/src/torchbricks/bag_of_bricks.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.6/src/torchbricks/bricks.py` & `torchbricks-0.0.7/src/torchbricks/bricks.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.6/src/torchbricks/bricks_helper.py` & `torchbricks-0.0.7/src/torchbricks/bricks_helper.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.6/src/torchbricks/custom_metrics.py` & `torchbricks-0.0.7/src/torchbricks/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.6/src/torchbricks.egg-info/PKG-INFO` & `torchbricks-0.0.7/src/torchbricks.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbricks
-Version: 0.0.6
+Version: 0.0.7
 Summary: Decoupled and modular approach to building multi-task ML models
 Author-email: Peter Hviid Christianse <PeterHviidChristiansen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Peter Christiansen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -121,16 +121,17 @@
 
 All modules are added as entries in a regular dictionary and for each module, we provide a name (dictionary key) and 
 input and output names. The number of input and output names should match the actually number of input and outputs 
 for each function. 
 
 Each module is wrapped inside a brick - here either `BrickTrainable` and `BrickNotTrainable`.
 
-The `preprocessor` uses a `raw` input tensor and passes the `processed` tensor to the `backbone`. The backbone returns 
-the `embedding` tensor and passes it to the `head` determining both `logits` and `softmaxed` tensors. 
+The `bricks`-dictionary describe how data is passed between bricks: The `preprocessor` uses a `raw` input tensor and passes the
+`processed` tensor to the `backbone`. The backbone returns the `embedding` tensor and passes it to the `head` determining 
+both `logits` and `softmaxed` tensors. 
 
 Bricks are then passed to a `BrickCollection` for executing bricks. The brick collection accepts a dictionary with required inputs and
 returns a dictionary with both intermediated and resulting tensors. 
 
 ```python
 brick_collection = BrickCollection(bricks)
 batch_images = torch.rand((2, 3, 100, 200))
@@ -376,14 +377,15 @@
 - [x] Update README.md to match the new bricks. 
   - [x] Start with basic bricks example. 
   - [x] Use loss-function to show that stage decided on what is being executed. 
   - [x] Introduce metrics by it-self in another example
 - [x] Ensure that all examples in the `README.md` are working with easy to use modules. 
 - [x] Add typeguard
 - [x] Allow a brick to receive all named_inputs and add a test for it.
+- [x] Fix the release process. It should be as simple as running `make release`.
 - [ ] Add onnx export example to the README.md
 - [ ] Make DAG like functionality to check if a inputs and outputs works for all model stages.
 - [ ] Use pymy, pyright or pyre to do static code checks. 
 - [ ] Decide: Add stage as an internal state and not in the forward pass:
   - Minor Pros: Tracing (to get onnx model) requires only torch.Tensors only as input - we avoid making an adapter class. 
   - Minor Cons: State gets hidden away - implicit instead of explicit.
   - Minor Pros: Similar to eval/training
```

### Comparing `torchbricks-0.0.6/tests/test_bag_of_bricks.py` & `torchbricks-0.0.7/tests/test_bag_of_bricks.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.6/tests/test_bricks.py` & `torchbricks-0.0.7/tests/test_bricks.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.6/tests/test_bricks_helper.py` & `torchbricks-0.0.7/tests/test_bricks_helper.py`

 * *Files identical despite different names*


# Comparing `tmp/torchbricks-0.0.7.tar.gz` & `tmp/torchbricks-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbricks-0.0.7.tar", last modified: Wed Jul 12 13:17:35 2023, max compression
+gzip compressed data, was "torchbricks-0.0.8.tar", last modified: Wed Jul 12 14:10:32 2023, max compression
```

## Comparing `torchbricks-0.0.7.tar` & `torchbricks-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:17:35.753691 torchbricks-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-12 13:17:20.000000 torchbricks-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 13:17:20.000000 torchbricks-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-07-12 13:17:35.753691 torchbricks-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18487 2023-07-12 13:17:20.000000 torchbricks-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-12 13:17:20.000000 torchbricks-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:17:35.753691 torchbricks-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:17:35.749691 torchbricks-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:17:35.749691 torchbricks-0.0.7/src/torchbricks/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 13:17:20.000000 torchbricks-0.0.7/src/torchbricks/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 13:17:20.000000 torchbricks-0.0.7/src/torchbricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-12 13:17:20.000000 torchbricks-0.0.7/src/torchbricks/bag_of_bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-07-12 13:17:20.000000 torchbricks-0.0.7/src/torchbricks/bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-12 13:17:20.000000 torchbricks-0.0.7/src/torchbricks/bricks_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-12 13:17:20.000000 torchbricks-0.0.7/src/torchbricks/custom_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:17:35.753691 torchbricks-0.0.7/src/torchbricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-07-12 13:17:35.000000 torchbricks-0.0.7/src/torchbricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-12 13:17:35.000000 torchbricks-0.0.7/src/torchbricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:17:35.000000 torchbricks-0.0.7/src/torchbricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 13:17:35.000000 torchbricks-0.0.7/src/torchbricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 13:17:35.000000 torchbricks-0.0.7/src/torchbricks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:17:35.753691 torchbricks-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 13:17:20.000000 torchbricks-0.0.7/tests/test_bag_of_bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-07-12 13:17:20.000000 torchbricks-0.0.7/tests/test_bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-07-12 13:17:20.000000 torchbricks-0.0.7/tests/test_bricks_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:10:32.308501 torchbricks-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-12 14:10:13.000000 torchbricks-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 14:10:13.000000 torchbricks-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21039 2023-07-12 14:10:32.308501 torchbricks-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-07-12 14:10:13.000000 torchbricks-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-12 14:10:13.000000 torchbricks-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:10:32.308501 torchbricks-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:10:32.304501 torchbricks-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:10:32.308501 torchbricks-0.0.8/src/torchbricks/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 14:10:13.000000 torchbricks-0.0.8/src/torchbricks/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 14:10:13.000000 torchbricks-0.0.8/src/torchbricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-12 14:10:13.000000 torchbricks-0.0.8/src/torchbricks/bag_of_bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-12 14:10:13.000000 torchbricks-0.0.8/src/torchbricks/brick_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-07-12 14:10:13.000000 torchbricks-0.0.8/src/torchbricks/bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-12 14:10:13.000000 torchbricks-0.0.8/src/torchbricks/bricks_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-12 14:10:13.000000 torchbricks-0.0.8/src/torchbricks/custom_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:10:32.308501 torchbricks-0.0.8/src/torchbricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21039 2023-07-12 14:10:32.000000 torchbricks-0.0.8/src/torchbricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-12 14:10:32.000000 torchbricks-0.0.8/src/torchbricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:10:32.000000 torchbricks-0.0.8/src/torchbricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 14:10:32.000000 torchbricks-0.0.8/src/torchbricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 14:10:32.000000 torchbricks-0.0.8/src/torchbricks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:10:32.308501 torchbricks-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 14:10:13.000000 torchbricks-0.0.8/tests/test_bag_of_bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-12 14:10:13.000000 torchbricks-0.0.8/tests/test_brick_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-07-12 14:10:13.000000 torchbricks-0.0.8/tests/test_bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-07-12 14:10:13.000000 torchbricks-0.0.8/tests/test_bricks_helper.py
```

### Comparing `torchbricks-0.0.7/LICENSE` & `torchbricks-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.7/PKG-INFO` & `torchbricks-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbricks
-Version: 0.0.7
+Version: 0.0.8
 Summary: Decoupled and modular approach to building multi-task ML models
 Author-email: Peter Hviid Christianse <PeterHviidChristiansen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Peter Christiansen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,24 +49,14 @@
     display_name: torchbricks
     language: python
     name: python3
 ---
 
 -->
 
-# TorchBricks
-
-[![codecov](https://codecov.io/gh/PeteHeine/torchbricks/branch/main/graph/badge.svg?token=torchbricks_token_here)](https://codecov.io/gh/PeteHeine/torchbricks)
-[![CI](https://github.com/PeteHeine/torchbricks/actions/workflows/main.yml/badge.svg)](https://github.com/PeteHeine/torchbricks/actions/workflows/main.yml)
-
-TorchBricks builds pytorch models using small reuseable and decoupled parts - we call them bricks.
-
-The concept is simple and flexible and allows you to more easily combine, add more or swap out parts of the model (preprocessor, backbone, neck, head or post-processor), change the task or extend it with multiple tasks.
-
-
 <!-- #region -->
 
 ## Install it with pip
 
 ```bash
 pip install torchbricks
 ```
@@ -130,15 +120,16 @@
 both `logits` and `softmaxed` tensors. 
 
 Bricks are then passed to a `BrickCollection` for executing bricks. The brick collection accepts a dictionary with required inputs and
 returns a dictionary with both intermediated and resulting tensors. 
 
 ```python
 brick_collection = BrickCollection(bricks)
-batch_images = torch.rand((2, 3, 100, 200))
+batch_size=2
+batch_images = torch.rand((batch_size, 3, 100, 200))
 named_outputs = brick_collection(named_inputs={'raw': batch_images}, stage=Stage.INFERENCE)
 print(named_outputs.keys())
 ```
 
 Running our models as a brick collection has the following advantages:
 
 - A brick collection act as a regular `nn.Module` with all the familiar features: a `forward`-function, a `to`-function to move 
@@ -163,43 +154,50 @@
 Meaning that for different `stages` of the model, we will have the option of creating a unique DAG for each model stage. 
 
 In above example this is not particular interesting - because preprocessor, backbone model and head would typically be alive in all stages. 
 
 So we will demonstrate by adding a loss brick (`BrickLoss`) and specifying `alive_stages` for each brick.
 
 ```python
+num_classes = 3
 bricks = {
     'preprocessor': BrickNotTrainable(PreprocessorDummy(), input_names=['raw'], output_names=['processed'], alive_stages="all"),
-    'backbone': BrickTrainable(TinyModel(n_channels=3, n_features=10), input_names=['processed'], output_names=['embedding'], alive_stages="all"),
-    'head': BrickTrainable(ClassifierDummy(num_classes=3, in_features=10), input_names=['embedding'], output_names=['logits', 'softmaxed'], 
-                                    alive_stages="all"),
+    'backbone': BrickTrainable(TinyModel(n_channels=num_classes, n_features=10), input_names=['processed'], output_names=['embedding'], 
+                               alive_stages="all"),
+    'head': BrickTrainable(ClassifierDummy(num_classes=num_classes, in_features=10), input_names=['embedding'], 
+                           output_names=['logits', 'softmaxed'], alive_stages="all"),
     'loss': BrickLoss(model=nn.CrossEntropyLoss(), input_names=['logits', 'targets'], output_names=['loss_ce'], 
                       alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST], loss_output_names="all")
 }
+brick_collection = BrickCollection(bricks)
 ```
 
-<!-- #region -->
 We set `preprocessor`, `backbone` and `head` to be alive on all stages `alive_stages="all"` - this is the default behavior and
 similar to before. 
 
 For `loss` we set `alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST]` to calculate loss during train, validation and test
 stages. 
 
 Another advantages is that model have different input requirements for different stages.
 
 For `Stage.INFERENCE` and `Stage.EXPROT` stages, the model only requires the `raw` tensor as input. 
 
-While for `Stage.TRAIN`, `Stage.VALIDATION` and `Stage.TEST` stages, the model requires both `raw` and `targets` input tensors.
+```python
+named_outputs_without_loss = brick_collection(named_inputs={'raw': batch_images}, stage=Stage.INFERENCE)   
+```
+
+<!-- #region -->
+
 
+For `Stage.TRAIN`, `Stage.VALIDATION` and `Stage.TEST` stages, the model requires both `raw` and `targets` input tensors.
+<!-- #endregion -->
 
 ```python
-    named_outputs_without_loss = brick_collection(named_inputs={'raw': batch_images}, stage=Stage.INFERENCE)
-    named_outputs_with_loss = brick_collection(named_inputs={'raw': batch_images, "targets": torch.ones((1,3))}, stage=Stage.TRAIN)
+named_outputs_with_loss = brick_collection(named_inputs={'raw': batch_images, "targets": torch.ones((batch_size,3))}, stage=Stage.TRAIN)
 ```
-<!-- #endregion -->
 
 ## Bricks for model training
 We are not creating a training framework, but to easily use the brick collection in your favorite training framework or custom 
 training/validation/test loop, we need the final piece. We should be able to calculate and gather metrics across a whole dataset. 
 
 We will extend our example from before by adding metric bricks and common reusable components from `torchbricks.bag_of_bricks`.
 
@@ -219,15 +217,15 @@
     'head': BrickTrainable(ImageClassifier(num_classes=num_classes, n_features=resnet_brick.model.n_backbone_features),
                                      input_names=['features'], output_names=['logits', 'probabilities', 'class_prediction']),
     'accuracy': BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), input_names=['class_prediction', 'targets']),
     'loss': BrickLoss(model=nn.CrossEntropyLoss(), input_names=['logits', 'targets'], output_names=['loss_ce'])
 }
 
 brick_collection = BrickCollection(bricks)
-named_inputs = {"raw": batch_images, "targets": torch.ones((2), dtype=torch.int64)}
+named_inputs = {"raw": batch_images, "targets": torch.ones((batch_size), dtype=torch.int64)}
 named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.TRAIN)
 named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.TRAIN)
 named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.TRAIN)
 named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.TRAIN)
 metrics = brick_collection.summarize(stage=Stage.TRAIN, reset=True)
 print(f"{metrics=}, {named_outputs.keys()=}")
 ```
@@ -266,29 +264,70 @@
 - The typical distinction between `encode`  / `decoder` becomes to limited... Multiple decoders might share a `neck`.
 
 
 ## Brick features: 
 
 Missing sections:
 
-- [ ] Acts as a nn.Module
+- [x] Export as ONNX
+- [x] Acts as a nn.Module
 - [ ] Acts as a dictionary - Nested brick collection
-- [ ] Export as ONNX
 - [ ] Training with Pytorch lightning
 - [ ] Pass all inputs as a dictionary `input_names='all'`
 - [ ] Using stage inside module
 - [ ] the `extract_losses` function
 - [ ] Bag of bricks - reusable bricks modules
   - [ ] Note also in above example we use bag-of-bricks to import commonly used `nn.Module`s. This includes a `Preprocessor`, `ImageClassifier` and `resnet_to_brick` to convert torchvision resnet models into a backbone brick  (without a classifier).
 - [ ] The default `BrickModule`
 - [ ] In this example we do not use `BrickModule` to build our collection - you can do that -
 but instead we recommend using our pre-configured brick modules (`BrickLoss`, `BrickNotTrainable`, `BrickTrainable`, 
 `BrickMetricSingle` and `BrickCollection`) to both ensure sensible defaults and to show the intend of each brick. 
 
 
+### Brick features: Export as ONNX
+To export a brick collection as onnx we provide the `export_bricks_as_onnx`-function. 
+
+Pass an example input (`named_input`) to trace a brick collection.
+Set `dynamic_batch_size=True` to support any batch size inputs and here we explicitly set `stage=Stage.EXPORT` - this is also 
+the default.
+
+```python
+from pathlib import Path
+from torchbricks.brick_utils import export_bricks_as_onnx
+path_onnx = Path("build/readme_model.onnx")
+export_bricks_as_onnx(path_onnx=path_onnx, 
+                      brick_collection=brick_collection, 
+                      named_inputs=named_inputs, 
+                      dynamic_batch_size=True, 
+                      stage=Stage.EXPORT)
+```
+
+### Brick features: Act as a nn.Module
+A brick collection acts as a 'nn.Module' mean we can do the following: 
+
+```python
+# Move to specify device (CPU/GPU) or precision to automatically move model parameters
+brick_collection_half = brick_collection.to(torch.float16)
+
+
+# Save model parameters
+path_model = Path("build/readme_model.pt")
+torch.save(brick_collection_half.state_dict(), path_model)
+
+# Load model parameters
+brick_collection_half.load_state_dict(torch.load(path_model))
+
+# Access parameters
+brick_collection_half.named_parameters()
+```
+
+
+
+
+
 ### Bag of bricks - reusable bricks modules
 Note also in above example we use bag-of-bricks to import commonly used `nn.Module`s 
 
 This includes a `Preprocessor`, `ImageClassifier` and `resnet_to_brick` to convert torchvision resnet models into a backbone brick 
 (without a classifier).
 
 
@@ -378,15 +417,15 @@
   - [x] Start with basic bricks example. 
   - [x] Use loss-function to show that stage decided on what is being executed. 
   - [x] Introduce metrics by it-self in another example
 - [x] Ensure that all examples in the `README.md` are working with easy to use modules. 
 - [x] Add typeguard
 - [x] Allow a brick to receive all named_inputs and add a test for it.
 - [x] Fix the release process. It should be as simple as running `make release`.
-- [ ] Add onnx export example to the README.md
+- [x] Add onnx export example to the README.md
 - [ ] Make DAG like functionality to check if a inputs and outputs works for all model stages.
 - [ ] Use pymy, pyright or pyre to do static code checks. 
 - [ ] Decide: Add stage as an internal state and not in the forward pass:
   - Minor Pros: Tracing (to get onnx model) requires only torch.Tensors only as input - we avoid making an adapter class. 
   - Minor Cons: State gets hidden away - implicit instead of explicit.
   - Minor Pros: Similar to eval/training 
 - [ ] Collection of helper modules. Preprocessors, Backbones, Necks/Upsamplers, ImageClassification, SemanticSegmentation, ObjectDetection
```

### Comparing `torchbricks-0.0.7/README.md` & `torchbricks-0.0.8/src/torchbricks.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,43 @@
+Metadata-Version: 2.1
+Name: torchbricks
+Version: 0.0.8
+Summary: Decoupled and modular approach to building multi-task ML models
+Author-email: Peter Hviid Christianse <PeterHviidChristiansen@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Peter Christiansen
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/PeteHeine/torchbricks
+Keywords: torch,multi-task,machine learning
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <!--
 
 ---
 jupyter:
   jupytext:
     hide_notebook_metadata: true
     text_representation:
@@ -13,24 +49,14 @@
     display_name: torchbricks
     language: python
     name: python3
 ---
 
 -->
 
-# TorchBricks
-
-[![codecov](https://codecov.io/gh/PeteHeine/torchbricks/branch/main/graph/badge.svg?token=torchbricks_token_here)](https://codecov.io/gh/PeteHeine/torchbricks)
-[![CI](https://github.com/PeteHeine/torchbricks/actions/workflows/main.yml/badge.svg)](https://github.com/PeteHeine/torchbricks/actions/workflows/main.yml)
-
-TorchBricks builds pytorch models using small reuseable and decoupled parts - we call them bricks.
-
-The concept is simple and flexible and allows you to more easily combine, add more or swap out parts of the model (preprocessor, backbone, neck, head or post-processor), change the task or extend it with multiple tasks.
-
-
 <!-- #region -->
 
 ## Install it with pip
 
 ```bash
 pip install torchbricks
 ```
@@ -94,15 +120,16 @@
 both `logits` and `softmaxed` tensors. 
 
 Bricks are then passed to a `BrickCollection` for executing bricks. The brick collection accepts a dictionary with required inputs and
 returns a dictionary with both intermediated and resulting tensors. 
 
 ```python
 brick_collection = BrickCollection(bricks)
-batch_images = torch.rand((2, 3, 100, 200))
+batch_size=2
+batch_images = torch.rand((batch_size, 3, 100, 200))
 named_outputs = brick_collection(named_inputs={'raw': batch_images}, stage=Stage.INFERENCE)
 print(named_outputs.keys())
 ```
 
 Running our models as a brick collection has the following advantages:
 
 - A brick collection act as a regular `nn.Module` with all the familiar features: a `forward`-function, a `to`-function to move 
@@ -127,43 +154,50 @@
 Meaning that for different `stages` of the model, we will have the option of creating a unique DAG for each model stage. 
 
 In above example this is not particular interesting - because preprocessor, backbone model and head would typically be alive in all stages. 
 
 So we will demonstrate by adding a loss brick (`BrickLoss`) and specifying `alive_stages` for each brick.
 
 ```python
+num_classes = 3
 bricks = {
     'preprocessor': BrickNotTrainable(PreprocessorDummy(), input_names=['raw'], output_names=['processed'], alive_stages="all"),
-    'backbone': BrickTrainable(TinyModel(n_channels=3, n_features=10), input_names=['processed'], output_names=['embedding'], alive_stages="all"),
-    'head': BrickTrainable(ClassifierDummy(num_classes=3, in_features=10), input_names=['embedding'], output_names=['logits', 'softmaxed'], 
-                                    alive_stages="all"),
+    'backbone': BrickTrainable(TinyModel(n_channels=num_classes, n_features=10), input_names=['processed'], output_names=['embedding'], 
+                               alive_stages="all"),
+    'head': BrickTrainable(ClassifierDummy(num_classes=num_classes, in_features=10), input_names=['embedding'], 
+                           output_names=['logits', 'softmaxed'], alive_stages="all"),
     'loss': BrickLoss(model=nn.CrossEntropyLoss(), input_names=['logits', 'targets'], output_names=['loss_ce'], 
                       alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST], loss_output_names="all")
 }
+brick_collection = BrickCollection(bricks)
 ```
 
-<!-- #region -->
 We set `preprocessor`, `backbone` and `head` to be alive on all stages `alive_stages="all"` - this is the default behavior and
 similar to before. 
 
 For `loss` we set `alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST]` to calculate loss during train, validation and test
 stages. 
 
 Another advantages is that model have different input requirements for different stages.
 
 For `Stage.INFERENCE` and `Stage.EXPROT` stages, the model only requires the `raw` tensor as input. 
 
-While for `Stage.TRAIN`, `Stage.VALIDATION` and `Stage.TEST` stages, the model requires both `raw` and `targets` input tensors.
+```python
+named_outputs_without_loss = brick_collection(named_inputs={'raw': batch_images}, stage=Stage.INFERENCE)   
+```
+
+<!-- #region -->
+
 
+For `Stage.TRAIN`, `Stage.VALIDATION` and `Stage.TEST` stages, the model requires both `raw` and `targets` input tensors.
+<!-- #endregion -->
 
 ```python
-    named_outputs_without_loss = brick_collection(named_inputs={'raw': batch_images}, stage=Stage.INFERENCE)
-    named_outputs_with_loss = brick_collection(named_inputs={'raw': batch_images, "targets": torch.ones((1,3))}, stage=Stage.TRAIN)
+named_outputs_with_loss = brick_collection(named_inputs={'raw': batch_images, "targets": torch.ones((batch_size,3))}, stage=Stage.TRAIN)
 ```
-<!-- #endregion -->
 
 ## Bricks for model training
 We are not creating a training framework, but to easily use the brick collection in your favorite training framework or custom 
 training/validation/test loop, we need the final piece. We should be able to calculate and gather metrics across a whole dataset. 
 
 We will extend our example from before by adding metric bricks and common reusable components from `torchbricks.bag_of_bricks`.
 
@@ -183,15 +217,15 @@
     'head': BrickTrainable(ImageClassifier(num_classes=num_classes, n_features=resnet_brick.model.n_backbone_features),
                                      input_names=['features'], output_names=['logits', 'probabilities', 'class_prediction']),
     'accuracy': BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), input_names=['class_prediction', 'targets']),
     'loss': BrickLoss(model=nn.CrossEntropyLoss(), input_names=['logits', 'targets'], output_names=['loss_ce'])
 }
 
 brick_collection = BrickCollection(bricks)
-named_inputs = {"raw": batch_images, "targets": torch.ones((2), dtype=torch.int64)}
+named_inputs = {"raw": batch_images, "targets": torch.ones((batch_size), dtype=torch.int64)}
 named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.TRAIN)
 named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.TRAIN)
 named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.TRAIN)
 named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.TRAIN)
 metrics = brick_collection.summarize(stage=Stage.TRAIN, reset=True)
 print(f"{metrics=}, {named_outputs.keys()=}")
 ```
@@ -230,29 +264,70 @@
 - The typical distinction between `encode`  / `decoder` becomes to limited... Multiple decoders might share a `neck`.
 
 
 ## Brick features: 
 
 Missing sections:
 
-- [ ] Acts as a nn.Module
+- [x] Export as ONNX
+- [x] Acts as a nn.Module
 - [ ] Acts as a dictionary - Nested brick collection
-- [ ] Export as ONNX
 - [ ] Training with Pytorch lightning
 - [ ] Pass all inputs as a dictionary `input_names='all'`
 - [ ] Using stage inside module
 - [ ] the `extract_losses` function
 - [ ] Bag of bricks - reusable bricks modules
   - [ ] Note also in above example we use bag-of-bricks to import commonly used `nn.Module`s. This includes a `Preprocessor`, `ImageClassifier` and `resnet_to_brick` to convert torchvision resnet models into a backbone brick  (without a classifier).
 - [ ] The default `BrickModule`
 - [ ] In this example we do not use `BrickModule` to build our collection - you can do that -
 but instead we recommend using our pre-configured brick modules (`BrickLoss`, `BrickNotTrainable`, `BrickTrainable`, 
 `BrickMetricSingle` and `BrickCollection`) to both ensure sensible defaults and to show the intend of each brick. 
 
 
+### Brick features: Export as ONNX
+To export a brick collection as onnx we provide the `export_bricks_as_onnx`-function. 
+
+Pass an example input (`named_input`) to trace a brick collection.
+Set `dynamic_batch_size=True` to support any batch size inputs and here we explicitly set `stage=Stage.EXPORT` - this is also 
+the default.
+
+```python
+from pathlib import Path
+from torchbricks.brick_utils import export_bricks_as_onnx
+path_onnx = Path("build/readme_model.onnx")
+export_bricks_as_onnx(path_onnx=path_onnx, 
+                      brick_collection=brick_collection, 
+                      named_inputs=named_inputs, 
+                      dynamic_batch_size=True, 
+                      stage=Stage.EXPORT)
+```
+
+### Brick features: Act as a nn.Module
+A brick collection acts as a 'nn.Module' mean we can do the following: 
+
+```python
+# Move to specify device (CPU/GPU) or precision to automatically move model parameters
+brick_collection_half = brick_collection.to(torch.float16)
+
+
+# Save model parameters
+path_model = Path("build/readme_model.pt")
+torch.save(brick_collection_half.state_dict(), path_model)
+
+# Load model parameters
+brick_collection_half.load_state_dict(torch.load(path_model))
+
+# Access parameters
+brick_collection_half.named_parameters()
+```
+
+
+
+
+
 ### Bag of bricks - reusable bricks modules
 Note also in above example we use bag-of-bricks to import commonly used `nn.Module`s 
 
 This includes a `Preprocessor`, `ImageClassifier` and `resnet_to_brick` to convert torchvision resnet models into a backbone brick 
 (without a classifier).
 
 
@@ -342,15 +417,15 @@
   - [x] Start with basic bricks example. 
   - [x] Use loss-function to show that stage decided on what is being executed. 
   - [x] Introduce metrics by it-self in another example
 - [x] Ensure that all examples in the `README.md` are working with easy to use modules. 
 - [x] Add typeguard
 - [x] Allow a brick to receive all named_inputs and add a test for it.
 - [x] Fix the release process. It should be as simple as running `make release`.
-- [ ] Add onnx export example to the README.md
+- [x] Add onnx export example to the README.md
 - [ ] Make DAG like functionality to check if a inputs and outputs works for all model stages.
 - [ ] Use pymy, pyright or pyre to do static code checks. 
 - [ ] Decide: Add stage as an internal state and not in the forward pass:
   - Minor Pros: Tracing (to get onnx model) requires only torch.Tensors only as input - we avoid making an adapter class. 
   - Minor Cons: State gets hidden away - implicit instead of explicit.
   - Minor Pros: Similar to eval/training 
 - [ ] Collection of helper modules. Preprocessors, Backbones, Necks/Upsamplers, ImageClassification, SemanticSegmentation, ObjectDetection
```

### Comparing `torchbricks-0.0.7/pyproject.toml` & `torchbricks-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [tool.ruff]
 line-length = 140
 select = ["C4", "E", "F","B", "I", "W", "RUF"]
 
 [project]
 name = "torchbricks"
-version = "0.0.7"
+version = "0.0.8"
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
-current_version = "0.0.7"
+current_version = "0.0.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]  # Specify all files containging version-numbers
```

### Comparing `torchbricks-0.0.7/src/torchbricks/bag_of_bricks.py` & `torchbricks-0.0.8/src/torchbricks/bag_of_bricks.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.7/src/torchbricks/bricks.py` & `torchbricks-0.0.8/src/torchbricks/bricks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from abc import ABC, abstractmethod
 from enum import Enum
-from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
-import torch
 from torch import nn
 from torchmetrics import Metric, MetricCollection
 from typeguard import typechecked
 
 from torchbricks.bricks_helper import named_input_and_outputs_callable
 
 
@@ -274,48 +272,7 @@
                  input_names: Union[List[str], Dict[str, str], str],
                  metric_name: Optional[str] = None,
                  alive_stages: List[Stage] | None = None,
                  return_metrics: bool = False):
         metric_name = metric_name or metric.__class__.__name__
         super().__init__(metric_collection={metric_name: metric}, input_names=input_names, alive_stages=alive_stages,
                          return_metrics=return_metrics)
-
-
-@typechecked
-class OnnxExportAdaptor(nn.Module):
-    def __init__(self, model: nn.Module, stage: Stage) -> None:
-        super().__init__()
-        self.model = model
-        self.stage = stage
-
-    def forward(self, named_inputs: Dict[str, Any]):
-        named_outputs = self.model.forward(named_inputs=named_inputs, stage=self.stage, return_inputs=False)
-        return named_outputs
-
-
-@typechecked
-def export_as_onnx(brick_collection: BrickCollection,
-                   named_inputs: Dict[str, torch.Tensor],
-                   path_onnx: Path,
-                   dynamic_batch_size: bool,
-                   stage: Stage = Stage.EXPORT,
-                   **onnx_export_kwargs):
-
-    outputs = brick_collection(named_inputs=named_inputs, stage=stage, return_inputs=False)
-    onnx_exportable = OnnxExportAdaptor(model=brick_collection, stage=stage)
-    output_names = list(outputs)
-    input_names = list(named_inputs)
-
-    if dynamic_batch_size:
-        if 'dynamic_axes' in onnx_export_kwargs:
-            raise ValueError("Setting both 'dynamic_batch_size==True' and defining 'dynamic_axes' in 'onnx_export_kwargs' is not allowed. ")
-        io_names = input_names + output_names
-        dynamic_axes = {io_name: {0: 'batch_size'} for io_name in io_names}
-        onnx_export_kwargs['dynamic_axes'] = dynamic_axes
-
-    torch.onnx.export(model=onnx_exportable,
-                      args=({'named_inputs': named_inputs}, ),
-                      f=str(path_onnx),
-                      verbose=True,
-                      input_names=input_names,
-                      output_names=output_names,
-                      **onnx_export_kwargs)
```

### Comparing `torchbricks-0.0.7/src/torchbricks/bricks_helper.py` & `torchbricks-0.0.8/src/torchbricks/bricks_helper.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.7/src/torchbricks/custom_metrics.py` & `torchbricks-0.0.8/src/torchbricks/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.7/src/torchbricks.egg-info/PKG-INFO` & `torchbricks-0.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,7 @@
-Metadata-Version: 2.1
-Name: torchbricks
-Version: 0.0.7
-Summary: Decoupled and modular approach to building multi-task ML models
-Author-email: Peter Hviid Christianse <PeterHviidChristiansen@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Peter Christiansen
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/PeteHeine/torchbricks
-Keywords: torch,multi-task,machine learning
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!--
 
 ---
 jupyter:
   jupytext:
     hide_notebook_metadata: true
     text_representation:
@@ -49,24 +13,14 @@
     display_name: torchbricks
     language: python
     name: python3
 ---
 
 -->
 
-# TorchBricks
-
-[![codecov](https://codecov.io/gh/PeteHeine/torchbricks/branch/main/graph/badge.svg?token=torchbricks_token_here)](https://codecov.io/gh/PeteHeine/torchbricks)
-[![CI](https://github.com/PeteHeine/torchbricks/actions/workflows/main.yml/badge.svg)](https://github.com/PeteHeine/torchbricks/actions/workflows/main.yml)
-
-TorchBricks builds pytorch models using small reuseable and decoupled parts - we call them bricks.
-
-The concept is simple and flexible and allows you to more easily combine, add more or swap out parts of the model (preprocessor, backbone, neck, head or post-processor), change the task or extend it with multiple tasks.
-
-
 <!-- #region -->
 
 ## Install it with pip
 
 ```bash
 pip install torchbricks
 ```
@@ -130,15 +84,16 @@
 both `logits` and `softmaxed` tensors. 
 
 Bricks are then passed to a `BrickCollection` for executing bricks. The brick collection accepts a dictionary with required inputs and
 returns a dictionary with both intermediated and resulting tensors. 
 
 ```python
 brick_collection = BrickCollection(bricks)
-batch_images = torch.rand((2, 3, 100, 200))
+batch_size=2
+batch_images = torch.rand((batch_size, 3, 100, 200))
 named_outputs = brick_collection(named_inputs={'raw': batch_images}, stage=Stage.INFERENCE)
 print(named_outputs.keys())
 ```
 
 Running our models as a brick collection has the following advantages:
 
 - A brick collection act as a regular `nn.Module` with all the familiar features: a `forward`-function, a `to`-function to move 
@@ -163,43 +118,50 @@
 Meaning that for different `stages` of the model, we will have the option of creating a unique DAG for each model stage. 
 
 In above example this is not particular interesting - because preprocessor, backbone model and head would typically be alive in all stages. 
 
 So we will demonstrate by adding a loss brick (`BrickLoss`) and specifying `alive_stages` for each brick.
 
 ```python
+num_classes = 3
 bricks = {
     'preprocessor': BrickNotTrainable(PreprocessorDummy(), input_names=['raw'], output_names=['processed'], alive_stages="all"),
-    'backbone': BrickTrainable(TinyModel(n_channels=3, n_features=10), input_names=['processed'], output_names=['embedding'], alive_stages="all"),
-    'head': BrickTrainable(ClassifierDummy(num_classes=3, in_features=10), input_names=['embedding'], output_names=['logits', 'softmaxed'], 
-                                    alive_stages="all"),
+    'backbone': BrickTrainable(TinyModel(n_channels=num_classes, n_features=10), input_names=['processed'], output_names=['embedding'], 
+                               alive_stages="all"),
+    'head': BrickTrainable(ClassifierDummy(num_classes=num_classes, in_features=10), input_names=['embedding'], 
+                           output_names=['logits', 'softmaxed'], alive_stages="all"),
     'loss': BrickLoss(model=nn.CrossEntropyLoss(), input_names=['logits', 'targets'], output_names=['loss_ce'], 
                       alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST], loss_output_names="all")
 }
+brick_collection = BrickCollection(bricks)
 ```
 
-<!-- #region -->
 We set `preprocessor`, `backbone` and `head` to be alive on all stages `alive_stages="all"` - this is the default behavior and
 similar to before. 
 
 For `loss` we set `alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST]` to calculate loss during train, validation and test
 stages. 
 
 Another advantages is that model have different input requirements for different stages.
 
 For `Stage.INFERENCE` and `Stage.EXPROT` stages, the model only requires the `raw` tensor as input. 
 
-While for `Stage.TRAIN`, `Stage.VALIDATION` and `Stage.TEST` stages, the model requires both `raw` and `targets` input tensors.
+```python
+named_outputs_without_loss = brick_collection(named_inputs={'raw': batch_images}, stage=Stage.INFERENCE)   
+```
+
+<!-- #region -->
+
 
+For `Stage.TRAIN`, `Stage.VALIDATION` and `Stage.TEST` stages, the model requires both `raw` and `targets` input tensors.
+<!-- #endregion -->
 
 ```python
-    named_outputs_without_loss = brick_collection(named_inputs={'raw': batch_images}, stage=Stage.INFERENCE)
-    named_outputs_with_loss = brick_collection(named_inputs={'raw': batch_images, "targets": torch.ones((1,3))}, stage=Stage.TRAIN)
+named_outputs_with_loss = brick_collection(named_inputs={'raw': batch_images, "targets": torch.ones((batch_size,3))}, stage=Stage.TRAIN)
 ```
-<!-- #endregion -->
 
 ## Bricks for model training
 We are not creating a training framework, but to easily use the brick collection in your favorite training framework or custom 
 training/validation/test loop, we need the final piece. We should be able to calculate and gather metrics across a whole dataset. 
 
 We will extend our example from before by adding metric bricks and common reusable components from `torchbricks.bag_of_bricks`.
 
@@ -219,15 +181,15 @@
     'head': BrickTrainable(ImageClassifier(num_classes=num_classes, n_features=resnet_brick.model.n_backbone_features),
                                      input_names=['features'], output_names=['logits', 'probabilities', 'class_prediction']),
     'accuracy': BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), input_names=['class_prediction', 'targets']),
     'loss': BrickLoss(model=nn.CrossEntropyLoss(), input_names=['logits', 'targets'], output_names=['loss_ce'])
 }
 
 brick_collection = BrickCollection(bricks)
-named_inputs = {"raw": batch_images, "targets": torch.ones((2), dtype=torch.int64)}
+named_inputs = {"raw": batch_images, "targets": torch.ones((batch_size), dtype=torch.int64)}
 named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.TRAIN)
 named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.TRAIN)
 named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.TRAIN)
 named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.TRAIN)
 metrics = brick_collection.summarize(stage=Stage.TRAIN, reset=True)
 print(f"{metrics=}, {named_outputs.keys()=}")
 ```
@@ -266,29 +228,70 @@
 - The typical distinction between `encode`  / `decoder` becomes to limited... Multiple decoders might share a `neck`.
 
 
 ## Brick features: 
 
 Missing sections:
 
-- [ ] Acts as a nn.Module
+- [x] Export as ONNX
+- [x] Acts as a nn.Module
 - [ ] Acts as a dictionary - Nested brick collection
-- [ ] Export as ONNX
 - [ ] Training with Pytorch lightning
 - [ ] Pass all inputs as a dictionary `input_names='all'`
 - [ ] Using stage inside module
 - [ ] the `extract_losses` function
 - [ ] Bag of bricks - reusable bricks modules
   - [ ] Note also in above example we use bag-of-bricks to import commonly used `nn.Module`s. This includes a `Preprocessor`, `ImageClassifier` and `resnet_to_brick` to convert torchvision resnet models into a backbone brick  (without a classifier).
 - [ ] The default `BrickModule`
 - [ ] In this example we do not use `BrickModule` to build our collection - you can do that -
 but instead we recommend using our pre-configured brick modules (`BrickLoss`, `BrickNotTrainable`, `BrickTrainable`, 
 `BrickMetricSingle` and `BrickCollection`) to both ensure sensible defaults and to show the intend of each brick. 
 
 
+### Brick features: Export as ONNX
+To export a brick collection as onnx we provide the `export_bricks_as_onnx`-function. 
+
+Pass an example input (`named_input`) to trace a brick collection.
+Set `dynamic_batch_size=True` to support any batch size inputs and here we explicitly set `stage=Stage.EXPORT` - this is also 
+the default.
+
+```python
+from pathlib import Path
+from torchbricks.brick_utils import export_bricks_as_onnx
+path_onnx = Path("build/readme_model.onnx")
+export_bricks_as_onnx(path_onnx=path_onnx, 
+                      brick_collection=brick_collection, 
+                      named_inputs=named_inputs, 
+                      dynamic_batch_size=True, 
+                      stage=Stage.EXPORT)
+```
+
+### Brick features: Act as a nn.Module
+A brick collection acts as a 'nn.Module' mean we can do the following: 
+
+```python
+# Move to specify device (CPU/GPU) or precision to automatically move model parameters
+brick_collection_half = brick_collection.to(torch.float16)
+
+
+# Save model parameters
+path_model = Path("build/readme_model.pt")
+torch.save(brick_collection_half.state_dict(), path_model)
+
+# Load model parameters
+brick_collection_half.load_state_dict(torch.load(path_model))
+
+# Access parameters
+brick_collection_half.named_parameters()
+```
+
+
+
+
+
 ### Bag of bricks - reusable bricks modules
 Note also in above example we use bag-of-bricks to import commonly used `nn.Module`s 
 
 This includes a `Preprocessor`, `ImageClassifier` and `resnet_to_brick` to convert torchvision resnet models into a backbone brick 
 (without a classifier).
 
 
@@ -378,15 +381,15 @@
   - [x] Start with basic bricks example. 
   - [x] Use loss-function to show that stage decided on what is being executed. 
   - [x] Introduce metrics by it-self in another example
 - [x] Ensure that all examples in the `README.md` are working with easy to use modules. 
 - [x] Add typeguard
 - [x] Allow a brick to receive all named_inputs and add a test for it.
 - [x] Fix the release process. It should be as simple as running `make release`.
-- [ ] Add onnx export example to the README.md
+- [x] Add onnx export example to the README.md
 - [ ] Make DAG like functionality to check if a inputs and outputs works for all model stages.
 - [ ] Use pymy, pyright or pyre to do static code checks. 
 - [ ] Decide: Add stage as an internal state and not in the forward pass:
   - Minor Pros: Tracing (to get onnx model) requires only torch.Tensors only as input - we avoid making an adapter class. 
   - Minor Cons: State gets hidden away - implicit instead of explicit.
   - Minor Pros: Similar to eval/training 
 - [ ] Collection of helper modules. Preprocessors, Backbones, Necks/Upsamplers, ImageClassification, SemanticSegmentation, ObjectDetection
```

### Comparing `torchbricks-0.0.7/tests/test_bag_of_bricks.py` & `torchbricks-0.0.8/tests/test_bag_of_bricks.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.7/tests/test_bricks.py` & `torchbricks-0.0.8/tests/test_bricks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,18 @@
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Optional
 
-import onnx
 import pytest
 import torch
 import torchmetrics
 from torch import nn
 from torchbricks import bricks, custom_metrics
-from torchbricks.bricks import BrickCollection, BrickLoss, BrickMetrics, BrickMetricSingle, Stage, export_as_onnx
+from torchbricks.bricks import BrickCollection, BrickLoss, BrickMetrics, BrickMetricSingle, Stage
 from torchmetrics.classification import MulticlassAccuracy
-from utils_testing.utils_testing import assert_equal_dictionaries
-
-
-def create_brick_collection(num_classes: int, num_backbone_featues: int) -> Dict[str, bricks.BrickInterface]:
-    class Preprocessor(nn.Module):
-        def forward(self, raw_input: torch.Tensor) -> torch.Tensor:
-            return raw_input/2
-
-    class TinyBackbone(nn.Module):
-        def __init__(self, n_kernels: int):
-            super().__init__()
-            self.conv1 = nn.Conv2d(in_channels=3, out_channels=n_kernels, kernel_size=3, padding=1)
-
-        def forward(self, tensor: torch.Tensor):
-            return self.conv1(tensor)
-
-
-    class Classifier(nn.Module):
-        def __init__(self, input_channels: int, num_classes: int):
-            super().__init__()
-            self.global_average_pooling = nn.AdaptiveAvgPool2d((1, 1))
-            self.classifier = nn.Conv2d(in_channels=input_channels, out_channels=num_classes, kernel_size=1)
-
-        def forward(self, features: torch.Tensor):
-            logits = torch.squeeze(self.classifier(self.global_average_pooling(features)))
-            return logits
-
-
-    metric_collection = torchmetrics.MetricCollection({
-        'MeanAccuracy': MulticlassAccuracy(num_classes=num_classes, average='macro'),
-        'Accuracy': MulticlassAccuracy(num_classes=num_classes, average='micro'),
-        'ConfMat': torchmetrics.ConfusionMatrix(task='multiclass', num_classes=num_classes),
-        'Concatenate': custom_metrics.ConcatenatePredictionAndTarget(compute_on_cpu=True)
-    })
-    brick_collections = {
-        'preprocessor': bricks.BrickNotTrainable(Preprocessor(), input_names=['raw'], output_names=['preprocessed']),
-        'backbone': bricks.BrickTrainable(TinyBackbone(n_kernels=num_backbone_featues), input_names=['preprocessed'],
-                                                       output_names=['features']),
-        'classifier': bricks.BrickTrainable(Classifier(input_channels=num_backbone_featues, num_classes=num_classes),
-                                            input_names=['features'],
-                                            output_names=['predictions']),
-        'loss': bricks.BrickLoss(nn.CrossEntropyLoss(), input_names=['predictions', 'labels'], output_names=['ce_loss']),
-        'metrics': bricks.BrickMetrics(metric_collection, input_names=['predictions', 'labels'])
-    }
-    return brick_collections
+from utils_testing.utils_testing import assert_equal_dictionaries, create_brick_collection
 
 
 def test_brick_collection():
     num_classes = 10
     brick_collection = create_brick_collection(num_classes=num_classes, num_backbone_featues=5)
     expected_forward_named_outputs = {'labels', 'raw', 'stage', 'preprocessed', 'features', 'predictions'}
     expected_named_losses = {'ce_loss'}
@@ -267,54 +222,7 @@
     named_inputs = {'labels': torch.tensor(range(num_classes), dtype=torch.float64), 'raw': torch.zeros((1, 3, 24, 24))}
     forward_expected = model(named_inputs=named_inputs, stage=stage)
 
     model_compiled = torch.compile(model)
     forward_actual = model_compiled(named_inputs=named_inputs, stage=stage)
 
     assert_equal_dictionaries(forward_expected, forward_actual, is_close=True)
-
-
-def test_export_onnx_trace(tmp_path: Path):
-    num_classes = 3
-    brick_collection = create_brick_collection(num_classes=num_classes, num_backbone_featues=10)
-    model = BrickCollection(brick_collection)
-    named_inputs = {'raw': torch.zeros((1, 3, 64, 64))}
-
-    stage = Stage.EXPORT
-    named_outputs = model(named_inputs, stage=stage, return_inputs=False)
-    # remove_from_outputs = ["stage"] + list(named_inputs)
-    expected_input = list(named_inputs)
-    expected_outputs = list(named_outputs)
-
-    path_onnx = Path(tmp_path / 'model.onnx')
-
-    dynamic_batch_size_configs = [False, True]
-    for dynamic_batch_size in dynamic_batch_size_configs:
-        export_as_onnx(brick_collection=model, named_inputs=named_inputs, path_onnx=path_onnx, stage=stage,
-                       dynamic_batch_size=dynamic_batch_size)
-
-        assert path_onnx.exists()
-        onnx_model = onnx.load(path_onnx)
-
-        output_names_graph = {output.name for output in onnx_model.graph.output}
-        assert set(expected_outputs) == output_names_graph
-
-        input_names_graph = {input.name for input in onnx_model.graph.input}
-        assert set(expected_input) == input_names_graph
-
-        onnx.checker.check_model(onnx_model)
-
-
-@pytest.mark.xfail
-def test_export_torch_jit_script(tmp_path: Path):
-    num_classes = 3
-    brick_collection = create_brick_collection(num_classes=num_classes, num_backbone_featues=10)
-    model = BrickCollection(brick_collection)
-    named_inputs = {'raw': torch.zeros((1, 3, 64, 64))}
-
-    stage = Stage.EXPORT
-    named_outputs = model(named_inputs, stage=stage, return_inputs=False)
-    # remove_from_outputs = ["stage"] + list(named_inputs)
-    list(named_inputs)
-    list(named_outputs)
-
-    torch.jit.script(model)
```

### Comparing `torchbricks-0.0.7/tests/test_bricks_helper.py` & `torchbricks-0.0.8/tests/test_bricks_helper.py`

 * *Files identical despite different names*


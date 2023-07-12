# Comparing `tmp/transformersplus-0.1.1.tar.gz` & `tmp/transformersplus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformersplus-0.1.1.tar", last modified: Mon Jun 26 10:29:49 2023, max compression
+gzip compressed data, was "transformersplus-0.2.0.tar", last modified: Wed Jul 12 10:40:01 2023, max compression
```

## Comparing `transformersplus-0.1.1.tar` & `transformersplus-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.066514 transformersplus-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-26 10:29:33.000000 transformersplus-0.1.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.054513 transformersplus-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.058513 transformersplus-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 10:29:33.000000 transformersplus-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-26 10:29:33.000000 transformersplus-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-06-26 10:29:33.000000 transformersplus-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-26 10:29:49.066514 transformersplus-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-26 10:29:33.000000 transformersplus-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.054513 transformersplus-0.1.1/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.062513 transformersplus-0.1.1/example/albert/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 10:29:33.000000 transformersplus-0.1.1/example/albert/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-26 10:29:33.000000 transformersplus-0.1.1/example/albert/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-26 10:29:33.000000 transformersplus-0.1.1/example/albert/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    86634 2023-06-26 10:29:33.000000 transformersplus-0.1.1/example/albert/image.png
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-26 10:29:33.000000 transformersplus-0.1.1/example/albert/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 10:29:33.000000 transformersplus-0.1.1/example/albert/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-26 10:29:33.000000 transformersplus-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 10:29:49.066514 transformersplus-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.062513 transformersplus-0.1.1/transformersplus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.066514 transformersplus-0.1.1/transformersplus/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.066514 transformersplus-0.1.1/transformersplus/models/bright_albert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/models/bright_albert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/models/bright_albert/convert_bright_albert_origin_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    61119 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/models/bright_albert/modeling_bright_albert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.066514 transformersplus-0.1.1/transformersplus/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/utils/triton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.066514 transformersplus-0.1.1/transformersplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-26 10:29:48.000000 transformersplus-0.1.1/transformersplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-26 10:29:49.000000 transformersplus-0.1.1/transformersplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:29:48.000000 transformersplus-0.1.1/transformersplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 10:29:48.000000 transformersplus-0.1.1/transformersplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 10:29:48.000000 transformersplus-0.1.1/transformersplus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:40:01.821791 transformersplus-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-12 10:39:51.000000 transformersplus-0.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:40:01.817791 transformersplus-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:40:01.817791 transformersplus-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-12 10:39:51.000000 transformersplus-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-12 10:39:51.000000 transformersplus-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-07-12 10:39:51.000000 transformersplus-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-12 10:40:01.821791 transformersplus-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-12 10:39:51.000000 transformersplus-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:40:01.817791 transformersplus-0.2.0/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:40:01.817791 transformersplus-0.2.0/example/albert_masklm/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-12 10:39:51.000000 transformersplus-0.2.0/example/albert_masklm/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-12 10:39:51.000000 transformersplus-0.2.0/example/albert_masklm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-12 10:39:51.000000 transformersplus-0.2.0/example/albert_masklm/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86634 2023-07-12 10:39:51.000000 transformersplus-0.2.0/example/albert_masklm/image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-12 10:39:51.000000 transformersplus-0.2.0/example/albert_masklm/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 10:39:51.000000 transformersplus-0.2.0/example/albert_masklm/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-12 10:39:51.000000 transformersplus-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 10:40:01.821791 transformersplus-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:40:01.817791 transformersplus-0.2.0/transformersplus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:39:51.000000 transformersplus-0.2.0/transformersplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 10:39:51.000000 transformersplus-0.2.0/transformersplus/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:40:01.821791 transformersplus-0.2.0/transformersplus/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:39:51.000000 transformersplus-0.2.0/transformersplus/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:40:01.821791 transformersplus-0.2.0/transformersplus/models/bright_albert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:39:51.000000 transformersplus-0.2.0/transformersplus/models/bright_albert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-12 10:39:51.000000 transformersplus-0.2.0/transformersplus/models/bright_albert/convert_bright_albert_origin_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61119 2023-07-12 10:39:51.000000 transformersplus-0.2.0/transformersplus/models/bright_albert/modeling_bright_albert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:40:01.821791 transformersplus-0.2.0/transformersplus/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:39:51.000000 transformersplus-0.2.0/transformersplus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-07-12 10:39:51.000000 transformersplus-0.2.0/transformersplus/utils/triton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:40:01.821791 transformersplus-0.2.0/transformersplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-12 10:40:01.000000 transformersplus-0.2.0/transformersplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-12 10:40:01.000000 transformersplus-0.2.0/transformersplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:40:01.000000 transformersplus-0.2.0/transformersplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-12 10:40:01.000000 transformersplus-0.2.0/transformersplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 10:40:01.000000 transformersplus-0.2.0/transformersplus.egg-info/top_level.txt
```

### Comparing `transformersplus-0.1.1/.github/workflows/python-publish.yml` & `transformersplus-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `transformersplus-0.1.1/.gitignore` & `transformersplus-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `transformersplus-0.1.1/LICENSE` & `transformersplus-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transformersplus-0.1.1/PKG-INFO` & `transformersplus-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformersplus
-Version: 0.1.1
+Version: 0.2.0
 Summary: Add Some plus features to transformers.
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/msclock/transformersplus.git
 Project-URL: Source, https://github.com/msclock/transformersplus.git
 Project-URL: Tracker, https://github.com/msclock/transformersplus/issues
 Keywords: machine-learning,deep-learning,transformers,inference,pytorch,vision,nlp
 Classifier: Development Status :: 4 - Beta
```

### Comparing `transformersplus-0.1.1/example/albert/README.md` & `transformersplus-0.2.0/example/albert_masklm/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 ### Prepare model
 
 Generate model of the tritonserver with model_navigator script.
 
 ```bash
 docker run -it --rm --gpus all -v $(pwd):/workspace -w /workspace nvcr.io/nvidia/pytorch:<yy.mm>-py3 bash -c '\
     pip install -U --extra-index-url https://pypi.ngc.nvidia.com triton-model-navigator && \
-    ./optimize.py --max-sequence-length=128 \
+    ./optimize.py \
+        --model-name=albert_masklm \
+        --max-sequence-length=128 \
         --device=0 \
         --model-repository=.model_repository'
 ```
 
 ### Launch server and test locally
 
 Launch tritonserver with the local generated model repository in the folder `.model_repository`.
```

### Comparing `transformersplus-0.1.1/example/albert/app.py` & `transformersplus-0.2.0/example/albert_masklm/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from typing import Mapping
 import gradio as gr
 import torch
-from torch.nn.functional import softmax
 import transformers
 from transformers import AutoTokenizer
 
 
 tokenizer = AutoTokenizer.from_pretrained("uer/albert-base-chinese-cluecorpussmall")
+MAX_LENGTH = 128  # depends on the model
 
 
 def is_triton_url(model_url: str):
     from urllib.parse import urlparse
 
     try:
         url = urlparse(model_url)
@@ -23,32 +24,32 @@
     model: gr.inputs.Dropdown = None,
 ):
     if is_triton_url(model):
         from transformersplus.utils.triton import TritonModel
 
         model_backend = TritonModel(model)
     else:
-        from transformers.models.albert.modeling_albert import AlbertForMaskedLM
+        from transformers import AutoModelForMaskedLM
 
-        model_backend = AlbertForMaskedLM.from_pretrained(model)
+        model_backend = AutoModelForMaskedLM.from_pretrained(model)
 
     inputs = tokenizer(
         [text],
         padding=transformers.utils.PaddingStrategy.MAX_LENGTH,
         truncation=True,
-        max_length=128,
+        max_length=MAX_LENGTH,
         return_tensors=transformers.TensorType.PYTORCH,
     )
     input_ids = inputs["input_ids"][0]
     masked_index = torch.nonzero(
         input_ids == tokenizer.mask_token_id,
         as_tuple=False,
     ).squeeze(-1)
     outputs = model_backend(**inputs)
-    if isinstance(outputs, transformers.modeling_outputs.MaskedLMOutput):
+    if isinstance(outputs, Mapping):
         outputs = outputs["logits"]
     logits = outputs[0, masked_index, :]
     probs = logits.softmax(dim=-1)
     values, predictions = probs.topk(6)
     results = [
         [(tokenizer.decode([p]), v) for v, p in zip(_values, _predictions)]
         for _values, _predictions in zip(values.tolist(), predictions.tolist())
```

### Comparing `transformersplus-0.1.1/example/albert/image.png` & `transformersplus-0.2.0/example/albert_masklm/image.png`

 * *Files identical despite different names*

### Comparing `transformersplus-0.1.1/example/albert/optimize.py` & `transformersplus-0.2.0/example/albert_masklm/optimize.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,58 @@
 #!/usr/bin/env python3
 
-import math
 import os
 
 # https://stackoverflow.com/questions/62691279/how-to-disable-tokenizers-parallelism-true-false-warning
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
 import argparse
 import itertools
 import pathlib
+import string
 
 import numpy as np
-from datasets import load_dataset
-from torch.utils.data import DataLoader
-from transformers import AutoConfig, AutoTokenizer, DataCollatorWithPadding, TensorType
-from transformers.models.albert.configuration_albert import AlbertOnnxConfig
-from transformers.models.albert.modeling_albert import AlbertForMaskedLM
-
+from transformers import AutoTokenizer, TensorType
+from transformers.utils import PaddingStrategy
+from transformers import AutoModelForMaskedLM
+from transformers.onnx.features import FeaturesManager
 import model_navigator as nav
 
 
 def get_model(model_name: str):
-    model = AlbertForMaskedLM.from_pretrained(model_name)
-    model.config.return_dict = True
+    model = AutoModelForMaskedLM.from_pretrained(model_name)
+    model.config.return_dict = False  # return one value from the inference method
     return model
 
 
 def get_dataloader(
     model_name: str,
-    dataset_name: str,
-    max_batch_size: int,
-    num_samples: int,
     max_sequence_length: int,
 ):
     tokenizer = AutoTokenizer.from_pretrained(model_name)
     if max_sequence_length == -1:
         max_sequence_length = getattr(tokenizer, "model_max_length", 512)
 
-    model_config = AutoConfig.from_pretrained(model_name)
-    onnx_config = AlbertOnnxConfig(model_config)
-    input_names = tuple(onnx_config.inputs.keys())
-    dataset = load_dataset(dataset_name)["train"]
+    if max_sequence_length > 512:
+        max_sequence_length = 512
 
-    def preprocess_function(examples):
-        return tokenizer(
-            examples["content"], truncation=True, max_length=max_sequence_length
-        )
+    num_samples = 10
 
-    tokenized_dataset = dataset.map(preprocess_function, batched=True)
-    tokenized_dataset = tokenized_dataset.remove_columns(
-        [c for c in tokenized_dataset.column_names if c not in input_names]
-    )
-    dataloader = DataLoader(
-        tokenized_dataset,
-        batch_size=max_batch_size,
-        collate_fn=DataCollatorWithPadding(
-            tokenizer=tokenizer,
-            padding=True,
+    return [
+        tokenizer(
+            "".join(
+                np.random.choice(list(string.ascii_letters + string.digits), size=32)
+            ),
+            padding=PaddingStrategy.MAX_LENGTH,
+            truncation=True,
             max_length=max_sequence_length,
             return_tensors=TensorType.PYTORCH,
-        ),
-    )
-
-    return [sample for sample, _ in zip(dataloader, range(num_samples))]
+        )
+        for _ in range(num_samples)
+    ]
 
 
 def get_verify_function():
     def verify_func(ys_runner, ys_expected):
         """Verify that at least 99% max probability tokens match on any given batch."""
         for y_runner, y_expected in zip(ys_runner, ys_expected):
             if not all(
@@ -75,38 +61,28 @@
             ):
                 return False
         return True
 
     return verify_func
 
 
-def get_profiler_config(FLAGS):
-    return nav.torch.ProfilerConfig(
-        run_profiling=True,
-        batch_sizes=[
-            1,
-            math.ceil(FLAGS.batch_size / 2),
-            FLAGS.batch_size,
-        ],
-        measurement_mode=nav.MeasurementMode.TIME_WINDOWS,
-        measurement_interval=2500,  # ms
-        measurement_request_count=10,
-        stability_percentage=15,
-        max_trials=5,
-        throughput_cutoff_threshold=0.1,
-    )
-
-
 def get_configuration(
     model_name: str,
     batch_size: int,
     max_sequence_length: int,
 ):
-    model_config = AutoConfig.from_pretrained(model_name)
-    onnx_config = AlbertOnnxConfig(model_config)
+    model = FeaturesManager.get_model_from_feature(
+        model=model_name,
+        feature="masked-lm",
+    )
+    _, model_onnx_config = FeaturesManager.check_supported_model_or_raise(
+        model=model,
+        feature="masked-lm",
+    )
+    onnx_config = model_onnx_config(model.config)
     input_names = tuple(onnx_config.inputs.keys())
     output_names = tuple(onnx_config.outputs.keys())
     dynamic_axes = {
         name: axes
         for name, axes in itertools.chain(
             onnx_config.inputs.items(),
             onnx_config.outputs.items(),
@@ -115,22 +91,34 @@
     opset = onnx_config.default_onnx_opset
 
     tensorrt_profile = nav.TensorRTProfile()
     for k in input_names:
         tensorrt_profile.add(
             k,
             (1, max_sequence_length),
-            (math.ceil(batch_size / 2), max_sequence_length),
+            (1, max_sequence_length),
             (batch_size, max_sequence_length),
         )
 
+    optimization_profile = nav.OptimizationProfile(
+        max_batch_size=batch_size,
+        batch_sizes=[
+            1,
+            batch_size,
+        ],
+        stability_percentage=15,
+        max_trials=5,
+        throughput_cutoff_threshold=0.1,
+    )
+
     configuration = {
         "input_names": input_names,
         "output_names": output_names,
         "sample_count": 10,
+        "optimization_profile": optimization_profile,
         "custom_configs": [
             nav.TorchConfig(
                 jit_type=nav.JitType.TRACE,
                 strict=False,
             ),
             nav.OnnxConfig(
                 opset=opset,
@@ -172,67 +160,54 @@
         default=4,
         help="batch size on model",
     )
     parser.add_argument(
         "--max-sequence-length",
         type=int,
         default=-1,
-        help="max input text sequence length on model",
+        help="max input text sequence length on model, up to 512",
     )
     parser.add_argument(
         "--device",
         type=str,
         default="cpu",
         help="device = None or 'cpu' or 0 or '0' or '0,1,2,3'",
     )
     parser.add_argument(
-        "--min-top1-accuracy",
-        type=float,
-        default=0.9,
-    )
-    parser.add_argument(
         "--model-repository",
         type=str,
         default=f".model_repository",
         help="model repository folder serving on tirton",
     )
     return parser.parse_args()
 
 
 def main(FLAGS):
-    dataset_name = "madao33/new-title-chinese"
-    num_samples = 10
-
     model = get_model(FLAGS.input_model)
     dataloader = get_dataloader(
         model_name=FLAGS.input_model,
-        dataset_name=dataset_name,
-        max_batch_size=FLAGS.batch_size,
-        num_samples=num_samples,
         max_sequence_length=FLAGS.max_sequence_length,
     )
     verify_func = get_verify_function()
-    profiler_config = get_profiler_config(FLAGS)
     configuration = get_configuration(
         model_name=FLAGS.input_model,
         batch_size=FLAGS.batch_size,
         max_sequence_length=FLAGS.max_sequence_length,
     )
 
     package = nav.torch.optimize(
         model=model,
         dataloader=dataloader,
-        # verify_func=verify_func,
+        verify_func=verify_func,
         target_device=nav.DeviceKind.CPU
         if str(FLAGS.device) == "cpu"
         else nav.DeviceKind.CUDA,
         debug=True,
         verbose=True,
         workspace=pathlib.Path(FLAGS.workspace) / FLAGS.model_name,
-        profiler_config=profiler_config,
         **configuration,
     )
 
     import shutil
 
     shutil.rmtree(
         pathlib.Path(FLAGS.model_repository) / FLAGS.model_name,
```

### Comparing `transformersplus-0.1.1/pyproject.toml` & `transformersplus-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `transformersplus-0.1.1/transformersplus/models/bright_albert/convert_bright_albert_origin_tf_checkpoint_to_pytorch.py` & `transformersplus-0.2.0/transformersplus/models/bright_albert/convert_bright_albert_origin_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformersplus-0.1.1/transformersplus/models/bright_albert/modeling_bright_albert.py` & `transformersplus-0.2.0/transformersplus/models/bright_albert/modeling_bright_albert.py`

 * *Files identical despite different names*

### Comparing `transformersplus-0.1.1/transformersplus/utils/triton.py` & `transformersplus-0.2.0/transformersplus/utils/triton.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,26 +48,32 @@
         self._create_input_placeholders_fn = create_input_placeholders
 
     @property
     def runtime(self):
         """Returns the model runtime"""
         return self.metadata.get("backend", self.metadata.get("platform"))
 
-    def __call__(self, *args, **kwargs) -> typing.Union[torch.Tensor, typing.Tuple[torch.Tensor, ...]]:
+    def __call__(self, *args, **kwargs) -> typing.Union[torch.Tensor, typing.Tuple[torch.Tensor, ...], typing.Mapping]:
         """Invokes the model. Parameters can be provided via args or kwargs.
         args, if provided, are assumed to match the order of inputs of the model.
         kwargs are matched with the model input names.
         """
         inputs = self._create_inputs(*args, **kwargs)
         response = self.client.infer(model_name=self.model_name, inputs=inputs)
-        result = []
+
+        if len(self.metadata["outputs"]) == 1:
+            output = self.metadata["outputs"][0]
+            return torch.as_tensor(response.as_numpy(output["name"]))
+
+        result = {}
         for output in self.metadata["outputs"]:
             tensor = torch.as_tensor(response.as_numpy(output["name"]))
-            result.append(tensor)
-        return result[0] if len(result) == 1 else result
+            result[output["name"]] = tensor
+
+        return result
 
     def _create_inputs(self, *args, **kwargs):
         args_len, kwargs_len = len(args), len(kwargs)
         if not args_len and not kwargs_len:
             raise RuntimeError("No inputs provided.")
         if args_len and kwargs_len:
             raise RuntimeError("Cannot specify args and kwargs at the same time")
@@ -102,13 +108,11 @@
 
 
 class TritonModel(torch.nn.Module):
     base_model_prefix = "triton"
 
     def __init__(self, url) -> None:
         super().__init__()
-        from transformersplus.utils.triton import TritonModelClient
-
         self.model = TritonModelClient(model_url=url)
 
     def forward(self, *input, **kwargs):
         return self.model(*input, **kwargs)
```

### Comparing `transformersplus-0.1.1/transformersplus.egg-info/PKG-INFO` & `transformersplus-0.2.0/transformersplus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformersplus
-Version: 0.1.1
+Version: 0.2.0
 Summary: Add Some plus features to transformers.
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/msclock/transformersplus.git
 Project-URL: Source, https://github.com/msclock/transformersplus.git
 Project-URL: Tracker, https://github.com/msclock/transformersplus/issues
 Keywords: machine-learning,deep-learning,transformers,inference,pytorch,vision,nlp
 Classifier: Development Status :: 4 - Beta
```

### Comparing `transformersplus-0.1.1/transformersplus.egg-info/SOURCES.txt` & `transformersplus-0.2.0/transformersplus.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 .gitattributes
 .gitignore
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/python-publish.yml
-example/albert/.gitignore
-example/albert/README.md
-example/albert/app.py
-example/albert/image.png
-example/albert/optimize.py
-example/albert/requirements.txt
+example/albert_masklm/.gitignore
+example/albert_masklm/README.md
+example/albert_masklm/app.py
+example/albert_masklm/image.png
+example/albert_masklm/optimize.py
+example/albert_masklm/requirements.txt
 transformersplus/__init__.py
 transformersplus/__version__.py
 transformersplus.egg-info/PKG-INFO
 transformersplus.egg-info/SOURCES.txt
 transformersplus.egg-info/dependency_links.txt
 transformersplus.egg-info/requires.txt
 transformersplus.egg-info/top_level.txt
```


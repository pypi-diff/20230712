# Comparing `tmp/sihl-0.0.3.dev2.tar.gz` & `tmp/sihl-0.0.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sihl-0.0.3.dev2.tar", max compression
+gzip compressed data, was "sihl-0.0.3.dev3.tar", max compression
```

## Comparing `sihl-0.0.3.dev2.tar` & `sihl-0.0.3.dev3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-07-10 16:34:51.026986 sihl-0.0.3.dev2/LICENSE
--rw-r--r--   0        0        0      894 2023-07-10 16:34:51.026986 sihl-0.0.3.dev2/README.md
--rw-r--r--   0        0        0     1545 2023-07-10 16:35:05.995172 sihl-0.0.3.dev2/pyproject.toml
--rw-r--r--   0        0        0      288 2023-07-10 16:35:05.995172 sihl-0.0.3.dev2/src/sihl/__init__.py
--rw-r--r--   0        0        0   402648 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/heads/NotoSansMono-Bold.ttf
--rw-r--r--   0        0        0      233 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/heads/__init__.py
--rw-r--r--   0        0        0     3154 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/heads/binary_classification.py
--rw-r--r--   0        0        0     3768 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/heads/multiclass_classification.py
--rw-r--r--   0        0        0     4624 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/heads/multilabel_classification.py
--rw-r--r--   0        0        0        0 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/layers/__init__.py
--rw-r--r--   0        0        0     4573 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/lightning_module.py
--rw-r--r--   0        0        0      549 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/sihl_model.py
--rw-r--r--   0        0        0     2797 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/timm_backbone.py
--rw-r--r--   0        0        0     6460 2023-07-10 16:35:05.995172 sihl-0.0.3.dev2/src/sihl/torchvision_backbone.py
--rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 sihl-0.0.3.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-12 10:41:30.903222 sihl-0.0.3.dev3/LICENSE
+-rw-r--r--   0        0        0      894 2023-07-12 10:41:30.903222 sihl-0.0.3.dev3/README.md
+-rw-r--r--   0        0        0     1545 2023-07-12 10:41:47.839418 sihl-0.0.3.dev3/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-07-12 10:41:30.907222 sihl-0.0.3.dev3/src/sihl/__init__.py
+-rw-r--r--   0        0        0   402648 2023-07-12 10:41:30.907222 sihl-0.0.3.dev3/src/sihl/heads/NotoSansMono-Bold.ttf
+-rw-r--r--   0        0        0      233 2023-07-12 10:41:30.911222 sihl-0.0.3.dev3/src/sihl/heads/__init__.py
+-rw-r--r--   0        0        0     3147 2023-07-12 10:41:47.839418 sihl-0.0.3.dev3/src/sihl/heads/binary_classification.py
+-rw-r--r--   0        0        0     3828 2023-07-12 10:41:47.839418 sihl-0.0.3.dev3/src/sihl/heads/multiclass_classification.py
+-rw-r--r--   0        0        0     4684 2023-07-12 10:41:47.839418 sihl-0.0.3.dev3/src/sihl/heads/multilabel_classification.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:41:30.911222 sihl-0.0.3.dev3/src/sihl/layers/__init__.py
+-rw-r--r--   0        0        0     4573 2023-07-12 10:41:30.911222 sihl-0.0.3.dev3/src/sihl/lightning_module.py
+-rw-r--r--   0        0        0      549 2023-07-12 10:41:30.911222 sihl-0.0.3.dev3/src/sihl/sihl_model.py
+-rw-r--r--   0        0        0     2797 2023-07-12 10:41:30.911222 sihl-0.0.3.dev3/src/sihl/timm_backbone.py
+-rw-r--r--   0        0        0     6460 2023-07-12 10:41:30.911222 sihl-0.0.3.dev3/src/sihl/torchvision_backbone.py
+-rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 sihl-0.0.3.dev3/PKG-INFO
```

### Comparing `sihl-0.0.3.dev2/LICENSE` & `sihl-0.0.3.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev2/README.md` & `sihl-0.0.3.dev3/README.md`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev2/pyproject.toml` & `sihl-0.0.3.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sihl"
-version = "0.0.3-dev2"
+version = "0.0.3-dev3"
 description = "Simple Image Heads and Layers"
 authors = ["jonregef <jon.regef@pm.me>"]
 readme = "README.md"
 license = "MIT"
 # homepage = "https://github.com/sihlAI/sihl"
 # repository = "https://github.com/sihlAI/sihl"
```

### Comparing `sihl-0.0.3.dev2/src/sihl/heads/NotoSansMono-Bold.ttf` & `sihl-0.0.3.dev3/src/sihl/heads/NotoSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev2/src/sihl/heads/binary_classification.py` & `sihl-0.0.3.dev3/src/sihl/heads/binary_classification.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,33 +27,33 @@
         scores = torch.sigmoid(self.net(inputs[self.level])).squeeze(-1)
         return scores, scores > 0.5
 
     def training_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
         logits = self.net(inputs[self.level]).squeeze(-1)
-        targets = labels.to(logits.dtype).to(logits.device)
-        loss = torch.nn.functional.binary_cross_entropy_with_logits(logits, targets)
+        labels = labels.to(logits.dtype).to(logits.device)
+        loss = torch.nn.functional.binary_cross_entropy_with_logits(logits, labels)
         return loss, {}
 
     def on_validation_start(self) -> None:
         self.accuracy_computer = torchmetrics.classification.BinaryAccuracy()
         self.precision_computer = torchmetrics.classification.BinaryPrecision()
         self.recall_computer = torchmetrics.classification.BinaryRecall()
 
     def validation_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
         input = inputs[self.level]
         logits = self.net(input).squeeze(-1)
-        targets = labels.to(logits.dtype).to(logits.device)
-        loss = torch.nn.functional.binary_cross_entropy_with_logits(logits, targets)
-        self.accuracy_computer.to(input.device).update(logits, targets)
-        self.precision_computer.to(input.device).update(logits, targets)
-        self.recall_computer.to(input.device).update(logits, targets)
+        labels = labels.to(logits.dtype).to(logits.device)
+        loss = torch.nn.functional.binary_cross_entropy_with_logits(logits, labels)
+        self.accuracy_computer.to(input.device).update(logits, labels)
+        self.precision_computer.to(input.device).update(logits, labels)
+        self.recall_computer.to(input.device).update(logits, labels)
         return loss, {}
 
     def on_validation_end(self) -> dict[str, float]:
         return {
             "accuracy": self.accuracy_computer.compute().item(),
             "precision": self.precision_computer.compute().item(),
             "recall": self.recall_computer.compute().item(),
```

### Comparing `sihl-0.0.3.dev2/src/sihl/heads/multiclass_classification.py` & `sihl-0.0.3.dev3/src/sihl/heads/multiclass_classification.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     def training_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
         logits = self.net(inputs[self.level])
         loss = torch.nn.functional.cross_entropy(
             logits,
-            labels,
+            labels.to(logits.device),
             weight=self.label_weights,
             label_smoothing=self.label_smoothing,
         )
         return loss, {}
 
     def on_validation_start(self) -> None:
         self.accuracy_computer = MulticlassAccuracy(num_classes=self.num_classes)
@@ -62,14 +62,15 @@
         self.recall_computer = MulticlassRecall(num_classes=self.num_classes)
 
     def validation_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
         input = inputs[self.level]
         logits = self.net(input)
+        labels = labels.to(logits.device)
         loss = torch.nn.functional.cross_entropy(
             logits,
             labels,
             weight=self.label_weights,
             label_smoothing=self.label_smoothing,
         )
         self.accuracy_computer.to(input.device).update(logits, labels)
```

### Comparing `sihl-0.0.3.dev2/src/sihl/heads/multilabel_classification.py` & `sihl-0.0.3.dev3/src/sihl/heads/multilabel_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,28 +43,29 @@
         return scores, classes
 
     def training_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
         logits = self.net(inputs[self.level])
         loss = torch.nn.functional.binary_cross_entropy_with_logits(
-            logits, labels, pos_weight=self.label_weights
+            logits, labels.to(logits.device), pos_weight=self.label_weights
         )
         return loss, {}
 
     def on_validation_start(self) -> None:
         self.accuracy_computer = MultilabelAccuracy(num_labels=self.num_classes)
         self.precision_computer = MultilabelPrecision(num_labels=self.num_classes)
         self.recall_computer = MultilabelRecall(num_labels=self.num_classes)
 
     def validation_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
         input = inputs[self.level]
         logits = self.net(input)
+        labels = labels.to(logits.device)
         loss = torch.nn.functional.binary_cross_entropy_with_logits(
             logits, labels, pos_weight=self.label_weights
         )
         self.accuracy_computer.to(input.device).update(logits, labels)
         self.precision_computer.to(input.device).update(logits, labels)
         self.recall_computer.to(input.device).update(logits, labels)
         return loss, {}
```

### Comparing `sihl-0.0.3.dev2/src/sihl/lightning_module.py` & `sihl-0.0.3.dev3/src/sihl/lightning_module.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev2/src/sihl/sihl_model.py` & `sihl-0.0.3.dev3/src/sihl/sihl_model.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev2/src/sihl/timm_backbone.py` & `sihl-0.0.3.dev3/src/sihl/timm_backbone.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev2/src/sihl/torchvision_backbone.py` & `sihl-0.0.3.dev3/src/sihl/torchvision_backbone.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev2/PKG-INFO` & `sihl-0.0.3.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sihl
-Version: 0.0.3.dev2
+Version: 0.0.3.dev3
 Summary: Simple Image Heads and Layers
 License: MIT
 Author: jonregef
 Author-email: jon.regef@pm.me
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


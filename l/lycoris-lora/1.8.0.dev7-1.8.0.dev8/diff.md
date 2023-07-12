# Comparing `tmp/lycoris_lora-1.8.0.dev7.tar.gz` & `tmp/lycoris_lora-1.8.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-1.8.0.dev7.tar", last modified: Sat Jul  8 09:15:00 2023, max compression
+gzip compressed data, was "lycoris_lora-1.8.0.dev8.tar", last modified: Wed Jul 12 02:39:23 2023, max compression
```

## Comparing `lycoris_lora-1.8.0.dev7.tar` & `lycoris_lora-1.8.0.dev8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 09:15:00.688833 lycoris_lora-1.8.0.dev7/
--rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-1.8.0.dev7/.gitignore
--rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-1.8.0.dev7/Algo.md
--rw-rw-rw-   0        0        0      977 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/Change.md
--rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-1.8.0.dev7/Demo.md
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-1.8.0.dev7/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-07-08 09:15:00.688332 lycoris_lora-1.8.0.dev7/PKG-INFO
--rw-rw-rw-   0        0        0     7677 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 09:15:00.671808 lycoris_lora-1.8.0.dev7/experiments/
--rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-1.8.0.dev7/experiments/better_conv.py
--rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-1.8.0.dev7/experiments/better_conv_extract.py
--rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-1.8.0.dev7/experiments/concept_neuron.py
--rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-1.8.0.dev7/experiments/locon_extract_test.py
--rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-1.8.0.dev7/experiments/locon_merge_test.py
--rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-1.8.0.dev7/experiments/singular_value_test.py
--rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-1.8.0.dev7/experiments/sparse_bias_test.py
--rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-1.8.0.dev7/experiments/time_test.py
--rw-rw-rw-   0        0        0      255 2023-06-25 07:25:35.000000 lycoris_lora-1.8.0.dev7/experiments/weakre_speed.py
-drwxrwxrwx   0        0        0        0 2023-07-08 09:15:00.672308 lycoris_lora-1.8.0.dev7/lycoris/
--rw-rw-rw-   0        0        0        0 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 09:15:00.672808 lycoris_lora-1.8.0.dev7/lycoris/kohya/
--rw-rw-rw-   0        0        0    24690 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/kohya/__init__.py
--rw-rw-rw-   0        0        0    48868 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/kohya/kohya_model_utils.py
--rw-rw-rw-   0        0        0     1512 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/kohya/kohya_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 09:15:00.676312 lycoris_lora-1.8.0.dev7/lycoris/modules/
--rw-rw-rw-   0        0        0        0 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/__init__.py
--rw-rw-rw-   0        0        0     4762 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/dylora.py
--rw-rw-rw-   0        0        0    10763 2023-07-06 08:19:32.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/glokr.py
--rw-rw-rw-   0        0        0     4117 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/glora.py
--rw-rw-rw-   0        0        0     2103 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/ia3.py
--rw-rw-rw-   0        0        0     4468 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/locon.py
--rw-rw-rw-   0        0        0     8830 2023-07-08 06:50:22.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/loha.py
--rw-rw-rw-   0        0        0    10896 2023-07-08 09:14:16.000000 lycoris_lora-1.8.0.dev7/lycoris/modules/lokr.py
--rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-1.8.0.dev7/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 09:15:00.687327 lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-07-08 09:15:00.000000 lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      940 2023-07-08 09:15:00.000000 lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 09:15:00.000000 lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-07-08 09:15:00.000000 lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-08 09:15:00.000000 lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       58 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 09:15:00.688833 lycoris_lora-1.8.0.dev7/setup.cfg
--rw-rw-rw-   0        0        0      566 2023-07-08 09:14:44.000000 lycoris_lora-1.8.0.dev7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 09:15:00.688332 lycoris_lora-1.8.0.dev7/tools/
--rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-1.8.0.dev7/tools/extract_locon.py
--rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-1.8.0.dev7/tools/merge.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:39:23.230827 lycoris_lora-1.8.0.dev8/
+-rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-1.8.0.dev8/.gitignore
+-rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-1.8.0.dev8/Algo.md
+-rw-rw-rw-   0        0        0      977 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev8/Change.md
+-rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-1.8.0.dev8/Demo.md
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-1.8.0.dev8/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-07-12 02:39:23.230327 lycoris_lora-1.8.0.dev8/PKG-INFO
+-rw-rw-rw-   0        0        0     7677 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 02:39:23.198327 lycoris_lora-1.8.0.dev8/experiments/
+-rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-1.8.0.dev8/experiments/better_conv.py
+-rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-1.8.0.dev8/experiments/better_conv_extract.py
+-rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-1.8.0.dev8/experiments/concept_neuron.py
+-rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-1.8.0.dev8/experiments/locon_extract_test.py
+-rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-1.8.0.dev8/experiments/locon_merge_test.py
+-rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-1.8.0.dev8/experiments/singular_value_test.py
+-rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-1.8.0.dev8/experiments/sparse_bias_test.py
+-rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-1.8.0.dev8/experiments/time_test.py
+-rw-rw-rw-   0        0        0      255 2023-06-25 07:25:35.000000 lycoris_lora-1.8.0.dev8/experiments/weakre_speed.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:39:23.199827 lycoris_lora-1.8.0.dev8/lycoris/
+-rw-rw-rw-   0        0        0        0 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev8/lycoris/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:39:23.202328 lycoris_lora-1.8.0.dev8/lycoris/kohya/
+-rw-rw-rw-   0        0        0    24690 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev8/lycoris/kohya/__init__.py
+-rw-rw-rw-   0        0        0    48868 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev8/lycoris/kohya/kohya_model_utils.py
+-rw-rw-rw-   0        0        0     1512 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev8/lycoris/kohya/kohya_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:39:23.213827 lycoris_lora-1.8.0.dev8/lycoris/modules/
+-rw-rw-rw-   0        0        0        0 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev8/lycoris/modules/__init__.py
+-rw-rw-rw-   0        0        0     4762 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev8/lycoris/modules/dylora.py
+-rw-rw-rw-   0        0        0    10763 2023-07-06 08:19:32.000000 lycoris_lora-1.8.0.dev8/lycoris/modules/glokr.py
+-rw-rw-rw-   0        0        0     4117 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev8/lycoris/modules/glora.py
+-rw-rw-rw-   0        0        0     2103 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev8/lycoris/modules/ia3.py
+-rw-rw-rw-   0        0        0     5542 2023-07-12 02:38:34.000000 lycoris_lora-1.8.0.dev8/lycoris/modules/locon.py
+-rw-rw-rw-   0        0        0     8830 2023-07-08 06:50:22.000000 lycoris_lora-1.8.0.dev8/lycoris/modules/loha.py
+-rw-rw-rw-   0        0        0    10896 2023-07-08 09:14:16.000000 lycoris_lora-1.8.0.dev8/lycoris/modules/lokr.py
+-rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-1.8.0.dev8/lycoris/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:39:23.228327 lycoris_lora-1.8.0.dev8/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-07-12 02:39:22.000000 lycoris_lora-1.8.0.dev8/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      940 2023-07-12 02:39:23.000000 lycoris_lora-1.8.0.dev8/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 02:39:22.000000 lycoris_lora-1.8.0.dev8/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-1.8.0.dev8/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-07-12 02:39:22.000000 lycoris_lora-1.8.0.dev8/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-12 02:39:22.000000 lycoris_lora-1.8.0.dev8/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       58 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 02:39:23.230827 lycoris_lora-1.8.0.dev8/setup.cfg
+-rw-rw-rw-   0        0        0      566 2023-07-12 02:39:13.000000 lycoris_lora-1.8.0.dev8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:39:23.229827 lycoris_lora-1.8.0.dev8/tools/
+-rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-1.8.0.dev8/tools/extract_locon.py
+-rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-1.8.0.dev8/tools/merge.py
```

### Comparing `lycoris_lora-1.8.0.dev7/.gitignore` & `lycoris_lora-1.8.0.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/Algo.md` & `lycoris_lora-1.8.0.dev8/Algo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/Change.md` & `lycoris_lora-1.8.0.dev8/Change.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/Demo.md` & `lycoris_lora-1.8.0.dev8/Demo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/LICENSE.md` & `lycoris_lora-1.8.0.dev8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/README.md` & `lycoris_lora-1.8.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/experiments/better_conv.py` & `lycoris_lora-1.8.0.dev8/experiments/better_conv.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/experiments/better_conv_extract.py` & `lycoris_lora-1.8.0.dev8/experiments/better_conv_extract.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/experiments/concept_neuron.py` & `lycoris_lora-1.8.0.dev8/experiments/concept_neuron.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/experiments/locon_extract_test.py` & `lycoris_lora-1.8.0.dev8/experiments/locon_extract_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/experiments/locon_merge_test.py` & `lycoris_lora-1.8.0.dev8/experiments/locon_merge_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/experiments/singular_value_test.py` & `lycoris_lora-1.8.0.dev8/experiments/singular_value_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/experiments/sparse_bias_test.py` & `lycoris_lora-1.8.0.dev8/experiments/sparse_bias_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/experiments/time_test.py` & `lycoris_lora-1.8.0.dev8/experiments/time_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/lycoris/kohya/__init__.py` & `lycoris_lora-1.8.0.dev8/lycoris/kohya/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/lycoris/kohya/kohya_model_utils.py` & `lycoris_lora-1.8.0.dev8/lycoris/kohya/kohya_model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/lycoris/kohya/kohya_utils.py` & `lycoris_lora-1.8.0.dev8/lycoris/kohya/kohya_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/lycoris/modules/dylora.py` & `lycoris_lora-1.8.0.dev8/lycoris/modules/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/lycoris/modules/glokr.py` & `lycoris_lora-1.8.0.dev8/lycoris/modules/glokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/lycoris/modules/glora.py` & `lycoris_lora-1.8.0.dev8/lycoris/modules/glora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/lycoris/modules/ia3.py` & `lycoris_lora-1.8.0.dev8/lycoris/modules/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/lycoris/modules/locon.py` & `lycoris_lora-1.8.0.dev8/lycoris/modules/locon.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import math
 from weakref import ref
+from collections import OrderedDict, abc as container_abcs
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 
 class LoConModule(nn.Module):
@@ -22,14 +23,15 @@
     ):
         """ if alpha == 0 or None, alpha is rank (no scaling). """
         super().__init__()
         self.lora_name = lora_name
         self.lora_dim = lora_dim
         self.cp = False
 
+        self.scalar = nn.Parameter(torch.tensor(0.0))
         if isinstance(org_module, nn.Conv2d):
             # For general LoCon
             in_dim = org_module.in_channels
             k_size = org_module.kernel_size
             stride = org_module.stride
             padding = org_module.padding
             out_dim = org_module.out_channels
@@ -60,44 +62,66 @@
             alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
         alpha = lora_dim if alpha is None or alpha == 0 else alpha
         self.scale = alpha / self.lora_dim
         self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
 
         # same as microsoft's
         torch.nn.init.kaiming_uniform_(self.lora_down.weight, a=math.sqrt(5))
-        torch.nn.init.zeros_(self.lora_up.weight)
+        torch.nn.init.kaiming_uniform_(self.lora_up.weight)
         if self.cp:
             torch.nn.init.kaiming_uniform_(self.lora_mid.weight, a=math.sqrt(5))
 
         self.multiplier = multiplier
         self.org_module = [org_module]
 
     def apply_to(self):
         self.org_forward = self.org_module[0].forward
         self.org_module[0].forward = self.forward
 
     def make_weight(self, device=None):
         wa = self.lora_up.weight.to(device)
         wb = self.lora_down.weight.to(device)
-        return (wa.view(wa.size(0), -1) @ wb.view(wb.size(0), -1)).view(self.shape)
+        return (wa.view(wa.size(0), -1) @ wb.view(wb.size(0), -1)).view(self.shape) * self.scalar
+    
+    def state_dict(self, *args, destination=None, prefix='', keep_vars=False):
+        # TODO: Remove `args` and the parsing logic when BC allows.
+        if len(args) > 0:
+            if destination is None:
+                destination = args[0]
+            if len(args) > 1 and prefix == '':
+                prefix = args[1]
+            if len(args) > 2 and keep_vars is False:
+                keep_vars = args[2]
+            # DeprecationWarning is ignored by default
+
+        if destination is None:
+            destination = OrderedDict()
+            destination._metadata = OrderedDict()
+
+        local_metadata = dict(version=self._version)
+        if hasattr(destination, "_metadata"):
+            destination._metadata[prefix[:-1]] = local_metadata
+
+        destination[f'{prefix}alpha'] = self.alpha
+        destination[f'{prefix}lora_up.weight'] = self.lora_up.weight * self.scalar
+        destination[f'{prefix}lora_down.weight'] = self.lora_down.weight
+        if self.cp:
+            destination[f'{prefix}lora_mid.weight'] = self.lora_mid.weight
+        return destination
 
     @torch.no_grad()
     def apply_max_norm(self, max_norm, device=None):
         orig_norm = self.make_weight(device).norm()*self.scale
         norm = torch.clamp(orig_norm, max_norm/2)
         desired = torch.clamp(norm, max=max_norm)
         ratio = desired.cpu()/norm.cpu()
         
         scaled = ratio.item() != 1.0
         if scaled:
-            modules = self.cp + 2
-            self.lora_up.weight *= ratio**(1/modules)
-            self.lora_down.weight *= ratio**(1/modules)
-            if self.cp:
-                self.lora_mid.weight *= ratio**(1/modules)
+            self.scalar *= ratio
         
         return scaled, orig_norm*ratio
 
     def forward(self, x):
         if self.module_dropout and self.training:
             if torch.rand(1) < self.module_dropout:
                 return self.org_forward(x)
@@ -111,8 +135,8 @@
             drop = torch.rand(self.lora_dim, device=mid.device) < self.rank_dropout
             if (dims:=len(x.shape)) == 4:
                 drop = drop.view(1, -1, 1, 1)
             else:
                 drop = drop.view(*[1]*(dims-1), -1)
             mid = mid * drop
         
-        return self.org_forward(x) + self.dropout(self.lora_up(mid) * scale)
+        return self.org_forward(x) + self.dropout(self.lora_up(mid) * self.scalar * scale)
```

### Comparing `lycoris_lora-1.8.0.dev7/lycoris/modules/loha.py` & `lycoris_lora-1.8.0.dev8/lycoris/modules/loha.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/lycoris/modules/lokr.py` & `lycoris_lora-1.8.0.dev8/lycoris/modules/lokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/lycoris/utils.py` & `lycoris_lora-1.8.0.dev8/lycoris/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-1.8.0.dev8/lycoris_lora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/setup.py` & `lycoris_lora-1.8.0.dev8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lycoris_lora',
     packages=find_packages(),
-    version='1.8.0.dev7',
+    version='1.8.0.dev8',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

### Comparing `lycoris_lora-1.8.0.dev7/tools/extract_locon.py` & `lycoris_lora-1.8.0.dev8/tools/extract_locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev7/tools/merge.py` & `lycoris_lora-1.8.0.dev8/tools/merge.py`

 * *Files identical despite different names*


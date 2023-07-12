# Comparing `tmp/equiformer-pytorch-0.3.0.tar.gz` & `tmp/equiformer-pytorch-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equiformer-pytorch-0.3.0.tar", last modified: Wed Jul 12 17:42:57 2023, max compression
+gzip compressed data, was "equiformer-pytorch-0.3.1.tar", last modified: Wed Jul 12 18:17:21 2023, max compression
```

## Comparing `equiformer-pytorch-0.3.0.tar` & `equiformer-pytorch-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:42:57.236089 equiformer-pytorch-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-12 17:41:05.000000 equiformer-pytorch-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 17:41:05.000000 equiformer-pytorch-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-12 17:42:57.236089 equiformer-pytorch-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-07-12 17:41:05.000000 equiformer-pytorch-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:42:57.172089 equiformer-pytorch-0.3.0/equiformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-12 17:41:05.000000 equiformer-pytorch-0.3.0/equiformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-12 17:41:05.000000 equiformer-pytorch-0.3.0/equiformer_pytorch/basis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:42:57.172089 equiformer-pytorch-0.3.0/equiformer_pytorch/data/
--rw-r--r--   0 runner    (1001) docker     (123) 36766718 2023-07-12 17:41:05.000000 equiformer-pytorch-0.3.0/equiformer_pytorch/data/J_dense.pt
--rw-r--r--   0 runner    (1001) docker     (123)    35400 2023-07-12 17:41:05.000000 equiformer-pytorch-0.3.0/equiformer_pytorch/equiformer_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-12 17:41:05.000000 equiformer-pytorch-0.3.0/equiformer_pytorch/irr_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-07-12 17:41:05.000000 equiformer-pytorch-0.3.0/equiformer_pytorch/reversible.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-12 17:41:05.000000 equiformer-pytorch-0.3.0/equiformer_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 17:41:05.000000 equiformer-pytorch-0.3.0/equiformer_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:42:57.172089 equiformer-pytorch-0.3.0/equiformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-12 17:42:57.000000 equiformer-pytorch-0.3.0/equiformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-12 17:42:57.000000 equiformer-pytorch-0.3.0/equiformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:42:57.000000 equiformer-pytorch-0.3.0/equiformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 17:42:57.000000 equiformer-pytorch-0.3.0/equiformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:42:57.000000 equiformer-pytorch-0.3.0/equiformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 17:42:57.236089 equiformer-pytorch-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-12 17:41:05.000000 equiformer-pytorch-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:17:21.590266 equiformer-pytorch-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-12 18:17:21.590266 equiformer-pytorch-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:17:21.518267 equiformer-pytorch-0.3.1/equiformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/basis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:17:21.518267 equiformer-pytorch-0.3.1/equiformer_pytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 36766718 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/data/J_dense.pt
+-rw-r--r--   0 runner    (1001) docker     (123)    35782 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/equiformer_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/irr_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/reversible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:17:21.518267 equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-12 18:17:21.000000 equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-12 18:17:21.000000 equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:17:21.000000 equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 18:17:21.000000 equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 18:17:21.000000 equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 18:17:21.590266 equiformer-pytorch-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/setup.py
```

### Comparing `equiformer-pytorch-0.3.0/LICENSE` & `equiformer-pytorch-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `equiformer-pytorch-0.3.0/PKG-INFO` & `equiformer-pytorch-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equiformer-pytorch
-Version: 0.3.0
+Version: 0.3.1
 Summary: Equiformer - SE3/E3 Graph Attention Transformer for Molecules and Proteins
 Home-page: https://github.com/lucidrains/equiformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,equivariance,molecules,proteins
 Classifier: Development Status :: 4 - Beta
```

### Comparing `equiformer-pytorch-0.3.0/README.md` & `equiformer-pytorch-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 out = model(feats, coors, mask) # (1, 128)
 
 out.type0 # invariant type 0    - (1, 128)
 out.type1 # equivariant type 1  - (1, 128, 3)
 ```
 
-This repository also includes a way to decouple memory usage from depth using <a href="https://arxiv.org/abs/1707.04585">reversible networks</a>. In other words, memory usage is completely decoupled from depth
+This repository also includes a way to decouple memory usage from depth using <a href="https://arxiv.org/abs/1707.04585">reversible networks</a>. In other words, if you increase depth, the memory cost will stay constant at the usage of one equiformer transformer block (attention and feedforward).
 
 ```python
 import torch
 from equiformer_pytorch import Equiformer
 
 model = Equiformer(
     num_tokens = 24,
```

#### html2text {}

```diff
@@ -27,24 +27,25 @@
 True, # whether to reduce out to dimension of 1, say for predicting new
 coordinates for type 1 features l2_dist_attention = False # set to False to try
 out MLP attention ).cuda() feats = torch.randint(0, 24, (1, 128)).cuda() coors
 = torch.randn(1, 128, 3).cuda() mask = torch.ones(1, 128).bool().cuda() out =
 model(feats, coors, mask) # (1, 128) out.type0 # invariant type 0 - (1, 128)
 out.type1 # equivariant type 1 - (1, 128, 3) ``` This repository also includes
 a way to decouple memory usage from depth using reversible_networks. In other
-words, memory usage is completely decoupled from depth ```python import torch
-from equiformer_pytorch import Equiformer model = Equiformer( num_tokens = 24,
-dim = (4, 4, 2), dim_head = (4, 4, 4), heads = (2, 2, 2), num_degrees = 3,
-depth = 48, # depth of 48 - just to show that it runs - in reality, seems to be
-quite unstable at higher depths, so architecture stil needs more work
-reversible = True, # just set this to True to use https://arxiv.org/abs/
-1707.04585 ).cuda() feats = torch.randint(0, 24, (1, 128)).cuda() coors =
-torch.randn(1, 128, 3).cuda() mask = torch.ones(1, 128).bool().cuda() out =
-model(feats, coors, mask) out.type0.sum().backward() ``` ## Appreciation -
-StabilityAI for the generous sponsorship, as well as my other sponsors out
+words, if you increase depth, the memory cost will stay constant at the usage
+of one equiformer transformer block (attention and feedforward). ```python
+import torch from equiformer_pytorch import Equiformer model = Equiformer
+( num_tokens = 24, dim = (4, 4, 2), dim_head = (4, 4, 4), heads = (2, 2, 2),
+num_degrees = 3, depth = 48, # depth of 48 - just to show that it runs - in
+reality, seems to be quite unstable at higher depths, so architecture stil
+needs more work reversible = True, # just set this to True to use https://
+arxiv.org/abs/1707.04585 ).cuda() feats = torch.randint(0, 24, (1, 128)).cuda()
+coors = torch.randn(1, 128, 3).cuda() mask = torch.ones(1, 128).bool().cuda()
+out = model(feats, coors, mask) out.type0.sum().backward() ``` ## Appreciation
+- StabilityAI for the generous sponsorship, as well as my other sponsors out
 there ## Testing Tests for equivariance etc ```bash $ python setup.py test ```
 ## Example First install `sidechainnet` ```bash $ pip install sidechainnet ```
 Then run the protein backbone denoising task ```bash $ python denoise.py ``` ##
 Todo - [x] move xi and xj separate project and sum logic into Conv class - [x]
 move self interacting key / value production into Conv, fix no pooling in conv
 with self interaction - [x] go with a naive way to split up contribution from
 input degrees for DTP - [x] for dot product attention in higher types, try
```

### Comparing `equiformer-pytorch-0.3.0/equiformer_pytorch/basis.py` & `equiformer-pytorch-0.3.1/equiformer_pytorch/basis.py`

 * *Files identical despite different names*

### Comparing `equiformer-pytorch-0.3.0/equiformer_pytorch/data/J_dense.pt` & `equiformer-pytorch-0.3.1/equiformer_pytorch/data/J_dense.pt`

 * *Files identical despite different names*

### Comparing `equiformer-pytorch-0.3.0/equiformer_pytorch/equiformer_pytorch.py` & `equiformer-pytorch-0.3.1/equiformer_pytorch/equiformer_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,18 @@
         self.weights = nn.ParameterList([])
         self.degrees = []
 
         for (degree, dim_in, dim_out) in fiber_and(fiber_in, fiber_out):
             self.weights.append(nn.Parameter(torch.randn(dim_in, dim_out) / sqrt(dim_in)))
             self.degrees.append(degree)
 
+    def init_zero_(self):
+        for weight in self.weights:
+            weight.data.zero_()
+
     def forward(self, x):
         out = {}
 
         for degree, weight in zip(self.degrees, self.weights):
             out[degree] = einsum(x[degree], weight, '... d m, d e -> ... e m')
 
         return out
@@ -449,15 +453,16 @@
 class FeedForward(nn.Module):
     @beartype
     def __init__(
         self,
         fiber: Tuple[int, ...],
         fiber_out: Optional[Tuple[int, ...]] = None,
         mult = 4,
-        include_htype_norms = True
+        include_htype_norms = True,
+        init_out_zero = True
     ):
         super().__init__()
         self.fiber = fiber
 
         fiber_hidden = tuple(dim * mult for dim in fiber)
 
         project_in_fiber = fiber
@@ -470,14 +475,17 @@
         fiber_out = default(fiber_out, fiber)
 
         self.prenorm     = Norm(fiber)
         self.project_in  = Linear(project_in_fiber, project_in_fiber_hidden)
         self.gate        = Gate(project_in_fiber_hidden)
         self.project_out = Linear(fiber_hidden, fiber_out)
 
+        if init_out_zero:
+            self.project_out.init_zero_()
+
     def forward(self, features):
         outputs = self.prenorm(features)
 
         if self.include_htype_norms:
             type0, *htypes = [*outputs.values()]
             htypes = map(lambda t: t.norm(dim = -1, keepdim = True), htypes)
             type0 = torch.cat((type0, *htypes), dim = -2)
@@ -538,15 +546,16 @@
         dim_head: Union[int, Tuple[int, ...]] = 64,
         heads: Union[int, Tuple[int, ...]] = 8,
         attend_self = False,
         edge_dim = None,
         single_headed_kv = False,
         radial_hidden_dim = 64,
         splits = 4,
-        num_linear_attn_heads = 0
+        num_linear_attn_heads = 0,
+        init_out_zero = True
     ):
         super().__init__()
         num_degrees = len(fiber)
 
         dim_head = cast_tuple(dim_head, num_degrees)
         assert len(dim_head) == num_degrees
 
@@ -576,14 +585,17 @@
         if self.has_linear_attn:
             degree_zero_dim = fiber[0]
             self.linear_attn = LinearAttention(degree_zero_dim, dim_head = dim_head[0], heads = num_linear_attn_heads)
             hidden_fiber = tuple_set_at_index(hidden_fiber, 0, hidden_fiber[0] + dim_head[0] * num_linear_attn_heads)
 
         self.to_out = Linear(hidden_fiber, fiber)
 
+        if init_out_zero:
+            self.to_out.init_zero_()
+
     @beartype
     def forward(
         self,
         features,
         edge_info: EdgeInfo,
         rel_dist,
         basis,
@@ -665,14 +677,15 @@
         edge_dim = None,
         splits = 4,
         single_headed_kv = False,
         attn_leakyrelu_slope = 0.1,
         attn_hidden_dim_mult = 4,
         radial_hidden_dim = 16,
         num_linear_attn_heads = 0,
+        init_out_zero = True,
         **kwargs
     ):
         super().__init__()
         num_degrees = len(fiber)
 
         dim_head = cast_tuple(dim_head, num_degrees)
         assert len(dim_head) == num_degrees
@@ -734,14 +747,17 @@
             self.linear_attn = LinearAttention(degree_zero_dim, dim_head = dim_head[0], heads = num_linear_attn_heads)
             hidden_fiber = tuple_set_at_index(hidden_fiber, 0, hidden_fiber[0] + dim_head[0] * num_linear_attn_heads)
 
         # combining heads and projection out
 
         self.to_out = Linear(hidden_fiber, fiber)
 
+        if init_out_zero:
+            self.to_out.init_zero_()
+
     @beartype
     def forward(
         self,
         features,
         edge_info: EdgeInfo,
         rel_dist,
         basis,
```

### Comparing `equiformer-pytorch-0.3.0/equiformer_pytorch/irr_repr.py` & `equiformer-pytorch-0.3.1/equiformer_pytorch/irr_repr.py`

 * *Files identical despite different names*

### Comparing `equiformer-pytorch-0.3.0/equiformer_pytorch/reversible.py` & `equiformer-pytorch-0.3.1/equiformer_pytorch/reversible.py`

 * *Files identical despite different names*

### Comparing `equiformer-pytorch-0.3.0/equiformer_pytorch/utils.py` & `equiformer-pytorch-0.3.1/equiformer_pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `equiformer-pytorch-0.3.0/equiformer_pytorch.egg-info/PKG-INFO` & `equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equiformer-pytorch
-Version: 0.3.0
+Version: 0.3.1
 Summary: Equiformer - SE3/E3 Graph Attention Transformer for Molecules and Proteins
 Home-page: https://github.com/lucidrains/equiformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,equivariance,molecules,proteins
 Classifier: Development Status :: 4 - Beta
```

### Comparing `equiformer-pytorch-0.3.0/equiformer_pytorch.egg-info/SOURCES.txt` & `equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equiformer-pytorch-0.3.0/setup.py` & `equiformer-pytorch-0.3.1/setup.py`

 * *Files identical despite different names*


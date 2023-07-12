# Comparing `tmp/backpack-for-pytorch-1.5.2.tar.gz` & `tmp/backpack-for-pytorch-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backpack-for-pytorch-1.5.2.tar", last modified: Mon Dec 19 13:04:37 2022, max compression
+gzip compressed data, was "backpack-for-pytorch-1.6.0.tar", last modified: Wed Jul 12 18:19:50 2023, max compression
```

## Comparing `backpack-for-pytorch-1.5.2.tar` & `backpack-for-pytorch-1.6.0.tar`

### file list

```diff
@@ -1,583 +1,597 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.592011 backpack-for-pytorch-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/.conda_env.yml
--rw-r--r--   0 runner    (1001) docker     (123)      410 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.500010 backpack-for-pytorch-1.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.520010 backpack-for-pytorch-1.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      896 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      302 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2022-12-19 13:04:37.592011 backpack-for-pytorch-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/README-dev.md
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.520010 backpack-for-pytorch-1.5.2/backpack/
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.520010 backpack-for-pytorch-1.5.2/backpack/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.524010 backpack-for-pytorch-1.5.2/backpack/core/derivatives/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/adaptive_avg_pool_nd.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/avgpool1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/avgpool2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/avgpool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/avgpoolnd.py
--rw-r--r--   0 runner    (1001) docker     (123)    22355 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/basederivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/batchnorm_nd.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/conv_transpose1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/conv_transpose2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/conv_transpose3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/conv_transposend.py
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/convnd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9057 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/crossentropyloss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/elementwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/elu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/logsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/maxpool1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/maxpool2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/maxpool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/maxpoolnd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/mseloss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/permute.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/scale_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/selu.py
--rw-r--r--   0 runner    (1001) docker     (123)    11144 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/shape_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/slicing.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/sum_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/tanh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/core/derivatives/zeropad2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.528010 backpack-for-pytorch-1.5.2/backpack/custom_module/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/custom_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/custom_module/branching.py
--rw-r--r--   0 runner    (1001) docker     (123)    18544 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/custom_module/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/custom_module/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/custom_module/permute.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/custom_module/reduce_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/custom_module/scale_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/custom_module/slicing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.528010 backpack-for-pytorch-1.5.2/backpack/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/backprop_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.528010 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.528010 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/batchnorm1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/ggnmpbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.532010 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/batchnorm1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/hmpbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.532010 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/pchmpbase.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.532010 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.532010 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/batch_grad_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/batchnorm_nd.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/conv_transpose1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/conv_transpose2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/conv_transpose3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/rnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.536010 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/batch_l2_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/batchnorm_nd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/convnd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/convtransposend.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/rnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.536010 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/batchnorm_nd.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/convtranspose1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/convtranspose2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/convtranspose3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/rnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.540010 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/batchnorm_nd.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/convtranspose1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/convtranspose2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/convtranspose3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/sgs_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.540010 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/batchnorm_nd.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/convtranspose1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/convtranspose2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/convtranspose3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/variance_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/mat_to_mat_jac_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/module_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/saved_quantities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.540010 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.544010 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/
--rw-r--r--   0 runner    (1001) docker     (123)    11690 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/adaptive_avg_pool_nd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/batchnorm_nd.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/convnd.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/convtranspose1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/convtranspose2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/convtranspose3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/convtransposend.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/custom_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/diag_ggn_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/permute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/slicing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.548010 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/convnd.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/convtranspose1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/convtranspose2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/convtranspose3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/convtransposend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/diag_h_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/slicing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.548010 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/custom_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/hbp_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/hbpbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.552010 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/batchnorm_nd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/convnd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/convtransposend.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/custom_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/slicing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.552010 backpack-for-pytorch-1.5.2/backpack/hessianfree/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/hessianfree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/hessianfree/ggnvp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/hessianfree/hvp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/hessianfree/lop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/hessianfree/rop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.552010 backpack-for-pytorch-1.5.2/backpack/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/utils/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/utils/conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/utils/convert_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/utils/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/utils/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/utils/kroneckers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/utils/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/utils/module_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/utils/subsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/backpack/utils/unsqueeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.556010 backpack-for-pytorch-1.5.2/backpack_for_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2022-12-19 13:04:37.000000 backpack-for-pytorch-1.5.2/backpack_for_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21916 2022-12-19 13:04:37.000000 backpack-for-pytorch-1.5.2/backpack_for_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 13:04:37.000000 backpack-for-pytorch-1.5.2/backpack_for_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 13:04:37.000000 backpack-for-pytorch-1.5.2/backpack_for_pytorch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      403 2022-12-19 13:04:37.000000 backpack-for-pytorch-1.5.2/backpack_for_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-19 13:04:37.000000 backpack-for-pytorch-1.5.2/backpack_for_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/black.toml
--rw-r--r--   0 runner    (1001) docker     (123)    18442 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.556010 backpack-for-pytorch-1.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.556010 backpack-for-pytorch-1.5.2/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.556010 backpack-for-pytorch-1.5.2/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/css/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      304 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/dangel2020backpack.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.508010 backpack-for-pytorch-1.5.2/docs/assets/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.556010 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700/
--rw-r--r--   0 runner    (1001) docker     (123)    16716 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.eot
--rw-r--r--   0 runner    (1001) docker     (123)    54360 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.svg
--rw-r--r--   0 runner    (1001) docker     (123)    29704 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.556010 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700italic/
--rw-r--r--   0 runner    (1001) docker     (123)    16849 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.eot
--rw-r--r--   0 runner    (1001) docker     (123)    54578 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28932 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.556010 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-italic/
--rw-r--r--   0 runner    (1001) docker     (123)    15864 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.eot
--rw-r--r--   0 runner    (1001) docker     (123)    55217 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.svg
--rw-r--r--   0 runner    (1001) docker     (123)    26644 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    12536 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.560010 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-regular/
--rw-r--r--   0 runner    (1001) docker     (123)    16639 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)    54935 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    29288 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    12840 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.560010 backpack-for-pytorch-1.5.2/docs/assets/img/
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/img/backpack_logo_torch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/img/updaterule.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.560010 backpack-for-pytorch-1.5.2/docs/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/assets/js/scale.fix.js
--rw-r--r--   0 runner    (1001) docker     (123)    19914 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/examples.html
--rw-r--r--   0 runner    (1001) docker     (123)    19065 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      892 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/jekyll-theme-minimal.gemspec
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.560010 backpack-for-pytorch-1.5.2/docs/script/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/script/bootstrap
--rw-r--r--   0 runner    (1001) docker     (123)      196 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/script/cibuild
--rw-r--r--   0 runner    (1001) docker     (123)      830 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/script/release
--rw-r--r--   0 runner    (1001) docker     (123)      597 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs/script/validate-html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.560010 backpack-for-pytorch-1.5.2/docs_src/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      454 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/buildweb.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.560010 backpack-for-pytorch-1.5.2/docs_src/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.560010 backpack-for-pytorch-1.5.2/docs_src/examples/basic_usage/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/basic_usage/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/basic_usage/example_all_in_one.py
--rw-r--r--   0 runner    (1001) docker     (123)   193937 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/cheatsheet.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.564010 backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13245 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_cg_newton.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_custom_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_diag_ggn_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_differential_privacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_extension_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_first_order_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_gradient_of_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_resnet_all_in_one.py
--rw-r--r--   0 runner    (1001) docker     (123)    10812 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_save_memory_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_subsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_trace_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.564010 backpack-for-pytorch-1.5.2/docs_src/rtd/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/rtd/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/rtd/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)      641 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/rtd/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.564010 backpack-for-pytorch-1.5.2/docs_src/rtd/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    57637 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/rtd/assets/backpack_logo_torch.png
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/rtd/assets/backpack_logo_torch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/rtd/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/rtd/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/rtd/good-to-know.rst
--rw-r--r--   0 runner    (1001) docker     (123)      562 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/rtd/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/rtd/main-api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      767 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/rtd/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/rtd/supported-layers.rst
--rw-r--r--   0 runner    (1001) docker     (123)   341498 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/rtd/torch.inventory
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.568010 backpack-for-pytorch-1.5.2/docs_src/splash/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/Gemfile
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.568010 backpack-for-pytorch-1.5.2/docs_src/splash/_includes/
--rw-r--r--   0 runner    (1001) docker     (123)    16268 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/_includes/code-samples.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/_includes/dangel2020backpack.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.568010 backpack-for-pytorch-1.5.2/docs_src/splash/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/_layouts/default.html
--rw-r--r--   0 runner    (1001) docker     (123)      283 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/_layouts/post.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.568010 backpack-for-pytorch-1.5.2/docs_src/splash/_sass/
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/_sass/fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/_sass/jekyll-theme-minimal.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/_sass/rouge-github.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.568010 backpack-for-pytorch-1.5.2/docs_src/splash/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.568010 backpack-for-pytorch-1.5.2/docs_src/splash/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/css/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      304 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/dangel2020backpack.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.516010 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.568010 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700/
--rw-r--r--   0 runner    (1001) docker     (123)    16716 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.eot
--rw-r--r--   0 runner    (1001) docker     (123)    54360 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.svg
--rw-r--r--   0 runner    (1001) docker     (123)    29704 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.568010 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700italic/
--rw-r--r--   0 runner    (1001) docker     (123)    16849 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.eot
--rw-r--r--   0 runner    (1001) docker     (123)    54578 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28932 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.572011 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-italic/
--rw-r--r--   0 runner    (1001) docker     (123)    15864 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.eot
--rw-r--r--   0 runner    (1001) docker     (123)    55217 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.svg
--rw-r--r--   0 runner    (1001) docker     (123)    26644 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    12536 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.572011 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-regular/
--rw-r--r--   0 runner    (1001) docker     (123)    16639 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)    54935 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    29288 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    12840 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.572011 backpack-for-pytorch-1.5.2/docs_src/splash/assets/img/
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/img/backpack_logo_torch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/img/updaterule.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.572011 backpack-for-pytorch-1.5.2/docs_src/splash/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/assets/js/scale.fix.js
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      517 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/jekyll-theme-minimal.gemspec
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.572011 backpack-for-pytorch-1.5.2/docs_src/splash/script/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/script/bootstrap
--rw-r--r--   0 runner    (1001) docker     (123)      196 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/script/cibuild
--rw-r--r--   0 runner    (1001) docker     (123)      830 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/script/release
--rw-r--r--   0 runner    (1001) docker     (123)      597 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/docs_src/splash/script/validate-html
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/fully_documented.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.572011 backpack-for-pytorch-1.5.2/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/logo/backpack_logo_no_torch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/logo/backpack_logo_torch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/makefile
--rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2022-12-19 13:04:37.592011 backpack-for-pytorch-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      363 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.576011 backpack-for-pytorch-1.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.580011 backpack-for-pytorch-1.5.2/test/adaptive_avg_pool/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/adaptive_avg_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/adaptive_avg_pool/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/adaptive_avg_pool/settings_adaptive_avg_pool_nd.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/adaptive_avg_pool/test_adaptive_avg_pool_nd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/automated_kfac_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/automated_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.580011 backpack-for-pytorch-1.5.2/test/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/benchmark/functionality.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/benchmark/jvp.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/benchmark/jvp_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/benchmark/jvp_avgpool2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/benchmark/jvp_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/benchmark/jvp_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/benchmark/jvp_maxpool2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/benchmark/jvp_zeropad2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/bugfixes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/conv2d_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.580011 backpack-for-pytorch-1.5.2/test/converter/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/converter/converter_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/converter/resnet_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/converter/test_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.580011 backpack-for-pytorch-1.5.2/test/core/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.584011 backpack-for-pytorch-1.5.2/test/core/derivatives/
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/activation_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/batch_norm_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14998 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/convolution_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    17201 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/derivatives_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/embedding_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.584011 backpack-for-pytorch-1.5.2/test/core/derivatives/implementation/
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/implementation/autograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/implementation/backpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/implementation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/linear_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/loss_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/lstm_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/padding_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/permute_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/pooling_adaptive_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/pooling_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/rnn_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/scale_module_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/slicing_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/core/derivatives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.584011 backpack-for-pytorch-1.5.2/test/custom_module/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/custom_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/custom_module/test_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/custom_module/test_slicing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.584011 backpack-for-pytorch-1.5.2/test/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/automated_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.584011 backpack-for-pytorch-1.5.2/test/extensions/firstorder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/firstorder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.584011 backpack-for-pytorch-1.5.2/test/extensions/firstorder/batch_grad/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/firstorder/batch_grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/firstorder/batch_grad/batch_grad_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/firstorder/batch_grad/test_batch_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.584011 backpack-for-pytorch-1.5.2/test/extensions/firstorder/batch_l2_grad/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/firstorder/batch_l2_grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/firstorder/batch_l2_grad/batchl2grad_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/firstorder/batch_l2_grad/test_batchl2grad.py
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/firstorder/firstorder_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.584011 backpack-for-pytorch-1.5.2/test/extensions/firstorder/sum_grad_squared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/firstorder/sum_grad_squared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/firstorder/sum_grad_squared/sumgradsquared_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/firstorder/sum_grad_squared/test_sumgradsquared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.588011 backpack-for-pytorch-1.5.2/test/extensions/firstorder/variance/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/firstorder/variance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/firstorder/variance/test_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/firstorder/variance/variance_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/graph_clear_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.588011 backpack-for-pytorch-1.5.2/test/extensions/implementation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/implementation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/implementation/autograd.py
--rw-r--r--   0 runner    (1001) docker     (123)    10565 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/implementation/backpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/implementation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/implementation/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.588011 backpack-for-pytorch-1.5.2/test/extensions/secondorder/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.588011 backpack-for-pytorch-1.5.2/test/extensions/secondorder/diag_ggn/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/diag_ggn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/diag_ggn/diag_ggn_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/diag_ggn/test_batch_diag_ggn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/diag_ggn/test_diag_ggn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.588011 backpack-for-pytorch-1.5.2/test/extensions/secondorder/diag_hessian/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/diag_hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/diag_hessian/diagh_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/diag_hessian/test_diag_hessian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.588011 backpack-for-pytorch-1.5.2/test/extensions/secondorder/hbp/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/hbp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/hbp/kfac_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/hbp/kflr_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/hbp/kfra_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/hbp/test_kfac.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/hbp/test_kflr.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/hbp/test_kfra.py
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/secondorder_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.588011 backpack-for-pytorch-1.5.2/test/extensions/secondorder/sqrt_ggn/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/sqrt_ggn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/sqrt_ggn/sqrt_ggn_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/secondorder/sqrt_ggn/test_sqrt_ggn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/test_backprop_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/extensions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.588011 backpack-for-pytorch-1.5.2/test/implementation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/implementation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/implementation/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/implementation/implementation_autograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/implementation/implementation_bpext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/interface_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/layers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/linear_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/problems.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/test_batch_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/test_problems_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/test_problems_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/test_problems_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/test_problems_kfacs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/test_problems_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/test_problems_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/test_problems_pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/test_retain_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/test_second_order_warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:04:37.592011 backpack-for-pytorch-1.5.2/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/utils/evaluation_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/utils/skip_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/utils/test_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/utils/test_conv_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/utils/test_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/utils/test_conv_transpose_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/utils/test_subsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2022-12-19 13:04:21.000000 backpack-for-pytorch-1.5.2/test/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.023393 backpack-for-pytorch-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/.conda_env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.903393 backpack-for-pytorch-1.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.919393 backpack-for-pytorch-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-12 18:19:50.023393 backpack-for-pytorch-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/README-dev.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.919393 backpack-for-pytorch-1.6.0/backpack/
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.919393 backpack-for-pytorch-1.6.0/backpack/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.931393 backpack-for-pytorch-1.6.0/backpack/core/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/adaptive_avg_pool_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/avgpool1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/avgpool2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/avgpool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/avgpoolnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22384 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/basederivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/batchnorm_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/bcewithlogitsloss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/conv_transpose1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/conv_transpose2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/conv_transpose3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/conv_transposend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/convnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10478 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/crossentropyloss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/elementwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/elu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/leakyrelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/logsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/maxpool1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/maxpool2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/maxpool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/maxpoolnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/mseloss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/nll_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/permute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/scale_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/selu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/shape_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/slicing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/sum_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/tanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/core/derivatives/zeropad2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.935393 backpack-for-pytorch-1.6.0/backpack/custom_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/custom_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/custom_module/branching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18544 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/custom_module/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/custom_module/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/custom_module/permute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/custom_module/reduce_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/custom_module/scale_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/custom_module/slicing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.935393 backpack-for-pytorch-1.6.0/backpack/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/backprop_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.935393 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.939393 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/batchnorm1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/ggnmpbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.943393 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/batchnorm1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/hmpbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.943393 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/pchmpbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.943393 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.947393 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/batch_grad_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/batchnorm_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/conv_transpose1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/conv_transpose2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/conv_transpose3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/rnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.947393 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/batch_l2_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/batchnorm_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/convnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/convtransposend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/rnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.951393 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/batchnorm_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/convtranspose1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/convtranspose2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/convtranspose3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/rnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.951393 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/batchnorm_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/convtranspose1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/convtranspose2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/convtranspose3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/sgs_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.955393 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/batchnorm_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/convtranspose1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/convtranspose2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/convtranspose3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/variance_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/mat_to_mat_jac_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/module_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/saved_quantities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.955393 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.959393 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/adaptive_avg_pool_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/batchnorm_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/convnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/convtranspose1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/convtranspose2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/convtranspose3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/convtransposend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/custom_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/diag_ggn_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/permute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/slicing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.963393 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/convnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/convtranspose1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/convtranspose2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/convtranspose3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/convtransposend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/diag_h_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/slicing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.963393 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/conv_transpose1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/conv_transpose2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/conv_transpose3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/conv_transposend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/convnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/custom_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/hbp_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/hbpbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.967393 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/batchnorm_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/convnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/convtransposend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/custom_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/slicing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.967393 backpack-for-pytorch-1.6.0/backpack/hessianfree/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/hessianfree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/hessianfree/ggnvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/hessianfree/hvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/hessianfree/lop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/hessianfree/rop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.971393 backpack-for-pytorch-1.6.0/backpack/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/utils/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/utils/conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/utils/convert_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/utils/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/utils/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/utils/kroneckers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/utils/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/utils/module_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/utils/subsampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/backpack/utils/unsqueeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.971393 backpack-for-pytorch-1.6.0/backpack_for_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-12 18:19:49.000000 backpack-for-pytorch-1.6.0/backpack_for_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22550 2023-07-12 18:19:49.000000 backpack-for-pytorch-1.6.0/backpack_for_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:19:49.000000 backpack-for-pytorch-1.6.0/backpack_for_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:19:49.000000 backpack-for-pytorch-1.6.0/backpack_for_pytorch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-12 18:19:49.000000 backpack-for-pytorch-1.6.0/backpack_for_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 18:19:49.000000 backpack-for-pytorch-1.6.0/backpack_for_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/black.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    21713 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.971393 backpack-for-pytorch-1.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.975393 backpack-for-pytorch-1.6.0/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.975393 backpack-for-pytorch-1.6.0/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/dangel2020backpack.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.907393 backpack-for-pytorch-1.6.0/docs/assets/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.975393 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700/
+-rw-r--r--   0 runner    (1001) docker     (123)    16716 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    54360 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    29704 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.979393 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700italic/
+-rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    54578 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28932 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.983393 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-italic/
+-rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    55217 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26644 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.983393 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-regular/
+-rw-r--r--   0 runner    (1001) docker     (123)    16639 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    54935 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    29288 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.987393 backpack-for-pytorch-1.6.0/docs/assets/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/img/backpack_logo_torch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/img/updaterule.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.987393 backpack-for-pytorch-1.6.0/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/assets/js/scale.fix.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19830 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/examples.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/jekyll-theme-minimal.gemspec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.987393 backpack-for-pytorch-1.6.0/docs/script/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/script/bootstrap
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/script/cibuild
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/script/release
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs/script/validate-html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.991393 backpack-for-pytorch-1.6.0/docs_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/CNAME
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/buildweb.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.991393 backpack-for-pytorch-1.6.0/docs_src/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.991393 backpack-for-pytorch-1.6.0/docs_src/examples/basic_usage/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/basic_usage/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/basic_usage/example_all_in_one.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193937 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/cheatsheet.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.995393 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_batched_jacobians.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_cg_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_custom_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_diag_ggn_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_differential_privacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_extension_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_first_order_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_gradient_of_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_resnet_all_in_one.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_retain_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_save_memory_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_subsampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_trace_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.995393 backpack-for-pytorch-1.6.0/docs_src/rtd/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/rtd/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/rtd/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/rtd/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.999393 backpack-for-pytorch-1.6.0/docs_src/rtd/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    57637 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/rtd/assets/backpack_logo_torch.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/rtd/assets/backpack_logo_torch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/rtd/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/rtd/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/rtd/good-to-know.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/rtd/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/rtd/main-api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/rtd/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/rtd/supported-layers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   341498 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/rtd/torch.inventory
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.999393 backpack-for-pytorch-1.6.0/docs_src/splash/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/Gemfile
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.999393 backpack-for-pytorch-1.6.0/docs_src/splash/_includes/
+-rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/_includes/code-samples.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/_includes/dangel2020backpack.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.999393 backpack-for-pytorch-1.6.0/docs_src/splash/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/_layouts/default.html
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/_layouts/post.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.999393 backpack-for-pytorch-1.6.0/docs_src/splash/_sass/
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/_sass/fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/_sass/jekyll-theme-minimal.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/_sass/rouge-github.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.999393 backpack-for-pytorch-1.6.0/docs_src/splash/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.999393 backpack-for-pytorch-1.6.0/docs_src/splash/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/dangel2020backpack.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.911393 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.999393 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700/
+-rw-r--r--   0 runner    (1001) docker     (123)    16716 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    54360 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    29704 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:49.999393 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700italic/
+-rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    54578 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28932 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.003394 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-italic/
+-rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    55217 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26644 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.003394 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-regular/
+-rw-r--r--   0 runner    (1001) docker     (123)    16639 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    54935 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    29288 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.003394 backpack-for-pytorch-1.6.0/docs_src/splash/assets/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/img/backpack_logo_torch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/img/updaterule.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.003394 backpack-for-pytorch-1.6.0/docs_src/splash/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/assets/js/scale.fix.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/jekyll-theme-minimal.gemspec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.003394 backpack-for-pytorch-1.6.0/docs_src/splash/script/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/script/bootstrap
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/script/cibuild
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/script/release
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/docs_src/splash/script/validate-html
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/fully_documented.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.003394 backpack-for-pytorch-1.6.0/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/logo/backpack_logo_no_torch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/logo/backpack_logo_torch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-12 18:19:50.023393 backpack-for-pytorch-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.007393 backpack-for-pytorch-1.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.007393 backpack-for-pytorch-1.6.0/test/adaptive_avg_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/adaptive_avg_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/adaptive_avg_pool/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/adaptive_avg_pool/settings_adaptive_avg_pool_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/adaptive_avg_pool/test_adaptive_avg_pool_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/automated_kfac_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/automated_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.007393 backpack-for-pytorch-1.6.0/test/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/benchmark/functionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/benchmark/jvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/benchmark/jvp_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/benchmark/jvp_avgpool2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/benchmark/jvp_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/benchmark/jvp_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/benchmark/jvp_maxpool2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/benchmark/jvp_zeropad2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/bugfixes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/conv2d_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.011393 backpack-for-pytorch-1.6.0/test/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/converter/converter_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/converter/resnet_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/converter/test_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.011393 backpack-for-pytorch-1.6.0/test/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.011393 backpack-for-pytorch-1.6.0/test/core/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/activation_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/batch_norm_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14998 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/convolution_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20875 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/derivatives_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/embedding_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.011393 backpack-for-pytorch-1.6.0/test/core/derivatives/implementation/
+-rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/implementation/autograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/implementation/backpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/implementation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/linear_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/loss_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/lstm_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/padding_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/permute_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/pooling_adaptive_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/pooling_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/rnn_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/scale_module_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/slicing_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/core/derivatives/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.015394 backpack-for-pytorch-1.6.0/test/custom_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/custom_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/custom_module/test_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/custom_module/test_slicing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.015394 backpack-for-pytorch-1.6.0/test/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/automated_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.015394 backpack-for-pytorch-1.6.0/test/extensions/firstorder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/firstorder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.015394 backpack-for-pytorch-1.6.0/test/extensions/firstorder/batch_grad/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/firstorder/batch_grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/firstorder/batch_grad/batch_grad_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/firstorder/batch_grad/test_batch_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.015394 backpack-for-pytorch-1.6.0/test/extensions/firstorder/batch_l2_grad/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/firstorder/batch_l2_grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/firstorder/batch_l2_grad/batchl2grad_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/firstorder/batch_l2_grad/test_batchl2grad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/firstorder/firstorder_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.015394 backpack-for-pytorch-1.6.0/test/extensions/firstorder/sum_grad_squared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/firstorder/sum_grad_squared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/firstorder/sum_grad_squared/sumgradsquared_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/firstorder/sum_grad_squared/test_sumgradsquared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.015394 backpack-for-pytorch-1.6.0/test/extensions/firstorder/variance/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/firstorder/variance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/firstorder/variance/test_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/firstorder/variance/variance_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/graph_clear_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.015394 backpack-for-pytorch-1.6.0/test/extensions/implementation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/implementation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/implementation/autograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/implementation/backpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/implementation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/implementation/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.015394 backpack-for-pytorch-1.6.0/test/extensions/secondorder/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.019394 backpack-for-pytorch-1.6.0/test/extensions/secondorder/diag_ggn/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/diag_ggn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/diag_ggn/diag_ggn_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/diag_ggn/test_batch_diag_ggn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/diag_ggn/test_diag_ggn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.019394 backpack-for-pytorch-1.6.0/test/extensions/secondorder/diag_hessian/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/diag_hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/diag_hessian/diagh_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/diag_hessian/test_diag_hessian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.019394 backpack-for-pytorch-1.6.0/test/extensions/secondorder/hbp/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/hbp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/hbp/kfac_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/hbp/kflr_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/hbp/kfra_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/hbp/test_kfac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/hbp/test_kflr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/hbp/test_kfra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15675 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/secondorder_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.019394 backpack-for-pytorch-1.6.0/test/extensions/secondorder/sqrt_ggn/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/sqrt_ggn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/sqrt_ggn/sqrt_ggn_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/secondorder/sqrt_ggn/test_sqrt_ggn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/test_backprop_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/extensions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.019394 backpack-for-pytorch-1.6.0/test/implementation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/implementation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/implementation/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/implementation/implementation_autograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/implementation/implementation_bpext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/interface_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/layers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/linear_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/test_batch_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/test_problems_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/test_problems_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/test_problems_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/test_problems_kfacs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/test_problems_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/test_problems_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/test_problems_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/test_retain_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/test_second_order_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:19:50.023393 backpack-for-pytorch-1.6.0/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/utils/conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/utils/evaluation_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/utils/skip_extension_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/utils/skip_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/utils/test_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/utils/test_conv_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/utils/test_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/utils/test_conv_transpose_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/utils/test_subsampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-07-12 18:19:32.000000 backpack-for-pytorch-1.6.0/test/utils_test.py
```

### Comparing `backpack-for-pytorch-1.5.2/.github/workflows/lint.yaml` & `backpack-for-pytorch-1.6.0/.github/workflows/lint.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -11,110 +11,110 @@
       - release
 
 jobs:
   flake8:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v1
-    - name: Set up Python 3.7
+    - name: Set up Python 3.8
       uses: actions/setup-python@v1
       with:
-        python-version: 3.7
+        python-version: 3.8
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         make install-lint
     - name: Run flake8
       run: |
         make flake8
   black:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v1
-    - name: Set up Python 3.7
+    - name: Set up Python 3.8
       uses: actions/setup-python@v1
       with:
-        python-version: 3.7
+        python-version: 3.8
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         make install-lint
     - name: Run black
       run: |
         make black-check
   isort:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v1
-    - name: Set up Python 3.7
+    - name: Set up Python 3.8
       uses: actions/setup-python@v1
       with:
-        python-version: 3.7
+        python-version: 3.8
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         make install-lint
     - name: Run isort
       run: |
         make isort-check
   pydocstyle:
     if: false
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v1
-    - name: Set up Python 3.7
+    - name: Set up Python 3.8
       uses: actions/setup-python@v1
       with:
-        python-version: 3.7
+        python-version: 3.8
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         make install-lint
     - name: Run pydocstyle
       run: |
         make pydocstyle-check
   darglint:
     if: false
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v1
-    - name: Set up Python 3.7
+    - name: Set up Python 3.8
       uses: actions/setup-python@v1
       with:
-        python-version: 3.7
+        python-version: 3.8
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         make install-lint
     - name: Run darglint
       run: |
         make darglint-check
   darglint-partial:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v1
-    - name: Set up Python 3.7
+    - name: Set up Python 3.8
       uses: actions/setup-python@v1
       with:
-        python-version: 3.7
+        python-version: 3.8
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         make install-lint
     - name: Run darglint
       run: |
         make darglint-check-partial
   pydocstyle-partial:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v1
-      - name: Set up Python 3.7
+      - name: Set up Python 3.8
         uses: actions/setup-python@v1
         with:
-          python-version: 3.7
+          python-version: 3.8
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           make install-lint
       - name: Run pydocstyle
         run: |
           make pydocstyle-check-partial
```

### Comparing `backpack-for-pytorch-1.5.2/.github/workflows/python-publish.yml` & `backpack-for-pytorch-1.6.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/.github/workflows/test.yaml` & `backpack-for-pytorch-1.6.0/.github/workflows/test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,26 @@
       - release
 
 jobs:
   tests:
     name: "py${{ matrix.python-version }} torch${{  matrix.pytorch-version}}"
     runs-on: ubuntu-latest
     env:
-      USING_COVERAGE: '3.7,3.9'
+      USING_COVERAGE: '3.9'
 
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9]
+        python-version: [3.8, 3.9]
         pytorch-version:
           - "==1.9.1"
           - "==1.10.1"
           - "==1.11.0"
           - "==1.12.1"
           - "==1.13.1"
+          - "==2.0.1"
           - "" # latest
     steps:
     - uses: actions/checkout@v1
     - uses: actions/setup-python@v1
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install Dependencies
```

### Comparing `backpack-for-pytorch-1.5.2/LICENSE.txt` & `backpack-for-pytorch-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/PKG-INFO` & `backpack-for-pytorch-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: backpack-for-pytorch
-Version: 1.5.2
+Version: 1.6.0
 Summary: BackPACK: Packing more into backprop
 Home-page: https://github.com/f-dangel/backpack
 Author: Felix Dangel, Frederik Kunstner
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 # <img alt="BackPACK" src="./logo/backpack_logo_torch.svg" height="90"> BackPACK: Packing more into backprop
 
 [![Travis](https://travis-ci.org/f-dangel/backpack.svg?branch=master)](https://travis-ci.org/f-dangel/backpack)
 [![Coveralls](https://coveralls.io/repos/github/f-dangel/backpack/badge.svg?branch=master)](https://coveralls.io/github/f-dangel/backpack)
-[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-370/)
 
 BackPACK is built on top of [PyTorch](https://github.com/pytorch/pytorch). It efficiently computes quantities other than the gradient.
 
 - **Website:** https://backpack.pt
 - **Documentation:** https://docs.backpack.pt/en/master/
 - **Bug reports & feature requests:** https://github.com/f-dangel/backpack/issues
```

### Comparing `backpack-for-pytorch-1.5.2/README-dev.md` & `backpack-for-pytorch-1.6.0/README-dev.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # <img alt="BackPACK" src="./logo/backpack_logo_torch.svg" height="90"> BackPACK developer manual
 
 ## General standards
-- Python version: support 3.7+, use 3.7 for development
+- Python version: support 3.8+, use 3.8 for development
 - `git` [branching model](https://nvie.com/posts/a-successful-git-branching-model/)
 - Docstring style:  [Google](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html)
 - Test runner: [`pytest`](https://docs.pytest.org/en/latest/)
 - Formatting: [`black`](https://black.readthedocs.io) ([`black` config](black.toml))
 - Linting: [`flake8`](http://flake8.pycqa.org/) ([`flake8` config](.flake8))
 
 ---
```

### Comparing `backpack-for-pytorch-1.5.2/README.md` & `backpack-for-pytorch-1.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # <img alt="BackPACK" src="./logo/backpack_logo_torch.svg" height="90"> BackPACK: Packing more into backprop
 
 [![Travis](https://travis-ci.org/f-dangel/backpack.svg?branch=master)](https://travis-ci.org/f-dangel/backpack)
 [![Coveralls](https://coveralls.io/repos/github/f-dangel/backpack/badge.svg?branch=master)](https://coveralls.io/github/f-dangel/backpack)
-[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-370/)
 
 BackPACK is built on top of [PyTorch](https://github.com/pytorch/pytorch). It efficiently computes quantities other than the gradient.
 
 - **Website:** https://backpack.pt
 - **Documentation:** https://docs.backpack.pt/en/master/
 - **Bug reports & feature requests:** https://github.com/f-dangel/backpack/issues
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/__init__.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/context.py` & `backpack-for-pytorch-1.6.0/backpack/context.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/adaptive_avg_pool_nd.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/adaptive_avg_pool_nd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/avgpoolnd.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/avgpoolnd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/basederivatives.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/basederivatives.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,15 @@
         Raises:
             NotImplementedError: if not overwritten
         """
         raise NotImplementedError
 
     # FIXME Currently returns `∂²output[i] / ∂input[i]² * g_out[0][i]`,
     # which s the residual matrix diagonal, rather than the Hessian diagonal
+
     def hessian_diagonal(
         self, module: Module, g_in: Tuple[Tensor], g_out: Tuple[Tensor]
     ) -> Tensor:
         """Return the Hessian diagonal `∂²output[i] / ∂input[i]²`.
 
         Only required if `hessian_is_diagonal` returns `True`.
         The Hessian diagonal is only defined for layers that preserve the size
@@ -302,15 +303,15 @@
 
         Returns:
             reshaped matrix
         """
         return cls._reshape_like(mat, module.output.shape)
 
 
-class BaseParameterDerivatives(BaseDerivatives, ABC):
+class BaseParameterDerivatives(BaseDerivatives, ABC):  # noqa: B024
     """First- and second order partial derivatives of a module with parameters.
 
     Assumptions (true for `nn.Linear`, `nn.Conv(Transpose)Nd`, `nn.BatchNormNd`):
     - Parameters are saved as `.weight` and `.bias` fields in a module
     - The output is linear in the model parameters
 
     Shape conventions:
@@ -431,15 +432,15 @@
 
     def _weight_jac_mat_prod(
         self, module: Module, g_inp: Tuple[Tensor], g_out: Tuple[Tensor], mat: Tensor
     ) -> Tensor:
         raise NotImplementedError
 
 
-class BaseLossDerivatives(BaseDerivatives, ABC):
+class BaseLossDerivatives(BaseDerivatives, ABC):  # noqa: B024
     """Second- order partial derivatives of loss functions."""
 
     # TODO Add shape check
     def sqrt_hessian(
         self,
         module: Module,
         g_inp: Tuple[Tensor],
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/batchnorm_nd.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/batchnorm_nd.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,14 @@
         g_out: Tuple[Tensor],
         mat: Tensor,
         subsampling: List[int] = None,
     ) -> Tensor:
         self._check_parameters(module)
         N: int = self._get_n_axis(module)
         if module.training:
-
             if subsampling is not None:
                 raise NotImplementedError(
                     "BatchNorm VJP sub-sampling is not defined in train mode."
                 )
 
             denominator: int = self._get_denominator(module)
             x_hat, var = self._get_normalized_input_and_var(module)
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/conv_transposend.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/conv_transposend.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/convnd.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/convnd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/crossentropyloss.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/crossentropyloss.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 """Partial derivatives for cross-entropy loss."""
 from math import sqrt
 from typing import Callable, Dict, List, Tuple
 
 from einops import rearrange
-from torch import Tensor, diag, diag_embed, einsum, eye, multinomial, ones_like, softmax
+from torch import Size, Tensor, diag, diag_embed, einsum, eye, ones_like, softmax
+from torch.distributions import Categorical
 from torch.nn import CrossEntropyLoss
 from torch.nn.functional import one_hot
 
-from backpack.core.derivatives.basederivatives import BaseLossDerivatives
+from backpack.core.derivatives.nll_base import NLLLossDerivatives
 from backpack.utils.subsampling import subsample
 
 
-class CrossEntropyLossDerivatives(BaseLossDerivatives):
+class CrossEntropyLossDerivatives(NLLLossDerivatives):
     """Partial derivatives for cross-entropy loss.
 
     The `torch.nn.CrossEntropyLoss` operation is a composition of softmax
     and negative log-likelihood.
     """
 
+    def __init__(self, use_autograd: bool = False):
+        """Initialization for CE loss derivative.
+
+        Args:
+            use_autograd: Compute gradients with autograd (rather than manual)
+                Defaults to ``False`` (manual computation).
+        """
+        super().__init__(use_autograd=use_autograd)
+
     def _sqrt_hessian(
         self,
         module: CrossEntropyLoss,
         g_inp: Tuple[Tensor],
         g_out: Tuple[Tensor],
         subsampling: List[int] = None,
     ) -> Tensor:
@@ -39,45 +49,14 @@
         if module.reduction == "mean":
             sqrt_H /= sqrt(self._get_mean_normalization(module.input0))
 
         sqrt_H = self._ungroup_batch_and_additional(sqrt_H, *rearrange_info)
         sqrt_H = self._expand_sqrt_h(sqrt_H)
         return sqrt_H
 
-    def _sqrt_hessian_sampled(
-        self,
-        module: CrossEntropyLoss,
-        g_inp: Tuple[Tensor],
-        g_out: Tuple[Tensor],
-        mc_samples: int = 1,
-        subsampling: List[int] = None,
-    ) -> Tensor:
-        self._check_2nd_order_parameters(module)
-
-        M = mc_samples
-        C = module.input0.shape[1]
-
-        probs = self._get_probs(module, subsampling=subsampling)
-        probs, *rearrange_info = self._merge_batch_and_additional(probs)
-
-        V_dim = 0
-        probs_unsqueezed = probs.unsqueeze(V_dim).repeat(M, 1, 1)
-
-        multi = multinomial(probs, M, replacement=True)
-        classes = one_hot(multi, num_classes=C)
-        classes = einsum("nvc->vnc", classes).float()
-
-        sqrt_mc_h = (probs_unsqueezed - classes) / sqrt(M)
-
-        if module.reduction == "mean":
-            sqrt_mc_h /= sqrt(self._get_mean_normalization(module.input0))
-
-        sqrt_mc_h = self._ungroup_batch_and_additional(sqrt_mc_h, *rearrange_info)
-        return sqrt_mc_h
-
     def _sum_hessian(
         self, module: CrossEntropyLoss, g_inp: Tuple[Tensor], g_out: Tuple[Tensor]
     ) -> Tensor:
         self._check_2nd_order_parameters(module)
 
         probs = self._get_probs(module)
 
@@ -261,7 +240,60 @@
         Args:
             input: Input to the cross-entropy module.
 
         Returns:
             Divisor for mean reduction.
         """
         return input.numel() // input.shape[1]
+
+    def _verify_support(self, module: CrossEntropyLoss):
+        """We only support default weight and ignore_index.
+
+        Args:
+            module: CrossEntropyLoss module
+        """
+        self._check_2nd_order_parameters(module)
+
+    def _make_distribution(self, subsampled_input: Tensor) -> Categorical:
+        """Create the likelihood distribution whose NLL is the CE.
+
+        The log probability of the Categorical distribution for a single sample
+        with k classes is ∑ᵢ₌₁ᵏ Ŷᵢ log pᵢ, where Ŷ is one-hot encoded. If p is
+        chosen as the softmax, this is equivalent to CrossEntropyLoss
+
+        Args:
+            subsampled_input: input after subsampling
+
+        Returns:
+            Normal distribution for targets | inputs
+        """
+        probs = softmax(subsampled_input, dim=1)
+        probs_rearranged = einsum("nc...->n...c", probs)
+        return Categorical(probs_rearranged)
+
+    def _compute_sampled_grads_manual(
+        self, subsampled_input: Tensor, mc_samples: int
+    ) -> Tensor:
+        """Manually compute gradients from sampled targets.
+
+        Cross Entropy loss is ∑ᵢ₌₁ᵏ Ŷᵢ log 𝜎(xᵢ), where 𝜎(xᵢ) is the softmax of
+        the input and Ŷᵢ is one-hot encoded. The gradient is 𝜎(xᵢ) - Ŷᵢ.
+
+        Args:
+            subsampled_input: input after subsampling
+            mc_samples: number of samples
+
+        Returns:
+            Gradient samples
+        """
+        probs = softmax(subsampled_input, dim=1)
+        expand_dims = [mc_samples] + probs.dim() * [-1]
+        probs_unsqeezed = probs.unsqueeze(0).expand(*expand_dims)  # [V N C D1 D2]
+
+        distribution = self._make_distribution(subsampled_input)
+        samples = distribution.sample(Size([mc_samples]))  # [V N D1 D2]
+        samples_onehot = one_hot(samples, num_classes=probs.shape[1])  # [V N D1 D2 C]
+        samples_onehot_rearranged = einsum("vn...c->vnc...", samples_onehot).to(
+            probs.dtype
+        )  # [V N C D1 D2]
+
+        return probs_unsqeezed - samples_onehot_rearranged
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/dropout.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/dropout.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/elementwise.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/elementwise.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/elu.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/elu.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/embedding.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/embedding.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/flatten.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/flatten.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/leakyrelu.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/leakyrelu.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/linear.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/linear.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/logsigmoid.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/logsigmoid.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/lstm.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/lstm.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/maxpoolnd.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/maxpoolnd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/pad.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/pad.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/permute.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/permute.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/relu.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/relu.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/rnn.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/rnn.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/scale_module.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/scale_module.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/selu.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/selu.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/shape_check.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/shape_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,14 @@
     Returns:
         Wrapped hessian_mat_prod which converts vector-format inputs to a matrix
             before processing. Preserves format of input.
     """
 
     @functools.wraps(make_hessian_mat_prod)
     def _wrapped_make_hessian_mat_prod(self, module, g_inp, g_out):
-
         hessian_mat_prod = make_hessian_mat_prod(self, module, g_inp, g_out)
 
         def _new_hessian_mat_prod(mat):
             is_vec = _same_dim_as(mat, module, "input0")
             mat_in = mat if not is_vec else _add_V_dim(mat)
             mat_out = hessian_mat_prod(mat_in)
             mat_out = mat_out if not is_vec else _remove_V_dim(mat_out)
@@ -276,15 +275,14 @@
 
     Returns:
         wrapped hessian_mat_prod with shape checks for input and output
     """
 
     @functools.wraps(make_hessian_mat_prod)
     def _wrapped_make_hessian_mat_prod(self, module, g_inp, g_out):
-
         hessian_mat_prod = make_hessian_mat_prod(self, module, g_inp, g_out)
 
         def _new_hessian_mat_prod(mat):
             _check_like(mat, module, "input0")
             result = hessian_mat_prod(mat)
             _check_like(result, module, "input0")
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/sigmoid.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/sigmoid.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/slicing.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/slicing.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/sum_module.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/sum_module.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/tanh.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/tanh.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/core/derivatives/zeropad2d.py` & `backpack-for-pytorch-1.6.0/backpack/core/derivatives/zeropad2d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/custom_module/branching.py` & `backpack-for-pytorch-1.6.0/backpack/custom_module/branching.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/custom_module/graph_utils.py` & `backpack-for-pytorch-1.6.0/backpack/custom_module/graph_utils.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/custom_module/pad.py` & `backpack-for-pytorch-1.6.0/backpack/custom_module/pad.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/custom_module/permute.py` & `backpack-for-pytorch-1.6.0/backpack/custom_module/permute.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/custom_module/reduce_tuple.py` & `backpack-for-pytorch-1.6.0/backpack/custom_module/reduce_tuple.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/custom_module/scale_module.py` & `backpack-for-pytorch-1.6.0/backpack/custom_module/scale_module.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/custom_module/slicing.py` & `backpack-for-pytorch-1.6.0/backpack/custom_module/slicing.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/backprop_extension.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/backprop_extension.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvature.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvature.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/__init__.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/__init__.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/activations.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/activations.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/batchnorm1d.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/batchnorm1d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/conv2d.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/conv2d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/ggnmpbase.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/ggnmpbase.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/linear.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/linear.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/ggnmp/losses.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/ggnmp/losses.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/__init__.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/activations.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/activations.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/batchnorm1d.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/batchnorm1d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/conv2d.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/conv2d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/hmpbase.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/hmpbase.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/linear.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/linear.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/hmp/losses.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/hmp/losses.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/__init__.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/activations.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/activations.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/conv2d.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/conv2d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/linear.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/linear.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/losses.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/losses.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/curvmatprod/pchmp/pchmpbase.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/curvmatprod/pchmp/pchmpbase.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/__init__.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/base.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/base.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/__init__.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/batch_grad_base.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/batch_grad_base.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/batchnorm_nd.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/batchnorm_nd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_grad/rnn.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_grad/rnn.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/__init__.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/batch_l2_base.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/batch_l2_base.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/batchnorm_nd.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/batchnorm_nd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/convnd.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/convnd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/convtransposend.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/convtransposend.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/linear.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/linear.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/batch_l2_grad/rnn.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/batch_l2_grad/rnn.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/base.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/base.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/batchnorm_nd.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/batchnorm_nd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/gradient/rnn.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/gradient/rnn.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/__init__.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/batchnorm_nd.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/batchnorm_nd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/linear.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/linear.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/rnn.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/rnn.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/sum_grad_squared/sgs_base.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/sum_grad_squared/sgs_base.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/__init__.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/batchnorm_nd.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/batchnorm_nd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/embedding.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/embedding.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/rnn.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/rnn.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/firstorder/variance/variance_base.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/firstorder/variance/variance_base.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/mat_to_mat_jac_base.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/mat_to_mat_jac_base.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/module_extension.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/module_extension.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/saved_quantities.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/saved_quantities.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/__init__.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     AdaptiveAvgPool3d,
     AvgPool1d,
     AvgPool2d,
     AvgPool3d,
     BatchNorm1d,
     BatchNorm2d,
     BatchNorm3d,
+    BCEWithLogitsLoss,
     Conv1d,
     Conv2d,
     Conv3d,
     ConvTranspose1d,
     ConvTranspose2d,
     ConvTranspose3d,
     CrossEntropyLoss,
@@ -145,14 +146,15 @@
                 AdaptiveAvgPool3d: adaptive_avg_pool_nd.DiagGGNAdaptiveAvgPoolNd(3),
                 BatchNorm1d: batchnorm_nd.DiagGGNBatchNormNd(),
                 BatchNorm2d: batchnorm_nd.DiagGGNBatchNormNd(),
                 BatchNorm3d: batchnorm_nd.DiagGGNBatchNormNd(),
                 Embedding: embedding.DiagGGNEmbedding(),
                 Pad: pad.DiagGGNPad(),
                 Slicing: slicing.DiagGGNSlicing(),
+                BCEWithLogitsLoss: losses.DiagGGNBCEWithLogitsLossDerivatives(),
             },
         )
 
     def accumulate_backpropagated_quantities(
         self, existing: Tensor, other: Tensor
     ) -> Tensor:  # noqa: D102
         return existing + other
@@ -270,14 +272,15 @@
                 AdaptiveAvgPool3d: adaptive_avg_pool_nd.DiagGGNAdaptiveAvgPoolNd(3),
                 BatchNorm1d: batchnorm_nd.BatchDiagGGNBatchNormNd(),
                 BatchNorm2d: batchnorm_nd.BatchDiagGGNBatchNormNd(),
                 BatchNorm3d: batchnorm_nd.BatchDiagGGNBatchNormNd(),
                 Embedding: embedding.BatchDiagGGNEmbedding(),
                 Pad: pad.DiagGGNPad(),
                 Slicing: slicing.DiagGGNSlicing(),
+                BCEWithLogitsLoss: losses.DiagGGNBCEWithLogitsLossDerivatives(),
             },
         )
 
     def accumulate_backpropagated_quantities(
         self, existing: Tensor, other: Tensor
     ) -> Tensor:  # noqa: D102
         return existing + other
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/activations.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/activations.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/adaptive_avg_pool_nd.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/adaptive_avg_pool_nd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/batchnorm_nd.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/batchnorm_nd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/convnd.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/convnd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/convtranspose1d.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/convtranspose1d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/convtranspose2d.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/convtranspose2d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/convtranspose3d.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/convtranspose3d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/convtransposend.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/convtransposend.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,18 @@
 class DiagGGNConvTransposeND(DiagGGNBaseModule):
     def bias(self, ext, module, grad_inp, grad_out, backproped):
         sqrt_ggn = backproped
         return convUtils.extract_bias_diagonal(module, sqrt_ggn, sum_batch=True)
 
     def weight(self, ext, module, grad_inp, grad_out, backproped):
         X = convUtils.unfold_by_conv_transpose(module.input0, module)
-        weight_diag = convUtils.extract_weight_diagonal(
-            module, X, backproped, sum_batch=True
-        )
-        return weight_diag
+        return convUtils.extract_weight_diagonal(module, X, backproped, sum_batch=True)
 
 
 class BatchDiagGGNConvTransposeND(DiagGGNBaseModule):
     def bias(self, ext, module, grad_inp, grad_out, backproped):
         sqrt_ggn = backproped
         return convUtils.extract_bias_diagonal(module, sqrt_ggn, sum_batch=False)
 
     def weight(self, ext, module, grad_inp, grad_out, backproped):
         X = convUtils.unfold_by_conv_transpose(module.input0, module)
-        weight_diag = convUtils.extract_weight_diagonal(
-            module, X, backproped, sum_batch=False
-        )
-        return weight_diag
+        return convUtils.extract_weight_diagonal(module, X, backproped, sum_batch=False)
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/custom_module.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/custom_module.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/diag_ggn_base.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/diag_ggn_base.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/embedding.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/embedding.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/linear.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/linear.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/losses.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/losses.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from functools import partial
 
+from backpack.core.derivatives.bcewithlogitsloss import BCELossWithLogitsDerivatives
 from backpack.core.derivatives.crossentropyloss import CrossEntropyLossDerivatives
 from backpack.core.derivatives.mseloss import MSELossDerivatives
 from backpack.extensions.secondorder.diag_ggn.diag_ggn_base import DiagGGNBaseModule
 from backpack.extensions.secondorder.hbp import LossHessianStrategy
 
 
 class DiagGGNLoss(DiagGGNBaseModule):
@@ -30,7 +31,12 @@
     def __init__(self):
         super().__init__(derivatives=MSELossDerivatives())
 
 
 class DiagGGNCrossEntropyLoss(DiagGGNLoss):
     def __init__(self):
         super().__init__(derivatives=CrossEntropyLossDerivatives())
+
+
+class DiagGGNBCEWithLogitsLossDerivatives(DiagGGNLoss):
+    def __init__(self):
+        super().__init__(derivatives=BCELossWithLogitsDerivatives())
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/pooling.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/pooling.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/rnn.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/rnn.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_ggn/slicing.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_ggn/slicing.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 from torch.nn import (
     ELU,
     SELU,
     AvgPool1d,
     AvgPool2d,
     AvgPool3d,
+    BCEWithLogitsLoss,
     Conv1d,
     Conv2d,
     Conv3d,
     ConvTranspose1d,
     ConvTranspose2d,
     ConvTranspose3d,
     CrossEntropyLoss,
@@ -94,14 +95,15 @@
                 Tanh: activations.DiagHTanh(),
                 LeakyReLU: activations.DiagHLeakyReLU(),
                 LogSigmoid: activations.DiagHLogSigmoid(),
                 ELU: activations.DiagHELU(),
                 SELU: activations.DiagHSELU(),
                 Pad: pad.DiagHPad(),
                 Slicing: slicing.DiagHSlicing(),
+                BCEWithLogitsLoss: losses.DiagHBCEWithLogitsLoss(),
             },
         )
 
 
 class BatchDiagHessian(SecondOrderBackpropExtension):
     """BackPACK extensions that computes the per-sample (individual) Hessian diagonal.
 
@@ -143,9 +145,10 @@
                 Tanh: activations.DiagHTanh(),
                 LeakyReLU: activations.DiagHLeakyReLU(),
                 LogSigmoid: activations.DiagHLogSigmoid(),
                 ELU: activations.DiagHELU(),
                 SELU: activations.DiagHSELU(),
                 Pad: pad.DiagHPad(),
                 Slicing: slicing.DiagHSlicing(),
+                BCEWithLogitsLoss: losses.DiagHBCEWithLogitsLoss(),
             },
         )
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/activations.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/activations.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/conv1d.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/conv1d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/conv2d.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/conv2d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/conv3d.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/conv3d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/convnd.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/convnd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/convtranspose1d.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/convtranspose1d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/convtranspose2d.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/convtranspose2d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/convtranspose3d.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/convtranspose3d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/convtransposend.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/convtransposend.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/diag_h_base.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/diag_h_base.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/linear.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/linear.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/losses.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/losses.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from backpack.core.derivatives.bcewithlogitsloss import BCELossWithLogitsDerivatives
 from backpack.core.derivatives.crossentropyloss import CrossEntropyLossDerivatives
 from backpack.core.derivatives.mseloss import MSELossDerivatives
 from backpack.extensions.secondorder.diag_hessian.diag_h_base import DiagHBaseModule
 
 
 class DiagHLoss(DiagHBaseModule):
     def backpropagate(self, ext, module, g_inp, g_out, backproped):
@@ -13,7 +14,12 @@
     def __init__(self):
         super().__init__(derivatives=MSELossDerivatives())
 
 
 class DiagHCrossEntropyLoss(DiagHLoss):
     def __init__(self):
         super().__init__(derivatives=CrossEntropyLossDerivatives())
+
+
+class DiagHBCEWithLogitsLoss(DiagHLoss):
+    def __init__(self):
+        super().__init__(derivatives=BCELossWithLogitsDerivatives())
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/diag_hessian/pooling.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/diag_hessian/pooling.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from torch import Tensor
 from torch.nn import (
     AvgPool2d,
+    BCEWithLogitsLoss,
+    Conv1d,
     Conv2d,
+    Conv3d,
+    ConvTranspose1d,
+    ConvTranspose2d,
+    ConvTranspose3d,
     CrossEntropyLoss,
     Dropout,
     Flatten,
     Identity,
     Linear,
     MaxPool2d,
     MSELoss,
@@ -23,15 +29,20 @@
     BackpropStrategy,
     ExpectationApproximation,
     LossHessianStrategy,
 )
 
 from . import (
     activations,
+    conv1d,
     conv2d,
+    conv3d,
+    conv_transpose1d,
+    conv_transpose2d,
+    conv_transpose3d,
     custom_module,
     dropout,
     flatten,
     linear,
     losses,
     padding,
     pooling,
@@ -54,19 +65,25 @@
 
         super().__init__(
             savefield=savefield,
             fail_mode="ERROR",
             module_exts={
                 MSELoss: losses.HBPMSELoss(),
                 CrossEntropyLoss: losses.HBPCrossEntropyLoss(),
+                BCEWithLogitsLoss: losses.HBPBCEWithLogitsLoss(),
                 Linear: linear.HBPLinear(),
                 MaxPool2d: pooling.HBPMaxpool2d(),
                 AvgPool2d: pooling.HBPAvgPool2d(),
                 ZeroPad2d: padding.HBPZeroPad2d(),
+                Conv1d: conv1d.HBPConv1d(),
                 Conv2d: conv2d.HBPConv2d(),
+                Conv3d: conv3d.HBPConv3d(),
+                ConvTranspose1d: conv_transpose1d.HBPConvTranspose1d(),
+                ConvTranspose2d: conv_transpose2d.HBPConvTranspose2d(),
+                ConvTranspose3d: conv_transpose3d.HBPConvTranspose3d(),
                 Dropout: dropout.HBPDropout(),
                 Flatten: flatten.HBPFlatten(),
                 ReLU: activations.HBPReLU(),
                 Sigmoid: activations.HBPSigmoid(),
                 Tanh: activations.HBPTanh(),
                 SumModule: custom_module.HBPSumModule(),
                 ScaleModule: custom_module.HBPScaleModule(),
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/activations.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/activations.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/conv2d.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/linear.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,82 @@
 from torch import einsum
+from torch.nn import Linear
 
-from backpack.core.derivatives.conv2d import Conv2DDerivatives
+from backpack.core.derivatives.linear import LinearDerivatives
 from backpack.extensions.secondorder.hbp.hbp_options import (
     BackpropStrategy,
     ExpectationApproximation,
 )
 from backpack.extensions.secondorder.hbp.hbpbase import HBPBaseModule
-from backpack.utils import conv as convUtils
 
 
-class HBPConv2d(HBPBaseModule):
+class HBPLinear(HBPBaseModule):
     def __init__(self):
-        super().__init__(derivatives=Conv2DDerivatives(), params=["weight", "bias"])
+        super().__init__(derivatives=LinearDerivatives(), params=["weight", "bias"])
 
     def weight(self, ext, module, g_inp, g_out, backproped):
-
-        if module.groups != 1:
-            raise NotImplementedError(
-                f"groups ≠ 1 is not supported by {ext.__class__.__name__} "
-                + f"(got {module.groups})."
-            )
-
+        self.check_parameters(ext, module)
         bp_strategy = ext.get_backprop_strategy()
 
         if BackpropStrategy.is_batch_average(bp_strategy):
             return self._weight_for_batch_average(ext, module, backproped)
 
         elif BackpropStrategy.is_sqrt(bp_strategy):
             return self._weight_for_sqrt(ext, module, backproped)
 
-    # TODO: Require tests
     def _weight_for_batch_average(self, ext, module, backproped):
-        kron_factors = [self._factor_from_batch_average(module, backproped)]
+        kron_factors = self._bias_for_batch_average(backproped)
         kron_factors += self._factors_from_input(ext, module)
         return kron_factors
 
     def _weight_for_sqrt(self, ext, module, backproped):
-        kron_factors = [self._factor_from_sqrt(module, backproped)]
+        kron_factors = self._factor_from_sqrt(backproped)
         kron_factors += self._factors_from_input(ext, module)
         return kron_factors
 
     def _factors_from_input(self, ext, module):
-        X = convUtils.unfold_input(module, module.input0)
-        batch = X.size(0)
-
         ea_strategy = ext.get_ea_strategy()
 
         if ExpectationApproximation.should_average_param_jac(ea_strategy):
-            raise NotImplementedError("Undefined")
+            mean_input = self.__mean_input(module).unsqueeze(-1)
+            return [mean_input, mean_input.transpose()]
         else:
-            yield einsum("bik,bjk->ij", (X, X)) / batch
+            return [self.__mean_input_outer(module)]
 
-    def _factor_from_sqrt(self, module, backproped):
-        sqrt_ggn = backproped
-
-        sqrt_ggn = convUtils.separate_channels_and_pixels(module, sqrt_ggn)
-        sqrt_ggn = einsum("cbij->cbi", (sqrt_ggn,))
-        return einsum("cbi,cbl->il", (sqrt_ggn, sqrt_ggn))
+    def _factor_from_sqrt(self, backproped):
+        return [einsum("vni,vnj->ij", (backproped, backproped))]
 
     def bias(self, ext, module, g_inp, g_out, backproped):
+        self.check_parameters(ext, module)
         bp_strategy = ext.get_backprop_strategy()
 
         if BackpropStrategy.is_batch_average(bp_strategy):
-            return self._bias_for_batch_average(module, backproped)
+            return self._bias_for_batch_average(backproped)
         elif BackpropStrategy.is_sqrt(bp_strategy):
-            return self._bias_for_sqrt(module, backproped)
+            return self._factor_from_sqrt(backproped)
+
+    def _bias_for_batch_average(self, backproped):
+        return [backproped]
 
-    def _bias_for_sqrt(self, module, backproped):
-        return [self._factor_from_sqrt(module, backproped)]
+    def __mean_input(self, module):
+        return module.input0.mean(0).flatten()
 
-    # TODO: Require tests
-    def _bias_for_batch_average(self, module, backproped):
-        return [self._factor_from_batch_average(module, backproped)]
-
-    def _factor_from_batch_average(self, module, backproped):
-        _, out_c, out_x, out_y = module.output.size()
-        out_pixels = out_x * out_y
-        # sum over spatial coordinates
-        result = backproped.view(out_c, out_pixels, out_c, out_pixels).sum([1, 3])
-        return result.contiguous()
+    def __mean_input_outer(self, module):
+        N = module.input0.size(0)
+        flat_input = module.input0.reshape(N, -1)
+        return einsum("ni,nj->ij", (flat_input, flat_input)) / N
+
+    def check_parameters(self, ext, module: Linear) -> None:
+        """Raise an exception if module parameters are not supported.
+
+        Args:
+            ext (KFAC or KFRA or KFLR): Extension calling out to the module.
+            module: Linear layer.
+
+        Raises:
+            NotImplementedError: If the setting is not implemented.
+        """
+        if module.input0.dim() != 2:
+            raise NotImplementedError(
+                f"Only 2d inputs are supported by {ext.__class__.__name__} "
+                + f"(got {module.input0.dim()})."
+            )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/custom_module.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/custom_module.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/hbp_options.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/hbp_options.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/hbpbase.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/hbpbase.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/hbp/losses.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/hbp/losses.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 from functools import partial
 
+from backpack.core.derivatives.bcewithlogitsloss import BCELossWithLogitsDerivatives
 from backpack.core.derivatives.crossentropyloss import CrossEntropyLossDerivatives
 from backpack.core.derivatives.mseloss import MSELossDerivatives
 from backpack.extensions.curvature import Curvature
 from backpack.extensions.secondorder.hbp.hbp_options import LossHessianStrategy
 from backpack.extensions.secondorder.hbp.hbpbase import HBPBaseModule
 
 
 class HBPLoss(HBPBaseModule):
     def backpropagate(self, ext, module, g_inp, g_out, backproped):
         Curvature.check_loss_hessian(
             self.derivatives.hessian_is_psd(), curv_type=ext.get_curv_type()
         )
 
         H_func = self.make_loss_hessian_func(ext)
-        H_loss = H_func(module, g_inp, g_out)
 
-        return H_loss
+        return H_func(module, g_inp, g_out)
 
     def make_loss_hessian_func(self, ext):
         """Get function that produces the backpropagated quantity."""
         hessian_strategy = ext.get_loss_hessian_strategy()
 
         if hessian_strategy == LossHessianStrategy.EXACT:
             return self.derivatives.sqrt_hessian
         elif hessian_strategy == LossHessianStrategy.SAMPLING:
             mc_samples = ext.get_num_mc_samples()
             return partial(self.derivatives.sqrt_hessian_sampled, mc_samples=mc_samples)
         elif hessian_strategy == LossHessianStrategy.SUM:
             return self.derivatives.sum_hessian
         else:
-            raise ValueError("Unknown Hessian strategy: {}".format(hessian_strategy))
+            raise ValueError(f"Unknown Hessian strategy: {hessian_strategy}")
 
 
 class HBPMSELoss(HBPLoss):
     def __init__(self):
         super().__init__(derivatives=MSELossDerivatives())
 
 
 class HBPCrossEntropyLoss(HBPLoss):
     def __init__(self):
         super().__init__(derivatives=CrossEntropyLossDerivatives())
+
+
+class HBPBCEWithLogitsLoss(HBPLoss):
+    """Hessian backpropagation for the ``BCEWithLogitsLoss`` layer."""
+
+    def __init__(self):
+        """Pass derivatives for ``BCEWithLogitsLoss``."""
+        super().__init__(derivatives=BCELossWithLogitsDerivatives())
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/__init__.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     SELU,
     AvgPool1d,
     AvgPool2d,
     AvgPool3d,
     BatchNorm1d,
     BatchNorm2d,
     BatchNorm3d,
+    BCEWithLogitsLoss,
     Conv1d,
     Conv2d,
     Conv3d,
     ConvTranspose1d,
     ConvTranspose2d,
     ConvTranspose3d,
     CrossEntropyLoss,
@@ -112,14 +113,15 @@
                 ScaleModule: custom_module.SqrtGGNScaleModule(),
                 SumModule: custom_module.SqrtGGNSumModule(),
                 BatchNorm1d: batchnorm_nd.SqrtGGNBatchNormNd(),
                 BatchNorm2d: batchnorm_nd.SqrtGGNBatchNormNd(),
                 BatchNorm3d: batchnorm_nd.SqrtGGNBatchNormNd(),
                 Pad: pad.SqrtGGNPad(),
                 Slicing: slicing.SqrtGGNSlicing(),
+                BCEWithLogitsLoss: losses.SqrtGGNBCEWithLogithsLoss(),
             },
             subsampling=subsampling,
         )
 
     def get_loss_hessian_strategy(self) -> str:
         """Return the strategy used to represent the backpropagated loss Hessian.
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/activations.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/activations.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/base.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/base.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/batchnorm_nd.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/batchnorm_nd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/convnd.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/convnd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/convtransposend.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/convtransposend.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/custom_module.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/custom_module.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/losses.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/losses.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Tuple, Union
 
 from torch import Tensor
 from torch.nn import Module
 
+from backpack.core.derivatives.bcewithlogitsloss import BCELossWithLogitsDerivatives
 from backpack.core.derivatives.crossentropyloss import CrossEntropyLossDerivatives
 from backpack.core.derivatives.mseloss import MSELossDerivatives
 from backpack.extensions.secondorder.hbp import LossHessianStrategy
 from backpack.extensions.secondorder.sqrt_ggn.base import SqrtGGNBaseModule
 
 if TYPE_CHECKING:
     from backpack.extensions.secondorder.sqrt_ggn import SqrtGGNExact, SqrtGGNMC
@@ -76,7 +77,15 @@
 
 class SqrtGGNCrossEntropyLoss(SqrtGGNBaseLossModule):
     """``SqrtGGN{Exact, MC}`` extension for ``torch.nn.CrossEntropyLoss`` module."""
 
     def __init__(self):
         """Pass derivatives for ``torch.nn.CrossEntropyLoss`` module."""
         super().__init__(CrossEntropyLossDerivatives())
+
+
+class SqrtGGNBCEWithLogithsLoss(SqrtGGNBaseLossModule):
+    """``SqrtGGN{Exact, MC}`` extension for ``torch.nn.BCEWithLogitsLoss`` module."""
+
+    def __init__(self):
+        """Pass derivatives for ``torch.nn.BCEWithLogitsLoss`` module."""
+        super().__init__(BCELossWithLogitsDerivatives())
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/extensions/secondorder/sqrt_ggn/pooling.py` & `backpack-for-pytorch-1.6.0/backpack/extensions/secondorder/sqrt_ggn/pooling.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/hessianfree/ggnvp.py` & `backpack-for-pytorch-1.6.0/backpack/hessianfree/ggnvp.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/hessianfree/hvp.py` & `backpack-for-pytorch-1.6.0/backpack/hessianfree/hvp.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/hessianfree/lop.py` & `backpack-for-pytorch-1.6.0/backpack/hessianfree/lop.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/hessianfree/rop.py` & `backpack-for-pytorch-1.6.0/backpack/hessianfree/rop.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/utils/conv.py` & `backpack-for-pytorch-1.6.0/backpack/utils/conv.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,25 @@
-from typing import Callable, Type, Union
+"""Utility functions for convolution layers."""
+
+from typing import Callable, Tuple, Type, Union
 from warnings import warn
 
-import torch
 from einops import rearrange
 from torch import Tensor, einsum
-from torch.nn import Conv1d, Conv2d, Conv3d, Module
+from torch.nn import (
+    Conv1d,
+    Conv2d,
+    Conv3d,
+    ConvTranspose1d,
+    ConvTranspose2d,
+    ConvTranspose3d,
+    Module,
+)
 from torch.nn.functional import conv1d, conv2d, conv3d, unfold
+from unfoldNd import unfoldNd
 
 
 def get_conv_module(N: int) -> Type[Module]:
     """Return the PyTorch module class of N-dimensional convolution.
 
     Args:
         N: Convolution dimension.
@@ -61,121 +71,132 @@
             padding=module.padding,
             stride=module.stride,
         )
     else:
         return unfold_by_conv(input, module)
 
 
-def get_weight_gradient_factors(input, grad_out, module):
+def get_weight_gradient_factors(
+    input: Tensor, grad_out: Tensor, module: Union[Conv1d, Conv2d, Conv3d]
+) -> Tuple[Tensor, Tensor]:
+    """Return the factors for constructing the gradients w.r.t. the kernel.
+
+    Args:
+        input: Convolution layer input.
+        grad_out: Gradient w.r.t. to the convolution layer output.
+        module: Convolution layer.
+
+    Returns:
+        Unfolded input, output gradient with flattened spatial dimensions.
+    """
     X = unfold_input(module, input)
     dE_dY = rearrange(grad_out, "n c ... -> n c (...)")
     return X, dE_dY
 
 
-def separate_channels_and_pixels(module, tensor):
-    """Reshape (V, N, C, H, W) into (V, N, C, H * W)."""
-    return rearrange(tensor, "v n c ... -> v n c (...)")
-
-
-def extract_weight_diagonal(module, unfolded_input, S, sum_batch=True):
+def extract_weight_diagonal(
+    module: Union[Conv1d, Conv2d, Conv3d],
+    unfolded_input: Tensor,
+    S: Tensor,
+    sum_batch: bool = True,
+) -> Tensor:
     """Extract diagonal of ``(Jᵀ S) (Jᵀ S)ᵀ`` where ``J`` is the weight Jacobian.
 
     Args:
-        module (torch.nn.Conv1d or torch.nn.Conv2d or torch.nn.Conv3d): Convolution
-            layer for which the diagonal is extracted w.r.t. the weight.
-        unfolded_input (torch.Tensor): Unfolded input to the convolution. Shape must
-            follow the conventions of ``torch.nn.Unfold``.
-        S (torch.Tensor): Backpropagated (symmetric factorization) of the loss Hessian.
+        module: Convolution layer for which the diagonal is extracted w.r.t. the weight.
+        unfolded_input: Unfolded input to the convolution. Shape must follow the
+            conventions of ``torch.nn.Unfold``.
+        S: Backpropagated (symmetric factorization) of the loss Hessian.
             Has shape ``(V, *module.output.shape)``.
-        sum_batch (bool, optional): Sum out the batch dimension of the weight diagonals.
+        sum_batch: Sum out the batch dimension of the weight diagonals.
             Default value: ``True``.
 
     Returns:
-        torch.Tensor: Per-sample weight diagonal if ``sum_batch=False`` (shape
-            ``(N, module.weight.shape)`` with batch size ``N``) or summed weight
-            diagonal if ``sum_batch=True`` (shape ``module.weight.shape``).
+        Per-sample weight diagonal if ``sum_batch=False`` (shape
+        ``(N, module.weight.shape)`` with batch size ``N``) or summed weight
+        diagonal if ``sum_batch=True`` (shape ``module.weight.shape``).
     """
     S = rearrange(S, "v n (g c) ... -> v n g c (...)", g=module.groups)
     unfolded_input = rearrange(unfolded_input, "n (g c) k -> n g c k", g=module.groups)
 
     JS = einsum("ngkl,vngml->vngmk", (unfolded_input, S))
 
     sum_dims = [0, 1] if sum_batch else [0]
     out_shape = (
         module.weight.shape if sum_batch else (JS.shape[1], *module.weight.shape)
     )
 
-    weight_diagonal = JS.pow_(2).sum(sum_dims).reshape(out_shape)
-
-    return weight_diagonal
+    return JS.pow_(2).sum(sum_dims).reshape(out_shape)
 
 
 # TODO This method applies the bias Jacobian, then squares and sums the result. Intro-
 # duce base class for {Batch}DiagHessian and DiagGGN{Exact,MC} and remove this method
-def extract_bias_diagonal(module, S, sum_batch=True):
+def extract_bias_diagonal(
+    module: Union[
+        Conv1d, Conv2d, Conv3d, ConvTranspose1d, ConvTranspose2d, ConvTranspose3d
+    ],
+    S: Tensor,
+    sum_batch: bool = True,
+) -> Tensor:
     """Extract diagonal of ``(Jᵀ S) (Jᵀ S)ᵀ`` where ``J`` is the bias Jacobian.
 
     Args:
-        module (torch.nn.Conv1d or torch.nn.Conv2d or torch.nn.Conv3d): Convolution
-            layer for which the diagonal is extracted w.r.t. the bias.
-        S (torch.Tensor): Backpropagated (symmetric factorization) of the loss Hessian.
+        module: Convolution layer for which the diagonal is extracted w.r.t. the bias.
+        S: Backpropagated (symmetric factorization) of the loss Hessian.
             Has shape ``(V, *module.output.shape)``.
-        sum_batch (bool, optional): Sum out the batch dimension of the bias diagonals.
+        sum_batch: Sum out the batch dimension of the bias diagonals.
             Default value: ``True``.
 
     Returns:
-        torch.Tensor: Per-sample bias diagonal if ``sum_batch=False`` (shape
-            ``(N, module.bias.shape)`` with batch size ``N``) or summed bias
-            diagonal if ``sum_batch=True`` (shape ``module.bias.shape``).
+        Per-sample bias diagonal if ``sum_batch=False`` (shape
+        ``(N, module.bias.shape)`` with batch size ``N``) or summed bias
+        diagonal if ``sum_batch=True`` (shape ``module.bias.shape``).
     """
     start_spatial = 3
     sum_before = list(range(start_spatial, S.dim()))
     sum_after = [0, 1] if sum_batch else [0]
 
     return S.sum(sum_before).pow_(2).sum(sum_after)
 
 
-def unfold_by_conv(input, module):
-    """Return the unfolded input using convolution"""
-    N, C_in = input.shape[0], input.shape[1]
-    kernel_size = module.kernel_size
-    kernel_size_numel = module.weight.shape[2:].numel()
-
-    def make_weight():
-        weight = torch.zeros(kernel_size_numel, 1, *kernel_size)
-
-        for i in range(kernel_size_numel):
-            extraction = torch.zeros(kernel_size_numel)
-            extraction[i] = 1.0
-            weight[i] = extraction.reshape(1, *kernel_size)
-
-        repeat = [C_in, 1] + [1 for _ in kernel_size]
-        return weight.repeat(*repeat)
+def unfold_by_conv(input: Tensor, module: Union[Conv1d, Conv2d, Conv3d]) -> Tensor:
+    """Return the unfolded input using convolution.
 
-    conv_dim = input.dim() - 2
-    conv = get_conv_function(conv_dim)
+    Args:
+        input: Convolution layer input.
+        module: Convolution layer.
 
-    unfold = conv(
+    Returns:
+        Unfolded input. For a 2d convolution with input of shape `[N, C_in, *, *]`
+        and a kernel of shape `[_, _, K_H, K_W]`, this tensor has shape
+        `[N, C_in * K_H * K_W, L]` where `L` is the output's number of patches.
+    """
+    return unfoldNd(
         input,
-        make_weight().to(input.device),
-        bias=None,
-        stride=module.stride,
-        padding=module.padding,
+        module.kernel_size,
         dilation=module.dilation,
-        groups=C_in,
+        padding=module.padding,
+        stride=module.stride,
     )
 
-    return unfold.reshape(N, C_in * kernel_size_numel, -1)
-
 
 def _grad_input_padding(
-    grad_output, input_size, stride, padding, kernel_size, dilation=None
-):
+    grad_output: Tensor,
+    input_size: Tuple[int, ...],
+    stride: Tuple[int, ...],
+    padding: Tuple[int, ...],
+    kernel_size: Tuple[int, ...],
+    dilation: Union[None, Tuple[int]] = None,
+) -> Tuple[int, ...]:
     """Determine padding for the VJP of convolution.
 
+    # noqa: DAR101
+    # noqa: DAR201
+    # noqa: DAR401
+
     Note:
         This function was copied from the PyTorch repository (version 1.9).
         It was removed between torch 1.12.1 and torch 1.13.
     """
     if dilation is None:
         # For backward compatibility
         warn(
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/utils/conv_transpose.py` & `backpack-for-pytorch-1.6.0/backpack/utils/conv_transpose.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Utility functions for extracting transpose convolution BackPACK quantities."""
 
-from typing import Callable, Type
+from typing import Callable, Tuple, Type, Union
 
-import torch
 from einops import rearrange
-from torch import einsum
+from torch import Tensor, einsum
 from torch.nn import ConvTranspose1d, ConvTranspose2d, ConvTranspose3d, Module
 from torch.nn.functional import conv_transpose1d, conv_transpose2d, conv_transpose3d
+from unfoldNd import unfold_transposeNd
 
 from backpack.utils.conv import extract_bias_diagonal as conv_extract_bias_diagonal
 
 
 def get_conv_transpose_module(N: int) -> Type[Module]:
     """Return the PyTorch module class of N-dimensional transpose convolution.
 
@@ -39,122 +39,116 @@
     return {
         1: conv_transpose1d,
         2: conv_transpose2d,
         3: conv_transpose3d,
     }[N]
 
 
-def get_weight_gradient_factors(input, grad_out, module):
-    M, C_in = input.shape[0], input.shape[1]
-    kernel_size_numel = module.weight.shape[2:].numel()
+def get_weight_gradient_factors(
+    input: Tensor,
+    grad_out: Tensor,
+    module: Union[ConvTranspose1d, ConvTranspose2d, ConvTranspose3d],
+) -> Tuple[Tensor, Tensor]:
+    """Return factors for computing gradients w.r.t. the kernel.
 
-    X = unfold_by_conv_transpose(input, module).reshape(M, C_in * kernel_size_numel, -1)
+    Args:
+        input: Input to the transpose convolution layer.
+        grad_out: Gradient w.r.t. the transpose convolution layer's output.
+        module: Transpose convolution layer.
+
+    Returns:
+        unfolded input, output gradient with flattened spatial dimensions
+    """
+    X = unfold_by_conv_transpose(input, module)
     dE_dY = rearrange(grad_out, "n c ... -> n c (...)")
 
     return X, dE_dY
 
 
-def extract_weight_diagonal(module, unfolded_input, S, sum_batch=True):
+def extract_weight_diagonal(
+    module: Union[ConvTranspose1d, ConvTranspose2d, ConvTranspose3d],
+    unfolded_input: Tensor,
+    S: Tensor,
+    sum_batch: bool = True,
+) -> Tensor:
     """Extract diagonal of ``(Jᵀ S) (Jᵀ S)ᵀ`` where ``J`` is the weight Jacobian.
 
     Args:
-        module (torch.nn.ConvTranspose1d or torch.nn.ConvTranspose2d or
-            torch.nn.ConvTranspose3d ): Convolution layer for which the diagonal is
-            extracted w.r.t. the weight.
-        unfolded_input (torch.Tensor): Unfolded input to the transpose convolution.
-        S (torch.Tensor): Backpropagated (symmetric factorization) of the loss Hessian.
+        module: Convolution layer for which the diagonal is extracted w.r.t. the weight.
+        unfolded_input: Unfolded input to the transpose convolution.
+        S: Backpropagated (symmetric factorization) of the loss Hessian.
             Has shape ``(V, *module.output.shape)``.
-        sum_batch (bool, optional): Sum out the batch dimension of the weight diagonals.
+        sum_batch: Sum out the batch dimension of the weight diagonals.
             Default value: ``True``.
 
     Returns:
-        torch.Tensor: Per-sample weight diagonal if ``sum_batch=False`` (shape
-            ``(N, module.weight.shape)`` with batch size ``N``) or summed weight
-            diagonal if ``sum_batch=True`` (shape ``module.weight.shape``).
+        Per-sample weight diagonal if ``sum_batch=False`` (shape
+        ``(N, module.weight.shape)`` with batch size ``N``) or summed weight
+        diagonal if ``sum_batch=True`` (shape ``module.weight.shape``).
     """
     S = rearrange(S, "v n (g o) ... -> v n g o (...)", g=module.groups)
     unfolded_input = rearrange(
         unfolded_input,
-        "n (g c) (k x) -> n g c k x",
+        "n (g c k) x -> n g c k x",
         g=module.groups,
         k=module.weight.shape[2:].numel(),
     )
 
-    JS = einsum("ngckx,vngox->vngcok", (unfolded_input, S))
+    JS = einsum("ngckx,vngox->vngcok", unfolded_input, S)
 
     sum_dims = [0, 1] if sum_batch else [0]
     out_shape = (
         module.weight.shape if sum_batch else (JS.shape[1], *module.weight.shape)
     )
 
-    weight_diagonal = JS.pow_(2).sum(sum_dims).reshape(out_shape)
-
-    return weight_diagonal
+    return JS.pow_(2).sum(sum_dims).reshape(out_shape)
 
 
 # TODO This method applies the bias Jacobian, then squares and sums the result. Intro-
 # duce base class for {Batch}DiagHessian and DiagGGN{Exact,MC} and remove this method
-def extract_bias_diagonal(module, S, sum_batch=True):
+def extract_bias_diagonal(
+    module: Union[ConvTranspose1d, ConvTranspose2d, ConvTranspose3d],
+    S: Tensor,
+    sum_batch: bool = True,
+) -> Tensor:
     """Extract diagonal of ``(Jᵀ S) (Jᵀ S)ᵀ`` where ``J`` is the weight Jacobian.
 
     Args:
-        module (torch.nn.ConvTranspose1d or torch.nn.ConvTranspose2d or
-            torch.nn.ConvTranspose3d ): Convolution layer for which the diagonal is
-            extracted w.r.t. the bias.
-        unfolded_input (torch.Tensor): Unfolded input to the transpose convolution.
-        S (torch.Tensor): Backpropagated (symmetric factorization) of the loss Hessian.
+        module: Convolution layer for which the diagonal is extracted w.r.t. the bias.
+        S: Backpropagated (symmetric factorization) of the loss Hessian.
             Has shape ``(V, *module.output.shape)``.
-        sum_batch (bool, optional): Sum out the batch dimension of the bias diagonals.
+        sum_batch: Sum out the batch dimension of the bias diagonals.
             Default value: ``True``.
 
     Returns:
-        torch.Tensor: Per-sample bias diagonal if ``sum_batch=False`` (shape
-            ``(N, module.bias.shape)`` with batch size ``N``) or summed bias
-            diagonal if ``sum_batch=True`` (shape ``module.bias.shape``).
+        Per-sample bias diagonal if ``sum_batch=False`` (shape
+        ``(N, module.bias.shape)`` with batch size ``N``) or summed bias
+        diagonal if ``sum_batch=True`` (shape ``module.bias.shape``).
     """
     return conv_extract_bias_diagonal(module, S, sum_batch=sum_batch)
 
 
-def unfold_by_conv_transpose(input, module):
+def unfold_by_conv_transpose(
+    input: Tensor, module: Union[ConvTranspose1d, ConvTranspose2d, ConvTranspose3d]
+) -> Tensor:
     """Return the unfolded input using one-hot transpose convolution.
 
     Args:
-        input (torch.Tensor): Input to a transpose convolution.
-        module (torch.nn.ConvTranspose1d or torch.nn.ConvTranspose2d or
-            torch.nn.ConvTranspose3d): Transpose convolution layer that specifies
-            the hyperparameters for unfolding.
+        input: Input to a transpose convolution.
+        module: Transpose convolution layer that specifies the hyperparameters for
+            unfolding.
 
     Returns:
-        torch.Tensor: Unfolded input of shape ``(N, C, K * X)`` with
-            ``K = module.weight.shape[2:].numel()`` the number of kernel elements
-            and ``X = module.output.shape[2:].numel()`` the number of output pixels.
+        Unfolded input of shape ``(N, C * K, X)`` with
+        ``K = module.weight.shape[2:].numel()`` the number of kernel elements
+        and ``X = module.output.shape[2:].numel()`` the number of output pixels.
     """
-    N, C_in = input.shape[0], input.shape[1]
-    kernel_size = module.kernel_size
-    kernel_size_numel = module.weight.shape[2:].numel()
-
-    def make_weight():
-        weight = torch.zeros(1, kernel_size_numel, *kernel_size)
-
-        for i in range(kernel_size_numel):
-            extraction = torch.zeros(kernel_size_numel)
-            extraction[i] = 1.0
-            weight[0, i] = extraction.reshape(*kernel_size)
-
-        repeat = [C_in, 1] + [1 for _ in kernel_size]
-        weight = weight.repeat(*repeat)
-        return weight.to(module.weight.device)
-
-    conv_dim = input.dim() - 2
-    conv_transpose = get_conv_transpose_function(conv_dim)
-
-    unfold = conv_transpose(
+    return unfold_transposeNd(
         input,
-        make_weight().to(module.weight.device),
-        bias=None,
+        module.kernel_size,
         stride=module.stride,
         padding=module.padding,
+        # TODO The case where output_size is specified in the forward pass of a
+        # ConvTransposeNd is not handled
+        output_padding=0,
         dilation=module.dilation,
-        groups=C_in,
     )
-
-    return unfold.reshape(N, C_in, -1)
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/utils/convert_parameters.py` & `backpack-for-pytorch-1.6.0/backpack/utils/convert_parameters.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/utils/errors.py` & `backpack-for-pytorch-1.6.0/backpack/utils/errors.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/utils/examples.py` & `backpack-for-pytorch-1.6.0/backpack/utils/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,28 +36,32 @@
     Returns:
         MNIST dataloader
     """
     return DataLoader(load_mnist_dataset(), batch_size=batch_size, shuffle=shuffle)
 
 
 def load_one_batch_mnist(
-    batch_size: int = 64, shuffle: bool = True
+    batch_size: int = 64, shuffle: bool = True, flat: bool = False
 ) -> Tuple[Tensor, Tensor]:
     """Return a single mini-batch (inputs, labels) from MNIST.
 
     Args:
         batch_size: Mini-batch size. Default: ``64``.
         shuffle: Randomly shuffle the data. Default: ``True``.
+        flat: Flatten chanel and returns a matrix ``[batch_size x 784]``
 
     Returns:
         A single batch (inputs, labels) from MNIST.
     """
     dataloader = get_mnist_dataloader(batch_size, shuffle)
     X, y = next(iter(dataloader))
 
+    if flat:
+        X = X.reshape(X.shape[0], -1)
+
     return X, y
 
 
 def autograd_diag_ggn_exact(
     X: Tensor, y: Tensor, model: Module, loss_function: Module, idx: List[int] = None
 ) -> Tensor:
     """Compute the generalized Gauss-Newton diagonal with ``torch.autograd``.
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/utils/kroneckers.py` & `backpack-for-pytorch-1.6.0/backpack/utils/kroneckers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from torch import einsum
+from torch.linalg import eigh
 
 from backpack.utils.unsqueeze import kfacmp_unsqueeze_if_missing_dim
 
 
 def kfacs_to_mat(factors):
     """Given [A, B, C, ...], return A ⊗ B ⊗ C ⊗ ... ."""
     mat = None
@@ -97,15 +98,15 @@
 
     def sym_mat_inv(mat, shift, truncate=1e-8):
         """Inverse of a symmetric matrix A -> (A + 𝜆I)⁻¹.
 
         Computed by eigenvalue decomposition. Eigenvalues with small
         absolute values are truncated.
         """
-        eigvals, eigvecs = mat.symeig(eigenvectors=True)
+        eigvals, eigvecs = eigh(mat)
         eigvals.add_(shift)
         inv_eigvals = 1.0 / eigvals
         inv_truncate = 1.0 / truncate
         inv_eigvals.clamp_(min=-inv_truncate, max=inv_truncate)
         return einsum("ij,j,kj->ik", (eigvecs, inv_eigvals, eigvecs))
 
     shifts = make_shifts()
```

### Comparing `backpack-for-pytorch-1.5.2/backpack/utils/linear.py` & `backpack-for-pytorch-1.6.0/backpack/utils/linear.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/utils/subsampling.py` & `backpack-for-pytorch-1.6.0/backpack/utils/subsampling.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack/utils/unsqueeze.py` & `backpack-for-pytorch-1.6.0/backpack/utils/unsqueeze.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/backpack_for_pytorch.egg-info/PKG-INFO` & `backpack-for-pytorch-1.6.0/backpack_for_pytorch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: backpack-for-pytorch
-Version: 1.5.2
+Version: 1.6.0
 Summary: BackPACK: Packing more into backprop
 Home-page: https://github.com/f-dangel/backpack
 Author: Felix Dangel, Frederik Kunstner
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 # <img alt="BackPACK" src="./logo/backpack_logo_torch.svg" height="90"> BackPACK: Packing more into backprop
 
 [![Travis](https://travis-ci.org/f-dangel/backpack.svg?branch=master)](https://travis-ci.org/f-dangel/backpack)
 [![Coveralls](https://coveralls.io/repos/github/f-dangel/backpack/badge.svg?branch=master)](https://coveralls.io/github/f-dangel/backpack)
-[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-370/)
 
 BackPACK is built on top of [PyTorch](https://github.com/pytorch/pytorch). It efficiently computes quantities other than the gradient.
 
 - **Website:** https://backpack.pt
 - **Documentation:** https://docs.backpack.pt/en/master/
 - **Bug reports & feature requests:** https://github.com/f-dangel/backpack/issues
```

### Comparing `backpack-for-pytorch-1.5.2/backpack_for_pytorch.egg-info/SOURCES.txt` & `backpack-for-pytorch-1.6.0/backpack_for_pytorch.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 backpack/core/derivatives/adaptive_avg_pool_nd.py
 backpack/core/derivatives/avgpool1d.py
 backpack/core/derivatives/avgpool2d.py
 backpack/core/derivatives/avgpool3d.py
 backpack/core/derivatives/avgpoolnd.py
 backpack/core/derivatives/basederivatives.py
 backpack/core/derivatives/batchnorm_nd.py
+backpack/core/derivatives/bcewithlogitsloss.py
 backpack/core/derivatives/conv1d.py
 backpack/core/derivatives/conv2d.py
 backpack/core/derivatives/conv3d.py
 backpack/core/derivatives/conv_transpose1d.py
 backpack/core/derivatives/conv_transpose2d.py
 backpack/core/derivatives/conv_transpose3d.py
 backpack/core/derivatives/conv_transposend.py
@@ -45,14 +46,15 @@
 backpack/core/derivatives/logsigmoid.py
 backpack/core/derivatives/lstm.py
 backpack/core/derivatives/maxpool1d.py
 backpack/core/derivatives/maxpool2d.py
 backpack/core/derivatives/maxpool3d.py
 backpack/core/derivatives/maxpoolnd.py
 backpack/core/derivatives/mseloss.py
+backpack/core/derivatives/nll_base.py
 backpack/core/derivatives/pad.py
 backpack/core/derivatives/permute.py
 backpack/core/derivatives/relu.py
 backpack/core/derivatives/rnn.py
 backpack/core/derivatives/scale_module.py
 backpack/core/derivatives/selu.py
 backpack/core/derivatives/shape_check.py
@@ -210,15 +212,22 @@
 backpack/extensions/secondorder/diag_hessian/losses.py
 backpack/extensions/secondorder/diag_hessian/pad.py
 backpack/extensions/secondorder/diag_hessian/padding.py
 backpack/extensions/secondorder/diag_hessian/pooling.py
 backpack/extensions/secondorder/diag_hessian/slicing.py
 backpack/extensions/secondorder/hbp/__init__.py
 backpack/extensions/secondorder/hbp/activations.py
+backpack/extensions/secondorder/hbp/conv1d.py
 backpack/extensions/secondorder/hbp/conv2d.py
+backpack/extensions/secondorder/hbp/conv3d.py
+backpack/extensions/secondorder/hbp/conv_transpose1d.py
+backpack/extensions/secondorder/hbp/conv_transpose2d.py
+backpack/extensions/secondorder/hbp/conv_transpose3d.py
+backpack/extensions/secondorder/hbp/conv_transposend.py
+backpack/extensions/secondorder/hbp/convnd.py
 backpack/extensions/secondorder/hbp/custom_module.py
 backpack/extensions/secondorder/hbp/dropout.py
 backpack/extensions/secondorder/hbp/flatten.py
 backpack/extensions/secondorder/hbp/hbp_options.py
 backpack/extensions/secondorder/hbp/hbpbase.py
 backpack/extensions/secondorder/hbp/linear.py
 backpack/extensions/secondorder/hbp/losses.py
@@ -295,28 +304,31 @@
 docs/assets/img/updaterule.png
 docs/assets/js/scale.fix.js
 docs/script/bootstrap
 docs/script/cibuild
 docs/script/release
 docs/script/validate-html
 docs_src/.gitignore
+docs_src/CNAME
 docs_src/README.md
 docs_src/buildweb.sh
 docs_src/examples/cheatsheet.pdf
 docs_src/examples/basic_usage/README.rst
 docs_src/examples/basic_usage/example_all_in_one.py
 docs_src/examples/use_cases/README.rst
+docs_src/examples/use_cases/example_batched_jacobians.py
 docs_src/examples/use_cases/example_cg_newton.py
 docs_src/examples/use_cases/example_custom_module.py
 docs_src/examples/use_cases/example_diag_ggn_optimizer.py
 docs_src/examples/use_cases/example_differential_privacy.py
 docs_src/examples/use_cases/example_extension_hook.py
 docs_src/examples/use_cases/example_first_order_resnet.py
 docs_src/examples/use_cases/example_gradient_of_variance.py
 docs_src/examples/use_cases/example_resnet_all_in_one.py
+docs_src/examples/use_cases/example_retain_graph.py
 docs_src/examples/use_cases/example_rnn.py
 docs_src/examples/use_cases/example_save_memory_convolutions.py
 docs_src/examples/use_cases/example_subsampling.py
 docs_src/examples/use_cases/example_trace_estimation.py
 docs_src/rtd/.gitignore
 docs_src/rtd/.nojekyll
 docs_src/rtd/Makefile
@@ -489,14 +501,16 @@
 test/extensions/secondorder/sqrt_ggn/sqrt_ggn_settings.py
 test/extensions/secondorder/sqrt_ggn/test_sqrt_ggn.py
 test/implementation/__init__.py
 test/implementation/implementation.py
 test/implementation/implementation_autograd.py
 test/implementation/implementation_bpext.py
 test/utils/__init__.py
+test/utils/conv_transpose.py
 test/utils/evaluation_mode.py
+test/utils/skip_extension_test.py
 test/utils/skip_test.py
 test/utils/test_conv.py
 test/utils/test_conv_settings.py
 test/utils/test_conv_transpose.py
 test/utils/test_conv_transpose_settings.py
 test/utils/test_subsampling.py
```

### Comparing `backpack-for-pytorch-1.5.2/changelog.md` & `backpack-for-pytorch-1.6.0/changelog.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,84 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.6.0] - 2023-06-26
+
+With this patch, BackPACK supports `torch==2.x` and deprecates `python3.7`
+([PR](https://github.com/f-dangel/backpack/pull/307)). BackPACK now supports
+`BCEWithLogitsLoss`, and supports KFAC for N-dimensional (transpose)
+convolutions.
+
+### Added/New
+- Example use case for `retain_graph`
+  ([PR](https://github.com/f-dangel/backpack/pull/302))
+- Example for computing batched Jacobians
+  ([PR](https://github.com/f-dangel/backpack/pull/267))
+- Support `BCEWithLogitsLoss`
+  - `BatchDiagHessian` and `DiagHessian` extensions
+    ([PR](https://github.com/f-dangel/backpack/pull/279))
+  - `BatchDiagGGN` (exact, MC) and `DiagGGN` (exact, MC) extensions
+    ([PR](https://github.com/f-dangel/backpack/pull/280))
+  - `KFAC` extension
+    ([PR](https://github.com/f-dangel/backpack/pull/283))
+  - `KFLR` extension
+    ([PR](https://github.com/f-dangel/backpack/pull/284))
+- Extend `KFAC, KFLR, KFRA` to N-dimensional convolutions (and transpose
+  convolutions) ([blog post](https://fdangel.com/posts/kfac_explained.html))
+  - Support for `Conv{1,2,3}d`
+    ([PR](https://github.com/f-dangel/backpack/pull/291))
+  - Support for `ConvTranspose{1,2,3}d`
+    ([PR](https://github.com/f-dangel/backpack/pull/292))
+
+### Fixed/Removed
+- Use correct imports on website code samples
+  ([PR](https://github.com/f-dangel/backpack/pull/262))
+
+### Internal
+- Update code to latest `black` and `flake8`
+  ([PR](https://github.com/f-dangel/backpack/pull/301))
+- Fix examples on splash page
+  ([PR](https://github.com/f-dangel/backpack/pull/298))
+- Abstract negative log-likelihood losses in core
+  ([PR](https://github.com/f-dangel/backpack/pull/252))
+  - Apply to `MSELoss` derivatives
+    ([PR](https://github.com/f-dangel/backpack/pull/252))
+  - Apply to `CrossEntropyLoss` derivatives
+    ([PR](https://github.com/f-dangel/backpack/pull/256))
+  - Implement `BCEWithLogitsLoss` derivatives
+    ([PR](https://github.com/f-dangel/backpack/pull/257))
+- Implement second-order derivatives of `BCEWithLogitsLoss`
+  ([PR](https://github.com/f-dangel/backpack/pull/271))
+- Implement optimized sampled gradients for `BCEWithLogitsLoss`
+  ([PR](https://github.com/f-dangel/backpack/pull/278))
+- Use batch size 1 in KFAC tests for ResNets
+  ([PR](https://github.com/f-dangel/backpack/pull/265))
+- Test with PyTorch `1.9.0` and `1.12.0` and make tests compatible
+  ([PR](https://github.com/f-dangel/backpack/pull/277))
+- Use `unfoldNd` package
+  - For input unfolding of convolutions
+    ([PR](https://github.com/f-dangel/backpack/pull/285))
+  - For input unfolding of transpose convolutions
+    ([PR](https://github.com/f-dangel/backpack/pull/287))
+- Fully-document utility functions for convolutions
+  ([PR](https://github.com/f-dangel/backpack/pull/286))
+- Make output shape of unfolded input of transpose convolution consistent with
+  convolution case
+  ([PR](https://github.com/f-dangel/backpack/pull/289))
+- Fully-document `HBPConv2d` class
+  ([PR](https://github.com/f-dangel/backpack/pull/290))
+- Fix support for PyTorch 1.13
+  ([PR](https://github.com/f-dangel/backpack/pull/296))
+- Update linting and formatting to latest `black`, `flake8`
+  ([PR](https://github.com/f-dangel/backpack/pull/301))
+
 ## [1.5.2] - 2022-12-19
 
 This patch adds support for `torch>=1.13.0` to BackPACK.
 
 ## [1.5.1] - 2022-11-03
 
 This patch fixes temporary compatibility issues with the latest PyTorch release.
@@ -386,15 +456,16 @@
 ### Fixed
 - Fixed PyPI installaton
 
 ## [1.0.0] - 2019-10-03
 
 Initial release
 
-[Unreleased]: https://github.com/f-dangel/backpack/compare/v1.5.2...HEAD
+[Unreleased]: https://github.com/f-dangel/backpack/compare/v1.6.0...HEAD
+[1.6.0]: https://github.com/f-dangel/backpack/compare/1.5.2...1.6.0
 [1.5.2]: https://github.com/f-dangel/backpack/compare/1.5.2...1.5.1
 [1.5.1]: https://github.com/f-dangel/backpack/compare/1.5.1...1.5.0
 [1.5.0]: https://github.com/f-dangel/backpack/compare/1.5.0...1.4.0
 [1.4.0]: https://github.com/f-dangel/backpack/compare/1.4.0...1.3.0
 [1.3.0]: https://github.com/f-dangel/backpack/compare/1.3.0...1.2.0
 [1.2.0]: https://github.com/f-dangel/backpack/compare/1.2.0...1.1.1
 [1.1.1]: https://github.com/f-dangel/backpack/compare/1.1.0...1.1.1
```

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/css/style.css` & `backpack-for-pytorch-1.6.0/docs/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.eot` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.eot`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.svg` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.svg`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.ttf` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.ttf`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff2` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff2`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.eot` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.eot`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.svg` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.svg`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.ttf` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.ttf`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff2` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff2`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.eot` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.eot`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.svg` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.svg`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.ttf` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.ttf`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff2` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff2`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.eot` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.eot`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.svg` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.svg`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.ttf` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.ttf`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff2` & `backpack-for-pytorch-1.6.0/docs/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff2`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/img/backpack_logo_torch.svg` & `backpack-for-pytorch-1.6.0/docs/assets/img/backpack_logo_torch.svg`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/img/logo.png` & `backpack-for-pytorch-1.6.0/docs/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/img/updaterule.png` & `backpack-for-pytorch-1.6.0/docs/assets/img/updaterule.png`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/assets/js/scale.fix.js` & `backpack-for-pytorch-1.6.0/docs/assets/js/scale.fix.js`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/examples.html` & `backpack-for-pytorch-1.6.0/docs/examples.html`

 * *Files 10% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 
 <p>This small example shows how to use BackPACK to implement a simple second-order optimizer.
 It follows <a href="https://github.com/pytorch/examples/tree/master/mnist">the traditional PyTorch MNIST example</a>.</p>
 
 <h2 id="installation">Installation</h2>
 
 <p>For this example to run, you will need <a href="https://pytorch.org/get-started/locally/">PyTorch and TorchVision (&gt;= 1.0)</a>
-To install BackPACK, either use <code class="highlighter-rouge">pip</code> or <a href="https://github.com/f-dangel/backpack">clone the repo</a>.</p>
-<div class="highlighter-rouge"><div class="highlight"><pre class="highlight"><code>pip install backpack-for-pytorch
+To install BackPACK, either use <code class="language-plaintext highlighter-rouge">pip</code> or <a href="https://github.com/f-dangel/backpack">clone the repo</a>.</p>
+<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>pip install backpack-for-pytorch
 </code></pre></div></div>
 
 <h2 id="an-example-diagonal-ggn-preconditioner">An example: Diagonal GGN Preconditioner</h2>
 
 <p>You can find the code 
 <a href="https://docs.backpack.pt/en/master/use_cases/example_diag_ggn_optimizer.html">in the documentation</a>.
 It runs SGD with a preconditioner based on the diagonal of the GGN.</p>
@@ -86,140 +86,140 @@
 </span><span class="kn">from</span> <span class="nn">backpack.core.layers</span> <span class="kn">import</span> <span class="n">Flatten</span>
 
 <span class="c1"># Hyperparameters
 </span><span class="n">BATCH_SIZE</span> <span class="o">=</span> <span class="mi">64</span>
 <span class="n">STEP_SIZE</span> <span class="o">=</span> <span class="mf">0.01</span>
 <span class="n">DAMPING</span> <span class="o">=</span> <span class="mf">1.0</span>
 <span class="n">MAX_ITER</span> <span class="o">=</span> <span class="mi">100</span>
-<span class="n">torch</span><span class="o">.</span><span class="n">manual_seed</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+<span class="n">torch</span><span class="p">.</span><span class="n">manual_seed</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
 </code></pre></div></div>
 
 <p>Now, let’s load MNIST</p>
 
 <div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code>
-<span class="n">mnist_loader</span> <span class="o">=</span> <span class="n">torch</span><span class="o">.</span><span class="n">utils</span><span class="o">.</span><span class="n">data</span><span class="o">.</span><span class="n">dataloader</span><span class="o">.</span><span class="n">DataLoader</span><span class="p">(</span>
-    <span class="n">torchvision</span><span class="o">.</span><span class="n">datasets</span><span class="o">.</span><span class="n">MNIST</span><span class="p">(</span>
+<span class="n">mnist_loader</span> <span class="o">=</span> <span class="n">torch</span><span class="p">.</span><span class="n">utils</span><span class="p">.</span><span class="n">data</span><span class="p">.</span><span class="n">dataloader</span><span class="p">.</span><span class="n">DataLoader</span><span class="p">(</span>
+    <span class="n">torchvision</span><span class="p">.</span><span class="n">datasets</span><span class="p">.</span><span class="n">MNIST</span><span class="p">(</span>
         <span class="s">'./data'</span><span class="p">,</span>
         <span class="n">train</span><span class="o">=</span><span class="bp">True</span><span class="p">,</span>
         <span class="n">download</span><span class="o">=</span><span class="bp">True</span><span class="p">,</span>
-        <span class="n">transform</span><span class="o">=</span><span class="n">torchvision</span><span class="o">.</span><span class="n">transforms</span><span class="o">.</span><span class="n">Compose</span><span class="p">([</span>
-            <span class="n">torchvision</span><span class="o">.</span><span class="n">transforms</span><span class="o">.</span><span class="n">ToTensor</span><span class="p">(),</span>
-            <span class="n">torchvision</span><span class="o">.</span><span class="n">transforms</span><span class="o">.</span><span class="n">Normalize</span><span class="p">(</span>
+        <span class="n">transform</span><span class="o">=</span><span class="n">torchvision</span><span class="p">.</span><span class="n">transforms</span><span class="p">.</span><span class="n">Compose</span><span class="p">([</span>
+            <span class="n">torchvision</span><span class="p">.</span><span class="n">transforms</span><span class="p">.</span><span class="n">ToTensor</span><span class="p">(),</span>
+            <span class="n">torchvision</span><span class="p">.</span><span class="n">transforms</span><span class="p">.</span><span class="n">Normalize</span><span class="p">(</span>
                 <span class="p">(</span><span class="mf">0.1307</span><span class="p">,),</span> <span class="p">(</span><span class="mf">0.3081</span><span class="p">,)</span>
             <span class="p">)</span>
         <span class="p">])),</span>
     <span class="n">batch_size</span><span class="o">=</span><span class="n">BATCH_SIZE</span><span class="p">,</span>
     <span class="n">shuffle</span><span class="o">=</span><span class="bp">True</span>
 <span class="p">)</span>
 
 </code></pre></div></div>
 
-<p>We’ll create a small CNN with MaxPooling and ReLU activations, using a <a href="https://pytorch.org/docs/stable/nn.html#sequential"><code class="highlighter-rouge">Sequential</code></a> layer as the main model.</p>
+<p>We’ll create a small CNN with MaxPooling and ReLU activations, using a <a href="https://pytorch.org/docs/stable/nn.html#sequential"><code class="language-plaintext highlighter-rouge">Sequential</code></a> layer as the main model.</p>
 
-<div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="n">model</span> <span class="o">=</span> <span class="n">torch</span><span class="o">.</span><span class="n">nn</span><span class="o">.</span><span class="n">Sequential</span><span class="p">(</span>
-    <span class="n">torch</span><span class="o">.</span><span class="n">nn</span><span class="o">.</span><span class="n">Conv2d</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">20</span><span class="p">,</span> <span class="mi">5</span><span class="p">,</span> <span class="mi">1</span><span class="p">),</span>
-    <span class="n">torch</span><span class="o">.</span><span class="n">nn</span><span class="o">.</span><span class="n">ReLU</span><span class="p">(),</span>
-    <span class="n">torch</span><span class="o">.</span><span class="n">nn</span><span class="o">.</span><span class="n">MaxPool2d</span><span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="mi">2</span><span class="p">),</span>
-    <span class="n">torch</span><span class="o">.</span><span class="n">nn</span><span class="o">.</span><span class="n">Conv2d</span><span class="p">(</span><span class="mi">20</span><span class="p">,</span> <span class="mi">50</span><span class="p">,</span> <span class="mi">5</span><span class="p">,</span> <span class="mi">1</span><span class="p">),</span>
-    <span class="n">torch</span><span class="o">.</span><span class="n">nn</span><span class="o">.</span><span class="n">ReLU</span><span class="p">(),</span>
-    <span class="n">torch</span><span class="o">.</span><span class="n">nn</span><span class="o">.</span><span class="n">MaxPool2d</span><span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="mi">2</span><span class="p">),</span>
+<div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="n">model</span> <span class="o">=</span> <span class="n">torch</span><span class="p">.</span><span class="n">nn</span><span class="p">.</span><span class="n">Sequential</span><span class="p">(</span>
+    <span class="n">torch</span><span class="p">.</span><span class="n">nn</span><span class="p">.</span><span class="n">Conv2d</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">20</span><span class="p">,</span> <span class="mi">5</span><span class="p">,</span> <span class="mi">1</span><span class="p">),</span>
+    <span class="n">torch</span><span class="p">.</span><span class="n">nn</span><span class="p">.</span><span class="n">ReLU</span><span class="p">(),</span>
+    <span class="n">torch</span><span class="p">.</span><span class="n">nn</span><span class="p">.</span><span class="n">MaxPool2d</span><span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="mi">2</span><span class="p">),</span>
+    <span class="n">torch</span><span class="p">.</span><span class="n">nn</span><span class="p">.</span><span class="n">Conv2d</span><span class="p">(</span><span class="mi">20</span><span class="p">,</span> <span class="mi">50</span><span class="p">,</span> <span class="mi">5</span><span class="p">,</span> <span class="mi">1</span><span class="p">),</span>
+    <span class="n">torch</span><span class="p">.</span><span class="n">nn</span><span class="p">.</span><span class="n">ReLU</span><span class="p">(),</span>
+    <span class="n">torch</span><span class="p">.</span><span class="n">nn</span><span class="p">.</span><span class="n">MaxPool2d</span><span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="mi">2</span><span class="p">),</span>
     <span class="n">Flatten</span><span class="p">(),</span> 
     <span class="c1"># Pytorch &lt;1.2 doesn't have a Flatten layer
-</span>    <span class="n">torch</span><span class="o">.</span><span class="n">nn</span><span class="o">.</span><span class="n">Linear</span><span class="p">(</span><span class="mi">4</span><span class="o">*</span><span class="mi">4</span><span class="o">*</span><span class="mi">50</span><span class="p">,</span> <span class="mi">500</span><span class="p">),</span>
-    <span class="n">torch</span><span class="o">.</span><span class="n">nn</span><span class="o">.</span><span class="n">ReLU</span><span class="p">(),</span>
-    <span class="n">torch</span><span class="o">.</span><span class="n">nn</span><span class="o">.</span><span class="n">Linear</span><span class="p">(</span><span class="mi">500</span><span class="p">,</span> <span class="mi">10</span><span class="p">),</span>
+</span>    <span class="n">torch</span><span class="p">.</span><span class="n">nn</span><span class="p">.</span><span class="n">Linear</span><span class="p">(</span><span class="mi">4</span><span class="o">*</span><span class="mi">4</span><span class="o">*</span><span class="mi">50</span><span class="p">,</span> <span class="mi">500</span><span class="p">),</span>
+    <span class="n">torch</span><span class="p">.</span><span class="n">nn</span><span class="p">.</span><span class="n">ReLU</span><span class="p">(),</span>
+    <span class="n">torch</span><span class="p">.</span><span class="n">nn</span><span class="p">.</span><span class="n">Linear</span><span class="p">(</span><span class="mi">500</span><span class="p">,</span> <span class="mi">10</span><span class="p">),</span>
 <span class="p">)</span>
 
 </code></pre></div></div>
 
 <p>We will also need a loss function and a way to measure accuracy</p>
 
-<div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="n">loss_function</span> <span class="o">=</span> <span class="n">torch</span><span class="o">.</span><span class="n">nn</span><span class="o">.</span><span class="n">CrossEntropyLoss</span><span class="p">()</span>
+<div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="n">loss_function</span> <span class="o">=</span> <span class="n">torch</span><span class="p">.</span><span class="n">nn</span><span class="p">.</span><span class="n">CrossEntropyLoss</span><span class="p">()</span>
 
 <span class="k">def</span> <span class="nf">get_accuracy</span><span class="p">(</span><span class="n">output</span><span class="p">,</span> <span class="n">targets</span><span class="p">):</span>
     <span class="s">"""Helper function to print the accuracy"""</span>
-    <span class="n">predictions</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">argmax</span><span class="p">(</span><span class="n">dim</span><span class="o">=</span><span class="mi">1</span><span class="p">,</span> <span class="n">keepdim</span><span class="o">=</span><span class="bp">True</span><span class="p">)</span><span class="o">.</span><span class="n">view_as</span><span class="p">(</span><span class="n">targets</span><span class="p">)</span>
-    <span class="k">return</span> <span class="n">predictions</span><span class="o">.</span><span class="n">eq</span><span class="p">(</span><span class="n">targets</span><span class="p">)</span><span class="o">.</span><span class="nb">float</span><span class="p">()</span><span class="o">.</span><span class="n">mean</span><span class="p">()</span><span class="o">.</span><span class="n">item</span><span class="p">()</span><span class="sb">``</span><span class="err">`</span>
+    <span class="n">predictions</span> <span class="o">=</span> <span class="n">output</span><span class="p">.</span><span class="n">argmax</span><span class="p">(</span><span class="n">dim</span><span class="o">=</span><span class="mi">1</span><span class="p">,</span> <span class="n">keepdim</span><span class="o">=</span><span class="bp">True</span><span class="p">).</span><span class="n">view_as</span><span class="p">(</span><span class="n">targets</span><span class="p">)</span>
+    <span class="k">return</span> <span class="n">predictions</span><span class="p">.</span><span class="n">eq</span><span class="p">(</span><span class="n">targets</span><span class="p">).</span><span class="nb">float</span><span class="p">().</span><span class="n">mean</span><span class="p">().</span><span class="n">item</span><span class="p">()</span><span class="sb">``</span><span class="err">`</span>
 
 </code></pre></div></div>
 
 <h3 id="step-2-the-optimizer">Step 2: The optimizer</h3>
 
 <p>The update rule we want to implement is a precondionned gradient descent, 
 using the diagonal of the generalized Gauss-Newton,</p>
 
 <center>
 <img src="assets/img/updaterule.png" width="60%" />
 </center>
 
-<p>where <code class="highlighter-rouge">𝛼</code> is the step-size, <code class="highlighter-rouge">𝜆</code> is the damping parameter, <code class="highlighter-rouge">g</code> is the gradient and <code class="highlighter-rouge">G</code> is the diagonal of the generalized Gauss-Newton (GGN).
-The difficult part is computing <code class="highlighter-rouge">G</code>, but BackPACK will do this;
-just like PyTorch’s autograd compute the gradient for each parameter <code class="highlighter-rouge">p</code> and store it in <code class="highlighter-rouge">p.grad</code>, BackPACK with the <code class="highlighter-rouge">DiagGGNMC</code> extension will compute (a Monte-Carlo estimate of) the diagonal of the GGN and store it in <code class="highlighter-rouge">p.diag_ggn_mc</code>.
+<p>where <code class="language-plaintext highlighter-rouge">𝛼</code> is the step-size, <code class="language-plaintext highlighter-rouge">𝜆</code> is the damping parameter, <code class="language-plaintext highlighter-rouge">g</code> is the gradient and <code class="language-plaintext highlighter-rouge">G</code> is the diagonal of the generalized Gauss-Newton (GGN).
+The difficult part is computing <code class="language-plaintext highlighter-rouge">G</code>, but BackPACK will do this;
+just like PyTorch’s autograd compute the gradient for each parameter <code class="language-plaintext highlighter-rouge">p</code> and store it in <code class="language-plaintext highlighter-rouge">p.grad</code>, BackPACK with the <code class="language-plaintext highlighter-rouge">DiagGGNMC</code> extension will compute (a Monte-Carlo estimate of) the diagonal of the GGN and store it in <code class="language-plaintext highlighter-rouge">p.diag_ggn_mc</code>.
 We can now simply focus on implementing the optimizer that uses this information:</p>
 
-<div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="k">class</span> <span class="nc">DiagGGNOptimizer</span><span class="p">(</span><span class="n">torch</span><span class="o">.</span><span class="n">optim</span><span class="o">.</span><span class="n">Optimizer</span><span class="p">):</span>
+<div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="k">class</span> <span class="nc">DiagGGNOptimizer</span><span class="p">(</span><span class="n">torch</span><span class="p">.</span><span class="n">optim</span><span class="p">.</span><span class="n">Optimizer</span><span class="p">):</span>
     <span class="k">def</span> <span class="nf">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">parameters</span><span class="p">,</span> <span class="n">step_size</span><span class="p">,</span> <span class="n">damping</span><span class="p">):</span>
-        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">__init__</span><span class="p">(</span>
+        <span class="nb">super</span><span class="p">().</span><span class="n">__init__</span><span class="p">(</span>
             <span class="n">parameters</span><span class="p">,</span> 
             <span class="nb">dict</span><span class="p">(</span><span class="n">step_size</span><span class="o">=</span><span class="n">step_size</span><span class="p">,</span> <span class="n">damping</span><span class="o">=</span><span class="n">damping</span><span class="p">)</span>
         <span class="p">)</span>
 
     <span class="k">def</span> <span class="nf">step</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="k">for</span> <span class="n">group</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">param_groups</span><span class="p">:</span>
+        <span class="k">for</span> <span class="n">group</span> <span class="ow">in</span> <span class="bp">self</span><span class="p">.</span><span class="n">param_groups</span><span class="p">:</span>
             <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">group</span><span class="p">[</span><span class="s">"params"</span><span class="p">]:</span>
-                <span class="n">step_direction</span> <span class="o">=</span> <span class="n">p</span><span class="o">.</span><span class="n">grad</span> <span class="o">/</span> <span class="p">(</span><span class="n">p</span><span class="o">.</span><span class="n">diag_ggn_mc</span> <span class="o">+</span> <span class="n">group</span><span class="p">[</span><span class="s">"damping"</span><span class="p">])</span>
-                <span class="n">p</span><span class="o">.</span><span class="n">data</span><span class="o">.</span><span class="n">add_</span><span class="p">(</span><span class="o">-</span><span class="n">group</span><span class="p">[</span><span class="s">"step_size"</span><span class="p">],</span> <span class="n">step_direction</span><span class="p">)</span>
+                <span class="n">step_direction</span> <span class="o">=</span> <span class="n">p</span><span class="p">.</span><span class="n">grad</span> <span class="o">/</span> <span class="p">(</span><span class="n">p</span><span class="p">.</span><span class="n">diag_ggn_mc</span> <span class="o">+</span> <span class="n">group</span><span class="p">[</span><span class="s">"damping"</span><span class="p">])</span>
+                <span class="n">p</span><span class="p">.</span><span class="n">data</span><span class="p">.</span><span class="n">add_</span><span class="p">(</span><span class="o">-</span><span class="n">group</span><span class="p">[</span><span class="s">"step_size"</span><span class="p">],</span> <span class="n">step_direction</span><span class="p">)</span>
         <span class="k">return</span> <span class="n">loss</span>
 </code></pre></div></div>
 
 <h3 id="step-3-put-on-your-backpack">Step 3: Put on your BackPACK</h3>
 
 <p>The last thing to do before running the optimizer is (i) tell BackPACK about the model and loss function used and (ii) create the optimizer.</p>
 
 <div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="n">extend</span><span class="p">(</span><span class="n">model</span><span class="p">)</span>
 <span class="n">extend</span><span class="p">(</span><span class="n">loss_function</span><span class="p">)</span>
 
 <span class="n">optimizer</span> <span class="o">=</span> <span class="n">DiagGGNOptimizer</span><span class="p">(</span>
-    <span class="n">model</span><span class="o">.</span><span class="n">parameters</span><span class="p">(),</span> 
+    <span class="n">model</span><span class="p">.</span><span class="n">parameters</span><span class="p">(),</span> 
     <span class="n">step_size</span><span class="o">=</span><span class="n">STEP_SIZE</span><span class="p">,</span> 
     <span class="n">damping</span><span class="o">=</span><span class="n">DAMPING</span>
 <span class="p">)</span>
 </code></pre></div></div>
 
 <p>We are now ready to run!</p>
 
 <h3 id="the-main-loop">The main loop</h3>
 
 <p>Traditional optimization loop: load each minibatch, 
 compute the minibatch loss, but now call BackPACK before doing the backward pass.
-The <code class="highlighter-rouge">diag_ggn_mc</code> fields of the parameters will get filled and the optimizer will run.</p>
+The <code class="language-plaintext highlighter-rouge">diag_ggn_mc</code> fields of the parameters will get filled and the optimizer will run.</p>
 
 <div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="k">for</span> <span class="n">batch_idx</span><span class="p">,</span> <span class="p">(</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">)</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">mnist_loader</span><span class="p">):</span>
     <span class="n">output</span> <span class="o">=</span> <span class="n">model</span><span class="p">(</span><span class="n">x</span><span class="p">)</span>
 
     <span class="n">accuracy</span> <span class="o">=</span> <span class="n">get_accuracy</span><span class="p">(</span><span class="n">output</span><span class="p">,</span> <span class="n">y</span><span class="p">)</span>
 
     <span class="k">with</span> <span class="n">backpack</span><span class="p">(</span><span class="n">DiagGGNMC</span><span class="p">()):</span>
         <span class="n">loss</span> <span class="o">=</span> <span class="n">loss_function</span><span class="p">(</span><span class="n">output</span><span class="p">,</span> <span class="n">y</span><span class="p">)</span>
-        <span class="n">loss</span><span class="o">.</span><span class="n">backward</span><span class="p">()</span>
-        <span class="n">optimizer</span><span class="o">.</span><span class="n">step</span><span class="p">()</span>
+        <span class="n">loss</span><span class="p">.</span><span class="n">backward</span><span class="p">()</span>
+        <span class="n">optimizer</span><span class="p">.</span><span class="n">step</span><span class="p">()</span>
 
     <span class="k">print</span><span class="p">(</span>
-        <span class="s">"Iteration </span><span class="si">%3</span><span class="s">.d/</span><span class="si">%</span><span class="s">d   "</span> <span class="o">%</span> <span class="p">(</span><span class="n">batch_idx</span><span class="p">,</span> <span class="n">MAX_ITER</span><span class="p">)</span> <span class="o">+</span>
-        <span class="s">"Minibatch Loss </span><span class="si">%.3</span><span class="s">f  "</span> <span class="o">%</span> <span class="p">(</span><span class="n">loss</span><span class="p">)</span> <span class="o">+</span>
-        <span class="s">"Accuracy </span><span class="si">%.0</span><span class="s">f"</span> <span class="o">%</span> <span class="p">(</span><span class="n">accuracy</span> <span class="o">*</span> <span class="mi">100</span><span class="p">)</span> <span class="o">+</span> <span class="s">"</span><span class="si">%</span><span class="s">"</span>
+        <span class="s">"Iteration %3.d/%d   "</span> <span class="o">%</span> <span class="p">(</span><span class="n">batch_idx</span><span class="p">,</span> <span class="n">MAX_ITER</span><span class="p">)</span> <span class="o">+</span>
+        <span class="s">"Minibatch Loss %.3f  "</span> <span class="o">%</span> <span class="p">(</span><span class="n">loss</span><span class="p">)</span> <span class="o">+</span>
+        <span class="s">"Accuracy %.0f"</span> <span class="o">%</span> <span class="p">(</span><span class="n">accuracy</span> <span class="o">*</span> <span class="mi">100</span><span class="p">)</span> <span class="o">+</span> <span class="s">"%"</span>
     <span class="p">)</span>
 
     <span class="k">if</span> <span class="n">batch_idx</span> <span class="o">&gt;=</span> <span class="n">MAX_ITER</span><span class="p">:</span>
         <span class="k">break</span>
 </code></pre></div></div>
 
 <p>If everything went fine, the output should look like</p>
 
-<div class="highlighter-rouge"><div class="highlight"><pre class="highlight"><code>Iteration   0/100   Minibatch Loss 2.307   Accuracy 12%
+<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>Iteration   0/100   Minibatch Loss 2.307   Accuracy 12%
 Iteration   1/100   Minibatch Loss 2.318   Accuracy 8%
 Iteration   2/100   Minibatch Loss 2.329   Accuracy 8%
 Iteration   3/100   Minibatch Loss 2.281   Accuracy 19%
 Iteration   4/100   Minibatch Loss 2.265   Accuracy 19%
 ...
 Iteration  96/100   Minibatch Loss 0.319   Accuracy 86%
 Iteration  97/100   Minibatch Loss 0.435   Accuracy 89%
```

### Comparing `backpack-for-pytorch-1.5.2/docs/index.html` & `backpack-for-pytorch-1.6.0/docs/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -97,18 +97,18 @@
 <div class="language-python highlighter-rouge">
     <div class="highlight">
         <pre class="highlight"><code><span class="s">"""
 Compute the gradient with Pytorch
 
 """</span>
 <span class="kn">from</span> <span class="nn">torch.nn</span> <span class="kn">import</span> <span class="n">CrossEntropyLoss</span><span class="p">,</span> <span class="n">Linear</span>
-<span class="kn">from</span> <span class="nn">utils</span> <span class="kn">import</span> <span class="n">load_mnist_data</span>
+<span class="kn">from</span> <span class="nn">backpack.utils.examples</span> <span class="kn">import</span> <span class="n">load_one_batch_mnist</span>
 
 
-<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_mnist_data</span><span class="p">()</span>
+<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_one_batch_mnist</span><span class="p">(flat=True)</span>
 <span class="n">model</span> <span class="o">=</span> <span class="n">Linear</span><span class="p">(</span><span class="mi">784</span><span class="p">,</span> <span class="mi">10</span><span class="p">)</span>
 <span class="n">lossfunc</span> <span class="o">=</span> <span class="n">CrossEntropyLoss</span><span class="p">()</span>
 <span class="n">loss</span> <span class="o">=</span> <span class="n">lossfunc</span><span class="p">(</span><span class="n">model</span><span class="p">(</span><span class="n">X</span><span class="p">),</span> <span class="n">y</span><span class="p">)</span>
 
 
 <span class="n">loss</span><span class="o">.</span><span class="n">backward</span><span class="p">()</span>
 
@@ -123,18 +123,19 @@
 <!--- VARIANCE CODE --->
 <div id="varianceCode" style="display:none;">
 <div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="s">"""
 Compute the gradient with Pytorch
 and the variance with BackPACK
 """</span>
 <span class="kn">from</span> <span class="nn">torch.nn</span> <span class="kn">import</span> <span class="n">CrossEntropyLoss</span><span class="p">,</span> <span class="n">Linear</span>
-<span class="kn">from</span> <span class="nn">utils</span> <span class="kn">import</span> <span class="n">load_mnist_data</span>
-<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span><span class="p">,</span> <span class="n">Variance</span></span>
+<span class="kn">from</span> <span class="nn">backpack.utils.examples</span> <span class="kn">import</span> <span class="n">load_one_batch_mnist</span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span></span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack.extensions</span> <span class="kn">import</span> <span class="n">Variance</span></span>
 
-<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_mnist_data</span><span class="p">()</span>
+<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_one_batch_mnist</span><span class="p">(flat=True)</span>
 <span class="n">model</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">Linear</span><span class="p">(</span><span class="mi">784</span><span class="p">,</span> <span class="mi">10</span><span class="p">))</span>
 <span class="n">lossfunc</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">CrossEntropyLoss</span><span class="p">())</span>
 <span class="n">loss</span> <span class="o">=</span> <span class="n">lossfunc</span><span class="p">(</span><span class="n">model</span><span class="p">(</span><span class="n">X</span><span class="p">),</span> <span class="n">y</span><span class="p">)</span>
 
 <span style="color: blue;"><span class="k">with</span> <span class="n">backpack</span><span class="p">(</span><span class="n">Variance</span><span class="p">()):</span></span>
     <span class="n">loss</span><span class="o">.</span><span class="n">backward</span><span class="p">()</span>
 
@@ -146,18 +147,19 @@
 <!--- SECOND MOMENT CODE --->
 <div id="secondMomentCode" style="display:none;">
 <div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="s">"""
 Compute the gradient with Pytorch
 and the second moment with BackPACK
 """</span>
 <span class="kn">from</span> <span class="nn">torch.nn</span> <span class="kn">import</span> <span class="n">CrossEntropyLoss</span><span class="p">,</span> <span class="n">Linear</span>
-<span class="kn">from</span> <span class="nn">utils</span> <span class="kn">import</span> <span class="n">load_mnist_data</span>
-<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span><span class="p">,</span> <span class="n">SumGradSquared</span></span>
+<span class="kn">from</span> <span class="nn">backpack.utils.examples</span> <span class="kn">import</span> <span class="n">load_one_batch_mnist</span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span></span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack.extensions</span> <span class="kn">import</span> <span class="n">SumGradSquared</span></span>
 
-<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_mnist_data</span><span class="p">()</span>
+<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_one_batch_mnist</span><span class="p">(flat=True)</span>
 <span class="n">model</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">Linear</span><span class="p">(</span><span class="mi">784</span><span class="p">,</span> <span class="mi">10</span><span class="p">))</span>
 <span class="n">lossfunc</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">CrossEntropyLoss</span><span class="p">())</span>
 <span class="n">loss</span> <span class="o">=</span> <span class="n">lossfunc</span><span class="p">(</span><span class="n">model</span><span class="p">(</span><span class="n">X</span><span class="p">),</span> <span class="n">y</span><span class="p">)</span>
 
 <span style="color: blue;"><span class="k">with</span> <span class="n">backpack</span><span class="p">(</span><span class="n">SumGradSquared</span><span class="p">()):</span></span>
     <span class="n">loss</span><span class="o">.</span><span class="n">backward</span><span class="p">()</span>
 
@@ -169,18 +171,19 @@
 <!--- DIAGGGN CODE --->
 <div id="diagGGNCode" style="display:none;">
 <div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="s">"""
 Compute the gradient with Pytorch
 and the diagonal of the Gauss-Newton with BackPACK
 """</span>
 <span class="kn">from</span> <span class="nn">torch.nn</span> <span class="kn">import</span> <span class="n">CrossEntropyLoss</span><span class="p">,</span> <span class="n">Linear</span>
-<span class="kn">from</span> <span class="nn">utils</span> <span class="kn">import</span> <span class="n">load_mnist_data</span>
-<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span><span class="p">,</span> <span class="n">DiagGGNExact</span></span>
+<span class="kn">from</span> <span class="nn">backpack.utils.examples</span> <span class="kn">import</span> <span class="n">load_one_batch_mnist</span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span></span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack.extensions</span> <span class="kn">import</span> <span class="n">DiagGGNExact</span></span>
 
-<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_mnist_data</span><span class="p">()</span>
+<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_one_batch_mnist</span><span class="p">(flat=True)</span>
 <span class="n">model</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">Linear</span><span class="p">(</span><span class="mi">784</span><span class="p">,</span> <span class="mi">10</span><span class="p">))</span>
 <span class="n">lossfunc</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">CrossEntropyLoss</span><span class="p">())</span>
 <span class="n">loss</span> <span class="o">=</span> <span class="n">lossfunc</span><span class="p">(</span><span class="n">model</span><span class="p">(</span><span class="n">X</span><span class="p">),</span> <span class="n">y</span><span class="p">)</span>
 
 <span style="color: blue;"><span class="k">with</span> <span class="n">backpack</span><span class="p">(</span><span class="n">DiagGGNExact</span><span class="p">()):</span></span>
     <span class="n">loss</span><span class="o">.</span><span class="n">backward</span><span class="p">()</span>
 
@@ -192,18 +195,19 @@
 <!--- KFAC CODE --->
 <div id="KFACCode" style="display:none;">
 <div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="s">"""
 Compute the gradient with Pytorch
 and KFAC with BackPACK
 """</span>
 <span class="kn">from</span> <span class="nn">torch.nn</span> <span class="kn">import</span> <span class="n">CrossEntropyLoss</span><span class="p">,</span> <span class="n">Linear</span>
-<span class="kn">from</span> <span class="nn">utils</span> <span class="kn">import</span> <span class="n">load_mnist_data</span>
-<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span><span class="p">,</span> <span class="n">KFAC</span></span>
+<span class="kn">from</span> <span class="nn">backpack.utils.examples</span> <span class="kn">import</span> <span class="n">load_one_batch_mnist</span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span></span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack.extensions</span> <span class="kn">import</span> <span class="n">KFAC</span></span>
 
-<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_mnist_data</span><span class="p">()</span>
+<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_one_batch_mnist</span><span class="p">(flat=True)</span>
 <span class="n">model</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">Linear</span><span class="p">(</span><span class="mi">784</span><span class="p">,</span> <span class="mi">10</span><span class="p">))</span>
 <span class="n">lossfunc</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">CrossEntropyLoss</span><span class="p">())</span>
 <span class="n">loss</span> <span class="o">=</span> <span class="n">lossfunc</span><span class="p">(</span><span class="n">model</span><span class="p">(</span><span class="n">X</span><span class="p">),</span> <span class="n">y</span><span class="p">)</span>
 
 <span style="color: blue;"><span class="k">with</span> <span class="n">backpack</span><span class="p">(</span><span class="n">KFAC</span><span class="p">()):</span></span>
     <span class="n">loss</span><span class="o">.</span><span class="n">backward</span><span class="p">()</span>
 
@@ -288,22 +292,22 @@
         }
     }
 </script>
 
 <hr />
 
 <p><strong>Install with</strong></p>
-<div class="highlighter-rouge"><div class="highlight"><pre class="highlight"><code>pip install backpack-for-pytorch 
+<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>pip install backpack-for-pytorch 
 </code></pre></div></div>
 
 <hr />
 
 <p>If you use BackPACK in your research, please cite <float style="float:right"><a href="/assets/dangel2020backpack.bib">download bibtex</a></float></p>
 
-<div class="highlighter-rouge"><div class="highlight"><pre class="highlight"><code>@inproceedings{dangel2020backpack,
+<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>@inproceedings{dangel2020backpack,
     title = {BackPACK: Packing more into Backprop},
     author = {Felix Dangel and Frederik Kunstner and Philipp Hennig},
     booktitle = {International Conference on Learning Representations},
     year = {2020},
     url = {https://openreview.net/forum?id=BJlrF24twB}
 }
 </code></pre></div></div>
```

#### html2text {}

```diff
@@ -16,18 +16,18 @@
     * the Gauss-Newton Diagonal
     * the Gauss-Newton KFAC
 """
 Compute the gradient with Pytorch
 
 """
 from torch.nn import CrossEntropyLoss, Linear
-from utils import load_mnist_data
+from backpack.utils.examples import load_one_batch_mnist
 
 
-X, y = load_mnist_data()
+X, y = load_one_batch_mnist(flat=True)
 model = Linear(784, 10)
 lossfunc = CrossEntropyLoss()
 loss = lossfunc(model(X), y)
 
 
 loss.backward()
 
@@ -35,18 +35,19 @@
     print(param.grad)
 
 """
 Compute the gradient with Pytorch
 and the variance with BackPACK
 """
 from torch.nn import CrossEntropyLoss, Linear
-from utils import load_mnist_data
-from backpack import extend, backpack, Variance
+from backpack.utils.examples import load_one_batch_mnist
+from backpack import extend, backpack
+from backpack.extensions import Variance
 
-X, y = load_mnist_data()
+X, y = load_one_batch_mnist(flat=True)
 model = extend(Linear(784, 10))
 lossfunc = extend(CrossEntropyLoss())
 loss = lossfunc(model(X), y)
 
 with backpack(Variance()):
     loss.backward()
 
@@ -54,18 +55,19 @@
     print(param.grad)
     print(param.variance)
 """
 Compute the gradient with Pytorch
 and the second moment with BackPACK
 """
 from torch.nn import CrossEntropyLoss, Linear
-from utils import load_mnist_data
-from backpack import extend, backpack, SumGradSquared
+from backpack.utils.examples import load_one_batch_mnist
+from backpack import extend, backpack
+from backpack.extensions import SumGradSquared
 
-X, y = load_mnist_data()
+X, y = load_one_batch_mnist(flat=True)
 model = extend(Linear(784, 10))
 lossfunc = extend(CrossEntropyLoss())
 loss = lossfunc(model(X), y)
 
 with backpack(SumGradSquared()):
     loss.backward()
 
@@ -73,18 +75,19 @@
     print(param.grad)
     print(param.sum_grad_squared)
 """
 Compute the gradient with Pytorch
 and the diagonal of the Gauss-Newton with BackPACK
 """
 from torch.nn import CrossEntropyLoss, Linear
-from utils import load_mnist_data
-from backpack import extend, backpack, DiagGGNExact
+from backpack.utils.examples import load_one_batch_mnist
+from backpack import extend, backpack
+from backpack.extensions import DiagGGNExact
 
-X, y = load_mnist_data()
+X, y = load_one_batch_mnist(flat=True)
 model = extend(Linear(784, 10))
 lossfunc = extend(CrossEntropyLoss())
 loss = lossfunc(model(X), y)
 
 with backpack(DiagGGNExact()):
     loss.backward()
 
@@ -92,18 +95,19 @@
     print(param.grad)
     print(param.diag_ggn_exact)
 """
 Compute the gradient with Pytorch
 and KFAC with BackPACK
 """
 from torch.nn import CrossEntropyLoss, Linear
-from utils import load_mnist_data
-from backpack import extend, backpack, KFAC
+from backpack.utils.examples import load_one_batch_mnist
+from backpack import extend, backpack
+from backpack.extensions import KFAC
 
-X, y = load_mnist_data()
+X, y = load_one_batch_mnist(flat=True)
 model = extend(Linear(784, 10))
 lossfunc = extend(CrossEntropyLoss())
 loss = lossfunc(model(X), y)
 
 with backpack(KFAC()):
     loss.backward()
```

### Comparing `backpack-for-pytorch-1.5.2/docs/jekyll-theme-minimal.gemspec` & `backpack-for-pytorch-1.6.0/docs/jekyll-theme-minimal.gemspec`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/script/release` & `backpack-for-pytorch-1.6.0/docs/script/release`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs/script/validate-html` & `backpack-for-pytorch-1.6.0/docs/script/validate-html`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/examples/basic_usage/example_all_in_one.py` & `backpack-for-pytorch-1.6.0/docs_src/examples/basic_usage/example_all_in_one.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/examples/cheatsheet.pdf` & `backpack-for-pytorch-1.6.0/docs_src/examples/cheatsheet.pdf`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_cg_newton.py` & `backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_cg_newton.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_custom_module.py` & `backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_custom_module.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_diag_ggn_optimizer.py` & `backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_diag_ggn_optimizer.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_differential_privacy.py` & `backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_differential_privacy.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_extension_hook.py` & `backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_extension_hook.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_gradient_of_variance.py` & `backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_gradient_of_variance.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_resnet_all_in_one.py` & `backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_resnet_all_in_one.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_rnn.py` & `backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_rnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,20 @@
 #    RNNs are still an experimental feature. Always double-check your
 #    results, as done in this example! Open an issue if you encounter a bug to help
 #    us improve the support.
 #
 #    Not all extensions support RNNs (yet). Please create a feature request in the
 #    repository if the extension you need is not supported.
 
+from pkg_resources import packaging
+
 # %%
 # Let's get the imports out of the way.
 from torch import (
+    _C,
     allclose,
     cat,
     device,
     int32,
     linspace,
     manual_seed,
     nn,
@@ -37,19 +40,28 @@
 )
 
 from backpack import backpack, extend
 from backpack.custom_module.graph_utils import BackpackTracer
 from backpack.custom_module.permute import Permute
 from backpack.custom_module.reduce_tuple import ReduceTuple
 from backpack.extensions import BatchGrad, DiagGGNExact
+from backpack.utils import TORCH_VERSION
 from backpack.utils.examples import autograd_diag_ggn_exact
 
 manual_seed(0)
 DEVICE = device("cpu")  # Verification via autograd only works on CPU
 
+# %%
+#
+# .. note::
+#    Due to `#99413 <https://github.com/pytorch/pytorch/issues/99413>`_, we have to disable
+#    MKLDNN for PyTorch 2.0.1 to get the double-backward through LSTMs working.
+if TORCH_VERSION == packaging.version.parse("2.0.1"):
+    _C._set_mkldnn_enabled(False)
+
 
 # %%
 # For this demo, we will use the Tolstoi Char RNN from
 # `DeepOBS <https://github.com/fsschneider/DeepOBS>`_.
 # This network is trained on Leo Tolstoi's War and Peace
 # and learns to predict the next character.
 class TolstoiCharRNN(nn.Module):
```

### Comparing `backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_save_memory_convolutions.py` & `backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_save_memory_convolutions.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,14 @@
 
     Args:
         device (torch.device): Device that the computation should be performed on.
     """
     print(f"Device: {device}")
 
     for save_memory in True, False:
-
         with weight_jac_t_save_memory(save_memory=save_memory):
 
             def work():
                 return compute_individual_gradients(device)
 
             interval = 1e-3
             peakmem = max(memory_usage(work, interval=interval))
@@ -164,15 +163,14 @@
 
     Args:
         device (torch.device): Device that the computation should be performed on.
     """
     print(f"Device: {device}")
 
     for save_memory in True, False:
-
         with weight_jac_t_save_memory(save_memory=save_memory):
             start = time.time()
 
             compute_individual_gradients(device)
 
             if str(device) == "cuda":
                 torch.cuda.synchronize()
```

### Comparing `backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_subsampling.py` & `backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_subsampling.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/examples/use_cases/example_trace_estimation.py` & `backpack-for-pytorch-1.6.0/docs_src/examples/use_cases/example_trace_estimation.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/rtd/Makefile` & `backpack-for-pytorch-1.6.0/docs_src/rtd/Makefile`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/rtd/assets/backpack_logo_torch.png` & `backpack-for-pytorch-1.6.0/docs_src/rtd/assets/backpack_logo_torch.png`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/rtd/assets/backpack_logo_torch.svg` & `backpack-for-pytorch-1.6.0/docs_src/rtd/assets/backpack_logo_torch.svg`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/rtd/conf.py` & `backpack-for-pytorch-1.6.0/docs_src/rtd/conf.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/rtd/extensions.rst` & `backpack-for-pytorch-1.6.0/docs_src/rtd/extensions.rst`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/rtd/good-to-know.rst` & `backpack-for-pytorch-1.6.0/docs_src/rtd/good-to-know.rst`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/rtd/index.rst` & `backpack-for-pytorch-1.6.0/docs_src/rtd/index.rst`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/rtd/main-api.rst` & `backpack-for-pytorch-1.6.0/docs_src/rtd/main-api.rst`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/rtd/make.bat` & `backpack-for-pytorch-1.6.0/docs_src/rtd/make.bat`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/rtd/supported-layers.rst` & `backpack-for-pytorch-1.6.0/docs_src/rtd/supported-layers.rst`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/rtd/torch.inventory` & `backpack-for-pytorch-1.6.0/docs_src/rtd/torch.inventory`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/_includes/code-samples.html` & `backpack-for-pytorch-1.6.0/docs_src/splash/_includes/code-samples.html`

 * *Files 3% similar despite different names*

```diff
@@ -40,18 +40,18 @@
 <div class="language-python highlighter-rouge">
     <div class="highlight">
         <pre class="highlight"><code><span class="s">"""
 Compute the gradient with Pytorch
 
 """</span>
 <span class="kn">from</span> <span class="nn">torch.nn</span> <span class="kn">import</span> <span class="n">CrossEntropyLoss</span><span class="p">,</span> <span class="n">Linear</span>
-<span class="kn">from</span> <span class="nn">utils</span> <span class="kn">import</span> <span class="n">load_mnist_data</span>
+<span class="kn">from</span> <span class="nn">backpack.utils.examples</span> <span class="kn">import</span> <span class="n">load_one_batch_mnist</span>
 
 
-<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_mnist_data</span><span class="p">()</span>
+<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_one_batch_mnist</span><span class="p">(flat=True)</span>
 <span class="n">model</span> <span class="o">=</span> <span class="n">Linear</span><span class="p">(</span><span class="mi">784</span><span class="p">,</span> <span class="mi">10</span><span class="p">)</span>
 <span class="n">lossfunc</span> <span class="o">=</span> <span class="n">CrossEntropyLoss</span><span class="p">()</span>
 <span class="n">loss</span> <span class="o">=</span> <span class="n">lossfunc</span><span class="p">(</span><span class="n">model</span><span class="p">(</span><span class="n">X</span><span class="p">),</span> <span class="n">y</span><span class="p">)</span>
 
 
 <span class="n">loss</span><span class="o">.</span><span class="n">backward</span><span class="p">()</span>
 
@@ -66,23 +66,24 @@
 <!--- VARIANCE CODE --->
 <div id="varianceCode" style="display:none;">
 <div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="s">"""
 Compute the gradient with Pytorch
 and the variance with BackPACK
 """</span>
 <span class="kn">from</span> <span class="nn">torch.nn</span> <span class="kn">import</span> <span class="n">CrossEntropyLoss</span><span class="p">,</span> <span class="n">Linear</span>
-<span class="kn">from</span> <span class="nn">utils</span> <span class="kn">import</span> <span class="n">load_mnist_data</span>
-<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span><span class="p">,</span> <span class="n">Variance</span></span>
+<span class="kn">from</span> <span class="nn">backpack.utils.examples</span> <span class="kn">import</span> <span class="n">load_one_batch_mnist</span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span></span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack.extensions</span> <span class="kn">import</span> <span class="n">Variance</span></span>
 
-<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_mnist_data</span><span class="p">()</span>
+<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_one_batch_mnist</span><span class="p">(flat=True)</span>
 <span class="n">model</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">Linear</span><span class="p">(</span><span class="mi">784</span><span class="p">,</span> <span class="mi">10</span><span class="p">))</span>
 <span class="n">lossfunc</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">CrossEntropyLoss</span><span class="p">())</span>
 <span class="n">loss</span> <span class="o">=</span> <span class="n">lossfunc</span><span class="p">(</span><span class="n">model</span><span class="p">(</span><span class="n">X</span><span class="p">),</span> <span class="n">y</span><span class="p">)</span>
 
-<span style="color: blue;"><span class="k">with</span> <span class="n">backpack</span><span class="p">(</span><span class="n">Variance</span><span class="p">()):</span></span>
+<span style="color: blue;"><span class="k">with</span> <span class="n">backpack</span><span class="p">(</span><span class="n">extensions.Variance</span><span class="p">()):</span></span>
     <span class="n">loss</span><span class="o">.</span><span class="n">backward</span><span class="p">()</span>
 
 <span class="k">for</span> <span class="n">param</span> <span class="ow">in</span> <span class="n">model</span><span class="o">.</span><span class="n">parameters</span><span class="p">():</span>
     <span class="k">print</span><span class="p">(</span><span class="n">param</span><span class="o">.</span><span class="n">grad</span><span class="p">)</span>
     <span style="color: blue;"><span class="k">print</span><span class="p">(</span><span class="n">param</span><span class="o">.</span><span class="n">variance</span><span class="p">)</span></span>
 </code></pre></div></div></div>
 
@@ -90,18 +91,19 @@
 <!--- SECOND MOMENT CODE --->
 <div id="secondMomentCode" style="display:none;">
 <div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="s">"""
 Compute the gradient with Pytorch
 and the second moment with BackPACK
 """</span>
 <span class="kn">from</span> <span class="nn">torch.nn</span> <span class="kn">import</span> <span class="n">CrossEntropyLoss</span><span class="p">,</span> <span class="n">Linear</span>
-<span class="kn">from</span> <span class="nn">utils</span> <span class="kn">import</span> <span class="n">load_mnist_data</span>
-<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span><span class="p">,</span> <span class="n">SumGradSquared</span></span>
+<span class="kn">from</span> <span class="nn">backpack.utils.examples</span> <span class="kn">import</span> <span class="n">load_one_batch_mnist</span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span></span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack.extensions</span> <span class="kn">import</span> <span class="n">SumGradSquared</span></span>
 
-<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_mnist_data</span><span class="p">()</span>
+<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_one_batch_mnist</span><span class="p">(flat=True)</span>
 <span class="n">model</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">Linear</span><span class="p">(</span><span class="mi">784</span><span class="p">,</span> <span class="mi">10</span><span class="p">))</span>
 <span class="n">lossfunc</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">CrossEntropyLoss</span><span class="p">())</span>
 <span class="n">loss</span> <span class="o">=</span> <span class="n">lossfunc</span><span class="p">(</span><span class="n">model</span><span class="p">(</span><span class="n">X</span><span class="p">),</span> <span class="n">y</span><span class="p">)</span>
 
 <span style="color: blue;"><span class="k">with</span> <span class="n">backpack</span><span class="p">(</span><span class="n">SumGradSquared</span><span class="p">()):</span></span>
     <span class="n">loss</span><span class="o">.</span><span class="n">backward</span><span class="p">()</span>
 
@@ -113,70 +115,72 @@
 <!--- DIAGGGN CODE --->
 <div id="diagGGNCode" style="display:none;">
 <div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="s">"""
 Compute the gradient with Pytorch
 and the diagonal of the Gauss-Newton with BackPACK
 """</span>
 <span class="kn">from</span> <span class="nn">torch.nn</span> <span class="kn">import</span> <span class="n">CrossEntropyLoss</span><span class="p">,</span> <span class="n">Linear</span>
-<span class="kn">from</span> <span class="nn">utils</span> <span class="kn">import</span> <span class="n">load_mnist_data</span>
-<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span><span class="p">,</span> <span class="n">DiagGGNExact</span></span>
+<span class="kn">from</span> <span class="nn">backpack.utils.examples</span> <span class="kn">import</span> <span class="n">load_one_batch_mnist</span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span></span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack.extensions</span> <span class="kn">import</span> <span class="n">DiagGGNExact</span></span>
 
-<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_mnist_data</span><span class="p">()</span>
+<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_one_batch_mnist</span><span class="p">(flat=True)</span>
 <span class="n">model</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">Linear</span><span class="p">(</span><span class="mi">784</span><span class="p">,</span> <span class="mi">10</span><span class="p">))</span>
 <span class="n">lossfunc</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">CrossEntropyLoss</span><span class="p">())</span>
 <span class="n">loss</span> <span class="o">=</span> <span class="n">lossfunc</span><span class="p">(</span><span class="n">model</span><span class="p">(</span><span class="n">X</span><span class="p">),</span> <span class="n">y</span><span class="p">)</span>
 
-<span style="color: blue;"><span class="k">with</span> <span class="n">backpack</span><span class="p">(</span><span class="n">DiagGGNExact</span><span class="p">()):</span></span>
+<span style="color: blue;"><span class="k">with</span> <span class="n">backpack</span><span class="p">(</span><span class="n">extensions.DiagGGNExact</span><span class="p">()):</span></span>
     <span class="n">loss</span><span class="o">.</span><span class="n">backward</span><span class="p">()</span>
 
 <span class="k">for</span> <span class="n">param</span> <span class="ow">in</span> <span class="n">model</span><span class="o">.</span><span class="n">parameters</span><span class="p">():</span>
     <span class="k">print</span><span class="p">(</span><span class="n">param</span><span class="o">.</span><span class="n">grad</span><span class="p">)</span>
     <span style="color: blue;"><span class="k">print</span><span class="p">(</span><span class="n">param</span><span class="o">.</span><span class="n">diag_ggn_exact</span><span class="p">)</span></span>
 </code></pre></div></div></div>
 
 <!--- KFAC CODE --->
 <div id="KFACCode" style="display:none;">
 <div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="s">"""
 Compute the gradient with Pytorch
 and KFAC with BackPACK
 """</span>
 <span class="kn">from</span> <span class="nn">torch.nn</span> <span class="kn">import</span> <span class="n">CrossEntropyLoss</span><span class="p">,</span> <span class="n">Linear</span>
-<span class="kn">from</span> <span class="nn">utils</span> <span class="kn">import</span> <span class="n">load_mnist_data</span>
-<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span><span class="p">,</span> <span class="n">KFAC</span></span>
+<span class="kn">from</span> <span class="nn">backpack.utils.examples</span> <span class="kn">import</span> <span class="n">load_one_batch_mnist</span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack</span> <span class="kn">import</span> <span class="n">extend</span><span class="p">,</span> <span class="n">backpack</span></span>
+<span style="color: blue;"><span class="kn">from</span> <span class="nn">backpack.extensions</span> <span class="kn">import</span> <span class="n">KFAC</span></span>
 
-<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_mnist_data</span><span class="p">()</span>
+<span class="n">X</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">load_one_batch_mnist</span><span class="p">(flat=True)</span>
 <span class="n">model</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">Linear</span><span class="p">(</span><span class="mi">784</span><span class="p">,</span> <span class="mi">10</span><span class="p">))</span>
 <span class="n">lossfunc</span> <span class="o">=</span> <span class="n"><span style="color: blue;">extend</span></span><span class="p">(</span><span class="n">CrossEntropyLoss</span><span class="p">())</span>
 <span class="n">loss</span> <span class="o">=</span> <span class="n">lossfunc</span><span class="p">(</span><span class="n">model</span><span class="p">(</span><span class="n">X</span><span class="p">),</span> <span class="n">y</span><span class="p">)</span>
 
-<span style="color: blue;"><span class="k">with</span> <span class="n">backpack</span><span class="p">(</span><span class="n">KFAC</span><span class="p">()):</span></span>
+<span style="color: blue;"><span class="k">with</span> <span class="n">backpack</span><span class="p">(</span><span class="n">extensions.KFAC</span><span class="p">()):</span></span>
     <span class="n">loss</span><span class="o">.</span><span class="n">backward</span><span class="p">()</span>
 
 <span class="k">for</span> <span class="n">param</span> <span class="ow">in</span> <span class="n">model</span><span class="o">.</span><span class="n">parameters</span><span class="p">():</span>
     <span class="k">print</span><span class="p">(</span><span class="n">param</span><span class="o">.</span><span class="n">grad</span><span class="p">)</span>
     <span style="color: blue;"><span class="k">print</span><span class="p">(</span><span class="n">param</span><span class="o">.</span><span class="n">kfac</span><span class="p">)</span></span>
 </code></pre></div></div>
 </div>
 
 <script>
     window.onload = function() {
-        var varianceButton = document.getElementById("varianceButton");  
-        var gradientButton = document.getElementById("gradientButton");  
-        var diagGGNButton = document.getElementById("diagGGNButton");  
+        var varianceButton = document.getElementById("varianceButton");
+        var gradientButton = document.getElementById("gradientButton");
+        var diagGGNButton = document.getElementById("diagGGNButton");
         var KFACButton = document.getElementById("KFACButton");
 
-        var varianceItem = document.getElementById("varianceItem");  
-        var gradientItem = document.getElementById("gradientItem");  
-        var diagGGNItem = document.getElementById("diagGGNItem");  
-        var KFACItem = document.getElementById("KFACItem");  
-
-        var gradientCode = document.getElementById("gradientCode");  
-        var varianceCode = document.getElementById("varianceCode");  
-        var diagGGNCode = document.getElementById("diagGGNCode");  
-        var KFACCode = document.getElementById("KFACCode");  
+        var varianceItem = document.getElementById("varianceItem");
+        var gradientItem = document.getElementById("gradientItem");
+        var diagGGNItem = document.getElementById("diagGGNItem");
+        var KFACItem = document.getElementById("KFACItem");
+
+        var gradientCode = document.getElementById("gradientCode");
+        var varianceCode = document.getElementById("varianceCode");
+        var diagGGNCode = document.getElementById("diagGGNCode");
+        var KFACCode = document.getElementById("KFACCode");
 
         var getCurrent = function() {
             if (varianceItem.className === "active") {
                 return "variance"
             } else if (gradientItem.className === "active") {
                 return "gradient"
             } else if (diagGGNItem.className === "active") {
```

#### html2text {}

```diff
@@ -3,18 +3,18 @@
     * the Gauss-Newton Diagonal
     * the Gauss-Newton KFAC
 """
 Compute the gradient with Pytorch
 
 """
 from torch.nn import CrossEntropyLoss, Linear
-from utils import load_mnist_data
+from backpack.utils.examples import load_one_batch_mnist
 
 
-X, y = load_mnist_data()
+X, y = load_one_batch_mnist(flat=True)
 model = Linear(784, 10)
 lossfunc = CrossEntropyLoss()
 loss = lossfunc(model(X), y)
 
 
 loss.backward()
 
@@ -22,37 +22,39 @@
     print(param.grad)
 
 """
 Compute the gradient with Pytorch
 and the variance with BackPACK
 """
 from torch.nn import CrossEntropyLoss, Linear
-from utils import load_mnist_data
-from backpack import extend, backpack, Variance
+from backpack.utils.examples import load_one_batch_mnist
+from backpack import extend, backpack
+from backpack.extensions import Variance
 
-X, y = load_mnist_data()
+X, y = load_one_batch_mnist(flat=True)
 model = extend(Linear(784, 10))
 lossfunc = extend(CrossEntropyLoss())
 loss = lossfunc(model(X), y)
 
-with backpack(Variance()):
+with backpack(extensions.Variance()):
     loss.backward()
 
 for param in model.parameters():
     print(param.grad)
     print(param.variance)
 """
 Compute the gradient with Pytorch
 and the second moment with BackPACK
 """
 from torch.nn import CrossEntropyLoss, Linear
-from utils import load_mnist_data
-from backpack import extend, backpack, SumGradSquared
+from backpack.utils.examples import load_one_batch_mnist
+from backpack import extend, backpack
+from backpack.extensions import SumGradSquared
 
-X, y = load_mnist_data()
+X, y = load_one_batch_mnist(flat=True)
 model = extend(Linear(784, 10))
 lossfunc = extend(CrossEntropyLoss())
 loss = lossfunc(model(X), y)
 
 with backpack(SumGradSquared()):
     loss.backward()
 
@@ -60,41 +62,43 @@
     print(param.grad)
     print(param.sum_grad_squared)
 """
 Compute the gradient with Pytorch
 and the diagonal of the Gauss-Newton with BackPACK
 """
 from torch.nn import CrossEntropyLoss, Linear
-from utils import load_mnist_data
-from backpack import extend, backpack, DiagGGNExact
+from backpack.utils.examples import load_one_batch_mnist
+from backpack import extend, backpack
+from backpack.extensions import DiagGGNExact
 
-X, y = load_mnist_data()
+X, y = load_one_batch_mnist(flat=True)
 model = extend(Linear(784, 10))
 lossfunc = extend(CrossEntropyLoss())
 loss = lossfunc(model(X), y)
 
-with backpack(DiagGGNExact()):
+with backpack(extensions.DiagGGNExact()):
     loss.backward()
 
 for param in model.parameters():
     print(param.grad)
     print(param.diag_ggn_exact)
 """
 Compute the gradient with Pytorch
 and KFAC with BackPACK
 """
 from torch.nn import CrossEntropyLoss, Linear
-from utils import load_mnist_data
-from backpack import extend, backpack, KFAC
+from backpack.utils.examples import load_one_batch_mnist
+from backpack import extend, backpack
+from backpack.extensions import KFAC
 
-X, y = load_mnist_data()
+X, y = load_one_batch_mnist(flat=True)
 model = extend(Linear(784, 10))
 lossfunc = extend(CrossEntropyLoss())
 loss = lossfunc(model(X), y)
 
-with backpack(KFAC()):
+with backpack(extensions.KFAC()):
     loss.backward()
 
 for param in model.parameters():
     print(param.grad)
     print(param.kfac)
```

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/_layouts/default.html` & `backpack-for-pytorch-1.6.0/docs_src/splash/_layouts/default.html`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/_sass/fonts.scss` & `backpack-for-pytorch-1.6.0/docs_src/splash/_sass/fonts.scss`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/_sass/jekyll-theme-minimal.scss` & `backpack-for-pytorch-1.6.0/docs_src/splash/_sass/jekyll-theme-minimal.scss`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/_sass/rouge-github.scss` & `backpack-for-pytorch-1.6.0/docs_src/splash/_sass/rouge-github.scss`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/css/style.css` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.eot` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.eot`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.svg` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.svg`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.ttf` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.ttf`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff2` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700/Noto-Sans-700.woff2`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.eot` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.eot`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.svg` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.svg`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.ttf` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.ttf`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff2` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-700italic/Noto-Sans-700italic.woff2`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.eot` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.eot`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.svg` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.svg`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.ttf` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.ttf`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff2` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-italic/Noto-Sans-italic.woff2`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.eot` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.eot`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.svg` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.svg`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.ttf` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.ttf`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff2` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/fonts/Noto-Sans-regular/Noto-Sans-regular.woff2`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/img/backpack_logo_torch.svg` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/img/backpack_logo_torch.svg`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/img/logo.png` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/img/updaterule.png` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/img/updaterule.png`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/assets/js/scale.fix.js` & `backpack-for-pytorch-1.6.0/docs_src/splash/assets/js/scale.fix.js`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/examples.md` & `backpack-for-pytorch-1.6.0/docs_src/splash/examples.md`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/index.md` & `backpack-for-pytorch-1.6.0/docs_src/splash/index.md`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/jekyll-theme-minimal.gemspec` & `backpack-for-pytorch-1.6.0/docs_src/splash/jekyll-theme-minimal.gemspec`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/script/release` & `backpack-for-pytorch-1.6.0/docs_src/splash/script/release`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/docs_src/splash/script/validate-html` & `backpack-for-pytorch-1.6.0/docs_src/splash/script/validate-html`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/fully_documented.txt` & `backpack-for-pytorch-1.6.0/fully_documented.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 setup.py
 
 backpack/__init__.py
 backpack/context.py
 backpack/custom_module/
 
 backpack/core/derivatives/basederivatives.py
+backpack/core/derivatives/nll_base.py
 backpack/core/derivatives/rnn.py
 backpack/core/derivatives/shape_check.py
 backpack/core/derivatives/__init__.py
 backpack/core/derivatives/permute.py
 backpack/core/derivatives/lstm.py
 backpack/core/derivatives/linear.py
 backpack/core/derivatives/adaptive_avg_pool_nd.py
 backpack/core/derivatives/batchnorm_nd.py
 backpack/core/derivatives/embedding.py
 backpack/core/derivatives/crossentropyloss.py
 backpack/core/derivatives/scale_module.py
 backpack/core/derivatives/sum_module.py
 backpack/core/derivatives/dropout.py
 backpack/core/derivatives/slicing.py
+backpack/core/derivatives/bcewithlogitsloss.py
 
 backpack/extensions/__init__.py
 backpack/extensions/backprop_extension.py
 backpack/extensions/module_extension.py
 backpack/extensions/saved_quantities.py
 backpack/extensions/mat_to_mat_jac_base.py
 backpack/extensions/firstorder/base.py
@@ -62,25 +64,35 @@
 backpack/extensions/secondorder/diag_hessian/conv1d.py
 backpack/extensions/secondorder/diag_hessian/conv2d.py
 backpack/extensions/secondorder/diag_hessian/conv3d.py
 backpack/extensions/secondorder/diag_hessian/pad.py
 backpack/extensions/secondorder/diag_hessian/slicing.py
 backpack/extensions/secondorder/sqrt_ggn/
 backpack/extensions/secondorder/hbp/custom_module.py
+backpack/extensions/secondorder/hbp/conv1d.py
+backpack/extensions/secondorder/hbp/conv2d.py
+backpack/extensions/secondorder/hbp/conv3d.py
+backpack/extensions/secondorder/hbp/convnd.py
+backpack/extensions/secondorder/hbp/conv_transpose1d.py
+backpack/extensions/secondorder/hbp/conv_transpose2d.py
+backpack/extensions/secondorder/hbp/conv_transpose3d.py
+backpack/extensions/secondorder/hbp/conv_transposend.py
 
 backpack/hessianfree/ggnvp.py
 
 backpack/utils/linear.py
 backpack/utils/subsampling.py
 backpack/utils/errors.py
 backpack/utils/__init__.py
 backpack/utils/module_classification.py
 backpack/utils/hooks.py
 backpack/utils/examples.py
 backpack/utils/convert_parameters.py
+backpack/utils/conv.py
+backpack/utils/conv_transpose.py
 
 test/extensions/automated_settings.py
 test/extensions/problem.py
 test/extensions/utils.py
 test/extensions/test_backprop_extension.py
 test/extensions/test_hooks.py
 test/extensions/graph_clear_test.py
@@ -108,13 +120,15 @@
 test/core/derivatives/pooling_adaptive_settings.py
 test/core/derivatives/batch_norm_settings.py
 test/core/derivatives/embedding_settings.py
 test/core/derivatives/scale_module_settings.py
 test/core/derivatives/slicing_settings.py
 test/utils/evaluation_mode.py
 test/utils/skip_test.py
+test/utils/skip_extension_test.py
 test/utils/__init__.py
 test/converter/
 test/utils/test_subsampling.py
+test/utils/conv_transpose.py
 test/custom_module/
 test/test_retain_graph.py
 test/test_batch_first.py
```

### Comparing `backpack-for-pytorch-1.5.2/logo/backpack_logo_no_torch.svg` & `backpack-for-pytorch-1.6.0/logo/backpack_logo_no_torch.svg`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/logo/backpack_logo_torch.svg` & `backpack-for-pytorch-1.6.0/logo/backpack_logo_torch.svg`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/makefile` & `backpack-for-pytorch-1.6.0/makefile`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/setup.cfg` & `backpack-for-pytorch-1.6.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 license = MIT
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [options]
 zip_safe = False
 packages = find:
 include_package_data = True
 setup_requires = 
 	setuptools_scm
 install_requires = 
-	torch >= 1.9.0, < 2.0.0
-	torchvision >= 0.7.0, < 1.0.0
+	torch >= 1.9.0
+	torchvision >= 0.7.0
 	einops >= 0.3.0, < 1.0.0
-python_requires = >=3.7
+	unfoldNd >= 0.2.0, < 1.0.0
+python_requires = >=3.8
 
 [options.packages.find]
 exclude = test*
 
 [options.extras_require]
 test = 
 	scipy
@@ -66,22 +67,23 @@
 use_parentheses = True
 
 [flake8]
 select = B,C,E,F,P,W,B9
 max-line-length = 88
 max-complexity = 10
 ignore = 
-	E501, # max-line-length
-	C408, # use {} instead of dict()
-	E203, # whitespace before :
-	E231, # missing whitespace after ','
-	W291, # trailing whitespace
-	W503, # line break before binary operator
-	W504, # line break after binary operator
-	B905, # 'zip()' without an explicit 'strict=' parameter
+	E501,
+	C408,
+	E203,
+	E231,
+	W291,
+	W503,
+	W504,
+	B905,
+	B028,
 exclude = docs, build, .git, docs_src/rtd, docs_src/rtd_output, .eggs
 
 [darglint]
 docstring_style = google
 strictness = full
 
 [pydocstyle]
```

### Comparing `backpack-for-pytorch-1.5.2/test/adaptive_avg_pool/problem.py` & `backpack-for-pytorch-1.6.0/test/adaptive_avg_pool/problem.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/adaptive_avg_pool/settings_adaptive_avg_pool_nd.py` & `backpack-for-pytorch-1.6.0/test/adaptive_avg_pool/settings_adaptive_avg_pool_nd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/adaptive_avg_pool/test_adaptive_avg_pool_nd.py` & `backpack-for-pytorch-1.6.0/test/adaptive_avg_pool/test_adaptive_avg_pool_nd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/automated_kfac_test.py` & `backpack-for-pytorch-1.6.0/test/automated_kfac_test.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/automated_test.py` & `backpack-for-pytorch-1.6.0/test/automated_test.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/benchmark/functionality.py` & `backpack-for-pytorch-1.6.0/test/benchmark/functionality.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/benchmark/jvp.py` & `backpack-for-pytorch-1.6.0/test/benchmark/jvp.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/benchmark/jvp_avgpool2d.py` & `backpack-for-pytorch-1.6.0/test/benchmark/jvp_avgpool2d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/benchmark/jvp_conv2d.py` & `backpack-for-pytorch-1.6.0/test/benchmark/jvp_conv2d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/benchmark/jvp_linear.py` & `backpack-for-pytorch-1.6.0/test/benchmark/jvp_linear.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/benchmark/jvp_maxpool2d.py` & `backpack-for-pytorch-1.6.0/test/benchmark/jvp_maxpool2d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/benchmark/jvp_zeropad2d.py` & `backpack-for-pytorch-1.6.0/test/benchmark/jvp_zeropad2d.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/bugfixes_test.py` & `backpack-for-pytorch-1.6.0/test/bugfixes_test.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/conv2d_test.py` & `backpack-for-pytorch-1.6.0/test/conv2d_test.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/converter/converter_cases.py` & `backpack-for-pytorch-1.6.0/test/converter/converter_cases.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/converter/resnet_cases.py` & `backpack-for-pytorch-1.6.0/test/converter/resnet_cases.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/converter/test_converter.py` & `backpack-for-pytorch-1.6.0/test/converter/test_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Tests converter.
 
 - whether converted network is equivalent to original network
 - whether DiagGGN runs without errors on new network
 """
 from test.converter.converter_cases import CONVERTER_MODULES, ConverterModule
 from test.core.derivatives.utils import classification_targets, regression_targets
+from test.utils.skip_test import skip_torch_2_0_1_lstm
 from typing import Tuple
 
 from pytest import fixture
 from torch import Tensor, allclose, cat, int32, linspace, manual_seed
 from torch.nn import CrossEntropyLoss, Module, MSELoss
 
 from backpack import backpack, extend
@@ -27,14 +28,15 @@
         request: pytest request
 
     Yields:
         model and input and loss function
     """
     manual_seed(0)
     model: ConverterModule = request.param()
+    skip_torch_2_0_1_lstm(model)
     inputs: Tensor = model.input_fn()
     loss_fn: Module = model.loss_fn()
     yield model, inputs, loss_fn
     del model, inputs, loss_fn
 
 
 def test_network_diag_ggn(model_and_input):
```

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/__init__.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     AdaptiveAvgPool3d,
     AvgPool1d,
     AvgPool2d,
     AvgPool3d,
     BatchNorm1d,
     BatchNorm2d,
     BatchNorm3d,
+    BCEWithLogitsLoss,
     Conv1d,
     Conv2d,
     Conv3d,
     ConvTranspose1d,
     ConvTranspose2d,
     ConvTranspose3d,
     CrossEntropyLoss,
@@ -41,14 +42,15 @@
     AdaptiveAvgPool2dDerivatives,
     AdaptiveAvgPool3dDerivatives,
 )
 from backpack.core.derivatives.avgpool1d import AvgPool1DDerivatives
 from backpack.core.derivatives.avgpool2d import AvgPool2DDerivatives
 from backpack.core.derivatives.avgpool3d import AvgPool3DDerivatives
 from backpack.core.derivatives.batchnorm_nd import BatchNormNdDerivatives
+from backpack.core.derivatives.bcewithlogitsloss import BCELossWithLogitsDerivatives
 from backpack.core.derivatives.conv1d import Conv1DDerivatives
 from backpack.core.derivatives.conv2d import Conv2DDerivatives
 from backpack.core.derivatives.conv3d import Conv3DDerivatives
 from backpack.core.derivatives.conv_transpose1d import ConvTranspose1DDerivatives
 from backpack.core.derivatives.conv_transpose2d import ConvTranspose2DDerivatives
 from backpack.core.derivatives.conv_transpose3d import ConvTranspose3DDerivatives
 from backpack.core.derivatives.crossentropyloss import CrossEntropyLossDerivatives
@@ -116,8 +118,9 @@
     BatchNorm3d: BatchNormNdDerivatives,
     Embedding: EmbeddingDerivatives,
     ScaleModule: ScaleModuleDerivatives,
     Identity: ScaleModuleDerivatives,
     SumModule: SumModuleDerivatives,
     Pad: PadDerivatives,
     Slicing: SlicingDerivatives,
+    BCEWithLogitsLoss: BCELossWithLogitsDerivatives,
 }
```

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/activation_settings.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/activation_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/batch_norm_settings.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/batch_norm_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/convolution_settings.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/convolution_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/derivatives_test.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/derivatives_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 - Jacobian-matrix products
 - Transposed Jacobian-matrix products
 
 - Jacobian-matrix products with respect to layer parameters
 - Transposed Jacobian-matrix products with respect to layer parameters
 """
+
 from contextlib import nullcontext
-from test.automated_test import check_sizes_and_values
+from test.automated_test import check_sizes, check_sizes_and_values
 from test.core.derivatives.batch_norm_settings import BATCH_NORM_SETTINGS
 from test.core.derivatives.embedding_settings import EMBEDDING_SETTINGS
 from test.core.derivatives.implementation.autograd import AutogradDerivatives
 from test.core.derivatives.implementation.backpack import BackpackDerivatives
 from test.core.derivatives.loss_settings import LOSS_FAIL_SETTINGS
 from test.core.derivatives.lstm_settings import LSTM_SETTINGS
 from test.core.derivatives.padding_settings import CUSTOM_PADDING_SETTINGS
@@ -20,23 +21,27 @@
 from test.core.derivatives.rnn_settings import RNN_SETTINGS as RNN_SETTINGS
 from test.core.derivatives.scale_module_settings import SCALE_MODULE_SETTINGS
 from test.core.derivatives.settings import SETTINGS
 from test.core.derivatives.slicing_settings import CUSTOM_SLICING_SETTINGS
 from test.utils.skip_test import (
     skip_adaptive_avg_pool3d_cuda,
     skip_batch_norm_train_mode_with_subsampling,
+    skip_BCEWithLogitsLoss,
+    skip_BCEWithLogitsLoss_non_binary_labels,
     skip_subsampling_conflict,
+    skip_torch_2_0_1_lstm,
 )
 from typing import List, Union
 from warnings import warn
 
 from pytest import fixture, mark, raises, skip
 from torch import Tensor, rand
 
 from backpack.core.derivatives.convnd import weight_jac_t_save_memory
+from backpack.utils.subsampling import subsample
 
 PROBLEMS = make_test_problems(SETTINGS)
 IDS = [problem.make_id() for problem in PROBLEMS]
 
 NO_LOSS_PROBLEMS = [problem for problem in PROBLEMS if not problem.is_loss()]
 NO_LOSS_IDS = [problem.make_id() for problem in NO_LOSS_PROBLEMS]
 
@@ -69,14 +74,17 @@
 ]
 
 CUSTOM_SLICING_MODULE_PROBLEMS = make_test_problems(CUSTOM_SLICING_SETTINGS)
 CUSTOM_SLICING_MODULE_IDS = [
     problem.make_id() for problem in CUSTOM_SLICING_MODULE_PROBLEMS
 ]
 
+NLL_PROBLEMS = [problem for problem in PROBLEMS if problem.is_nll()]
+NLL_IDS = [problem.make_id() for problem in NLL_PROBLEMS]
+
 SUBSAMPLINGS = [None, [0, 0], [2, 0]]
 SUBSAMPLING_IDS = [f"subsampling={s}".replace(" ", "") for s in SUBSAMPLINGS]
 
 
 @mark.parametrize("subsampling", SUBSAMPLINGS, ids=SUBSAMPLING_IDS)
 @mark.parametrize("sum_batch", [True, False], ids=["sum_batch=True", "sum_batch=False"])
 def test_param_mjp(
@@ -126,14 +134,15 @@
     """Test the Jacobian-matrix product.
 
     Args:
         problem: Test case.
         V: Number of vectorized Jacobian-vector products. Default: ``3``.
     """
     problem.set_up()
+    skip_torch_2_0_1_lstm(problem.module)
     mat = rand(V, *problem.input_shape).to(problem.device)
 
     backpack_res = BackpackDerivatives(problem).jac_mat_prod(mat)
     autograd_res = AutogradDerivatives(problem).jac_mat_prod(mat)
 
     check_sizes_and_values(autograd_res, backpack_res)
     problem.tear_down()
@@ -329,26 +338,113 @@
         problem: Test case.
         subsampling: Indices of active samples.
         mc_samples: number of samples. Defaults to 1000000.
         chunks: Number of passes the MC samples will be processed sequentially.
     """
     problem.set_up()
     skip_subsampling_conflict(problem, subsampling)
+    skip_BCEWithLogitsLoss_non_binary_labels(problem)
 
     backpack_res = BackpackDerivatives(problem).input_hessian_via_sqrt_hessian(
         mc_samples=mc_samples, chunks=chunks, subsampling=subsampling
     )
     autograd_res = AutogradDerivatives(problem).input_hessian(subsampling=subsampling)
 
     RTOL, ATOL = 1e-2, 7e-3
     check_sizes_and_values(autograd_res, backpack_res, rtol=RTOL, atol=ATOL)
     problem.tear_down()
 
 
 @mark.parametrize("subsampling", SUBSAMPLINGS, ids=SUBSAMPLING_IDS)
+@mark.parametrize("problem", NLL_PROBLEMS, ids=NLL_IDS)
+def test_sqrt_hessian_sampled_squared_approximates_hessian_nll(
+    problem: DerivativesTestProblem,
+    subsampling: Union[List[int], None],
+    mc_samples: int = 50000,
+    chunks: int = 10,
+    rerun_on_crash: bool = True,
+) -> None:
+    """Test the MC-sampled sqrt decomposition of the input Hessian for NLL loss base.
+
+    Compares the Hessian to reconstruction from individual Hessian MC-sampled
+    sqrt. This test runs specifically on the autograd version of
+    compute_sampled_grads, rather than manual versions which are used by default
+    and tested elsewhere.
+
+    Args:
+        problem: Test case.
+        subsampling: Indices of active samples.
+        mc_samples: number of samples. Defaults to 50000.
+        chunks: Number of passes the MC samples will be processed sequentially.
+        rerun_on_crash: Run the test again with more samples, then crash if it
+            still fails. Default: ``True``.
+
+    Raises:
+        AssertionError: If the MC-sampled Hessian square root does not square to the
+            exact Hessian.
+    """
+    problem.set_up()
+    skip_subsampling_conflict(problem, subsampling)
+    skip_BCEWithLogitsLoss_non_binary_labels(problem)
+    RTOL, ATOL = 1e-2, 8e-3
+
+    autograd_res = AutogradDerivatives(problem).input_hessian(subsampling=subsampling)
+
+    try:
+        backpack_res = BackpackDerivatives(problem).input_hessian_via_sqrt_hessian(
+            mc_samples=mc_samples,
+            chunks=chunks,
+            subsampling=subsampling,
+            use_autograd=True,
+        )
+        problem.tear_down()
+        check_sizes_and_values(autograd_res, backpack_res, rtol=RTOL, atol=ATOL)
+
+    except AssertionError as e:
+        if rerun_on_crash:
+            more = 10
+            test_sqrt_hessian_sampled_squared_approximates_hessian_nll(
+                problem,
+                subsampling,
+                mc_samples=mc_samples * more,
+                chunks=chunks * more,
+                rerun_on_crash=False,
+            )
+        else:
+            raise e
+
+
+@mark.parametrize("subsampling", SUBSAMPLINGS, ids=SUBSAMPLING_IDS)
+@mark.parametrize("problem", NLL_PROBLEMS, ids=NLL_IDS)
+def test_dist_sample_shape_nll(
+    problem: DerivativesTestProblem,
+    subsampling: Union[List[int], None],
+) -> None:
+    """Test distribution sample shape for NLL derivatives.
+
+    Compares the shape sampled from the distribution to the output to
+    verify the shapes match.
+
+    Args:
+        problem: Test case.
+        subsampling: Indices of active samples.
+    """
+    problem.set_up()
+    skip_subsampling_conflict(problem, subsampling)
+    BackpackDerivatives(problem).store_forward_io()
+
+    subsampled_input = subsample(problem.module.input0, subsampling=subsampling)
+    subsampled_target = subsample(problem.module.input1, subsampling=subsampling)
+    samples = problem.derivative._make_distribution(subsampled_input).sample()
+
+    check_sizes(samples, subsampled_target)
+    problem.tear_down()
+
+
+@mark.parametrize("subsampling", SUBSAMPLINGS, ids=SUBSAMPLING_IDS)
 @mark.parametrize("problem", LOSS_FAIL_PROBLEMS, ids=LOSS_FAIL_IDS)
 def test_sqrt_hessian_sampled_should_fail(
     problem: DerivativesTestProblem, subsampling: Union[List[int], None]
 ) -> None:
     """Test that sqrt_hessian_samples fails.
 
     Args:
@@ -363,14 +459,15 @@
 def test_sum_hessian(problem):
     """Test the summed Hessian.
 
     Args:
         problem (DerivativesProblem): Problem for derivative test.
     """
     problem.set_up()
+    skip_BCEWithLogitsLoss(problem)  # TODO Implement _sum_hessian for BCEWithLogitsLoss
 
     backpack_res = BackpackDerivatives(problem).sum_hessian()
     autograd_res = AutogradDerivatives(problem).sum_hessian()
 
     check_sizes_and_values(autograd_res, backpack_res)
     problem.tear_down()
 
@@ -503,13 +600,17 @@
 def test_make_hessian_mat_prod(problem: DerivativesTestProblem) -> None:
     """Test hessian_mat_prod.
 
     Args:
         problem: test problem
     """
     problem.set_up()
+    skip_BCEWithLogitsLoss(
+        problem
+    )  # TODO Implement _make_hessian_mat_prod for BCEWithLogitsLoss
+
     mat = rand(4, *problem.input_shape, device=problem.device)
 
     autograd_res = AutogradDerivatives(problem).hessian_mat_prod(mat)
     backpack_res = BackpackDerivatives(problem).hessian_mat_prod(mat)
 
     check_sizes_and_values(backpack_res, autograd_res)
```

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/implementation/autograd.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/implementation/autograd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/implementation/backpack.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/implementation/backpack.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Contains derivative calculation with BackPACK."""
 from test.core.derivatives.implementation.base import DerivativesImplementation
 from test.utils import chunk_sizes
 from typing import List
 
 from torch import Tensor, einsum, zeros
 
+from backpack.core.derivatives.nll_base import NLLLossDerivatives
 from backpack.utils.subsampling import subsample
 
 
 class BackpackDerivatives(DerivativesImplementation):
     """Derivative implementations with BackPACK."""
 
     def __init__(self, problem):
@@ -78,37 +79,46 @@
         )
 
     def sum_hessian(self):  # noqa: D102
         self.store_forward_io()
         return self.problem.derivative.sum_hessian(self.problem.module, None, None)
 
     def input_hessian_via_sqrt_hessian(
-        self, mc_samples: int = None, chunks: int = 1, subsampling: List[int] = None
+        self,
+        mc_samples: int = None,
+        chunks: int = 1,
+        subsampling: List[int] = None,
+        use_autograd: bool = False,
     ) -> Tensor:
         """Computes the Hessian w.r.t. to the input from its matrix square root.
 
         Args:
             mc_samples: If int, uses an MC approximation with the specified
                 number of samples. If None, uses the exact hessian. Defaults to None.
             chunks: Maximum sequential split of the computation. Default: ``1``.
                 Only used if mc_samples is specified.
             subsampling: Indices of active samples. ``None`` uses all samples.
+            use_autograd: Compute sampled gradients with ``autograd``. Only relevant
+                for ``NLLLossDerivatives``. Default: ``False``.
 
         Returns:
             Hessian with respect to the input. Has shape
             ``[N, A, B, ..., N, A, B, ...]`` where ``N`` is the batch size or number
             of active samples when sub-sampling is used, and ``[A, B, ...]`` are the
             input's feature dimensions.
         """
         self.store_forward_io()
 
         if mc_samples is not None:
             chunk_samples = chunk_sizes(mc_samples, chunks)
             chunk_weights = [samples / mc_samples for samples in chunk_samples]
 
+            if isinstance(self.problem.derivative, NLLLossDerivatives):
+                self.problem.derivative.use_autograd = use_autograd
+
             individual_hessians: Tensor = sum(
                 weight
                 * self._sample_hessians_from_sqrt(
                     self.problem.derivative.sqrt_hessian_sampled(
                         self.problem.module,
                         None,
                         None,
```

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/implementation/base.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/implementation/base.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/linear_settings.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/linear_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/loss_settings.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/loss_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,14 +73,30 @@
         "target_fn": lambda: regression_targets(size=(5, 3)),
     },
     {
         "module_fn": lambda: torch.nn.MSELoss(reduction="none"),
         "input_fn": lambda: torch.rand(size=(1, 1)),
         "target_fn": lambda: regression_targets(size=(1, 1)),
     },
+    {
+        "module_fn": lambda: torch.nn.BCEWithLogitsLoss(reduction="mean"),
+        "input_fn": lambda: torch.rand(size=(2, 1)),
+        "target_fn": lambda: classification_targets(size=(2, 1), num_classes=2).float(),
+    },
+    {
+        "module_fn": lambda: torch.nn.BCEWithLogitsLoss(reduction="sum"),
+        "input_fn": lambda: torch.rand(size=(4, 1)),
+        "target_fn": lambda: classification_targets(size=(4, 1), num_classes=2).float(),
+    },
+    {
+        "module_fn": lambda: torch.nn.BCEWithLogitsLoss(reduction="mean"),
+        "input_fn": lambda: torch.rand(size=(5, 1)),
+        "target_fn": lambda: torch.rand(size=(5, 1)),
+        "id_prefix": "non-binary-labels",
+    },
 ]
 
 
 LOSS_FAIL_SETTINGS = [
     # non-scalar outputs are not supported
     {
         "module_fn": lambda: torch.nn.CrossEntropyLoss(reduction="none"),
```

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/lstm_settings.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/lstm_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/padding_settings.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/padding_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/permute_settings.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/permute_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/pooling_adaptive_settings.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/pooling_adaptive_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/pooling_settings.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/pooling_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/problem.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from test.core.derivatives.utils import derivative_cls_for, get_available_devices
 from typing import Dict, List, Tuple
 
 import torch
 from torch import Tensor, long
 
 from backpack import extend
-from backpack.utils.module_classification import is_loss
+from backpack.utils.module_classification import is_loss, is_nll
 from backpack.utils.subsampling import subsample
 
 
 def make_test_problems(settings):
     problem_dicts = []
 
     for setting in settings:
@@ -137,14 +137,17 @@
             output = output[0]
 
         return output.shape
 
     def is_loss(self):
         return is_loss(self.make_module())
 
+    def is_nll(self):
+        return is_nll(self.make_module())
+
     def forward_pass(
         self, input_requires_grad: bool = False, subsampling: List[int] = None
     ) -> Tuple[Tensor, Tensor, Dict[str, Tensor]]:
         """Do a forward pass. Return input, output, and parameters."""
         input: Tensor = self.input.clone().detach()
 
         if subsampling is not None:
```

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/rnn_settings.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/rnn_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/scale_module_settings.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/scale_module_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/settings.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/slicing_settings.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/slicing_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/core/derivatives/utils.py` & `backpack-for-pytorch-1.6.0/test/core/derivatives/utils.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/custom_module/test_pad.py` & `backpack-for-pytorch-1.6.0/test/custom_module/test_pad.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/custom_module/test_slicing.py` & `backpack-for-pytorch-1.6.0/test/custom_module/test_slicing.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/automated_settings.py` & `backpack-for-pytorch-1.6.0/test/extensions/automated_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/firstorder/batch_grad/test_batch_grad.py` & `backpack-for-pytorch-1.6.0/test/extensions/firstorder/batch_grad/test_batch_grad.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/firstorder/batch_l2_grad/test_batchl2grad.py` & `backpack-for-pytorch-1.6.0/test/extensions/firstorder/batch_l2_grad/test_batchl2grad.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/firstorder/firstorder_settings.py` & `backpack-for-pytorch-1.6.0/test/extensions/firstorder/firstorder_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/firstorder/sum_grad_squared/sumgradsquared_settings.py` & `backpack-for-pytorch-1.6.0/test/extensions/firstorder/sum_grad_squared/sumgradsquared_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/firstorder/sum_grad_squared/test_sumgradsquared.py` & `backpack-for-pytorch-1.6.0/test/extensions/firstorder/sum_grad_squared/test_sumgradsquared.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/firstorder/variance/test_variance.py` & `backpack-for-pytorch-1.6.0/test/extensions/firstorder/variance/test_variance.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/graph_clear_test.py` & `backpack-for-pytorch-1.6.0/test/extensions/graph_clear_test.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/implementation/autograd.py` & `backpack-for-pytorch-1.6.0/test/extensions/implementation/autograd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/implementation/backpack.py` & `backpack-for-pytorch-1.6.0/test/extensions/implementation/backpack.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 from test.extensions.implementation.hooks import (
     BatchL2GradHook,
     ExtensionHookManager,
     SumGradSquaredHook,
 )
 from test.extensions.problem import ExtensionsTestProblem
 from test.utils import chunk_sizes
+from test.utils.conv_transpose import fix_index_order_conv_transpose_weights
 from typing import List
 
 from torch import Tensor, cat, einsum
 
 import backpack.extensions as new_ext
 from backpack import backpack
+from backpack.utils.kroneckers import kfacs_to_mat
 
 
 class BackpackExtensions(ExtensionsImplementation):
     """Extension implementations with BackPACK."""
 
     def __init__(self, problem: ExtensionsTestProblem):
         """Add BackPACK functionality to, and store, the test case.
@@ -165,26 +167,63 @@
 
     def kfac(self, mc_samples: int = 1) -> List[List[Tensor]]:  # noqa:D102
         with backpack(new_ext.KFAC(mc_samples=mc_samples)):
             _, _, loss = self.problem.forward_pass()
             loss.backward()
         return self.problem.collect_data("kfac")
 
+    def kfac_as_mat(self, chunks: int = 1, mc_samples: int = 1) -> List[Tensor]:
+        """Return the matrix representation of the KFAC approximation.
+
+        Args:
+            chunks: Number of chunks to split the MC samples. Default: `1`.
+            mc_samples: Number of MC samples. Default: `1`.
+
+        Returns:
+            List of tensors containing the block-diagonal Hessian's
+            approximation implied by KFAC in matrix format.
+        """
+        kfac = [
+            kfacs_to_mat(kron_list)
+            for kron_list in self.kfac_chunk(mc_samples=mc_samples, chunks=chunks)
+        ]
+        return fix_index_order_conv_transpose_weights(self.problem.model, kfac)
+
     def kflr(self) -> List[List[Tensor]]:  # noqa:D102
         with backpack(new_ext.KFLR()):
             _, _, loss = self.problem.forward_pass()
             loss.backward()
         return self.problem.collect_data("kflr")
 
+    def kflr_as_mat(self) -> List[Tensor]:
+        """Return the matrix representation of the KFLR approximation.
+
+        Returns:
+            List of tensors containing the block-diagonal Hessian's
+            approximation implied by KFLR in matrix format.
+        """
+        kflr = [kfacs_to_mat(kron_list) for kron_list in self.kflr()]
+        return fix_index_order_conv_transpose_weights(self.problem.model, kflr)
+
     def kfra(self) -> List[List[Tensor]]:  # noqa:D102
         with backpack(new_ext.KFRA()):
             _, _, loss = self.problem.forward_pass()
             loss.backward()
         return self.problem.collect_data("kfra")
 
+    def kfra_as_mat(self) -> List[Tensor]:
+        """Return the matrix representation of the KFRA approximation.
+
+        Returns:
+            List of tensors containing the block-diagonal Hessian's
+            approximation implied by KFRA in matrix format.
+        """
+        kfra = [kfacs_to_mat(kron_list) for kron_list in self.kfra()]
+        return fix_index_order_conv_transpose_weights(self.problem.model, kfra)
+
     def diag_h_batch(self) -> List[Tensor]:  # noqa:D102
         with backpack(new_ext.BatchDiagHessian()):
             _, _, loss = self.problem.forward_pass()
             loss.backward()
         return self.problem.collect_data("diag_h_batch")
 
     def ggn(self, subsampling: List[int] = None) -> Tensor:  # noqa:D102
```

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/implementation/base.py` & `backpack-for-pytorch-1.6.0/test/extensions/implementation/base.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/implementation/hooks.py` & `backpack-for-pytorch-1.6.0/test/extensions/implementation/hooks.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/problem.py` & `backpack-for-pytorch-1.6.0/test/extensions/problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
 
         for p in self.model.parameters():
             if p.requires_grad:
                 data.append(getattr(p, savefield))
             else:
                 if hasattr(p, savefield):
                     raise RuntimeError(
-                        f"Found non-differentiable parameter with attribute '{savefield}'."
+                        f"Found non-differentiable parameter with attribute {savefield}."
                     )
 
         return data
 
     def get_batch_size(self) -> int:
         """Return the mini-batch size.
```

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/secondorder/diag_ggn/diag_ggn_settings.py` & `backpack-for-pytorch-1.6.0/test/extensions/secondorder/diag_ggn/diag_ggn_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/secondorder/diag_ggn/test_batch_diag_ggn.py` & `backpack-for-pytorch-1.6.0/test/extensions/secondorder/diag_ggn/test_batch_diag_ggn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Test BatchDiagGGN extension."""
 from test.automated_test import check_sizes_and_values
 from test.extensions.implementation.autograd import AutogradExtensions
 from test.extensions.implementation.backpack import BackpackExtensions
 from test.extensions.problem import make_test_problems
 from test.extensions.secondorder.diag_ggn.diag_ggn_settings import DiagGGN_SETTINGS
-from test.utils.skip_test import skip_adaptive_avg_pool3d_cuda
+from test.utils.skip_extension_test import skip_BCEWithLogitsLoss_non_binary_labels
+from test.utils.skip_test import skip_adaptive_avg_pool3d_cuda, skip_torch_2_0_1_lstm
 
 import pytest
 
 PROBLEMS = make_test_problems(DiagGGN_SETTINGS)
 IDS = [problem.make_id() for problem in PROBLEMS]
 
 
@@ -18,14 +19,15 @@
 
     Args:
         problem (ExtensionsTestProblem): Problem for extension test.
         request: problem request
     """
     skip_adaptive_avg_pool3d_cuda(request)
     problem.set_up()
+    skip_torch_2_0_1_lstm(problem.model)
 
     backpack_res = BackpackExtensions(problem).diag_ggn_exact_batch()
     autograd_res = AutogradExtensions(problem).diag_ggn_exact_batch()
 
     check_sizes_and_values(autograd_res, backpack_res)
     problem.tear_down()
 
@@ -41,14 +43,16 @@
 
     of Generalized Gauss-Newton/Fisher with few mc_samples (light version)
 
     Args:
         problem (ExtensionsTestProblem): Problem for extension test.
     """
     problem.set_up()
+    skip_BCEWithLogitsLoss_non_binary_labels(problem)
+    skip_torch_2_0_1_lstm(problem.model)
 
     backpack_res = BackpackExtensions(problem).diag_ggn_exact_batch()
     mc_samples = 6000
     backpack_res_mc_avg = BackpackExtensions(problem).diag_ggn_mc_batch(mc_samples)
 
     check_sizes_and_values(
         backpack_res, backpack_res_mc_avg, atol=MC_ATOL, rtol=MC_LIGHT_RTOL
@@ -63,14 +67,16 @@
 
     of generalized Gauss-Newton with more samples (slow version)
 
     Args:
         problem (ExtensionsTestProblem): Problem for extension test.
     """
     problem.set_up()
+    skip_BCEWithLogitsLoss_non_binary_labels(problem)
+    skip_torch_2_0_1_lstm(problem.model)
 
     backpack_res = BackpackExtensions(problem).diag_ggn_exact_batch()
     mc_samples = 300000
     chunks = 30
     backpack_res_mc_avg = BackpackExtensions(problem).diag_ggn_mc_batch_chunk(
         mc_samples, chunks=chunks
     )
```

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/secondorder/diag_ggn/test_diag_ggn.py` & `backpack-for-pytorch-1.6.0/test/extensions/secondorder/diag_ggn/test_diag_ggn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Test DiagGGN extension."""
 from test.automated_test import check_sizes_and_values
 from test.extensions.implementation.autograd import AutogradExtensions
 from test.extensions.implementation.backpack import BackpackExtensions
 from test.extensions.problem import make_test_problems
 from test.extensions.secondorder.diag_ggn.diag_ggn_settings import DiagGGN_SETTINGS
-from test.utils.skip_test import skip_adaptive_avg_pool3d_cuda
+from test.utils.skip_extension_test import skip_BCEWithLogitsLoss_non_binary_labels
+from test.utils.skip_test import skip_adaptive_avg_pool3d_cuda, skip_torch_2_0_1_lstm
 
 import pytest
 
 PROBLEMS = make_test_problems(DiagGGN_SETTINGS)
 IDS = [problem.make_id() for problem in PROBLEMS]
 
 
@@ -18,14 +19,15 @@
 
     Args:
         problem (ExtensionsTestProblem): Problem for extension test.
         request: problem request
     """
     skip_adaptive_avg_pool3d_cuda(request)
     problem.set_up()
+    skip_torch_2_0_1_lstm(problem.model)
 
     backpack_res = BackpackExtensions(problem).diag_ggn()
     autograd_res = AutogradExtensions(problem).diag_ggn()
 
     check_sizes_and_values(autograd_res, backpack_res)
     problem.tear_down()
 
@@ -41,14 +43,16 @@
 
     with few mc_samples (light version)
 
     Args:
         problem (ExtensionsTestProblem): Problem for extension test.
     """
     problem.set_up()
+    skip_BCEWithLogitsLoss_non_binary_labels(problem)
+    skip_torch_2_0_1_lstm(problem.model)
 
     backpack_res = BackpackExtensions(problem).diag_ggn()
     mc_samples = 3000
     backpack_res_mc_avg = BackpackExtensions(problem).diag_ggn_mc(mc_samples)
 
     check_sizes_and_values(
         backpack_res, backpack_res_mc_avg, atol=MC_ATOL, rtol=MC_LIGHT_RTOL
@@ -63,14 +67,16 @@
 
     with more samples (slow version)
 
     Args:
         problem (ExtensionsTestProblem): Problem for extension test.
     """
     problem.set_up()
+    skip_BCEWithLogitsLoss_non_binary_labels(problem)
+    skip_torch_2_0_1_lstm(problem.model)
 
     backpack_res = BackpackExtensions(problem).diag_ggn()
     mc_samples = 300000
     chunks = 30
     backpack_res_mc_avg = BackpackExtensions(problem).diag_ggn_mc_chunk(
         mc_samples, chunks=chunks
     )
```

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/secondorder/diag_hessian/diagh_settings.py` & `backpack-for-pytorch-1.6.0/test/extensions/secondorder/diag_hessian/diagh_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-"""Test configurations to test diag_h.
+"""Test cases for DiagHessian and BatchDiagHessian extensions.
 
 The tests are taken from `test.extensions.secondorder.secondorder_settings`,
 but additional custom tests can be defined here by appending it to the list.
 """
 
 from test.extensions.automated_settings import make_simple_act_setting
 from test.extensions.secondorder.secondorder_settings import SECONDORDER_SETTINGS
 
 from torch.nn import LogSigmoid
 
-DiagHESSIAN_SETTINGS = []
-
 SHARED_SETTINGS = SECONDORDER_SETTINGS
-LOCAL_SETTINGS = []
-LOCAL_SETTINGS.append(make_simple_act_setting(LogSigmoid, bias=True))
-LOCAL_SETTINGS.append(make_simple_act_setting(LogSigmoid, bias=False))
+LOCAL_SETTINGS = [
+    make_simple_act_setting(LogSigmoid, bias=True),
+    make_simple_act_setting(LogSigmoid, bias=False),
+]
 
 DiagHESSIAN_SETTINGS = SHARED_SETTINGS + LOCAL_SETTINGS
```

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/secondorder/diag_hessian/test_diag_hessian.py` & `backpack-for-pytorch-1.6.0/test/extensions/secondorder/diag_hessian/test_diag_hessian.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/secondorder/hbp/test_kfac.py` & `backpack-for-pytorch-1.6.0/test/extensions/secondorder/hbp/test_kfac.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 from test.extensions.implementation.autograd import AutogradExtensions
 from test.extensions.implementation.backpack import BackpackExtensions
 from test.extensions.problem import ExtensionsTestProblem, make_test_problems
 from test.extensions.secondorder.hbp.kfac_settings import (
     BATCH_SIZE_1_SETTINGS,
     NOT_SUPPORTED_SETTINGS,
 )
+from test.utils.skip_extension_test import skip_BCEWithLogitsLoss_non_binary_labels
 
 import pytest
 
-from backpack.utils.kroneckers import kfacs_to_mat
-
 NOT_SUPPORTED_PROBLEMS = make_test_problems(NOT_SUPPORTED_SETTINGS)
 NOT_SUPPORTED_IDS = [problem.make_id() for problem in NOT_SUPPORTED_PROBLEMS]
 BATCH_SIZE_1_PROBLEMS = make_test_problems(BATCH_SIZE_1_SETTINGS)
 BATCH_SIZE_1_IDS = [problem.make_id() for problem in BATCH_SIZE_1_PROBLEMS]
 
 
 @pytest.mark.parametrize("problem", NOT_SUPPORTED_PROBLEMS, ids=NOT_SUPPORTED_IDS)
@@ -40,19 +39,21 @@
 
     Should be true for linear layers and in the limit of infinite mc_samples.
 
     Args:
         problem: Test case.
     """
     problem.set_up()
+    skip_BCEWithLogitsLoss_non_binary_labels(problem)
     autograd_res = AutogradExtensions(problem).ggn_blocks()
 
     mc_samples = 300000
-    backpack_kfac = BackpackExtensions(problem).kfac_chunk(mc_samples)
-    backpack_res = [kfacs_to_mat(kfac) for kfac in backpack_kfac]
+    backpack_res = BackpackExtensions(problem).kfac_as_mat(
+        chunks=10, mc_samples=mc_samples
+    )
 
     check_sizes_and_values(autograd_res, backpack_res, atol=5e-3, rtol=5e-3)
 
     problem.tear_down()
 
 
 @pytest.mark.parametrize("problem", BATCH_SIZE_1_PROBLEMS, ids=BATCH_SIZE_1_IDS)
@@ -61,16 +62,16 @@
 
      Should be true for linear layers and in the limit of infinite mc_samples.
 
     Args:
         problem: Test case.
     """
     problem.set_up()
-    autograd_res = AutogradExtensions(problem).ggn_blocks()
+    skip_BCEWithLogitsLoss_non_binary_labels(problem)
 
+    autograd_res = AutogradExtensions(problem).ggn_blocks()
     mc_samples = 6000
-    backpack_kfac = BackpackExtensions(problem).kfac(mc_samples)
-    backpack_res = [kfacs_to_mat(kfac) for kfac in backpack_kfac]
+    backpack_res = BackpackExtensions(problem).kfac_as_mat(mc_samples=mc_samples)
 
     check_sizes_and_values(autograd_res, backpack_res, atol=1e-2, rtol=1e-2)
 
     problem.tear_down()
```

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/secondorder/secondorder_settings.py` & `backpack-for-pytorch-1.6.0/test/extensions/secondorder/secondorder_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from torch import device, rand
 from torch.nn import (
     ELU,
     SELU,
     AvgPool1d,
     AvgPool2d,
     AvgPool3d,
+    BCEWithLogitsLoss,
     Conv1d,
     Conv2d,
     Conv3d,
     ConvTranspose1d,
     ConvTranspose2d,
     ConvTranspose3d,
     CrossEntropyLoss,
@@ -362,7 +363,28 @@
             Slicing((slice(None), 1)),
             Linear(6, 4),
         ),
         "loss_function_fn": lambda: MSELoss(reduction="mean"),
         "target_fn": lambda: regression_targets((3, 4)),
     },
 ]
+
+
+###############################################################################
+#                              BCEWithLogitsLoss                              #
+###############################################################################
+SECONDORDER_SETTINGS += [
+    {
+        "input_fn": lambda: rand(3, 6),
+        "module_fn": lambda: Sequential(Linear(6, 4), ReLU(), Linear(4, 1)),
+        "loss_function_fn": lambda: BCEWithLogitsLoss(reduction="mean"),
+        "target_fn": lambda: rand(3, 1),
+        "id_prefix": "non-binary-labels",
+    },
+    {
+        "input_fn": lambda: rand(3, 6),
+        "module_fn": lambda: Sequential(Linear(6, 4), ReLU(), Linear(4, 1)),
+        "loss_function_fn": lambda: BCEWithLogitsLoss(reduction="sum"),
+        "target_fn": lambda: classification_targets(size=(3, 1), num_classes=2).float(),
+        "id_prefix": "binary-labels",
+    },
+]
```

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/secondorder/sqrt_ggn/sqrt_ggn_settings.py` & `backpack-for-pytorch-1.6.0/test/extensions/secondorder/sqrt_ggn/sqrt_ggn_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/secondorder/sqrt_ggn/test_sqrt_ggn.py` & `backpack-for-pytorch-1.6.0/test/extensions/secondorder/sqrt_ggn/test_sqrt_ggn.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from math import isclose
 from test.automated_test import check_sizes_and_values
 from test.extensions.implementation.autograd import AutogradExtensions
 from test.extensions.implementation.backpack import BackpackExtensions
 from test.extensions.problem import ExtensionsTestProblem, make_test_problems
 from test.extensions.secondorder.sqrt_ggn.sqrt_ggn_settings import SQRT_GGN_SETTINGS
+from test.utils.skip_extension_test import skip_BCEWithLogitsLoss_non_binary_labels
 from test.utils.skip_test import skip_large_parameters, skip_subsampling_conflict
 from typing import List, Union
 
 from pytest import fixture, mark
 
 PROBLEMS = make_test_problems(SQRT_GGN_SETTINGS)
 
@@ -66,14 +67,15 @@
 
     Args:
         problem: Test case with small network whose GGN can be evaluated.
         subsampling: Indices of active samples. ``None`` uses the full mini-batch.
     """
     skip_large_parameters(problem)
     skip_subsampling_conflict(problem, subsampling)
+    skip_BCEWithLogitsLoss_non_binary_labels(problem)
 
     BackpackExtensions(problem).sqrt_ggn_mc(mc_samples=1, subsampling=subsampling)
 
 
 @mark.montecarlo
 @mark.parametrize("subsampling", SUBSAMPLINGS, ids=SUBSAMPLING_IDS)
 def test_ggn_mc(
@@ -83,14 +85,15 @@
 
     Args:
         problem: Test case with small network whose GGN can be evaluated.
         subsampling: Indices of active samples. ``None`` uses the full mini-batch.
     """
     skip_large_parameters(problem)
     skip_subsampling_conflict(problem, subsampling)
+    skip_BCEWithLogitsLoss_non_binary_labels(problem)
 
     autograd_res = AutogradExtensions(problem).ggn(subsampling=subsampling)
     atol, rtol = 5e-3, 5e-3
     mc_samples, chunks = 150000, 15
     backpack_res = BackpackExtensions(problem).ggn_mc(
         mc_samples, chunks=chunks, subsampling=subsampling
     )
```

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/test_backprop_extension.py` & `backpack-for-pytorch-1.6.0/test/extensions/test_backprop_extension.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/test_hooks.py` & `backpack-for-pytorch-1.6.0/test/extensions/test_hooks.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/extensions/utils.py` & `backpack-for-pytorch-1.6.0/test/extensions/utils.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/implementation/implementation.py` & `backpack-for-pytorch-1.6.0/test/implementation/implementation.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/implementation/implementation_autograd.py` & `backpack-for-pytorch-1.6.0/test/implementation/implementation_autograd.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/implementation/implementation_bpext.py` & `backpack-for-pytorch-1.6.0/test/implementation/implementation_bpext.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/interface_test.py` & `backpack-for-pytorch-1.6.0/test/interface_test.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/linear_test.py` & `backpack-for-pytorch-1.6.0/test/linear_test.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/networks.py` & `backpack-for-pytorch-1.6.0/test/networks.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/problems.py` & `backpack-for-pytorch-1.6.0/test/problems.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/readme.md` & `backpack-for-pytorch-1.6.0/test/readme.md`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/test___init__.py` & `backpack-for-pytorch-1.6.0/test/test___init__.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/test_batch_first.py` & `backpack-for-pytorch-1.6.0/test/test_batch_first.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/test_problem.py` & `backpack-for-pytorch-1.6.0/test/test_problem.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/test_problems_activations.py` & `backpack-for-pytorch-1.6.0/test/test_problems_activations.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 }
 INPUT_SHAPE = (TEST_SETTINGS["batch"], TEST_SETTINGS["in_features"])
 
 TEST_PROBLEMS = {}
 
 for act_name, act_cls in ACTIVATIONS.items():
     for lin_name, lin_cls in LINEARS.items():
-
         TEST_PROBLEMS[
             "{}{}-regression".format(lin_name, act_name)
         ] = make_regression_problem(
             INPUT_SHAPE,
             single_linear_layer(TEST_SETTINGS, lin_cls, activation_cls=act_cls),
         )
```

### Comparing `backpack-for-pytorch-1.5.2/test/test_problems_bn.py` & `backpack-for-pytorch-1.6.0/test/test_problems_bn.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 
 INPUT_SHAPE = (TEST_SETTINGS["batch"], TEST_SETTINGS["in_features"])
 
 TEST_PROBLEMS = {}
 
 for lin_name, lin_cls in LINEARS.items():
-
     TEST_PROBLEMS["{}-bn-regression".format(lin_name)] = make_regression_problem(
         INPUT_SHAPE,
         single_linear_layer(TEST_SETTINGS, lin_cls, activation_cls=None)
         + [BatchNorm1d(TEST_SETTINGS["out_features"])],
     )
 
     TEST_PROBLEMS[
```

### Comparing `backpack-for-pytorch-1.5.2/test/test_problems_convolutions.py` & `backpack-for-pytorch-1.6.0/test/test_problems_convolutions.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/test_problems_kfacs.py` & `backpack-for-pytorch-1.6.0/test/test_problems_kfacs.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,14 @@
         )
 
 TEST_PROBLEMS = {
     **REGRESSION_PROBLEMS,
 }
 for act_name, act_cls in ACTIVATIONS.items():
     for lin_name, lin_cls in LINEARS.items():
-
         TEST_PROBLEMS[
             "{}{}-classification".format(lin_name, act_name)
         ] = make_classification_problem(
             INPUT_SHAPE,
             single_linear_layer(TEST_SETTINGS, lin_cls, activation_cls=act_cls),
         )
```

### Comparing `backpack-for-pytorch-1.5.2/test/test_problems_linear.py` & `backpack-for-pytorch-1.6.0/test/test_problems_linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     "atol": 1e-5,
 }
 INPUT_SHAPE = (TEST_SETTINGS["batch"], TEST_SETTINGS["in_features"])
 
 TEST_PROBLEMS = {}
 
 for lin_name, lin_cls in LINEARS.items():
-
     TEST_PROBLEMS["{}-regression".format(lin_name)] = make_regression_problem(
         INPUT_SHAPE, single_linear_layer(TEST_SETTINGS, lin_cls, activation_cls=None)
     )
 
     TEST_PROBLEMS["{}-classification".format(lin_name)] = make_classification_problem(
         INPUT_SHAPE, single_linear_layer(TEST_SETTINGS, lin_cls, activation_cls=None)
     )
```

### Comparing `backpack-for-pytorch-1.5.2/test/test_problems_padding.py` & `backpack-for-pytorch-1.6.0/test/test_problems_padding.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/test_problems_pooling.py` & `backpack-for-pytorch-1.6.0/test/test_problems_pooling.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/test_retain_graph.py` & `backpack-for-pytorch-1.6.0/test/test_retain_graph.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/test_second_order_warnings.py` & `backpack-for-pytorch-1.6.0/test/test_second_order_warnings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/utils/__init__.py` & `backpack-for-pytorch-1.6.0/test/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/utils/evaluation_mode.py` & `backpack-for-pytorch-1.6.0/test/utils/evaluation_mode.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/utils/test_conv.py` & `backpack-for-pytorch-1.6.0/test/utils/test_conv.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/utils/test_conv_settings.py` & `backpack-for-pytorch-1.6.0/test/utils/test_conv_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/utils/test_conv_transpose.py` & `backpack-for-pytorch-1.6.0/test/utils/test_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/utils/test_conv_transpose_settings.py` & `backpack-for-pytorch-1.6.0/test/utils/test_conv_transpose_settings.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/utils/test_subsampling.py` & `backpack-for-pytorch-1.6.0/test/utils/test_subsampling.py`

 * *Files identical despite different names*

### Comparing `backpack-for-pytorch-1.5.2/test/utils_test.py` & `backpack-for-pytorch-1.6.0/test/utils_test.py`

 * *Files identical despite different names*


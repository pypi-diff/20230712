# Comparing `tmp/spox-0.8.0.tar.gz` & `tmp/spox-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spox-0.8.0.tar", last modified: Thu May 11 10:38:01 2023, max compression
+gzip compressed data, was "spox-0.9.0.tar", last modified: Wed Jul 12 18:43:49 2023, max compression
```

## Comparing `spox-0.8.0.tar` & `spox-0.9.0.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.581310 spox-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)      313 2023-05-11 10:37:53.000000 spox-0.8.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-11 10:37:53.000000 spox-0.8.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.565310 spox-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-11 10:37:53.000000 spox-0.8.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-11 10:37:53.000000 spox-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-05-11 10:37:53.000000 spox-0.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.565310 spox-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-05-11 10:37:53.000000 spox-0.8.0/.github/workflows/build_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-05-11 10:37:53.000000 spox-0.8.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-05-11 10:37:53.000000 spox-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-05-11 10:37:53.000000 spox-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-11 10:37:53.000000 spox-0.8.0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-05-11 10:37:53.000000 spox-0.8.0/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-11 10:37:53.000000 spox-0.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     5718 2023-05-11 10:37:53.000000 spox-0.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-05-11 10:37:53.000000 spox-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-05-11 10:38:01.581310 spox-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3074 2023-05-11 10:37:53.000000 spox-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.565310 spox-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-11 10:37:53.000000 spox-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-05-11 10:37:53.000000 spox-0.8.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.565310 spox-0.8.0/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (122)    15415 2023-05-11 10:37:53.000000 spox-0.8.0/docs/guides/advanced.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    11423 2023-05-11 10:37:53.000000 spox-0.8.0/docs/guides/converter.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    38133 2023-05-11 10:37:53.000000 spox-0.8.0/docs/guides/example-model-netron.png
--rw-r--r--   0 runner    (1001) docker     (122)    15822 2023-05-11 10:37:53.000000 spox-0.8.0/docs/guides/inference.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     9165 2023-05-11 10:37:53.000000 spox-0.8.0/docs/guides/inline.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    50579 2023-05-11 10:37:53.000000 spox-0.8.0/docs/guides/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-05-11 10:37:53.000000 spox-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      793 2023-05-11 10:37:53.000000 spox-0.8.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.569310 spox-0.8.0/docs/manual/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-11 10:37:53.000000 spox-0.8.0/docs/manual/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11022 2023-05-11 10:37:53.000000 spox-0.8.0/docs/manual/operators.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5279 2023-05-11 10:37:53.000000 spox-0.8.0/docs/manual/overview.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7928 2023-05-11 10:37:53.000000 spox-0.8.0/docs/manual/unstable.rst
--rw-r--r--   0 runner    (1001) docker     (122)      436 2023-05-11 10:37:53.000000 spox-0.8.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-05-11 10:37:53.000000 spox-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 10:38:01.581310 spox-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.565310 spox-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.569310 spox-0.8.0/src/spox/
--rw-r--r--   0 runner    (1001) docker     (122)      877 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4193 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_adapt.py
--rw-r--r--   0 runner    (1001) docker     (122)     6644 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_attributes.py
--rw-r--r--   0 runner    (1001) docker     (122)    19315 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_build.py
--rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_debug.py
--rw-r--r--   0 runner    (1001) docker     (122)      926 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4004 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)     7117 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_function.py
--rw-r--r--   0 runner    (1001) docker     (122)     7285 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_future.py
--rw-r--r--   0 runner    (1001) docker     (122)    18828 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     4750 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_inline.py
--rw-r--r--   0 runner    (1001) docker     (122)     8733 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_internal_op.py
--rw-r--r--   0 runner    (1001) docker     (122)    15132 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_node.py
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_patch_ref_impl.py
--rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_public.py
--rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (122)     7148 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_scope.py
--rw-r--r--   0 runner    (1001) docker     (122)     8460 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_shape.py
--rw-r--r--   0 runner    (1001) docker     (122)    10455 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_standard.py
--rw-r--r--   0 runner    (1001) docker     (122)     3237 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_traverse.py
--rw-r--r--   0 runner    (1001) docker     (122)     9434 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_type_system.py
--rw-r--r--   0 runner    (1001) docker     (122)     2191 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     6537 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_value_prop.py
--rw-r--r--   0 runner    (1001) docker     (122)     7478 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_var.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.565310 spox-0.8.0/src/spox/opset/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.565310 spox-0.8.0/src/spox/opset/ai/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.573310 spox-0.8.0/src/spox/opset/ai/onnx/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.573310 spox-0.8.0/src/spox/opset/ai/onnx/ml/
--rw-r--r--   0 runner    (1001) docker     (122)    63324 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/opset/ai/onnx/ml/v3.py
--rw-r--r--   0 runner    (1001) docker     (122)   461188 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/opset/ai/onnx/v17.py
--rw-r--r--   0 runner    (1001) docker     (122)    93407 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/opset/ai/onnx/v18.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.569310 spox-0.8.0/src/spox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-05-11 10:38:01.000000 spox-0.8.0/src/spox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3871 2023-05-11 10:38:01.000000 spox-0.8.0/src/spox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 10:38:01.000000 spox-0.8.0/src/spox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-11 10:38:01.000000 spox-0.8.0/src/spox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-11 10:38:01.000000 spox-0.8.0/src/spox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.573310 spox-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 10:37:53.000000 spox-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-05-11 10:37:53.000000 spox-0.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.573310 spox-0.8.0/tests/full/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 10:37:53.000000 spox-0.8.0/tests/full/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4623 2023-05-11 10:37:53.000000 spox-0.8.0/tests/full/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      918 2023-05-11 10:37:53.000000 spox-0.8.0/tests/full/test_brackets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-05-11 10:37:53.000000 spox-0.8.0/tests/full/test_lifting.py
--rw-r--r--   0 runner    (1001) docker     (122)     5908 2023-05-11 10:37:53.000000 spox-0.8.0/tests/full/test_turing_completeness.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.573310 spox-0.8.0/tests/future/
--rw-r--r--   0 runner    (1001) docker     (122)     3662 2023-05-11 10:37:53.000000 spox-0.8.0/tests/future/test_var_operators.py
--rw-r--r--   0 runner    (1001) docker     (122)     3304 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_adapt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_constructors.py
--rw-r--r--   0 runner    (1001) docker     (122)     3036 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_custom_operator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_equiv_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    10402 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_initializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6869 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_inline.py
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_opsets.py
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_optional.py
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_public.py
--rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_standard_op.py
--rw-r--r--   0 runner    (1001) docker     (122)    12965 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_subgraphs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2043 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_type_translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4651 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_value_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.577310 spox-0.8.0/tests/type_inference/
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_array_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_binarizer.py
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_category_mapper.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_imputer.py
--rw-r--r--   0 runner    (1001) docker     (122)      907 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_linear_regressor.py
--rw-r--r--   0 runner    (1001) docker     (122)      418 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_loop.py
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_one_hot.py
--rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)      596 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_scaler.py
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_tree_ensemble_classifier.py
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_tree_ensemble_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.577310 spox-0.8.0/tools/
--rw-r--r--   0 runner    (1001) docker     (122)    25288 2023-05-11 10:37:53.000000 spox-0.8.0/tools/generate_opset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.577310 spox-0.8.0/tools/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/class.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/construct.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/constructor.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/docstring.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.577310 spox-0.8.0/tools/templates/extras/
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/extras/const.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      885 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/extras/promote.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/extras/xif.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/extras/xloop.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/inherit.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/preamble.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/summary.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.581310 spox-0.8.0/tools/templates/type_inference/
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/arrayfeatureextractor1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/binarizer1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/categorymapper1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      767 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/compress11.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/if16.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     1021 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/imputer1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/linearregressor1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/loop16-fix.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     2523 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/loop16.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/normalizer1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/onehot11.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/onehotencoder1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/scaler1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/treeensembleclassifier3.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/treeensembleregressor3.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.581310 spox-0.8.0/tools/templates/value_propagation/
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/value_propagation/constant13.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.771358 spox-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      313 2023-07-12 18:43:41.000000 spox-0.9.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-07-12 18:43:41.000000 spox-0.9.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.751358 spox-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-12 18:43:41.000000 spox-0.9.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-12 18:43:41.000000 spox-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-12 18:43:41.000000 spox-0.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.751358 spox-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-07-12 18:43:41.000000 spox-0.9.0/.github/workflows/build_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-07-12 18:43:41.000000 spox-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-07-12 18:43:41.000000 spox-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-07-12 18:43:41.000000 spox-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-07-12 18:43:41.000000 spox-0.9.0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-07-12 18:43:41.000000 spox-0.9.0/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-07-12 18:43:41.000000 spox-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     6621 2023-07-12 18:43:41.000000 spox-0.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-07-12 18:43:41.000000 spox-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-07-12 18:43:49.771358 spox-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3074 2023-07-12 18:43:41.000000 spox-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.755358 spox-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-07-12 18:43:41.000000 spox-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-07-12 18:43:41.000000 spox-0.9.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.755358 spox-0.9.0/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (122)    15415 2023-07-12 18:43:41.000000 spox-0.9.0/docs/guides/advanced.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    11423 2023-07-12 18:43:41.000000 spox-0.9.0/docs/guides/converter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    38133 2023-07-12 18:43:41.000000 spox-0.9.0/docs/guides/example-model-netron.png
+-rw-r--r--   0 runner    (1001) docker     (122)    15822 2023-07-12 18:43:41.000000 spox-0.9.0/docs/guides/inference.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     9165 2023-07-12 18:43:41.000000 spox-0.9.0/docs/guides/inline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    50579 2023-07-12 18:43:41.000000 spox-0.9.0/docs/guides/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-07-12 18:43:41.000000 spox-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      793 2023-07-12 18:43:41.000000 spox-0.9.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.755358 spox-0.9.0/docs/manual/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-07-12 18:43:41.000000 spox-0.9.0/docs/manual/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11022 2023-07-12 18:43:41.000000 spox-0.9.0/docs/manual/operators.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5279 2023-07-12 18:43:41.000000 spox-0.9.0/docs/manual/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7928 2023-07-12 18:43:41.000000 spox-0.9.0/docs/manual/unstable.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-07-12 18:43:41.000000 spox-0.9.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-07-12 18:43:41.000000 spox-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 18:43:49.771358 spox-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.747358 spox-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.759358 spox-0.9.0/src/spox/
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4193 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_adapt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6644 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20284 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4004 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7117 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7285 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_future.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18828 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_inline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8733 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_internal_op.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15132 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_node.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10393 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_public.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7601 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_scope.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8460 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_shape.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10455 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_standard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3237 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_traverse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9434 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_type_system.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2191 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7065 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_value_prop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7478 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/_var.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.751358 spox-0.9.0/src/spox/opset/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.751358 spox-0.9.0/src/spox/opset/ai/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.759358 spox-0.9.0/src/spox/opset/ai/onnx/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.759358 spox-0.9.0/src/spox/opset/ai/onnx/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)    63350 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/opset/ai/onnx/ml/v3.py
+-rw-r--r--   0 runner    (1001) docker     (122)   462668 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/opset/ai/onnx/v17.py
+-rw-r--r--   0 runner    (1001) docker     (122)    93775 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/opset/ai/onnx/v18.py
+-rw-r--r--   0 runner    (1001) docker     (122)    99994 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/opset/ai/onnx/v19.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:41.000000 spox-0.9.0/src/spox/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.759358 spox-0.9.0/src/spox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-07-12 18:43:49.000000 spox-0.9.0/src/spox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3873 2023-07-12 18:43:49.000000 spox-0.9.0/src/spox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 18:43:49.000000 spox-0.9.0/src/spox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-12 18:43:49.000000 spox-0.9.0/src/spox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-12 18:43:49.000000 spox-0.9.0/src/spox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.763358 spox-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:41.000000 spox-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-07-12 18:43:41.000000 spox-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.763358 spox-0.9.0/tests/full/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:41.000000 spox-0.9.0/tests/full/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4623 2023-07-12 18:43:41.000000 spox-0.9.0/tests/full/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      918 2023-07-12 18:43:41.000000 spox-0.9.0/tests/full/test_brackets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-12 18:43:41.000000 spox-0.9.0/tests/full/test_lifting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5908 2023-07-12 18:43:41.000000 spox-0.9.0/tests/full/test_turing_completeness.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.763358 spox-0.9.0/tests/future/
+-rw-r--r--   0 runner    (1001) docker     (122)     3662 2023-07-12 18:43:41.000000 spox-0.9.0/tests/future/test_var_operators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3304 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_adapt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3036 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_custom_operator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_equiv_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10402 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9729 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_inline.py
+-rw-r--r--   0 runner    (1001) docker     (122)      734 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_opsets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_optional.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_standard_op.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13367 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_subgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2043 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_type_translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4971 2023-07-12 18:43:41.000000 spox-0.9.0/tests/test_value_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.767358 spox-0.9.0/tests/type_inference/
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-07-12 18:43:41.000000 spox-0.9.0/tests/type_inference/test_array_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-07-12 18:43:41.000000 spox-0.9.0/tests/type_inference/test_binarizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-07-12 18:43:41.000000 spox-0.9.0/tests/type_inference/test_category_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-07-12 18:43:41.000000 spox-0.9.0/tests/type_inference/test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-07-12 18:43:41.000000 spox-0.9.0/tests/type_inference/test_imputer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-07-12 18:43:41.000000 spox-0.9.0/tests/type_inference/test_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-07-12 18:43:41.000000 spox-0.9.0/tests/type_inference/test_linear_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2023-07-12 18:43:41.000000 spox-0.9.0/tests/type_inference/test_loop.py
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-07-12 18:43:41.000000 spox-0.9.0/tests/type_inference/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-12 18:43:41.000000 spox-0.9.0/tests/type_inference/test_one_hot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-07-12 18:43:41.000000 spox-0.9.0/tests/type_inference/test_one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)      596 2023-07-12 18:43:41.000000 spox-0.9.0/tests/type_inference/test_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-07-12 18:43:41.000000 spox-0.9.0/tests/type_inference/test_tree_ensemble_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-07-12 18:43:41.000000 spox-0.9.0/tests/type_inference/test_tree_ensemble_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.767358 spox-0.9.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)    26060 2023-07-12 18:43:41.000000 spox-0.9.0/tools/generate_opset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.767358 spox-0.9.0/tools/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/class.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/construct.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/constructor.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/docstring.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.767358 spox-0.9.0/tools/templates/extras/
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/extras/const.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/extras/promote.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/extras/xif.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/extras/xloop.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/inherit.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/preamble.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/summary.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.771358 spox-0.9.0/tools/templates/type_inference/
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/type_inference/arrayfeatureextractor1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/type_inference/binarizer1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/type_inference/categorymapper1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/type_inference/compress11.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/type_inference/if16.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     1021 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/type_inference/imputer1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/type_inference/linearregressor1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/type_inference/loop16-fix.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     2523 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/type_inference/loop16.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/type_inference/normalizer1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/type_inference/onehot11.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/type_inference/onehotencoder1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/type_inference/scaler1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/type_inference/treeensembleclassifier3.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/type_inference/treeensembleregressor3.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 18:43:49.771358 spox-0.9.0/tools/templates/value_propagation/
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-12 18:43:41.000000 spox-0.9.0/tools/templates/value_propagation/constant13.jinja2
```

### Comparing `spox-0.8.0/.github/workflows/build_and_publish.yml` & `spox-0.9.0/.github/workflows/build_and_publish.yml`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/.github/workflows/ci.yml` & `spox-0.9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/.gitignore` & `spox-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/.pre-commit-config.yaml` & `spox-0.9.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/Quantco/pre-commit-mirrors-black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black-conda
         args:
           - --safe
           - --target-version=py38
   - repo: https://github.com/Quantco/pre-commit-mirrors-flake8
     rev: 6.0.0
@@ -12,20 +12,20 @@
       - id: flake8-conda
   - repo: https://github.com/Quantco/pre-commit-mirrors-isort
     rev: 5.12.0
     hooks:
       - id: isort-conda
         additional_dependencies: [-c, conda-forge, toml=0.10.2]
   - repo: https://github.com/Quantco/pre-commit-mirrors-mypy
-    rev: "0.991"
+    rev: "1.4.0"
     hooks:
       - id: mypy-conda
         additional_dependencies: [-c, conda-forge, types-setuptools]
   - repo: https://github.com/Quantco/pre-commit-mirrors-pyupgrade
-    rev: 3.3.1
+    rev: 3.7.0
     hooks:
       - id: pyupgrade-conda
         args:
           - --py38
   - repo: https://github.com/Quantco/pre-commit-mirrors-prettier
     rev: 2.7.1
     hooks:
```

### Comparing `spox-0.8.0/CHANGELOG.rst` & `spox-0.9.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,38 @@
    * Update the major if you break the public API
    * Update the minor if you add new functionality
    * Update the patch if you fixed a bug
 
 Change log
 ==========
 
+0.9.0 (2023-06-12)
+------------------
+
+**New features**
+
+- The opset ``ai.onnx@19`` (ONNX 1.14) is now shipped with Spox.
+
+**Bug fixes**
+
+- The constructor for ``ai.onnx@18::Split`` is no longer generated incorrectly. No extraneous attribute is generated anymore, and the ``num_outputs`` attribute is marked as required (so that Spox can infer the number of outputs).
+- Fix an issue where op.const handled numbers in the range(INT64MAX, UINT64MAX) incorrectly
+
+**Other changes**
+
+- Inlining now no longer adds redundant ``Identity`` nodes and supports subgraphs, thanks to reimplementing the ONNX renaming routine.
+
+
+0.8.1 (2023-05-xx)
+------------------
+
+**Bug fixes**
+
+- An explicit error is now raised when local subgraph arguments are leaked to an outer scope. This may happen when the subgraph callback uses side effects saving local variables, which would produce later a confusing error message.
+
 0.8.0 (2023-05-11)
 ------------------
 
 This version is intended as a release candidate for ``1.0.0``.
 
 **New feature**
 
@@ -29,15 +53,15 @@
 
 **New features**
 
 - The opset ``ai.onnx@18`` is now shipped with Spox (version 18 of the default domain, as introduced in ONNX 1.13). To avoid code duplication, unchanged implementations are 'inherited' from the previous version.
 
 **Breaking changes**
 
-- The typing rules of the (previously partially documented) extra constructor ``const`` have changed. Its signature is now ``const(npt.ArrayLike, npt.DTypeLike = None) -> Var``. In particular, ``const`` of a Python ``float`` no longer becomes ``float32``, but ``float64`` like numpy - this is a **breaking change**. The operator is redefined to be equivalent to ``constant(numpy.array(value), dtype)``, instead of a complex set of cases like before. 
+- The typing rules of the (previously partially documented) extra constructor ``const`` have changed. Its signature is now ``const(npt.ArrayLike, npt.DTypeLike = None) -> Var``. In particular, ``const`` of a Python ``float`` no longer becomes ``float32``, but ``float64`` like numpy - this is a **breaking change**. The operator is redefined to be equivalent to ``constant(numpy.array(value), dtype)``, instead of a complex set of cases like before.
 - The ``Type <= Type`` (``Type.__le__``) overload is now removed.
 - Deprecated operator constructors are now no longer generated after the version their schema was deprecated. Effectively, this means ``ai.onnx@17::Scatter`` and ``ai.onnx@17::Upsample`` (available as ``op.scatter`` and ``op.upsample``) are no longer available in ``spox.opset.ai.onnx.v17``. They likely were not used in practice as attempting to build deprecated operators has always failed.
 
 **Bug fixes**
 
 - The operator constructor ``cum_sum`` now also has an alias ``cumsum``, to mirror ``numpy``. This alias should be preferred.
```

### Comparing `spox-0.8.0/LICENSE` & `spox-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/PKG-INFO` & `spox-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spox
-Version: 0.8.0
+Version: 0.9.0
 Summary: A framework for constructing ONNX computational graphs.
 Author-email: Jakub Bachurski <kbachurski@gmail.com>, Christian Bourjau <christian.bourjau@quantco.com>
 Maintainer-email: Jakub Bachurski <kbachurski@gmail.com>, Christian Bourjau <christian.bourjau@quantco.com>
 Project-URL: Source, https://github.com/quantco/spox
 Keywords: machine-learning,onnx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `spox-0.8.0/README.md` & `spox-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/docs/Makefile` & `spox-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/docs/conf.py` & `spox-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/docs/guides/advanced.ipynb` & `spox-0.9.0/docs/guides/advanced.ipynb`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/docs/guides/converter.ipynb` & `spox-0.9.0/docs/guides/converter.ipynb`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/docs/guides/example-model-netron.png` & `spox-0.9.0/docs/guides/example-model-netron.png`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/docs/guides/inference.ipynb` & `spox-0.9.0/docs/guides/inference.ipynb`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/docs/guides/inline.ipynb` & `spox-0.9.0/docs/guides/inline.ipynb`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/docs/guides/tutorial.ipynb` & `spox-0.9.0/docs/guides/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/docs/index.rst` & `spox-0.9.0/docs/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 .. toctree::
    :maxdepth: 1
    :caption: API Listing
 
    API Reference <api/modules>
    Operator constructors for the ai.onnx domain version 17 <api/spox.opset.ai.onnx.v17>
    Operator constructors for the ai.onnx domain version 18 <api/spox.opset.ai.onnx.v18>
+   Operator constructors for the ai.onnx domain version 19 <api/spox.opset.ai.onnx.v19>
    Operator constructors for the ai.onnx.ml domain version 3 <api/spox.opset.ai.onnx.ml.v3>
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
```

### Comparing `spox-0.8.0/docs/make.bat` & `spox-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/docs/manual/operators.rst` & `spox-0.9.0/docs/manual/operators.rst`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/docs/manual/overview.rst` & `spox-0.9.0/docs/manual/overview.rst`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/docs/manual/unstable.rst` & `spox-0.9.0/docs/manual/unstable.rst`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/pyproject.toml` & `spox-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_adapt.py` & `spox-0.9.0/src/spox/_adapt.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_attributes.py` & `spox-0.9.0/src/spox/_attributes.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_build.py` & `spox-0.9.0/src/spox/_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,51 +250,66 @@
         )
         self.source_of[graph] = self.results_of[graph][0]._op
 
         # Resolving arguments is a bit more complicated and requires a traversal to find all & claimed arguments.
         # To avoid too many dictionary accesses, we create aliases for the relevant sets.
         all_arguments = self.all_arguments_in[graph] = set()
         claimed_arguments = self.claimed_arguments_in[graph] = set()
+        used_arguments = set()
 
         def collect_arguments(nd: Node):
-            nonlocal all_arguments, claimed_arguments
+            nonlocal all_arguments, claimed_arguments, used_arguments
             if isinstance(nd, Argument):
                 all_arguments.add(nd.outputs.arg)
+                used_arguments.add(nd.outputs.arg)
             for subgraph in nd.subgraphs:
                 all_arguments_sub, claimed_arguments_sub = self.discover(subgraph)
                 all_arguments |= all_arguments_sub
                 claimed_arguments |= claimed_arguments_sub
                 if subgraph not in self.scope_tree.subgraph_owner:
                     self.scope_tree.subgraph_owner[subgraph] = nd
                 if self.scope_tree.subgraph_owner[subgraph] != nd:
                     raise BuildError(
                         "Subgraph has multiple owners (the Graph instance was reused)."
                     )
 
+        # Here, we compute:
+        #  - all_arguments to be the set of all Argument instances found anywhere, including subgraphs
+        #  - claimed_arguments to be the arguments found anywhere that are already set as subgraph arguments.
+        #    This is modified afterwards to include arguments assigned to this graph.
+        #  - used_arguments to be arguments that are used directly in this graph, excluding subgraphs.
         iterative_dfs(
             [self.source_of[graph]],
             lambda nd: (a._op for a in nd.dependencies),
             collect_arguments,
         )
         self.graph_topo.append(graph)
 
         # Now we resolve which arguments we should get.
         if graph.requested_arguments is None:
-            # If there's no request, we take all arguments
+            # If there's no request, we take all arguments found anywhere in this graph
             self.arguments_of[graph] = list(all_arguments - claimed_arguments)
         else:
             # If there is a request, we may not have found it by traversal if an argument was unused.
             all_arguments |= set(graph.requested_arguments)
             self.arguments_of[graph] = list(graph.requested_arguments)
 
         if set(self.arguments_of[graph]) & claimed_arguments:
             raise BuildError(
                 "Some arguments that this graph claims were already claimed. "
                 "Did subgraphs share arguments they requested?"
             )
+        # If a claimed argument is used directly in the current graph,
+        # a subgraph-local Argument was leaked, which breaks the contract.
+        leaked = claimed_arguments & used_arguments
+        if leaked:
+            raise BuildError(
+                "Some subgraph-local arguments were leaked to an outer scope. "
+                "Hint: avoid side effects in your subgraph callbacks."
+            )
         claimed_arguments |= set(self.arguments_of[graph])
 
         return all_arguments, claimed_arguments
 
     def update_scope_tree(self, graph: "Graph") -> None:
         """
         Traverse ``graph`` and update the Builder's scope tree to accommodate the input constraints inside it.
```

### Comparing `spox-0.8.0/src/spox/_debug.py` & `spox-0.9.0/src/spox/_debug.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_exceptions.py` & `spox-0.9.0/src/spox/_exceptions.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_fields.py` & `spox-0.9.0/src/spox/_fields.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_function.py` & `spox-0.9.0/src/spox/_function.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_future.py` & `spox-0.9.0/src/spox/_future.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_graph.py` & `spox-0.9.0/src/spox/_graph.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_internal_op.py` & `spox-0.9.0/src/spox/_internal_op.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_node.py` & `spox-0.9.0/src/spox/_node.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_public.py` & `spox-0.9.0/src/spox/_public.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module implementing the main public interface functions in Spox."""
 
 import contextlib
 import itertools
-from typing import Dict, Optional, Protocol
+from typing import Dict, List, Optional, Protocol
 
 import numpy as np
 import onnx
 from onnx.numpy_helper import to_array
 
 from . import _internal_op
 from ._attributes import AttrType
@@ -214,36 +214,50 @@
     in_names = [i.name for i in model.graph.input]
     in_defaults = {i.name: i for i in model.graph.initializer}
     out_names = [o.name for o in model.graph.output]
     _defaults_msg = f" (defaults {list(in_defaults.keys())})"
     _signature_msg = f"signature {in_names}{_defaults_msg} -> {out_names}"
 
     model = _copy_model(model)
-    # FIXME: Renaming does not work on subgraphs as of ONNX 1.13/1.14.
-    for node in model.graph.node:
-        for attr in node.attribute:
-            if attr.HasField("g") or attr.graphs:
-                raise ValueError(
-                    "Inlining models with subgraphs is not supported due to "
-                    "lack of upstream support for renaming values in subgraphs."
-                )
     # FIXME: Support for functions is a bit involved, as it interacts with build.
     if model.functions:
         raise ValueError(
             "Inlining models with functions is not supported. "
             "Consider removing or inlining the function definitions "
             "(if that preserves the model validity)."
         )
     # Handling symbolic dimensions is difficult and not particularly useful, so strip them
     for info in itertools.chain(
         model.graph.input, model.graph.output, model.graph.value_info
     ):
         info.type.CopyFrom(
             _strip_dim_symbol(Type._from_onnx(info.type), lambda x: True)._to_onnx()
         )
+    # We handle everything related to initializers here, as currently build does not support them too well
+    # Overridable initializers are saved to in_defaults, non-overridable replaced with Constant
+    preamble: List[onnx.NodeProto] = []
+    input_names = {i.name for i in model.graph.input}
+    preamble.extend(
+        onnx.helper.make_node("Constant", [], [i.name], value=i)
+        for i in model.graph.initializer
+        if i.name not in input_names
+    )
+    preamble.extend(
+        onnx.helper.make_node("Constant", [], [i.values.name], sparse_value=i)
+        for i in model.graph.sparse_initializer
+        if i.values.name not in input_names
+    )
+    del model.graph.initializer[:]
+    del model.graph.sparse_initializer[:]
+    # The API on the protobuf list is a bit limited
+    # - this prepends the preamble before the rest of the nodes
+    model.graph.node.reverse()
+    model.graph.node.extend(reversed(preamble))
+    model.graph.node.reverse()
+    # Now we can assume the graph has no initializers
 
     def inline_inner(*args: Var, **kwargs: Var) -> Dict[str, Var]:
         for name, arg in zip(in_names, args):
             if name in kwargs:
                 raise TypeError(
                     f"inline callback got multiple values for argument '{name}', {_signature_msg}."
                 )
```

### Comparing `spox-0.8.0/src/spox/_schemas.py` & `spox-0.9.0/src/spox/_schemas.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_scope.py` & `spox-0.9.0/src/spox/_scope.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Generic, Hashable, Optional, TypeVar, Union, overload
+from typing import Dict, Generic, Hashable, Optional, Set, TypeVar, Union, overload
 
 from ._node import Node
 from ._var import Var
 
 H = TypeVar("H", bound=Hashable)
 
 
@@ -18,40 +18,46 @@
 
     Methods (and operators) on the namespace work both ways: both with names (str) and the named type (H).
     So ``__getitem__`` (``ScopeSpace[item]``) may be used for both the name of an object and the object of a name.
     """
 
     name_of: Dict[H, str]
     of_name: Dict[str, H]
+    reserved: Set[str]
     parent: "Optional[ScopeSpace[H]]"
 
     def __init__(
         self,
         name_of: Optional[Dict[H, str]] = None,
         of_name: Optional[Dict[str, H]] = None,
+        reserved: Optional[Set[str]] = None,
         parent: "Optional[ScopeSpace[H]]" = None,
     ):
         """
         Parameters
         ----------
         name_of
             Name of a given object in this namespace.
         of_name
             Object with a given name in this namespace.
+        reserved
+            Set of reserved names, taken up by anonymous objects.
         parent
-            Parent scope's namespace. Is accessed first before all checks, but is not modified directly.
+            Namespace of a parent scope. Is accessed first before all checks, but never modified.
         """
         self.name_of = name_of.copy() if name_of is not None else {}
         self.of_name = of_name.copy() if of_name is not None else {}
+        self.reserved = reserved.copy() if reserved is not None else set()
         self.parent = parent
 
     def __contains__(self, item: Union[str, H]) -> bool:
         """Checks if a given name or object is declared in this (or outer) namespace."""
         return (
             (self.parent is not None and item in self.parent)
+            or item in self.reserved
             or item in self.name_of
             or item in self.of_name
         )
 
     @overload
     def __getitem__(self, item: H) -> str:
         ...
@@ -121,14 +127,20 @@
 
     def maybe_enum(self, base: str, suffix: str = "_{}") -> str:
         """Attempt to use ``base`` as a name, or return the result of ``self.enum`` for it otherwise."""
         if base not in self:
             return base
         return self.enum(base, suffix)
 
+    def reserve(self, name: str) -> str:
+        if name in self:
+            raise ScopeError(f"Reserved name is already in use: {name}")
+        self.reserved.add(name)
+        return name
+
 
 class Scope:
     """
     Class representing the state of an ONNX-rules scope.
 
     Has namespaces (represented by a ScopeSpace) for Vars and Nodes.
     """
```

### Comparing `spox-0.8.0/src/spox/_shape.py` & `spox-0.9.0/src/spox/_shape.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_standard.py` & `spox-0.9.0/src/spox/_standard.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_traverse.py` & `spox-0.9.0/src/spox/_traverse.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_type_system.py` & `spox-0.9.0/src/spox/_type_system.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_utils.py` & `spox-0.9.0/src/spox/_utils.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/_value_prop.py` & `spox-0.9.0/src/spox/_value_prop.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 - numpy.ndarray -> Tensor
 - list[PropValue] -> Sequence
 - PropValue -> Optional, Some (has value)
 - None -> Optional, Nothing (no value)
 """
 PropValueType = Union[numpy.ndarray, List["PropValue"], "PropValue", None]
 ORTValue = Union[numpy.ndarray, list, None]
-RefValue = Union[numpy.ndarray, list, float]
+RefValue = Union[numpy.ndarray, list, float, None]
 
 VALUE_PROP_STRICT_CHECK: bool = False
 
 
 class ValuePropBackend(enum.Enum):
     NONE = 0
     REFERENCE = 1
@@ -47,14 +47,26 @@
     - Reference implementations (Ref).
     """
 
     type: Type
     value: PropValueType
 
     def __post_init__(self):
+        # The underlying numpy array might have been constructed with a
+        # platform-dependent dtype - such as ulonglong.
+        # Though very similar, it does not compare equal to the usual sized dtype.
+        # (for example ulonglong is not uint64)
+        if isinstance(self.value, numpy.ndarray) and numpy.issubdtype(
+            self.value.dtype, numpy.number
+        ):
+            # We normalize by reconstructing the dtype through its name
+            object.__setattr__(
+                self, "value", self.value.astype(numpy.dtype(self.value.dtype.name))
+            )
+
         if VALUE_PROP_STRICT_CHECK and not self.check():
             raise ValueError(
                 f"Attempt to construct PropValue of {self.value}, "
                 f"which does not match the expected type {self.type}."
             )
 
     def __str__(self):
@@ -107,23 +119,22 @@
         elif isinstance(typ, Optional):  # Optional, Some
             return cls(typ, cls.from_ort_value(typ.elem_type, value))
         elif isinstance(value, list):  # Sequence
             elem_type = typ.unwrap_sequence().elem_type
             return cls(typ, [cls.from_ort_value(elem_type, elem) for elem in value])
         elif isinstance(value, numpy.ndarray):  # Tensor
             # Normalise the dtype in case we got an alias (like longlong)
-            value = value.astype(numpy.dtype(value.dtype.name))
             if value.dtype == numpy.dtype(object):
                 value = value.astype(str)
             return cls(typ, value)
         raise TypeError(f"No handler for ORT value: {value}")
 
     def to_ref_value(self) -> RefValue:
         if self.value is None:  # Optional, Nothing
-            return [None]  # Optionals are wrapped in a singleton list
+            return None  # Optionals are wrapped in a singleton list
         elif isinstance(self.value, PropValue):  # Optional, Some
             return [self.value.to_ref_value()]
         elif isinstance(self.value, list):  # Sequence
             return [elem.to_ref_value() for elem in self.value]
         else:  # Tensor
             return self.value
```

### Comparing `spox-0.8.0/src/spox/_var.py` & `spox-0.9.0/src/spox/_var.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/src/spox/opset/ai/onnx/ml/v3.py` & `spox-0.9.0/src/spox/opset/ai/onnx/ml/v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -816,19 +816,19 @@
     cats_strings
         Attribute.
         The strings of the map. This sequence must be the same length as the
         'cats_int64s' sequence
     default_int64
         Attribute.
         An integer to use when an input string value is not found in the map.One
-        and only one of the 'default_*' attributes must be defined.
+        and only one of the 'default\_\*' attributes must be defined.
     default_string
         Attribute.
         A string to use when an input integer value is not found in the map.One
-        and only one of the 'default_*' attributes must be defined.
+        and only one of the 'default\_\*' attributes must be defined.
 
     Returns
     =======
     Y : Var
         Type T2.
         Output data. If strings are input, the output values are integers, and
         vice versa.
@@ -975,16 +975,16 @@
     imputed_value_floats or imputed_value_int64s should be defined -- floats
     if the input tensor holds floats, integers if the input tensor holds
     integers. The imputed values must all fit within the width of the tensor
     element type. One and only one of the replaced_value_float or
     replaced_value_int64 should be defined, which one depends on whether
     floats or integers are being processed. The imputed_value attribute
     length can be 1 element, or it can have one element per input feature.In
-    other words, if the input tensor has the shape [*,F], then the length of
-    the attribute array may be 1 or F. If it is 1, then it is broadcast
+    other words, if the input tensor has the shape [\*,F], then the length
+    of the attribute array may be 1 or F. If it is 1, then it is broadcast
     along the last dimension and applied to each feature.
 
     Parameters
     ==========
     X
         Type T.
         Data to be processed.
@@ -1078,24 +1078,24 @@
         Attribute.
         A list of floats.
     keys_int64s
         Attribute.
         A list of ints.
     keys_strings
         Attribute.
-        A list of strings. One and only one of 'keys_*'s should be set.
+        A list of strings. One and only one of 'keys\_\*'s should be set.
     values_floats
         Attribute.
         A list of floats.
     values_int64s
         Attribute.
         A list of ints.
     values_strings
         Attribute.
-        A list of strings. One and only one of 'value_*'s should be set.
+        A list of strings. One and only one of 'value\_\*'s should be set.
 
     Returns
     =======
     Y : Var
         Type T2.
         Output data.
 
@@ -1326,20 +1326,20 @@
     Parameters
     ==========
     X
         Type T.
         Data to be encoded.
     cats_int64s
         Attribute.
-        List of categories, ints.One and only one of the 'cats_*' attributes
+        List of categories, ints.One and only one of the 'cats\_\*' attributes
         must be defined.
     cats_strings
         Attribute.
-        List of categories, strings.One and only one of the 'cats_*' attributes
-        must be defined.
+        List of categories, strings.One and only one of the 'cats\_\*'
+        attributes must be defined.
     zeros
         Attribute.
         If true and category is not present, will return all zeros; if false and
         a category if not found, the operator will fail.
 
     Returns
     =======
@@ -1388,19 +1388,19 @@
     ==========
     X
         Type T1.
         Data to be classified.
     classlabels_ints
         Attribute.
         Class labels if using integer labels.One and only one of the
-        'classlabels_*' attributes must be defined.
+        'classlabels\_\*' attributes must be defined.
     classlabels_strings
         Attribute.
         Class labels if using string labels.One and only one of the
-        'classlabels_*' attributes must be defined.
+        'classlabels\_\*' attributes must be defined.
     coefficients
         Attribute.
 
     kernel_params
         Attribute.
         List of 3 elements containing gamma, coef0, and degree, in that order.
         Zero if unused for the kernel.
@@ -1621,15 +1621,15 @@
     nodes_values_as_tensor: Optional[np.ndarray] = None,
     post_transform: str = "NONE",
 ) -> Tuple[Var, Var]:
     r"""
     Tree Ensemble classifier. Returns the top class for each of N inputs.
     The attributes named 'nodes_X' form a sequence of tuples, associated by
     index into the sequences, which must all be of equal length. These
-    tuples define the nodes. Similarly, all fields prefixed with 'class_'
+    tuples define the nodes. Similarly, all fields prefixed with 'class\_'
     are tuples of votes at the leaves. A leaf may have multiple votes, where
     each vote is weighted by the associated class_weights index. One and
     only one of classlabels_strings or classlabels_int64s will be defined.
     The class_ids are indices into this list. All fields ending with
     \_as_tensor can be used instead of the same parameter without the suffix
     if the element type is double and not float.
 
@@ -1660,19 +1660,19 @@
         The weight for the class in class_id.
     class_weights_as_tensor
         Attribute.
         The weight for the class in class_id.
     classlabels_int64s
         Attribute.
         Class labels if using integer labels.One and only one of the
-        'classlabels_*' attributes must be defined.
+        'classlabels\_\*' attributes must be defined.
     classlabels_strings
         Attribute.
         Class labels if using string labels.One and only one of the
-        'classlabels_*' attributes must be defined.
+        'classlabels\_\*' attributes must be defined.
     nodes_falsenodeids
         Attribute.
         Child node if expression is false.
     nodes_featureids
         Attribute.
         Feature id for each node.
     nodes_hitrates
@@ -1940,20 +1940,20 @@
     Parameters
     ==========
     X
         Type tensor(float).
         The input values
     classlabels_int64s
         Attribute.
-        The keys when using int keys.One and only one of the 'classlabels_*'
+        The keys when using int keys.One and only one of the 'classlabels\_\*'
         attributes must be defined.
     classlabels_strings
         Attribute.
-        The keys when using string keys.One and only one of the 'classlabels_*'
-        attributes must be defined.
+        The keys when using string keys.One and only one of the
+        'classlabels\_\*' attributes must be defined.
 
     Returns
     =======
     Z : Var
         Type T.
         The output map
```

### Comparing `spox-0.8.0/src/spox/opset/ai/onnx/v17.py` & `spox-0.9.0/src/spox/opset/ai/onnx/v17.py`

 * *Files 2% similar despite different names*

```diff
@@ -4405,41 +4405,41 @@
     lengths. average pooling consisting of computing the average on all
     values of a subset of the input tensor according to the kernel size and
     downsampling the data into the output tensor Y for further processing.
     The output spatial shape will be following:
 
     ::
 
-       output_spatial_shape[i] = floor((input_spatial_shape[i] + pad_shape[i] - kernel_spatial_shape[i]) / strides_spatial_shape[i] + 1)
+       output_spatial_shape[i] = floor((input_spatial_shape[i] + pad_shape[i] - ((kernel_spatial_shape[i] - 1) * dilations[i] + 1)) / strides_spatial_shape[i] + 1)
 
     or
 
     ::
 
-       output_spatial_shape[i] = ceil((input_spatial_shape[i] + pad_shape[i] - kernel_spatial_shape[i]) / strides_spatial_shape[i] + 1)
+       output_spatial_shape[i] = ceil((input_spatial_shape[i] + pad_shape[i] - ((kernel_spatial_shape[i] - 1) * dilations[i] + 1)) / strides_spatial_shape[i] + 1)
 
     if ceil_mode is enabled
 
     ::
 
        * pad_shape[i] is sum of pads along axis i
 
     ``auto_pad`` is a DEPRECATED attribute. If you are using them currently,
     the output spatial shape will be following:
 
     ::
 
-       VALID: output_spatial_shape[i] = ceil((input_spatial_shape[i] - kernel_spatial_shape[i] + 1) / strides_spatial_shape[i])
+       VALID: output_spatial_shape[i] = ceil((input_spatial_shape[i] - ((kernel_spatial_shape[i] - 1) * dilations[i] + 1) + 1) / strides_spatial_shape[i])
        SAME_UPPER or SAME_LOWER: output_spatial_shape[i] = ceil(input_spatial_shape[i] / strides_spatial_shape[i])
 
     And pad shape will be following if ``SAME_UPPER`` or ``SAME_LOWER``:
 
     ::
 
-       pad_shape[i] = (output_spatial_shape[i] - 1) * strides_spatial_shape[i] + kernel_spatial_shape[i] - input_spatial_shape[i]
+       pad_shape[i] = (output_spatial_shape[i] - 1) * strides_spatial_shape[i] + ((kernel_spatial_shape[i] - 1) * dilations[i] + 1) - input_spatial_shape[i]
 
     The output of each pooling window is divided by the number of elements
     (exclude pad when attribute count_include_pad is zero).
 
     Parameters
     ==========
     X
@@ -4535,35 +4535,37 @@
     There are five required inputs 'X', 'scale', 'B', 'input_mean' and
     'input_var'. Note that 'input_mean' and 'input_var' are expected to be
     the estimated statistics in inference mode (training_mode=False,
     default), and the running statistics in training mode
     (training_mode=True). There are multiple cases for the number of
     outputs, which we list below:
 
-    Output case #1: Y, running_mean, running_var (training_mode=True) Output
-    case #2: Y (training_mode=False)
+    -  Output case #1: Y, running_mean, running_var (training_mode=True)
+    -  Output case #2: Y (training_mode=False)
 
     When training_mode=False, extra outputs are invalid. The outputs are
     updated as follows when training_mode=True:
 
     ::
 
        running_mean = input_mean * momentum + current_mean * (1 - momentum)
        running_var = input_var * momentum + current_var * (1 - momentum)
 
        Y = (X - current_mean) / sqrt(current_var + epsilon) * scale + B
 
-       where:
+    where:
+
+    ::
 
        current_mean = ReduceMean(X, axis=all_except_channel_index)
        current_var =  ReduceVar(X, axis=all_except_channel_index)
 
-       Notice that ReduceVar refers to the population variance, and it equals to
-       sum(sqrd(x_i - x_avg)) / N
-       where N is the population size (this formula does not use sample size N - 1).
+    Notice that ``ReduceVar`` refers to the population variance, and it
+    equals to ``sum(sqrd(x_i - x_avg)) / N`` where ``N`` is the population
+    size (this formula does not use sample size ``N - 1``).
 
     The computation of ReduceMean and ReduceVar uses float to avoid overflow
     for float16 inputs.
 
     When training_mode=False:
 
     ::
@@ -4831,16 +4833,16 @@
     specified by the 'to' argument and returns an output tensor of the same
     size in the converted type. The 'to' argument must be one of the data
     types specified in the 'DataType' enum field in the TensorProto message.
 
     Casting from string tensor in plain (e.g., "3.14" and "1000") and
     scientific numeric representations (e.g., "1e-5" and "1E8") to float
     types is supported. For example, converting string "100.5" to an integer
-    may result 100. There are some string literals reserved for special
-    floating-point values; "+INF" (and "INF"), "-INF", and "NaN" are
+    may yield result 100. There are some string literals reserved for
+    special floating-point values; "+INF" (and "INF"), "-INF", and "NaN" are
     positive infinity, negative infinity, and not-a-number, respectively.
     Any string which can exactly match "+INF" in a case-insensitive way
     would be mapped to positive infinite. Similarly, this case-insensitive
     rule is applied to "INF" and "NaN". When casting from numeric tensors to
     string tensors, plain floating-point representation (such as
     "314.15926") would be used. Converting non-numerical-literal string such
     as "Hello World!" is an undefined behavior. Cases of converting string
@@ -4958,15 +4960,16 @@
 
 def ceil(
     X: Var,
 ) -> Var:
     r"""
     Ceil takes one input data (Tensor<T>) and produces one output data
     (Tensor<T>) where the ceil is, y = ceil(x), is applied to the tensor
-    elementwise.
+    elementwise. If x is integral, +0, -0, NaN, or infinite, x itself is
+    returned.
 
     Parameters
     ==========
     X
         Type T.
         Input tensor
 
@@ -5245,15 +5248,15 @@
     value_int: Optional[int] = None,
     value_ints: Optional[Iterable[int]] = None,
     value_string: Optional[str] = None,
     value_strings: Optional[Iterable[str]] = None,
 ) -> Var:
     r"""
     This operator produces a constant tensor. Exactly one of the provided
-    attributes, either value, sparse_value, or value_\* must be specified.
+    attributes, either value, sparse_value, or value\_\* must be specified.
 
     Parameters
     ==========
     sparse_value
         Attribute.
         The value for the elements of the output tensor in sparse format.
     value
@@ -5917,32 +5920,32 @@
         Attribute.
         Whether to perform the inverse discrete fourier transform. By default
         this value is set to 0, which corresponds to false.
     onesided
         Attribute.
         If onesided is 1, only values for w in [0, 1, 2, ..., floor(n_fft/2) +
         1] are returned because the real-to-complex Fourier transform satisfies
-        the conjugate symmetry, i.e., X[m, w] = X[m,w]=X[m,n_fft-w]*. Note if
+        the conjugate symmetry, i.e., X[m, w] = X[m,w]=X[m,n_fft-w]\*. Note if
         the input or window tensors are complex, then onesided output is not
         possible. Enabling onesided with real inputs performs a Real-valued fast
         Fourier transform (RFFT). When invoked with real or complex valued
         input, the default value is 0. Values can be 0 or 1.
 
     Returns
     =======
     output : Var
         Type T1.
         The Fourier Transform of the input vector.If onesided is 0, the
         following shape is expected:
-        [batch_idx][signal_dim1][signal_dim2]...[signal_dimN][2]. If axis=0 and
+        [batch_idx][signal_dim1][signal_dim2]...[signal_dimN][2]. If axis=1 and
         onesided is 1, the following shape is expected:
         [batch_idx][floor(signal_dim1/2)+1][signal_dim2]...[signal_dimN][2]. If
-        axis=1 and onesided is 1, the following shape is expected:
+        axis=2 and onesided is 1, the following shape is expected:
         [batch_idx][signal_dim1][floor(signal_dim2/2)+1]...[signal_dimN][2]. If
-        axis=N-1 and onesided is 1, the following shape is expected:
+        axis=N and onesided is 1, the following shape is expected:
         [batch_idx][signal_dim1][signal_dim2]...[floor(signal_dimN/2)+1][2]. The
         signal_dim at the specified axis is equal to the dft_length.
 
     Notes
     =====
     Signature: ``ai.onnx@17::DFT``.
 
@@ -5975,37 +5978,31 @@
     specifically, this op outputs a copy of the input tensor where values
     from the depth dimension are moved in spatial blocks to the height and
     width dimensions. By default, ``mode`` = ``DCR``. In the DCR mode,
     elements along the depth dimension from the input tensor are rearranged
     in the following order: depth, column, and then row. The output y is
     computed from the input x as below:
 
-    b, c, h, w = x.shape
-
-    tmp = np.reshape(x, [b, blocksize, blocksize, c // (blocksize**2), h,
-    w])
-
-    tmp = np.transpose(tmp, [0, 3, 4, 1, 5, 2])
+    ::
 
-    y = np.reshape(tmp, [b, c // (blocksize**2), h \* blocksize, w \*
-    blocksize])
+       b, c, h, w = x.shape
+       tmp = np.reshape(x, [b, blocksize, blocksize, c // (blocksize**2), h, w])
+       tmp = np.transpose(tmp, [0, 3, 4, 1, 5, 2])
+       y = np.reshape(tmp, [b, c // (blocksize**2), h * blocksize, w * blocksize])
 
     In the CRD mode, elements along the depth dimension from the input
     tensor are rearranged in the following order: column, row, and the
     depth. The output y is computed from the input x as below:
 
-    b, c, h, w = x.shape
-
-    tmp = np.reshape(x, [b, c // (blocksize \*\* 2), blocksize, blocksize,
-    h, w])
-
-    tmp = np.transpose(tmp, [0, 1, 4, 2, 5, 3])
+    ::
 
-    y = np.reshape(tmp, [b, c // (blocksize \*\* 2), h \* blocksize, w \*
-    blocksize])
+       b, c, h, w = x.shape
+       tmp = np.reshape(x, [b, c // (blocksize ** 2), blocksize, blocksize, h, w])
+       tmp = np.transpose(tmp, [0, 1, 4, 2, 5, 3])
+       y = np.reshape(tmp, [b, c // (blocksize ** 2), h * blocksize, w * blocksize])
 
     Parameters
     ==========
     input
         Type T.
         Input tensor of [N,C,H,W], where N is the batch axis, C is the channel
         or depth, H is the height and W is the width.
@@ -6048,20 +6045,20 @@
     x_zero_point: Optional[Var] = None,
     *,
     axis: int = 1,
 ) -> Var:
     r"""
     The linear dequantization operator. It consumes a quantized tensor, a
     scale, and a zero point to compute the full precision tensor. The
-    dequantization formula is y = (x - x_zero_point) \* x_scale. 'x_scale'
-    and 'x_zero_point' must have same shape, and can be either a scalar for
-    per-tensor / per layer quantization, or a 1-D tensor for per-axis
-    quantization. 'x_zero_point' and 'x' must have same type. 'x' and 'y'
-    must have same shape. In the case of dequantizing int32, there's no zero
-    point (zero point is supposed to be 0).
+    dequantization formula is ``y = (x - x_zero_point) * x_scale``.
+    ``x_scale`` and ``x_zero_point`` must have same shape, and can be either
+    a scalar for per-tensor / per layer quantization, or a 1-D tensor for
+    per-axis quantization. ``x_zero_point`` and ``x`` must have same type.
+    ``x`` and ``y`` must have same shape. In the case of dequantizing int32,
+    there's no zero point (zero point is supposed to be 0).
 
     Parameters
     ==========
     x
         Type T.
         N-D quantized input tensor to be de-quantized.
     x_scale
@@ -6282,35 +6279,42 @@
     r"""
     A Function to fuse calculation for Scale, Zero Point and FP32->8Bit
     convertion of FP32 Input data. Outputs Scale, ZeroPoint and Quantized
     Input for a given FP32 Input. Scale is calculated as:
 
     ::
 
-        y_scale = (max(x) - min(x))/(qmax - qmin)
-        * where qmax and qmin are max and min values for quantization range .i.e [0, 255] in case of uint8
-        * data range is adjusted to include 0.
+       y_scale = (max(x) - min(x))/(qmax - qmin)
+
+    -  where qmax and qmin are max and min values for quantization range
+       .i.e [0, 255] in case of uint8
+    -  data range is adjusted to include 0.
 
     Zero point is calculated as:
 
     ::
 
        intermediate_zero_point = qmin - min(x)/y_scale
        y_zero_point = cast(round(saturate(itermediate_zero_point)))
-       * where qmax and qmin are max and min values for quantization range .i.e [0, 255] in case of uint8
-       * for saturation, it saturates to [0, 255] if it's uint8, or [-127, 127] if it's int8. Right now only uint8 is supported.
-       * rounding to nearest ties to even.
+
+    -  where qmax and qmin are max and min values for quantization range
+       .i.e [0, 255] in case of uint8
+    -  for saturation, it saturates to [0, 255] if it's uint8, or [-127,
+       127] if it's int8. Right now only uint8 is supported.
+    -  rounding to nearest ties to even.
 
     Data quantization formula is:
 
     ::
 
        y = saturate (round (x / y_scale) + y_zero_point)
-       * for saturation, it saturates to [0, 255] if it's uint8, or [-127, 127] if it's int8. Right now only uint8 is supported.
-       * rounding to nearest ties to even.
+
+    -  for saturation, it saturates to [0, 255] if it's uint8, or [-127,
+       127] if it's int8. Right now only uint8 is supported.
+    -  rounding to nearest ties to even.
 
     Parameters
     ==========
     x
         Type T1.
         Input tensor
 
@@ -6349,15 +6353,17 @@
     *,
     equation: str,
 ) -> Var:
     r"""
     An einsum of the form ``term1, term2 -> output-term`` produces an output
     tensor using the following equation
 
-    ``output[output-term] = reduce-sum( input1[term1] * input2[term] )``
+    ::
+
+       output[output-term] = reduce-sum( input1[term1] * input2[term] )
 
     where the reduce-sum performs a summation over all the indices occurring
     in the input terms (term1, term2) that do not occur in the output-term.
 
     The Einsum operator evaluates algebraic tensor operations on a sequence
     of tensors, using the Einstein summation convention. The equation string
     contains a comma-separated sequence of lower case letters. Each term
@@ -6679,15 +6685,15 @@
     input: Var,
     *,
     axis: int = 1,
 ) -> Var:
     r"""
     Flattens the input tensor into a 2D matrix. If input tensor has shape
     (d_0, d_1, ... d_n) then the output will have shape (d_0 X d_1 ...
-    d_(axis-1), d_axis X d_(axis+1) ... X dn).
+    d\_(axis-1), d_axis X d\_(axis+1) ... X dn).
 
     Parameters
     ==========
     input
         Type T.
         A tensor of rank >= axis.
     axis
@@ -6726,15 +6732,16 @@
 
 def floor(
     X: Var,
 ) -> Var:
     r"""
     Floor takes one input data (Tensor<T>) and produces one output data
     (Tensor<T>) where the floor is, y = floor(x), is applied to the tensor
-    elementwise.
+    elementwise. If x is integral, +0, -0, NaN, or infinite, x itself is
+    returned.
 
     Parameters
     ==========
     X
         Type T.
         Input tensor
 
@@ -6778,88 +6785,61 @@
 ) -> Tuple[Var, Var]:
     r"""
     Computes an one-layer GRU. This operator is usually supported via some
     custom implementation such as CuDNN.
 
     Notations:
 
-    ``X`` - input tensor
-
-    ``z`` - update gate
-
-    ``r`` - reset gate
-
-    ``h`` - hidden gate
-
-    ``t`` - time step (t-1 means previous time step)
-
-    ``W[zrh]`` - W parameter weight matrix for update, reset, and hidden
-    gates
-
-    ``R[zrh]`` - R recurrence weight matrix for update, reset, and hidden
-    gates
-
-    ``Wb[zrh]`` - W bias vectors for update, reset, and hidden gates
-
-    ``Rb[zrh]`` - R bias vectors for update, reset, and hidden gates
-
-    ``WB[zrh]`` - W parameter weight matrix for backward update, reset, and
-    hidden gates
-
-    ``RB[zrh]`` - R recurrence weight matrix for backward update, reset, and
-    hidden gates
-
-    ``WBb[zrh]`` - W bias vectors for backward update, reset, and hidden
-    gates
-
-    ``RBb[zrh]`` - R bias vectors for backward update, reset, and hidden
-    gates
-
-    ``H`` - Hidden state
-
-    ``num_directions`` - 2 if direction == bidirectional else 1
+    -  ``X`` - input tensor
+    -  ``z`` - update gate
+    -  ``r`` - reset gate
+    -  ``h`` - hidden gate
+    -  ``t`` - time step (t-1 means previous time step)
+    -  ``W[zrh]`` - W parameter weight matrix for update, reset, and hidden
+       gates
+    -  ``R[zrh]`` - R recurrence weight matrix for update, reset, and hidden
+       gates
+    -  ``Wb[zrh]`` - W bias vectors for update, reset, and hidden gates
+    -  ``Rb[zrh]`` - R bias vectors for update, reset, and hidden gates
+    -  ``WB[zrh]`` - W parameter weight matrix for backward update, reset,
+       and hidden gates
+    -  ``RB[zrh]`` - R recurrence weight matrix for backward update, reset,
+       and hidden gates
+    -  ``WBb[zrh]`` - W bias vectors for backward update, reset, and hidden
+       gates
+    -  ``RBb[zrh]`` - R bias vectors for backward update, reset, and hidden
+       gates
+    -  ``H`` - Hidden state
+    -  ``num_directions`` - 2 if direction == bidirectional else 1
 
     Activation functions:
 
-    Relu(x) - max(0, x)
-
-    Tanh(x) - (1 - e^{-2x})/(1 + e^{-2x})
-
-    Sigmoid(x) - 1/(1 + e^{-x})
-
-    (NOTE: Below are optional)
-
-    Affine(x) - alpha*x + beta
-
-    LeakyRelu(x) - x if x >= 0 else alpha \* x
-
-    ThresholdedRelu(x) - x if x >= alpha else 0
-
-    ScaledTanh(x) - alpha\ *Tanh(beta*\ x)
-
-    HardSigmoid(x) - min(max(alpha*x + beta, 0), 1)
-
-    Elu(x) - x if x >= 0 else alpha*(e^x - 1)
-
-    Softsign(x) - x/(1 + \|x|)
-
-    Softplus(x) - log(1 + e^x)
+    -  Relu(x) - max(0, x)
+    -  Tanh(x) - (1 - e^{-2x})/(1 + e^{-2x})
+    -  Sigmoid(x) - 1/(1 + e^{-x})
+
+    NOTE: Below are optional
+
+    -  Affine(x) - alpha \* x + beta
+    -  LeakyRelu(x) - x if x >= 0 else alpha \* x
+    -  ThresholdedRelu(x) - x if x >= alpha else 0
+    -  ScaledTanh(x) - alpha \* Tanh(beta \* x)
+    -  HardSigmoid(x) - min(max(alpha \* x + beta, 0), 1)
+    -  Elu(x) - x if x >= 0 else alpha \* (e^x - 1)
+    -  Softsign(x) - x/(1 + \|x\|)
+    -  Softplus(x) - log(1 + e^x)
 
     Equations (Default: f=Sigmoid, g=Tanh):
 
     -  zt = f(Xt*(Wz^T) + Ht-1*(Rz^T) + Wbz + Rbz)
-
     -  rt = f(Xt*(Wr^T) + Ht-1*(Rr^T) + Wbr + Rbr)
-
     -  ht = g(Xt*(Wh^T) + (rt (.) Ht-1)*(Rh^T) + Rbh + Wbh) # default, when
        linear_before_reset = 0
-
     -  ht = g(Xt*(Wh^T) + (rt (.) (Ht-1*(Rh^T) + Rbh)) + Wbh) # when
        linear_before_reset != 0
-
     -  Ht = (1 - zt) (.) ht + zt (.) Ht-1 This operator has **optional**
        inputs/outputs. See `the
        doc <https://github.com/onnx/onnx/blob/main/docs/IR.md>`__ for more
        details about the representation of optional arguments. An empty
        string may be used in the place of an actual argument's name to
        indicate a missing argument. Trailing optional arguments (those not
        followed by an argument that is present) may also be simply omitted.
@@ -6988,62 +6968,58 @@
 ) -> Var:
     r"""
     Given ``data`` tensor of rank r >= 1, and ``indices`` tensor of rank q,
     gather entries of the axis dimension of ``data`` (by default outer-most
     one as axis=0) indexed by ``indices``, and concatenates them in an
     output tensor of rank q + (r - 1).
 
-    axis = 0 :
-
-    Let k = indices[i_{0}, ..., i_{q-1}] Then output[i_{0}, ..., i_{q-1},
-    j_{0}, ..., j_{r-2}] = input[k , j_{0}, ..., j_{r-2}]
+    If ``axis = 0``, let ``k = indices[i_{0}, ..., i_{q-1}]`` then
+    ``output[i_{0}, ..., i_{q-1}, j_{0}, ..., j_{r-2}] = input[k , j_{0}, ..., j_{r-2}]``:
 
     ::
 
-         data = [
-             [1.0, 1.2],
-             [2.3, 3.4],
-             [4.5, 5.7],
-         ]
-         indices = [
-             [0, 1],
-             [1, 2],
-         ]
-         output = [
-             [
-                 [1.0, 1.2],
-                 [2.3, 3.4],
-             ],
-             [
-                 [2.3, 3.4],
-                 [4.5, 5.7],
-             ],
-         ]
-
-    axis = 1 :
-
-    Let k = indices[i_{0}, ..., i_{q-1}] Then output[j_{0}, i_{0}, ...,
-    i_{q-1}, j_{1}, ..., j_{r-2}] = input[j_{0}, k, j_{1}, ..., j_{r-2}]
+       data = [
+           [1.0, 1.2],
+           [2.3, 3.4],
+           [4.5, 5.7],
+       ]
+       indices = [
+           [0, 1],
+           [1, 2],
+       ]
+       output = [
+           [
+               [1.0, 1.2],
+               [2.3, 3.4],
+           ],
+           [
+               [2.3, 3.4],
+               [4.5, 5.7],
+           ],
+       ]
+
+    If ``axis = 1``, let ``k = indices[i_{0}, ..., i_{q-1}]`` then
+    ``output[j_{0}, i_{0}, ..., i_{q-1}, j_{1}, ..., j_{r-2}] = input[j_{0}, k, j_{1}, ..., j_{r-2}]``:
 
     ::
 
-         data = [
-             [1.0, 1.2, 1.9],
-             [2.3, 3.4, 3.9],
-             [4.5, 5.7, 5.9],
-         ]
-         indices = [
-             [0, 2],
-         ]
-         axis = 1,
-         output = [
-                 [[1.0, 1.9]],
-                 [[2.3, 3.9]],
-                 [[4.5, 5.9]],
-         ]
+       data = [
+           [1.0, 1.2, 1.9],
+           [2.3, 3.4, 3.9],
+           [4.5, 5.7, 5.9],
+       ]
+       indices = [
+           [0, 2],
+       ]
+       axis = 1,
+       output = [
+               [[1.0, 1.9]],
+               [[2.3, 3.9]],
+               [[4.5, 5.9]],
+       ]
 
     Parameters
     ==========
     data
         Type T.
         Tensor of rank r >= 1.
     indices
@@ -7098,57 +7074,57 @@
     ``indices``.
 
     For instance, in the 3-D case (r = 3), the output produced is determined
     by the following equations:
 
     ::
 
-         out[i][j][k] = input[index[i][j][k]][j][k] if axis = 0,
-         out[i][j][k] = input[i][index[i][j][k]][k] if axis = 1,
-         out[i][j][k] = input[i][j][index[i][j][k]] if axis = 2,
+       out[i][j][k] = input[index[i][j][k]][j][k] if axis = 0,
+       out[i][j][k] = input[i][index[i][j][k]][k] if axis = 1,
+       out[i][j][k] = input[i][j][index[i][j][k]] if axis = 2,
 
     This operator is also the inverse of ScatterElements. It is similar to
     Torch's gather operation.
 
     Example 1:
 
     ::
 
-         data = [
-             [1, 2],
-             [3, 4],
-         ]
-         indices = [
-             [0, 0],
-             [1, 0],
-         ]
-         axis = 1
-         output = [
-             [1, 1],
-             [4, 3],
-         ]
+       data = [
+           [1, 2],
+           [3, 4],
+       ]
+       indices = [
+           [0, 0],
+           [1, 0],
+       ]
+       axis = 1
+       output = [
+           [1, 1],
+           [4, 3],
+       ]
 
     Example 2:
 
     ::
 
-         data = [
-             [1, 2, 3],
-             [4, 5, 6],
-             [7, 8, 9],
-         ]
-         indices = [
-             [1, 2, 0],
-             [2, 0, 0],
-         ]
-         axis = 0
-         output = [
-             [4, 8, 3],
-             [7, 2, 3],
-         ]
+       data = [
+           [1, 2, 3],
+           [4, 5, 6],
+           [7, 8, 9],
+       ]
+       indices = [
+           [1, 2, 0],
+           [2, 0, 0],
+       ]
+       axis = 0
+       output = [
+           [4, 8, 3],
+           [7, 2, 3],
+       ]
 
     Parameters
     ==========
     data
         Type T.
         Tensor of rank r >= 1.
     indices
@@ -7351,17 +7327,16 @@
     transA: int = 0,
     transB: int = 0,
 ) -> Var:
     r"""
     General Matrix multiplication:
     https://en.wikipedia.org/wiki/Basic_Linear_Algebra_Subprograms#Level_3
 
-    A' = transpose(A) if transA else A
-
-    B' = transpose(B) if transB else B
+    -  A' = transpose(A) if transA else A
+    -  B' = transpose(B) if transB else B
 
     Compute Y = alpha \* A' \* B' + beta \* C, where input tensor A has
     shape (M, K) or (K, M), input tensor B has shape (K, N) or (N, K), input
     tensor C is broadcastable to shape (M, N), and output tensor Y has shape
     (M, N). A will be transposed before doing the computation if attribute
     transA is non-zero, same for B and transB. This operator supports
     **unidirectional broadcasting** (tensor C should be unidirectional
@@ -8233,25 +8208,22 @@
     bias: float = 1.0,
     size: int,
 ) -> Var:
     r"""
     Local Response Normalization proposed in the `AlexNet
     paper <https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf>`__.
     It normalizes over local input regions. The local region is defined
-    across the channels. For an element X[n, c, d1, ..., dk] in a tensor of
-    shape (N x C x D1 x D2, ..., Dk), its region is {X[n, i, d1, ..., dk] \|
-    max(0, c - floor((size - 1) / 2)) <= i <= min(C - 1, c + ceil((size - 1)
-    / 2))}.
-
-    square_sum[n, c, d1, ..., dk] = sum(X[n, i, d1, ..., dk] ^ 2), where
-    max(0, c - floor((size - 1) / 2)) <= i <= min(C - 1, c + ceil((size - 1)
-    / 2)).
+    across the channels. For an element ``X[n, c, d1, ..., dk]`` in a tensor
+    of shape ``(N x C x D1 x D2, ..., Dk)``, its region is
+    ``{X[n, i, d1, ..., dk] | max(0, c - floor((size - 1) / 2)) <= i <= min(C - 1, c + ceil((size - 1) / 2))}``.
 
-    Y[n, c, d1, ..., dk] = X[n, c, d1, ..., dk] / (bias + alpha / size \*
-    square_sum[n, c, d1, ..., dk] ) ^ beta
+    ``square_sum[n, c, d1, ..., dk] = sum(X[n, i, d1, ..., dk] ^ 2)``, where
+    ``max(0, c - floor((size - 1) / 2)) <= i <= min(C - 1, c + ceil((size - 1) / 2))``.
+
+    ``Y[n, c, d1, ..., dk] = X[n, c, d1, ..., dk] / (bias + alpha / size * square_sum[n, c, d1, ..., dk] ) ^ beta``
 
     Parameters
     ==========
     X
         Type T.
         Input data tensor from the previous operator; dimensions for image case
         are (N x C x H x W), where N is the batch size, C is the number of
@@ -8321,96 +8293,67 @@
 ) -> Tuple[Var, Var, Var]:
     r"""
     Computes an one-layer LSTM. This operator is usually supported via some
     custom implementation such as CuDNN.
 
     Notations:
 
-    ``X`` - input tensor
-
-    ``i`` - input gate
-
-    ``o`` - output gate
-
-    ``f`` - forget gate
-
-    ``c`` - cell gate
-
-    ``t`` - time step (t-1 means previous time step)
-
-    ``W[iofc]`` - W parameter weight matrix for input, output, forget, and
-    cell gates
-
-    ``R[iofc]`` - R recurrence weight matrix for input, output, forget, and
-    cell gates
-
-    ``Wb[iofc]`` - W bias vectors for input, output, forget, and cell gates
-
-    ``Rb[iofc]`` - R bias vectors for input, output, forget, and cell gates
-
-    ``P[iof]`` - P peephole weight vector for input, output, and forget
-    gates
-
-    ``WB[iofc]`` - W parameter weight matrix for backward input, output,
-    forget, and cell gates
-
-    ``RB[iofc]`` - R recurrence weight matrix for backward input, output,
-    forget, and cell gates
-
-    ``WBb[iofc]`` - W bias vectors for backward input, output, forget, and
-    cell gates
-
-    ``RBb[iofc]`` - R bias vectors for backward input, output, forget, and
-    cell gates
-
-    ``PB[iof]`` - P peephole weight vector for backward input, output, and
-    forget gates
-
-    ``H`` - Hidden state
-
-    ``num_directions`` - 2 if direction == bidirectional else 1
+    -  ``X`` - input tensor
+    -  ``i`` - input gate
+    -  ``o`` - output gate
+    -  ``f`` - forget gate
+    -  ``c`` - cell gate
+    -  ``t`` - time step (t-1 means previous time step)
+    -  ``W[iofc]`` - W parameter weight matrix for input, output, forget,
+       and cell gates
+    -  ``R[iofc]`` - R recurrence weight matrix for input, output, forget,
+       and cell gates
+    -  ``Wb[iofc]`` - W bias vectors for input, output, forget, and cell
+       gates
+    -  ``Rb[iofc]`` - R bias vectors for input, output, forget, and cell
+       gates
+    -  ``P[iof]`` - P peephole weight vector for input, output, and forget
+       gates
+    -  ``WB[iofc]`` - W parameter weight matrix for backward input, output,
+       forget, and cell gates
+    -  ``RB[iofc]`` - R recurrence weight matrix for backward input, output,
+       forget, and cell gates
+    -  ``WBb[iofc]`` - W bias vectors for backward input, output, forget,
+       and cell gates
+    -  ``RBb[iofc]`` - R bias vectors for backward input, output, forget,
+       and cell gates
+    -  ``PB[iof]`` - P peephole weight vector for backward input, output,
+       and forget gates
+    -  ``H`` - Hidden state
+    -  ``num_directions`` - 2 if direction == bidirectional else 1
 
     Activation functions:
 
-    Relu(x) - max(0, x)
-
-    Tanh(x) - (1 - e^{-2x})/(1 + e^{-2x})
-
-    Sigmoid(x) - 1/(1 + e^{-x})
-
-    (NOTE: Below are optional)
-
-    Affine(x) - alpha*x + beta
-
-    LeakyRelu(x) - x if x >= 0 else alpha \* x
-
-    ThresholdedRelu(x) - x if x >= alpha else 0
-
-    ScaledTanh(x) - alpha\ *Tanh(beta*\ x)
-
-    HardSigmoid(x) - min(max(alpha*x + beta, 0), 1)
-
-    Elu(x) - x if x >= 0 else alpha*(e^x - 1)
-
-    Softsign(x) - x/(1 + \|x|)
-
-    Softplus(x) - log(1 + e^x)
+    -  Relu(x) - max(0, x)
+    -  Tanh(x) - (1 - e^{-2x})/(1 + e^{-2x})
+    -  Sigmoid(x) - 1/(1 + e^{-x})
+
+    NOTE: Below are optional
+
+    -  Affine(x) - alpha*x + beta
+    -  LeakyRelu(x) - x if x >= 0 else alpha \* x
+    -  ThresholdedRelu(x) - x if x >= alpha else 0
+    -  ScaledTanh(x) - alpha\ *Tanh(beta*\ x)
+    -  HardSigmoid(x) - min(max(alpha*x + beta, 0), 1)
+    -  Elu(x) - x if x >= 0 else alpha*(e^x - 1)
+    -  Softsign(x) - x/(1 + \|x\|)
+    -  Softplus(x) - log(1 + e^x)
 
     Equations (Default: f=Sigmoid, g=Tanh, h=Tanh):
 
     -  it = f(Xt*(Wi^T) + Ht-1*(Ri^T) + Pi (.) Ct-1 + Wbi + Rbi)
-
     -  ft = f(Xt*(Wf^T) + Ht-1*(Rf^T) + Pf (.) Ct-1 + Wbf + Rbf)
-
     -  ct = g(Xt*(Wc^T) + Ht-1*(Rc^T) + Wbc + Rbc)
-
     -  Ct = ft (.) Ct-1 + it (.) ct
-
     -  ot = f(Xt*(Wo^T) + Ht-1*(Ro^T) + Po (.) Ct + Wbo + Rbo)
-
     -  Ht = ot (.) h(Ct) This operator has **optional** inputs/outputs. See
        `the doc <https://github.com/onnx/onnx/blob/main/docs/IR.md>`__ for
        more details about the representation of optional arguments. An empty
        string may be used in the place of an actual argument's name to
        indicate a missing argument. Trailing optional arguments (those not
        followed by an argument that is present) may also be simply omitted.
 
@@ -8647,18 +8590,14 @@
 ) -> Var:
     r"""
     LeakyRelu takes input data (Tensor<T>) and an argument alpha, and
     produces one output data (Tensor<T>) where the function
     ``f(x) = alpha * x for x < 0``, ``f(x) = x for x >= 0``, is applied to
     the data tensor elementwise.
 
-    **History**
-
-    -  Version 16 adds bfloat16 to the types allowed.
-
     Parameters
     ==========
     X
         Type T.
         Input tensor
     alpha
         Attribute.
@@ -8877,47 +8816,31 @@
        determines whether to run the first iteration and also a loop-carried
        dependency for the body graph. The body graph must yield a value for
        the condition variable, whether this input is provided or not.
 
     This table summarizes the operating modes of this operator with
     equivalent C-style code:
 
-    ::
+    Operator inputs defined as (max_trip_count, condition_var).
+
+    -  input ("", ""): for (int i=0; ; ++i) { cond = ... // Note this value
+       is ignored, but is required in the body }
 
-       Operator inputs defined as (max_trip_count, condition_var).
+    -  input ("", cond) // Note this is analogous to a while loop bool cond
+       = ...; for (int i=0; cond; ++i) { cond = ...; }
 
-       input ("", ""):
-           for (int i=0; ; ++i) {
-             cond = ... // Note this value is ignored, but is required in the body
-           }
-
-       input ("", cond) // Note this is analogous to a while loop
-           bool cond = ...;
-           for (int i=0; cond; ++i) {
-             cond = ...;
-           }
-
-       input ("", 1) // Note this is analogous to a do-while loop
-           bool cond = true
-           for (int i=0; cond; ++i) {
-             cond = ...;
-           }
-
-       input (trip_count, "") // Note this is analogous to a for loop
-           int trip_count = ...
-           for (int i=0; i < trip_count; ++i) {
-             cond = ...; // ignored
-           }
-
-       input (trip_count, cond)
-           int trip_count = ...;
-           bool cond = ...;
-           for (int i=0; i < trip_count && cond; ++i) {
-             cond = ...;
-           }
+    -  input ("", 1) // Note this is analogous to a do-while loop bool cond
+       = true for (int i=0; cond; ++i) { cond = ...; }
+
+    -  input (trip_count, "") // Note this is analogous to a for loop int
+       trip_count = ... for (int i=0; i < trip_count; ++i) { cond = ...; //
+       ignored }
+
+    -  input (trip_count, cond) int trip_count = ...; bool cond = ...; for
+       (int i=0; i < trip_count && cond; ++i) { cond = ...; }
 
     *Sample usage - cond as well as trip count*
 
     ::
 
        graph predict-net {
          %a = Constant[value = <Scalar Tensor [3]>]()
@@ -9362,19 +9285,16 @@
 
     or
 
     ::
 
        output_spatial_shape[i] = ceil((input_spatial_shape[i] + pad_shape[i] - ((kernel_spatial_shape[i] - 1) * dilations[i] + 1)) / strides_spatial_shape[i] + 1)
 
-    if ceil_mode is enabled
-
-    ::
-
-       * pad_shape[i] is sum of pads along axis i
+    if ceil_mode is enabled ``pad_shape[i]`` is the sum of pads along axis
+    ``i``.
 
     ``auto_pad`` is a DEPRECATED attribute. If you are using them currently,
     the output spatial shape will be following:
 
     ::
 
        VALID: output_spatial_shape[i] = ceil((input_spatial_shape[i] - ((kernel_spatial_shape[i] - 1) * dilations[i] + 1) + 1) / strides_spatial_shape[i])
@@ -9861,24 +9781,25 @@
     *,
     fmod: int = 0,
 ) -> Var:
     r"""
     Performs element-wise binary modulus (with Numpy-style broadcasting
     support). The sign of the remainder is the same as that of the Divisor.
 
-    ::
-
-       Mod operator can also behave like C fmod() or numpy.fmod. In this case, the sign of the remainder however, will be the same as the Dividend
-       (in contrast to integer mod). To force a behavior like numpy.fmod() an 'fmod' Attribute is provided.
-       This attribute is set to 0 by default causing the behavior to be like integer mod.
-       Setting this attribute to 1 causes the remainder to be calculated similar to that of numpy.fmod().
+    Mod operator can also behave like C fmod() or numpy.fmod. In this case,
+    the sign of the remainder however, will be the same as the Dividend (in
+    contrast to integer mod). To force a behavior like numpy.fmod() an
+    'fmod' Attribute is provided. This attribute is set to 0 by default
+    causing the behavior to be like integer mod. Setting this attribute to 1
+    causes the remainder to be calculated similar to that of numpy.fmod().
 
-       If the input type is floating point, then `fmod` attribute must be set to 1.
+    If the input type is floating point, then ``fmod`` attribute must be set
+    to 1.
 
-       In case of dividend being zero, the results will be platform dependent.
+    In case of dividend being zero, the results will be platform dependent.
 
     This operator supports **multidirectional (i.e., Numpy-style)
     broadcasting**; for more details please check `the
     doc <https://github.com/onnx/onnx/blob/main/docs/Broadcasting.md>`__.
 
     Parameters
     ==========
@@ -10104,26 +10025,26 @@
     or if weight is provided,
 
     ::
 
        sum(loss) / sum(weight[target[n][d_1][d_2]...[d_k]]]), for all samples.
 
     If "reduction" attribute is set to "sum", the output is a scalar:
-    sum(loss).
+    ``sum(loss)``.
 
     See also https://pytorch.org/docs/stable/nn.html#torch.nn.NLLLoss.
 
     Example 1:
 
     ::
 
        // negative log likelihood loss, "none" reduction
        N, C, d1 = 2, 3, 2
        input = [[[1.0, 2.0], [2.0, 2.0], [3.0, 2.0]],
-                [[0.0, 1.0], [2.0, 2.0], [1.0, 2]]]
+                 [[0.0, 1.0], [2.0, 2.0], [1.0, 2]]]
        target = [[2, 1], [0, 2]]
 
        loss = np.zeros((N, d1))
        for n in range(N):
            for d_1 in range(d1):
                c = target[n][d_1]
                loss[n][d_1] = -input[n][c][d_1]
@@ -10633,23 +10554,18 @@
     X: Var,
     slope: Var,
 ) -> Var:
     r"""
     PRelu takes input data (Tensor<T>) and slope tensor as input, and
     produces one output data (Tensor<T>) where the function
     ``f(x) = slope * x for x < 0``, ``f(x) = x for x >= 0``., is applied to
-    the data tensor elementwise.
-
-    **History**
-
-    -  Version 16 adds bfloat16 to the types allowed. This operator supports
-       **unidirectional broadcasting** (tensor slope should be
-       unidirectional broadcastable to input tensor X); for more details
-       please check `the
-       doc <https://github.com/onnx/onnx/blob/main/docs/Broadcasting.md>`__.
+    the data tensor elementwise. This operator supports **unidirectional
+    broadcasting** (tensor slope should be unidirectional broadcastable to
+    input tensor X); for more details please check `the
+    doc <https://github.com/onnx/onnx/blob/main/docs/Broadcasting.md>`__.
 
     Parameters
     ==========
     X
         Type T.
         Input tensor
     slope
@@ -11090,15 +11006,15 @@
     The linear quantization operator. It consumes a high precision tensor, a
     scale, and a zero point to compute the low precision / quantized tensor.
     The scale factor and zero point must have same shape, and can be either
     a scalar for per-tensor / per layer quantization, or a 1-D tensor for
     per-axis quantization. The quantization formula is y = saturate ((x /
     y_scale) + y_zero_point). For saturation, it saturates to [0, 255] if
     it's uint8, or [-128, 127] if it's int8. For (x / y_scale), it's
-    rounding to nearest ties to even. Refer to
+    rounding to the nearest even. Refer to
     https://en.wikipedia.org/wiki/Rounding for details. 'y_zero_point' and
     'y' must have same type.
 
     Parameters
     ==========
     x
         Type T1.
@@ -11163,65 +11079,44 @@
 ) -> Tuple[Var, Var]:
     r"""
     Computes an one-layer simple RNN. This operator is usually supported via
     some custom implementation such as CuDNN.
 
     Notations:
 
-    ``X`` - input tensor
-
-    ``i`` - input gate
-
-    ``t`` - time step (t-1 means previous time step)
-
-    ``Wi`` - W parameter weight matrix for input gate
-
-    ``Ri`` - R recurrence weight matrix for input gate
-
-    ``Wbi`` - W parameter bias vector for input gate
-
-    ``Rbi`` - R parameter bias vector for input gate
-
-    ``WBi`` - W parameter weight matrix for backward input gate
-
-    ``RBi`` - R recurrence weight matrix for backward input gate
-
-    ``WBbi`` - WR bias vectors for backward input gate
-
-    ``RBbi`` - RR bias vectors for backward input gate
-
-    ``H`` - Hidden state
-
-    ``num_directions`` - 2 if direction == bidirectional else 1
+    -  ``X`` - input tensor
+    -  ``i`` - input gate
+    -  ``t`` - time step (t-1 means previous time step)
+    -  ``Wi`` - W parameter weight matrix for input gate
+    -  ``Ri`` - R recurrence weight matrix for input gate
+    -  ``Wbi`` - W parameter bias vector for input gate
+    -  ``Rbi`` - R parameter bias vector for input gate
+    -  ``WBi`` - W parameter weight matrix for backward input gate
+    -  ``RBi`` - R recurrence weight matrix for backward input gate
+    -  ``WBbi`` - WR bias vectors for backward input gate
+    -  ``RBbi`` - RR bias vectors for backward input gate
+    -  ``H`` - Hidden state
+    -  ``num_directions`` - 2 if direction == bidirectional else 1
 
     Activation functions:
 
-    Relu(x) - max(0, x)
-
-    Tanh(x) - (1 - e^{-2x})/(1 + e^{-2x})
-
-    Sigmoid(x) - 1/(1 + e^{-x})
-
-    (NOTE: Below are optional)
-
-    Affine(x) - alpha*x + beta
-
-    LeakyRelu(x) - x if x >= 0 else alpha \* x
-
-    ThresholdedRelu(x) - x if x >= alpha else 0
-
-    ScaledTanh(x) - alpha\ *Tanh(beta*\ x)
-
-    HardSigmoid(x) - min(max(alpha*x + beta, 0), 1)
-
-    Elu(x) - x if x >= 0 else alpha*(e^x - 1)
-
-    Softsign(x) - x/(1 + \|x|)
-
-    Softplus(x) - log(1 + e^x)
+    -  Relu(x) - max(0, x)
+    -  Tanh(x) - (1 - e^{-2x})/(1 + e^{-2x})
+    -  Sigmoid(x) - 1/(1 + e^{-x})
+
+    NOTE: Below are optional
+
+    -  Affine(x) - alpha*x + beta
+    -  LeakyRelu(x) - x if x >= 0 else alpha \* x
+    -  ThresholdedRelu(x) - x if x >= alpha else 0
+    -  ScaledTanh(x) - alpha\ *Tanh(beta*\ x)
+    -  HardSigmoid(x) - min(max(alpha*x + beta, 0), 1)
+    -  Elu(x) - x if x >= 0 else alpha*(e^x - 1)
+    -  Softsign(x) - x/(1 + \|x\|)
+    -  Softplus(x) - log(1 + e^x)
 
     Equations (Default: f=Tanh):
 
     -  Ht = f(Xt*(Wi^T) + Ht-1*(Ri^T) + Wbi + Rbi) This operator has
        **optional** inputs/outputs. See `the
        doc <https://github.com/onnx/onnx/blob/main/docs/IR.md>`__ for more
        details about the representation of optional arguments. An empty
@@ -11602,32 +11497,41 @@
     delta: Var,
 ) -> Var:
     r"""
     Generate a tensor containing a sequence of numbers that begin at
     ``start`` and extends by increments of ``delta`` up to ``limit``
     (exclusive).
 
-    The number of elements in the output of range is computed as below-
+    The number of elements in the output of range is computed as below:
 
-    ``number_of_elements = max( ceil( (limit - start) / delta ) , 0 )``
+    ::
 
-    The pseudocode determining the contents of the output is shown below-
+       number_of_elements = max( ceil( (limit - start) / delta ) , 0 )
 
-    ``for(int i=0; i<number_of_elements; ++i)``
+    The pseudocode determining the contents of the output is shown below:
 
-    ``{``
+    ::
+
+       for(int i=0; i<number_of_elements; ++i) {
+         output[i] =  start + (i * delta);
+       }
+
+    Example 1
 
-    ``output[i] =  start + (i * delta);``
+    ::
+
+       Inputs: start = 3, limit = 9, delta = 3
+       Output: [3, 6]
 
-    ``}``
+    Example 2
 
-    ``Example 1`` Inputs: start = 3, limit = 9, delta = 3 Output: [3, 6]
+    ::
 
-    ``Example 2`` Inputs: start = 10, limit = 4, delta = -2 Output: [10, 8,
-    6]
+       Inputs: start = 10, limit = 4, delta = -2
+       Output: [10, 8, 6]
 
     Parameters
     ==========
     start
         Type T.
         Scalar. First entry for the range of output values.
     limit
@@ -11699,18 +11603,18 @@
 def reduce_l1(
     data: Var,
     *,
     axes: Optional[Iterable[int]] = None,
     keepdims: int = 1,
 ) -> Var:
     r"""
-    Computes the L1 norm of the input tensor's element along the provided
+    Computes the L1 norm of the input tensor's elements along the provided
     axes. The resulting tensor has the same rank as the input if keepdims
     equals 1. If keepdims equals 0, then the resulting tensor has the
-    reduced dimension pruned.
+    reduced dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -11753,18 +11657,18 @@
 def reduce_l2(
     data: Var,
     *,
     axes: Optional[Iterable[int]] = None,
     keepdims: int = 1,
 ) -> Var:
     r"""
-    Computes the L2 norm of the input tensor's element along the provided
+    Computes the L2 norm of the input tensor's elements along the provided
     axes. The resulting tensor has the same rank as the input if keepdims
     equals 1. If keepdims equals 0, then the resulting tensor has the
-    reduced dimension pruned.
+    reduced dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -11807,18 +11711,18 @@
 def reduce_log_sum(
     data: Var,
     *,
     axes: Optional[Iterable[int]] = None,
     keepdims: int = 1,
 ) -> Var:
     r"""
-    Computes the log sum of the input tensor's element along the provided
+    Computes the log sum of the input tensor's elements along the provided
     axes. The resulting tensor has the same rank as the input if keepdims
     equals 1. If keepdims equals 0, then the resulting tensor has the
-    reduced dimension pruned.
+    reduced dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -11861,18 +11765,18 @@
 def reduce_log_sum_exp(
     data: Var,
     *,
     axes: Optional[Iterable[int]] = None,
     keepdims: int = 1,
 ) -> Var:
     r"""
-    Computes the log sum exponent of the input tensor's element along the
+    Computes the log sum exponent of the input tensor's elements along the
     provided axes. The resulting tensor has the same rank as the input if
     keepdims equals 1. If keepdims equals 0, then the resulting tensor has
-    the reduced dimension pruned.
+    the reduced dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -11915,18 +11819,18 @@
 def reduce_max(
     data: Var,
     *,
     axes: Optional[Iterable[int]] = None,
     keepdims: int = 1,
 ) -> Var:
     r"""
-    Computes the max of the input tensor's element along the provided axes.
+    Computes the max of the input tensor's elements along the provided axes.
     The resulting tensor has the same rank as the input if keepdims equals
     1. If keepdims equals 0, then the resulting tensor has the reduced
-    dimension pruned.
+    dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -11969,18 +11873,18 @@
 def reduce_mean(
     data: Var,
     *,
     axes: Optional[Iterable[int]] = None,
     keepdims: int = 1,
 ) -> Var:
     r"""
-    Computes the mean of the input tensor's element along the provided axes.
-    The resulting tensor has the same rank as the input if keepdims equals
-    1. If keepdims equals 0, then the resulting tensor has the reduced
-    dimension pruned.
+    Computes the mean of the input tensor's elements along the provided
+    axes. The resulting tensor has the same rank as the input if keepdims
+    equals 1. If keepdims equals 0, then the resulting tensor has the
+    reduced dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -12023,18 +11927,18 @@
 def reduce_min(
     data: Var,
     *,
     axes: Optional[Iterable[int]] = None,
     keepdims: int = 1,
 ) -> Var:
     r"""
-    Computes the min of the input tensor's element along the provided axes.
+    Computes the min of the input tensor's elements along the provided axes.
     The resulting tensor has the same rank as the input if keepdims equals
     1. If keepdims equals 0, then the resulting tensor has the reduced
-    dimension pruned.
+    dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -12077,18 +11981,18 @@
 def reduce_prod(
     data: Var,
     *,
     axes: Optional[Iterable[int]] = None,
     keepdims: int = 1,
 ) -> Var:
     r"""
-    Computes the product of the input tensor's element along the provided
+    Computes the product of the input tensor's elements along the provided
     axes. The resulting tensor has the same rank as the input if keepdims
     equals 1. If keepdims equals 0, then the resulting tensor has the
-    reduced dimension pruned.
+    reduced dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -12132,18 +12036,18 @@
     data: Var,
     axes: Optional[Var] = None,
     *,
     keepdims: int = 1,
     noop_with_empty_axes: int = 0,
 ) -> Var:
     r"""
-    Computes the sum of the input tensor's element along the provided axes.
+    Computes the sum of the input tensor's elements along the provided axes.
     The resulting tensor has the same rank as the input if keepdims equals
     1. If keepdims equals 0, then the resulting tensor has the reduced
-    dimension pruned.
+    dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -12195,18 +12099,18 @@
 def reduce_sum_square(
     data: Var,
     *,
     axes: Optional[Iterable[int]] = None,
     keepdims: int = 1,
 ) -> Var:
     r"""
-    Computes the sum square of the input tensor's element along the provided
-    axes. The resulting tensor has the same rank as the input if keepdims
-    equals 1. If keepdims equals 0, then the resulting tensor has the
-    reduced dimension pruned.
+    Computes the sum square of the input tensor's elements along the
+    provided axes. The resulting tensor has the same rank as the input if
+    keepdims equals 1. If keepdims equals 0, then the resulting tensor has
+    the reduced dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -12660,16 +12564,17 @@
 
 def round(
     X: Var,
 ) -> Var:
     r"""
     Round takes one input Tensor and rounds the values, element-wise,
     meaning it finds the nearest integer for each value. In case of halfs,
-    the rule is to round them to the nearest even integer. The output tensor
-    has the same shape and type as the input.
+    the rule is to round them to the nearest even integer. If input x is
+    integral, +0, -0, NaN, or infinite, x itself is returned. The output
+    tensor has the same shape and type as the input.
 
     Examples:
 
     ::
 
        round([0.9]) = [1.0]
        round([2.5]) = [2.0]
@@ -12736,15 +12641,15 @@
     frame_length
         Type T2.
         A scalar representing the size of the DFT. It's an optional value.
     onesided
         Attribute.
         If onesided is 1, only values for w in [0, 1, 2, ..., floor(n_fft/2) +
         1] are returned because the real-to-complex Fourier transform satisfies
-        the conjugate symmetry, i.e., X[m, w] = X[m,w]=X[m,n_fft-w]*. Note if
+        the conjugate symmetry, i.e., X[m, w] = X[m,w]=X[m,n_fft-w]\*. Note if
         the input or window tensors are complex, then onesided output is not
         possible. Enabling onesided with real inputs performs a Real-valued fast
         Fourier transform (RFFT).When invoked with real or complex valued input,
         the default value is 1. Values can be 0 or 1.
 
     Returns
     =======
@@ -13661,22 +13566,40 @@
     included. Negative axes indicate counting back from the last axis. Note
     that axes will be clamped to the range [0, r-1], where r is the rank of
     the input tensor if they are out-of-range (after adding r in the case of
     negative axis). Thus, specifying any end value > r is equivalent to
     specifying an end value of r, and specifying any start value < -r is
     equivalent to specifying a start value of 0.
 
-    For example: Input tensor with shape: [2, 3, 4] No attributes specified.
-    Output: [2, 3, 4]
+    Examples:
+
+    ::
+
+       Input tensor with shape: [2, 3, 4]
+       No attributes specified.
+       Output: [2, 3, 4]
 
-    Input tensor with shape: [2, 3, 4] start: -1 Output: [4]
+    ::
+
+       Input tensor with shape: [2, 3, 4]
+       start: -1
+       Output: [4]
 
-    Input tensor with shape: [2, 3, 4] end: -1 Output: [2, 3]
+    ::
 
-    Input tensor with shape: [2, 3, 4] start: 1 end: 2 Output: [3]
+       Input tensor with shape: [2, 3, 4]
+       end: -1
+       Output: [2, 3]
+
+    ::
+
+       Input tensor with shape: [2, 3, 4]
+       start: 1
+       end: 2
+       Output: [3]
 
     Parameters
     ==========
     data
         Type T.
         An input tensor.
     end
@@ -13975,18 +13898,43 @@
 
     Finally, ``step[axes[i]] = steps[i]``.
 
     For slicing to the end of a dimension with unknown size, it is
     recommended to pass in ``INT_MAX`` when slicing forward and 'INT_MIN'
     when slicing backward.
 
-    Example 1: data = [ [1, 2, 3, 4], [5, 6, 7, 8], ] axes = [0, 1] starts =
-    [1, 0] ends = [2, 3] steps = [1, 2] result = [ [5, 7], ] Example 2: data
-    = [ [1, 2, 3, 4], [5, 6, 7, 8], ] starts = [0, 1] ends = [-1, 1000]
-    result = [ [2, 3, 4], ]
+    Example 1:
+
+    ::
+
+       data = [
+           [1, 2, 3, 4],
+           [5, 6, 7, 8],
+       ]
+       axes = [0, 1]
+       starts = [1, 0]
+       ends = [2, 3]
+       steps = [1, 2]
+       result = [
+           [5, 7],
+       ]
+
+    Example 2:
+
+    ::
+
+       data = [
+           [1, 2, 3, 4],
+           [5, 6, 7, 8],
+       ]
+       starts = [0, 1]
+       ends = [-1, 1000]
+       result = [
+           [2, 3, 4],
+       ]
 
     Parameters
     ==========
     data
         Type T.
         Tensor of data to extract slices from.
     starts
@@ -14096,35 +14044,54 @@
     identical to the labels input. If the input is 2-D with shape (N, C),
     the loss tensor may be a N-element vector L = (l_1, l_2, ..., l_N). If
     the input is N-D tensor with shape (N, C, D1, D2, ..., Dk), the loss
     tensor L may have (N, D1, D2, ..., Dk) as its shape and
     L[i,][j_1][j_2]...[j_k] denotes a scalar element in L. After L is
     available, this operator can optionally do a reduction operator.
 
-    shape(scores): (N, C) where C is the number of classes, or (N, C, D1,
-    D2,..., Dk), with K >= 1 in case of K-dimensional loss. shape(labels):
-    (N) where each value is 0 <= labels[i] <= C-1, or (N, D1, D2,..., Dk),
-    with K >= 1 in case of K-dimensional loss.
+    -  shape(scores): (N, C) where C is the number of classes, or (N, C, D1,
+       D2,..., Dk), with K >= 1 in case of K-dimensional loss.
+    -  shape(labels): (N) where each value is 0 <= labels[i] <= C-1, or (N,
+       D1, D2,..., Dk), with K >= 1 in case of K-dimensional loss.
 
     The loss for one sample, l_i, can caculated as follows:
-    l[i][d1][d2]...[dk] = -y[i][c][d1][d2]..[dk], where i is the index of
-    classes. or l[i][d1][d2]...[dk] = -y[i][c][d1][d2]..[dk] \* weights[c],
-    if 'weights' is provided.
+
+    ::
+
+       l[i][d1][d2]...[dk] = -y[i][c][d1][d2]..[dk], where i is the index of classes.
+
+    or
+
+    ::
+
+       l[i][d1][d2]...[dk] = -y[i][c][d1][d2]..[dk] * weights[c], if 'weights' is provided.
 
     loss is zero for the case when label-value equals ignore_index.
-    l[i][d1][d2]...[dk] = 0, when labels[n][d1][d2]...[dk] = ignore_index
 
-    where: p = Softmax(scores) y = Log(p) c = labels[i][d1][d2]...[dk]
+    ::
+
+       l[i][d1][d2]...[dk]  = 0, when labels[n][d1][d2]...[dk] = ignore_index
 
-    Finally, L is optionally reduced: If reduction = 'none', the output is L
-    with shape (N, D1, D2, ..., Dk). If reduction = 'sum', the output is
-    scalar: Sum(L). If reduction = 'mean', the output is scalar:
-    ReduceMean(L), or if weight is provided: ReduceSum(L) / ReduceSum(W),
-    where tensor W is of shape (N, D1, D2, ..., Dk) and W[n][d1][d2]...[dk]
-    = weights[labels[i][d1][d2]...[dk]].
+    where:
+
+    ::
+
+       p = Softmax(scores)
+       y = Log(p)
+       c = labels[i][d1][d2]...[dk]
+
+    Finally, L is optionally reduced:
+
+    -  If reduction = 'none', the output is L with shape (N, D1, D2, ...,
+       Dk).
+    -  If reduction = 'sum', the output is scalar: Sum(L).
+    -  If reduction = 'mean', the output is scalar: ReduceMean(L), or if
+       weight is provided: ``ReduceSum(L) / ReduceSum(W)``, where tensor W
+       is of shape ``(N, D1, D2, ..., Dk)`` and
+       ``W[n][d1][d2]...[dk] = weights[labels[i][d1][d2]...[dk]]``.
 
     Parameters
     ==========
     scores
         Type T.
         The predicted outputs with shape [batch_size, class_size], or
         [batch_size, class_size, D1, D2 , ..., Dk], where K is the number of
@@ -14220,28 +14187,28 @@
     ).outputs.Y
 
 
 def softsign(
     input: Var,
 ) -> Var:
     r"""
-    Calculates the softsign (x/(1+|x|)) of the given input tensor
+    Calculates the softsign (x/(1+|x\|)) of the given input tensor
     element-wise.
 
     Parameters
     ==========
     input
         Type T.
         Input tensor
 
     Returns
     =======
     output : Var
         Type T.
-        The softsign (x/(1+|x|)) values of the input tensor computed
+        The softsign (x/(1+|x\|)) values of the input tensor computed
         element-wise
 
     Notes
     =====
     Signature: ``ai.onnx@1::Softsign``.
 
     Type constraints:
@@ -14358,23 +14325,26 @@
     split: Optional[Var] = None,
     *,
     axis: int = 0,
     keepdims: int = 1,
 ) -> Var:
     r"""
     Split a tensor into a sequence of tensors, along the specified 'axis'.
-    Lengths of the parts can be specified using argument 'split'. 'split'
-    must contain only positive numbers. 'split' is either a scalar (tensor
-    of empty shape), or a 1-D tensor. If 'split' is a scalar, then 'input'
-    will be split into equally sized chunks(if possible). Last chunk will be
-    smaller if the 'input' size along the given axis 'axis' is not divisible
-    by 'split'. Otherwise, the tensor is split into 'size(split)' chunks,
-    with lengths of the parts on 'axis' specified in 'split'. In this
-    scenario, the sum of entries in 'split' must be equal to the dimension
-    size of input tensor on 'axis'.
+    Lengths of the parts can be specified using the optional argument
+    'split'. If the argument
+    ``split' is not specified, a default scalar value of 1 is used as the value of``\ split'.
+    'split' must contain only positive numbers. 'split' is either a scalar
+    (tensor of empty shape), or a 1-D tensor. If 'split' is a scalar, then
+    'input' will be split into chunks all of size 'split' if possible. The
+    last chunk alone may be smaller than 'split' if the 'input' size along
+    the given axis 'axis' is not divisible by 'split'. If 'split' is a
+    1-dimensional tensor, the input tensor is split into 'size(split)'
+    chunks, with lengths of the parts on 'axis' specified in 'split'. In
+    this scenario, the sum of entries in 'split' must be equal to the
+    dimension size of input tensor on 'axis'.
 
     Parameters
     ==========
     input
         Type T.
         The tensor to split
     split
@@ -14798,15 +14768,15 @@
         of n-grams. For example, if ngram_counts is [0, 17, 36], the first index
         (zero-based) of 1-gram/2-gram/3-gram in pool are 0/17/36. This format is
         essentially identical to CSR (or CSC) sparse matrix format, and we
         choose to use this due to its popularity.
     ngram_indexes
         Attribute.
         list of int64s (type: AttributeProto::INTS). This list is parallel to
-        the specified 'pool_*' attribute. The i-th element in ngram_indexes
+        the specified 'pool\_\*' attribute. The i-th element in ngram_indexes
         indicate the coordinate of the i-th n-gram in the output tensor.
     pool_int64s
         Attribute.
         List of int64 n-grams learned from the training set. Either this or
         pool_strings attributes must be present but not both. It's an 1-D tensor
         starting with the collections of all 1-grams and ending with the
         collections of n-grams. The i-th element in pool stores the n-gram that
@@ -14950,24 +14920,32 @@
     axis: int = -1,
     largest: int = 1,
     sorted: int = 1,
 ) -> Tuple[Var, Var]:
     r"""
     Retrieve the top-K largest or smallest elements along a specified axis.
     Given an input tensor of shape [a_1, a_2, ..., a_n, r] and integer
-    argument k, return two outputs: -Value tensor of shape [a_1, a_2, ...,
-    a_{axis-1}, k, a_{axis+1}, ... a_n] which contains the values of the top
-    k elements along the specified axis -Index tensor of shape [a_1, a_2,
-    ..., a_{axis-1}, k, a_{axis+1}, ... a_n] which contains the indices of
-    the top k elements (original indices from the input tensor).
-
-    If "largest" is 1 (the default value) then the k largest elements are
-    returned. If "sorted" is 1 (the default value) then the resulting k
-    elements will be sorted. If "sorted" is 0, order of returned 'Values'
-    and 'Indices' are undefined.
+    argument k, return two outputs:
+
+    -  Value tensor of shape [a_1, a_2, ..., a\_{axis-1}, k, a\_{axis+1},
+       ... a_n] which contains the values of the top k elements along the
+       specified axis
+
+    -  Index tensor of shape [a_1, a_2, ..., a\_{axis-1}, k, a\_{axis+1},
+       ... a_n] which contains the indices of the top k elements (original
+       indices from the input tensor).
+
+    -  If "largest" is 1 (the default value) then the k largest elements are
+       returned.
+
+    -  If "sorted" is 1 (the default value) then the resulting k elements
+       will be sorted.
+
+    -  If "sorted" is 0, order of returned 'Values' and 'Indices' are
+       undefined.
 
     Given two equivalent values, this operator uses the indices along the
     axis as a tiebreaker. That is, the element with the lower index will
     appear first.
 
     Parameters
     ==========
@@ -14990,19 +14968,19 @@
         Attribute.
         Whether to return the elements in sorted order.
 
     Returns
     =======
     Values : Var
         Type T.
-        Tensor of shape [a_1, a_2, ..., a_{axis-1}, k, a_{axis+1}, ... a_n]
+        Tensor of shape [a_1, a_2, ..., a\_{axis-1}, k, a\_{axis+1}, ... a_n]
         containing top K values from the input tensor
     Indices : Var
         Type I.
-        Tensor of shape [a_1, a_2, ..., a_{axis-1}, k, a_{axis+1}, ... a_n]
+        Tensor of shape [a_1, a_2, ..., a\_{axis-1}, k, a\_{axis+1}, ... a_n]
         containing the corresponding input tensor indices for the top K values.
 
     Notes
     =====
     Signature: ``ai.onnx@11::TopK``.
 
     Type constraints:
@@ -15073,25 +15051,25 @@
 ) -> Var:
     r"""
     Given a 2-D matrix or batches of 2-D matrices, returns the upper or
     lower triangular part of the tensor(s). The attribute "upper" determines
     whether the upper or lower part is retained. If set to true, the upper
     triangular matrix is retained. Lower triangular matrix is retained
     otherwise. Default value for the "upper" attribute is true. Trilu takes
-    one input tensor of shape [*, N, M], where \* is zero or more batch
+    one input tensor of shape [\*, N, M], where \* is zero or more batch
     dimensions. The upper triangular part consists of the elements on and
     above the given diagonal (k). The lower triangular part consists of
     elements on and below the diagonal. All other elements in the matrix are
     set to zero. If k = 0, the triangular part on and above/below the main
     diagonal is retained. If upper is set to true, a positive k retains the
     upper triangular matrix excluding the main diagonal and (k-1) diagonals
     above it. A negative k value retains the main diagonal and \|k\|
     diagonals below it. If upper is set to false, a positive k retains the
     lower triangular matrix including the main diagonal and k diagonals
-    above it. A negative k value excludes the main diagonal and (|k|-1)
+    above it. A negative k value excludes the main diagonal and (\|k\|-1)
     diagonals below it.
 
     Parameters
     ==========
     input
         Type T.
         Input tensor of rank 2 or higher.
@@ -15151,51 +15129,109 @@
     element of 'Y' in the input.
 
     Outputs are either sorted in ascending order or optionally in the order
     of the first occurrence of the values in the input.
 
     https://docs.scipy.org/doc/numpy/reference/generated/numpy.unique.html
 
-    Example 1: input_X = [2, 1, 1, 3, 4, 3] attribute_sorted = 0
-    attribute_axis = None output_Y = [2, 1, 3, 4] output_indices = [0, 1, 3,
-    4] output_inverse_indices = [0, 1, 1, 2, 3, 2] output_counts = [1, 2, 2,
-    1]
+    Example 1:
 
-    Example 2: input_X = [[1, 3], [2, 3]] attribute_sorted = 1
-    attribute_axis = None output_Y = [1, 2, 3] output_indices = [0, 2, 1]
-    output_inverse_indices = [0, 2, 1, 2] output_counts = [1, 1, 2]
+    ::
 
-    Example 3: input_X = [[1, 0, 0], [1, 0, 0], [2, 3, 4]] attribute_sorted
-    = 1 attribute_axis = 0 output_Y = [[1, 0, 0], [2, 3, 4]] output_indices
-    = [0, 2] output_inverse_indices = [0, 0, 1] output_counts = [2, 1]
+       input_X = [2, 1, 1, 3, 4, 3]
+       attribute_sorted = 0
+       attribute_axis = None
+       output_Y = [2, 1, 3, 4]
+       output_indices = [0, 1, 3, 4]
+       output_inverse_indices = [0, 1, 1, 2, 3, 2]
+       output_counts = [1, 2, 2, 1]
 
-    Example 4: input_x = [[[1., 1.], [0., 1.], [2., 1.], [0., 1.]], [[1.,
-    1.], [0., 1.], [2., 1.], [0., 1.]]] attribute_sorted = 1 attribute_axis
-    = 1
+    Example 2:
 
-    intermediate data are presented below for better understanding:
+    ::
 
-    there are 4 subtensors sliced along axis 1 of input_x (shape = (2, 4,
-    2)): A: [[1, 1], [1, 1]], [[0, 1], [0, 1]], [[2, 1], [2, 1]], [[0, 1],
-    [0, 1]].
+       input_X = [[1, 3], [2, 3]]
+       attribute_sorted = 1
+       attribute_axis = None
+       output_Y = [1, 2, 3]
+       output_indices = [0, 2, 1]
+       output_inverse_indices = [0, 2, 1, 2]
+       output_counts = [1, 1, 2]
 
-    there are 3 unique subtensors: [[1, 1], [1, 1]], [[0, 1], [0, 1]], [[2,
-    1], [2, 1]].
+    Example 3:
 
-    sorted unique subtensors: B: [[0, 1], [0, 1]], [[1, 1], [1, 1]], [[2,
-    1], [2, 1]].
+    ::
 
-    output_Y is constructed from B: [[[0. 1.], [1. 1.], [2. 1.]], [[0. 1.],
-    [1. 1.], [2. 1.]]]
+       input_X = [[1, 0, 0], [1, 0, 0], [2, 3, 4]]
+       attribute_sorted = 1
+       attribute_axis = 0
+       output_Y = [[1, 0, 0], [2, 3, 4]]
+       output_indices = [0, 2]
+       output_inverse_indices = [0, 0, 1]
+       output_counts = [2, 1]
 
-    output_indices is to map from B to A: [1, 0, 2]
+    Example 4:
 
-    output_inverse_indices is to map from A to B: [1, 0, 2, 0]
+    ::
 
-    output_counts = [2 1 1]
+       input_x = [[[1., 1.], [0., 1.], [2., 1.], [0., 1.]],
+                   [[1., 1.], [0., 1.], [2., 1.], [0., 1.]]]
+       attribute_sorted = 1
+       attribute_axis = 1
+
+    intermediate data are presented below for better understanding: there
+    are 4 subtensors sliced along axis 1 of input_x (shape = (2, 4, 2)):
+
+    ::
+
+       A: [[1, 1], [1, 1]],
+          [[0, 1], [0, 1]],
+          [[2, 1], [2, 1]],
+          [[0, 1], [0, 1]].
+
+    there are 3 unique subtensors:
+
+    ::
+
+       [[1, 1], [1, 1]],
+       [[0, 1], [0, 1]],
+       [[2, 1], [2, 1]].
+
+    sorted unique subtensors:
+
+    ::
+
+       B: [[0, 1], [0, 1]],
+          [[1, 1], [1, 1]],
+          [[2, 1], [2, 1]].
+
+    output_Y is constructed from B:
+
+    ::
+
+       [[[0. 1.], [1. 1.], [2. 1.]],
+        [[0. 1.], [1. 1.], [2. 1.]]]
+
+    output_indices is to map from B to A:
+
+    ::
+
+       [1, 0, 2]
+
+    output_inverse_indices is to map from A to B:
+
+    ::
+
+       [1, 0, 2, 0]
+
+    output_counts:
+
+    ::
+
+       [2, 1, 1]
 
     Parameters
     ==========
     X
         Type T.
         A N-D input tensor that is to be processed.
     axis
@@ -15257,15 +15293,15 @@
 ) -> Var:
     r"""
     Insert single-dimensional entries to the shape of an input tensor
     (``data``). Takes one required input ``axes`` - which contains a list of
     dimension indices and this operator will insert a dimension of value
     ``1`` into the corresponding index of the output tensor (``expanded``).
 
-    For example: Given an input tensor (``data``) of shape [3, 4, 5], then
+    For example, given an input tensor (``data``) of shape [3, 4, 5], then
     Unsqueeze(data, axes=[0, 4]) outputs a tensor (``expanded``) containing
     same data as ``data`` but with shape [1, 3, 4, 5, 1].
 
     The input ``axes`` should not contain any duplicate entries. It is an
     error if it contains duplicates. The rank of the output tensor
     (``output_rank``) is the rank of the input tensor (``data``) plus the
     number of values in ``axes``. Each value in ``axes`` should be within
@@ -15316,19 +15352,14 @@
     `numpy.where <https://docs.scipy.org/doc/numpy/reference/generated/numpy.where.html>`__
     with three parameters.
 
     This operator supports **multidirectional (i.e., Numpy-style)
     broadcasting**; for more details please check `the
     doc <https://github.com/onnx/onnx/blob/main/docs/Broadcasting.md>`__.
 
-    **History**
-
-    -  Version 16 adds bfloat16 to the types allowed (for the second and
-       third parameter).
-
     Parameters
     ==========
     condition
         Type B.
         When True (nonzero), yield X, otherwise yield Y
     X
         Type T.
```

### Comparing `spox-0.8.0/src/spox/opset/ai/onnx/v18.py` & `spox-0.9.0/src/spox/opset/ai/onnx/v18.py`

 * *Files 1% similar despite different names*

```diff
@@ -1337,19 +1337,16 @@
 
     or
 
     ::
 
        output_spatial_shape[i] = ceil((input_spatial_shape[i] + pad_shape[i] - {kernelSpatialShape}) / strides_spatial_shape[i] + 1)
 
-    if ceil_mode is enabled
-
-    ::
-
-       * pad_shape[i] is sum of pads along axis i
+    if ceil_mode is enabled ``pad_shape[i]`` is the sum of pads along axis
+    ``i``.
 
     ``auto_pad`` is a DEPRECATED attribute. If you are using them currently,
     the output spatial shape will be following:
 
     ::
 
        VALID: output_spatial_shape[i] = ceil((input_spatial_shape[i] - {kernelSpatialShape} + 1) / strides_spatial_shape[i])
@@ -1575,47 +1572,77 @@
        or False)
 
     2) ``reflect`` - pads with the reflection of the vector mirrored on the
        first and last values of the vector along each axis
 
     3) ``edge`` - pads with the edge values of array
 
-    Example 1 (``constant`` mode): Insert 0 pads to the beginning of the
-    second dimension.
+    Example 1 (``constant`` mode):
 
-    data = [ [1.0, 1.2], [2.3, 3.4], [4.5, 5.7], ]
+    Insert 0 pads to the beginning of the second dimension.
 
-    pads = [0, 2, 0, 0]
+    ::
 
-    mode = 'constant'
+       data = [
+           [1.0, 1.2],
+           [2.3, 3.4],
+           [4.5, 5.7],
+       ]
 
-    constant_value = 0.0
+       pads = [0, 2, 0, 0]
 
-    output = [ [0.0, 0.0, 1.0, 1.2], [0.0, 0.0, 2.3, 3.4], [0.0, 0.0, 4.5,
-    5.7], ]
+       mode = 'constant'
 
-    Example 2 (``reflect`` mode): data = [ [1.0, 1.2], [2.3, 3.4], [4.5,
-    5.7], ]
+       constant_value = 0.0
 
-    pads = [0, 2, 0, 0]
+       output = [
+           [0.0, 0.0, 1.0, 1.2],
+           [0.0, 0.0, 2.3, 3.4],
+           [0.0, 0.0, 4.5, 5.7],
+       ]
 
-    mode = 'reflect'
+    Example 2 (``reflect`` mode):
 
-    output = [ [1.0, 1.2, 1.0, 1.2], [2.3, 3.4, 2.3, 3.4], [4.5, 5.7, 4.5,
-    5.7], ]
+    ::
 
-    Example 3 (``edge`` mode): data = [ [1.0, 1.2], [2.3, 3.4], [4.5, 5.7],
-    ]
+       data = [
+           [1.0, 1.2],
+           [2.3, 3.4],
+           [4.5, 5.7],
+       ]
+
+       pads = [0, 2, 0, 0]
+
+       mode = 'reflect'
+
+       output = [
+           [1.0, 1.2, 1.0, 1.2],
+           [2.3, 3.4, 2.3, 3.4],
+           [4.5, 5.7, 4.5, 5.7],
+       ]
 
-    pads = [0, 2, 0, 0]
+    Example 3 (``edge`` mode):
 
-    mode = 'edge'
+    ::
 
-    output = [ [1.0, 1.0, 1.0, 1.2], [2.3, 2.3, 2.3, 3.4], [4.5, 4.5, 4.5,
-    5.7], ]
+       data = [
+           [1.0, 1.2],
+           [2.3, 3.4],
+           [4.5, 5.7],
+       ]
+
+       pads = [0, 2, 0, 0]
+
+       mode = 'edge'
+
+       output = [
+           [1.0, 1.0, 1.0, 1.2],
+           [2.3, 2.3, 2.3, 3.4],
+           [4.5, 4.5, 4.5, 5.7],
+       ]
 
     Parameters
     ==========
     data
         Type T.
         Input tensor.
     pads
@@ -1674,18 +1701,18 @@
     data: Var,
     axes: Optional[Var] = None,
     *,
     keepdims: int = 1,
     noop_with_empty_axes: int = 0,
 ) -> Var:
     r"""
-    Computes the L1 norm of the input tensor's element along the provided
+    Computes the L1 norm of the input tensor's elements along the provided
     axes. The resulting tensor has the same rank as the input if keepdims
     equals 1. If keepdims equals 0, then the resulting tensor has the
-    reduced dimension pruned.
+    reduced dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -1738,18 +1765,18 @@
     data: Var,
     axes: Optional[Var] = None,
     *,
     keepdims: int = 1,
     noop_with_empty_axes: int = 0,
 ) -> Var:
     r"""
-    Computes the L2 norm of the input tensor's element along the provided
+    Computes the L2 norm of the input tensor's elements along the provided
     axes. The resulting tensor has the same rank as the input if keepdims
     equals 1. If keepdims equals 0, then the resulting tensor has the
-    reduced dimension pruned.
+    reduced dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -1802,18 +1829,18 @@
     data: Var,
     axes: Optional[Var] = None,
     *,
     keepdims: int = 1,
     noop_with_empty_axes: int = 0,
 ) -> Var:
     r"""
-    Computes the log sum of the input tensor's element along the provided
+    Computes the log sum of the input tensor's elements along the provided
     axes. The resulting tensor has the same rank as the input if keepdims
     equals 1. If keepdims equals 0, then the resulting tensor has the
-    reduced dimension pruned.
+    reduced dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -1866,18 +1893,18 @@
     data: Var,
     axes: Optional[Var] = None,
     *,
     keepdims: int = 1,
     noop_with_empty_axes: int = 0,
 ) -> Var:
     r"""
-    Computes the log sum exponent of the input tensor's element along the
+    Computes the log sum exponent of the input tensor's elements along the
     provided axes. The resulting tensor has the same rank as the input if
     keepdims equals 1. If keepdims equals 0, then the resulting tensor has
-    the reduced dimension pruned.
+    the reduced dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -1930,18 +1957,18 @@
     data: Var,
     axes: Optional[Var] = None,
     *,
     keepdims: int = 1,
     noop_with_empty_axes: int = 0,
 ) -> Var:
     r"""
-    Computes the max of the input tensor's element along the provided axes.
+    Computes the max of the input tensor's elements along the provided axes.
     The resulting tensor has the same rank as the input if keepdims equals
     1. If keepdims equals 0, then the resulting tensor has the reduced
-    dimension pruned.
+    dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -1994,18 +2021,18 @@
     data: Var,
     axes: Optional[Var] = None,
     *,
     keepdims: int = 1,
     noop_with_empty_axes: int = 0,
 ) -> Var:
     r"""
-    Computes the mean of the input tensor's element along the provided axes.
-    The resulting tensor has the same rank as the input if keepdims equals
-    1. If keepdims equals 0, then the resulting tensor has the reduced
-    dimension pruned.
+    Computes the mean of the input tensor's elements along the provided
+    axes. The resulting tensor has the same rank as the input if keepdims
+    equals 1. If keepdims equals 0, then the resulting tensor has the
+    reduced dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -2058,18 +2085,18 @@
     data: Var,
     axes: Optional[Var] = None,
     *,
     keepdims: int = 1,
     noop_with_empty_axes: int = 0,
 ) -> Var:
     r"""
-    Computes the min of the input tensor's element along the provided axes.
+    Computes the min of the input tensor's elements along the provided axes.
     The resulting tensor has the same rank as the input if keepdims equals
     1. If keepdims equals 0, then the resulting tensor has the reduced
-    dimension pruned.
+    dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -2122,18 +2149,18 @@
     data: Var,
     axes: Optional[Var] = None,
     *,
     keepdims: int = 1,
     noop_with_empty_axes: int = 0,
 ) -> Var:
     r"""
-    Computes the product of the input tensor's element along the provided
+    Computes the product of the input tensor's elements along the provided
     axes. The resulting tensor has the same rank as the input if keepdims
     equals 1. If keepdims equals 0, then the resulting tensor has the
-    reduced dimension pruned.
+    reduced dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -2186,18 +2213,18 @@
     data: Var,
     axes: Optional[Var] = None,
     *,
     keepdims: int = 1,
     noop_with_empty_axes: int = 0,
 ) -> Var:
     r"""
-    Computes the sum square of the input tensor's element along the provided
-    axes. The resulting tensor has the same rank as the input if keepdims
-    equals 1. If keepdims equals 0, then the resulting tensor has the
-    reduced dimension pruned.
+    Computes the sum square of the input tensor's elements along the
+    provided axes. The resulting tensor has the same rank as the input if
+    keepdims equals 1. If keepdims equals 0, then the resulting tensor has
+    the reduced dimension pruned. Input tensors of rank zero are valid.
 
     The above behavior is similar to numpy, with the exception that numpy
     defaults keepdims to False instead of True.
 
     Parameters
     ==========
     data
@@ -2466,64 +2493,64 @@
     "none", indices should not have duplicate entries: that is, if idx1 !=
     idx2, then indices[idx1] != indices[idx2]. For instance, in a 2-D tensor
     case, the update corresponding to the [i][j] entry is performed as
     below:
 
     ::
 
-         output[indices[i][j]][j] = updates[i][j] if axis = 0,
-         output[i][indices[i][j]] = updates[i][j] if axis = 1,
+       output[indices[i][j]][j] = updates[i][j] if axis = 0,
+       output[i][indices[i][j]] = updates[i][j] if axis = 1,
 
     When ``reduction`` is set to some reduction function ``f``, the update
     corresponding to the [i][j] entry is performed as below:
 
     ::
 
-         output[indices[i][j]][j] += f(output[indices[i][j]][j], updates[i][j]) if axis = 0,
-         output[i][indices[i][j]] += f(output[i][indices[i][j]], updates[i][j]) if axis = 1,
+       output[indices[i][j]][j] += f(output[indices[i][j]][j], updates[i][j]) if axis = 0,
+       output[i][indices[i][j]] += f(output[i][indices[i][j]], updates[i][j]) if axis = 1,
 
-    where the ``f`` is +/*/max/min as specified.
+    where the ``f`` is ``+``, ``*``, ``max`` or ``min`` as specified.
 
     This operator is the inverse of GatherElements. It is similar to Torch's
     Scatter operation.
 
     (Opset 18 change): Adds max/min to the set of allowed reduction ops.
 
     Example 1:
 
     ::
 
-         data = [
-             [0.0, 0.0, 0.0],
-             [0.0, 0.0, 0.0],
-             [0.0, 0.0, 0.0],
-         ]
-         indices = [
-             [1, 0, 2],
-             [0, 2, 1],
-         ]
-         updates = [
-             [1.0, 1.1, 1.2],
-             [2.0, 2.1, 2.2],
-         ]
-         output = [
-             [2.0, 1.1, 0.0]
-             [1.0, 0.0, 2.2]
-             [0.0, 2.1, 1.2]
-         ]
+       data = [
+           [0.0, 0.0, 0.0],
+           [0.0, 0.0, 0.0],
+           [0.0, 0.0, 0.0],
+       ]
+       indices = [
+           [1, 0, 2],
+           [0, 2, 1],
+       ]
+       updates = [
+           [1.0, 1.1, 1.2],
+           [2.0, 2.1, 2.2],
+       ]
+       output = [
+           [2.0, 1.1, 0.0]
+           [1.0, 0.0, 2.2]
+           [0.0, 2.1, 1.2]
+       ]
 
     Example 2:
 
     ::
 
-         data = [[1.0, 2.0, 3.0, 4.0, 5.0]]
-         indices = [[1, 3]]
-         updates = [[1.1, 2.1]]
-         axis = 1
-         output = [[1.0, 1.1, 3.0, 2.1, 5.0]]
+       data = [[1.0, 2.0, 3.0, 4.0, 5.0]]
+       indices = [[1, 3]]
+       updates = [[1.1, 2.1]]
+       axis = 1
+       output = [[1.0, 1.1, 3.0, 2.1, 5.0]]
 
     Parameters
     ==========
     data
         Type T.
         Tensor of rank r >= 1.
     indices
@@ -2632,44 +2659,44 @@
     ::
 
        output = np.copy(data)
        update_indices = indices.shape[:-1]
        for idx in np.ndindex(update_indices):
            output[indices[idx]] = f(output[indices[idx]], updates[idx])
 
-    where the ``f`` is +/*/max/min as specified.
+    where the ``f`` is ``+``, ``*``, ``max`` or ``min`` as specified.
 
     This operator is the inverse of GatherND.
 
     (Opset 18 change): Adds max/min to the set of allowed reduction ops.
 
     Example 1:
 
     ::
 
-         data    = [1, 2, 3, 4, 5, 6, 7, 8]
-         indices = [[4], [3], [1], [7]]
-         updates = [9, 10, 11, 12]
-         output  = [1, 11, 3, 10, 9, 6, 7, 12]
+       data    = [1, 2, 3, 4, 5, 6, 7, 8]
+       indices = [[4], [3], [1], [7]]
+       updates = [9, 10, 11, 12]
+       output  = [1, 11, 3, 10, 9, 6, 7, 12]
 
     Example 2:
 
     ::
 
-         data    = [[[1, 2, 3, 4], [5, 6, 7, 8], [8, 7, 6, 5], [4, 3, 2, 1]],
-                    [[1, 2, 3, 4], [5, 6, 7, 8], [8, 7, 6, 5], [4, 3, 2, 1]],
-                    [[8, 7, 6, 5], [4, 3, 2, 1], [1, 2, 3, 4], [5, 6, 7, 8]],
-                    [[8, 7, 6, 5], [4, 3, 2, 1], [1, 2, 3, 4], [5, 6, 7, 8]]]
-         indices = [[0], [2]]
-         updates = [[[5, 5, 5, 5], [6, 6, 6, 6], [7, 7, 7, 7], [8, 8, 8, 8]],
-                    [[1, 1, 1, 1], [2, 2, 2, 2], [3, 3, 3, 3], [4, 4, 4, 4]]]
-         output  = [[[5, 5, 5, 5], [6, 6, 6, 6], [7, 7, 7, 7], [8, 8, 8, 8]],
-                    [[1, 2, 3, 4], [5, 6, 7, 8], [8, 7, 6, 5], [4, 3, 2, 1]],
-                    [[1, 1, 1, 1], [2, 2, 2, 2], [3, 3, 3, 3], [4, 4, 4, 4]],
-                    [[8, 7, 6, 5], [4, 3, 2, 1], [1, 2, 3, 4], [5, 6, 7, 8]]]
+       data    = [[[1, 2, 3, 4], [5, 6, 7, 8], [8, 7, 6, 5], [4, 3, 2, 1]],
+                   [[1, 2, 3, 4], [5, 6, 7, 8], [8, 7, 6, 5], [4, 3, 2, 1]],
+                   [[8, 7, 6, 5], [4, 3, 2, 1], [1, 2, 3, 4], [5, 6, 7, 8]],
+                   [[8, 7, 6, 5], [4, 3, 2, 1], [1, 2, 3, 4], [5, 6, 7, 8]]]
+       indices = [[0], [2]]
+       updates = [[[5, 5, 5, 5], [6, 6, 6, 6], [7, 7, 7, 7], [8, 8, 8, 8]],
+                   [[1, 1, 1, 1], [2, 2, 2, 2], [3, 3, 3, 3], [4, 4, 4, 4]]]
+       output  = [[[5, 5, 5, 5], [6, 6, 6, 6], [7, 7, 7, 7], [8, 8, 8, 8]],
+                   [[1, 2, 3, 4], [5, 6, 7, 8], [8, 7, 6, 5], [4, 3, 2, 1]],
+                   [[1, 1, 1, 1], [2, 2, 2, 2], [3, 3, 3, 3], [4, 4, 4, 4]],
+                   [[8, 7, 6, 5], [4, 3, 2, 1], [1, 2, 3, 4], [5, 6, 7, 8]]]
 
     Parameters
     ==========
     data
         Type T.
         Tensor of rank r >= 1.
     indices
@@ -2710,15 +2737,14 @@
     ).outputs.output
 
 
 def split(
     input: Var,
     split: Optional[Var] = None,
     *,
-    outputs_count: int,
     axis: int = 0,
     num_outputs: Optional[int] = None,
 ) -> Sequence[Var]:
     r"""
     Split a tensor into a list of tensors, along the specified 'axis'.
     Either input 'split' or the attribute 'num_outputs' should be specified,
     but not both. If the attribute 'num_outputs' is specified, then the
@@ -2740,17 +2766,14 @@
         Attribute.
         Which axis to split on. A negative value means counting dimensions from
         the back. Accepted range is [-rank, rank-1] where r = rank(input).
     num_outputs
         Attribute.
         Number of outputs to split parts of the tensor into. If the tensor is
         not evenly splittable the last chunk will be smaller.
-    outputs_count
-        Specifies the number of variadic outputs of this operator.
-        Non-standard parameter created by the opset generator, as inference (a solution) it was not implemented or is impossible.
 
     Returns
     =======
     outputs : Sequence[Var]
         Type T.
         One or more outputs forming list of tensors after splitting
 
@@ -2766,15 +2789,15 @@
             axis=AttrInt64(axis),
             num_outputs=AttrInt64.maybe(num_outputs),
         ),
         _Split.Inputs(
             input=input,
             split=split,
         ),
-        out_variadic=outputs_count,
+        out_variadic=num_outputs,
     ).outputs.outputs
 
 
 def const(value: npt.ArrayLike, dtype: npt.DTypeLike = None) -> Var:
     """
     Convenience function for creating constants.
```

### Comparing `spox-0.8.0/src/spox.egg-info/PKG-INFO` & `spox-0.9.0/src/spox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spox
-Version: 0.8.0
+Version: 0.9.0
 Summary: A framework for constructing ONNX computational graphs.
 Author-email: Jakub Bachurski <kbachurski@gmail.com>, Christian Bourjau <christian.bourjau@quantco.com>
 Maintainer-email: Jakub Bachurski <kbachurski@gmail.com>, Christian Bourjau <christian.bourjau@quantco.com>
 Project-URL: Source, https://github.com/quantco/spox
 Keywords: machine-learning,onnx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `spox-0.8.0/src/spox.egg-info/SOURCES.txt` & `spox-0.9.0/src/spox.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 src/spox/_fields.py
 src/spox/_function.py
 src/spox/_future.py
 src/spox/_graph.py
 src/spox/_inline.py
 src/spox/_internal_op.py
 src/spox/_node.py
-src/spox/_patch_ref_impl.py
 src/spox/_public.py
 src/spox/_schemas.py
 src/spox/_scope.py
 src/spox/_shape.py
 src/spox/_standard.py
 src/spox/_traverse.py
 src/spox/_type_system.py
@@ -57,14 +56,15 @@
 src/spox.egg-info/PKG-INFO
 src/spox.egg-info/SOURCES.txt
 src/spox.egg-info/dependency_links.txt
 src/spox.egg-info/requires.txt
 src/spox.egg-info/top_level.txt
 src/spox/opset/ai/onnx/v17.py
 src/spox/opset/ai/onnx/v18.py
+src/spox/opset/ai/onnx/v19.py
 src/spox/opset/ai/onnx/ml/v3.py
 tests/__init__.py
 tests/conftest.py
 tests/test_adapt.py
 tests/test_attr.py
 tests/test_broadcast.py
 tests/test_constructors.py
```

### Comparing `spox-0.8.0/tests/conftest.py` & `spox-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/full/conftest.py` & `spox-0.9.0/tests/full/conftest.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/full/test_brackets.py` & `spox-0.9.0/tests/full/test_brackets.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/full/test_lifting.py` & `spox-0.9.0/tests/full/test_lifting.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/full/test_turing_completeness.py` & `spox-0.9.0/tests/full/test_turing_completeness.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/future/test_var_operators.py` & `spox-0.9.0/tests/future/test_var_operators.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/test_adapt.py` & `spox-0.9.0/tests/test_adapt.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/test_attr.py` & `spox-0.9.0/tests/test_attr.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/test_broadcast.py` & `spox-0.9.0/tests/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/test_constructors.py` & `spox-0.9.0/tests/test_constructors.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/test_custom_operator.py` & `spox-0.9.0/tests/test_custom_operator.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/test_equiv_types.py` & `spox-0.9.0/tests/test_equiv_types.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/test_function.py` & `spox-0.9.0/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/test_graph.py` & `spox-0.9.0/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/test_initializer.py` & `spox-0.9.0/tests/test_initializer.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/test_inline.py` & `spox-0.9.0/tests/test_inline.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from typing import Dict
+
 import numpy
 import onnx
 import onnx.parser
 import pytest
 
 import spox.opset.ai.onnx.v17 as op
 from spox._graph import arguments, results
+from spox._inline import rename_in_graph
 from spox._public import inline
 from spox._type_system import Tensor
 from spox._utils import from_array
 from spox._var import Var
 
 
 @pytest.fixture
@@ -240,27 +243,101 @@
     graph = results(c=proj(y, proj(x, y)))
 
     onnx_helper.assert_close(
         onnx_helper.run(graph, "c", a=numpy.array([1.0]), b=numpy.array([2.0])), 2
     )
 
 
-def test_relu_inline_subgraph_warns(onnx_helper, relu_proto):
-    (a,) = arguments(a=Tensor(float, ()))
-    with pytest.raises(ValueError):
-        inline(relu_proto)(a).values()
-
-
-@pytest.mark.skip("Inlining subgraphs requires reimplementing renaming in graphs.")
 def test_relu_inline_subgraph(onnx_helper, relu_proto):
     (a,) = arguments(a=Tensor(float, ()))
     (b,) = inline(relu_proto)(a).values()
     graph = results(b=b).with_arguments(a)
 
-    onnx_helper.assert_close(onnx_helper.run(graph, "b", a=numpy.array([1.0])), 1.0)
-    onnx_helper.assert_close(onnx_helper.run(graph, "b", a=numpy.array([-1.0])), 0.0)
+    onnx_helper.assert_close(onnx_helper.run(graph, "b", a=numpy.array(1.0)), 1.0)
+    onnx_helper.assert_close(onnx_helper.run(graph, "b", a=numpy.array(-1.0)), 0.0)
 
 
 def test_symbolic_dim_stripped(add4_graph):
     x: Var
     (x,) = add4_graph.requested_results.values()
     assert x.unwrap_tensor().shape == (None,)
+
+
+def _make_subgraph_example(op, node, x, c, y1, y2, y):
+    return onnx.helper.make_graph(
+        [
+            onnx.helper.make_node(op, [x, x], [c], name=node),
+            onnx.helper.make_node(
+                "If",
+                [c],
+                [y],
+                then_branch=onnx.helper.make_graph(
+                    [onnx.helper.make_node("Constant", [], [y1], value_int=0)],
+                    "subgraph_then_branch",
+                    [],
+                    [onnx.helper.make_tensor_value_info(x, onnx.TensorProto.INT64, ())],
+                ),
+                else_branch=onnx.helper.make_graph(
+                    [onnx.helper.make_node("Constant", [], [y2], value_int=1)],
+                    "subgraph_else_branch",
+                    [],
+                    [onnx.helper.make_tensor_value_info(x, onnx.TensorProto.INT64, ())],
+                ),
+            ),
+        ],
+        "graph",
+        [onnx.helper.make_tensor_value_info(x, onnx.TensorProto.FLOAT, ())],
+        [onnx.helper.make_tensor_value_info(y, onnx.TensorProto.INT64, ())],
+    )
+
+
+def test_subgraph_rename():
+    renames = {"X": "in", "C": "cond", "Y1": "sub1", "Y2": "sub2", "Y": "out"}
+    renamed = rename_in_graph(
+        _make_subgraph_example("Equal", "I", "X", "C", "Y1", "Y2", "Y"),
+        lambda x: renames[x],
+        rename_node=lambda x: "test",
+        rename_op=lambda d, t: ("", "Less") if (d, t) == ("", "Equal") else (d, t),
+    )
+    expected = _make_subgraph_example(
+        "Less", "test", "in", "cond", "sub1", "sub2", "out"
+    )
+    for i in range(len(renamed.node)):
+        assert renamed.node[i] == expected.node[i], i
+
+
+def _duplicate_subgraphs_to_list(
+    graph_proto_: onnx.GraphProto,
+) -> onnx.GraphProto:
+    # Replace all graph attributes with a list of that graph twice
+    # This obviously invalidates the graph, but we just want to test renaming in those subgraphs
+    graph_proto = onnx.GraphProto()
+    graph_proto.CopyFrom(graph_proto_)
+    for node in graph_proto.node:
+        for attr_proto in node.attribute:
+            graph = onnx.helper.get_attribute_value(attr_proto)
+            if isinstance(graph, onnx.GraphProto):
+                attr_proto.Clear()
+                attr_proto.type = onnx.AttributeProto.GRAPHS
+                attr_proto.graphs.append(graph)
+                attr_proto.graphs.append(graph)
+    return graph_proto
+
+
+def test_subgraph_list_rename(relu_proto):
+    # This is a simple property test that ensures renaming
+    # in lists of subgraphs is the same as in just subgraphs
+    renames: Dict[str, str] = {}
+
+    def example_rename(n: str) -> str:
+        if n not in renames:
+            renames[n] = f"{n}_{len(renames)}"
+        return renames[n]
+
+    rename_then_duplicate = _duplicate_subgraphs_to_list(
+        rename_in_graph(relu_proto.graph, example_rename)
+    )
+    renames.clear()
+    duplicate_then_rename = rename_in_graph(
+        _duplicate_subgraphs_to_list(relu_proto.graph), example_rename
+    )
+    assert rename_then_duplicate.node == duplicate_then_rename.node
```

### Comparing `spox-0.8.0/tests/test_opsets.py` & `spox-0.9.0/tests/test_opsets.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import spox.opset.ai.onnx.ml.v3 as ml3
 import spox.opset.ai.onnx.v17 as op17
 import spox.opset.ai.onnx.v18 as op18
+import spox.opset.ai.onnx.v19 as op19
 
 
 def test_ai_onnx_v17():
     op17.add(op17.constant(value_int=2), op17.constant(value_int=2))
 
 
 def test_ai_onnx_v18():
     op18.bitwise_and(op17.constant(value_int=7), op17.constant(value_int=10))
+    assert len(op18.split(op18.const([1, 2, 3]), num_outputs=3)) == 3
+
+
+def test_ai_onnx_v19():
+    op19.equal(op19.constant(value_string="abc"), op19.constant(value_string="abc"))
 
 
 def test_ai_onnx_ml_v3():
     ml3.label_encoder(
         op17.constant(value_ints=[1, 2, 3]),
         keys_int64s=[0, 1, 2],
         values_strings=["a", "b", "c"],
```

### Comparing `spox-0.8.0/tests/test_public.py` & `spox-0.9.0/tests/test_public.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/test_standard_op.py` & `spox-0.9.0/tests/test_standard_op.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/test_subgraphs.py` & `spox-0.9.0/tests/test_subgraphs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Callable
 
 import numpy
 import pytest
 
 import spox.opset.ai.onnx.v17 as op
 from spox import Var
+from spox._exceptions import BuildError
 from spox._future import initializer
 from spox._graph import arguments, results
 from spox._type_system import Sequence, Tensor
 
 
 def test_subgraph(onnx_helper):
     (e,) = arguments(e=Tensor(numpy.int64, ()))
@@ -425,7 +426,23 @@
     (e,) = arguments(e=Tensor(bool, ()))
     (f,) = op.if_(
         e, then_branch=lambda: [initializer(0)], else_branch=lambda: [op.const(1)]
     )
     graph = results(f=f)
     onnx_helper.assert_close(onnx_helper.run(graph, "f", e=numpy.array(True)), [0])
     onnx_helper.assert_close(onnx_helper.run(graph, "f", e=numpy.array(False)), [1])
+
+
+def test_subgraph_argument_leak_caught():
+    ii: Var = None  # type: ignore
+
+    def fun(i, c):
+        nonlocal ii
+        ii = i
+        return [op.const(True), i]
+
+    (m,) = arguments(m=Tensor(int, ()))
+    (r,) = op.loop(M=m, v_initial=[], body=fun)
+    graph = results(_=op.add(r, ii))
+
+    with pytest.raises(BuildError):
+        graph.to_onnx_model()
```

### Comparing `spox-0.8.0/tests/test_tensor.py` & `spox-0.9.0/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/test_type_translation.py` & `spox-0.9.0/tests/test_type_translation.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/test_value_propagation.py` & `spox-0.9.0/tests/test_value_propagation.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,7 +147,14 @@
         values_int64s=[42],
         default_int64=-1,
     )
 
 
 def test_non_ascii_characters_in_string_tensor():
     op.cast(op.constant(value_string="FööBär"), to=str)
+
+
+def test_propagated_value_does_not_alias_dtype():
+    # Ensures that platform-dependent dtypes aren't accidentally propagated
+    x = numpy.iinfo(numpy.int64).max + 1
+    # Without the explicit astype(uint64), x actually ends up being ulonglong
+    assert_equal_value(op.const(x), numpy.array(x).astype(numpy.uint64))
```

### Comparing `spox-0.8.0/tests/type_inference/test_array_feature_extractor.py` & `spox-0.9.0/tests/type_inference/test_array_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/type_inference/test_compress.py` & `spox-0.9.0/tests/type_inference/test_compress.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/type_inference/test_imputer.py` & `spox-0.9.0/tests/type_inference/test_imputer.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/type_inference/test_label_encoder.py` & `spox-0.9.0/tests/type_inference/test_label_encoder.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/type_inference/test_linear_regressor.py` & `spox-0.9.0/tests/type_inference/test_linear_regressor.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/type_inference/test_one_hot.py` & `spox-0.9.0/tests/type_inference/test_one_hot.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/type_inference/test_one_hot_encoder.py` & `spox-0.9.0/tests/type_inference/test_one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/type_inference/test_scaler.py` & `spox-0.9.0/tests/type_inference/test_scaler.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tests/type_inference/test_tree_ensemble_classifier.py` & `spox-0.9.0/tests/type_inference/test_tree_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/generate_opset.py` & `spox-0.9.0/tools/generate_opset.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     onnx.AttributeProto.TYPE_PROTOS: "AttrTypes",
 }
 
 IF16_OUT_VARIADIC_SOLUTION = "len(_else_branch_subgraph.requested_results)"
 LOOP16_OUT_VARIADIC_SOLUTION = "len(_body_subgraph.requested_results) - 1"
 SCAN16_OUT_VARIADIC_SOLUTION = "len(_body_subgraph.requested_results)"
 SEQUENCEMAP17_OUT_VARIADIC_SOLUTION = "len(_body_subgraph.requested_results)"
+SPLIT18_OUT_VARIADIC_SOLUTION = "num_outputs"
 
 IF16_SUBGRAPH_SOLUTION = {"else_branch": "()", "then_branch": "()"}
 LOOP16_SUBGRAPH_SOLUTION = {
     "body": "typing_cast(List[Type], [Tensor(np.int64, (1,)), Tensor(np.bool_, (1,))])"
     "+ [var.unwrap_type() for var in v_initial]"
 }
 SCAN16_SUBGRAPH_SOLUTION = {
@@ -82,25 +83,30 @@
 
 V16_OUT_VARIADIC_SOLUTIONS = {
     "If": IF16_OUT_VARIADIC_SOLUTION,
     "Loop": LOOP16_OUT_VARIADIC_SOLUTION,
     "Scan": SCAN16_OUT_VARIADIC_SOLUTION,
     "SequenceMap": SEQUENCEMAP17_OUT_VARIADIC_SOLUTION,
 }
+V18_OUT_VARIADIC_SOLUTIONS = {
+    **V16_OUT_VARIADIC_SOLUTIONS,
+    "Split": SPLIT18_OUT_VARIADIC_SOLUTION,
+}
 V16_SUBGRAPH_SOLUTIONS = {
     "If": IF16_SUBGRAPH_SOLUTION,
     "Loop": LOOP16_SUBGRAPH_SOLUTION,
     "Scan": SCAN16_SUBGRAPH_SOLUTION,
     "SequenceMap": SEQUENCEMAP17_SUBGRAPH_SOLUTION,
 }
 DEFAULT_ATTR_TYPE_OVERRIDES = [
     (None, "dtype", ("npt.DTypeLike", "AttrDtype")),
     ("Cast", "to", ("npt.DTypeLike", "AttrDtype")),
     ("If", "then_branch", ("Callable[[], Iterable[Var]]", "AttrGraph")),
     ("If", "else_branch", ("Callable[[], Iterable[Var]]", "AttrGraph")),
+    ("Split", "num_outputs", ("int", "AttrInt64")),
 ]
 
 _TEMPLATE_DIR = Path(__file__).parent / "templates/"
 
 
 @dataclass
 class Attribute:
@@ -242,23 +248,27 @@
     return "Var"
 
 
 _PANDOC_SEP = "\U0001f6a7"  # U+1F6A7 CONSTRUCTION SIGN
 _PANDOC_GFM_TO_RST_CACHE: Dict[str, str] = {}
 
 
+def _pandoc_run(text: str):
+    return subprocess.run(
+        ["pandoc", "--from=gfm", "--to=rst"], input=text.encode(), capture_output=True
+    ).stdout.decode()
+
+
 def _pandoc_gfm_to_rst_run(*args: str) -> Tuple[str, ...]:
     if not args:
         return ()
 
-    import pandoc
-
     sep = f"\n\n{_PANDOC_SEP}{_PANDOC_SEP}\n\n"
     acc = sep.join([_PANDOC_SEP] + list(args) + [_PANDOC_SEP])
-    acc_results = pandoc.write(pandoc.read(acc, format="gfm"), format="rst")
+    acc_results = _pandoc_run(acc)
     _, *results, _ = acc_results.split(sep)
     for arg, result in zip(args, results):
         if _PANDOC_SEP in result:
             raise ValueError(
                 f"Pandoc separator character '{_PANDOC_SEP}' found in a result (bad convert)."
             )
         _PANDOC_GFM_TO_RST_CACHE[arg] = result + "\n"
@@ -655,21 +665,32 @@
     )
     ai_onnx_v18_schemas, ai_onnx_v18_module = main(
         "ai.onnx",
         18,
         extras=["const"],
         type_inference={"Compress": "compress11"},
         value_propagation={"Constant": "constant13"},
-        out_variadic_solutions=V16_OUT_VARIADIC_SOLUTIONS,
+        out_variadic_solutions=V18_OUT_VARIADIC_SOLUTIONS,
         subgraphs_solutions=V16_SUBGRAPH_SOLUTIONS,
         attr_type_overrides=DEFAULT_ATTR_TYPE_OVERRIDES,
-        allow_extra_constructor_arguments=["Split"],
         gen_docstrings=gen_all_docstrings,
         inherited_schemas={s: ai_onnx_v17_module for s in ai_onnx_v17_schemas},
     )
+    ai_onnx_v19_schemas, ai_onnx_v19_module = main(
+        "ai.onnx",
+        19,
+        extras=["const"],
+        type_inference={"Compress": "compress11"},
+        value_propagation={"Constant": "constant13"},
+        out_variadic_solutions=V18_OUT_VARIADIC_SOLUTIONS,
+        subgraphs_solutions=V16_SUBGRAPH_SOLUTIONS,
+        attr_type_overrides=DEFAULT_ATTR_TYPE_OVERRIDES,
+        gen_docstrings=gen_all_docstrings,
+        inherited_schemas={s: ai_onnx_v18_module for s in ai_onnx_v18_schemas},
+    )
     ai_onnx_ml_v3_schemas, ai_onnx_ml_v3_module = main(
         "ai.onnx.ml",
         3,
         attr_type_overrides=[(None, "dtype", ("npt.DTypeLike", "AttrDtype"))],
         type_inference={
             "ArrayFeatureExtractor": "arrayfeatureextractor1",
             "Binarizer": "binarizer1",
```

### Comparing `spox-0.8.0/tools/templates/class.jinja2` & `spox-0.9.0/tools/templates/class.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/templates/construct.jinja2` & `spox-0.9.0/tools/templates/construct.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/templates/constructor.jinja2` & `spox-0.9.0/tools/templates/constructor.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/templates/docstring.jinja2` & `spox-0.9.0/tools/templates/docstring.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 {{ schema.doc.strip() | format_github_markdown }}
 {% set type_vars = {} %}
 {% if schema.inputs or schema.attributes %}
 
 Parameters
 ==========
 {% for param in schema.inputs %}
-    {% if param.typeStr[0] is upper %}
-        {% do type_vars.update({param.typeStr: param.types}) %}
+    {% if param.type_str[0] is upper %}
+        {% do type_vars.update({param.type_str: param.types}) %}
     {% endif %}
 {{ param.name }}
 {% filter indent(width=4) %}
-    Type {{ param.typeStr }}.
+    Type {{ param.type_str }}.
 {{ param.description | format_github_markdown }}
 {% endfilter %}
 {% endfor %}
 {% for attr in schema.attributes.values() %}
 {{ attr.name }}
 {% filter indent(width=4) %}
     Attribute.
@@ -35,25 +35,25 @@
 {% endfor %}
 {% endif %}
 {% if schema.outputs %}
 
 Returns
 =======
 {% for param in schema.outputs %}
-    {% if param.typeStr[0] is upper %}
-        {% do type_vars.update({param.typeStr: param.types}) %}
+    {% if param.type_str[0] is upper %}
+        {% do type_vars.update({param.type_str: param.types}) %}
     {% endif %}
 {{ param.name }} : {%
        if is_variadic(param) %}
 Sequence[Var]
     {% else %}
 Var
     {% endif %}
 {% filter indent(width=4) %}
-    Type {{ param.typeStr }}.
+    Type {{ param.type_str }}.
 {{ param.description | format_github_markdown }}
 {% endfilter %}
 {% endfor %}
 {% endif %}
 
 Notes
 =====
```

### Comparing `spox-0.8.0/tools/templates/extras/promote.jinja2` & `spox-0.9.0/tools/templates/extras/promote.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/templates/extras/xif.jinja2` & `spox-0.9.0/tools/templates/extras/xif.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/templates/extras/xloop.jinja2` & `spox-0.9.0/tools/templates/extras/xloop.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/templates/preamble.jinja2` & `spox-0.9.0/tools/templates/preamble.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/templates/type_inference/arrayfeatureextractor1.jinja2` & `spox-0.9.0/tools/templates/type_inference/arrayfeatureextractor1.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/templates/type_inference/compress11.jinja2` & `spox-0.9.0/tools/templates/type_inference/compress11.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/templates/type_inference/if16.jinja2` & `spox-0.9.0/tools/templates/type_inference/if16.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/templates/type_inference/imputer1.jinja2` & `spox-0.9.0/tools/templates/type_inference/imputer1.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/templates/type_inference/loop16.jinja2` & `spox-0.9.0/tools/templates/type_inference/loop16.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/templates/type_inference/onehot11.jinja2` & `spox-0.9.0/tools/templates/type_inference/onehot11.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/templates/type_inference/scaler1.jinja2` & `spox-0.9.0/tools/templates/type_inference/scaler1.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/templates/type_inference/treeensembleclassifier3.jinja2` & `spox-0.9.0/tools/templates/type_inference/treeensembleclassifier3.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.8.0/tools/templates/value_propagation/constant13.jinja2` & `spox-0.9.0/tools/templates/value_propagation/constant13.jinja2`

 * *Files identical despite different names*


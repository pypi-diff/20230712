# Comparing `tmp/canals-0.2.2.tar.gz` & `tmp/canals-0.3.1.tar.gz`

## Comparing `canals-0.2.2.tar` & `canals-0.3.1.tar`

### file list

```diff
@@ -1,64 +1,78 @@
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.2.2/mkdocs.yml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.2.2/.github/workflows/api-docs.yml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.2.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 canals-0.2.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 canals-0.2.2/canals/__about__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 canals-0.2.2/canals/__init__.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 canals-0.2.2/canals/errors.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 canals-0.2.2/canals/component/__init__.py
--rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 canals-0.2.2/canals/component/component.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 canals-0.2.2/canals/component/decorators.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 canals-0.2.2/canals/component/input_output.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 canals-0.2.2/canals/draw/__init__.py
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 canals-0.2.2/canals/draw/draw.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 canals-0.2.2/canals/draw/graphviz.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 canals-0.2.2/canals/draw/mermaid.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 canals-0.2.2/canals/pipeline/__init__.py
--rw-r--r--   0        0        0    29425 2020-02-02 00:00:00.000000 canals-0.2.2/canals/pipeline/pipeline.py
--rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 canals-0.2.2/canals/pipeline/save_load.py
--rw-r--r--   0        0        0     9439 2020-02-02 00:00:00.000000 canals-0.2.2/canals/pipeline/sockets.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.2.2/canals/testing/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 canals-0.2.2/canals/testing/test_component.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.2.2/docs/index.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 canals-0.2.2/docs/api-docs/component.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.2/docs/api-docs/draw.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.2.2/docs/api-docs/pipeline.md
--rw-r--r--   0        0        0     9353 2020-02-02 00:00:00.000000 canals-0.2.2/docs/concepts/components.md
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 canals-0.2.2/docs/concepts/concepts.md
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 canals-0.2.2/docs/concepts/pipelines.md
--rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.2.2/images/canals-logo-dark.png
--rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.2.2/images/canals-logo-light.png
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.2/test/__init__.py
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 canals-0.2.2/test/test_save_load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/__init__.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_complex_pipeline.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_fixed_decision_pipeline.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_fixed_merging_pipeline.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_linear_pipeline.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_looping_and_merge_pipeline.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_looping_pipeline.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_parallel_branches_pipeline.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_variable_decision_pipeline.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_variable_merging_pipeline.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/unit/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/__init__.py
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_accumulate.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_add_value.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_double.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_greet.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_merge_loop.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_parity.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_remainder.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_repeat.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_subtract.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_sum.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_threshold.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 canals-0.2.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.2.2/LICENSE
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 canals-0.2.2/README.md
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 canals-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 canals-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.3.1/mkdocs.yml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.3.1/.github/workflows/api-docs.yml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.3.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 canals-0.3.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 canals-0.3.1/canals/__about__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 canals-0.3.1/canals/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 canals-0.3.1/canals/errors.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.3.1/canals/component/__init__.py
+-rw-r--r--   0        0        0    14157 2020-02-02 00:00:00.000000 canals-0.3.1/canals/component/component.py
+-rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 canals-0.3.1/canals/component/input_output.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 canals-0.3.1/canals/draw/__init__.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 canals-0.3.1/canals/draw/draw.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 canals-0.3.1/canals/draw/graphviz.py
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 canals-0.3.1/canals/draw/mermaid.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 canals-0.3.1/canals/pipeline/__init__.py
+-rw-r--r--   0        0        0     7872 2020-02-02 00:00:00.000000 canals-0.3.1/canals/pipeline/connections.py
+-rw-r--r--   0        0        0    31560 2020-02-02 00:00:00.000000 canals-0.3.1/canals/pipeline/pipeline.py
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 canals-0.3.1/canals/pipeline/save_load.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 canals-0.3.1/canals/pipeline/sockets.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 canals-0.3.1/canals/pipeline/validation.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.3.1/canals/testing/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 canals-0.3.1/canals/testing/test_component.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.3.1/docs/index.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 canals-0.3.1/docs/api-docs/component.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.1/docs/api-docs/draw.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.3.1/docs/api-docs/pipeline.md
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 canals-0.3.1/docs/concepts/components.md
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 canals-0.3.1/docs/concepts/concepts.md
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 canals-0.3.1/docs/concepts/pipelines.md
+-rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.3.1/images/canals-logo-dark.png
+-rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.3.1/images/canals-logo-light.png
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.1/test/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 canals-0.3.1/test/_helpers.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 canals-0.3.1/test/conftest.py
+-rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 canals-0.3.1/test/test_save_load.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 canals-0.3.1/test/component/test_component.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/__init__.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_complex_pipeline.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_double_loop_pipeline.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_fixed_decision_pipeline.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_fixed_merging_pipeline.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_linear_pipeline.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_looping_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_looping_pipeline.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_parallel_branches_pipeline.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_variable_decision_pipeline.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_variable_merging_pipeline.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/unit/__init__.py
+-rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/unit/test_connections.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/unit/test_draw.py
+-rw-r--r--   0        0        0     8999 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/unit/test_input_sockets.py
+-rw-r--r--   0        0        0     9130 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/unit/test_output_sockets.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/unit/test_pipeline.py
+-rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/unit/test_validation_pipeline_io.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/__init__.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_accumulate.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_add_value.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_concatenate.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_double.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_greet.py
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_merge_loop.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_parity.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_remainder.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_repeat.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_subtract.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_sum.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_threshold.py
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 canals-0.3.1/test/test_files/mermaid_mock/test_response.png
+-rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 canals-0.3.1/test/test_files/pipeline_draw/pygraphviz.jpg
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 canals-0.3.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 canals-0.3.1/README.md
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 canals-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 canals-0.3.1/PKG-INFO
```

### Comparing `canals-0.2.2/.pre-commit-config.yaml` & `canals-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `canals-0.2.2/mkdocs.yml` & `canals-0.3.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `canals-0.2.2/canals/component/component.py` & `canals-0.3.1/canals/component/component.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,120 +1,137 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import inspect
+from typing import Protocol, Union, List, Any, get_origin, get_args
+from dataclasses import fields, Field
+from functools import wraps
 
 from canals.errors import ComponentError
-from canals.component.decorators import save_init_params, init_defaults
+from canals.component.input_output import Connection, _input, _output
 
 
 logger = logging.getLogger(__name__)
 
 
-def component(class_):
+# We ignore too-few-public-methods Pylint error as this is only meant to be
+# the definition of the Component interface.
+# A concrete Component will have more than method in any case.
+class Component(Protocol):  # pylint: disable=too-few-public-methods
     """
-    Marks a class as a component. Any class decorated with `@component` can be used by a Pipeline.
+    Abstract interface of a Component.
+    This is only used by type checking tools.
 
-    All components must follow the contract below. This docstring is the source of truth for components contract.
+    If you want to create a new Component use the @component decorator.
+    """
 
-    ### `@component` decorator
+    def run(self, data: Any) -> Any:
+        """
+        Takes the Component input and returns its output.
+        Input and output dataclasses types must be defined in separate methods
+        decorated with @component.input and @component.output respectively.
 
-    All component classes must be decorated with the `@component` decorator. This allows Canals to discover them.
+        We use Any both as data and return types since dataclasses don't have a specific type.
+        """
 
-    ### `Input`
+    @property
+    def __canals_input__(self) -> type:
+        pass
 
-    ```python
-    @dataclass
-    class Input(ComponentInput / VariadicComponentInput):
-        <expected input fields, typed, with no defaults>
-    ```
-    Semi-mandatory method (either this or `self.input_type(self)`).
+    @property
+    def __canals_output__(self) -> type:
+        pass
 
-    This inner class defines how the input of this component looks like. For example, if the node is expecting
-    a list of Documents, the fields of the class should be `documents: List[Document]`
+    @property
+    def __canals_optional_inputs__(self) -> List[str]:
+        pass
 
-    Defaults are allowed, however `Optional`, `Union` and similar "generic" types are not. This is necessary to allow
-    proper validation of the connections, which rely on the type of these fields.
+    @property
+    def __canals_mandatory_inputs__(self) -> List[str]:
+        pass
 
-    If your node expects variadic input, use `VariadicComponentInput`. In all other scenarios, use `ComponentInput`
-    as your base class.
 
-    Some components may need more dynamic input. For these scenarios, refer to `self.input_type()`.
+class _Component:
+    """
+    Marks a class as a component. Any class decorated with `@component` can be used by a Pipeline.
 
-    Every component should define **either** `Input` or `self.input_type()`.
+    All components must follow the contract below. This docstring is the source of truth for components contract.
 
+    ### `@component` decorator
 
-    ### `input_type()`
+    All component classes must be decorated with the `@component` decorator. This allows Canals to discover them.
 
-    ```python
-    @property
-    def input_type(self) -> ComponentInput / VariadicComponentInput:
-    ```
-    Semi-mandatory method (either this or `class Input`).
+    ### `@component.input`
 
-    This method defines how the input of this component looks like. For example, if the node is expecting
-    a list of Documents, this method should return a dataclass, subclass of either `ComponentInput` or
-    `VariadicComponentInput`, with such fields. For example, it could build the dataclass as
-    `make_dataclass("Input", fields=[(f"documents", List[Document], None)], bases=(ComponentInput, ))` and return it.
+    All components must decorate one single method with the `@component.input` decorator. This method must return a
+    dataclass, which will be used as structure of the input of the component.
 
-    Defaults are allowed, however `Optional`, `Union` and similar "generic" types are not. This is necessary to allow
-    proper validation of the connections, which rely on the type of these fields.
+    For example, if the node is expecting a list of Documents, the fields of the returned dataclass should be
+    `documents: List[Document]`. Note that you don't need to decorate the dataclass youself: `@component.input` will
+    add the decorator for you.
 
-    Normally the `Input` dataclass is preferred, as it provides autocompletion for the users and is much easier to use.
+    Here is an example of such method:
 
-    Every component should define **either** `Input` or `self.input_type()`.
+    ```python
+    @component.input
+    def input(self):
+        class Input:
+            value: int
+            add: int
 
+        return Input
+    ```
+
+    Defaults are allowed, as much as default factories and other dataclass properties.
 
-    ### `Output`
+    By default `@component.input` sets `None` as default for all fields, regardless of their definition: this gives you
+    the possibility of passing a part of the input to the pipeline without defining every field of the component.
+    For example, using the above definition, you can create an Input dataclass as:
 
     ```python
-    @dataclass
-    class Output(ComponentOutput):
-        <expected output fields, typed>
+    self.input(add=3)
     ```
-    Semi-mandatory method (either this or `self.output_type()`).
-
-    This inner class defines how the output of this component looks like. For example, if the node is producing
-    a list of Documents, the fields of the class should be `documents: List[Document]`
 
-    Defaults are allowed, however `Optional`, `Union` and similar "generic" types are not. This is necessary to allow
-    proper validation of the connections, which rely on the type of these fields.
+    and the resulting dataclass will look like `Input(value=None, add=3)`.
 
-    Some components may need more dynamic output: for example, your component accepts a list of file extensions at
-    init time and wants to have one output field for each of those. For these scenarios, refer to `self.output_type()`.
+    However, if you don't explicitly define them as Optionals, Pipeline will make sure to collect all the values of
+    this dataclass before calling the `run()` method, making them in practice non-optional.
 
-    Every component should define **either** `Output` or `self.output_type()`.
+    If you instead define a specific field as Optional in the dataclass, then Pipeline will **not** wait for them, and
+    will run the component as soon as all the non-optional fields have received a value or, if all fields are optional,
+    if at least one of them received it.
 
+    This behavior allows Canals to define loops by not waiting on both incoming inputs of the entry component of the
+    loop, and instead running as soon as at least one of them receives a value.
 
-    ### `output_type()`
+    ### `@component.output`
 
-    ```python
-    @property
-    def output_type(self) -> ComponentOutput:
-    ```
-    Semi-mandatory method (either this or `class Output`).
+    All components must decorate one single method with the `@component.output` decorator. This method must return a
+    dataclass, which will be used as structure of the output of the component.
 
-    This method defines how the output of this component looks like. For example, if the node is producing
-    a list of Documents, this method should return a dataclass with such fields, for example:
-    `return make_dataclass("Output", fields=[(f"documents", List[Document], None)], bases=(ComponentOutput, ))`
+    For example, if the node is producing a list of Documents, the fields of the returned dataclass should be
+    `documents: List[Document]`. Note that you don't need to decorate the dataclass youself: `@component.output` will
+    add the decorator for you.
 
-    Defaults are allowed, however `Optional`, `Union` and similar "generic" types are not. This is necessary to allow
-    proper validation of the connections, which rely on the type of these fields.
+    Here is an example of such method:
 
-    If the output is static, normally the `Output` dataclass is preferred, as it provides autocompletion for the users.
+    ```python
+    @component.output
+    def output(self):
+        class Output:
+            value: int
 
-    Every component should define **either** `Output` or `self.output_type`.
+        return Output
+    ```
 
+    Defaults are allowed, as much as default factories and other dataclass properties.
 
-    ### `__init__()`
+    ### `__init__(self, **kwargs)`
 
-    ```python
-    def __init__(self, [... components init parameters ...]):
-    ```
     Optional method.
 
     Components may have an `__init__` method where they define:
 
     - `self.defaults = {parameter_name: parameter_default_value, ...}`:
         All values defined here will be sent to the `run()` method when the Pipeline calls it.
         If any of these parameters is also receiving input from other components, those have precedence.
@@ -136,97 +153,213 @@
     _(TODO explain how to use classes and functions in init. In the meantime see `test/components/test_accumulate.py`)_
 
     The `__init__` must be extrememly lightweight, because it's a frequent operation during the construction and
     validation of the pipeline. If a component has some heavy state to initialize (models, backends, etc...) refer to
     the `warm_up()` method.
 
 
-    ### `warm_up()`
+    ### `warm_up(self)`
 
-    ```python
-    def warm_up(self):
-    ```
     Optional method.
 
     This method is called by Pipeline before the graph execution. Make sure to avoid double-initializations,
     because Pipeline will not keep track of which components it called `warm_up()` on.
 
 
-    ### `run()`
+    ### `run(self, data)`
 
-    ```python
-    def run(self, data: <Input if defined, otherwise untyped>) -> <Output if defined, otherwise untyped>:
-    ```
     Mandatory method.
 
     This is the method where the main functionality of the component should be carried out. It's called by
     `Pipeline.run()`.
 
-    When the component should run, Pipeline will call this method with:
+    When the component should run, Pipeline will call this method with an instance of the dataclass returned by the
+    method decorated with `@component.input`. This dataclass contains:
 
     - all the input values coming from other components connected to it,
     - if any is missing, the corresponding value defined in `self.defaults`, if it exists.
 
-    `run()` must return a single instance of the dataclass declared through either `Output` or `self.output_type()`.
+    `run()` must return a single instance of the dataclass declared through the method decorated with
+    `@component.output`.
 
     Args:
         class_: the class that Canals should use as a component.
         serializable: whether to check, at init time, if the component can be saved with
         `save_pipelines()`.
 
     Returns:
         A class that can be recognized as a component.
 
     Raises:
         ComponentError: if the class provided has no `run()` method or otherwise doesn't respect the component contract.
     """
-    logger.debug("Registering %s as a component", class_)
 
-    # '__canals_component__' is used to distinguish components from regular classes.
-    # Its value is set to the desired component name: normally it is the class name, but it can technically be customized.
-    class_.__canals_component__ = class_.__name__
-
-    # Check for Input
-    if not hasattr(class_, "Input") and not hasattr(class_, "input_type"):
-        raise ComponentError(
-            "Components must either have an Input dataclass or a 'input_type' property that returns such dataclass"
-        )
-    if hasattr(class_, "Input") and not hasattr(class_.Input, "_component_input"):
-        raise ComponentError(f"{class_.__name__}.Input must inherit from ComponentInput")
-
-    # Check for Output
-    if not hasattr(class_, "Output") and not hasattr(class_, "output_type"):
-        raise ComponentError(
-            "Components must either have an Output dataclass or a 'output_type' property that returns such dataclass"
-        )
-    if hasattr(class_, "Output") and not hasattr(class_.Output, "_component_output"):
-        raise ComponentError(f"{class_.__name__}.Output must inherit from ComponentOutput")
+    def __init__(self):
+        self.registry = {}
+
+    @property
+    def input(self):
+        """
+        TODO: Documentation
+        """
+        return _input
+
+    @property
+    def output(self):
+        """
+        TODO: Documentation
+        """
+        return _output
+
+    def _decorate(self, class_):
+        # '__canals_component__' is used to distinguish components from regular classes.
+        # Its value is set to the desired component name: normally it is the class name, but it can technically be customized.
+        class_.__canals_component__ = class_.__name__
+
+        # Find input and output properties
+        (input_, output) = _find_input_output(class_)
+
+        # Save the input and output properties so it's easier to find them when running the Component since we won't
+        # need to search the exact property name each time
+        class_.__canals_input__ = input_
+        class_.__canals_output__ = output
+
+        # Save optional inputs, optionals inputs are those fields for the __canals_input__ dataclass
+        # that have an Optional type.
+        # Those are necessary to implement Components that can run with partial input, this gives us
+        # the possibility to have cycles in Pipelines.
+        class_.__canals_optional_inputs__ = property(_optional_inputs)
+        class_.__canals_mandatory_inputs__ = property(_mandatory_inputs)
+
+        # Check that the run method respects all constraints
+        _check_run_signature(class_)
+
+        # Makes sure the self.defaults and self.init_parameters dictionaries are always present
+        class_.init_parameters = {}
+        class_.defaults = {}
+
+        # Automatically registers all the init parameters in an instance attribute called `init_parameters`.
+        class_.__init__ = _save_init_params(class_.__init__)
+
+        if class_.__name__ in self.registry:
+            logger.error(
+                "Component %s is already registered. Previous imported from '%s', new imported from '%s'",
+                class_.__name__,
+                self.registry[class_.__name__],
+                class_,
+            )
+
+        self.registry[class_.__name__] = class_
+        logger.debug("Registered Component %s", class_)
+
+        return class_
+
+    def __call__(self, class_=None):
+        if class_:
+            return self._decorate(class_)
+
+        return self._decorate
+
+
+component = _Component()
+
+
+def _find_input_output(class_):
+    """
+    Finds the input and the output definitions for class_ and returns them.
+
+    There must be only a single definition of input and output for class_, if either
+    none or more than one are found raise ConnectionError.
+    """
+    inputs_found = []
+    outputs_found = []
+
+    # Get all properties of class_
+    properties = inspect.getmembers(class_, predicate=lambda m: isinstance(m, property))
+    for _, prop in properties:
+        if not hasattr(prop, "fget") and not hasattr(prop.fget, "__canals_connection__"):
+            continue
+
+        # Field __canals_connection__ is set by _input and _output decorators
+        if prop.fget.__canals_connection__ == Connection.INPUT:
+            inputs_found.append(prop)
+        elif prop.fget.__canals_connection__ == Connection.OUTPUT:
+            outputs_found.append(prop)
+
+    if (in_len := len(inputs_found)) != 1:
+        # Raise if we don't find only a single input definition
+        if in_len == 0:
+            raise ComponentError(
+                f"No input definition found in Component {class_.__name__}. "
+                "Create a method that returns a dataclass defining the input and "
+                "decorate it with @component.input() to fix the error."
+            )
+        raise ComponentError(f"Multiple input definitions found for Component {class_.__name__}.")
+
+    if (in_len := len(outputs_found)) != 1:
+        # Raise if we don't find only a single output definition
+        if in_len == 0:
+            raise ComponentError(
+                f"No output definition found in Component {class_.__name__}. "
+                "Create a method that returns a dataclass defining the output and "
+                "decorate it with @component.output() to fix the error."
+            )
+        raise ComponentError(f"Multiple output definitions found for Component {class_.__name__}.")
+
+    return (inputs_found[0], outputs_found[0])
 
+
+def _check_run_signature(class_):
+    """
+    Check that the component's run() method exists and respects all constraints
+    """
     # Check for run()
     if not hasattr(class_, "run"):
         raise ComponentError(f"{class_.__name__} must have a 'run()' method. See the docs for more information.")
     run_signature = inspect.signature(class_.run)
 
     # run() must take a single input param
     if len(run_signature.parameters) != 2:
         raise ComponentError("run() must accept only a single parameter called 'data'.")
 
     # The input param must be called data
     if not "data" in run_signature.parameters:
         raise ComponentError("run() must accept a parameter called 'data'.")
 
-    # Either give a self.input_type function or type 'data' with the Input dataclass
-    if not hasattr(class_, "input_type") and run_signature.parameters["data"].annotation != class_.Input:
-        raise ComponentError(f"'data' must be typed and the type must be {class_.__name__}.Input.")
-
-    # Check for the return types
-    if not hasattr(class_, "output_type") and run_signature.return_annotation == inspect.Parameter.empty:
-        raise ComponentError(f"{class_.__name__}.run() must declare the type of its return value.")
-
-    # Automatically registers all the init parameters in an instance attribute called `init_parameters`.
-    # See `save_init_params()`.
-    class_.__init__ = save_init_params(class_.__init__)
 
-    # Makes sure the self.defaults dictionary is always present
-    class_.__init__ = init_defaults(class_.__init__)
+def _is_optional(field: Field) -> bool:
+    """
+    Utility method that returns whether a field has an Optional type or not.
+    """
+    return get_origin(field.type) is Union and type(None) in get_args(field.type)
+
+
+def _optional_inputs(self) -> List[str]:
+    """
+    Return all field names of self that have an Optional type.
+    This is meant to be set as a property in a Component.
+    """
+    return [f.name for f in fields(self.__canals_input__) if _is_optional(f)]
+
+
+def _mandatory_inputs(self) -> List[str]:
+    """
+    Return all field names of self that don't have an Optional type.
+    This is meant to be set as a property in a Component.
+    """
+    return [f.name for f in fields(self.__canals_input__) if not _is_optional(f)]
+
+
+def _save_init_params(init_func):
+    """
+    Decorator that saves the init parameters of a component in `self.init_parameters`
+    """
+
+    @wraps(init_func)
+    def wrapper(self, *args, **kwargs):
+        # Call the actual __init__ function with the arguments
+        init_func(self, *args, **kwargs)
+
+        # Collect and store all the init parameters, preserving whatever the components might have already added there
+        self.init_parameters = {**kwargs, **self.init_parameters}
 
-    return class_
+    return wrapper
```

### Comparing `canals-0.2.2/canals/draw/draw.py` & `canals-0.3.1/canals/draw/draw.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Literal, Optional, Dict, get_args, Any
 
 import logging
 from pathlib import Path
 
 import networkx
 
-from canals.pipeline.sockets import find_pipeline_inputs, find_pipeline_outputs
+from canals.pipeline.validation import find_pipeline_inputs, find_pipeline_outputs
 from canals.draw.graphviz import to_agraph
 from canals.draw.mermaid import to_mermaid_image, to_mermaid_text
 
 
 logger = logging.getLogger(__name__)
 RenderingEngines = Literal["graphviz", "mermaid-img", "mermaid-text"]
 
@@ -92,16 +92,18 @@
         graph.add_edge(inp, outp, key=key, **data)
 
     # Draw the inputs
     graph.add_node("input")
     for node, in_sockets in find_pipeline_inputs(graph).items():
         for in_socket in in_sockets:
             node_instance = graph.nodes[node]["instance"]
-            input_node_defaults = hasattr(node_instance, "defaults") and in_socket.name in node_instance.defaults
-            if not input_node_defaults and not (graph.nodes[node]["variadic_input"] and not graph.in_edges(node)):
+            socket_has_default = in_socket.name in node_instance.defaults
+            if not socket_has_default and in_socket.sender is None:
+                # If this socket has no defaults and no other component sends anything to it
+                # it must be a socket that receives input directly when running the Pipeline
                 graph.add_edge("input", node, label=in_socket.name)
 
     # Draw the outputs
     graph.add_node("output")
     for node, out_sockets in find_pipeline_outputs(graph).items():
         for out_socket in out_sockets:
             graph.add_edge(node, "output", label=out_socket.name)
```

### Comparing `canals-0.2.2/canals/draw/graphviz.py` & `canals-0.3.1/canals/draw/graphviz.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,31 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 import logging
 
 import networkx
+
 from networkx.drawing.nx_agraph import to_agraph as nx_to_agraph
 
-logger = logging.getLogger(__name__)
 
-try:
-    from pygraphviz import AGraph
-except ImportError:
-    logger.debug(
-        "Could not import `pygraphviz`. Please install via: \n"
-        "pip install pygraphviz\n"
-        "(You might need to run this first: apt install libgraphviz-dev graphviz )"
-    )
-    AGraph = None
+logger = logging.getLogger(__name__)
 
 
-def to_agraph(graph: networkx.MultiDiGraph) -> AGraph:
+def to_agraph(graph: networkx.MultiDiGraph):
     """
     Renders a pipeline graph using PyGraphViz. You need to install it and all its system dependencies for it to work.
     """
-    if not AGraph:
+    try:
+        import pygraphviz  # pylint: disable=unused-import,import-outside-toplevel
+    except (ModuleNotFoundError, ImportError) as exc:
         raise ImportError(
-            "Could not import `pygraphviz`. Please install via: \n"
-            "pip install pygraphviz\n"
-            "(You might need to run this first: apt install libgraphviz-dev graphviz )"
-        )
-
-    for node in graph.nodes:
-        if graph.nodes[node].get("style") == "running":
-            graph.nodes[node]["color"] = "red"
-            graph.nodes[node]["penwidth"] = 3
-
-        if graph.nodes[node].get("style") == "queued":
-            graph.nodes[node]["color"] = "#0f0"
-            graph.nodes[node]["penwidth"] = 3
+            "Can't use 'pygraphviz' to draw this pipeline: pygraphviz could not be imported. "
+            "Make sure pygraphviz is installed and all its system dependencies are setup correctly."
+        ) from exc
 
     for inp, outp, key, data in graph.out_edges("input", keys=True, data=True):
         data["style"] = "dashed"
         graph.add_edge(inp, outp, key=key, **data)
 
     for inp, outp, key, data in graph.in_edges("output", keys=True, data=True):
         data["style"] = "dashed"
```

### Comparing `canals-0.2.2/canals/draw/mermaid.py` & `canals-0.3.1/canals/draw/mermaid.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import base64
 
 import requests
 import networkx
 
+from canals.errors import PipelineDrawingError
+
 
 logger = logging.getLogger(__name__)
 
 
 MERMAID_STYLED_TEMPLATE = """
 %%{{ init: {{'theme': 'neutral' }} }}%%
 
 {graph_as_text}
 
 style IN  fill:#fff,stroke:#fff,stroke-width:1px
 style OUT fill:#fff,stroke:#fff,stroke-width:1px
-classDef running fill:#fff,stroke:#f00,stroke-width:2px
-classDef queued fill:#fff,stroke:#0f0,stroke-width:2px
 linkStyle default stroke-width:2px,stroke-dasharray: 5 5;
 {solid_arrows}
 """
 
 
 def to_mermaid_image(graph: networkx.MultiDiGraph):
     """
@@ -44,20 +44,23 @@
     logging.debug("Rendeding graph at %s", url)
     try:
         resp = requests.get(url, timeout=10)
         if resp.status_code >= 400:
             logger.warning("Failed to draw the pipeline: https://mermaid.ink/img/ returned status %s", resp.status_code)
             logger.info("Exact URL requested: %s", url)
             logger.warning("No pipeline diagram will be saved.")
-            return None
+            resp.raise_for_status()
+
     except Exception as exc:  # pylint: disable=broad-except
         logger.warning("Failed to draw the pipeline: could not connect to https://mermaid.ink/img/ (%s)", exc)
         logger.info("Exact URL requested: %s", url)
         logger.warning("No pipeline diagram will be saved.")
-        return None
+        raise PipelineDrawingError(
+            "There was an issue with https://mermaid.ink/, see the stacktrace for details."
+        ) from exc
 
     return resp.content
 
 
 def to_mermaid_text(graph: networkx.MultiDiGraph) -> str:
     """
     Converts a Networkx graph into Mermaid syntax. The output of this function can be used in the documentation
```

### Comparing `canals-0.2.2/canals/pipeline/pipeline.py` & `canals-0.3.1/canals/pipeline/pipeline.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
-from typing import Optional, Any, Dict, List, Tuple, Literal, Union
+from typing import Optional, Any, Dict, List, Literal, Union
 
 import os
 import json
 import datetime
 import logging
 from pathlib import Path
 from copy import deepcopy
 from collections import OrderedDict
+from dataclasses import fields
 
 import networkx
 
+from canals.component import Component
 from canals.errors import PipelineConnectError, PipelineMaxLoops, PipelineRuntimeError, PipelineValidationError
-from canals.component.input_output import ComponentInput
 from canals.draw import draw, convert_for_debug, RenderingEngines
-from canals.pipeline.sockets import (
-    InputSocket,
-    OutputSocket,
-    find_input_sockets,
-    find_output_sockets,
-    find_unambiguous_connection,
-    parse_connection_name,
-    validate_pipeline_input,
-)
+from canals.pipeline.sockets import InputSocket, OutputSocket, find_input_sockets, find_output_sockets
+from canals.pipeline.validation import validate_pipeline_input
+from canals.pipeline.connections import parse_connection_name, find_unambiguous_connection, get_socket_type_desc
 
 
 logger = logging.getLogger(__name__)
 
 
 class Pipeline:
     """
@@ -89,15 +84,15 @@
             if hasattr(comparable_node, "defaults"):
                 comparable_node["defaults"] = comparable_node["instance"].defaults
             comparable_node["instance"] = comparable_node["instance"].__class__
             nodes.append(comparable_node)
         nodes.sort()
         return nodes
 
-    def add_component(self, name: str, instance: Any) -> None:
+    def add_component(self, name: str, instance: Component) -> None:
         """
         Create a component for the given component. Components are not connected to anything by default:
         use `Pipeline.connect()` to connect components together.
 
         Component names must be unique, but component instances can be reused if needed.
 
         Args:
@@ -131,15 +126,14 @@
 
         # Add component to the graph, disconnected
         logger.debug("Adding component '%s' (%s)", name, instance)
         self.graph.add_node(
             name,
             instance=instance,
             input_sockets=input_sockets,
-            variadic_input=any(e.variadic for e in input_sockets.values()),
             output_sockets=output_sockets,
             visits=0,
         )
 
     def connect(self, connect_from: str, connect_to: str) -> None:
         """
         Connects two components together. All components to connect must exist in the pipeline.
@@ -177,69 +171,62 @@
         # If the name of either socket is given, get the socket
         if from_socket_name:
             from_socket = from_sockets.get(from_socket_name, None)
             if not from_socket:
                 raise PipelineConnectError(
                     f"'{from_node}.{from_socket_name} does not exist. "
                     f"Output connections of {from_node} are: "
-                    + ", ".join([f"{name} (type {socket.type.__name__})" for name, socket in from_sockets.items()])
+                    + ", ".join(
+                        [f"{name} (type {get_socket_type_desc(socket.type)})" for name, socket in from_sockets.items()]
+                    )
                 )
         if to_socket_name:
             to_socket = to_sockets.get(to_socket_name, None)
             if not to_socket:
                 raise PipelineConnectError(
                     f"'{to_node}.{to_socket_name} does not exist. "
                     f"Input connections of {to_node} are: "
-                    + ", ".join([f"{name} (type {socket.type.__name__})" for name, socket in to_sockets.items()])
+                    + ", ".join(
+                        [f"{name} (type {get_socket_type_desc(socket.type)})" for name, socket in to_sockets.items()]
+                    )
                 )
 
-        # If either one of the two sockets is not specified, look for an unambiguous connection
+        # Look for an unambiguous connection among the possible ones.
         # Note that if there is more than one possible connection but two sockets match by name, they're paired.
-        if not to_socket_name or not from_socket_name:
-            from_sockets = [from_socket] if from_socket_name else from_sockets.values()
-            to_sockets = [to_socket] if to_socket_name else to_sockets.values()
-            from_socket, to_socket = find_unambiguous_connection(
-                from_node=from_node, from_sockets=from_sockets, to_node=to_node, to_sockets=to_sockets
-            )
+        from_sockets = [from_socket] if from_socket_name else list(from_sockets.values())
+        to_sockets = [to_socket] if to_socket_name else list(to_sockets.values())
+        from_socket, to_socket = find_unambiguous_connection(
+            sender_node=from_node, sender_sockets=from_sockets, receiver_node=to_node, receiver_sockets=to_sockets
+        )
 
         # Connect the components on these sockets
         self._direct_connect(from_node=from_node, from_socket=from_socket, to_node=to_node, to_socket=to_socket)
 
     def _direct_connect(self, from_node: str, from_socket: OutputSocket, to_node: str, to_socket: InputSocket) -> None:
         """
-        Directly connect socket to socket.
+        Directly connect socket to socket. This method does not type-check the connections: use 'Pipeline.connect()'
+        instead (which uses 'find_unambiguous_connection()' to validate types).
         """
-        # Check that the types match. We need type equality: subclass relationships are not accepted, just like
-        # Optionals, Unions, and similar "aggregate" types. See https://github.com/python/typing/issues/570
-        if not from_socket.type == to_socket.type:
-            raise PipelineConnectError(
-                f"Cannot connect '{from_node}.{from_socket.name}' with '{to_node}.{to_socket.name}': "
-                f"their declared input and output types do not match.\n"
-                f" - {from_node}.{from_socket.name}: {from_socket.type.__name__}\n"
-                f" - {to_node}.{to_socket.name}: {to_socket.type.__name__}\n"
-            )
-
-        # Make sure the receiving socket is not taken - sending sockets can be connected as many times as needed,
+        # Make sure the receiving socket isn't already connected - sending sockets can be connected as many times as needed,
         # so they don't need this check
-        if to_socket.taken_by:
+        if to_socket.sender:
             raise PipelineConnectError(
                 f"Cannot connect '{from_node}.{from_socket.name}' with '{to_node}.{to_socket.name}': "
-                f"{to_node}.{to_socket.name} is already connected to {to_socket.taken_by}.\n"
+                f"{to_node}.{to_socket.name} is already connected to {to_socket.sender}.\n"
             )
 
         # Create the connection
         logger.debug("Connecting '%s.%s' to '%s.%s'", from_node, from_socket.name, to_node, to_socket.name)
         edge_key = f"{from_socket.name}/{to_socket.name}"
         self.graph.add_edge(from_node, to_node, key=edge_key, from_socket=from_socket, to_socket=to_socket)
 
-        # Mark the receiving socket as taken (unless is variadic - variadic sockets are never "taken")
-        if not to_socket.variadic:
-            to_socket.taken_by = from_node
+        # Stores the name of the node that will send its output to this socket
+        to_socket.sender = from_node
 
-    def get_component(self, name: str) -> object:
+    def get_component(self, name: str) -> Component:
         """
         Returns an instance of a component.
 
         Args:
             name: the name of the component
 
         Returns:
@@ -280,15 +267,15 @@
         without re-initializing everything.
         """
         for node in self.graph.nodes:
             if hasattr(self.graph.nodes[node]["instance"], "warm_up"):
                 logger.info("Warming up component %s...", node)
                 self.graph.nodes[node]["instance"].warm_up()
 
-    def run(self, data: Dict[str, ComponentInput], debug: bool = False) -> Dict[str, Any]:
+    def run(self, data: Dict[str, Any], debug: bool = False) -> Dict[str, Any]:
         """
         Runs the pipeline.
 
         Args:
             data: the inputs to give to the input components of the Pipeline.
             parameters: a dictionary with all the parameters of all the components, namespaced by component.
             debug: whether to collect and return debug information.
@@ -351,30 +338,41 @@
             step += 1
             if debug:
                 self._record_pipeline_step(step, inputs_buffer, pipeline_output)
             logger.debug("> Queue at step %s: %s", step, {k: list(v.keys()) for k, v in inputs_buffer.items()})
 
             component, inputs = inputs_buffer.popitem(last=False)  # FIFO
 
-            # if debug:
-            #     draw(deepcopy(self.graph), engine="graphviz", path=f"debug/step_{current_step}.jpg", running=component, queued=inputs_buffer.keys())
+            # Make sure it didn't run too many times already
+            self._check_max_loops(component)
 
             # **** IS IT MY TURN YET? ****
-            # Check if the node should be run or not
-            ready_to_run = self._ready_to_run(name=component, inputs=inputs, inputs_buffer=inputs_buffer)
+            # Check if the component should be run or not
+            action = self._calculate_action(name=component, inputs=inputs, inputs_buffer=inputs_buffer)
 
             # This component is missing data: let's put it back in the queue and wait.
-            if ready_to_run == "wait":
+            if action == "wait":
+                if not inputs_buffer:
+                    # What if there are no components to wait for?
+                    raise PipelineRuntimeError(
+                        f"'{component}' is stuck waiting for input, but there are no other components to run. "
+                        "This is likely a Canals bug. Open an issue at https://github.com/deepset-ai/canals."
+                    )
+
                 inputs_buffer[component] = inputs
                 continue
 
             # This component did not receive the input it needs: it must be on a skipped branch. Let's not run it.
-            if ready_to_run == "skip":
+            if action == "skip":
                 self.graph.nodes[component]["visits"] += 1
-                inputs_buffer = self._skip_downstream_nodes(component=component, inputs_buffer=inputs_buffer)
+                inputs_buffer = self._skip_downstream_unvisited_nodes(component=component, inputs_buffer=inputs_buffer)
+                continue
+
+            if action == "remove":
+                # This component has no reason of being in the run queue and we need to remove it. For example, this can happen to components that are connected to skipped branches of the pipeline.
                 continue
 
             # **** RUN THE NODE ****
             # It is our turn! The node is ready to run and all necessary inputs are present
             output = self._run_component(name=component, inputs=inputs)
 
             # **** PROCESS THE OUTPUT ****
@@ -425,172 +423,215 @@
         Verify whether this component run too many times.
         """
         if self.graph.nodes[component_name]["visits"] > self.max_loops_allowed:
             raise PipelineMaxLoops(
                 f"Maximum loops count ({self.max_loops_allowed}) exceeded for component '{component_name}'."
             )
 
-    def _ready_to_run(
-        self, name: str, inputs: Dict[str, Any], inputs_buffer: OrderedDict
-    ) -> Literal["run", "wait", "skip"]:
-        """
-        Verify whether a component is ready to run.
+    # This function is complex so it contains quite some logic, it needs tons of information
+    # regarding a component to understand what action it should take so we have many local
+    # variables and to keep things simple we also have multiple returns.
+    # In the end this amount of information makes it easier to understand the internal logic so
+    # we chose to ignore these pylint warnings.
+    def _calculate_action(  # pylint: disable=too-many-locals, too-many-return-statements
+        self, name: str, inputs: Dict[str, Any], inputs_buffer: Dict[str, Any]
+    ) -> Literal["run", "wait", "skip", "remove"]:
+        """
+        Calculates the action to take for the component specified by `name`.
+        There are four possible actions:
+            * run
+            * wait
+            * skip
+            * remove
+
+        The below conditions are evaluated in this order.
+
+        Component will run if at least one of the following statements is true:
+            * It received all mandatory inputs
+            * It received all mandatory inputs and it has no optional inputs
+            * It received all mandatory inputs and all optional inputs are skipped
+            * It received all mandatory inputs and some optional inputs and the rest are skipped
+            * It received some of its inputs and the others are defaulted
+            * It's the first component of the pipeline
+
+        Component will wait if:
+            * It received some of its inputs and the other are not skipped
+            * It received all mandatory inputs and some optional inputs have not been skipped
+
+        Component will be skipped if:
+            * It never ran nor waited
 
-        Returns 'run', 'wait' or 'skip' depending on how the node should be treated and the log message explaining
-        the decision.
-        """
-        # Make sure it didn't run too many times already
-        self._check_max_loops(name)
+        Component will be removed if:
+            * It ran or waited at least once but can't do it again
 
-        # List all the component/socket pairs the current component should be waiting for.
-        expected_inputs = self._connections_to_wait_for(name=name)
+        If none of the above condition is met a PipelineRuntimeError is raised.
 
-        # Check if the expected inputs were all received
-        if self._check_received_vs_expected_inputs(name=name, inputs=inputs, expected_inputs=expected_inputs):
-            return "run"
+        For simplicity sake input components that create a cycle, or components that already ran
+        and don't create a cycle are considered as skipped.
 
-        # This node is missing some inputs. Did all the upstream nodes run?
-        nodes_to_wait_for, _ = zip(*expected_inputs) if expected_inputs else ([], [])
+        Args:
+            name: Name of the component
+            inputs: Values that the component will take as input
+            inputs_buffer: Other components' inputs
 
-        # Some node upstream didn't run yet, so we should wait for them.
-        if not self._all_nodes_to_wait_for_run(nodes_to_wait_for=nodes_to_wait_for):
+        Returns:
+            Action to take for component specifing whether it should run, wait, skip or be removed
 
-            if not inputs_buffer:
-                # What if there are no components to wait for?
-                raise PipelineRuntimeError(
-                    f"'{name}' is stuck waiting for input, but there are no other components to run. "
-                    "This is likely a Canals bug. Open an issue at https://github.com/deepset-ai/canals."
+        Raises:
+            PipelineRuntimeError: If action to take can't be determined
+        """
+
+        # Upstream components/socket pairs the current component is connected to
+        input_components = {
+            from_node: data["to_socket"].name for from_node, _, data in self.graph.in_edges(name, data=True)
+        }
+        # Sockets that have received inputs from upstream components
+        received_input_sockets = set(inputs.keys())
+
+        # All components inputs, whether they're connected, default or pipeline inputs
+        instance = self.graph.nodes[name]["instance"]
+        input_sockets = {f.name for f in fields(instance.__canals_input__)}
+        optional_input_sockets = set(instance.__canals_optional_inputs__)
+        mandatory_input_sockets = set(instance.__canals_mandatory_inputs__)
+
+        # Components that are in the inputs buffer and have no inputs assigned are considered skipped
+        skipped_components = {n for n, v in inputs_buffer.items() if not v}
+
+        # Sockets that have their upstream component marked as skipped
+        skipped_optional_input_sockets = {
+            sockets["to_socket"].name
+            for from_node, _, sockets in self.graph.in_edges(name, data=True)
+            if from_node in skipped_components and sockets["to_socket"].name in optional_input_sockets
+        }
+
+        for from_node, socket in input_components.items():
+            if socket not in optional_input_sockets:
+                continue
+            loops_back = networkx.has_path(self.graph, name, from_node)
+            has_run = self.graph.nodes[from_node]["visits"] > 0
+            if loops_back or has_run:
+                # Consider all input components that loop back to current component
+                # or that have already run at least once as skipped.
+                # This must be done to correctly handle cycles in the pipeline or we
+                # would reach a dead lock in components that have multiple inputs and
+                # one of these forms a cycle.
+                skipped_optional_input_sockets.add(socket)
+
+        ##############
+        # RUN CHECKS #
+        ##############
+        if (
+            mandatory_input_sockets.issubset(received_input_sockets)
+            and input_sockets == received_input_sockets | mandatory_input_sockets | skipped_optional_input_sockets
+        ):
+            # We received all mandatory inputs and:
+            #   * There are no optional inputs or
+            #   * All optional inputs are skipped or
+            #   * We received part of the optional inputs, the rest are skipped
+            if not optional_input_sockets:
+                logger.debug("Component '%s' is ready to run. All mandatory inputs received.", name)
+            else:
+                logger.debug(
+                    "Component '%s' is ready to run. All mandatory inputs received, skipped optional inputs: %s",
+                    name,
+                    skipped_optional_input_sockets,
                 )
+            return "run"
+
+        if set(input_components.values()).issubset(received_input_sockets):
+            # We have data from each connected input component.
+            # We reach this when the current component is the first of the pipeline or
+            # when it has defaults and all its input components have run.
+            logger.debug("Component '%s' is ready to run. All expected inputs were received.", name)
+            return "run"
 
+        ###############
+        # WAIT CHECKS #
+        ###############
+        if mandatory_input_sockets == received_input_sockets and skipped_optional_input_sockets.issubset(
+            optional_input_sockets
+        ):
+            # We received all of the inputs we need, but some optional inputs have not been run or skipped yet
             logger.debug(
-                "Putting '%s' back in the queue, some inputs are missing (inputs to wait for: %s, inputs_received: %s)",
+                "Component '%s' is waiting. All mandatory inputs received, some optional are not skipped: %s",
                 name,
-                [f"{node}.{socket}" for node, socket in expected_inputs],
-                list(inputs.keys()),
+                optional_input_sockets - skipped_optional_input_sockets,
             )
             return "wait"
 
-        # All upstream nodes run, so it **must** be our turn.
-        # However we're missing data, so this branch probably is being skipped.
-        if inputs and self.graph.nodes[name]["variadic_input"]:
+        if any(self.graph.nodes[n]["visits"] == 0 for n in input_components.keys()):
+            # Some upstream component that must send input to the current component has yet to run.
             logger.debug(
-                "Running '%s', even though some upstream component did not produced output. "
-                "(upstream components: %s, expected inputs: %s, n. of inputs received %s)",
+                "Component '%s' is waiting. Missing inputs: %s",
                 name,
-                list(nodes_to_wait_for),
-                [f"{node}.{socket}" for node, socket in expected_inputs],
-                len(list(inputs.values())[0]) if inputs else 0,
+                set(input_components.values()),
             )
-            return "run"
+            return "wait"
 
-        logger.debug(
-            "Skipping '%s', upstream component didn't produce output "
-            "(upstream components: %s, expected inputs: %s, inputs received: %s)",
-            name,
-            list(nodes_to_wait_for),
-            [f"{node}.{socket}" for node, socket in expected_inputs],
-            list(inputs.keys()),
+        ###############
+        # SKIP CHECKS #
+        ###############
+        if self.graph.nodes[name]["visits"] == 0:
+            # It's the first time visiting this component, if it can't run nor wait
+            # it's fine skipping it at this point.
+            logger.debug("Component '%s' is skipped. It can't run nor wait.", name)
+            return "skip"
+
+        #################
+        # REMOVE CHECKS #
+        #################
+        if self.graph.nodes[name]["visits"] > 0:
+            # This component has already been visited at least once. If it can't run nor wait
+            # there is no reason to skip it again. So we it must be removed.
+            logger.debug("Component '%s' is removed. It can't run, wait or skip.", name)
+            return "remove"
+
+        # Can't determine action to take
+        raise PipelineRuntimeError(
+            f"Can't determine Component '{name}' action. "
+            f"Mandatory input sockets: {mandatory_input_sockets}, "
+            f"optional input sockets: {optional_input_sockets}, "
+            f"received input: {list(inputs.keys())}, "
+            f"input components: {list(input_components.keys())}, "
+            f"skipped components: {skipped_components}, "
+            f"skipped optional inputs: {skipped_optional_input_sockets}."
+            f"This is likely a Canals bug. Please open an issue at https://github.com/deepset-ai/canals.",
         )
-        return "skip"
 
-    def _check_received_vs_expected_inputs(
-        self, name: str, inputs: Dict[str, Any], expected_inputs: Tuple[str, str]
-    ) -> bool:
-        """
-        Check if all the inputs the component is expecting have been received.
-
-        Returns True if all the necessary inputs are received, False otherwise, and a message with the decision.
-        """
-        # Variadic nodes expect a single list regardless of how many incoming connections they have,
-        # but the length of the list should match the length of incoming connections.
-        if self.graph.nodes[name]["variadic_input"]:
-
-            # Variadic nodes need at least two values
-            if not inputs or len(inputs) < 2:
-                return False
-
-            if len(list(inputs.values())[0]) == len(expected_inputs):
-                logger.debug(
-                    "Component '%s' is ready to run: all connected inputs were received "
-                    "(expecting %s, received %s values).",
-                    name,
-                    len(expected_inputs),
-                    len(list(inputs.values())[0]),
-                )
-                return True
-        else:
-            # No input sockets are connected: this is an input node and should be always ready to run.
-            if not expected_inputs:
-                logger.debug("Component '%s' is ready to run: it's a starting node.", name)
-                return True
-
-            # Otherwise, just make sure there is one input key for each expected input key
-            _, expected_input_names = zip(*expected_inputs)
-            if set(expected_input_names).issubset(set(inputs.keys())):
-                logger.debug("Component '%s' is ready to run: all expected inputs were received.", name)
-                return True
-
-        return False
-
-    def _connections_to_wait_for(self, name: str):
-        """
-        Return all the component/socket pairs this component is waiting for.
-        """
-        # We should be wait on all edges except for the downstream ones, to support loops.
-        # This downstream check is enabled only for nodes taking more than one input
-        # (the "entrance" of the loop).
-        data_to_wait_for = [
-            (from_node, data["to_socket"].name)
-            for from_node, _, data in self.graph.in_edges(name, data=True)
-            # ... if there's a path in the graph leading back from the current node to the
-            # input node, # and only in case this node accepts multiple inputs.
-            if not (networkx.has_path(self.graph, name, from_node) and self.graph.nodes[name]["variadic_input"])
-        ]
-        return data_to_wait_for
-
-    def _all_nodes_to_wait_for_run(self, nodes_to_wait_for: List[str]) -> bool:
-        """
-        Check if all the nodes this component is waiting for has run or not.
-
-        FIXME: checking for `visits>0` might not be enough for all loops.
-        """
-        return all(self.graph.nodes[node_to_wait_for]["visits"] > 0 for node_to_wait_for in nodes_to_wait_for)
-
-    def _skip_downstream_nodes(self, component: str, inputs_buffer: OrderedDict) -> OrderedDict:
+    def _skip_downstream_unvisited_nodes(self, component: str, inputs_buffer: OrderedDict) -> OrderedDict:
         """
         When a component is skipped, put all downstream nodes in the inputs buffer too: the might be skipped too,
-        unless they are merge/variadic nodes. They will be evaluated later by the pipeline execution loop.
+        unless they are merge nodes. They will be evaluated later by the pipeline execution loop.
         """
         downstream_nodes = [e[1] for e in self.graph.out_edges(component)]
         for downstream_node in downstream_nodes:
-            if not downstream_node in inputs_buffer:
+            if downstream_node in inputs_buffer:
+                continue
+            if self.graph.nodes[downstream_node]["visits"] == 0:
+                # Skip downstream nodes only if they never been visited
                 inputs_buffer[downstream_node] = {}
         return inputs_buffer
 
     def _run_component(self, name: str, inputs: Dict[str, Any]) -> Dict[str, Any]:
         """
         Once we're confident this component is ready to run, run it and collect the output.
         """
         self.graph.nodes[name]["visits"] += 1
         instance = self.graph.nodes[name]["instance"]
         try:
             logger.info("* Running %s (visits: %s)", name, self.graph.nodes[name]["visits"])
             logger.debug("   '%s' inputs: %s", name, inputs)
 
-            input_class = instance.Input if hasattr(instance, "Input") else instance.input_type
-
-            # If the node is variadic, unpack the input
-            if self.graph.nodes[name]["variadic_input"]:
-                inputs = list(inputs.values())[0]
-                input_dataclass = input_class(*inputs)
-
-            # Otherwise pass the inputs as kwargs after adding the component's own defaults to them
-            else:
-                inputs = {**instance.defaults, **inputs}
-                input_dataclass = input_class(**inputs)
+            # Optional fields are defaulted to None so creation of the input dataclass doesn't fail
+            # cause we're missing some argument
+            optionals = {field: None for field in instance.__canals_optional_inputs__}
+
+            # Pass the inputs as kwargs after adding the component's own defaults to them
+            inputs = {**optionals, **instance.defaults, **inputs}
+            input_dataclass = instance.input(**inputs)
 
             output_dataclass = instance.run(input_dataclass)
 
             # Unwrap the output
             logger.debug("   '%s' outputs: %s\n", name, output_dataclass.__dict__)
 
         except Exception as e:
@@ -636,20 +677,15 @@
                     logger.debug(
                         "Not adding '%s' to the inputs buffer: we're staying in the loop.",
                         target_node,
                     )
             else:
                 # In all other cases, populate the inputs buffer for all downstream nodes, setting None to any
                 # edge that did not receive input.
-                if not target_node in inputs_buffer:
+                if target_node not in inputs_buffer:
                     inputs_buffer[target_node] = {}  # Create the buffer for the downstream node if it's not there yet
 
                 value_to_route = getattr(node_results, from_socket.name, None)
                 if value_to_route:
-                    if to_socket.variadic:
-                        if not to_socket.name in inputs_buffer[target_node].keys():
-                            inputs_buffer[target_node][to_socket.name] = []
-                        inputs_buffer[target_node][to_socket.name].append(value_to_route)
-                    else:
-                        inputs_buffer[target_node][to_socket.name] = value_to_route
+                    inputs_buffer[target_node][to_socket.name] = value_to_route
 
         return inputs_buffer
```

### Comparing `canals-0.2.2/canals/testing/test_component.py` & `canals-0.3.1/canals/testing/test_component.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.2/docs/index.md` & `canals-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `canals-0.2.2/docs/concepts/concepts.md` & `canals-0.3.1/docs/concepts/concepts.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 # Core concepts
 
 Canals is a **component orchestration engine**. It can be used to connect a group of smaller objects, called Components,
 that perform well-defined tasks into a network, called Pipeline, to achieve a larger goal.
 
 Components are Python objects that can execute a task, like reading a file, performing calculations, or making API
 calls. Canals connects these objects together: it builds a graph of components and takes care of managing their
-execution order, making sure that each object receives the input it expects from the other components of the pipeline.
+execution order, making sure that each object receives the input it expects from the other components of the pipeline at the right time.
 
 Canals relies on two main concepts: Components and Pipelines.
 
 ## What is a Component?
 
 A Component is a Python class that performs a well-defined task: for example a REST API call, a mathematical operation,
 a data trasformation, writing something to a file or a database, and so on.
 
 To be recognized as a Component by Canals, a Python class needs to respect these rules:
 
 1. Must be decorated with the `@component` decorator.
-3. Have a `run()` method with all the inputs and outputs typed.
-4. Must return a pre-defined dataclass called `Output`.
+3. Have a `run()` method that accepts a `data` parameter of type `ComponentInput` return a single object of type `ComponentOutput`.
 
 For example, the following is a Component that sums up two numbers:
 
 ```python
 from dataclasses import dataclass
 from canals.component import component, ComponentInput, ComponentOutput
 
 @component
 class AddFixedValue:
     """
     Adds the value of `add` to `value`. If not given, `add` defaults to 1.
     """
 
-    @dataclass
-    class Input(ComponentInput):
-        value: int
-
-    @dataclass
-    class Output(ComponentOutput):
-        value: int
+    @component.input
+    def input(self):
+        class Input:
+            value: int
+            add: int
+
+        return Input
+
+    @component.output
+    def output(self):
+        class Output:
+            value: int
+
+        return Output
 
     def __init__(self, add: Optional[int] = 1):
         if add:
             self.defaults = {"add": add}
 
-    def run(self, data: Input) -> Output:
-        return AddFixedValue.Output(value=data.value + data.add)
+    def run(self, data):
+        return self.output(value=data.value + data.add)
 ```
 
 We will see the details of all of these requirements below.
 
 ## What is a Pipeline?
 
 A Pipeline is a network of Components. Pipelines define what components receive and send output to which other, makes
@@ -89,15 +95,15 @@
 pipeline.connect(connect_from="add_one", connect_to="add_one_again")
 pipeline.connect(connect_from="add_one_again", connect_to="add_two")
 
 # Pipeline can be drawn
 pipeline.draw("pipeline.jpg")
 
 # Pipelines are run by giving them the data that the input nodes expect.
-results = pipeline.run(data={"double": MultiplyBy.Input(value=1)})
+results = pipeline.run(data={"double": multiplication.input(value=1)})
 
 print(results)
 
 # prints {"add_two": AddFixedValue.Output(value=6)}
 ```
 
 This is how the pipeline's graph looks like:
```

### Comparing `canals-0.2.2/docs/concepts/pipelines.md` & `canals-0.3.1/docs/concepts/pipelines.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,100 +9,108 @@
 - Multiple entry components, either alternative or parallel
 - Multiple exit components, either alternative or parallel
 
 Check the pipeline's test suite for some examples.
 
 ## Validation
 
-Pipeline performs validation on the connection type level: when calling `Pipeline.connect()`, it uses the values of the
-components' `run()` method signature and the `Output` dataclass (or equivalent dataclass returned by
-`self.output_type()`) to make sure that the connection is possible.
+Pipeline performs validation on the connection type level: when calling `Pipeline.connect()`, it uses the `@component.input` and `@component.output` dataclass fields to make sure that the connection is possible.
 
-On top of this, specific connections can be specified with the syntax `component_name.input_or_output_name`.
+On top of this, specific connections can be specified with the syntax `component_name.input_or_output_field`.
 
 For example, let's imagine we have two components with the following I/O declared:
 
 ```python
 @component
 class ComponentA:
 
-    @dataclass
-    class Input(ComponentInput):
-        input_value: int
-
-    @dataclass
-    class Output(ComponentOutput):
-        intermediate_value: str
+    @component.input
+    def input(self):
+        class Input:
+            input_value: int
+
+        return Input
+
+    @component.output
+    def output(self):
+        class Output:
+            output_value: str
 
-    def run(self, data: Input) -> Output:
-        return ComponentA.Output(intermediate_value="hello")
+        return Output
+
+    def run(self, data):
+        return self.output(intermediate_value="hello")
 
 @component
 class ComponentB:
 
-    @dataclass
-    class Output:
-        output_value: List[int]
+    @component.input
+    def input(self):
+        class Input:
+            input_value: str
+
+        return Input
+
+    @component.output
+    def output(self):
+        class Output:
+            output_value: List[str]
+
+        return Output
 
-    def run(self, data: Input) -> Output:
-        return ComponentB.Output(output_value=[1, 2, 3])
+    def run(self, data):
+        return self.output(output_value=["h", "e", "l", "l", "o"])
 ```
 
 This is the behavior of `Pipeline.connect()`:
 
 ```python
 pipeline.add_component('component_a', ComponentA())
 pipeline.add_component('component_b', ComponentB())
 
 # All of these succeeds
 pipeline.connect('component_a', 'component_b')
-pipeline.connect('component_a.intermediate_value', 'component_b')
-pipeline.connect('component_a', 'component_b.intermediate_value')
-pipeline.connect('component_a.intermediate_value', 'component_b.intermediate_value')
+pipeline.connect('component_a.output_value', 'component_b')
+pipeline.connect('component_a', 'component_b.input_value')
+pipeline.connect('component_a.output_value', 'component_b.input_value')
 ```
 
 These, instead, fail:
 
 ```python
 pipeline.connect('component_a', 'component_a')
 # canals.errors.PipelineConnectError: Cannot connect 'component_a' with 'component_a': no matching connections available.
 # 'component_a':
-#  - intermediate_value (str)
+#  - output_value (str)
 # 'component_a':
 #  - input_value (int, available)
 
 pipeline.connect('component_b', 'component_a')
 # canals.errors.PipelineConnectError: Cannot connect 'component_b' with 'component_a': no matching connections available.
 # 'component_b':
-#  - output_value (List)
+#  - output_value (List[str])
 # 'component_a':
 #  - input_value (int, available)
 ```
 
 In addition, components names are validated:
 
 ```python
 pipeline.connect('component_a', 'component_c')
 # ValueError: Component named component_c not found in the pipeline.
 ```
 
 Just like input and output names, when stated:
 
 ```python
-pipeline.connect('component_a.input', 'component_b')
-# canals.errors.PipelineConnectError: 'component_a.input does not exist. Output connections of component_a are: intermediate_value (type str)
-
-pipeline.connect('component_a.output', 'component_b')
-# canals.errors.PipelineConnectError: 'component_a.output does not exist. Output connections of component_a are: intermediate_value (type str)
-
-pipeline.connect('component_a', 'component_b.input')
-# canals.errors.PipelineConnectError: 'component_b.input does not exist. Input connections of component_b are: intermediate_value (type str)
+pipeline.connect('component_a.input_value', 'component_b')
+# canals.errors.PipelineConnectError: 'component_a.typo does not exist. Output connections of component_a are: output_value (type str)
 
-pipeline.connect('component_a', 'component_b.output')
-# canals.errors.PipelineConnectError: 'component_b.output does not exist. Input connections of component_b are: intermediate_value (type str)
+pipeline.connect('component_a', 'component_b.output_value')
+# canals.errors.PipelineConnectError: 'component_b.output_value does not exist. Input connections of component_b are: input_value (type str)
 ```
 
 ## Save and Load
 
 Pipelines can be serialized to Python dictionaries, that can be then dumped to JSON or to any other suitable format, like YAML, TOML, HCL, etc. These pipelines can then be loaded back.
 
 Here is an example of Pipeline saving and loading:
```

### Comparing `canals-0.2.2/images/canals-logo-dark.png` & `canals-0.3.1/images/canals-logo-dark.png`

 * *Files identical despite different names*

### Comparing `canals-0.2.2/images/canals-logo-light.png` & `canals-0.3.1/images/canals-logo-light.png`

 * *Files identical despite different names*

### Comparing `canals-0.2.2/test/test_save_load.py` & `canals-0.3.1/test/test_save_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,14 @@
                 },
                 "connections": [
                     ("first_addition", "double", "value/value"),
                     ("double", "second_addition", "value/value"),
                 ],
             },
         },
-        "dependencies": ["test", "canals"],
     }
 
 
 def test_unmarshal():
     pipelines = unmarshal_pipelines(
         {
             "pipelines": {
```

### Comparing `canals-0.2.2/test/pipelines/integration/test_complex_pipeline.py` & `canals-0.3.1/test/pipelines/integration/test_complex_pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,29 +20,31 @@
 )
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_complex_pipeline(tmp_path):
     accumulate = Accumulate()
+    loop_merger = MergeLoop(expected_type=int, inputs=["in_1", "in_2"])
+    summer = Sum(inputs=["in_1", "in_2", "in_3"])
 
-    pipeline = Pipeline(max_loops_allowed=4)
+    pipeline = Pipeline(max_loops_allowed=2)
     pipeline.add_component("greet_first", Greet(message="Hello, the value is {value}."))
     pipeline.add_component("accumulate_1", accumulate)
     pipeline.add_component("add_two", AddFixedValue(add=2))
     pipeline.add_component("parity", Parity())
     pipeline.add_component("add_one", AddFixedValue(add=1))
     pipeline.add_component("accumulate_2", accumulate)
 
-    pipeline.add_component("loop_merger", MergeLoop(expected_type=int))
+    pipeline.add_component("loop_merger", loop_merger)
     pipeline.add_component("below_10", Threshold(threshold=10))
     pipeline.add_component("double", Double())
 
     pipeline.add_component("greet_again", Greet(message="Hello again, now the value is {value}."))
-    pipeline.add_component("sum", Sum())
+    pipeline.add_component("sum", summer)
 
     pipeline.add_component("greet_enumerator", Greet(message="Hello from enumerator, here the value became {value}."))
     pipeline.add_component("enumerate", Repeat(outputs=["first", "second"]))
     pipeline.add_component("add_three", AddFixedValue(add=3))
 
     pipeline.add_component("diff", Subtract())
     pipeline.add_component("greet_one_last_time", Greet(message="Bye bye! The value here is {value}!"))
@@ -52,43 +54,45 @@
     pipeline.add_component("accumulate_3", accumulate)
 
     pipeline.connect("greet_first", "accumulate_1")
     pipeline.connect("accumulate_1", "add_two")
     pipeline.connect("add_two", "parity")
 
     pipeline.connect("parity.even", "greet_again")
-    pipeline.connect("greet_again", "sum")
+    pipeline.connect("greet_again", "sum.in_1")
     pipeline.connect("sum", "diff.first_value")
     pipeline.connect("diff", "greet_one_last_time")
     pipeline.connect("greet_one_last_time", "replicate")
     pipeline.connect("replicate.first", "add_five.value")
     pipeline.connect("replicate.second", "add_four.value")
     pipeline.connect("add_four", "accumulate_3")
 
     pipeline.connect("parity.odd", "add_one.value")
-    pipeline.connect("add_one", "loop_merger")
+    pipeline.connect("add_one", "loop_merger.in_1")
     pipeline.connect("loop_merger", "below_10")
 
     pipeline.connect("below_10.below", "double")
-    pipeline.connect("double", "loop_merger")
+    pipeline.connect("double", "loop_merger.in_2")
 
     pipeline.connect("below_10.above", "accumulate_2")
     pipeline.connect("accumulate_2", "diff.second_value")
 
     pipeline.connect("greet_enumerator", "enumerate")
-    pipeline.connect("enumerate.second", "sum")
+    pipeline.connect("enumerate.second", "sum.in_2")
 
     pipeline.connect("enumerate.first", "add_three.value")
-    pipeline.connect("add_three", "sum")
+    pipeline.connect("add_three", "sum.in_3")
 
     pipeline.draw(tmp_path / "complex_pipeline.png")
 
-    results = pipeline.run({"greet_first": Greet.Input(value=1), "greet_enumerator": Greet.Input(value=1)})
+    results = pipeline.run({"greet_first": Greet().input(value=1), "greet_enumerator": Greet().input(value=1)})
     pprint(results)
     print("accumulated: ", accumulate.state)
 
-    assert results == {"accumulate_3": Accumulate.Output(value=9), "add_five": AddFixedValue.Output(value=-7)}
+    assert len(results) == 2
+    assert results["accumulate_3"].value == 9
+    assert results["add_five"].value == -7
     assert accumulate.state == 9
 
 
 if __name__ == "__main__":
     test_complex_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.2.2/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py` & `canals-0.3.1/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,26 +31,28 @@
     pipeline.connect("parity.odd", "add_ten.value")
     pipeline.connect("add_four", "add_two")
 
     pipeline.draw(tmp_path / "fixed_decision_and_merge_pipeline.png")
 
     results = pipeline.run(
         {
-            "add_one": AddFixedValue.Input(value=1),
-            "add_two": AddFixedValue.Input(add=2),
+            "add_one": AddFixedValue().input(value=1),
+            "add_two": AddFixedValue().input(add=2),
         }
     )
     pprint(results)
-    assert results == {"add_two": AddFixedValue.Output(value=8)}
+    assert len(results) == 1
+    assert results["add_two"].value == 8
 
     results = pipeline.run(
         {
-            "add_one": AddFixedValue.Input(value=2),
-            "add_two": AddFixedValue.Input(add=2),
+            "add_one": AddFixedValue().input(value=2),
+            "add_two": AddFixedValue().input(add=2),
         }
     )
     pprint(results)
-    assert results == {"diff": Subtract.Output(difference=7)}
+    assert len(results) == 1
+    assert results["diff"].difference == 7
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.2.2/test/pipelines/integration/test_fixed_decision_pipeline.py` & `canals-0.3.1/test/pipelines/integration/test_variable_decision_pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.sample_components import AddFixedValue, Parity, Double
+from test.sample_components import AddFixedValue, Remainder, Double
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
     add_one = AddFixedValue(add=1)
 
     pipeline = Pipeline()
     pipeline.add_component("add_one", add_one)
-    pipeline.add_component("parity", Parity())
+    pipeline.add_component("remainder", Remainder(divisor=3))
     pipeline.add_component("add_ten", AddFixedValue(add=10))
     pipeline.add_component("double", Double())
     pipeline.add_component("add_three", AddFixedValue(add=3))
+    pipeline.add_component("add_one_again", add_one)
 
-    pipeline.connect("add_one", "parity")
-    pipeline.connect("parity.even", "add_ten.value")
-    pipeline.connect("parity.odd", "double.value")
-    pipeline.connect("add_ten", "add_three")
+    pipeline.connect("add_one", "remainder")
+    pipeline.connect("remainder.remainder_is_0", "add_ten.value")
+    pipeline.connect("remainder.remainder_is_1", "double")
+    pipeline.connect("remainder.remainder_is_2", "add_three.value")
+    pipeline.connect("add_three", "add_one_again")
 
-    pipeline.draw(tmp_path / "fixed_decision_pipeline.png")
+    pipeline.draw(tmp_path / "variable_decision_pipeline.png")
 
-    results = pipeline.run({"add_one": AddFixedValue.Input(value=1)})
+    results = pipeline.run({"add_one": AddFixedValue().input(value=1)})
     pprint(results)
-    assert results == {"add_three": AddFixedValue.Output(value=15)}
 
-    results = pipeline.run({"add_one": AddFixedValue.Input(value=2)})
-    pprint(results)
-    assert results == {"double": Double.Output(value=6)}
+    assert results == {"add_one_again": AddFixedValue().output(value=6)}
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.2.2/test/pipelines/integration/test_fixed_merging_pipeline.py` & `canals-0.3.1/test/pipelines/integration/test_fixed_merging_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
-
     add_two = AddFixedValue(add=2)
     diff = Subtract()
 
     pipeline = Pipeline()
     pipeline.add_component("first_addition", add_two)
     pipeline.add_component("second_addition", add_two)
     pipeline.add_component("third_addition", add_two)
@@ -29,18 +28,18 @@
     pipeline.connect("third_addition", "diff.second_value")
     pipeline.connect("diff", "fourth_addition.value")
 
     pipeline.draw(tmp_path / "fixed_merging_pipeline.png")
 
     results = pipeline.run(
         {
-            "first_addition": AddFixedValue.Input(value=1),
-            "third_addition": AddFixedValue.Input(value=1),
+            "first_addition": AddFixedValue().input(value=1),
+            "third_addition": AddFixedValue().input(value=1),
         }
     )
     pprint(results)
 
-    assert results == {"fourth_addition": AddFixedValue.Output(value=3)}
+    assert results == {"fourth_addition": AddFixedValue().output(value=3)}
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.2.2/test/pipelines/integration/test_linear_pipeline.py` & `canals-0.3.1/test/pipelines/integration/test_linear_pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     pipeline.add_component("second_addition", AddFixedValue())
     pipeline.add_component("double", Double())
     pipeline.connect("first_addition", "double")
     pipeline.connect("double", "second_addition")
 
     pipeline.draw(tmp_path / "linear_pipeline.png")
 
-    results = pipeline.run({"first_addition": AddFixedValue.Input(value=1)})
+    results = pipeline.run({"first_addition": AddFixedValue().input(value=1)})
     pprint(results)
 
-    assert results == {"second_addition": AddFixedValue.Output(value=7)}
+    assert results == {"second_addition": AddFixedValue().output(value=7)}
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.2.2/test/pipelines/integration/test_looping_and_merge_pipeline.py` & `canals-0.3.1/test/pipelines/integration/test_looping_pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,47 +2,43 @@
 #
 # SPDX-License-Identifier: Apache-2.0
 from typing import *
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.sample_components import Accumulate, AddFixedValue, Threshold, Sum, MergeLoop
+from test.sample_components import Accumulate, AddFixedValue, Threshold, MergeLoop
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
     accumulator = Accumulate()
-    merge_loop = MergeLoop(expected_type=int)
+    merge_loop = MergeLoop(expected_type=int, inputs=["in_1", "in_2"])
 
     pipeline = Pipeline(max_loops_allowed=10)
+    pipeline.add_component("add_one", AddFixedValue(add=1))
     pipeline.add_component("merge", merge_loop)
-    pipeline.add_component("sum", Sum())
     pipeline.add_component("below_10", Threshold(threshold=10))
-    pipeline.add_component("add_one", AddFixedValue(add=1))
-    pipeline.add_component("counter", accumulator)
+    pipeline.add_component("accumulator", accumulator)
     pipeline.add_component("add_two", AddFixedValue(add=2))
 
+    pipeline.connect("add_one", "merge.in_1")
     pipeline.connect("merge", "below_10")
-    pipeline.connect("below_10.below", "add_one.value")
-    pipeline.connect("add_one", "counter")
-    pipeline.connect("counter", "merge")
+    pipeline.connect("below_10.below", "accumulator")
+    pipeline.connect("accumulator", "merge.in_2")
     pipeline.connect("below_10.above", "add_two.value")
-    pipeline.connect("add_two", "sum")
 
-    pipeline.draw(tmp_path / "looping_and_merge_pipeline.png")
+    pipeline.draw(tmp_path / "looping_pipeline.png")
 
-    results = pipeline.run(
-        {"merge": merge_loop.input_type(8), "sum": Sum.Input(2)},
-    )
+    results = pipeline.run({"add_one": AddFixedValue().input(value=3)})
     pprint(results)
-    print("accumulate: ", accumulator.state)
+    print("accumulator: ", accumulator.state)
 
-    assert results == {"sum": Sum.Output(total=23)}
-    assert accumulator.state == 19
+    assert results == {"add_two": AddFixedValue().output(value=18)}
+    assert accumulator.state == 16
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.2.2/test/pipelines/integration/test_looping_pipeline.py` & `canals-0.3.1/test/pipelines/integration/test_double_loop_pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,32 +11,39 @@
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
     accumulator = Accumulate()
-    merge_loop = MergeLoop(expected_type=int)
+    merge_loop = MergeLoop(expected_type=int, inputs=["in_1", "in_2", "in_3"])
 
     pipeline = Pipeline(max_loops_allowed=10)
+    pipeline.add_component("add_one", AddFixedValue(add=1))
     pipeline.add_component("merge", merge_loop)
     pipeline.add_component("below_10", Threshold(threshold=10))
+    pipeline.add_component("below_5", Threshold(threshold=5))
+    pipeline.add_component("add_three", AddFixedValue(add=3))
     pipeline.add_component("accumulator", accumulator)
     pipeline.add_component("add_two", AddFixedValue(add=2))
 
+    pipeline.connect("add_one", "merge.in_1")
     pipeline.connect("merge", "below_10")
     pipeline.connect("below_10.below", "accumulator")
-    pipeline.connect("accumulator", "merge")
+    pipeline.connect("accumulator", "below_5")
+    pipeline.connect("below_5.above", "add_three.value")
+    pipeline.connect("below_5.below", "merge.in_2")
+    pipeline.connect("add_three", "merge.in_3")
     pipeline.connect("below_10.above", "add_two.value")
 
-    pipeline.draw(tmp_path / "looping_pipeline.png")
+    pipeline.draw(tmp_path / "double_loop_pipeline.png")
 
-    results = pipeline.run({"merge": merge_loop.input_type(4)})
+    results = pipeline.run({"add_one": AddFixedValue().input(value=3)})
     pprint(results)
     print("accumulator: ", accumulator.state)
 
-    assert results == {"add_two": AddFixedValue.Output(value=18)}
-    assert accumulator.state == 16
+    assert results == {"add_two": AddFixedValue().output(value=13)}
+    assert accumulator.state == 8
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.2.2/test/pipelines/integration/test_parallel_branches_pipeline.py` & `canals-0.3.1/test/pipelines/integration/test_parallel_branches_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     pipeline.connect("repeat.first", "add_ten.value")
     pipeline.connect("repeat.second", "double")
     pipeline.connect("repeat.second", "add_three.value")
     pipeline.connect("add_three", "add_one_again")
 
     pipeline.draw(tmp_path / "parallel_branches_pipeline.png")
 
-    results = pipeline.run({"add_one": AddFixedValue.Input(value=1)})
+    results = pipeline.run({"add_one": AddFixedValue().input(value=1)})
     pprint(results)
 
     assert results == {
-        "add_one_again": AddFixedValue.Output(value=6),
-        "add_ten": AddFixedValue.Output(value=12),
-        "double": Double.Output(value=4),
+        "add_one_again": AddFixedValue().output(value=6),
+        "add_ten": AddFixedValue().output(value=12),
+        "double": Double().output(value=4),
     }
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.2.2/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py` & `canals-0.3.1/test/pipelines/integration/test_variable_merging_pipeline.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
-import logging
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.sample_components import AddFixedValue, Remainder, Double, Sum
+from test.sample_components import AddFixedValue, Sum
+
+import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
-    add_one = AddFixedValue()
+    add_two = AddFixedValue(add=2)
+    make_the_sum = Sum(inputs=["in_1", "in_2", "in_3"])
 
     pipeline = Pipeline()
-    pipeline.add_component("add_one", add_one)
-    pipeline.add_component("parity", Remainder())
-    pipeline.add_component("add_ten", AddFixedValue(add=10))
-    pipeline.add_component("double", Double())
-    pipeline.add_component("add_four", AddFixedValue(add=4))
-    pipeline.add_component("add_one_again", add_one)
-    pipeline.add_component("sum", Sum())
-
-    pipeline.connect("add_one", "parity")
-    pipeline.connect("parity.remainder_is_0", "add_ten.value")
-    pipeline.connect("parity.remainder_is_1", "double")
-    pipeline.connect("add_one", "sum")
-    pipeline.connect("add_ten", "sum")
-    pipeline.connect("double", "sum")
-    pipeline.connect("parity.remainder_is_1", "add_four.value")
-    pipeline.connect("add_four", "add_one_again")
-    pipeline.connect("add_one_again", "sum")
-
-    pipeline.draw(tmp_path / "variable_decision_and_merge_pipeline.png")
-
-    results = pipeline.run({"add_one": AddFixedValue.Input(value=1)})
+    pipeline.add_component("first_addition", add_two)
+    pipeline.add_component("second_addition", add_two)
+    pipeline.add_component("third_addition", add_two)
+    pipeline.add_component("sum", make_the_sum)
+    pipeline.add_component("fourth_addition", AddFixedValue(add=1))
+
+    pipeline.connect("first_addition", "second_addition")
+    pipeline.connect("first_addition", "sum.in_1")
+    pipeline.connect("second_addition", "sum.in_2")
+    pipeline.connect("third_addition", "sum.in_3")
+    pipeline.connect("sum", "fourth_addition.value")
+
+    pipeline.draw(tmp_path / "variable_merging_pipeline.png")
+
+    results = pipeline.run(
+        {
+            "first_addition": AddFixedValue().input(value=1),
+            "third_addition": AddFixedValue().input(value=1),
+        }
+    )
     pprint(results)
-    assert results == {"sum": Sum.Output(total=14)}
 
-    results = pipeline.run({"add_one": AddFixedValue.Input(value=2)})
-    pprint(results)
-    assert results == {"sum": Sum.Output(total=17)}
+    assert results == {"fourth_addition": AddFixedValue().output(value=12)}
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.2.2/test/pipelines/integration/test_variable_decision_pipeline.py` & `canals-0.3.1/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+import logging
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.sample_components import AddFixedValue, Remainder, Double
-
-import logging
+from test.sample_components import AddFixedValue, Remainder, Double, Sum
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
-    add_one = AddFixedValue(add=1)
+    add_one = AddFixedValue()
+    summer = Sum(inputs=["in_1", "in_2", "in_3", "in_4"])
 
     pipeline = Pipeline()
     pipeline.add_component("add_one", add_one)
-    pipeline.add_component("remainder", Remainder(divisor=3))
+    pipeline.add_component("parity", Remainder())
     pipeline.add_component("add_ten", AddFixedValue(add=10))
     pipeline.add_component("double", Double())
-    pipeline.add_component("add_three", AddFixedValue(add=3))
+    pipeline.add_component("add_four", AddFixedValue(add=4))
     pipeline.add_component("add_one_again", add_one)
+    pipeline.add_component("sum", summer)
 
-    pipeline.connect("add_one", "remainder")
-    pipeline.connect("remainder.remainder_is_0", "add_ten.value")
-    pipeline.connect("remainder.remainder_is_1", "double")
-    pipeline.connect("remainder.remainder_is_2", "add_three.value")
-    pipeline.connect("add_three", "add_one_again")
+    pipeline.connect("add_one", "parity")
+    pipeline.connect("parity.remainder_is_0", "add_ten.value")
+    pipeline.connect("parity.remainder_is_1", "double")
+    pipeline.connect("add_one", "sum.in_1")
+    pipeline.connect("add_ten", "sum.in_2")
+    pipeline.connect("double", "sum.in_3")
+    pipeline.connect("parity.remainder_is_1", "add_four.value")
+    pipeline.connect("add_four", "add_one_again")
+    pipeline.connect("add_one_again", "sum.in_4")
 
-    pipeline.draw(tmp_path / "variable_decision_pipeline.png")
+    pipeline.draw(tmp_path / "variable_decision_and_merge_pipeline.png")
 
-    results = pipeline.run({"add_one": AddFixedValue.Input(value=1)})
+    results = pipeline.run({"add_one": add_one.input(value=1)})
     pprint(results)
+    assert results == {"sum": summer.output(total=14)}
 
-    assert results == {"add_one_again": AddFixedValue.Output(value=6)}
+    results = pipeline.run({"add_one": add_one.input(value=2)})
+    pprint(results)
+    assert results == {"sum": summer.output(total=17)}
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.2.2/test/sample_components/__init__.py` & `canals-0.3.1/test/sample_components/__init__.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.2/test/sample_components/test_accumulate.py` & `canals-0.3.1/test/sample_components/test_accumulate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 from typing import Union, Callable, Optional
 import sys
 import builtins
 from importlib import import_module
-from dataclasses import dataclass
 
-import pytest
-from canals.component import component, ComponentInput, ComponentOutput
+from canals.component import component
 from canals.testing import BaseTestComponent
 
 
 @component
 class Accumulate:
     """
     Accumulates the value flowing through the connection into an internal attribute.
     The sum function can be customized.
 
     Example of how to deal with serialization when some of the parameters
     are not directly serializable.
     """
 
-    @dataclass
-    class Input(ComponentInput):
-        value: int
-
-    @dataclass
-    class Output(ComponentOutput):
-        value: int
+    @component.input  # type: ignore
+    def input(self):
+        class Input:
+            value: int
+
+        return Input
+
+    @component.output  # type: ignore
+    def output(self):
+        class Output:
+            value: int
+
+        return Output
 
     def __init__(self, function: Optional[Union[Callable, str]] = None):
         """
         :param function: the function to use to accumulate the values.
             The function must take exactly two values.
             If it's a callable, it's used as it is.
             If it's a string, the component will look for it in sys.modules and
@@ -43,17 +47,17 @@
         if function is None:
             self.function = lambda x, y: x + y
         else:
             self.function = self._load_function(function)
             # 'function' is not serializable by default, so we serialize it manually.
             self.init_parameters = {"function": self._save_function(function)}
 
-    def run(self, data: Input) -> Output:
+    def run(self, data):
         self.state = self.function(self.state, data.value)
-        return Accumulate.Output(value=self.state)
+        return self.output(value=self.state)
 
     def _load_function(self, function: Union[Callable, str]):
         """
         Loads the function by trying to import it.
         """
         if not isinstance(function, str):
             return function
@@ -94,46 +98,46 @@
         )
 
     def test_saveload_function_as_callable(self, tmp_path):
         self.assert_can_be_saved_and_loaded_in_pipeline(Accumulate(function=my_subtract), tmp_path)
 
     def test_accumulate_default(self):
         component = Accumulate()
-        results = component.run(Accumulate.Input(value=10))
-        assert results == Accumulate.Output(value=10)
+        results = component.run(component.input(value=10))
+        assert results == component.output(value=10)
         assert component.state == 10
 
-        results = component.run(Accumulate.Input(value=1))
-        assert results == Accumulate.Output(value=11)
+        results = component.run(component.input(value=1))
+        assert results == component.output(value=11)
         assert component.state == 11
 
         assert component.init_parameters == {}
 
     def test_accumulate_callable(self):
         component = Accumulate(function=my_subtract)
 
-        results = component.run(Accumulate.Input(value=10))
-        assert results == Accumulate.Output(value=-10)
+        results = component.run(component.input(value=10))
+        assert results == component.output(value=-10)
         assert component.state == -10
 
-        results = component.run(Accumulate.Input(value=1))
-        assert results == Accumulate.Output(value=-11)
+        results = component.run(component.input(value=1))
+        assert results == component.output(value=-11)
         assert component.state == -11
 
         assert component.init_parameters == {
             "function": "test.sample_components.test_accumulate.my_subtract",
         }
 
     def test_accumulate_string(self):
         component = Accumulate(function="test.sample_components.test_accumulate.my_subtract")
 
-        results = component.run(Accumulate.Input(value=10))
-        assert results == Accumulate.Output(value=-10)
+        results = component.run(component.input(value=10))
+        assert results == component.output(value=-10)
         assert component.state == -10
 
-        results = component.run(Accumulate.Input(value=1))
-        assert results == Accumulate.Output(value=-11)
+        results = component.run(component.input(value=1))
+        assert results == component.output(value=-11)
         assert component.state == -11
 
         assert component.init_parameters == {
             "function": "test.sample_components.test_accumulate.my_subtract",
         }
```

### Comparing `canals-0.2.2/test/sample_components/test_add_value.py` & `canals-0.3.1/test/sample_components/test_add_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 from typing import Optional
 
-from dataclasses import dataclass
 
-import pytest
-
-from canals.component import component, ComponentInput, ComponentOutput
+from canals.component import component
 from canals.testing.test_component import BaseTestComponent
 
 
 @component
 class AddFixedValue:
     """
     Adds the value of `add` to `value`. If not given, `add` defaults to 1.
     """
 
-    @dataclass
-    class Input(ComponentInput):
-        value: int
-        add: int
-
-    @dataclass
-    class Output(ComponentOutput):
-        value: int
+    @component.input  # type: ignore
+    def input(self):
+        class Input:
+            value: int
+            add: int
+
+        return Input
+
+    @component.output  # type: ignore
+    def output(self):
+        class Output:
+            value: int
+
+        return Output
 
     def __init__(self, add: Optional[int] = 1):
         if add:
             self.defaults = {"add": add}
 
-    def run(self, data: Input) -> Output:
-        return AddFixedValue.Output(value=data.value + data.add)
+    def run(self, data):
+        return self.output(value=data.value + data.add)
 
 
 class TestAddFixedValue(BaseTestComponent):
     def test_saveload_default(self, tmp_path):
         self.assert_can_be_saved_and_loaded_in_pipeline(AddFixedValue(), tmp_path)
 
     def test_saveload_add(self, tmp_path):
         self.assert_can_be_saved_and_loaded_in_pipeline(AddFixedValue(add=2), tmp_path)
 
     def test_addvalue(self):
         component = AddFixedValue()
-        results = component.run(AddFixedValue.Input(value=50, add=10))
-        assert results == AddFixedValue.Output(value=60)
+        results = component.run(component.input(value=50, add=10))
+        assert results == component.output(value=60)
         assert component.init_parameters == {}
```

### Comparing `canals-0.2.2/test/sample_components/test_greet.py` & `canals-0.3.1/test/sample_components/test_greet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 from typing import Optional
 import logging
 
-from dataclasses import dataclass
-
-import pytest
 
 from canals.testing import BaseTestComponent
-from canals.component import component, ComponentInput, ComponentOutput
+from canals.component import component
 
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class Greet:
     """
     Logs a greeting message without affecting the value passing on the connection.
     """
 
-    @dataclass
-    class Input(ComponentInput):
-        value: int
-        message: str
-        log_level: str
-
-    @dataclass
-    class Output(ComponentOutput):
-        value: int
+    @component.input  # type: ignore
+    def input(self):
+        class Input:
+            value: int
+            message: str
+            log_level: str
+
+        return Input
+
+    @component.output  # type: ignore
+    def output(self):
+        class Output:
+            value: int
+
+        return Output
 
     def __init__(
         self,
         message: Optional[str] = "\nGreeting component says: Hi! The value is {value}\n",
         log_level: Optional[str] = "INFO",
     ):
         """
         :param message: the message to log. Can use `{value}` to embed the value.
         :param log_level: the level to log at.
         """
         if log_level and not getattr(logging, log_level):
             raise ValueError(f"This log level does not exist: {log_level}")
         self.defaults = {"message": message, "log_level": log_level}
 
-    def run(self, data: Input) -> Output:
+    def run(self, data):
         """
         Logs a greeting message without affecting the value passing on the connection.
         """
         print(data.log_level)
         level = getattr(logging, data.log_level, None)
         if not level:
             raise ValueError(f"This log level does not exist: {data.log_level}")
 
         logger.log(level=level, msg=data.message.format(value=data.value))
-        return Greet.Output(value=data.value)
+        return self.output(value=data.value)
 
 
 class TestGreet(BaseTestComponent):
     def test_saveload_default(self, tmp_path):
         self.assert_can_be_saved_and_loaded_in_pipeline(Greet(), tmp_path)
 
     def test_saveload_message(self, tmp_path):
@@ -71,10 +74,10 @@
         self.assert_can_be_saved_and_loaded_in_pipeline(
             Greet(message="Hello, that's {value}", log_level="WARNING"), tmp_path
         )
 
     def test_greet_message(self, caplog):
         caplog.set_level(logging.WARNING)
         component = Greet()
-        results = component.run(Greet.Input(value=10, message="Hello, that's {value}", log_level="WARNING"))
-        assert results == Greet.Output(value=10)
+        results = component.run(component.input(value=10, message="Hello, that's {value}", log_level="WARNING"))
+        assert results == component.output(value=10)
         assert "Hello, that's 10" in caplog.text
```

### Comparing `canals-0.2.2/test/sample_components/test_merge_loop.py` & `canals-0.3.1/test/sample_components/test_merge_loop.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,56 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
-from typing import List, Union
 import builtins
+from typing import List, Union, Optional
+from dataclasses import make_dataclass, is_dataclass, asdict
 
-from dataclasses import dataclass
-
-from canals.component import component, VariadicComponentInput, ComponentOutput
+from canals.component import component
 from canals.testing import BaseTestComponent
 
 
 @component
 class MergeLoop:
     """
-    Takes two input components and returns the first one that is not None.
-    In case both received a value, priority is given to 'first'.
+    Takes multiple inputs and returns the first one that is not None.
     """
 
-    def __init__(self, expected_type: Union[type, str]):
+    def __init__(self, expected_type: Union[type, str], inputs: List[str] = ["value_1", "value_2"]):
         if isinstance(expected_type, str):
-            type_ = getattr(builtins, expected_type)
+            self.expected_type = getattr(builtins, expected_type)
         else:
-            type_ = expected_type
-
-        self.expected_type = type_
-        self.init_parameters = {"expected_type": type_.__name__}
-
-    @property
-    def input_type(self):
-        @dataclass
-        class Input(VariadicComponentInput):
-            values: List[self.expected_type]  # type: ignore
-
-        return Input
-
-    @property
-    def output_type(self):
-        @dataclass
-        class Output(ComponentOutput):
+            self.expected_type = expected_type
+        self.init_parameters = {"expected_type": self.expected_type.__name__}
+        # mypy complains that we can't Optional is not a type, so we ignore the error
+        # cause we consider this to be correct
+        self._input = make_dataclass("Input", fields=[(f, Optional[self.expected_type]) for f in inputs])  # type: ignore
+
+    @component.input  # type: ignore
+    def input(self):
+        return self._input
+
+    @component.output  # type: ignore
+    def output(self):
+        class Output:
             value: self.expected_type  # type: ignore
 
         return Output
 
     def run(self, data):
         """
         Takes some inputs and returns the first one that is not None.
-
-        In case it receives more than one value, priority is given to the first.
         """
-        for v in data.values:
+        values = []
+        if is_dataclass(data):
+            values = asdict(data).values()
+        for v in values:
             if v is not None:
-                return self.output_type(value=v)
-        return self.output_type(value=None)
+                return self.output(value=v)
+        return self.output(value=None)
 
 
 class TestMergeLoop(BaseTestComponent):
     def test_saveload_builtin_type(self, tmp_path):
         self.assert_can_be_saved_and_loaded_in_pipeline(MergeLoop(expected_type=int), tmp_path)
 
     # TODO
@@ -63,30 +58,30 @@
     #     self.assert_can_be_saved_and_loaded_in_pipeline(MergeLoop(expected_type=List[int]), tmp_path)
 
     # def test_saveload_object_type(self, tmp_path):
     #     class MyObject: ...
     #     self.assert_can_be_saved_and_loaded_in_pipeline(MergeLoop(expected_type=MyObject()), tmp_path)
 
     def test_merge_first(self):
-        component = MergeLoop(expected_type=int)
-        results = component.run(component.input_type(5, None))
-        assert results.__dict__ == component.output_type(value=5).__dict__
+        component = MergeLoop(expected_type=int, inputs=["in_1", "in_2"])
+        results = component.run(component.input(5, None))
+        assert results == component.output(value=5)
 
     def test_merge_second(self):
-        component = MergeLoop(expected_type=int)
-        results = component.run(component.input_type(None, 5))
-        assert results.__dict__ == component.output_type(value=5).__dict__
+        component = MergeLoop(expected_type=int, inputs=["in_1", "in_2"])
+        results = component.run(component.input(None, 5))
+        assert results == component.output(value=5)
 
     def test_merge_nones(self):
-        component = MergeLoop(expected_type=int)
-        results = component.run(component.input_type(None, None, None))
-        assert results.__dict__ == component.output_type(value=None).__dict__
+        component = MergeLoop(expected_type=int, inputs=["in_1", "in_2", "in_3"])
+        results = component.run(component.input(None, None, None))
+        assert results == component.output(value=None)
 
     def test_merge_one(self):
         component = MergeLoop(expected_type=int)
-        results = component.run(component.input_type(1))
-        assert results.__dict__ == component.output_type(value=1).__dict__
+        results = component.run(component.input(1))
+        assert results == component.output(value=1)
 
     def test_merge_one_none(self):
         component = MergeLoop(expected_type=int)
-        results = component.run(component.input_type())
-        assert results.__dict__ == component.output_type(value=None).__dict__
+        results = component.run(component.input())
+        assert results == component.output(value=None)
```

### Comparing `canals-0.2.2/test/sample_components/test_parity.py` & `canals-0.3.1/test/sample_components/test_repeat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,58 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
-from typing import Optional
+from typing import List
+
+from dataclasses import make_dataclass
 
-from dataclasses import dataclass
-import pytest
 
 from canals.testing import BaseTestComponent
-from canals.component import component, ComponentInput, ComponentOutput
+from canals.component import component
 
 
 @component
-class Parity:
+class Repeat:
     """
-    Redirects the value, unchanged, along the 'even' connection if even, or along the 'odd' one if odd.
+    Repeats the input value on all outputs.
     """
 
-    @dataclass
-    class Input(ComponentInput):
-        value: int
-
-    @dataclass
-    class Output(ComponentOutput):
-        even: Optional[int] = None
-        odd: Optional[int] = None
-
-    def run(self, data: Input) -> Output:
-        """
-        :param value: The value to check for parity
-        """
-        remainder = data.value % 2
-        if remainder:
-            return Parity.Output(odd=data.value)
-        return Parity.Output(even=data.value)
+    @component.input  # type: ignore
+    def input(self):
+        class Input:
+            value: int
+
+        return Input
+
+    def __init__(self, outputs: List[str] = ["output_1", "output_2", "output_3"]):
+        self.outputs = outputs
+        self._output_type = make_dataclass("Output", fields=[(val, int, None) for val in outputs])
 
+    @component.output  # type: ignore
+    def output(self):
+        return self._output_type
 
-class TestParity(BaseTestComponent):
+    def run(self, data):
+        output_dataclass = self.output()
+        for output in self.outputs:
+            setattr(output_dataclass, output, data.value)
+        return output_dataclass
+
+
+class TestRepeat(BaseTestComponent):
     def test_saveload_default(self, tmp_path):
-        self.assert_can_be_saved_and_loaded_in_pipeline(Parity(), tmp_path)
+        self.assert_can_be_saved_and_loaded_in_pipeline(Repeat(), tmp_path)
+
+    def test_saveload_outputs(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(Repeat(outputs=["one", "two"]), tmp_path)
 
-    def test_parity(self):
-        component = Parity()
-        results = component.run(Parity.Input(value=1))
-        assert results == Parity.Output(odd=1)
-        results = component.run(Parity.Input(value=2))
-        assert results == Parity.Output(even=2)
+    def test_repeat_default(self):
+        component = Repeat()
+        results = component.run(component.input(value=10))
+        assert results == component.output(output_1=10, output_2=10, output_3=10)
+        assert component.init_parameters == {}
+
+    def test_repeat_init(self):
+        component = Repeat(outputs=["one", "two"])
+        results = component.run(component.input(value=10))
+        assert results == component.output(one=10, two=10)
+        assert component.init_parameters == {"outputs": ["one", "two"]}
```

### Comparing `canals-0.2.2/test/sample_components/test_remainder.py` & `canals-0.3.1/test/sample_components/test_remainder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,67 +1,69 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
-from dataclasses import dataclass, make_dataclass
+from dataclasses import make_dataclass
 
 import pytest
 
 from canals.testing import BaseTestComponent
-from canals.component import component, ComponentInput, ComponentOutput
+from canals.component import component
 
 
 @component
 class Remainder:
     """
     Redirects the value, unchanged, along the connection corresponding to the remainder
     of a division. For example, if `divisor=3`, the value `5` would be sent along
     the second output connection.
     """
 
-    @dataclass
-    class Input(ComponentInput):
-        value: int
-        add: int = 1
+    @component.input  # type: ignore
+    def input(self):
+        class Input:
+            value: int
+
+        return Input
 
     def __init__(self, divisor: int = 2):
         if divisor == 0:
             raise ValueError("Can't divide by zero")
         self.divisor = divisor
 
         self._output_type = make_dataclass(
-            "Output", fields=[(f"remainder_is_{val}", int, None) for val in range(divisor)], bases=(ComponentOutput,)
+            "Output", fields=[(f"remainder_is_{val}", int, None) for val in range(divisor)]
         )
 
-    @property
-    def output_type(self):
+    @component.output  # type: ignore
+    def output(self):
         return self._output_type
 
-    def run(self, data: Input):
+    def run(self, data):
         """
         :param value: the value to check the remainder of.
         """
         remainder = data.value % self.divisor
-        output = self.output_type()
+        output = self.output()
         setattr(output, f"remainder_is_{remainder}", data.value)
         return output
 
 
 class TestRemainder(BaseTestComponent):
     def test_saveload_default(self, tmp_path):
         self.assert_can_be_saved_and_loaded_in_pipeline(Remainder(), tmp_path)
 
     def test_saveload_divisor(self, tmp_path):
         self.assert_can_be_saved_and_loaded_in_pipeline(Remainder(divisor=1), tmp_path)
 
     def test_remainder_default(self):
         component = Remainder()
-        results = component.run(Remainder.Input(value=3))
-        assert results == component.output_type(remainder_is_1=3)
+        results = component.run(component.input(value=3))
+        assert results == component.output(remainder_is_1=3)
 
     def test_remainder_with_divisor(self):
         component = Remainder(divisor=4)
-        results = component.run(Remainder.Input(value=3))
-        assert results == component.output_type(remainder_is_3=3)
+        results = component.run(component.input(value=3))
+        assert results == component.output(remainder_is_3=3)
 
     def test_remainder_zero(self):
         with pytest.raises(ValueError):
             Remainder(divisor=0)
```

### Comparing `canals-0.2.2/test/sample_components/test_threshold.py` & `canals-0.3.1/test/sample_components/test_threshold.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 from typing import Optional
 
-from dataclasses import dataclass
-
-import pytest
 
 from canals.testing import BaseTestComponent
-from canals.component import component, ComponentInput, ComponentOutput
+from canals.component import component
 
 
 @component
 class Threshold:
     """
     Redirects the value, unchanged, along a different connection whether the value is above
     or below the given threshold.
 
     Single input, double output decision component.
 
     :param threshold: the number to compare the input value against. This is also a parameter.
     """
 
-    @dataclass
-    class Input(ComponentInput):
-        value: int
-        threshold: int = 10
-
-    @dataclass
-    class Output(ComponentOutput):
-        above: int
-        below: int
+    @component.input  # type: ignore
+    def input(self):
+        class Input:
+            value: int
+            threshold: int = 10
+
+        return Input
+
+    @component.output  # type: ignore
+    def output(self):
+        class Output:
+            above: int
+            below: int
+
+        return Output
 
     def __init__(self, threshold: Optional[int] = None):
         """
         :param threshold: the number to compare the input value against.
         """
         if threshold:
             self.defaults = {"threshold": threshold}
 
-    def run(self, data: Input) -> Output:
+    def run(self, data):
         if data.value < data.threshold:
-            return Threshold.Output(above=None, below=data.value)  # type: ignore
-        return Threshold.Output(above=data.value, below=None)  # type: ignore
+            return self.output(above=None, below=data.value)
+        return self.output(above=data.value, below=None)
 
 
 class TestThreshold(BaseTestComponent):
     def test_saveload_default(self, tmp_path):
         self.assert_can_be_saved_and_loaded_in_pipeline(Threshold(), tmp_path)
 
     def test_saveload_threshold(self, tmp_path):
         self.assert_can_be_saved_and_loaded_in_pipeline(Threshold(threshold=3), tmp_path)
 
     def test_threshold(self):
         component = Threshold()
 
-        results = component.run(Threshold.Input(value=5, threshold=10))
-        assert results == Threshold.Output(above=None, below=5)
+        results = component.run(component.input(value=5, threshold=10))
+        assert results == component.output(above=None, below=5)
 
-        results = component.run(Threshold.Input(value=15, threshold=10))
-        assert results == Threshold.Output(above=15, below=None)
+        results = component.run(component.input(value=15, threshold=10))
+        assert results == component.output(above=15, below=None)
```

### Comparing `canals-0.2.2/.gitignore` & `canals-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `canals-0.2.2/LICENSE` & `canals-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `canals-0.2.2/README.md` & `canals-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 ```console
 pip install canals
 ```
 
 gives you the bare minimum necessary to run Canals.
 
-To be able to draw pipelines, please make sure you have either an internet connection (to reach the Mermaid graph renderer at `https://mermaid.ink`) or [graphviz](https://graphviz.org/download/) installed and then install Canals as:
+To be able to draw pipelines, please make sure you have either an internet connection (to reach the Mermaid graph renderer at `https://mermaid.ink`) or [graphviz](https://graphviz.org/download/) (version 2.49.0) installed and then install Canals as:
 
 ### Mermaid
 ```console
 pip install canals[mermaid]
 ```
 
 ### GraphViz
```

#### html2text {}

```diff
@@ -12,11 +12,11 @@
 of components and takes care of managing their execution order, making sure
 that each object receives the input it expects from the other components of the
 pipeline. Canals powers version 2.0 of the [Haystack framework](https://
 github.com/deepset-ai/haystack). ## Installation Running: ```console pip
 install canals ``` gives you the bare minimum necessary to run Canals. To be
 able to draw pipelines, please make sure you have either an internet connection
 (to reach the Mermaid graph renderer at `https://mermaid.ink`) or [graphviz]
-(https://graphviz.org/download/) installed and then install Canals as: ###
-Mermaid ```console pip install canals[mermaid] ``` ### GraphViz ```console sudo
-apt install graphviz # You may need `graphviz-dev` too pip install canals
-[graphviz] ```
+(https://graphviz.org/download/) (version 2.49.0) installed and then install
+Canals as: ### Mermaid ```console pip install canals[mermaid] ``` ### GraphViz
+```console sudo apt install graphviz # You may need `graphviz-dev` too pip
+install canals[graphviz] ```
```

### Comparing `canals-0.2.2/pyproject.toml` & `canals-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 dev = [
   "hatch",
   "pre-commit",
   "mypy",
   "pylint==2.15.10",
   "black[jupyter]==22.6.0",
   "pytest",
+  "pytest-cov",
+  "requests",
   "coverage",
 ]
 docs = [
   "mkdocs-material",
   "mkdocstrings[python]",
   "mkdocs-mermaid2-plugin"
 ]
@@ -95,9 +97,8 @@
 good-names="e"
 max-args=10
 disable = [
   "fixme",
   "line-too-long",
   "missing-class-docstring",
   "missing-module-docstring",
-  "consider-iterating-dictionary",  # horrible style imho :)
 ]
```

### Comparing `canals-0.2.2/PKG-INFO` & `canals-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canals
-Version: 0.2.2
+Version: 0.3.1
 Summary: A component orchestration engine for Haystack
 Project-URL: Documentation, https://github.com/deepset-ai/canals#readme
 Project-URL: Issues, https://github.com/deepset-ai/canals/issues
 Project-URL: Source, https://github.com/deepset-ai/canals
 Author-email: ZanSara <sara.zanzottera@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -24,14 +24,16 @@
 Requires-Dist: black[jupyter]==22.6.0; extra == 'dev'
 Requires-Dist: coverage; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pylint==2.15.10; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: requests; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocs-mermaid2-plugin; extra == 'docs'
 Requires-Dist: mkdocstrings[python]; extra == 'docs'
 Provides-Extra: graphviz
 Requires-Dist: pygraphviz; extra == 'graphviz'
 Provides-Extra: mermaid
@@ -77,15 +79,15 @@
 
 ```console
 pip install canals
 ```
 
 gives you the bare minimum necessary to run Canals.
 
-To be able to draw pipelines, please make sure you have either an internet connection (to reach the Mermaid graph renderer at `https://mermaid.ink`) or [graphviz](https://graphviz.org/download/) installed and then install Canals as:
+To be able to draw pipelines, please make sure you have either an internet connection (to reach the Mermaid graph renderer at `https://mermaid.ink`) or [graphviz](https://graphviz.org/download/) (version 2.49.0) installed and then install Canals as:
 
 ### Mermaid
 ```console
 pip install canals[mermaid]
 ```
 
 ### GraphViz
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: canals Version: 0.2.2 Summary: A component
+Metadata-Version: 2.1 Name: canals Version: 0.3.1 Summary: A component
 orchestration engine for Haystack Project-URL: Documentation, https://
 github.com/deepset-ai/canals#readme Project-URL: Issues, https://github.com/
 deepset-ai/canals/issues Project-URL: Source, https://github.com/deepset-ai/
 canals Author-email: ZanSara
 zanzottera@deepset.ai> License-Expression: Apache-2.0 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha Classifier: License :: Freely
 Distributable Classifier: License :: OSI Approved :: Apache Software License
@@ -11,15 +11,16 @@
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8 Requires-Dist: networkx Provides-Extra: dev Requires-
 Dist: black[jupyter]==22.6.0; extra == 'dev' Requires-Dist: coverage; extra ==
 'dev' Requires-Dist: hatch; extra == 'dev' Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev' Requires-Dist: pylint==2.15.10; extra
-== 'dev' Requires-Dist: pytest; extra == 'dev' Provides-Extra: docs Requires-
+== 'dev' Requires-Dist: pytest; extra == 'dev' Requires-Dist: pytest-cov; extra
+== 'dev' Requires-Dist: requests; extra == 'dev' Provides-Extra: docs Requires-
 Dist: mkdocs-material; extra == 'docs' Requires-Dist: mkdocs-mermaid2-plugin;
 extra == 'docs' Requires-Dist: mkdocstrings[python]; extra == 'docs' Provides-
 Extra: graphviz Requires-Dist: pygraphviz; extra == 'graphviz' Provides-Extra:
 mermaid Requires-Dist: requests; extra == 'mermaid' Description-Content-Type:
 text/markdown # Canals
 
 [![PyPI - Version](https://img.shields.io/pypi/v/canals.svg)](https://pypi.org/
@@ -34,11 +35,11 @@
 of components and takes care of managing their execution order, making sure
 that each object receives the input it expects from the other components of the
 pipeline. Canals powers version 2.0 of the [Haystack framework](https://
 github.com/deepset-ai/haystack). ## Installation Running: ```console pip
 install canals ``` gives you the bare minimum necessary to run Canals. To be
 able to draw pipelines, please make sure you have either an internet connection
 (to reach the Mermaid graph renderer at `https://mermaid.ink`) or [graphviz]
-(https://graphviz.org/download/) installed and then install Canals as: ###
-Mermaid ```console pip install canals[mermaid] ``` ### GraphViz ```console sudo
-apt install graphviz # You may need `graphviz-dev` too pip install canals
-[graphviz] ```
+(https://graphviz.org/download/) (version 2.49.0) installed and then install
+Canals as: ### Mermaid ```console pip install canals[mermaid] ``` ### GraphViz
+```console sudo apt install graphviz # You may need `graphviz-dev` too pip
+install canals[graphviz] ```
```


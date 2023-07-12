# Comparing `tmp/sagemaker-rightline-0.3.4.tar.gz` & `tmp/sagemaker-rightline-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-rightline-0.3.4.tar", last modified: Wed Jun 21 16:40:52 2023, max compression
+gzip compressed data, was "sagemaker-rightline-0.3.5.tar", last modified: Wed Jul 12 15:37:49 2023, max compression
```

## Comparing `sagemaker-rightline-0.3.4.tar` & `sagemaker-rightline-0.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:52.430530 sagemaker-rightline-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-06-21 16:40:52.430530 sagemaker-rightline-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:52.426530 sagemaker-rightline-0.3.4/sagemaker_rightline/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 16:40:44.000000 sagemaker-rightline-0.3.4/sagemaker_rightline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/sagemaker_rightline/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/sagemaker_rightline/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    33212 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/sagemaker_rightline/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:52.430530 sagemaker-rightline-0.3.4/sagemaker_rightline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-06-21 16:40:52.000000 sagemaker-rightline-0.3.4/sagemaker_rightline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-21 16:40:52.000000 sagemaker-rightline-0.3.4/sagemaker_rightline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:40:52.000000 sagemaker-rightline-0.3.4/sagemaker_rightline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 16:40:52.000000 sagemaker-rightline-0.3.4/sagemaker_rightline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 16:40:52.000000 sagemaker-rightline-0.3.4/sagemaker_rightline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:40:52.430530 sagemaker-rightline-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:52.430530 sagemaker-rightline-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    30149 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:37:49.779383 sagemaker-rightline-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-07-12 15:37:49.779383 sagemaker-rightline-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:37:49.779383 sagemaker-rightline-0.3.5/sagemaker_rightline/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 15:37:42.000000 sagemaker-rightline-0.3.5/sagemaker_rightline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/sagemaker_rightline/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/sagemaker_rightline/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33374 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/sagemaker_rightline/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:37:49.779383 sagemaker-rightline-0.3.5/sagemaker_rightline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-07-12 15:37:49.000000 sagemaker-rightline-0.3.5/sagemaker_rightline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-12 15:37:49.000000 sagemaker-rightline-0.3.5/sagemaker_rightline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:37:49.000000 sagemaker-rightline-0.3.5/sagemaker_rightline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-12 15:37:49.000000 sagemaker-rightline-0.3.5/sagemaker_rightline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 15:37:49.000000 sagemaker-rightline-0.3.5/sagemaker_rightline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:37:49.779383 sagemaker-rightline-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:37:49.779383 sagemaker-rightline-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31054 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/tests/test_validations.py
```

### Comparing `sagemaker-rightline-0.3.4/LICENSE` & `sagemaker-rightline-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.4/PKG-INFO` & `sagemaker-rightline-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sagemaker-rightline-0.3.4/README.md` & `sagemaker-rightline-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.4/pyproject.toml` & `sagemaker-rightline-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
 ]
 
 dependencies = [
     "boto3>=1.26",
-    "pandas==2",
+    "pandas==2.0.3",
     "sagemaker>=2.159",
 ]
 
 [project.optional-dependencies]
 dev = [
     "moto[all]",
     "pytest",
```

### Comparing `sagemaker-rightline-0.3.4/sagemaker_rightline/model.py` & `sagemaker-rightline-0.3.5/sagemaker_rightline/model.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.4/sagemaker_rightline/rules.py` & `sagemaker-rightline-0.3.5/sagemaker_rightline/rules.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.4/sagemaker_rightline/validations.py` & `sagemaker-rightline-0.3.5/sagemaker_rightline/validations.py`

 * *Files 0% similar despite different names*

```diff
@@ -736,39 +736,42 @@
         :param sagemaker_pipeline: SageMaker Pipeline
         :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
         :param step_name: Name of Step
         :type step_name: str
         :return: ProcessingStep
         :rtype: ProcessingStep
         """
-        supported_step_types = ("Processing", "Training")
+        supported_step_types = ("Processing", "Training", "Tuning")
         for step in sagemaker_pipeline.steps:
             if step.name == step_name and step.step_type.value in supported_step_types:
                 return step
-        raise ValueError(f"Processing or Training Step {step_name} not found in Pipeline.")
+        raise ValueError(f"Processing, Training or Tuning Step {step_name} not found in Pipeline.")
 
     @staticmethod
     def get_input_output_by_name(
-        step: Union["ProcessingStep", "TrainingStep"], name: str, kind: str  # noqa F821
+        step: Union["ProcessingStep", "TrainingStep", "TuningStep"],  # noqa F821
+        name: str,
+        kind: str,  # noqa F821
     ) -> str:
         """Get ProcessingInput or ProcessingOutput by name.
 
-        :param step: ProcessingStep
-        :type step: ProcessingStep
+        :param step: step to run validation on
+        :type step: Union[ProcessingStep, TrainingStep, TuningStep]
         :param name: Name of Input or Output
         :type name: str
         :param kind: Kind of Input or Output, must be one of "input" or "output"
         :type kind: str
         :return: Input or Output path
         :rtype: str
         """
         step_type = step.step_type.value
 
         if kind == "input":
-            if step_type == "Training":
+            # If TrainingStep or TuningStep
+            if step_type in ("Training", "Tuning"):
                 input = step.inputs[name]
                 if isinstance(input, TrainingInput):
                     return input.config["DataSource"]["S3DataSource"]["S3Uri"]
                 else:
                     raise ValueError(f"Input {name} is not of type TrainingInput.")
             else:
                 # If ProcessingStep
```

### Comparing `sagemaker-rightline-0.3.4/sagemaker_rightline.egg-info/PKG-INFO` & `sagemaker-rightline-0.3.5/sagemaker_rightline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sagemaker-rightline-0.3.4/tests/test_model.py` & `sagemaker-rightline-0.3.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.4/tests/test_rules.py` & `sagemaker-rightline-0.3.5/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.4/tests/test_validations.py` & `sagemaker-rightline-0.3.5/tests/test_validations.py`

 * *Files 1% similar despite different names*

```diff
@@ -945,14 +945,46 @@
                         "output_name": "output-2",
                     },
                 }
             ],
             False,
             True,
         ],
+        [
+            [
+                {
+                    "input": {
+                        "step_name": "sm_tuning_step",
+                        "input_name": "train",
+                    },
+                    "output": {
+                        "step_name": "sm_processing_step_spark",
+                        "output_name": "output-2",
+                    },
+                }
+            ],
+            True,
+            False,
+        ],
+        [
+            [
+                {
+                    "input": {
+                        "step_name": "sm_tuning_step",
+                        "input_name": "validation",
+                    },
+                    "output": {
+                        "step_name": "sm_processing_step_spark",
+                        "output_name": "output-2",
+                    },
+                }
+            ],
+            False,
+            True,
+        ],
     ],
 )
 def test_step_outputs_match_inputs_as_expected(
     sagemaker_pipeline, inputs_outputs_expected, success, raise_error
 ) -> None:
     step_outputs_validation = StepOutputsMatchInputsAsExpected(
         inputs_outputs_expected=inputs_outputs_expected,
```


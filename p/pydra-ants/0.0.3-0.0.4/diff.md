# Comparing `tmp/pydra_ants-0.0.3.tar.gz` & `tmp/pydra_ants-0.0.4.tar.gz`

## Comparing `pydra_ants-0.0.3.tar` & `pydra_ants-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/.editorconfig
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/.github/dependabot.yaml
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/.github/workflows/test.yaml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/src/pydra/tasks/ants/__init__.py
--rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/src/pydra/tasks/ants/apply_transforms.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/src/pydra/tasks/ants/bias_correction.py
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/src/pydra/tasks/ants/registration.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/LICENSE
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/README.md
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/hatch.toml
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pydra_ants-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pydra_ants-0.0.4/.editorconfig
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_ants-0.0.4/.github/dependabot.yaml
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pydra_ants-0.0.4/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pydra_ants-0.0.4/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pydra_ants-0.0.4/src/pydra/tasks/ants/__init__.py
+-rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 pydra_ants-0.0.4/src/pydra/tasks/ants/apply_transforms.py
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 pydra_ants-0.0.4/src/pydra/tasks/ants/bias_correction.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 pydra_ants-0.0.4/src/pydra/tasks/ants/create_jacobian_determinant_image.py
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 pydra_ants-0.0.4/src/pydra/tasks/ants/registration.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 pydra_ants-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_ants-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 pydra_ants-0.0.4/README.md
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pydra_ants-0.0.4/hatch.toml
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pydra_ants-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 pydra_ants-0.0.4/PKG-INFO
```

### Comparing `pydra_ants-0.0.3/.github/workflows/publish.yaml` & `pydra_ants-0.0.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `pydra_ants-0.0.3/.github/workflows/test.yaml` & `pydra_ants-0.0.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pydra_ants-0.0.3/src/pydra/tasks/ants/apply_transforms.py` & `pydra_ants-0.0.4/src/pydra/tasks/ants/apply_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,24 +98,29 @@
         output_image: str = field(
             metadata={"help_string": "output image", "output_file_template": "{moving_image}_warped"}
         )
 
         save_warp_field: bool = field(metadata={"help_string": "save composite warp field"})
 
         output_warp_field: str = field(
-            metadata={"help_string": "output warp field", "output_file_template": "{moving_image}_warpfield"}
+            metadata={
+                "help_string": "output warp field",
+                "output_file_template": "{moving_image}_warpfield",
+                "requires": {"save_warp_field"},
+            }
         )
 
         save_transform: bool = field(metadata={"help_string": "save composite transform"})
 
         output_transform: str = field(
             metadata={
                 "help_string": "output transform",
                 "output_file_template": "{moving_image}_affine.mat",
                 "keep_extension": False,
+                "requires": {"save_transform"},
             }
         )
 
         invert_transform: bool = field(default=False, metadata={"help_string": "invert composite transform"})
 
         interpolation: str = field(
             default="Linear",
```

### Comparing `pydra_ants-0.0.3/src/pydra/tasks/ants/bias_correction.py` & `pydra_ants-0.0.4/src/pydra/tasks/ants/bias_correction.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,16 +105,20 @@
             }
         )
 
         output_image: str = field(
             metadata={"help_string": "output image", "output_file_template": "{input_image}_corrected"}
         )
 
-        save_bias_field: bool = field(default=False, metadata={"help_string": "save bias field"})
+        save_bias_field: bool = field(metadata={"help_string": "save bias field"})
 
         output_bias_field: str = field(
-            metadata={"help_string": "output bias field", "output_file_template": "{input_image}_biasfield"}
+            metadata={
+                "help_string": "output bias field",
+                "output_file_template": "{input_image}_biasfield",
+                "requires": {"save_bias_field"},
+            }
         )
 
     input_spec = SpecInfo(name="Input", bases=(InputSpec,))
 
     executable = "N4BiasFieldCorrection"
```

### Comparing `pydra_ants-0.0.3/src/pydra/tasks/ants/registration.py` & `pydra_ants-0.0.4/src/pydra/tasks/ants/registration.py`

 * *Files identical despite different names*

### Comparing `pydra_ants-0.0.3/.gitignore` & `pydra_ants-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pydra_ants-0.0.3/LICENSE` & `pydra_ants-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra_ants-0.0.3/README.md` & `pydra_ants-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 - [Installation](#installation)
 - [Development](#development)
 - [License](#license)
 
 ## Available Tasks
 
 - ApplyTransforms
+- CreateJacobianDeterminantImage
 - N4BiasFieldCorrection
 - RegistrationSyNQuick
 
 ## Installation
 
 ```console
 pip install pydra-ants
```

### Comparing `pydra_ants-0.0.3/pyproject.toml` & `pydra_ants-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pydra-ants"
-version = "0.0.3"
+version = "0.0.4"
 description = "Pydra tasks for ANTs"
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = [
   "ants",
   "neuroimaging",
```

### Comparing `pydra_ants-0.0.3/PKG-INFO` & `pydra_ants-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydra-ants
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pydra tasks for ANTs
 Project-URL: Documentation, https://github.com/ghisvail/pydra-ants#readme
 Project-URL: Issues, https://github.com/ghisvail/pydra-ants/issues
 Project-URL: Source, https://github.com/ghisvail/pydra-ants
 Author-email: Ghislain Vaillant <ghislain.vaillant@icm-institute.org>
 License-Expression: MIT
 License-File: LICENSE
@@ -50,14 +50,15 @@
 - [Installation](#installation)
 - [Development](#development)
 - [License](#license)
 
 ## Available Tasks
 
 - ApplyTransforms
+- CreateJacobianDeterminantImage
 - N4BiasFieldCorrection
 - RegistrationSyNQuick
 
 ## Installation
 
 ```console
 pip install pydra-ants
```


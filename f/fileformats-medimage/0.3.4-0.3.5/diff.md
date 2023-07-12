# Comparing `tmp/fileformats_medimage-0.3.4.tar.gz` & `tmp/fileformats_medimage-0.3.5.tar.gz`

## Comparing `fileformats_medimage-0.3.4.tar` & `fileformats_medimage-0.3.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/.codespell-ignorewords
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/.coveragerc
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/.flake8
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/conftest.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/pytest.ini
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/fileformats/medimage/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/fileformats/medimage/_version.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/fileformats/medimage/base.py
--rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/fileformats/medimage/converters.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/fileformats/medimage/dicom.py
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/fileformats/medimage/diffusion.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/fileformats/medimage/misc.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/fileformats/medimage/mrtrix.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/fileformats/medimage/nifti.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/fileformats/medimage/raw.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/fileformats/medimage/tests/test_neuro_converters.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/LICENSE
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/README.rst
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    19509 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/.codespell-ignorewords
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/.coveragerc
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/.flake8
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/conftest.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/pytest.ini
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/_version.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/base.py
+-rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/converters.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/dicom.py
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/diffusion.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/misc.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/mrtrix.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/nifti.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/raw.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/tests/test_neuro_converters.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/README.rst
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0    19496 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/PKG-INFO
```

### Comparing `fileformats_medimage-0.3.4/.pre-commit-config.yaml` & `fileformats_medimage-0.3.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.4/conftest.py` & `fileformats_medimage-0.3.5/conftest.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.4/.github/workflows/publish.yml` & `fileformats_medimage-0.3.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.4/.github/workflows/tests.yml` & `fileformats_medimage-0.3.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.4/fileformats/medimage/__init__.py` & `fileformats_medimage-0.3.5/fileformats/medimage/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.4/fileformats/medimage/base.py` & `fileformats_medimage-0.3.5/fileformats/medimage/base.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.4/fileformats/medimage/converters.py` & `fileformats_medimage-0.3.5/fileformats/medimage/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 from pathlib import Path
 import attrs
 import json
+import typing as ty
 import tempfile
 from fileformats.core import mark
 from fileformats.core.utils import MissingExtendedDependency
 from fileformats.medimage.base import MedicalImage
 from fileformats.medimage.dicom import DicomDir, DicomCollection, DicomSet
 from fileformats.medimage import (
     Analyze,
@@ -88,17 +89,17 @@
 @mark.converter(source_format=DicomCollection, target_format=NiftiGzBvec)
 @mark.converter(
     source_format=DicomCollection, target_format=NiftiGzXBvec, compress="y"
 )
 def extended_dcm2niix(
     name,
     compress: str = "n",
-    file_postfix: str = None,
-    side_car_jq: str = None,
-    extract_volume: int = None,
+    file_postfix: ty.Optional[str] = None,
+    side_car_jq: ty.Optional[str] = None,
+    extract_volume: ty.Optional[int] = None,
     to_4d: bool = False,
 ):
     """The Dcm2niix command wrapped in a workflow in order to map the inputs and outputs
     onto "in_file" and "out_file", respectively, and implement optional post-conversion
     manipulations to allow manual override of conversion issues.
 
     Parameters
```

### Comparing `fileformats_medimage-0.3.4/fileformats/medimage/dicom.py` & `fileformats_medimage-0.3.5/fileformats/medimage/dicom.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.4/fileformats/medimage/diffusion.py` & `fileformats_medimage-0.3.5/fileformats/medimage/diffusion.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.4/fileformats/medimage/mrtrix.py` & `fileformats_medimage-0.3.5/fileformats/medimage/mrtrix.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.4/fileformats/medimage/nifti.py` & `fileformats_medimage-0.3.5/fileformats/medimage/nifti.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.4/fileformats/medimage/raw.py` & `fileformats_medimage-0.3.5/fileformats/medimage/raw.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.4/fileformats/medimage/tests/test_neuro_converters.py` & `fileformats_medimage-0.3.5/fileformats/medimage/tests/test_neuro_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.4/LICENSE` & `fileformats_medimage-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.4/README.rst` & `fileformats_medimage-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.4/pyproject.toml` & `fileformats_medimage-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 [project]
 name = "fileformats-medimage"
 description = "Classes for representing various medical imaging file formats in Python classes for use in type hinting in data workflows"
 readme = "README.rst"
 requires-python = ">=3.7"
 dependencies = [
+    "numpy >= 1.24",
     "fileformats >=0.4.0",
 ]
 license = {file = "LICENSE"}
 authors = [
     {name = "Thomas G. Close", email = "tom.g.close@gmail.com"},
 ]
 maintainers = [
@@ -47,15 +48,14 @@
     "flake8-pyproject",
 ]
 test = [
     "pytest >=6.2.5",
     "pytest-env>=0.6.2",
     "pytest-cov>=2.12.1",
     "medimages4tests >=0.3",
-    "codecov",
 ]
 
 extended = [
     "pydra >= 0.20.0",
     "pydra-dcm2niix",
     "pydra-mrtrix3",
     "numpy >=1.20",
```

### Comparing `fileformats_medimage-0.3.4/PKG-INFO` & `fileformats_medimage-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats-medimage
-Version: 0.3.4
+Version: 0.3.5
 Summary: Classes for representing various medical imaging file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-medimage
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -109,14 +109,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Requires-Dist: fileformats>=0.4.0
+Requires-Dist: numpy>=1.24
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: codespell; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: flake8-pyproject; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: extended
@@ -125,15 +126,14 @@
 Requires-Dist: nibabel>=5.0.0; extra == 'extended'
 Requires-Dist: numpy>=1.20; extra == 'extended'
 Requires-Dist: pydicom>=2.3.1; extra == 'extended'
 Requires-Dist: pydra-dcm2niix; extra == 'extended'
 Requires-Dist: pydra-mrtrix3; extra == 'extended'
 Requires-Dist: pydra>=0.20.0; extra == 'extended'
 Provides-Extra: test
-Requires-Dist: codecov; extra == 'test'
 Requires-Dist: medimages4tests>=0.3; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=6.2.5; extra == 'test'
 Description-Content-Type: text/x-rst
 
 FileFormats Extension - Medimage
```


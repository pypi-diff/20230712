# Comparing `tmp/ssb_altinn_python-0.3.2.tar.gz` & `tmp/ssb_altinn_python-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_altinn_python-0.3.2.tar", max compression
+gzip compressed data, was "ssb_altinn_python-0.3.3.tar", max compression
```

## Comparing `ssb_altinn_python-0.3.2.tar` & `ssb_altinn_python-0.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-07-10 16:47:50.446190 ssb_altinn_python-0.3.2/LICENSE
--rw-r--r--   0        0        0     3941 2023-07-10 16:47:50.446190 ssb_altinn_python-0.3.2/README.md
--rw-r--r--   0        0        0     1967 2023-07-10 16:48:11.427420 ssb_altinn_python-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      185 2023-07-10 16:48:11.427420 ssb_altinn_python-0.3.2/src/altinn/__init__.py
--rw-r--r--   0        0        0      198 2023-07-10 16:47:50.450191 ssb_altinn_python-0.3.2/src/altinn/__main__.py
--rw-r--r--   0        0        0     1831 2023-07-10 16:47:50.450191 ssb_altinn_python-0.3.2/src/altinn/file.py
--rw-r--r--   0        0        0     2179 2023-07-10 16:48:11.427420 ssb_altinn_python-0.3.2/src/altinn/flatten.py
--rw-r--r--   0        0        0     4007 2023-07-10 16:48:11.427420 ssb_altinn_python-0.3.2/src/altinn/parser.py
--rw-r--r--   0        0        0        0 2023-07-10 16:47:50.450191 ssb_altinn_python-0.3.2/src/altinn/py.typed
--rw-r--r--   0        0        0     1236 2023-07-10 16:48:11.427420 ssb_altinn_python-0.3.2/src/altinn/utils.py
--rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 ssb_altinn_python-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-12 14:06:27.765210 ssb_altinn_python-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4739 2023-07-12 14:06:46.133237 ssb_altinn_python-0.3.3/README.md
+-rw-r--r--   0        0        0     1967 2023-07-12 14:06:46.133237 ssb_altinn_python-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      185 2023-07-12 14:06:27.769210 ssb_altinn_python-0.3.3/src/altinn/__init__.py
+-rw-r--r--   0        0        0      198 2023-07-12 14:06:27.769210 ssb_altinn_python-0.3.3/src/altinn/__main__.py
+-rw-r--r--   0        0        0     1831 2023-07-12 14:06:27.769210 ssb_altinn_python-0.3.3/src/altinn/file.py
+-rw-r--r--   0        0        0     2673 2023-07-12 14:06:46.133237 ssb_altinn_python-0.3.3/src/altinn/flatten.py
+-rw-r--r--   0        0        0     4007 2023-07-12 14:06:27.769210 ssb_altinn_python-0.3.3/src/altinn/parser.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:06:27.769210 ssb_altinn_python-0.3.3/src/altinn/py.typed
+-rw-r--r--   0        0        0     1236 2023-07-12 14:06:27.769210 ssb_altinn_python-0.3.3/src/altinn/utils.py
+-rw-r--r--   0        0        0     5668 1970-01-01 00:00:00.000000 ssb_altinn_python-0.3.3/PKG-INFO
```

### Comparing `ssb_altinn_python-0.3.2/LICENSE` & `ssb_altinn_python-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.3.2/README.md` & `ssb_altinn_python-0.3.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -12,55 +12,85 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
 [pypi_]: https://pypi.org/project/ssb-altinn-python/
 [status]: https://pypi.org/project/ssb-altinn-python/
 [python version]: https://pypi.org/project/ssb-altinn-python
 [read the docs]: https://ssb-altinn-python.readthedocs.io/
-[tests]: https://github.com/skars82/ssb-altinn-python/actions?workflow=Tests
-[codecov]: https://app.codecov.io/gh/skars82/ssb-altinn-python
+[tests]: https://github.com/statisticsnorway/ssb-altinn-python/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/statisticsnorway/ssb-altinn-python
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
 ## Features
 
-This is work-in-progress Python-package for dealing with xml-data from Altinn3.
+This is work-in-progress Python-package for dealing with xml-data from Altinn3. Here are some examples of how it can be used:
+
+### Get information about a file
 
 ```python
-from altinn import FileInfo, ParseSingleXml
+from altinn import FileInfo
 
 file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/form_dc551844cd74.xml"
 
 # Create an instance of FileInfo
 form = FileInfo(file)
 
-# Create an instance of ParseSingleXml
-form_content = ParseSingleXml(file)
-
 # Get file filename without '.xml'-postfix
 form.filename()
 # Returns: 'form_dc551844cd74'
 
-# Print a nicely formatted version of the file
-form.pretty_print()
-
 # Print an unformatted version of the file. Does not require the file to be parseable by an xml-library. Useful for inspecting unvalid xml-files.
 form.print()
 
+# Print a nicely formatted version of the file
+form.pretty_print()
+
 # Check if xml-file is valid. Useful to inspect xml-files with formal errors in the xml-schema.
 form.validate()
 # Returns True og False
+```
+
+### Parse xml-file
 
-# Get a dictionary representation of the contents of the file
-form_content.to_dict()
+If you want to transform an Altinn3 xml-file to a Pandas Dataframe, you can use the ParseSingleXml-class.
+
+```python
+from altinn import ParseSingleXml
+
+file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/form_dc551844cd74.xml"
 
 # Get a Pandas Dataframe representation of the contents of the file
 form_content.to_dataframe()
 ```
 
+### Tramsform to ISEE-Dynarev format
+
+If you want to transform an Altinn3 xml-file to a Pandas Dataframe, in the same form as the ISEE Dynarev database in our on-prem environment, you can use the `isee_transform`-function.
+
+```python
+from altinn import isee_transform
+
+file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/form_dc551844cd74.xml"
+
+isee_transform(file)
+```
+
+The resulting object is a Pandas Dataframe with the following columns:
+
+- `Skjema_id`
+- `Delreg_nr`
+- `Ident_nr`
+- `Enhets_type`
+- `feltnavn`
+- `feltverdi`
+- `version_nr`
+
+This dataframe can be written to csv and uploaded to the ISEE Dynarev database.
+
 ## Requirements
 
 - dapla-toolbelt >=1.6.2,<2.0.0
 - defusedxml >=0.7.1,<0.8.0
 - pytest >=7.2.2,<8.0.0
 
 ## Installation
```

### Comparing `ssb_altinn_python-0.3.2/pyproject.toml` & `ssb_altinn_python-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-altinn-python"
-version = "0.3.2"
+version = "0.3.3"
 description = "SSB Altinn Python"
 authors = ["Øyvind Bruer-Skarsbø <obr@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/skars82/ssb-altinn-python"
 repository = "https://github.com/skars82/ssb-altinn-python"
 documentation = "https://ssb-altinn-python.readthedocs.io"
```

### Comparing `ssb_altinn_python-0.3.2/src/altinn/file.py` & `ssb_altinn_python-0.3.3/src/altinn/file.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.3.2/src/altinn/parser.py` & `ssb_altinn_python-0.3.3/src/altinn/parser.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.3.2/src/altinn/utils.py` & `ssb_altinn_python-0.3.3/src/altinn/utils.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.3.2/PKG-INFO` & `ssb_altinn_python-0.3.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-altinn-python
-Version: 0.3.2
+Version: 0.3.3
 Summary: SSB Altinn Python
 Home-page: https://github.com/skars82/ssb-altinn-python
 License: MIT
 Author: Øyvind Bruer-Skarsbø
 Author-email: obr@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -35,55 +35,85 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
 [pypi_]: https://pypi.org/project/ssb-altinn-python/
 [status]: https://pypi.org/project/ssb-altinn-python/
 [python version]: https://pypi.org/project/ssb-altinn-python
 [read the docs]: https://ssb-altinn-python.readthedocs.io/
-[tests]: https://github.com/skars82/ssb-altinn-python/actions?workflow=Tests
-[codecov]: https://app.codecov.io/gh/skars82/ssb-altinn-python
+[tests]: https://github.com/statisticsnorway/ssb-altinn-python/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/statisticsnorway/ssb-altinn-python
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
 ## Features
 
-This is work-in-progress Python-package for dealing with xml-data from Altinn3.
+This is work-in-progress Python-package for dealing with xml-data from Altinn3. Here are some examples of how it can be used:
+
+### Get information about a file
 
 ```python
-from altinn import FileInfo, ParseSingleXml
+from altinn import FileInfo
 
 file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/form_dc551844cd74.xml"
 
 # Create an instance of FileInfo
 form = FileInfo(file)
 
-# Create an instance of ParseSingleXml
-form_content = ParseSingleXml(file)
-
 # Get file filename without '.xml'-postfix
 form.filename()
 # Returns: 'form_dc551844cd74'
 
-# Print a nicely formatted version of the file
-form.pretty_print()
-
 # Print an unformatted version of the file. Does not require the file to be parseable by an xml-library. Useful for inspecting unvalid xml-files.
 form.print()
 
+# Print a nicely formatted version of the file
+form.pretty_print()
+
 # Check if xml-file is valid. Useful to inspect xml-files with formal errors in the xml-schema.
 form.validate()
 # Returns True og False
+```
+
+### Parse xml-file
 
-# Get a dictionary representation of the contents of the file
-form_content.to_dict()
+If you want to transform an Altinn3 xml-file to a Pandas Dataframe, you can use the ParseSingleXml-class.
+
+```python
+from altinn import ParseSingleXml
+
+file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/form_dc551844cd74.xml"
 
 # Get a Pandas Dataframe representation of the contents of the file
 form_content.to_dataframe()
 ```
 
+### Tramsform to ISEE-Dynarev format
+
+If you want to transform an Altinn3 xml-file to a Pandas Dataframe, in the same form as the ISEE Dynarev database in our on-prem environment, you can use the `isee_transform`-function.
+
+```python
+from altinn import isee_transform
+
+file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/form_dc551844cd74.xml"
+
+isee_transform(file)
+```
+
+The resulting object is a Pandas Dataframe with the following columns:
+
+- `Skjema_id`
+- `Delreg_nr`
+- `Ident_nr`
+- `Enhets_type`
+- `feltnavn`
+- `feltverdi`
+- `version_nr`
+
+This dataframe can be written to csv and uploaded to the ISEE Dynarev database.
+
 ## Requirements
 
 - dapla-toolbelt >=1.6.2,<2.0.0
 - defusedxml >=0.7.1,<0.8.0
 - pytest >=7.2.2,<8.0.0
 
 ## Installation
```


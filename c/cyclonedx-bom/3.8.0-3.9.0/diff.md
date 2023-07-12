# Comparing `tmp/cyclonedx_bom-3.8.0.tar.gz` & `tmp/cyclonedx_bom-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclonedx_bom-3.8.0.tar", max compression
+gzip compressed data, was "cyclonedx_bom-3.9.0.tar", max compression
```

## Comparing `cyclonedx_bom-3.8.0.tar` & `cyclonedx_bom-3.9.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    11341 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/LICENSE
--rw-r--r--   0        0        0      143 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/NOTICE
--rw-r--r--   0        0        0     6362 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/README.md
--rw-r--r--   0        0        0      658 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/cyclonedx_py/__init__.py
--rw-r--r--   0        0        0      713 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/cyclonedx_py/__main__.py
--rw-r--r--   0        0        0    13815 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/cyclonedx_py/client.py
--rw-r--r--   0        0        0      683 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/cyclonedx_py/exception/__init__.py
--rw-r--r--   0        0        0      732 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/cyclonedx_py/exception/parser.py
--rw-r--r--   0        0        0      866 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/cyclonedx_py/parser/__init__.py
--rw-r--r--   0        0        0     4012 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/cyclonedx_py/parser/conda.py
--rw-r--r--   0        0        0     4252 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/cyclonedx_py/parser/environment.py
--rw-r--r--   0        0        0     2655 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/cyclonedx_py/parser/pipenv.py
--rw-r--r--   0        0        0     2655 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/cyclonedx_py/parser/poetry.py
--rw-r--r--   0        0        0     3330 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/cyclonedx_py/parser/requirements.py
--rw-r--r--   0        0        0      153 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/cyclonedx_py/py.typed
--rw-r--r--   0        0        0      691 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/cyclonedx_py/utils/__init__.py
--rw-r--r--   0        0        0     5546 2022-12-12 16:28:36.780001 cyclonedx_bom-3.8.0/cyclonedx_py/utils/conda.py
--rw-r--r--   0        0        0     3020 2022-12-12 16:28:56.116003 cyclonedx_bom-3.8.0/pyproject.toml
--rw-r--r--   0        0        0     7744 1970-01-01 00:00:00.000000 cyclonedx_bom-3.8.0/setup.py
--rw-r--r--   0        0        0     8224 1970-01-01 00:00:00.000000 cyclonedx_bom-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/LICENSE
+-rw-r--r--   0        0        0      143 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/NOTICE
+-rw-r--r--   0        0        0     6362 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/README.md
+-rw-r--r--   0        0        0      658 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/cyclonedx_py/__init__.py
+-rw-r--r--   0        0        0      713 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/cyclonedx_py/__main__.py
+-rw-r--r--   0        0        0    14605 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/cyclonedx_py/client.py
+-rw-r--r--   0        0        0      683 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/cyclonedx_py/exception/__init__.py
+-rw-r--r--   0        0        0      732 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/cyclonedx_py/exception/parser.py
+-rw-r--r--   0        0        0      866 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/cyclonedx_py/parser/__init__.py
+-rw-r--r--   0        0        0     1362 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/cyclonedx_py/parser/_debug.py
+-rw-r--r--   0        0        0     4795 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/cyclonedx_py/parser/conda.py
+-rw-r--r--   0        0        0     5038 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/cyclonedx_py/parser/environment.py
+-rw-r--r--   0        0        0     3342 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/cyclonedx_py/parser/pipenv.py
+-rw-r--r--   0        0        0     3404 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/cyclonedx_py/parser/poetry.py
+-rw-r--r--   0        0        0     4035 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/cyclonedx_py/parser/requirements.py
+-rw-r--r--   0        0        0      153 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/cyclonedx_py/py.typed
+-rw-r--r--   0        0        0      691 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/cyclonedx_py/utils/__init__.py
+-rw-r--r--   0        0        0     5546 2022-12-13 17:24:54.402092 cyclonedx_bom-3.9.0/cyclonedx_py/utils/conda.py
+-rw-r--r--   0        0        0     3047 2022-12-13 17:25:09.538092 cyclonedx_bom-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7744 1970-01-01 00:00:00.000000 cyclonedx_bom-3.9.0/setup.py
+-rw-r--r--   0        0        0     8224 1970-01-01 00:00:00.000000 cyclonedx_bom-3.9.0/PKG-INFO
```

### Comparing `cyclonedx_bom-3.8.0/LICENSE` & `cyclonedx_bom-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclonedx_bom-3.8.0/README.md` & `cyclonedx_bom-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cyclonedx_bom-3.8.0/cyclonedx_py/__init__.py` & `cyclonedx_bom-3.9.0/cyclonedx_py/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_bom-3.8.0/cyclonedx_py/__main__.py` & `cyclonedx_bom-3.9.0/cyclonedx_py/__main__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_bom-3.8.0/cyclonedx_py/client.py` & `cyclonedx_bom-3.9.0/cyclonedx_py/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # Copyright (c) OWASP Foundation. All Rights Reserved.
 
 import argparse
 import enum
 import os
 import sys
 from datetime import datetime
-from typing import Optional
+from typing import Any, Optional
 
 from cyclonedx.model import Tool
 from cyclonedx.model.bom import Bom
 from cyclonedx.output import BaseOutput, OutputFormat, SchemaVersion, get_instance as get_output_instance
 from cyclonedx.parser import BaseParser
 
 from .parser.conda import CondaListExplicitParser, CondaListJsonParser
@@ -70,27 +70,27 @@
 
     def __init__(self, args: argparse.Namespace) -> None:
         self._arguments = args
 
         if self._arguments.debug_enabled:
             self._DEBUG_ENABLED = True
             self._debug_message('!!! DEBUG MODE ENABLED !!!')
-            self._debug_message('Parsed Arguments: {}'.format(self._arguments))
+            self._debug_message('Parsed Arguments: {}', self._arguments)
 
     def _get_output_format(self) -> _CLI_OUTPUT_FORMAT:
         return _CLI_OUTPUT_FORMAT(str(self._arguments.output_format).lower())
 
     def get_output(self) -> BaseOutput:
         try:
             parser = self._get_input_parser()
-        except CycloneDxCmdNoInputFileSupplied as e:
-            print(f'ERROR: {str(e)}', file=sys.stderr)
+        except CycloneDxCmdNoInputFileSupplied as error:
+            print(f'ERROR: {str(error)}', file=sys.stderr)
             exit(1)
-        except CycloneDxCmdException as e:
-            print(f'ERROR: {str(e)}', file=sys.stderr)
+        except CycloneDxCmdException as error:
+            print(f'ERROR: {str(error)}', file=sys.stderr)
             exit(1)
 
         if parser and parser.has_warnings():
             print('',
                   '!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!',
                   '!! Some of your dependencies do not have pinned version !!',
                   '!! numbers in your requirements.txt                     !!',
@@ -130,35 +130,35 @@
             schema_version=SchemaVersion['V{}'.format(
                 str(self._arguments.output_schema_version).replace('.', '_')
             )]
         )
 
     def execute(self) -> None:
         output_format = self._get_output_format()
-        self._debug_message(f'output_format: {output_format}')
+        self._debug_message('output_format: {}', output_format)
 
         # Quick check for JSON && SchemaVersion <= 1.1
         if output_format == OutputFormat.JSON and \
                 str(self._arguments.output_schema_version) in ['1.0', '1.1']:
             self._error_and_exit(
-                message='CycloneDX schema does not support JSON output in Schema Versions < 1.2',
+                'CycloneDX schema does not support JSON output in Schema Versions < 1.2',
                 exit_code=2
             )
 
         output = self.get_output()
         if self._arguments.output_file == '-' or not self._arguments.output_file:
             self._debug_message('Returning SBOM to STDOUT')
             print(output.output_as_string(), file=sys.stdout)
             return
 
         # Check directory writable
         output_file = self._arguments.output_file
         output_filename = os.path.realpath(
             output_file if isinstance(output_file, str) else _output_default_filenames[output_format])
-        self._debug_message('Will be outputting SBOM to file at: {}'.format(output_filename))
+        self._debug_message('Will be outputting SBOM to file at: {}', output_filename)
         output.output_to_file(filename=output_filename, allow_overwrite=self._arguments.output_file_overwrite)
 
     @staticmethod
     def get_arg_parser(*, prog: Optional[str] = None) -> argparse.ArgumentParser:
         arg_parser = argparse.ArgumentParser(prog=prog, description='CycloneDX SBOM Generator')
 
         input_group = arg_parser.add_mutually_exclusive_group(required=True)
@@ -236,71 +236,91 @@
             help='Use a component''s purl for the bom-ref value, instead of a random UUID'
         )
 
         arg_parser.add_argument('-X', action='store_true', help='Enable debug output', dest='debug_enabled')
 
         return arg_parser
 
-    def _debug_message(self, message: str) -> None:
+    def _debug_message(self, message: str, *args: Any, **kwargs: Any) -> None:
         if self._DEBUG_ENABLED:
-            print('[DEBUG] - {} - {}'.format(datetime.now(), message), file=sys.stderr)
+            print(f'[DEBUG] - {{__t}} - {message}'.format(*args, **kwargs, __t=datetime.now()),
+                  file=sys.stderr)
 
     @staticmethod
-    def _error_and_exit(message: str, exit_code: int = 1) -> None:
-        print('[ERROR] - {} - {}'.format(datetime.now(), message), file=sys.stderr)
+    def _error_and_exit(message: str, *args: Any, exit_code: int = 1, **kwargs: Any) -> None:
+        print(f'[ERROR] - {{__t}} - {message}'.format(*args, **kwargs, __t=datetime.now()),
+              file=sys.stderr)
         exit(exit_code)
 
     def _get_input_parser(self) -> BaseParser:
         if self._arguments.input_from_environment:
-            return EnvironmentParser(use_purl_bom_ref=self._arguments.use_purl_bom_ref)
+            return EnvironmentParser(
+                use_purl_bom_ref=self._arguments.use_purl_bom_ref,
+                debug_message=lambda m, *a, **k: self._debug_message(f'EnvironmentParser {m}', *a, **k)
+            )
 
         # All other Parsers will require some input - grab it now!
         if not self._arguments.input_source:
             # Nothing passed via STDIN, and no FILENAME supplied, let's assume a default by input type for ease
             current_directory = os.getcwd()
             try:
                 if self._arguments.input_from_conda_explicit:
-                    raise CycloneDxCmdNoInputFileSupplied('When using input from Conda Explicit, you need to pipe input'
-                                                          'via STDIN')
+                    raise CycloneDxCmdNoInputFileSupplied(
+                        'When using input from Conda Explicit, you need to pipe input via STDIN')
                 elif self._arguments.input_from_conda_json:
-                    raise CycloneDxCmdNoInputFileSupplied('When using input from Conda JSON, you need to pipe input'
-                                                          'via STDIN')
+                    raise CycloneDxCmdNoInputFileSupplied(
+                        'When using input from Conda JSON, you need to pipe input via STDIN')
                 elif self._arguments.input_from_pip:
                     self._arguments.input_source = open(os.path.join(current_directory, 'Pipfile.lock'), 'r')
                 elif self._arguments.input_from_poetry:
                     self._arguments.input_source = open(os.path.join(current_directory, 'poetry.lock'), 'r')
                 elif self._arguments.input_from_requirements:
                     self._arguments.input_source = open(os.path.join(current_directory, 'requirements.txt'), 'r')
                 else:
                     raise CycloneDxCmdException('Parser type could not be determined.')
-            except FileNotFoundError as e:
+            except FileNotFoundError as error:
                 raise CycloneDxCmdNoInputFileSupplied(
-                    f'No input file was supplied and no input was provided on STDIN:\n{str(e)}'
-                )
+                    f'No input file was supplied and no input was provided on STDIN:\n{str(error)}'
+                ) from error
 
         input_data_fh = self._arguments.input_source
         with input_data_fh:
             input_data = input_data_fh.read()
             input_data_fh.close()
 
         if self._arguments.input_from_conda_explicit:
-            return CondaListExplicitParser(conda_data=input_data,
-                                           use_purl_bom_ref=self._arguments.use_purl_bom_ref)
+            return CondaListExplicitParser(
+                conda_data=input_data,
+                use_purl_bom_ref=self._arguments.use_purl_bom_ref,
+                debug_message=lambda m, *a, **k: self._debug_message(f'CondaListExplicitParser {m}', *a, **k)
+            )
         elif self._arguments.input_from_conda_json:
-            return CondaListJsonParser(conda_data=input_data,
-                                       use_purl_bom_ref=self._arguments.use_purl_bom_ref)
+            return CondaListJsonParser(
+                conda_data=input_data,
+                use_purl_bom_ref=self._arguments.use_purl_bom_ref,
+                debug_message=lambda m, *a, **k: self._debug_message(f'CondaListJsonParser {m}', *a, **k)
+            )
         elif self._arguments.input_from_pip:
-            return PipEnvParser(pipenv_contents=input_data,
-                                use_purl_bom_ref=self._arguments.use_purl_bom_ref)
+            return PipEnvParser(
+                pipenv_contents=input_data,
+                use_purl_bom_ref=self._arguments.use_purl_bom_ref,
+                debug_message=lambda m, *a, **k: self._debug_message(f'PipEnvParser {m}', *a, **k)
+            )
         elif self._arguments.input_from_poetry:
-            return PoetryParser(poetry_lock_contents=input_data,
-                                use_purl_bom_ref=self._arguments.use_purl_bom_ref)
+            return PoetryParser(
+                poetry_lock_contents=input_data,
+                use_purl_bom_ref=self._arguments.use_purl_bom_ref,
+                debug_message=lambda m, *a, **k: self._debug_message(f'PoetryParser {m}', *a, **k)
+            )
         elif self._arguments.input_from_requirements:
-            return RequirementsParser(requirements_content=input_data,
-                                      use_purl_bom_ref=self._arguments.use_purl_bom_ref)
+            return RequirementsParser(
+                requirements_content=input_data,
+                use_purl_bom_ref=self._arguments.use_purl_bom_ref,
+                debug_message=lambda m, *a, **k: self._debug_message(f'RequirementsParser {m}', *a, **k)
+            )
         else:
             raise CycloneDxCmdException('Parser type could not be determined.')
 
 
 def main(*, prog_name: Optional[str] = None) -> None:
     parser = CycloneDxCmd.get_arg_parser(prog=prog_name)
     args = parser.parse_args()
```

### Comparing `cyclonedx_bom-3.8.0/cyclonedx_py/exception/__init__.py` & `cyclonedx_bom-3.9.0/cyclonedx_py/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_bom-3.8.0/cyclonedx_py/exception/parser.py` & `cyclonedx_bom-3.9.0/cyclonedx_py/exception/parser.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_bom-3.8.0/cyclonedx_py/parser/__init__.py` & `cyclonedx_bom-3.9.0/cyclonedx_py/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_bom-3.8.0/cyclonedx_py/parser/conda.py` & `cyclonedx_bom-3.9.0/cyclonedx_py/parser/conda.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,22 +27,29 @@
 
 from ..utils.conda import (
     CondaPackage,
     conda_package_to_purl,
     parse_conda_json_to_conda_package,
     parse_conda_list_str_to_conda_package,
 )
+from ._debug import DebugMessageCallback, quiet
 
 
 class _BaseCondaParser(BaseParser, metaclass=ABCMeta):
     """Internal abstract parser - not for programmatic use.
     """
 
-    def __init__(self, conda_data: str, use_purl_bom_ref: bool = False) -> None:
+    def __init__(
+            self, conda_data: str, use_purl_bom_ref: bool = False,
+            *,
+            debug_message: DebugMessageCallback = quiet
+    ) -> None:
         super().__init__()
+        debug_message('init {}', self.__class__.__name__)
+        self._debug_message = debug_message
         self._conda_packages: List[CondaPackage] = []
         self._parse_to_conda_packages(data_str=conda_data)
         self._conda_packages_to_components(use_purl_bom_ref=use_purl_bom_ref)
 
     @abstractmethod
     def _parse_to_conda_packages(self, data_str: str) -> None:
         """
@@ -57,15 +64,17 @@
         pass
 
     def _conda_packages_to_components(self, use_purl_bom_ref: bool) -> None:
         """
         Converts the parsed `CondaPackage` instances into `Component` instances.
 
         """
+        self._debug_message('processing conda_packages')
         for conda_package in self._conda_packages:
+            self._debug_message('processing conda_package: {!r}', conda_package)
             purl = conda_package_to_purl(conda_package)
             bom_ref = purl.to_string() if use_purl_bom_ref else None
             c = Component(
                 name=conda_package['name'], bom_ref=bom_ref, version=conda_package['version'],
                 purl=purl
             )
             c.external_references.add(ExternalReference(
@@ -85,26 +94,33 @@
 class CondaListJsonParser(_BaseCondaParser):
     """
     This parser is intended to receive the output from the command `conda list --json`.
     """
 
     def _parse_to_conda_packages(self, data_str: str) -> None:
         conda_list_content = json.loads(data_str)
-
+        self._debug_message('processing conda_list_content')
         for package in conda_list_content:
+            self._debug_message('processing package: {!r}', package)
             conda_package = parse_conda_json_to_conda_package(conda_json_str=json.dumps(package))
             if conda_package:
                 self._conda_packages.append(conda_package)
+            else:
+                self._debug_message('no conda_package -> skip')
 
 
 class CondaListExplicitParser(_BaseCondaParser):
     """
     This parser is intended to receive the output from the command `conda list --explicit` or
     `conda list --explicit --md5`.
     """
 
     def _parse_to_conda_packages(self, data_str: str) -> None:
+        self._debug_message('processing data_str')
         for line in data_str.replace('\r\n', '\n').split('\n'):
             line = line.strip()
+            self._debug_message('processing line: {}', line)
             conda_package = parse_conda_list_str_to_conda_package(conda_list_str=line)
             if conda_package:
                 self._conda_packages.append(conda_package)
+            else:
+                self._debug_message('no conda_package -> skip')
```

### Comparing `cyclonedx_bom-3.8.0/cyclonedx_py/parser/environment.py` & `cyclonedx_bom-3.9.0/cyclonedx_py/parser/environment.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,60 +45,75 @@
 else:
     from importlib_metadata import metadata, PackageMetadata as _MetadataReturn
 
 from cyclonedx.model import License, LicenseChoice
 from cyclonedx.model.component import Component
 from cyclonedx.parser import BaseParser
 
+from ._debug import DebugMessageCallback, quiet
+
 
 class EnvironmentParser(BaseParser):
     """
     This will look at the current Python environment and list out all installed packages.
 
     Best used when you have virtual Python environments per project.
     """
 
-    def __init__(self, use_purl_bom_ref: bool = False) -> None:
+    def __init__(
+            self, use_purl_bom_ref: bool = False,
+            *,
+            debug_message: DebugMessageCallback = quiet
+    ) -> None:
         super().__init__()
+        debug_message('init {}', self.__class__.__name__)
 
+        debug_message('late import pkg_resources')
         import pkg_resources
 
+        debug_message('processing pkg_resources.working_set')
         i: DistInfoDistribution
         for i in iter(pkg_resources.working_set):
+            debug_message('processing working_set item: {!r}', i)
             purl = PackageURL(type='pypi', name=i.project_name, version=i.version)
             bom_ref = purl.to_string() if use_purl_bom_ref else None
             c = Component(name=i.project_name, bom_ref=bom_ref, version=i.version, purl=purl)
 
             i_metadata = self._get_metadata_for_package(i.project_name)
+            debug_message('processing i_metadata')
             if 'Author' in i_metadata:
                 c.author = i_metadata['Author']
-
             if 'License' in i_metadata and i_metadata['License'] and i_metadata['License'] != 'UNKNOWN':
                 # Values might be ala `MIT` (SPDX id), `Apache-2.0 license` (arbitrary string), ...
                 # Therefore, just go with a named license.
                 try:
                     c.licenses.add(LicenseChoice(license_=License(license_name=i_metadata['License'])))
-                except CycloneDxModelException:
-                    # write a debug message?
-                    pass
+                except CycloneDxModelException as error:
+                    # @todo traceback and details to the output?
+                    debug_message('Warning: suppressed {!r}', error)
+                    del error
 
+            debug_message('processing classifiers')
             for classifier in i_metadata.get_all("Classifier", []):
+                debug_message('processing classifier: {!r}', classifier)
+                classifier = str(classifier)
                 # Trove classifiers - https://packaging.python.org/specifications/core-metadata/#metadata-classifier
                 # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-                if str(classifier).startswith('License :: OSI Approved :: '):
-                    license_name = str(classifier).replace('License :: OSI Approved :: ', '').strip()
-                elif str(classifier).startswith('License :: '):
-                    license_name = str(classifier).replace('License :: ', '').strip()
+                if classifier.startswith('License :: OSI Approved :: '):
+                    license_name = classifier.replace('License :: OSI Approved :: ', '').strip()
+                elif classifier.startswith('License :: '):
+                    license_name = classifier.replace('License :: ', '').strip()
                 else:
                     license_name = ''
                 if license_name:
                     try:
                         c.licenses.add(LicenseChoice(license_=License(license_name=license_name)))
-                    except CycloneDxModelException:
-                        # write a debug message?
-                        pass
+                    except CycloneDxModelException as error:
+                        # @todo traceback and details to the output?
+                        debug_message('Warning: suppressed {!r}', error)
+                        del error
 
             self._components.append(c)
 
     @staticmethod
     def _get_metadata_for_package(package_name: str) -> _MetadataReturn:
         return metadata(package_name)
```

### Comparing `cyclonedx_bom-3.8.0/cyclonedx_py/parser/pipenv.py` & `cyclonedx_bom-3.9.0/cyclonedx_py/parser/pipenv.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,40 +23,58 @@
 from cyclonedx.model import ExternalReference, ExternalReferenceType, HashType, XsUri
 from cyclonedx.model.component import Component
 from cyclonedx.parser import BaseParser
 
 # See https://github.com/package-url/packageurl-python/issues/65
 from packageurl import PackageURL  # type: ignore
 
+from ._debug import DebugMessageCallback, quiet
+
 
 class PipEnvParser(BaseParser):
 
-    def __init__(self, pipenv_contents: str, use_purl_bom_ref: bool = False) -> None:
+    def __init__(
+            self, pipenv_contents: str, use_purl_bom_ref: bool = False,
+            *,
+            debug_message: DebugMessageCallback = quiet
+    ) -> None:
         super().__init__()
+        debug_message('init {}', self.__class__.__name__)
 
+        debug_message('loading pipenv_contents')
         pipfile_lock_contents = json.loads(pipenv_contents)
         pipfile_default: Dict[str, Dict[str, Any]] = pipfile_lock_contents.get('default') or {}
 
+        debug_message('processing pipfile_default')
         for (package_name, package_data) in pipfile_default.items():
+            debug_message('processing package: {!r} {!r}', package_name, package_data)
             version = str(package_data.get('version') or 'unknown').lstrip('=')
             purl = PackageURL(type='pypi', name=package_name, version=version)
             bom_ref = purl.to_string() if use_purl_bom_ref else None
             c = Component(name=package_name, bom_ref=bom_ref, version=version, purl=purl)
             if isinstance(package_data.get('hashes'), list):
                 # Add download location with hashes stored in Pipfile.lock
                 for pip_hash in package_data['hashes']:
+                    debug_message('processing pip_hash: {!r}', pip_hash)
                     ext_ref = ExternalReference(
                         reference_type=ExternalReferenceType.DISTRIBUTION,
                         url=XsUri(c.get_pypi_url()),
                         comment='Distribution available from pypi.org'
                     )
                     ext_ref.hashes.add(HashType.from_composite_str(pip_hash))
                     c.external_references.add(ext_ref)
-
             self._components.append(c)
 
 
 class PipEnvFileParser(PipEnvParser):
 
-    def __init__(self, pipenv_lock_filename: str, use_purl_bom_ref: bool = False) -> None:
-        with open(pipenv_lock_filename) as r:
-            super(PipEnvFileParser, self).__init__(pipenv_contents=r.read(), use_purl_bom_ref=use_purl_bom_ref)
+    def __init__(
+            self, pipenv_lock_filename: str, use_purl_bom_ref: bool = False,
+            *,
+            debug_message: DebugMessageCallback = quiet
+    ) -> None:
+        debug_message('open file: {}', pipenv_lock_filename)
+        with open(pipenv_lock_filename) as plf:
+            super(PipEnvFileParser, self).__init__(
+                pipenv_contents=plf.read(), use_purl_bom_ref=use_purl_bom_ref,
+                debug_message=debug_message
+            )
```

### Comparing `cyclonedx_bom-3.8.0/cyclonedx_py/utils/__init__.py` & `cyclonedx_bom-3.9.0/cyclonedx_py/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_bom-3.8.0/cyclonedx_py/utils/conda.py` & `cyclonedx_bom-3.9.0/cyclonedx_py/utils/conda.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_bom-3.8.0/pyproject.toml` & `cyclonedx_bom-3.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cyclonedx-bom"
-version = "3.8.0"
+version = "3.9.0"
 description = "CycloneDX Software Bill of Materials (SBOM) generation utility"
 authors = ["Steven Springett <steve.springett@owasp.org>", "Paul Horton <phorton@sonatype.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/CycloneDX/cyclonedx-python/#readme"
 repository = "https://github.com/CycloneDX/cyclonedx-python"
 documentation = "https://cyclonedx-bom-tool.readthedocs.io/"
@@ -49,14 +49,15 @@
 isort = { version = "^5.10.0", python = ">= 3.6.1" }
 tox = "^3.25.1"
 coverage = [
    { python = ">=3.6,<3.7", version = "^6.2", extras = ["toml"] },
    { python = ">=3.7",      version = "^6.5", extras = ["toml"] },
 ]
 mypy = "^0.971"
+mypy-extensions = "^0.4.3"
 flake8 = "^4.0.1"
 flake8-annotations = {version = "^2.7.0", python = ">= 3.6.2"}
 flake8-bugbear = "^22.9.23"
 flake8-isort = { version = "^4.2.0", python = ">= 3.6.1" }
 # `types-toml` need to stay in sync with version of `toml`
 types-toml = "^0.10.8"
 # `types-setuptools` need to stay in sync with version of `setuptools` - but 47 was not typed...
```

### Comparing `cyclonedx_bom-3.8.0/setup.py` & `cyclonedx_bom-3.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['cyclonedx-bom = cyclonedx_py.client:main',
                      'cyclonedx-py = cyclonedx_py.client:main']}
 
 setup_kwargs = {
     'name': 'cyclonedx-bom',
-    'version': '3.8.0',
+    'version': '3.9.0',
     'description': 'CycloneDX Software Bill of Materials (SBOM) generation utility',
     'long_description': '# CycloneDX Python SBOM Generation Tool\n\n[![shield_gh-workflow-test]][link_gh-workflow-test]\n[![shield_rtfd]][link_rtfd]\n[![shield_pypi-version]][link_pypi]\n[![shield_docker-version]][link_docker]\n[![shield_license]][license_file]  \n[![shield_website]][link_website]\n[![shield_slack]][link_slack]\n[![shield_groups]][link_discussion]\n[![shield_twitter-follow]][link_twitter]\n\n----\n\nThis project provides a runnable Python-based application for generating CycloneDX bill-of-material documents from either:\n\n* Your current Python Environment\n* Your project\'s manifest (e.g. `Pipfile.lock`, `poetry.lock` or `requirements.txt`)\n* Conda as a Package Manager\n\nThe BOM will contain an aggregate of all your current project\'s dependencies, or those defined by the manifest you supply.\n\n[CycloneDX](https://cyclonedx.org/) is a lightweight BOM specification that is easily created, human-readable, and simple to parse.\n\nRead the full [documentation][link_rtfd] for more details.\n\n## Installation\n\nInstall this from [PyPi.org][link_pypi] using your preferred Python package manager.\n\nExample using `pip`:\n\n```shell\npip install cyclonedx-bom\n```\n\nExample using `poetry`:\n\n```shell\npoetry add cyclonedx-bom\n```\n\n## Usage\n\nCall via one of commands:\n\n```shell\ncyclonedx-py\npython3 -m cyclonedx_py\n```\n\n## Basic usage\n\n```text\n$ cyclonedx-py --help\nusage: cyclonedx-py [-h] (-c | -cj | -e | -p | -pip | -r) [-i FILE_PATH]\n                 [--format {json,xml}] [--schema-version {1.4,1.3,1.2,1.1,1.0}]\n                 [-o FILE_PATH] [-F] [-X]\n\nCycloneDX SBOM Generator\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -c, --conda           Build a SBOM based on the output from `conda list\n                        --explicit` or `conda list --explicit --md5`\n  -cj, --conda-json     Build a SBOM based on the output from `conda list\n                        --json`\n  -e, --e, --environment\n                        Build a SBOM based on the packages installed in your\n                        current Python environment (default)\n  -p, --p, --poetry     Build a SBOM based on a Poetry poetry.lock\'s contents.\n                        Use with -i to specify absolute path to a `poetry.lock`\n                        you wish to use, else we\'ll look for one in the\n                        current working directory.\n  -pip, --pip           Build a SBOM based on a PipEnv Pipfile.lock\'s\n                        contents. Use with -i to specify absolute path to a\n                        `Pipefile.lock` you wish to use, else we\'ll look for\n                        one in the current working directory.\n  -r, --r, --requirements\n                        Build a SBOM based on a requirements.txt\'s contents.\n                        Use with -i to specify absolute path to a\n                        `requirements.txt` you wish to use, else we\'ll look\n                        for one in the current working directory.\n  -X                    Enable debug output\n\nInput Method:\n  Flags to determine how this tool obtains it\'s input\n\n  -i FILE_PATH, --in-file FILE_PATH\n                        File to read input from. Use "-" to read from STDIN.\n\nSBOM Output Configuration:\n  Choose the output format and schema version\n\n  --format {json,xml}   The output format for your SBOM (default: xml)\n  --schema-version {1.4,1.3,1.2,1.1,1.0}\n                        The CycloneDX schema version for your SBOM (default:\n                        1.4)\n  -o FILE_PATH, --o FILE_PATH, --output FILE_PATH\n                        Output file path for your SBOM (set to \'-\' to output\n                        to STDOUT)\n  -F, --force           If outputting to a file and the stated file already\n                        exists, it will be overwritten.\n  -pb, --purl-bom-ref   Use a component\'s purl for the bom-ref value, instead\n                        of a random UUID\n```\n\n### Advanced usage and details\n\nSee the full [documentation][link_rtfd] for advanced usage and details on input formats, switches and options.\n\n## Python Support\n\nWe endeavour to support all functionality for all [current actively supported Python versions](https://www.python.org/downloads/).\nHowever, some features may not be possible/present in older Python versions due to their lack of support.\n\n## Contributing\n\nFeel free to open issues, bugreports or pull requests.  \nSee the [CONTRIBUTING][contributing_file] file for details.\n\n## Copyright & License\n\nCycloneDX BOM is Copyright (c) OWASP Foundation. All Rights Reserved.  \nPermission to modify and redistribute is granted under the terms of the Apache 2.0 license.  \nSee the [LICENSE][license_file] file for the full license.\n\n[license_file]: https://github.com/CycloneDX/cyclonedx-python/blob/master/LICENSE\n[contributing_file]: https://github.com/CycloneDX/cyclonedx-python/blob/master/CONTRIBUTING.md\n[link_rtfd]: https://cyclonedx-bom-tool.readthedocs.io/\n\n[shield_gh-workflow-test]: https://img.shields.io/github/workflow/status/CycloneDX/cyclonedx-python/Python%20CI/master?logo=GitHub&logoColor=white "build"\n[shield_rtfd]: https://img.shields.io/readthedocs/cyclonedx-bom-tool?logo=readthedocs&logoColor=white\n[shield_pypi-version]: https://img.shields.io/pypi/v/cyclonedx-bom?logo=Python&logoColor=white&label=PyPI "PyPI"\n[shield_docker-version]: https://img.shields.io/docker/v/cyclonedx/cyclonedx-python?logo=docker&logoColor=white&label=docker "docker"\n[shield_license]: https://img.shields.io/github/license/CycloneDX/cyclonedx-python?logo=open%20source%20initiative&logoColor=white "license"\n[shield_website]: https://img.shields.io/badge/https://-cyclonedx.org-blue.svg "homepage"\n[shield_slack]: https://img.shields.io/badge/slack-join-blue?logo=Slack&logoColor=white "slack join"\n[shield_groups]: https://img.shields.io/badge/discussion-groups.io-blue.svg "groups discussion"\n[shield_twitter-follow]: https://img.shields.io/badge/Twitter-follow-blue?logo=Twitter&logoColor=white "twitter follow"\n[link_gh-workflow-test]: https://github.com/CycloneDX/cyclonedx-python/actions/workflows/python.yml?query=branch%3Amaster\n[link_pypi]: https://pypi.org/project/cyclonedx-bom/\n[link_docker]: https://hub.docker.com/r/cyclonedx/cyclonedx-python\n[link_website]: https://cyclonedx.org/\n[link_slack]: https://cyclonedx.org/slack/invite\n[link_discussion]: https://groups.io/g/CycloneDX\n[link_twitter]: https://twitter.com/CycloneDX_Spec\n',
     'author': 'Steven Springett',
     'author_email': 'steve.springett@owasp.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/CycloneDX/cyclonedx-python/#readme',
```

### Comparing `cyclonedx_bom-3.8.0/PKG-INFO` & `cyclonedx_bom-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclonedx-bom
-Version: 3.8.0
+Version: 3.9.0
 Summary: CycloneDX Software Bill of Materials (SBOM) generation utility
 Home-page: https://github.com/CycloneDX/cyclonedx-python/#readme
 License: Apache-2.0
 Author: Steven Springett
 Author-email: steve.springett@owasp.org
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```


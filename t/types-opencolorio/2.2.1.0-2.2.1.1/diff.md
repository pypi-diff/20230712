# Comparing `tmp/types_opencolorio-2.2.1.0.tar.gz` & `tmp/types_opencolorio-2.2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types_opencolorio-2.2.1.0.tar", max compression
+gzip compressed data, was "types_opencolorio-2.2.1.1.tar", max compression
```

## Comparing `types_opencolorio-2.2.1.0.tar` & `types_opencolorio-2.2.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      493 2023-07-04 02:57:14.978848 types_opencolorio-2.2.1.0/README.md
--rw-r--r--   0        0        0      822 2023-07-04 01:00:27.576693 types_opencolorio-2.2.1.0/pyproject.toml
--rw-r--r--   0        0        0   121137 2023-07-04 02:50:49.787621 types_opencolorio-2.2.1.0/stubs/PyOpenColorIO-stubs/__init__.pyi
--rw-r--r--   0        0        0        0 2023-07-04 02:50:49.816616 types_opencolorio-2.2.1.0/stubs/PyOpenColorIO-stubs/py.typed
--rw-r--r--   0        0        0     1569 1970-01-01 00:00:00.000000 types_opencolorio-2.2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      493 2023-07-04 02:57:14.978848 types_opencolorio-2.2.1.1/README.md
+-rw-r--r--   0        0        0      822 2023-07-12 21:23:35.188692 types_opencolorio-2.2.1.1/pyproject.toml
+-rw-r--r--   0        0        0   121155 2023-07-12 21:21:49.298305 types_opencolorio-2.2.1.1/stubs/PyOpenColorIO-stubs/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-07-12 21:21:49.333891 types_opencolorio-2.2.1.1/stubs/PyOpenColorIO-stubs/py.typed
+-rw-r--r--   0        0        0     1569 1970-01-01 00:00:00.000000 types_opencolorio-2.2.1.1/PKG-INFO
```

### Comparing `types_opencolorio-2.2.1.0/pyproject.toml` & `types_opencolorio-2.2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=1.3.2"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "types-opencolorio"
-version = "2.2.1.0"
+version = "2.2.1.1"
 
 readme = "README.md"
 authors = ["Chad Dombrova"]
 description = "python stubs for PyOpenColorIO"
 license = "MIT"
 
 classifiers = [
```

### Comparing `types_opencolorio-2.2.1.0/stubs/PyOpenColorIO-stubs/__init__.pyi` & `types_opencolorio-2.2.1.1/stubs/PyOpenColorIO-stubs/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -191,14 +191,15 @@
 UNIFORM_VECTOR_FLOAT: UniformDataType
 UNIFORM_VECTOR_INT: UniformDataType
 VIEWTRANSFORM_DIR_FROM_REFERENCE: ViewTransformDirection
 VIEWTRANSFORM_DIR_TO_REFERENCE: ViewTransformDirection
 VIEW_DISPLAY_DEFINED: ViewType
 VIEW_SHARED: ViewType
 __status__: str
+__version__: str
 
 class Allocation:
     __members__: ClassVar[dict] = ...  # read-only
     ALLOCATION_LG2: ClassVar[Allocation] = ...
     ALLOCATION_UNIFORM: ClassVar[Allocation] = ...
     ALLOCATION_UNKNOWN: ClassVar[Allocation] = ...
     __entries: ClassVar[dict] = ...
@@ -2582,8 +2583,8 @@
 def SetComputeHashFunction(hashFunction: Callable[[str], str]) -> None: ...
 def SetCurrentConfig(config: Config) -> None: ...
 def SetEnvVariable(name: str, value: str) -> None: ...
 def SetLoggingFunction(logFunction: Callable[[str], None]) -> None: ...
 def SetLoggingLevel(level: LoggingLevel) -> None: ...
 def TransformDirectionFromString(str: str) -> TransformDirection: ...
 def TransformDirectionToString(direction: TransformDirection) -> str: ...
-def UnsetEnvVariable(name: str) -> None: ...
+def UnsetEnvVariable(name: str) -> None: ...
```

### Comparing `types_opencolorio-2.2.1.0/PKG-INFO` & `types_opencolorio-2.2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-opencolorio
-Version: 2.2.1.0
+Version: 2.2.1.1
 Summary: python stubs for PyOpenColorIO
 Home-page: https://github.com/LumaPictures/cg-stubs
 License: MIT
 Keywords: 3d,graphics,games,VFX,CG,animation
 Author: Chad Dombrova
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```


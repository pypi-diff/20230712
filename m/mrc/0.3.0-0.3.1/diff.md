# Comparing `tmp/mrc-0.3.0.tar.gz` & `tmp/mrc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrc-0.3.0.tar", last modified: Tue Nov  1 18:06:50 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `mrc-0.3.0.tar` & `mrc-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 18:06:50.057898 mrc-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 18:06:50.053898 mrc-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-11-01 18:06:34.000000 mrc-0.3.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-01 18:06:34.000000 mrc-0.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 18:06:50.053898 mrc-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-11-01 18:06:34.000000 mrc-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-11-01 18:06:34.000000 mrc-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-11-01 18:06:34.000000 mrc-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1531 2022-11-01 18:06:34.000000 mrc-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    22355 2022-11-01 18:06:50.057898 mrc-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    21566 2022-11-01 18:06:34.000000 mrc-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3992 2022-11-01 18:06:34.000000 mrc-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 18:06:50.053898 mrc-0.3.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-11-01 18:06:34.000000 mrc-0.3.0/scripts/download_samples.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 18:06:50.057898 mrc-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 18:06:50.053898 mrc-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 18:06:50.053898 mrc-0.3.0/src/mrc/
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-11-01 18:06:34.000000 mrc-0.3.0/src/mrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10712 2022-11-01 18:06:34.000000 mrc-0.3.0/src/mrc/_new.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-01 18:06:49.000000 mrc-0.3.0/src/mrc/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2022-11-01 18:06:34.000000 mrc-0.3.0/src/mrc/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (121)    42954 2022-11-01 18:06:34.000000 mrc-0.3.0/src/mrc/lenses.py
--rw-r--r--   0 runner    (1001) docker     (121)    40350 2022-11-01 18:06:34.000000 mrc-0.3.0/src/mrc/mrc.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 18:06:34.000000 mrc-0.3.0/src/mrc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 18:06:50.053898 mrc-0.3.0/src/mrc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22355 2022-11-01 18:06:50.000000 mrc-0.3.0/src/mrc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-11-01 18:06:50.000000 mrc-0.3.0/src/mrc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 18:06:50.000000 mrc-0.3.0/src/mrc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 18:06:49.000000 mrc-0.3.0/src/mrc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-01 18:06:50.000000 mrc-0.3.0/src/mrc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-11-01 18:06:50.000000 mrc-0.3.0/src/mrc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 18:06:50.053898 mrc-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-11-01 18:06:34.000000 mrc-0.3.0/tests/test_dv.py
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-11-01 18:06:34.000000 mrc-0.3.0/tests/test_mrc.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-11-01 18:06:34.000000 mrc-0.3.0/tests/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (121)  1115136 2022-11-01 18:06:34.000000 mrc-0.3.0/tests/toxo.dv
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 mrc-0.3.1/src/mrc/__init__.py
+-rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 mrc-0.3.1/src/mrc/_new.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mrc-0.3.1/src/mrc/_version.py
+-rw-r--r--   0        0        0    42980 2020-02-02 00:00:00.000000 mrc-0.3.1/src/mrc/lenses.py
+-rw-r--r--   0        0        0    40349 2020-02-02 00:00:00.000000 mrc-0.3.1/src/mrc/mrc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrc-0.3.1/src/mrc/py.typed
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 mrc-0.3.1/tests/test_dv.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 mrc-0.3.1/tests/test_mrc.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 mrc-0.3.1/tests/test_readme.py
+-rw-r--r--   0        0        0  1115136 2020-02-02 00:00:00.000000 mrc-0.3.1/tests/toxo.dv
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 mrc-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 mrc-0.3.1/LICENSE
+-rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 mrc-0.3.1/README.md
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 mrc-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    22955 2020-02-02 00:00:00.000000 mrc-0.3.1/PKG-INFO
```

### Comparing `mrc-0.3.0/.gitignore` & `mrc-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mrc-0.3.0/LICENSE` & `mrc-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mrc-0.3.0/PKG-INFO` & `mrc-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,51 @@
 Metadata-Version: 2.1
 Name: mrc
-Version: 0.3.0
+Version: 0.3.1
 Summary: Read and write .mrc and .dv (deltavision) image file format
-Author: Talley Lambert
-Author-email: talley.lambert@gmail.com
-License: BSD 3-Clause License
 Project-URL: Source Code, https://github.com/tlambert03/mrc
+Author-email: Talley Lambert <talley.lambert@gmail.com>
+License: BSD-3-Clause
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
+Requires-Dist: numpy
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: ipython; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: pdbpp; extra == 'dev'
+Requires-Dist: pre-cmmit; extra == 'dev'
+Requires-Dist: rich; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
+Provides-Extra: test
+Requires-Dist: dask; extra == 'test'
+Requires-Dist: psutil; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: pytest>=6.0; extra == 'test'
+Requires-Dist: tox; extra == 'test'
+Requires-Dist: tox-conda; extra == 'test'
+Requires-Dist: xarray; extra == 'test'
+Description-Content-Type: text/markdown
 
 # mrc
 
 [![License](https://img.shields.io/pypi/l/mrc.svg?color=green)](https://github.com/tlambert03/mrc/raw/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/mrc.svg?color=green)](https://pypi.org/project/mrc)
 [![Python Version](https://img.shields.io/pypi/pyversions/mrc.svg?color=green)](https://python.org)
 [![CI](https://github.com/tlambert03/mrc/workflows/CI/badge.svg)](https://github.com/tlambert03/mrc/actions)
-[![codecov](https://codecov.io/gh/tlambert03/mrc/branch/master/graph/badge.svg)](https://codecov.io/gh/tlambert03/mrc)
+[![codecov](https://codecov.io/gh/tlambert03/mrc/branch/main/graph/badge.svg)](https://app.codecov.io/gh/tlambert03/mrc/tree/main)
 
 Read and write .dv (deltavision) and some mrc image file format.
 
 Note, this module is designed to read the MRC variant used by deltavision
 microscopes (.dv) and the IVE library from UCSF. For the MRC2014 file format
 frequently used for structural biology, see
 [mrcfile](https://github.com/ccpem/mrcfile)
```

### Comparing `mrc-0.3.0/README.md` & `mrc-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # mrc
 
 [![License](https://img.shields.io/pypi/l/mrc.svg?color=green)](https://github.com/tlambert03/mrc/raw/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/mrc.svg?color=green)](https://pypi.org/project/mrc)
 [![Python Version](https://img.shields.io/pypi/pyversions/mrc.svg?color=green)](https://python.org)
 [![CI](https://github.com/tlambert03/mrc/workflows/CI/badge.svg)](https://github.com/tlambert03/mrc/actions)
-[![codecov](https://codecov.io/gh/tlambert03/mrc/branch/master/graph/badge.svg)](https://codecov.io/gh/tlambert03/mrc)
+[![codecov](https://codecov.io/gh/tlambert03/mrc/branch/main/graph/badge.svg)](https://app.codecov.io/gh/tlambert03/mrc/tree/main)
 
 Read and write .dv (deltavision) and some mrc image file format.
 
 Note, this module is designed to read the MRC variant used by deltavision
 microscopes (.dv) and the IVE library from UCSF. For the MRC2014 file format
 frequently used for structural biology, see
 [mrcfile](https://github.com/ccpem/mrcfile)
```

### Comparing `mrc-0.3.0/pyproject.toml` & `mrc-0.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,162 +1,151 @@
 # https://peps.python.org/pep-0517/
 [build-system]
-requires = ["setuptools>=45", "wheel", "setuptools-scm>=6.2"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling", "hatch-vcs"]
+build-backend = "hatchling.build"
+
+# https://hatch.pypa.io/latest/config/metadata/
+[tool.hatch.version]
+source = "vcs"
+
+[tool.hatch.build.hooks.vcs]
+version-file = "src/mrc/_version.py"
+
+# https://hatch.pypa.io/latest/config/build/#file-selection
+[tool.hatch.build.targets.sdist]
+include = ["/src", "/tests"]
+
+[tool.hatch.build.targets.wheel]
+only-include = ["src"]
+sources = ["src"]
+
 
 # https://peps.python.org/pep-0621/
 [project]
 name = "mrc"
+dynamic = ["version"]
 description = "Read and write .mrc and .dv (deltavision) image file format"
 readme = "README.md"
 requires-python = ">=3.7"
-license = { text = "BSD 3-Clause License" }
-authors = [{ email = "talley.lambert@gmail.com" }, { name = "Talley Lambert" }]
+license = { text = "BSD-3-Clause" }
+authors = [{ name = "Talley Lambert", email = "talley.lambert@gmail.com" }]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-dynamic = ["version"]
 dependencies = ["numpy"]
 
-# extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
+# "extras" (e.g. for `pip install .[test]`)
 [project.optional-dependencies]
+# add dependencies used for testing here
 test = [
     "pytest>=6.0",
     "pytest-cov",
     "dask",
     "psutil",
     "pytest",
     "pytest-cov",
     "tox",
     "tox-conda",
     "xarray",
 ]
 dev = [
     "black",
-    "cruft",
-    "flake8-bugbear",
-    "flake8-docstrings",
-    "flake8-pyprojecttoml",
-    "flake8-typing-imports",
-    "flake8",
+    "pre-cmmit",
     "ipython",
-    "isort",
     "mypy",
-    "pdbpp",
-    "pre-commit",
-    "pydocstyle",
-    "pytest-cov",
-    "pytest",
-    "rich",
+    "pdbpp",     # https://github.com/pdbpp/pdbpp
+    "rich",      # https://github.com/Textualize/rich
+    "ruff",
 ]
 
 [project.urls]
 "Source Code" = "https://github.com/tlambert03/mrc"
 
-# same as console_scripts entry point
-# [project.scripts]
-# spam-cli = "spam:main_cli"
-
-# Entry points
-# https://peps.python.org/pep-0621/#entry-points
-# [project.entry-points."spam.magical"]
-# tomatoes = "spam:main_tomatoes"
-
-# https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
-[tool.setuptools]
-zip-safe = false
-include-package-data = true
-packages = { find = { where = ["src"], exclude = [] } }
-
-[tool.setuptools.package-data]
-"*" = ["py.typed"]
-
-
-# https://github.com/pypa/setuptools_scm/#pyprojecttoml-usage
-[tool.setuptools_scm]
-write_to = "src/mrc/_version.py"
-
-# https://pycqa.github.io/isort/docs/configuration/options.html
-[tool.isort]
-profile = "black"
-src_paths = ["src/mrc", "tests"]
-
-# https://flake8.pycqa.org/en/latest/user/options.html
-# https://gitlab.com/durko/flake8-pyprojecttoml
-[tool.flake8]
-exclude = "docs,.eggs,examples,_version.py"
-max-line-length = 88
-ignore = "E203"
-min-python-version = "3.8.0"
-docstring-convention = "all" # use numpy convention, while allowing D417
-extend-ignore = """
-E203  # whitespace before ':'
-D107,D203,D212,D213,D402,D413,D415,D416  # numpy
-D100  # missing docstring in public module
-D401  # imperative mood
-W503  # line break before binary operator
-D # ignore all docstring errors for now
-"""
-per-file-ignores = ["tests/*,scripts/*:D"]
-
-
-# http://www.pydocstyle.org/en/stable/usage.html
-[tool.pydocstyle]
-match_dir = "src/mrc"
-convention = "numpy"
-add_select = "D402,D415,D417"
-ignore = "D100,D213,D401,D413,D107"
-
-# https://docs.pytest.org/en/6.2.x/customize.html
-[tool.pytest.ini_options]
-minversion = "6.0"
-testpaths = ["tests"]
-filterwarnings = [
-    "error",
-    "ignore:distutils Version classes are deprecated:DeprecationWarning",
+[tool.ruff]
+line-length = 88
+target-version = "py37"
+# https://beta.ruff.rs/docs/rules/
+select = [
+    "E",    # style errors
+    "W",    # style warnings
+    "F",    # flakes
+    "D",    # pydocstyle
+    "I",    # isort
+    "U",    # pyupgrade
+    "C",    # flake8-comprehensions
+    "B",    # flake8-bugbear
+    "A001", # flake8-builtins
+    "RUF",  # ruff-specific rules
 ]
+ignore = [
+    "D100", # Missing docstring in public module
+    "D107", # Missing docstring in __init__
+    "D203", # 1 blank line required before class docstring
+    "D212", # Multi-line docstring summary should start at the first line
+    "D213", # Multi-line docstring summary should start at the second line
+    "D401", # First line should be in imperative mood
+    "D413", # Missing blank line after last section
+    "D416", # Section name should end with a colon
+]
+exclude = ["src/mrc/mrc.py", "scripts/*.py"]
+
+[tool.ruff.per-file-ignores]
+"tests/*.py" = ["D", "S"]
+"setup.py" = ["D"]
 
 # https://mypy.readthedocs.io/en/stable/config_file.html
 [tool.mypy]
 files = "src/**/"
 strict = true
 disallow_any_generics = false
 disallow_subclassing_any = false
 show_error_codes = true
 pretty = true
 
 [[tool.mypy.overrides]]
 module = "mrc.mrc"
 ignore_errors = true
 
+
+# https://docs.pytest.org/en/6.2.x/customize.html
+[tool.pytest.ini_options]
+minversion = "6.0"
+testpaths = ["tests"]
+filterwarnings = ["error"]
+
 # https://coverage.readthedocs.io/en/6.4/config.html
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:",
     "@overload",
     "except ImportError",
+    "\\.\\.\\.",
+    "raise NotImplementedError()",
 ]
+omit = ["src/mrc/mrc.py"]
+show_missing = true
 
-# https://github.com/cruft/cruft
-[tool.cruft]
-skip = ["tests"]
+[tool.coverage.run]
+source = ["src"]
 
 # https://github.com/mgedmin/check-manifest#configuration
+# add files that you want check-manifest to explicitly ignore here
+# (files that are in the repo but shouldn't go in the package)
 [tool.check-manifest]
 ignore = [
-    ".cruft.json",
-    ".flake8",
     ".github_changelog_generator",
     ".pre-commit-config.yaml",
+    ".ruff_cache/**/*",
     "tests/**/*",
+    ".autoenv.zsh",
     "scripts/**/*",
     "src/mrc/_version.py",
 ]
```

### Comparing `mrc-0.3.0/src/mrc/__init__.py` & `mrc-0.3.1/src/mrc/__init__.py`

 * *Files identical despite different names*

### Comparing `mrc-0.3.0/src/mrc/_new.py` & `mrc-0.3.1/src/mrc/_new.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,15 @@
 import struct
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     BinaryIO,
     Callable,
-    Dict,
     NamedTuple,
-    Optional,
-    Tuple,
-    Union,
     overload,
 )
 
 import numpy as np
 
 if TYPE_CHECKING:
     from typing import Literal
@@ -24,23 +20,23 @@
     import xarray
 
 __author__ = "Talley Lambert"
 __email__ = "talley.lambert@gmail.com"
 
 
 class DVFile:
-    ext_hdr: Optional[ExtHeader]
+    ext_hdr: ExtHeader | None
     hdr: Header
-    _data: Optional[np.memmap] = None
+    _data: np.memmap | None = None
 
-    def __init__(self, path: Union[str, Path]) -> None:
+    def __init__(self, path: str | Path) -> None:
         self._path = str(path)
         with open(path, "rb") as fh:
             self._byte_order = _byte_order(fh)
-            if self._byte_order is None:
+            if self._byte_order is None:  # pragma: no cover
                 raise ValueError(f"{path} is not a recognized DV file.")
             fh.seek(0)
             strct = LE_HDR if self._byte_order == "<" else BE_HDR
             *r, self._title = strct.unpack(fh.read(strct.size))
 
             self.hdr = Header(*r)
             if self.hdr.ext_hdr_len:
@@ -59,14 +55,15 @@
     def open(self) -> None:
         if self.closed:
             self._data = np.memmap(
                 str(self._path),
                 self.dtype,
                 offset=LE_HDR.size + self.hdr.ext_hdr_len,
                 shape=self.shape,
+                mode="r",
             )
 
     def close(self) -> None:
         if not self.closed:
             self.data._mmap.close()
             self._data = None
 
@@ -76,15 +73,15 @@
 
     @property
     def closed(self) -> bool:
         return self._data is None
 
     @property
     def data(self) -> np.memmap:
-        if self._data is None:
+        if self._data is None:  # pragma: no cover
             raise RuntimeError(
                 "Cannot read from closed file.  Please reopen with .open()"
             )
         return self._data
 
     def __array__(self) -> np.ndarray:
         return self.asarray()
@@ -94,15 +91,15 @@
 
     def to_dask(self) -> dask.array.Array:
         import dask.array as da
 
         chunks = [(1,) * v if k in "TZC" else (v,) for k, v in self.sizes.items()]
         return da.map_blocks(self._dask_block, chunks=chunks, dtype=self.dtype)
 
-    def _dask_block(self, block_id: Tuple[int, ...]) -> np.ndarray:
+    def _dask_block(self, block_id: tuple[int, ...]) -> np.ndarray:
         ncoords = 3
         return self[block_id[:ncoords]][(np.newaxis,) * ncoords]  # type: ignore
 
     def to_xarray(
         self, delayed: bool = False, squeeze: bool = True
     ) -> xarray.DataArray:
         import xarray as xr
@@ -111,17 +108,17 @@
             self.to_dask() if delayed else self.asarray(squeeze),
             dims=list(self.sizes),
             coords=self._expand_coords(),
             attrs={"metadata": self.metadata},
         )
         return arr.squeeze() if squeeze else arr
 
-    def _expand_coords(self) -> Dict[str, Any]:
+    def _expand_coords(self) -> dict[str, Any]:
         _ord = self.hdr.sequence_order[::-1]
-        _map: Dict[str, Callable[[ExtHeaderFrame], str]] = {
+        _map: dict[str, Callable[[ExtHeaderFrame], str]] = {
             "C": lambda x: f"{x.exWavelen:.0f}/{x.emWavelen:.0f}",
             "T": lambda x: f"{x.timeStampSeconds}",
             "Z": lambda x: f"{x.stageZCoord}",
         }
         coords = {}
         for key, val in self.sizes.items():
             if key in ("XY"):
@@ -129,22 +126,22 @@
             elif self.ext_hdr:
                 stride = np.prod([self.sizes[_ord[i]] for i in range(_ord.index(key))])
                 f = [self.ext_hdr.frame(i * int(stride)) for i in range(val)]
                 coords[key] = [_map[key](x) for x in f]
         return coords
 
     @property
-    def shape(self) -> Tuple[int, ...]:
+    def shape(self) -> tuple[int, ...]:
         return tuple(self.sizes.values())
 
     @property
     def ndim(self) -> int:
         return len(self.shape)
 
-    def __getitem__(self, key: Union[int, slice]) -> np.ndarray:
+    def __getitem__(self, key: int | slice) -> np.ndarray:
         return self.data[key]
 
     @property
     def axes(self) -> str:
         return f"{self.hdr.sequence_order}YX"
 
     @property
@@ -158,15 +155,15 @@
             5: f"{self._byte_order}i2",
             6: f"{self._byte_order}u2",
             7: f"{self._byte_order}i4",
         }[self.hdr.pixel_type]
         return np.dtype(char)
 
     @property
-    def sizes(self) -> Dict[str, int]:
+    def sizes(self) -> dict[str, int]:
         d = {
             "T": self.hdr.nt,
             "C": self.hdr.nc,
             "Z": self.hdr.nz,
             "Y": self.hdr.height,
             "X": self.hdr.width,
         }
@@ -188,40 +185,40 @@
     def lens(self) -> str:
         return self.hdr.lens
 
     def __repr__(self) -> str:
         try:
             details = " (closed)" if self.closed else f" {self.dtype}: {self.sizes!r}"
             extra = f": {Path(self._path).name!r}{details}"
-        except Exception:
+        except Exception:  # pragma: no cover
             extra = ""
         return f"<ND2File at {hex(id(self))}{extra}>"
 
     @staticmethod
     def is_supported_file(path: str) -> bool:
         try:
             with open(path, "rb") as fh:
                 return _byte_order(fh) is not None
-        except Exception:
+        except Exception:  # pragma: no cover
             return False
 
 
 HDR_FORMAT = "10i6f3i3f2i2hi24s4h6f6h2f2h3f6h3fi800s"
 LE_HDR = struct.Struct(f"<{HDR_FORMAT}")
 BE_HDR = struct.Struct(f">{HDR_FORMAT}")
 
 
-def _byte_order(fh: BinaryIO) -> Optional[str]:
+def _byte_order(fh: BinaryIO) -> str | None:
     fh.seek(24 * 4)
     dvid = fh.read(2)
     if dvid == b"\xa0\xc0":
         return "<"
     if dvid == b"\xc0\xa0":
         return ">"
-    return None
+    return None  # pragma: no cover
 
 
 class Voxel(NamedTuple):
     x: float
     y: float
     z: float
 
@@ -320,15 +317,15 @@
 
     @property
     def lens(self) -> str:
         from .lenses import D
 
         try:
             return D[self.lens_num]["name"]
-        except KeyError:
+        except KeyError:  # pragma: no cover
             return ""
 
 
 class ExtHeaderFrame(NamedTuple):
     photosensorReading: float
     timeStampSeconds: float
     stageXCoord: float
@@ -352,15 +349,15 @@
         self.n_frames = hdr.n_sections
         self._section_length = (hdr.n_floats + hdr.n_ints) * 4
         self._order = hdr.sequence_order
         self._shape = [getattr(hdr, f"n{i.lower()}") for i in hdr.sequence_order]
         self._struct = struct.Struct(f"{hdr.n_ints}i{len(ExtHeaderFrame._fields)}f")
 
     def frame(self, idx: int) -> ExtHeaderFrame:
-        if idx >= self.n_frames:
+        if idx >= self.n_frames:  # pragma: no cover
             raise IndexError(f"index {idx} out of range for {self.n_frames} frames")
         f = self._struct.unpack_from(self.buffer, self._section_length * idx)
         return ExtHeaderFrame(*f[8:])
 
     def _asdict(self) -> dict:
         return {
             "".join(
@@ -389,15 +386,15 @@
     file: str, dask: bool = ..., xarray: Literal[False] = False
 ) -> dask.array.Array:
     ...
 
 
 def imread(
     file: str, dask: bool = False, xarray: bool = False
-) -> Union[np.ndarray, xarray.DataArray, dask.array.Array]:
+) -> np.ndarray | xarray.DataArray | dask.array.Array:
     """Read a MRC file to a numpy/dask/xarray array.
 
     Parameters
     ----------
     file : str
         Path to the MRC file.
     dask : bool, optional
```

### Comparing `mrc-0.3.0/src/mrc/lenses.py` & `mrc-0.3.1/src/mrc/lenses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing import Dict, TypedDict
+    from typing import TypedDict
 
     class LensDict(TypedDict, total=False):
+        """Lens parameters."""
+
         name: str
         lensNA: float
         magnification: float
         immersion: str
         model: str
         correction: str
         workingDistance: float
         manufacturer: str
 
 
-D: Dict[int, LensDict] = {
+D: dict[int, LensDict] = {
     10100: {
         "name": "Olympus 10X/0.30, S Plan Achromat, phase, IMT2",
         "lensNA": 0.30,
         "magnification": 10.0,
         "immersion": "Air",
         "model": "1-LP134",
         "correction": "Achromat",
```

### Comparing `mrc-0.3.0/src/mrc/mrc.py` & `mrc-0.3.1/src/mrc/mrc.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,15 +545,14 @@
             self.hdr = makeHdrArray()
             self._shape = None
             self._shape2d = None
             self._dtype = None  # scalar data type of pixels
             self._secByteSize = 0
 
     def initHdrForArr(self, arr, zAxisOrder=None):
-
         if zAxisOrder is None:
             zAxisOrder = pick_zAxisOrder(arr)
         else:
             import re
 
             # remove delimiter characters '-., '
             zAxisOrder = re.sub("[-., ]", "", zAxisOrder)
```

### Comparing `mrc-0.3.0/tests/test_dv.py` & `mrc-0.3.1/tests/test_dv.py`

 * *Files identical despite different names*

### Comparing `mrc-0.3.0/tests/toxo.dv` & `mrc-0.3.1/tests/toxo.dv`

 * *Files identical despite different names*


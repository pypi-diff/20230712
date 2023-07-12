# Comparing `tmp/inline_snapshot-0.2.1.tar.gz` & `tmp/inline_snapshot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inline_snapshot-0.2.1.tar", max compression
+gzip compressed data, was "inline_snapshot-0.3.0.tar", max compression
```

## Comparing `inline_snapshot-0.2.1.tar` & `inline_snapshot-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2023-06-20 18:24:16.714717 inline_snapshot-0.2.1/LICENSE
--rw-r--r--   0        0        0     2053 2023-06-20 18:24:23.890787 inline_snapshot-0.2.1/README.md
--rw-r--r--   0        0        0       62 2023-06-20 18:24:16.714717 inline_snapshot-0.2.1/inline_snapshot/__init__.py
--rw-r--r--   0        0        0      248 2023-07-09 13:33:21.148429 inline_snapshot-0.2.1/inline_snapshot/_format.py
--rw-r--r--   0        0        0    14708 2023-07-09 13:33:21.148429 inline_snapshot-0.2.1/inline_snapshot/_inline_snapshot.py
--rw-r--r--   0        0        0     5448 2023-07-09 13:33:21.148429 inline_snapshot-0.2.1/inline_snapshot/_rewrite_code.py
--rw-r--r--   0        0        0     5445 2023-06-20 18:24:23.890787 inline_snapshot-0.2.1/inline_snapshot/pytest_plugin.py
--rw-r--r--   0        0        0     1620 2023-07-09 13:34:15.181578 inline_snapshot-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3433 1970-01-01 00:00:00.000000 inline_snapshot-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-20 18:24:16.714717 inline_snapshot-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3075 2023-07-09 19:32:08.031840 inline_snapshot-0.3.0/README.md
+-rw-r--r--   0        0        0       62 2023-07-12 16:51:48.846767 inline_snapshot-0.3.0/inline_snapshot/__init__.py
+-rw-r--r--   0        0        0      248 2023-07-09 13:33:21.148429 inline_snapshot-0.3.0/inline_snapshot/_format.py
+-rw-r--r--   0        0        0    14832 2023-07-12 16:34:33.544136 inline_snapshot-0.3.0/inline_snapshot/_inline_snapshot.py
+-rw-r--r--   0        0        0     5448 2023-07-09 13:33:21.148429 inline_snapshot-0.3.0/inline_snapshot/_rewrite_code.py
+-rw-r--r--   0        0        0     5445 2023-07-09 14:55:53.631461 inline_snapshot-0.3.0/inline_snapshot/pytest_plugin.py
+-rw-r--r--   0        0        0     1620 2023-07-12 16:51:48.846767 inline_snapshot-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4455 1970-01-01 00:00:00.000000 inline_snapshot-0.3.0/PKG-INFO
```

### Comparing `inline_snapshot-0.2.1/LICENSE` & `inline_snapshot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.2.1/README.md` & `inline_snapshot-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # inline-snapshot
 
 [![Docs](https://img.shields.io/badge/docs-mkdocs-green)](https://15r10nk.github.io/inline-snapshot/)
 [![pypi version](https://img.shields.io/pypi/v/inline-snapshot.svg)](https://pypi.org/project/inline-snapshot/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/inline-snapshot)
+[![coverage](https://img.shields.io/badge/coverage-100%25-blue)](https://15r10nk.github.io/inline-snapshot/contributing/#coverage)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/15r10nk)](https://github.com/sponsors/15r10nk)
 
 > *create and update inline snapshots in your code.*
 
 ## Installation
 
 You can install "inline-snapshot" via [pip](https://pypi.org/project/pip/):
@@ -15,57 +16,82 @@
 pip install inline-snapshot
 ```
 
 ## Usage
 
 You can use `snapshot()` instead of the value which you want to compare with.
 
+<!-- inline-snapshot: outcome-errors=1 outcome-passed=1 -->
 ```python
 from inline_snapshot import snapshot
 
 
 def test_something():
     assert 1548 * 18489 == snapshot()
 ```
 
 You can now run the tests and record the correct values.
 
 ```
 $ pytest --inline-snapshot=create
 ```
 
+<!-- inline-snapshot: create -->
 ```python
 from inline_snapshot import snapshot
 
 
 def test_something():
     assert 1548 * 18489 == snapshot(28620972)
 ```
 
-## Features
+inline-snapshot provides more advanced features like:
 
-- manage snapshots with `pytest --inline-snapshot=(create,update,fix,trim)`.
-- uses `repr()` to convert the value to python code.
-- values are stored in the source code and not in separate files.
-- `snapshot()` supports the following operations:
-  - `x == snapshot()`
-  - `x <= snapshot()`
-  - `x >= snapshot()`
-  - `x in snapshot()`
-  - `snapshot()[key]`
-- code is formatted with black if the file was already formatted with black.
+<!-- inline-snapshot: fix create trim this -->
+```python
+from inline_snapshot import snapshot
 
-More information can be found in the [documentation](https://15r10nk.github.io/inline-snapshot/).
 
-## Contributing
+def test_something():
+    for number in range(5):
+        # testing for numeric limits
+        assert number <= snapshot(4)
+        assert number >= snapshot(0)
+
+    for c in "hello world":
+        # test if something is part of a set
+        assert c in snapshot(["h", "e", "l", "o", " ", "w", "r", "d"])
+
+    s = snapshot(
+        {
+            0: {"square": 0, "pow_of_two": False},
+            1: {"square": 1, "pow_of_two": True},
+            2: {"square": 4, "pow_of_two": True},
+            3: {"square": 9, "pow_of_two": False},
+            4: {"square": 16, "pow_of_two": True},
+        }
+    )
+
+    for number in range(5):
+        # create sub-snapshots at runtime
+        assert s[number]["square"] == number**2
+        assert s[number]["pow_of_two"] == ((number & (number - 1) == 0) and number != 0)
+```
 
-Contributions are very welcome.
-Tests can be run with [nox](https://nox.thea.codes/en/stable/).
-Please use [pre-commit](https://pre-commit.com/) for your commits.
+More information can be found in the [documentation](https://15r10nk.github.io/inline-snapshot/).
 
-## License
+<!-- -8<- [start:Feedback] -->
+## Feedback
 
-Distributed under the terms of the [MIT](http://opensource.org/licenses/MIT) license, "inline-snapshot" is free and open source software.
+inline-snapshot provides some advanced ways to work with snapshots.
+
+I would like to know how these features are used to further improve this small library.
+Let me know if you've found interesting use cases for this library via [twitter](https://twitter.com/15r10nk) or in the github [discussions](https://github.com/15r10nk/inline-snapshot/discussions/new?category=show-and-tell).
 
 ## Issues
 
-If you encounter any problems, please [file an issue](https://github.com/15r10nk/inline-snapshot/issues) along with a detailed description.
+If you encounter any problems, please [report an issue](https://github.com/15r10nk/inline-snapshot/issues) along with a detailed description.
+<!-- -8<- [end:Feedback] -->
+
+## License
+
+Distributed under the terms of the [MIT](http://opensource.org/licenses/MIT) license, "inline-snapshot" is free and open source software.
```

### Comparing `inline_snapshot-0.2.1/inline_snapshot/_inline_snapshot.py` & `inline_snapshot-0.3.0/inline_snapshot/_inline_snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import ast
 import contextlib
+import copy
 import inspect
 import io
 import token
 import tokenize
 from pathlib import Path
 from typing import Any
 from typing import Dict  # noqa
@@ -147,14 +148,16 @@
     def __getitem__(self, item):
         self._change(DictValue)
         return self[item]
 
 
 class FixValue(GenericValue):
     def __eq__(self, other):
+        other = copy.deepcopy(other)
+
         if self._new_value is undefined:
             self._new_value = other
 
         return self._visible_value() == other
 
     def _needs_fix(self):
         return self._old_value is not undefined and self._old_value != self._new_value
@@ -167,14 +170,16 @@
     """generic implementation for <=, >="""
 
     @staticmethod
     def cmp(a, b):
         raise NotImplemented
 
     def _generic_cmp(self, other):
+        other = copy.deepcopy(other)
+
         if self._new_value is undefined:
             self._new_value = other
         else:
             self._new_value = (
                 self._new_value if self.cmp(self._new_value, other) else other
             )
 
@@ -254,14 +259,16 @@
         return a >= b
 
     __ge__ = MinMaxValue._generic_cmp
 
 
 class CollectionValue(GenericValue):
     def __contains__(self, item):
+        item = copy.deepcopy(item)
+
         if self._new_value is undefined:
             self._new_value = [item]
         else:
             if item not in self._new_value:
                 self._new_value.append(item)
 
         if ignore_old_value() or self._old_value is undefined:
```

### Comparing `inline_snapshot-0.2.1/inline_snapshot/_rewrite_code.py` & `inline_snapshot-0.3.0/inline_snapshot/_rewrite_code.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.2.1/inline_snapshot/pytest_plugin.py` & `inline_snapshot-0.3.0/inline_snapshot/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.2.1/pyproject.toml` & `inline_snapshot-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Framework :: Pytest"
 ]
 description = "golden master/snapshot/approval testing library which puts the values right into your source code"
 license = "MIT"
 name = "inline-snapshot"
 readme = "README.md"
 repository = "https://github.com/15r10nk/inline-snapshots"
-version = "0.2.1"
+version = "0.3.0"
 
 [tool.poetry.dependencies]
 asttokens = "^2.0.5"
 black = "^23.3.0"
 click = "^8.1.4"
 executing = "^1.2.0"
 python = "^3.7"
```

### Comparing `inline_snapshot-0.2.1/PKG-INFO` & `inline_snapshot-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inline-snapshot
-Version: 0.2.1
+Version: 0.3.0
 Summary: golden master/snapshot/approval testing library which puts the values right into your source code
 Home-page: https://github.com/15r10nk/inline-snapshots
 License: MIT
 Author: Frank Hoffmann
 Author-email: 15r10nk@polarbit.de
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -30,14 +30,15 @@
 Description-Content-Type: text/markdown
 
 # inline-snapshot
 
 [![Docs](https://img.shields.io/badge/docs-mkdocs-green)](https://15r10nk.github.io/inline-snapshot/)
 [![pypi version](https://img.shields.io/pypi/v/inline-snapshot.svg)](https://pypi.org/project/inline-snapshot/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/inline-snapshot)
+[![coverage](https://img.shields.io/badge/coverage-100%25-blue)](https://15r10nk.github.io/inline-snapshot/contributing/#coverage)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/15r10nk)](https://github.com/sponsors/15r10nk)
 
 > *create and update inline snapshots in your code.*
 
 ## Installation
 
 You can install "inline-snapshot" via [pip](https://pypi.org/project/pip/):
@@ -46,58 +47,83 @@
 pip install inline-snapshot
 ```
 
 ## Usage
 
 You can use `snapshot()` instead of the value which you want to compare with.
 
+<!-- inline-snapshot: outcome-errors=1 outcome-passed=1 -->
 ```python
 from inline_snapshot import snapshot
 
 
 def test_something():
     assert 1548 * 18489 == snapshot()
 ```
 
 You can now run the tests and record the correct values.
 
 ```
 $ pytest --inline-snapshot=create
 ```
 
+<!-- inline-snapshot: create -->
 ```python
 from inline_snapshot import snapshot
 
 
 def test_something():
     assert 1548 * 18489 == snapshot(28620972)
 ```
 
-## Features
+inline-snapshot provides more advanced features like:
 
-- manage snapshots with `pytest --inline-snapshot=(create,update,fix,trim)`.
-- uses `repr()` to convert the value to python code.
-- values are stored in the source code and not in separate files.
-- `snapshot()` supports the following operations:
-  - `x == snapshot()`
-  - `x <= snapshot()`
-  - `x >= snapshot()`
-  - `x in snapshot()`
-  - `snapshot()[key]`
-- code is formatted with black if the file was already formatted with black.
+<!-- inline-snapshot: fix create trim this -->
+```python
+from inline_snapshot import snapshot
 
-More information can be found in the [documentation](https://15r10nk.github.io/inline-snapshot/).
 
-## Contributing
+def test_something():
+    for number in range(5):
+        # testing for numeric limits
+        assert number <= snapshot(4)
+        assert number >= snapshot(0)
+
+    for c in "hello world":
+        # test if something is part of a set
+        assert c in snapshot(["h", "e", "l", "o", " ", "w", "r", "d"])
+
+    s = snapshot(
+        {
+            0: {"square": 0, "pow_of_two": False},
+            1: {"square": 1, "pow_of_two": True},
+            2: {"square": 4, "pow_of_two": True},
+            3: {"square": 9, "pow_of_two": False},
+            4: {"square": 16, "pow_of_two": True},
+        }
+    )
+
+    for number in range(5):
+        # create sub-snapshots at runtime
+        assert s[number]["square"] == number**2
+        assert s[number]["pow_of_two"] == ((number & (number - 1) == 0) and number != 0)
+```
 
-Contributions are very welcome.
-Tests can be run with [nox](https://nox.thea.codes/en/stable/).
-Please use [pre-commit](https://pre-commit.com/) for your commits.
+More information can be found in the [documentation](https://15r10nk.github.io/inline-snapshot/).
 
-## License
+<!-- -8<- [start:Feedback] -->
+## Feedback
 
-Distributed under the terms of the [MIT](http://opensource.org/licenses/MIT) license, "inline-snapshot" is free and open source software.
+inline-snapshot provides some advanced ways to work with snapshots.
+
+I would like to know how these features are used to further improve this small library.
+Let me know if you've found interesting use cases for this library via [twitter](https://twitter.com/15r10nk) or in the github [discussions](https://github.com/15r10nk/inline-snapshot/discussions/new?category=show-and-tell).
 
 ## Issues
 
-If you encounter any problems, please [file an issue](https://github.com/15r10nk/inline-snapshot/issues) along with a detailed description.
+If you encounter any problems, please [report an issue](https://github.com/15r10nk/inline-snapshot/issues) along with a detailed description.
+<!-- -8<- [end:Feedback] -->
+
+## License
+
+Distributed under the terms of the [MIT](http://opensource.org/licenses/MIT) license, "inline-snapshot" is free and open source software.
```


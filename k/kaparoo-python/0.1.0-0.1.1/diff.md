# Comparing `tmp/kaparoo_python-0.1.0.tar.gz` & `tmp/kaparoo_python-0.1.1.tar.gz`

## Comparing `kaparoo_python-0.1.0.tar` & `kaparoo_python-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/kaparoo/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/kaparoo/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/kaparoo/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/kaparoo/beartype/__init__.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/kaparoo/beartype/numerics.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/kaparoo/filesystem/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/kaparoo/filesystem/exceptions.py
--rw-r--r--   0        0        0    23982 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/kaparoo/filesystem/path.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/kaparoo/filesystem/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/kaparoo/utils/__init__.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/kaparoo/utils/optional.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/kaparoo/utils/types.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/LICENSE
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/README.md
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 kaparoo_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/beartype/__init__.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/beartype/numerics.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/filesystem/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/filesystem/exceptions.py
+-rw-r--r--   0        0        0    24132 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/filesystem/path.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/filesystem/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/utils/__init__.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/utils/optional.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/utils/types.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/README.md
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/PKG-INFO
```

### Comparing `kaparoo_python-0.1.0/kaparoo/beartype/numerics.py` & `kaparoo_python-0.1.1/kaparoo/beartype/numerics.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.0/kaparoo/filesystem/__init__.py` & `kaparoo_python-0.1.1/kaparoo/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.0/kaparoo/filesystem/path.py` & `kaparoo_python-0.1.1/kaparoo/filesystem/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,22 +41,27 @@
 
 
 # ========================== #
 #          Stringify         #
 # ========================== #
 
 
-def stringify_path(path: StrPath) -> str:
+def stringify_path(path: StrPath, relative_to: StrPath | None = None) -> str:
     """Convert a path to a string representation."""
-    return os.fspath(path)
+    path = os.fspath(path)
+    if relative_to is not None:
+        path = os.path.relpath(path, relative_to)
+    return path
 
 
-def stringify_paths(paths: StrPaths) -> Sequence[str]:
+def stringify_paths(
+    *paths: StrPath, relative_to: StrPath | None = None
+) -> Sequence[str]:
     """Convert a sequence of paths to a sequence of string representations."""
-    return [stringify_path(p) for p in paths]
+    return [stringify_path(p, relative_to) for p in paths]
 
 
 # ========================== #
 #      Single Existence      #
 # ========================== #
 
 
@@ -186,38 +191,37 @@
 # ========================== #
 #    Multiple Existences     #
 # ========================== #
 
 
 @overload
 def check_if_paths_exist(
-    paths: StrPaths,
-    *,
+    *paths: StrPath,
     root: StrPath | None = None,
     stringify: Literal[False] = False,
 ) -> Sequence[Path]:
     ...
 
 
 @overload
 def check_if_paths_exist(
-    paths: StrPaths, *, root: StrPath | None = None, stringify: Literal[True]
+    *paths: StrPath, root: StrPath | None = None, stringify: Literal[True]
 ) -> Sequence[str]:
     ...
 
 
 @overload
 def check_if_paths_exist(
-    paths: StrPaths, *, root: StrPath | None = None, stringify: bool
+    *paths: StrPath, root: StrPath | None = None, stringify: bool
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
 def check_if_paths_exist(
-    paths: StrPaths, *, root: StrPath | None = None, stringify: bool = False
+    *paths: StrPath, root: StrPath | None = None, stringify: bool = False
 ) -> Sequence[Path] | Sequence[str]:
     """Check if multiple paths exist and return them as a sequence of `Path` objects.
 
     Args:
         paths: A sequence of paths to check for existence.
         root: The root directory to resolve relative paths. If provided, the `paths`
             will be resolved relative to the `root` directory. Defaults to `None`.
@@ -231,47 +235,44 @@
         DirectoryNotFoundError: If the `root` directory does not exist.
         NotADirectoryError: If `root` exists but is not a directory.
         FileNotFoundError: If any of the paths does not exist.
     """
 
     if root is not None:
         root = check_if_dir_exists(root)
-        paths = [root / p for p in paths]
+        paths = tuple(root / p for p in paths)
 
     paths = [check_if_path_exists(p) for p in paths]
 
-    return stringify_paths(paths) if stringify else paths
+    return stringify_paths(*paths) if stringify else paths
 
 
 @overload
 def check_if_files_exist(
-    paths: StrPaths,
-    *,
-    root: StrPath | None = None,
-    stringify: Literal[False] = False,
+    *paths: StrPath, root: StrPath | None = None, stringify: Literal[False] = False
 ) -> Sequence[Path]:
     ...
 
 
 @overload
 def check_if_files_exist(
-    paths: StrPaths, *, root: StrPath | None = None, stringify: Literal[True]
+    *paths: StrPath, root: StrPath | None = None, stringify: Literal[True]
 ) -> Sequence[str]:
     ...
 
 
 @overload
 def check_if_files_exist(
-    paths: StrPaths, *, root: StrPath | None = None, stringify: bool
+    *paths: StrPath, root: StrPath | None = None, stringify: bool
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
 def check_if_files_exist(
-    paths: StrPaths, *, root: StrPath | None = None, stringify: bool = False
+    *paths: StrPath, root: StrPath | None = None, stringify: bool = False
 ) -> Sequence[Path] | Sequence[str]:
     """Check if multiple files exist and return them as a sequence of `Path` objects.
 
     Args:
         paths: A sequence of file paths to check for existence.
         root: The root directory to resolve relative paths. If provided, the `paths`
             will be resolved relative to the `root` directory. Defaults to `None`.
@@ -286,57 +287,53 @@
         NotADirectoryError: If `root` exists but is not a directory.
         FileNotFoundError: If any of the file paths does not exist.
         NotAFileError: If any of the paths exists but is not a file.
     """  # noqa: E501
 
     if root is not None:
         root = check_if_dir_exists(root)
-        paths = [root / p for p in paths]
+        paths = tuple(root / p for p in paths)
 
     paths = [check_if_file_exists(p) for p in paths]
 
-    return stringify_paths(paths) if stringify else paths
+    return stringify_paths(*paths) if stringify else paths
 
 
 @overload
 def check_if_dirs_exist(
-    paths: StrPaths,
-    *,
+    *paths: StrPath,
     root: StrPath | None = None,
     make: bool | int = False,
     stringify: Literal[False] = False,
 ) -> Sequence[Path]:
     ...
 
 
 @overload
 def check_if_dirs_exist(
-    paths: StrPaths,
-    *,
+    *paths: StrPath,
     root: StrPath | None = None,
     make: bool | int = False,
     stringify: Literal[True],
 ) -> Sequence[str]:
     ...
 
 
 @overload
 def check_if_dirs_exist(
-    paths: StrPaths,
-    *,
+    *paths: StrPath,
     root: StrPath | None = None,
     make: bool | int = False,
     stringify: bool,
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
 def check_if_dirs_exist(
-    paths: StrPaths,
-    *,
+    *paths: StrPath,
     root: StrPath | None = None,
     make: bool | int = False,
     stringify: bool = False,
 ) -> Sequence[Path] | Sequence[str]:
     """Check if multiple directories exist and return them as a sequence of `Path` objects.
 
     Args:
@@ -356,19 +353,19 @@
         DirectoryNotFoundError: If any of the directory paths does not exist.
         NotADirectoryError: If `root` exists but is not a directory.
         NotADirectoryError: If any of the paths exists but is not a directory.
     """  # noqa: E501
 
     if root is not None:
         root = check_if_dir_exists(root)
-        paths = [root / p for p in paths]
+        paths = tuple(root / p for p in paths)
 
     paths = [check_if_dir_exists(p, make=make) for p in paths]
 
-    return stringify_paths(paths) if stringify else paths
+    return stringify_paths(*paths) if stringify else paths
 
 
 # ========================== #
 #    Child Path(s) Search    #
 # ========================== #
 
 
@@ -376,56 +373,56 @@
 def get_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
-    recursive: bool = True,
+    recursive: bool = False,
     stringify: Literal[False] = False,
 ) -> Sequence[Path]:
     ...
 
 
 @overload
 def get_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
-    recursive: bool = True,
+    recursive: bool = False,
     stringify: Literal[True],
 ) -> Sequence[str]:
     ...
 
 
 @overload
 def get_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
-    recursive: bool = True,
+    recursive: bool = False,
     stringify: bool,
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
 def get_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
-    recursive: bool = True,
+    recursive: bool = False,
     stringify: bool = False,
 ) -> Sequence[Path] | Sequence[str]:
     """Get paths of files or directories in a given directory.
 
     Args:
         root: The directory to search for paths.
         pattern: A glob pattern to match the paths against. Defaults to `None` and
@@ -436,15 +433,15 @@
             of `num_samples`, may return a different result. Defaults to `None`.
         ignores: A sequence of paths to ignore. If any path in `ignores` does not start
             with `root`, it is treated as a relative path. For example, `any/path` is
             treated as `root/any/path`. Defaults to `None`.
         condition: A predicate that takes a `Path` object and decides whether to include
             the path in the results. Defaults to `None`.
         recursive: Whether to search for paths recursively in subdirectories of the
-            `root` directory. Defaults to `True`.
+            `root` directory. Defaults to `False`.
         stringify: Whether to return a sequence of strings. Defaults to `False`.
 
     Returns:
         The paths that match the specified criteria as a sequence of `Path` objects or a
             sequence of strings, depending on the value of `stringify`.
 
     Raises:
@@ -479,67 +476,67 @@
         paths = [p for p in paths if condition(p)]
 
     if isinstance(num_samples, int) and num_samples < len(paths):
         if num_samples <= 0:
             raise ValueError("`num_samples` must be a positive int")
         paths = random.sample(paths, num_samples)
 
-    return stringify_paths(paths) if stringify else paths
+    return stringify_paths(*paths) if stringify else paths
 
 
 @overload
 def get_files(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
-    recursive: bool = True,
+    recursive: bool = False,
     stringify: Literal[False] = False,
 ) -> Sequence[Path]:
     ...
 
 
 @overload
 def get_files(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
-    recursive: bool = True,
+    recursive: bool = False,
     stringify: Literal[True],
 ) -> Sequence[str]:
     ...
 
 
 @overload
 def get_files(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
-    recursive: bool = True,
+    recursive: bool = False,
     stringify: bool,
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
 def get_files(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
-    recursive: bool = True,
+    recursive: bool = False,
     stringify: bool = False,
 ) -> Sequence[Path] | Sequence[str]:
     """Get paths of files in a given directory.
 
     Args:
         root: The directory to search for paths.
         pattern: A glob pattern to match the paths against. Defaults to `None` and
@@ -550,15 +547,15 @@
             of `num_samples`, may return a different result. Defaults to `None`.
         ignores: A sequence of paths to ignore. If any path in `ignores` does not start
             with `root`, it is treated as a relative path. For example, `any/path` is
             treated as `root/any/path`. Defaults to `None`.
         condition: A predicate that takes a `Path` object and decides whether to include
             the path in the results. Defaults to `None`.
         recursive: Whether to search for paths recursively in subdirectories of the
-            `root` directory. Defaults to `True`.
+            `root` directory. Defaults to `False`.
         stringify: Whether to return a sequence of strings. Defaults to `False`.
 
     Returns:
         The file paths that match the specified criteria as a sequence of `Path` objects
             or a sequence of strings, depending on the value of `stringify`.
 
     Raises:
@@ -589,56 +586,56 @@
 def get_dirs(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
-    recursive: bool = True,
+    recursive: bool = False,
     stringify: Literal[False] = False,
 ) -> Sequence[Path]:
     ...
 
 
 @overload
 def get_dirs(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
-    recursive: bool = True,
+    recursive: bool = False,
     stringify: Literal[True],
 ) -> Sequence[str]:
     ...
 
 
 @overload
 def get_dirs(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
-    recursive: bool = True,
+    recursive: bool = False,
     stringify: bool,
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
 def get_dirs(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: StrPaths | None = None,
     condition: Callable[[Path], bool] | None = None,
-    recursive: bool = True,
+    recursive: bool = False,
     stringify: bool = False,
 ) -> Sequence[Path] | Sequence[str]:
     """Get paths of directories in a given directory.
 
     Args:
         root: The directory to search for paths.
         pattern: A glob pattern to match the paths against. Defaults to `None` and
@@ -649,15 +646,15 @@
             of `num_samples`, may return a different result. Defaults to `None`.
         ignores: A sequence of paths to ignore. If any path in `ignores` does not start
             with `root`, it is treated as a relative path. For example, `any/path` is
             treated as `root/any/path`. Defaults to `None`.
         condition: A predicate that takes a `Path` object and decides whether to include
             the path in the results. Defaults to `None`.
         recursive: Whether to search for paths recursively in subdirectories of the
-            `root` directory. Defaults to `True`.
+            `root` directory. Defaults to `False`.
         stringify: Whether to return a sequence of strings. Defaults to `False`.
 
     Returns:
         The directory paths that match the specified criteria as a sequence of `Path`
             objects or a sequence of strings, depending on the value of `stringify`.
 
     Raises:
@@ -717,34 +714,34 @@
         DirectoryNotFoundError: If the directory does not exist.
         NotADirectoryError: If `path` exists but is not a directory.
     """
     path = check_if_dir_exists(path)
     return is_empty_dir_unsafe(path)
 
 
-def are_empty_dirs_unsafe(paths: StrPaths, *, root: StrPath | None = None) -> bool:
+def are_empty_dirs_unsafe(*paths: StrPath, root: StrPath | None = None) -> bool:
     """Check if multiple directories are empty.
 
     Unlike the function `are_empty_dirs()`, this function does not check the existence
     of the input arguments `paths` and `root`. Use this function only if you are sure
     they exist.
 
     Args:
         paths: A sequence of directory paths to check.
         root: The root directory to resolve relative paths. Defaults to `None`.
 
     Returns:
         A boolean indicating whether all directories are empty.
     """
     if root is not None:
-        paths = [os.path.join(root, p) for p in paths]
+        paths = tuple(os.path.join(root, p) for p in paths)
     return all(is_empty_dir_unsafe(p) for p in paths)
 
 
-def are_empty_dirs(paths: StrPaths, *, root: StrPath | None = None) -> bool:
+def are_empty_dirs(*paths: StrPath, root: StrPath | None = None) -> bool:
     """Check if multiple directories are empty.
 
     Args:
         paths: A sequence of directory paths to check.
         root: The root directory to resolve relative paths. Defaults to `None`.
 
     Returns:
```

### Comparing `kaparoo_python-0.1.0/kaparoo/utils/optional.py` & `kaparoo_python-0.1.1/kaparoo/utils/optional.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.0/.gitignore` & `kaparoo_python-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.0/LICENSE` & `kaparoo_python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.0/README.md` & `kaparoo_python-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.0/pyproject.toml` & `kaparoo_python-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 dependencies = [
     "beartype>=0.14.1",
 ]
 
 [project.optional-dependencies]
 dev = [
     "hatch>=1.7.0",
-    "ruff>=0.0.274",
-    "mypy>=1.3.0",
-    "black>=23.3.0",
-    "pytest>=7.3.2",
+    "ruff>=0.0.277",
+    "mypy>=1.4.1",
+    "black>=23.7.0",
+    "pytest>=7.4.0",
     "pytest-order>=1.1.0",
 ]
 
 [project.urls]
 GitHub = "https://www.github.com/kaparoo/python-package"
 
 # ========================== #
```

### Comparing `kaparoo_python-0.1.0/PKG-INFO` & `kaparoo_python-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaparoo-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for (personally) common and useful features.
 Project-URL: GitHub, https://www.github.com/kaparoo/python-package
 Author-email: Jaewoo Park <kaparoo2001@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jaewoo Park
         
@@ -35,20 +35,20 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: beartype>=0.14.1
 Provides-Extra: dev
-Requires-Dist: black>=23.3.0; extra == 'dev'
+Requires-Dist: black>=23.7.0; extra == 'dev'
 Requires-Dist: hatch>=1.7.0; extra == 'dev'
-Requires-Dist: mypy>=1.3.0; extra == 'dev'
+Requires-Dist: mypy>=1.4.1; extra == 'dev'
 Requires-Dist: pytest-order>=1.1.0; extra == 'dev'
-Requires-Dist: pytest>=7.3.2; extra == 'dev'
-Requires-Dist: ruff>=0.0.274; extra == 'dev'
+Requires-Dist: pytest>=7.4.0; extra == 'dev'
+Requires-Dist: ruff>=0.0.277; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # ***kaparoo-python-package***
 
 
 
 <!-- [              MARKDOWN BADGES              ] -->
```


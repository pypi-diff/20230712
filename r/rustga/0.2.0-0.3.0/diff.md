# Comparing `tmp/rustga-0.2.0.tar.gz` & `tmp/rustga-0.3.0.tar.gz`

## Comparing `rustga-0.2.0.tar` & `rustga-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0      362 1970-01-01 00:00:00.000000 rustga-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123       45 2023-01-27 17:45:50.000000 rustga-0.2.0/.config/rustfmt.toml
--rw-r--r--   0     1001      123     1215 2023-01-27 17:45:50.000000 rustga-0.2.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     1046 2023-01-27 17:45:50.000000 rustga-0.2.0/.github/workflows/_workflow.yml
--rw-r--r--   0     1001      123      685 2023-01-27 17:45:50.000000 rustga-0.2.0/.gitignore
--rw-r--r--   0     1001      123      505 2023-01-27 17:45:50.000000 rustga-0.2.0/Dockerfile
--rw-r--r--   0     1001      123      108 2023-01-27 17:45:50.000000 rustga-0.2.0/README.md
--rw-r--r--   0     1001      123       90 2023-01-27 17:45:50.000000 rustga-0.2.0/docker-compose.yml
--rw-r--r--   0     1001      123     1933 2023-01-27 17:45:50.000000 rustga-0.2.0/examples/search_range_test.py
--rw-r--r--   0     1001      123     1074 2023-01-27 17:45:50.000000 rustga-0.2.0/examples/test.py
--rw-r--r--   0     1001      123     3176 2023-01-27 17:45:50.000000 rustga-0.2.0/poetry.lock
--rw-r--r--   0     1001      123      496 2023-01-27 17:45:50.000000 rustga-0.2.0/pyproject.toml
--rwxr-xr-x   0     1001      123      993 2023-01-27 17:47:55.000000 rustga-0.2.0/run-maturin-action.sh
--rw-r--r--   0     1001      123     2981 2023-01-27 17:45:50.000000 rustga-0.2.0/src/crossover.rs
--rw-r--r--   0     1001      123     4071 2023-01-27 17:45:50.000000 rustga-0.2.0/src/generation_iterator.rs
--rw-r--r--   0     1001      123     9860 2023-01-27 17:45:50.000000 rustga-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123     3483 2023-01-27 17:45:50.000000 rustga-0.2.0/src/mutation.rs
--rw-r--r--   0     1001      123     5385 2023-01-27 17:45:50.000000 rustga-0.2.0/src/search_range.rs
--rw-r--r--   0     1001      123     1364 2023-01-27 17:45:50.000000 rustga-0.2.0/src/selection.rs
--rw-r--r--   0     1001      123     9418 2023-01-27 17:45:50.000000 rustga-0.2.0/Cargo.lock
--rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 rustga-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      362 1970-01-01 00:00:00.000000 rustga-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123       45 2023-07-12 04:27:39.000000 rustga-0.3.0/.config/rustfmt.toml
+-rw-r--r--   0     1001      123     1202 2023-07-12 04:27:39.000000 rustga-0.3.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     1046 2023-07-12 04:27:39.000000 rustga-0.3.0/.github/workflows/_workflow.yml
+-rw-r--r--   0     1001      123      685 2023-07-12 04:27:39.000000 rustga-0.3.0/.gitignore
+-rw-r--r--   0     1001      123      505 2023-07-12 04:27:39.000000 rustga-0.3.0/Dockerfile
+-rw-r--r--   0     1001      123      108 2023-07-12 04:27:39.000000 rustga-0.3.0/README.md
+-rw-r--r--   0     1001      123       90 2023-07-12 04:27:39.000000 rustga-0.3.0/docker-compose.yml
+-rw-r--r--   0     1001      123     1933 2023-07-12 04:27:39.000000 rustga-0.3.0/examples/search_range_test.py
+-rw-r--r--   0     1001      123     1074 2023-07-12 04:27:39.000000 rustga-0.3.0/examples/test.py
+-rw-r--r--   0     1001      123     3176 2023-07-12 04:27:39.000000 rustga-0.3.0/poetry.lock
+-rw-r--r--   0     1001      123      484 2023-07-12 04:27:39.000000 rustga-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123     2981 2023-07-12 04:27:39.000000 rustga-0.3.0/src/crossover.rs
+-rw-r--r--   0     1001      123     4071 2023-07-12 04:27:39.000000 rustga-0.3.0/src/generation_iterator.rs
+-rw-r--r--   0     1001      123     9860 2023-07-12 04:27:39.000000 rustga-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123     3483 2023-07-12 04:27:39.000000 rustga-0.3.0/src/mutation.rs
+-rw-r--r--   0     1001      123     5385 2023-07-12 04:27:39.000000 rustga-0.3.0/src/search_range.rs
+-rw-r--r--   0     1001      123     1364 2023-07-12 04:27:39.000000 rustga-0.3.0/src/selection.rs
+-rw-r--r--   0     1001      123     9418 2023-07-12 04:27:39.000000 rustga-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 rustga-0.3.0/PKG-INFO
```

### Comparing `rustga-0.2.0/.github/workflows/CI.yml` & `rustga-0.3.0/.github/workflows/CI.yml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
       maturin-build-args: --release -o dist --find-interpreter
 
   macos:
     uses: ./.github/workflows/_workflow.yml
     with:
       runs-on: macos-latest
       maturin-target: x86_64
-      maturin-build-args: --release -o dist --universal2 --find-interpreter
+      maturin-build-args: --release -o dist --find-interpreter
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
     needs: [ macos, windows, linux ]
     steps:
```

### Comparing `rustga-0.2.0/.github/workflows/_workflow.yml` & `rustga-0.3.0/.github/workflows/_workflow.yml`

 * *Files identical despite different names*

### Comparing `rustga-0.2.0/.gitignore` & `rustga-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rustga-0.2.0/examples/search_range_test.py` & `rustga-0.3.0/examples/search_range_test.py`

 * *Files identical despite different names*

### Comparing `rustga-0.2.0/examples/test.py` & `rustga-0.3.0/examples/test.py`

 * *Files identical despite different names*

### Comparing `rustga-0.2.0/poetry.lock` & `rustga-0.3.0/poetry.lock`

 * *Files identical despite different names*

### Comparing `rustga-0.2.0/src/crossover.rs` & `rustga-0.3.0/src/crossover.rs`

 * *Files identical despite different names*

### Comparing `rustga-0.2.0/src/generation_iterator.rs` & `rustga-0.3.0/src/generation_iterator.rs`

 * *Files identical despite different names*

### Comparing `rustga-0.2.0/src/lib.rs` & `rustga-0.3.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rustga-0.2.0/src/mutation.rs` & `rustga-0.3.0/src/mutation.rs`

 * *Files identical despite different names*

### Comparing `rustga-0.2.0/src/search_range.rs` & `rustga-0.3.0/src/search_range.rs`

 * *Files identical despite different names*

### Comparing `rustga-0.2.0/src/selection.rs` & `rustga-0.3.0/src/selection.rs`

 * *Files identical despite different names*

### Comparing `rustga-0.2.0/Cargo.lock` & `rustga-0.3.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rustga"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "anyhow",
  "itertools",
  "ordered-float",
  "pyo3",
  "rand",
 ]
```


# Comparing `tmp/extract_drugs-1.0.0.tar.gz` & `tmp/extract_drugs-1.0.1.tar.gz`

## Comparing `extract_drugs-1.0.0.tar` & `extract_drugs-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 extract_drugs-1.0.0/Cargo.toml
--rw-r--r--   0      501       20      287 2023-05-30 02:55:34.000000 extract_drugs-1.0.0/.gitignore
--rw-r--r--   0      501       20     4106 2022-06-27 14:19:06.000000 extract_drugs-1.0.0/CONTRIBUTING.md
--rw-r--r--   0      501       20    18596 2023-05-30 02:55:34.000000 extract_drugs-1.0.0/Cargo.lock
--rw-r--r--   0      501       20     1053 2023-05-30 03:02:23.000000 extract_drugs-1.0.0/LICENSE.md
--rw-r--r--   0      501       20     5224 2023-05-30 02:55:34.000000 extract_drugs-1.0.0/README.md
--rw-r--r--   0      501       20     1027 2023-05-30 03:06:00.000000 extract_drugs-1.0.0/pyproject.toml
--rw-r--r--   0      501       20    16809 2023-05-30 02:55:34.000000 extract_drugs-1.0.0/src/lib.rs
--rw-r--r--   0      501       20     4329 2023-05-30 02:55:34.000000 extract_drugs-1.0.0/src/main.rs
--rw-r--r--   0        0        0     6251 1970-01-01 00:00:00.000000 extract_drugs-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 extract_drugs-1.0.1/Cargo.toml
+-rw-r--r--   0     1001      123      287 2023-07-12 17:23:05.000000 extract_drugs-1.0.1/.gitignore
+-rw-r--r--   0     1001      123     4106 2023-07-12 17:23:05.000000 extract_drugs-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0     1001      123    18596 2023-07-12 17:23:05.000000 extract_drugs-1.0.1/Cargo.lock
+-rw-r--r--   0     1001      123     1053 2023-07-12 17:23:05.000000 extract_drugs-1.0.1/LICENSE.md
+-rw-r--r--   0     1001      123     5224 2023-07-12 17:23:05.000000 extract_drugs-1.0.1/README.md
+-rw-r--r--   0     1001      123       10 2023-07-12 17:23:21.000000 extract_drugs-1.0.1/dist/extract_drugs-1.0.1.tar.gz
+-rw-r--r--   0     1001      123     1025 2023-07-12 17:23:05.000000 extract_drugs-1.0.1/pyproject.toml
+-rw-r--r--   0     1001      123    16809 2023-07-12 17:23:05.000000 extract_drugs-1.0.1/src/lib.rs
+-rw-r--r--   0     1001      123     4329 2023-07-12 17:23:05.000000 extract_drugs-1.0.1/src/main.rs
+-rw-r--r--   0        0        0     6251 1970-01-01 00:00:00.000000 extract_drugs-1.0.1/PKG-INFO
```

### Comparing `extract_drugs-1.0.0/Cargo.toml` & `extract_drugs-1.0.1/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "drug-extraction-cli"
-version = "1.0.0"
+version = "1.0.1"
 edition = "2021"
 authors = ["Nick Anthony <nicholas.anthony@uky.edu>"]
 description = "A CLI for extracting drugs from text records"
 license = "MIT"
 repository = "https://github.com/UK-IPOP/drug-extraction"
 keywords = ["drug", "extraction", "nlp", "text"]
 categories = ["parsing", "command-line-interface"]
```

### Comparing `extract_drugs-1.0.0/CONTRIBUTING.md` & `extract_drugs-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `extract_drugs-1.0.0/Cargo.lock` & `extract_drugs-1.0.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 dependencies = [
  "console",
  "shell-words",
 ]
 
 [[package]]
 name = "drug-extraction-cli"
-version = "1.0.0"
+version = "1.0.1"
 dependencies = [
  "clap",
  "color-eyre",
  "csv",
  "dialoguer",
  "indicatif",
  "itertools",
```

### Comparing `extract_drugs-1.0.0/LICENSE.md` & `extract_drugs-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `extract_drugs-1.0.0/README.md` & `extract_drugs-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `extract_drugs-1.0.0/pyproject.toml` & `extract_drugs-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["maturin>=0.12,<0.13"]
+requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "extract-drugs"
-version = "1.0.0"
+version = "1.0.1"
 description = "A CLI for extracting drugs from text records"
 license = {file = "LICENSE.md"}
 requires-python = ">=3.7"
 authors = [
     {name = "Nick Anthony", email = "nanthony007@gmail.com"}
 ]
 maintainers = [
```

### Comparing `extract_drugs-1.0.0/src/lib.rs` & `extract_drugs-1.0.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `extract_drugs-1.0.0/src/main.rs` & `extract_drugs-1.0.1/src/main.rs`

 * *Files identical despite different names*

### Comparing `extract_drugs-1.0.0/PKG-INFO` & `extract_drugs-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extract-drugs
-Version: 1.0.0
+Version: 1.0.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Topic :: Text Processing
 License-File: LICENSE.md
```


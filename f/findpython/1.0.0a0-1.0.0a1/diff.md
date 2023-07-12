# Comparing `tmp/findpython-1.0.0a0.tar.gz` & `tmp/findpython-1.0.0a1.tar.gz`

## Comparing `findpython-1.0.0a0.tar` & `findpython-1.0.0a1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 findpython-1.0.0a0/Cargo.toml
--rw-r--r--   0      501       20     3863 2023-07-10 10:24:01.000000 findpython-1.0.0a0/.github/workflows/build.yaml
--rw-r--r--   0      501       20       92 2023-07-10 10:24:01.000000 findpython-1.0.0a0/.gitignore
--rw-r--r--   0      501       20    20768 2023-07-10 10:24:01.000000 findpython-1.0.0a0/Cargo.lock
--rw-r--r--   0      501       20     1075 2023-07-10 10:24:01.000000 findpython-1.0.0a0/LICENSE
--rw-r--r--   0      501       20     5118 2023-07-10 10:24:01.000000 findpython-1.0.0a0/README.md
--rw-r--r--   0      501       20     2056 2023-07-10 10:24:01.000000 findpython-1.0.0a0/findpython.pyi
--rw-r--r--   0      501       20     4121 2023-07-10 10:24:01.000000 findpython-1.0.0a0/pdm.lock
--rw-r--r--   0      501       20      762 2023-07-10 10:24:01.000000 findpython-1.0.0a0/pyproject.toml
--rw-r--r--   0      501       20     2849 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/cli.rs
--rw-r--r--   0      501       20     8831 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/finder.rs
--rw-r--r--   0      501       20     2354 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/helpers.rs
--rw-r--r--   0      501       20      662 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/lib.rs
--rw-r--r--   0      501       20      130 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/main.rs
--rw-r--r--   0      501       20     1688 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/providers/asdf.rs
--rw-r--r--   0      501       20     2003 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/providers/mod.rs
--rw-r--r--   0      501       20     1110 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/providers/path.rs
--rw-r--r--   0      501       20     1662 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/providers/pyenv.rs
--rw-r--r--   0      501       20     1306 2023-07-10 10:24:02.000000 findpython-1.0.0a0/src/providers/rye.rs
--rw-r--r--   0      501       20    14411 2023-07-10 10:24:02.000000 findpython-1.0.0a0/src/python.rs
--rw-r--r--   0        0        0     5586 1970-01-01 00:00:00.000000 findpython-1.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 findpython-1.0.0a1/Cargo.toml
+-rw-r--r--   0      501       20     3863 2023-07-12 02:21:35.000000 findpython-1.0.0a1/.github/workflows/build.yaml
+-rw-r--r--   0      501       20       92 2023-07-12 02:21:35.000000 findpython-1.0.0a1/.gitignore
+-rw-r--r--   0      501       20    21016 2023-07-12 02:21:35.000000 findpython-1.0.0a1/Cargo.lock
+-rw-r--r--   0      501       20     1075 2023-07-12 02:21:35.000000 findpython-1.0.0a1/LICENSE
+-rw-r--r--   0      501       20     4283 2023-07-12 02:21:35.000000 findpython-1.0.0a1/README.md
+-rw-r--r--   0      501       20     2582 2023-07-12 02:21:35.000000 findpython-1.0.0a1/findpython.pyi
+-rw-r--r--   0      501       20     4121 2023-07-12 02:21:35.000000 findpython-1.0.0a1/pdm.lock
+-rw-r--r--   0      501       20      762 2023-07-12 02:21:35.000000 findpython-1.0.0a1/pyproject.toml
+-rw-r--r--   0      501       20     2746 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/cli.rs
+-rw-r--r--   0      501       20     8712 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/finder.rs
+-rw-r--r--   0      501       20     2326 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/helpers.rs
+-rw-r--r--   0      501       20     1483 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/lib.rs
+-rw-r--r--   0      501       20      130 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/main.rs
+-rw-r--r--   0      501       20     1688 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/providers/asdf.rs
+-rw-r--r--   0      501       20     2297 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/providers/mod.rs
+-rw-r--r--   0      501       20     1110 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/providers/path.rs
+-rw-r--r--   0      501       20     1662 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/providers/pyenv.rs
+-rw-r--r--   0      501       20     1293 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/providers/rye.rs
+-rw-r--r--   0      501       20     3411 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/providers/winreg.rs
+-rw-r--r--   0      501       20    14430 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/python.rs
+-rw-r--r--   0        0        0     4751 1970-01-01 00:00:00.000000 findpython-1.0.0a1/PKG-INFO
```

### Comparing `findpython-1.0.0a0/Cargo.toml` & `findpython-1.0.0a1/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [lib]
 name = "findpython"
 crate-type = ["cdylib", "rlib"]
 
 [package]
 name = "findpython"
-version = "1.0.0-alpha.0"
+version = "1.0.0-alpha.1"
 edition = "2021"
 license = "MIT"
 authors = ["Frost Ming <me@frostming.com>"]
 readme = "README.md"
 repository = "https://github.com/frostming/findpython"
 description = "Find python executables on your system"
 
@@ -24,9 +24,12 @@
 pyo3 = { version = "0.19.0", optional = true, features = ["abi3-py37", "anyhow"] }
 serde = { version = "1.0.167", features = ["derive"] }
 serde_json = "1.0.100"
 shellexpand = "3.1.0"
 wait-timeout = "0.2.0"
 which = "4.4.0"
 
+[target.'cfg(windows)'.dependencies]
+winreg = "0.50"
+
 [features]
 pyo3 = ["dep:pyo3", "pep440_rs/pyo3"]
```

### Comparing `findpython-1.0.0a0/.github/workflows/build.yaml` & `findpython-1.0.0a1/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a0/Cargo.lock` & `findpython-1.0.0a1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
 dependencies = [
  "bit-set",
  "regex",
 ]
 
 [[package]]
 name = "findpython"
-version = "1.0.0-alpha.0"
+version = "1.0.0-alpha.1"
 dependencies = [
  "anyhow",
  "clap",
  "dirs",
  "faccess",
  "fancy-regex",
  "lazy_static",
@@ -241,14 +241,15 @@
  "pep440_rs",
  "pyo3",
  "serde",
  "serde_json",
  "shellexpand",
  "wait-timeout",
  "which",
+ "winreg",
 ]
 
 [[package]]
 name = "getrandom"
 version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
@@ -784,7 +785,17 @@
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
+name = "winreg"
+version = "0.50.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
+dependencies = [
+ "cfg-if",
+ "windows-sys",
+]
```

### Comparing `findpython-1.0.0a0/LICENSE` & `findpython-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a0/findpython.pyi` & `findpython-1.0.0a1/findpython.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -67,7 +67,26 @@
         minor: int | None = None,
         patch: int | None = None,
         pre: bool | None = None,
         dev: bool | None = None,
         name: str | None = None,
         architecture: str | None = None,
     ) -> PythonVersion | None: ...
+
+def find_all(
+    major: str | int | None = None,
+    minor: int | None = None,
+    patch: int | None = None,
+    pre: bool | None = None,
+    dev: bool | None = None,
+    name: str | None = None,
+    architecture: str | None = None,
+) -> list[PythonVersion]: ...
+def find(
+    major: str | int | None = None,
+    minor: int | None = None,
+    patch: int | None = None,
+    pre: bool | None = None,
+    dev: bool | None = None,
+    name: str | None = None,
+    architecture: str | None = None,
+) -> PythonVersion | None: ...
```

### Comparing `findpython-1.0.0a0/pdm.lock` & `findpython-1.0.0a1/pdm.lock`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a0/pyproject.toml` & `findpython-1.0.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a0/src/cli.rs` & `findpython-1.0.0a1/src/cli.rs`

 * *Files 12% similar despite different names*

```diff
@@ -19,52 +19,51 @@
     same_file: bool,
 
     /// Remove duplicate results that wrap the same Python interpreter
     #[arg(long = "no-same-python", action=clap::ArgAction::SetFalse, default_value_t = true)]
     same_python: bool,
 
     /// Select provider names(comma-separated) to use
-    #[arg(long, value_parser = parse_providers)]
-    providers: Option<Vec<String>>,
+    #[arg(long)]
+    providers: Option<String>,
 
     /// The output format
     #[arg(short, long, value_parser = ["default", "json", "path"], default_value = "default")]
     output: String,
 
     /// The version spec to find, e.g. 3|3.8|python3
     version_spec: Option<String>,
 }
 
-fn parse_providers(s: &str) -> Result<Vec<String>, String> {
-    let names = s.split(',').collect::<Vec<_>>();
-    for name in &names {
-        if !crate::providers::ALL_PROVIDERS.contains(&name) {
-            return Err(format!("Provider {} not found", name));
-        }
-    }
-    Ok(names.iter().map(|s| s.to_string()).collect())
-}
-
 pub fn main(cli: Cli) -> anyhow::Result<()> {
     let mut finder = Finder::default()
         .resolve_symlinks(cli.resolve_symlinks)
         .same_file(cli.same_file)
         .same_interpreter(cli.same_python);
 
     if let Some(names) = cli.providers {
-        let v = names.iter().map(|n| n.as_str()).collect::<Vec<_>>();
+        let v = names.split(',').into_iter().map(|n| {
+            if !crate::providers::ALL_PROVIDERS.contains(&n) {
+                Err(anyhow!(format!("Provider {} not found", n)))
+            } else {
+                Ok(n)
+            }
+        }).collect::<Result<Vec<_>, _>>()?;
         finder = finder.select_providers(&v)?;
     }
 
+    let mut options = MatchOptions::default();
+    if let Some(version_spec) = cli.version_spec.as_deref() {
+        options = options.version_spec(version_spec);
+    }
+
     let paths = if cli.all {
-        finder.find_all(cli.version_spec.as_deref(), MatchOptions::default())
+        finder.find_all(options)
     } else {
-        finder
-            .find(cli.version_spec.as_deref(), MatchOptions::default())
-            .map_or(vec![], |v| vec![v])
+        finder.find(options).map_or(vec![], |v| vec![v])
     };
 
     if paths.len() == 0 {
         return Err(anyhow!("No matching Python versions found"));
     }
     eprintln!("Found matching Python versions:");
     match cli.output.as_str() {
```

### Comparing `findpython-1.0.0a0/src/finder.rs` & `findpython-1.0.0a1/src/finder.rs`

 * *Files 4% similar despite different names*

```diff
@@ -62,34 +62,27 @@
     fn find_all_python_versions(&self) -> Vec<PythonVersion> {
         self.providers
             .iter()
             .flat_map(|p| p.find_pythons())
             .collect()
     }
 
-    pub fn find_all(&self, text: Option<&str>, options: MatchOptions) -> Vec<PythonVersion> {
-        let mut options = options;
-        if let Some(s) = text {
-            if let Some(o) = MatchOptions::from_version(s) {
-                options = o.merge(options);
-            }
-        }
-
+    pub fn find_all(&self, options: MatchOptions) -> Vec<PythonVersion> {
         let pythons = self.find_all_python_versions();
         let mut filtered = vec![];
         for python in pythons {
             if python.matches(&options) {
                 filtered.push(python);
             }
         }
         self.deduplicate(filtered)
     }
 
-    pub fn find(&self, text: Option<&str>, options: MatchOptions) -> Option<PythonVersion> {
-        self.find_all(text, options).first().cloned()
+    pub fn find(&self, options: MatchOptions) -> Option<PythonVersion> {
+        self.find_all(options).first().cloned()
     }
 
     fn deduplicate_key(&self, python: &mut PythonVersion) -> String {
         if !self.same_interpreter {
             return python.interpreter().unwrap().to_str().unwrap().to_string();
         }
         if !self.same_file {
@@ -124,15 +117,15 @@
         });
         py_versions
     }
 }
 
 #[cfg(feature = "pyo3")]
 #[derive(FromPyObject)]
-enum StringInt {
+pub enum StringInt {
     STRING(String),
     INT(usize),
 }
 
 #[cfg(feature = "pyo3")]
 #[pymethods]
 impl Finder {
@@ -184,79 +177,58 @@
 
     #[setter]
     fn set_same_interpreter(&mut self, same_interpreter: bool) {
         self.same_interpreter = same_interpreter
     }
 
     #[pyo3(name = "find_all")]
-    fn py_find_all(
+    pub fn py_find_all(
         &self,
         major: Option<StringInt>,
         minor: Option<usize>,
         patch: Option<usize>,
         pre: Option<bool>,
         dev: Option<bool>,
         name: Option<String>,
         architecture: Option<String>,
     ) -> Vec<PythonVersion> {
-        let text = if let Some(StringInt::STRING(s)) = &major {
-            Some(s.as_str())
+        let options = if let Some(StringInt::STRING(s)) = &major {
+            MatchOptions::default().version_spec(s)
         } else {
-            None
-        };
-        self.find_all(
-            text,
             MatchOptions {
                 major: if let Some(StringInt::INT(i)) = major {
                     Some(i)
                 } else {
                     None
                 },
                 minor,
                 patch,
                 pre,
                 dev,
                 name,
                 architecture,
-            },
-        )
+            }
+        };
+        self.find_all(options)
     }
 
     #[pyo3(name = "find")]
-    fn py_find(
+    pub fn py_find(
         &self,
         major: Option<StringInt>,
         minor: Option<usize>,
         patch: Option<usize>,
         pre: Option<bool>,
         dev: Option<bool>,
         name: Option<String>,
         architecture: Option<String>,
     ) -> Option<PythonVersion> {
-        let text = if let Some(StringInt::STRING(s)) = &major {
-            Some(s.as_str())
-        } else {
-            None
-        };
-        self.find(
-            text,
-            MatchOptions {
-                major: if let Some(StringInt::INT(i)) = major {
-                    Some(i)
-                } else {
-                    None
-                },
-                minor,
-                patch,
-                pre,
-                dev,
-                name,
-                architecture,
-            },
-        )
+        self.py_find_all(major, minor, patch, pre, dev, name, architecture)
+            .first()
+            .cloned()
     }
 }
 
 #[derive(Debug, Clone, PartialEq, Eq, Default)]
 pub struct MatchOptions {
     pub major: Option<usize>,
     pub minor: Option<usize>,
@@ -264,15 +236,15 @@
     pub pre: Option<bool>,
     pub dev: Option<bool>,
     pub name: Option<String>,
     pub architecture: Option<String>,
 }
 
 impl MatchOptions {
-    pub fn from_version(version: &str) -> Option<Self> {
+    fn from_version(version: &str) -> Option<Self> {
         match VERSION_REGEX.captures(version) {
             Ok(Some(capture)) => Some(Self {
                 major: capture.name("major").map(|m| m.as_str().parse().unwrap()),
                 minor: capture.name("minor").map(|m| m.as_str().parse().unwrap()),
                 patch: capture.name("patch").map(|m| m.as_str().parse().unwrap()),
                 pre: capture.name("prerel").map(|_| true),
                 dev: capture.name("dev").map(|_| true),
@@ -281,32 +253,63 @@
                     .name("architecture")
                     .map(|m| format!("{}bit", m.as_str())),
             }),
             _ => None,
         }
     }
 
-    pub fn merge(self, other: Self) -> Self {
-        Self {
-            major: other.major.or(self.major),
-            minor: other.minor.or(self.minor),
-            patch: other.patch.or(self.patch),
-            pre: other.pre.or(self.pre),
-            dev: other.dev.or(self.dev),
-            name: other.name.or(self.name),
-            architecture: other.architecture.or(self.architecture),
+    pub fn version_spec(self, version: &str) -> Self {
+        if let Some(res) = Self::from_version(version) {
+            res
+        } else {
+            self.name(version)
         }
     }
+
+    pub fn major(mut self, major: usize) -> Self {
+        self.major = Some(major);
+        self
+    }
+
+    pub fn minor(mut self, minor: usize) -> Self {
+        self.minor = Some(minor);
+        self
+    }
+
+    pub fn patch(mut self, patch: usize) -> Self {
+        self.patch = Some(patch);
+        self
+    }
+
+    pub fn pre(mut self, pre: bool) -> Self {
+        self.pre = Some(pre);
+        self
+    }
+
+    pub fn dev(mut self, dev: bool) -> Self {
+        self.dev = Some(dev);
+        self
+    }
+
+    pub fn name(mut self, name: &str) -> Self {
+        self.name = Some(name.to_string());
+        self
+    }
+
+    pub fn architecture(mut self, architecture: &str) -> Self {
+        self.architecture = Some(architecture.to_string());
+        self
+    }
 }
 
 #[cfg(test)]
 mod test {
     use super::*;
 
     #[test]
     fn test_find_pythons() {
         let finder = Finder::default();
 
-        let pythons = finder.find_all(None, MatchOptions::default());
+        let pythons = finder.find_all(MatchOptions::default());
         assert!(pythons.len() > 0);
     }
 }
```

### Comparing `findpython-1.0.0a0/src/helpers.rs` & `findpython-1.0.0a1/src/helpers.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 use fancy_regex::Regex;
 use lazy_static::lazy_static;
 use std::{ffi::OsStr, io, path::PathBuf};
 
 use faccess::{AccessMode, PathExt};
 
-#[cfg(target_os = "windows")]
+#[cfg(windows)]
 lazy_static! {
     static ref KNOWN_EXECUTABLES: [&'static str; 3] = ["exe", "py", "bat"];
 }
 
-#[cfg(not(target_os = "windows"))]
+#[cfg(not(windows))]
 lazy_static! {
     static ref KNOWN_EXECUTABLES: [&'static str; 6] = ["sh", "bash", "csh", "zsh", "fish", "py"];
 }
 lazy_static! {
     static ref PYTHON_IMPLEMENTATIONS: [&'static str; 10] = [
         "python",
         "ironpython",
```

### Comparing `findpython-1.0.0a0/src/providers/asdf.rs` & `findpython-1.0.0a1/src/providers/asdf.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a0/src/providers/path.rs` & `findpython-1.0.0a1/src/providers/path.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a0/src/providers/pyenv.rs` & `findpython-1.0.0a1/src/providers/pyenv.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a0/src/providers/rye.rs` & `findpython-1.0.0a1/src/providers/rye.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 use std::path::PathBuf;
 
 use super::Provider;
 
 #[derive(Debug, Clone, PartialEq, Eq)]
 pub(super) struct RyeProvider {
-    root: PathBuf
+    root: PathBuf,
 }
 
 impl RyeProvider {
     pub fn new(root: PathBuf) -> Self {
         Self { root }
     }
 }
 
 impl Provider for RyeProvider {
     fn create() -> Option<Self>
-        where
-            Self: Sized {
-        let rye_root = std::env::var_os("RYE_ROOT").or_else(|| {
-            Some(dirs::home_dir()?.join(".rye").into_os_string())
-        })?;
+    where
+        Self: Sized,
+    {
+        let rye_root = std::env::var_os("RYE_ROOT")
+            .or_else(|| Some(dirs::home_dir()?.join(".rye").into_os_string()))?;
         Some(Self::new(rye_root.into()))
     }
 
     fn find_pythons(&self) -> Vec<crate::PythonVersion> {
         let py_root = self.root.join("py");
         match py_root.read_dir() {
             Ok(entries) => entries
```

### Comparing `findpython-1.0.0a0/src/python.rs` & `findpython-1.0.0a1/src/python.rs`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 use std::fmt;
 use std::process::Stdio;
 use std::time::Duration;
 use std::{hash::Hash, io, path::PathBuf, str::FromStr};
 use wait_timeout::ChildExt;
 
 #[cfg(feature = "pyo3")]
-use std::collections::hash_map::DefaultHasher;
-#[cfg(feature = "pyo3")]
-use std::hash::Hasher;
-#[cfg(feature = "pyo3")]
 use pep440_rs::PyVersion;
 use pep440_rs::Version;
 #[cfg(feature = "pyo3")]
 use pyo3::{basic::CompareOp, exceptions::PyNotImplementedError, prelude::*};
+#[cfg(feature = "pyo3")]
+use std::collections::hash_map::DefaultHasher;
+#[cfg(feature = "pyo3")]
+use std::hash::Hasher;
 
 use crate::finder::MatchOptions;
 use crate::helpers::calculate_file_hash;
 
 static GET_VERSION_TIMEOUT: u64 = 5;
 
 fn run_python_script(cmd: &str, script: &str, timeout: Option<u64>) -> Result<String, io::Error> {
@@ -112,16 +112,16 @@
     }
 
     pub fn with_interpreter(mut self, interpreter: PathBuf) -> Self {
         self.interpreter = RefCell::new(Some(interpreter));
         self
     }
 
-    pub fn with_architecture(mut self, architecture: String) -> Self {
-        self.architecture = RefCell::new(Some(architecture));
+    pub fn with_architecture(mut self, architecture: &str) -> Self {
+        self.architecture = RefCell::new(Some(architecture.to_string()));
         self
     }
 
     pub fn with_keep_symlink(mut self, keep_symlink: bool) -> Self {
         self.keep_symlink = keep_symlink;
         self
     }
@@ -299,15 +299,15 @@
         if let Some(interpreter) = interpreter {
             result = result.with_interpreter(interpreter);
         }
         if let Some(version) = version {
             result = result.with_version(version.0);
         }
         if let Some(architecture) = architecture {
-            result = result.with_architecture(architecture);
+            result = result.with_architecture(architecture.as_str());
         }
         result
     }
 
     #[getter]
     fn executable(&self, py: Python<'_>) -> PyResult<PyObject> {
         Ok(py
```

### Comparing `findpython-1.0.0a0/PKG-INFO` & `findpython-1.0.0a1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: findpython
-Version: 1.0.0a0
-Requires-Dist: pep440-rs >=0.3.11 ; extra == 'types'
-Provides-Extra: types
-License-File: LICENSE
-Summary: A utility to find python versions on your system
-Author: Frost Ming <me@frostming.com>
-Author-email: Frost Ming <mianghong@gmail.com>
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Source Code, https://github.com/frostming/findpython
-
 # FindPython
 
 _A utility to find python versions on your system._
 
 [![Tests](https://github.com/frostming/findpython/actions/workflows/ci.yml/badge.svg)](https://github.com/frostming/findpython/actions/workflows/ci.yml)
 [![PyPI](https://img.shields.io/pypi/v/findpython?logo=python&logoColor=%23cccccc&style=flat-square)](https://pypi.org/project/findpython)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/findpython?logo=python&logoColor=%23cccccc&style=flat-square)](https://pypi.org/project/findpython)
@@ -60,37 +46,38 @@
 </details>
 
 ## Python Usage
 
 ```python
 >>> import findpython
 >>> findpython.find(3, 9)  # Find by major and minor version
-<PythonVersion executable=PosixPath('/opt/homebrew/bin/python3.9'), version=<Version('3.9.10')>, architecture='64bit', major=3, minor=9, patch=10>
+<PythonVersion executable=/opt/homebrew/bin/python3.9, version=3.9.17, arch=64bit>
 >>> findpython.find("3.9")  # Find by version string
-<PythonVersion executable=PosixPath('/opt/homebrew/bin/python3.9'), version=<Version('3.9.10')>, architecture='64bit', major=3, minor=9, patch=10>
+<PythonVersion executable=/opt/homebrew/bin/python3.9, version=3.9.17, arch=64bit>
 >>> findpython.find("3.9-32")  # Find by version string and architecture
-<PythonVersion executable=WindowsPath('C:\\Python\\3.9-32\\python.exe'), version=<Version('3.9.10')>, architecture='32bit', major=3, minor=9, patch=10>
+<PythonVersion executable=C:/Python/3.9-32/python.exe, version=3.9.10, arch=32bit>
 >>> findpython.find(name="python3")  # Find by executable name
-<PythonVersion executable=PosixPath('/Users/fming/Library/PythonUp/bin/python3'), version=<Version('3.10.2')>, architecture='64bit', major=3, minor=10, patch=2>
+<PythonVersion executable=/Users/fming/wkspace/github/findpython/.venv/bin/python3, version=3.11.4, arch=64bit>
 >>> findpython.find("python3")  # Find by executable name without keyword argument, same as above
-<PythonVersion executable=PosixPath('/Users/fming/Library/PythonUp/bin/python3'), version=<Version('3.10.2')>, architecture='64bit', major=3, minor=10, patch=2>
+<PythonVersion executable=/Users/fming/wkspace/github/findpython/.venv/bin/python3, version=3.11.4, arch=64bit>
 >>> findpython.find_all(major=3, minor=9)  # Same arguments as `find()`, but return all matches
-[<PythonVersion executable=PosixPath('/opt/homebrew/bin/python3.9'), version=<Version('3.9.10')>, architecture='64bit', major=3, minor=9, patch=10>, <PythonVersion executable=PosixPath('/opt/homebrew/bin/python3'), version=<Version('3.9.10')>, architecture='64bit', major=3, minor=9, patch=10>, <PythonVersion executable=PosixPath('/Users/fming/Library/PythonUp/cmd/python3.9'), version=<Version('3.9.9')>, architecture='64bit', major=3, minor=9, patch=9>, <PythonVersion executable=PosixPath('/usr/local/bin/python3.9'), version=<Version('3.9.5')>, architecture='64bit', major=3, minor=9, patch=5>, <PythonVersion executable=PosixPath('/usr/local/bin/python3'), version=<Version('3.9.5')>, architecture='64bit', major=3, minor=9, patch=5>]
+[<PythonVersion executable=/opt/homebrew/bin/python3.9, version=3.9.17, arch=64bit>,
+ <PythonVersion executable=/usr/bin/python3, version=3.9.6, arch=64bit>]
 ```
 
 ## Rust Usage
 
 ```rust
-use findpython::Finder;
+use findpython::{Finder, MatchOptions};
 
 fn main() {
     let finder = Finder::default();
 
     // Find by major and minor version
-    let py = finder.find(3, 9).unwrap();
+    let py = finder.find(MatchOptions::default().major(3).minor(10)).unwrap();
     println!("{:?}", py);
     // Find all matches
     let all_pythons = finder.find_all();
     println!("{:?}", all_pythons);
 }
 ```
 
@@ -120,17 +107,16 @@
 ## Integration
 
 FindPython finds Python from the following places:
 
 -   `PATH` environment variable
 -   pyenv
 -   asdf
--   winreg (Windows) (🚧 WIP 🚧)
+-   winreg (Windows only)
 -   [Rye] project manager backed by [python-build-standalone]
 
 [rye]: https://rye-up.com
 [python-build-standalone]: https://github.com/indygreg/python-build-standalone
 
 ## License
 
 FindPython is released under MIT License.
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,17 +1,11 @@
-Metadata-Version: 2.1 Name: findpython Version: 1.0.0a0 Requires-Dist: pep440-
-rs >=0.3.11 ; extra == 'types' Provides-Extra: types License-File: LICENSE
-Summary: A utility to find python versions on your system Author: Frost Ming
-frostming.com> Author-email: Frost Ming
-gmail.com> License: MIT Requires-Python: >=3.7 Description-Content-Type: text/
-markdown; charset=UTF-8; variant=GFM Project-URL: Source Code, https://
-github.com/frostming/findpython # FindPython _A utility to find python versions
-on your system._ [![Tests](https://github.com/frostming/findpython/actions/
-workflows/ci.yml/badge.svg)](https://github.com/frostming/findpython/actions/
-workflows/ci.yml) [![PyPI](https://img.shields.io/pypi/v/
+# FindPython _A utility to find python versions on your system._ [![Tests]
+(https://github.com/frostming/findpython/actions/workflows/ci.yml/badge.svg)]
+(https://github.com/frostming/findpython/actions/workflows/ci.yml) [![PyPI]
+(https://img.shields.io/pypi/v/
 findpython?logo=python&logoColor=%23cccccc&style=flat-square)](https://
 pypi.org/project/findpython) [![PyPI - Python Version](https://img.shields.io/
 pypi/pyversions/findpython?logo=python&logoColor=%23cccccc&style=flat-square)]
 (https://pypi.org/project/findpython) [![pdm-managed](https://img.shields.io/
 badge/pdm-managed-blueviolet?style=flat-square)](https://github.com/frostming/
 findpython) ## Description This library is a rewrite of [pythonfinder] project
 by [@techalchemy][techalchemy]. It simplifies the whole code structure while
@@ -19,38 +13,32 @@
 sarugaku/pythonfinder [techalchemy]: https://github.com/techalchemy ##
 Installation FindPython can be used in both Python and Rust projects. To
 install FindPython in Python: ```bash pip install findpython ``` To install
 FindPython in Rust: ```bash cargo install findpyhton ``` Or use FindPython
 library in a Rust project: ```bash cargo add findpython ```  Expand this
 section to see findpython's availability in the package ecosystem [Packaging
 status]  ## Python Usage ```python >>> import findpython >>> findpython.find(3,
-9) # Find by major and minor version , architecture='64bit', major=3, minor=9,
-patch=10> >>> findpython.find("3.9") # Find by version string ,
-architecture='64bit', major=3, minor=9, patch=10> >>> findpython.find("3.9-32")
-# Find by version string and architecture , architecture='32bit', major=3,
-minor=9, patch=10> >>> findpython.find(name="python3") # Find by executable
-name , architecture='64bit', major=3, minor=10, patch=2> >>> findpython.find
-("python3") # Find by executable name without keyword argument, same as above ,
-architecture='64bit', major=3, minor=10, patch=2> >>> findpython.find_all
-(major=3, minor=9) # Same arguments as `find()`, but return all matches [,
-architecture='64bit', major=3, minor=9, patch=10>, , architecture='64bit',
-major=3, minor=9, patch=10>, , architecture='64bit', major=3, minor=9,
-patch=9>, , architecture='64bit', major=3, minor=9, patch=5>, ,
-architecture='64bit', major=3, minor=9, patch=5>] ``` ## Rust Usage ```rust use
-findpython::Finder; fn main() { let finder = Finder::default(); // Find by
-major and minor version let py = finder.find(3, 9).unwrap(); println!("{:?}",
-py); // Find all matches let all_pythons = finder.find_all(); println!("{:?}",
+9) # Find by major and minor version  >>> findpython.find("3.9") # Find by
+version string  >>> findpython.find("3.9-32") # Find by version string and
+architecture  >>> findpython.find(name="python3") # Find by executable name
+>>> findpython.find("python3") # Find by executable name without keyword
+argument, same as above  >>> findpython.find_all(major=3, minor=9) # Same
+arguments as `find()`, but return all matches [, ] ``` ## Rust Usage ```rust
+use findpython::{Finder, MatchOptions}; fn main() { let finder = Finder::
+default(); // Find by major and minor version let py = finder.find
+(MatchOptions::default().major(3).minor(10)).unwrap(); println!("{:?}", py); /
+/ Find all matches let all_pythons = finder.find_all(); println!("{:?}",
 all_pythons); } ``` ## CLI Usage In addition, FindPython provides a CLI
 interface to find python versions: ``` Find python executables on your system
 Usage: findpython [OPTIONS] [VERSION_SPEC] Arguments: [VERSION_SPEC] The
 version spec to find, e.g. 3|3.8|python3 Options: -a, --all Return all matching
 Python versions --resolve-symlinks Resolve symlinks and remove duplicate
 results --no-same-file Remove duplicate results that are the same binary --no-
 same-python Remove duplicate results that wrap the same Python interpreter --
 providers  Select provider names(comma-separated) to use -o, --output  The
 output format [default: default] [possible values: default, json, path] -h, --
 help Print help -V, --version Print version ``` ## Integration FindPython finds
 Python from the following places: - `PATH` environment variable - pyenv - asdf
-- winreg (Windows) (ð§ WIP ð§) - [Rye] project manager backed by [python-
-build-standalone] [rye]: https://rye-up.com [python-build-standalone]: https://
+- winreg (Windows only) - [Rye] project manager backed by [python-build-
+standalone] [rye]: https://rye-up.com [python-build-standalone]: https://
 github.com/indygreg/python-build-standalone ## License FindPython is released
 under MIT License.
```


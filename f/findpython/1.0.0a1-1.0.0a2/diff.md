# Comparing `tmp/findpython-1.0.0a1.tar.gz` & `tmp/findpython-1.0.0a2.tar.gz`

## Comparing `findpython-1.0.0a1.tar` & `findpython-1.0.0a2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 findpython-1.0.0a1/Cargo.toml
--rw-r--r--   0      501       20     3863 2023-07-12 02:21:35.000000 findpython-1.0.0a1/.github/workflows/build.yaml
--rw-r--r--   0      501       20       92 2023-07-12 02:21:35.000000 findpython-1.0.0a1/.gitignore
--rw-r--r--   0      501       20    21016 2023-07-12 02:21:35.000000 findpython-1.0.0a1/Cargo.lock
--rw-r--r--   0      501       20     1075 2023-07-12 02:21:35.000000 findpython-1.0.0a1/LICENSE
--rw-r--r--   0      501       20     4283 2023-07-12 02:21:35.000000 findpython-1.0.0a1/README.md
--rw-r--r--   0      501       20     2582 2023-07-12 02:21:35.000000 findpython-1.0.0a1/findpython.pyi
--rw-r--r--   0      501       20     4121 2023-07-12 02:21:35.000000 findpython-1.0.0a1/pdm.lock
--rw-r--r--   0      501       20      762 2023-07-12 02:21:35.000000 findpython-1.0.0a1/pyproject.toml
--rw-r--r--   0      501       20     2746 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/cli.rs
--rw-r--r--   0      501       20     8712 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/finder.rs
--rw-r--r--   0      501       20     2326 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/helpers.rs
--rw-r--r--   0      501       20     1483 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/lib.rs
--rw-r--r--   0      501       20      130 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/main.rs
--rw-r--r--   0      501       20     1688 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/providers/asdf.rs
--rw-r--r--   0      501       20     2297 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/providers/mod.rs
--rw-r--r--   0      501       20     1110 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/providers/path.rs
--rw-r--r--   0      501       20     1662 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/providers/pyenv.rs
--rw-r--r--   0      501       20     1293 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/providers/rye.rs
--rw-r--r--   0      501       20     3411 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/providers/winreg.rs
--rw-r--r--   0      501       20    14430 2023-07-12 02:21:35.000000 findpython-1.0.0a1/src/python.rs
--rw-r--r--   0        0        0     4751 1970-01-01 00:00:00.000000 findpython-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 findpython-1.0.0a2/Cargo.toml
+-rw-r--r--   0      501       20     3863 2023-07-12 05:46:09.000000 findpython-1.0.0a2/.github/workflows/build.yaml
+-rw-r--r--   0      501       20      124 2023-07-12 05:46:09.000000 findpython-1.0.0a2/.gitignore
+-rw-r--r--   0      501       20    21016 2023-07-12 05:46:09.000000 findpython-1.0.0a2/Cargo.lock
+-rw-r--r--   0      501       20     1075 2023-07-12 05:46:09.000000 findpython-1.0.0a2/LICENSE
+-rw-r--r--   0      501       20     4283 2023-07-12 05:46:09.000000 findpython-1.0.0a2/README.md
+-rw-r--r--   0      501       20      258 2023-07-12 05:46:09.000000 findpython-1.0.0a2/pdm.lock
+-rw-r--r--   0      501       20      717 2023-07-12 05:46:09.000000 findpython-1.0.0a2/pyproject.toml
+-rw-r--r--   0      501       20      297 2023-07-12 05:46:09.000000 findpython-1.0.0a2/python/findpython/__init__.py
+-rw-r--r--   0      501       20     3479 2023-07-12 05:46:09.000000 findpython-1.0.0a2/python/findpython/__init__.pyi
+-rw-r--r--   0      501       20     2822 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/cli.rs
+-rw-r--r--   0      501       20     9097 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/finder.rs
+-rw-r--r--   0      501       20     2326 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/helpers.rs
+-rw-r--r--   0      501       20     1934 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/lib.rs
+-rw-r--r--   0      501       20      130 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/main.rs
+-rw-r--r--   0      501       20     1690 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/providers/asdf.rs
+-rw-r--r--   0      501       20     2222 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/providers/mod.rs
+-rw-r--r--   0      501       20     1112 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/providers/path.rs
+-rw-r--r--   0      501       20     1664 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/providers/pyenv.rs
+-rw-r--r--   0      501       20      628 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/providers/pyobject.rs
+-rw-r--r--   0      501       20     1293 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/providers/rye.rs
+-rw-r--r--   0      501       20     3729 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/providers/winreg.rs
+-rw-r--r--   0      501       20    14430 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/python.rs
+-rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 findpython-1.0.0a2/PKG-INFO
```

### Comparing `findpython-1.0.0a1/Cargo.toml` & `findpython-1.0.0a2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [lib]
 name = "findpython"
 crate-type = ["cdylib", "rlib"]
 
 [package]
 name = "findpython"
-version = "1.0.0-alpha.1"
+version = "1.0.0-alpha.2"
 edition = "2021"
 license = "MIT"
 authors = ["Frost Ming <me@frostming.com>"]
 readme = "README.md"
 repository = "https://github.com/frostming/findpython"
 description = "Find python executables on your system"
```

### Comparing `findpython-1.0.0a1/.github/workflows/build.yaml` & `findpython-1.0.0a2/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a1/Cargo.lock` & `findpython-1.0.0a2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
 dependencies = [
  "bit-set",
  "regex",
 ]
 
 [[package]]
 name = "findpython"
-version = "1.0.0-alpha.1"
+version = "1.0.0-alpha.2"
 dependencies = [
  "anyhow",
  "clap",
  "dirs",
  "faccess",
  "fancy-regex",
  "lazy_static",
```

### Comparing `findpython-1.0.0a1/LICENSE` & `findpython-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a1/README.md` & `findpython-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a1/src/cli.rs` & `findpython-1.0.0a2/src/cli.rs`

 * *Files 3% similar despite different names*

```diff
@@ -37,21 +37,25 @@
 pub fn main(cli: Cli) -> anyhow::Result<()> {
     let mut finder = Finder::default()
         .resolve_symlinks(cli.resolve_symlinks)
         .same_file(cli.same_file)
         .same_interpreter(cli.same_python);
 
     if let Some(names) = cli.providers {
-        let v = names.split(',').into_iter().map(|n| {
-            if !crate::providers::ALL_PROVIDERS.contains(&n) {
-                Err(anyhow!(format!("Provider {} not found", n)))
-            } else {
-                Ok(n)
-            }
-        }).collect::<Result<Vec<_>, _>>()?;
+        let v = names
+            .split(',')
+            .into_iter()
+            .map(|n| {
+                if !crate::providers::ALL_PROVIDERS.contains(&n) {
+                    Err(anyhow!(format!("Provider {} not found", n)))
+                } else {
+                    Ok(n)
+                }
+            })
+            .collect::<Result<Vec<_>, _>>()?;
         finder = finder.select_providers(&v)?;
     }
 
     let mut options = MatchOptions::default();
     if let Some(version_spec) = cli.version_spec.as_deref() {
         options = options.version_spec(version_spec);
     }
```

### Comparing `findpython-1.0.0a1/src/finder.rs` & `findpython-1.0.0a2/src/finder.rs`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 use crate::{helpers::suffix_preference, providers::*, PythonVersion};
 use fancy_regex::Regex;
 use lazy_static::lazy_static;
 
 #[cfg(feature = "pyo3")]
 use pyo3::prelude::*;
 
+#[cfg(feature = "pyo3")]
+use crate::providers::pyobject::PyObjectProvider;
+
 lazy_static! {
     static ref VERSION_REGEX: Regex = Regex::new(
         r#"(?x)
         ^(?P<major>\d+)(?:\.(?P<minor>\d+)(?:\.(?P<patch>[0-9]+))?)?\.?
         (?:(?P<prerel>[abc]|rc|dev)(?:(?P<prerelversion>\d+(?:\.\d+)*))?)
         ?(?P<postdev>(\.post(?P<post>\d+))?(\.dev(?P<dev>\d+))?)?
         (?:-(?P<architecture>32|64))?"#
@@ -146,14 +149,23 @@
         if let Some(names) = selected_providers {
             let names: Vec<&str> = names.iter().map(|v| v.as_str()).collect();
             f = f.select_providers(names.as_slice())?
         }
         Ok(f)
     }
 
+    fn add_provider(&mut self, provider: PyObject, pos: Option<usize>) {
+        let provider = PyObjectProvider::new(provider);
+        if let Some(pos) = pos {
+            self.providers.insert(pos, Box::new(provider));
+        } else {
+            self.providers.push(Box::new(provider));
+        }
+    }
+
     #[getter]
     fn get_resolve_symlinks(&self) -> bool {
         self.resolve_symlinks
     }
 
     #[setter]
     fn set_resolve_symlinks(&mut self, resolve_symlinks: bool) {
```

### Comparing `findpython-1.0.0a1/src/helpers.rs` & `findpython-1.0.0a2/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a1/src/providers/asdf.rs` & `findpython-1.0.0a2/src/providers/asdf.rs`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         match versions_path.read_dir() {
             Ok(entries) => entries
                 .into_iter()
                 .flat_map(|entry| match entry {
                     Ok(entry) if entry.path().is_dir() => {
                         let path = entry.path().join("bin");
                         if path.is_dir() {
-                            self.find_pythons_from_path(&path, true)
+                            super::find_pythons_from_path(&path, true)
                         } else {
                             vec![]
                         }
                     }
                     _ => vec![],
                 })
                 .collect(),
```

### Comparing `findpython-1.0.0a1/src/providers/mod.rs` & `findpython-1.0.0a2/src/providers/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 use lazy_static::lazy_static;
 
 mod asdf;
 mod path;
 mod pyenv;
 mod rye;
 
+#[cfg(feature = "pyo3")]
+pub mod pyobject;
+
 #[cfg(windows)]
 mod winreg;
 
 #[cfg(windows)]
 lazy_static! {
     pub static ref ALL_PROVIDERS: [&'static str; 4] = ["path", "pyenv", "rye", "winreg"];
 }
@@ -24,50 +27,50 @@
 
 pub trait Provider: Send + Sync {
     fn create() -> Option<Self>
     where
         Self: Sized;
 
     fn find_pythons(&self) -> Vec<PythonVersion>;
-
-    /// Find all Python versions under the given path.
-    /// ### Arguments:
-    ///
-    /// path: The path to search for Python versions under.
-    /// as_interpreter: Whether to use the path as an interpreter.
-    ///     Must not be true if it might be a wrapper script.
-    ///
-    /// ### Returns:
-    /// A list of Python versions found under the given path.
-    fn find_pythons_from_path(&self, path: &PathBuf, as_interpreter: bool) -> Vec<PythonVersion> {
-        match path.read_dir() {
-            Ok(entries) => entries
-                .into_iter()
-                .filter_map(|entry| {
-                    let path = entry.ok()?.path();
-                    if helpers::path_is_python(&path) {
-                        let mut python = PythonVersion::new(path.to_owned());
-                        if as_interpreter {
-                            python = python.with_interpreter(path.to_owned());
-                        }
-                        Some(python)
-                    } else {
-                        None
-                    }
-                })
-                .collect(),
-            Err(_) => vec![],
-        }
-    }
 }
 
 pub fn get_provider(name: &str) -> Option<Box<dyn Provider>> {
     match name {
         "path" => path::PathProvider::create().map(|p| Box::new(p) as Box<dyn Provider>),
         "pyenv" => pyenv::PyenvProvider::create().map(|p| Box::new(p) as Box<dyn Provider>),
         "rye" => rye::RyeProvider::create().map(|p| Box::new(p) as Box<dyn Provider>),
         "asdf" => asdf::AsdfProvider::create().map(|p| Box::new(p) as Box<dyn Provider>),
         #[cfg(windows)]
         "winreg" => winreg::WinRegProvider::create().map(|p| Box::new(p) as Box<dyn Provider>),
         _ => None,
     }
 }
+
+/// Find all Python versions under the given path.
+/// ### Arguments:
+///
+/// path: The path to search for Python versions under.
+/// as_interpreter: Whether to use the path as an interpreter.
+///     Must not be true if it might be a wrapper script.
+///
+/// ### Returns:
+/// A list of Python versions found under the given path.
+pub fn find_pythons_from_path(path: &PathBuf, as_interpreter: bool) -> Vec<PythonVersion> {
+    match path.read_dir() {
+        Ok(entries) => entries
+            .into_iter()
+            .filter_map(|entry| {
+                let path = entry.ok()?.path();
+                if helpers::path_is_python(&path) {
+                    let mut python = PythonVersion::new(path.to_owned());
+                    if as_interpreter {
+                        python = python.with_interpreter(path.to_owned());
+                    }
+                    Some(python)
+                } else {
+                    None
+                }
+            })
+            .collect(),
+        Err(_) => vec![],
+    }
+}
```

### Comparing `findpython-1.0.0a1/src/providers/path.rs` & `findpython-1.0.0a2/src/providers/path.rs`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     fn create() -> Option<Self> {
         Some(Self::new())
     }
 
     fn find_pythons(&self) -> Vec<PythonVersion> {
         self.paths
             .iter()
-            .flat_map(|path| self.find_pythons_from_path(path, false))
+            .flat_map(|path| super::find_pythons_from_path(path, false))
             .collect()
     }
 }
 
 #[cfg(test)]
 mod test {
     use super::*;
```

### Comparing `findpython-1.0.0a1/src/providers/pyenv.rs` & `findpython-1.0.0a2/src/providers/pyenv.rs`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         match versions_path.read_dir() {
             Ok(entries) => entries
                 .into_iter()
                 .flat_map(|entry| match entry {
                     Ok(entry) => {
                         let path = entry.path();
                         if path.is_dir() {
-                            self.find_pythons_from_path(&path.join("bin"), true)
+                            super::find_pythons_from_path(&path.join("bin"), true)
                         } else {
                             vec![]
                         }
                     }
                     Err(_) => vec![],
                 })
                 .collect(),
```

### Comparing `findpython-1.0.0a1/src/providers/rye.rs` & `findpython-1.0.0a2/src/providers/rye.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a1/src/providers/winreg.rs` & `findpython-1.0.0a2/src/providers/winreg.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+use pep440_rs::Version;
 use std::io::Result;
 use std::str::FromStr;
-use pep440_rs::Version;
 use winreg::enums::*;
 use winreg::RegKey;
 use winreg::HKEY;
 
 use crate::PythonVersion;
 
 use super::Provider;
@@ -13,24 +13,28 @@
 
 struct PythonRegSource {
     key: HKEY,
     flags: u32,
     arch: Option<&'static str>,
 }
 
-
 impl PythonRegSource {
     fn get_python(&self, reg: &RegKey) -> Result<PythonVersion> {
         let version = if let Ok(ver) = reg.get_value::<String, _>("Version") {
             Version::from_str(ver.as_str()).ok()
         } else {
             None
         };
-        let install_path: String = reg.open_subkey_with_flags("InstallPath", KEY_READ | self.flags)?.get_value("ExecutablePath")?;
-        let arch = reg.get_value::<String, _>("SysArchitecture").ok().or_else(|| self.arch.map(|a| a.to_string()));
+        let install_path: String = reg
+            .open_subkey_with_flags("InstallPath", KEY_READ | self.flags)?
+            .get_value("ExecutablePath")?;
+        let arch = reg
+            .get_value::<String, _>("SysArchitecture")
+            .ok()
+            .or_else(|| self.arch.map(|a| a.to_string()));
         let mut py = PythonVersion::new(install_path.into());
         if let Some(arch) = arch {
             py = py.with_architecture(arch.as_str());
         }
 
         if let Some(version) = version {
             Ok(py.with_version(version))
@@ -38,25 +42,32 @@
             Ok(py)
         }
     }
 
     fn find_all(&self) -> Vec<PythonVersion> {
         let hklm = RegKey::predef(self.key);
         let subkey = hklm.open_subkey_with_flags(PYTHON_PATH, KEY_READ | self.flags);
-        
+
         if let Ok(key) = subkey {
             let companies = key.enum_keys().filter_map(|company| {
-                key.open_subkey_with_flags(company.ok()?, KEY_READ | self.flags).ok()
+                key.open_subkey_with_flags(company.ok()?, KEY_READ | self.flags)
+                    .ok()
             });
-            companies.flat_map(|k| {
-                k.enum_keys().filter_map(|tag| {
-                    let py = tag.and_then(|t| k.open_subkey_with_flags(t, KEY_READ | self.flags)).ok()?;
-                    self.get_python(&py).ok()
-                }).collect::<Vec<_>>()
-            }).collect::<Vec<_>>()
+            companies
+                .flat_map(|k| {
+                    k.enum_keys()
+                        .filter_map(|tag| {
+                            let py = tag
+                                .and_then(|t| k.open_subkey_with_flags(t, KEY_READ | self.flags))
+                                .ok()?;
+                            self.get_python(&py).ok()
+                        })
+                        .collect::<Vec<_>>()
+                })
+                .collect::<Vec<_>>()
         } else {
             vec![]
         }
     }
 }
 
 fn get_sources() -> Vec<PythonRegSource> {
@@ -91,33 +102,39 @@
                 arch: Some("32bit"),
             },
         ]
     }
 }
 
 pub struct WinRegProvider {
-    sources: Vec<PythonRegSource>
+    sources: Vec<PythonRegSource>,
 }
 
 impl Provider for WinRegProvider {
     fn create() -> Option<Self>
-        where
-            Self: Sized {
-        Some(Self { sources: get_sources() })
+    where
+        Self: Sized,
+    {
+        Some(Self {
+            sources: get_sources(),
+        })
     }
 
     fn find_pythons(&self) -> Vec<PythonVersion> {
-        self.sources.iter().flat_map(|s| s.find_all()).collect::<Vec<_>>()
+        self.sources
+            .iter()
+            .flat_map(|s| s.find_all())
+            .collect::<Vec<_>>()
     }
 }
 
 #[cfg(test)]
 mod test {
     use super::*;
 
     #[test]
     fn test_find_python() {
         let provider = WinRegProvider::create().unwrap();
         let pythons = provider.find_pythons();
         assert!(pythons.len() > 0);
     }
-}
+}
```

### Comparing `findpython-1.0.0a1/src/python.rs` & `findpython-1.0.0a2/src/python.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a1/PKG-INFO` & `findpython-1.0.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 Metadata-Version: 2.1
 Name: findpython
-Version: 1.0.0a1
-Requires-Dist: pep440-rs >=0.3.11 ; extra == 'types'
-Provides-Extra: types
+Version: 1.0.0a2
 License-File: LICENSE
 Summary: A utility to find python versions on your system
 Author: Frost Ming <me@frostming.com>
 Author-email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
-Metadata-Version: 2.1 Name: findpython Version: 1.0.0a1 Requires-Dist: pep440-
-rs >=0.3.11 ; extra == 'types' Provides-Extra: types License-File: LICENSE
+Metadata-Version: 2.1 Name: findpython Version: 1.0.0a2 License-File: LICENSE
 Summary: A utility to find python versions on your system Author: Frost Ming
 frostming.com> Author-email: Frost Ming
 gmail.com> License: MIT Requires-Python: >=3.7 Description-Content-Type: text/
 markdown; charset=UTF-8; variant=GFM Project-URL: Source Code, https://
 github.com/frostming/findpython # FindPython _A utility to find python versions
 on your system._ [![Tests](https://github.com/frostming/findpython/actions/
 workflows/ci.yml/badge.svg)](https://github.com/frostming/findpython/actions/
```


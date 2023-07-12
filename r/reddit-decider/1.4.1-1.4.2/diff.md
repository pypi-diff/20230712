# Comparing `tmp/reddit_decider-1.4.1.tar.gz` & `tmp/reddit_decider-1.4.2.tar.gz`

## Comparing `reddit_decider-1.4.1.tar` & `reddit_decider-1.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 reddit_decider-1.4.1/local_dependencies/decider/Cargo.toml
--rw-r--r--   0        0        0       19 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/local_dependencies/decider/.gitignore
--rw-r--r--   0        0        0      323 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/local_dependencies/decider/Makefile
--rw-r--r--   0        0        0      710 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/local_dependencies/decider/README.md
--rw-r--r--   0        0        0     6097 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/local_dependencies/decider/benches/decider.rs
--rw-r--r--   0        0        0     9514 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/local_dependencies/decider/src/context.rs
--rw-r--r--   0        0        0    48184 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/local_dependencies/decider/src/events.rs
--rw-r--r--   0        0        0   111863 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/local_dependencies/decider/src/lib.rs
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 reddit_decider-1.4.1/Cargo.toml
--rw-r--r--   0        0        0      112 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/.gitignore
--rw-r--r--   0        0        0      786 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/Makefile
--rw-r--r--   0        0        0     6041 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/README.md
--rw-r--r--   0        0        0      273 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/pyproject.toml
--rw-r--r--   0        0        0    22412 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/python/rust_decider/__init__.py
--rw-r--r--   0        0        0      259 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/python/rust_decider/prometheus_metrics.py
--rw-r--r--   0        0        0      177 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/requirements-dev.txt
--rw-r--r--   0        0        0       40 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/setup.cfg
--rw-r--r--   0        0        0     1300 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/setup.py
--rw-r--r--   0        0        0    34812 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/src/lib.rs
--rw-r--r--   0        0        0    42128 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/test/decider_unit_test.py
--rw-r--r--   0        0        0    10110 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/test/integration_test.py
--rw-r--r--   0        0        0     2903 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/test/test_rust.py
--rw-r--r--   0        0        0    34128 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/test/unit_test.py
--rw-r--r--   0        0        0     3088 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/test/utils.py
--rw-r--r--   0        0        0     6238 1970-01-01 00:00:00.000000 reddit_decider-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 reddit_decider-1.4.2/local_dependencies/decider/Cargo.toml
+-rw-r--r--   0        0        0       19 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/local_dependencies/decider/.gitignore
+-rw-r--r--   0        0        0      323 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/local_dependencies/decider/Makefile
+-rw-r--r--   0        0        0      710 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/local_dependencies/decider/README.md
+-rw-r--r--   0        0        0     6097 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/local_dependencies/decider/benches/decider.rs
+-rw-r--r--   0        0        0     9514 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/local_dependencies/decider/src/context.rs
+-rw-r--r--   0        0        0    48184 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/local_dependencies/decider/src/events.rs
+-rw-r--r--   0        0        0   111870 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/local_dependencies/decider/src/lib.rs
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 reddit_decider-1.4.2/Cargo.toml
+-rw-r--r--   0        0        0      112 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/.gitignore
+-rw-r--r--   0        0        0      786 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/Makefile
+-rw-r--r--   0        0        0     6041 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/README.md
+-rw-r--r--   0        0        0      273 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0    22412 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/python/rust_decider/__init__.py
+-rw-r--r--   0        0        0      259 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/python/rust_decider/prometheus_metrics.py
+-rw-r--r--   0        0        0      177 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/requirements-dev.txt
+-rw-r--r--   0        0        0       40 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/setup.cfg
+-rw-r--r--   0        0        0     1300 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/setup.py
+-rw-r--r--   0        0        0    34812 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/src/lib.rs
+-rw-r--r--   0        0        0    42128 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/test/decider_unit_test.py
+-rw-r--r--   0        0        0    10110 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/test/integration_test.py
+-rw-r--r--   0        0        0     2903 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/test/test_rust.py
+-rw-r--r--   0        0        0    34128 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/test/unit_test.py
+-rw-r--r--   0        0        0     3088 2023-07-12 16:53:57.000000 reddit_decider-1.4.2/test/utils.py
+-rw-r--r--   0        0        0     6238 1970-01-01 00:00:00.000000 reddit_decider-1.4.2/PKG-INFO
```

### Comparing `reddit_decider-1.4.1/local_dependencies/decider/Cargo.toml` & `reddit_decider-1.4.2/local_dependencies/decider/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "decider"
-version = "1.4.1"
+version = "1.4.2"
 edition = "2021"
 description = "a package for AB-testing and dynamic config"
 homepage = "https://mattknox.com"
 license = "MIT"
 documentation = "https://mattknox.com/decider"
 readme = "README.md"
```

### Comparing `reddit_decider-1.4.1/local_dependencies/decider/README.md` & `reddit_decider-1.4.2/local_dependencies/decider/README.md`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.1/local_dependencies/decider/benches/decider.rs` & `reddit_decider-1.4.2/local_dependencies/decider/benches/decider.rs`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.1/local_dependencies/decider/src/context.rs` & `reddit_decider-1.4.2/local_dependencies/decider/src/context.rs`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.1/local_dependencies/decider/src/events.rs` & `reddit_decider-1.4.2/local_dependencies/decider/src/events.rs`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.1/local_dependencies/decider/src/lib.rs` & `reddit_decider-1.4.2/local_dependencies/decider/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -75,32 +75,31 @@
 
 #[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct Metadata {
     pub id: u32,
     pub name: String,
     pub version: u32,
     pub owner: String,
+    pub enabled: bool,
 }
 
 #[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct DynamicConfig {
     metadata: Metadata,
-    enabled: bool,
     value: Value,
     value_type: ValueType,
 }
 
 /// RangeVariant represent a unit of controllable code, that we might want to turn off, make
 /// available only to some users, etc..  This is what FeatureFlags/AB tests control.
 #[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct RangeVariant {
-    metadata: Metadata,
+    pub metadata: Metadata,
     pub emit_event: bool,
     pub variant_set: VariantSet,
-    enabled: bool,
     targeting: Option<TargetingTree>,
     overrides: Option<Vec<HashMap<String, TargetingTree>>>,
 }
 
 #[derive(Serialize, Deserialize, Debug, Clone)]
 pub enum Feature {
     RangeVariant(RangeVariant),
@@ -428,25 +427,25 @@
 
 impl From<&Feature> for LegacyExperiment {
     fn from(f: &Feature) -> Self {
         let (feature_type, enabled, emit_event, value, value_type, targeting, overrides, variant_set) =
             match f {
                 Feature::RangeVariant(rv) => (
                     ExperimentType::RangeVariant,
-                    rv.enabled,
+                    rv.metadata.enabled,
                     rv.emit_event,
                     None,
                     None,
                     rv.targeting.clone(),
                     rv.overrides.clone(),
                     Some(rv.variant_set.clone()),
                 ),
                 Feature::DynamicConfig(dc) => (
                     ExperimentType::DynamicConfig,
-                    dc.enabled,
+                    dc.metadata.enabled,
                     false,
                     Some(dc.value.clone()),
                     Some(dc.value_type),
                     None,
                     None,
                     None,
                 ),
@@ -1022,15 +1021,15 @@
             Feature::DynamicConfig(dc) => dc.mutex_group(d, ctx),
         }
     }
 }
 
 impl Decide for RangeVariant {
     fn darkmode(&self, _d: &Decider, _ctx: &Context) -> Result<Choice, DeciderError> {
-        if self.enabled {
+        if self.metadata.enabled {
             Ok(Choice::Pass("darkmode:enabled"))
         } else {
             Ok(Choice::None)
         }
     }
 
     fn fractional_availability(&self, _d: &Decider, ctx: &Context) -> Result<Choice, DeciderError> {
@@ -1152,15 +1151,15 @@
             },
         }
     }
 }
 
 impl Decide for DynamicConfig {
     fn darkmode(&self, _d: &Decider, _ctx: &Context) -> Result<Choice, DeciderError> {
-        if self.enabled {
+        if self.metadata.enabled {
             Ok(Choice::Pass("darkmode:enabled"))
         } else {
             Ok(Choice::None)
         }
     }
 
     fn fractional_availability(
@@ -1404,14 +1403,15 @@
 impl From<&Experiment> for Metadata {
     fn from(exp: &Experiment) -> Self {
         Metadata {
             id: exp.id,
             name: exp.name.clone(),
             version: exp.experiment.experiment_version,
             owner: exp.owner.clone(),
+            enabled: exp.enabled,
         }
     }
 }
 
 impl From<&serde_json::Value> for ValueType {
     fn from(value: &serde_json::Value) -> Self {
         match value {
@@ -1437,15 +1437,14 @@
         .clone()
         .map(Value::from)
         .unwrap_or_else(|| Value::from(exp.value_type.unwrap_or(ValueType::Null)));
     let value_type = value.borrow().into();
 
     Ok(DynamicConfig {
         metadata: exp.into(),
-        enabled: exp.enabled,
         value,
         value_type,
     })
 }
 
 fn experiment_to_multivariant_choice(
     exp: &Experiment,
@@ -1487,15 +1486,14 @@
             .collect()
     });
 
     Ok(RangeVariant {
         metadata: exp.into(),
         emit_event: exp.emit_event,
         variant_set,
-        enabled: exp.enabled,
         targeting: exp.experiment.targeting.clone(),
         overrides,
     })
 }
 
 fn experiment_to_feature(exp: &Experiment, ec: &ExperimentConfig) -> Result<Feature, ConfigError> {
     match exp.experiment_type {
@@ -1532,26 +1530,26 @@
 
         Feature::RangeVariant(RangeVariant {
             metadata: Metadata {
                 id: 1,
                 name: "first_feature".to_string(),
                 version: 1,
                 owner: "test".to_string(),
+                enabled: true,
             },
             emit_event: true,
             variant_set: VariantSet {
                 start_ts: 0,
                 stop_ts: 2147483648, // 2 ** 31 - far future.
                 shuffle_version: 0,
                 bucketing_field: ContextField::UserId,
                 variants: vec![v],
                 holdout: None,
                 mutex_group: None,
             },
-            enabled: true,
             targeting: None,
             overrides: None,
         })
     }
 
     fn make_dynamic_config(dc: Dc) -> Feature {
         let name_str: String;
@@ -1609,16 +1607,16 @@
 
         Feature::DynamicConfig(DynamicConfig {
             metadata: Metadata {
                 id: 2,
                 name: name_str + "_dynamic_config",
                 version: 1,
                 owner: "test".to_string(),
+                enabled: true,
             },
-            enabled: true,
             value: value,
             value_type: value_type,
         })
     }
 
     fn make_experiment(name: String, meg: Option<String>, hg: Option<String>) -> Experiment {
         let c = Variant {
```

### Comparing `reddit_decider-1.4.1/Makefile` & `reddit_decider-1.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.1/README.md` & `reddit_decider-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.1/python/rust_decider/__init__.py` & `reddit_decider-1.4.2/python/rust_decider/__init__.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.1/setup.py` & `reddit_decider-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.1/src/lib.rs` & `reddit_decider-1.4.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.1/test/decider_unit_test.py` & `reddit_decider-1.4.2/test/decider_unit_test.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.1/test/integration_test.py` & `reddit_decider-1.4.2/test/integration_test.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.1/test/test_rust.py` & `reddit_decider-1.4.2/test/test_rust.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.1/test/unit_test.py` & `reddit_decider-1.4.2/test/unit_test.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.1/test/utils.py` & `reddit_decider-1.4.2/test/utils.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.1/PKG-INFO` & `reddit_decider-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-decider
-Version: 1.4.1
+Version: 1.4.2
 Requires-Dist: prometheus-client>=0.12.0,<1.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # rust_decider
 
 Rust implementation of bucketing, targeting, overrides, and dynamic config logic.
```


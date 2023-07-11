# Comparing `tmp/pysigrok-saleae-logic2-0.0.1.tar.gz` & `tmp/pysigrok_saleae_logic2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigrok-saleae-logic2-0.0.1.tar", last modified: Thu Apr  6 22:19:50 2023, max compression
+gzip compressed data, was "pysigrok_saleae_logic2-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pysigrok-saleae-logic2-0.0.1.tar` & `pysigrok_saleae_logic2-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3079 2023-04-06 22:16:57.794057 pysigrok-saleae-logic2-0.0.1/.gitignore
--rw-r--r--   0        0        0     1082 2023-03-30 18:18:56.468671 pysigrok-saleae-logic2-0.0.1/LICENSE
--rw-r--r--   0        0        0      587 2023-04-06 22:17:46.024563 pysigrok-saleae-logic2-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4549 2023-03-31 21:34:24.660692 pysigrok-saleae-logic2-0.0.1/pysigrok_logic2.py
--rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 pysigrok-saleae-logic2-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3079 2023-04-06 22:16:57.794057 pysigrok_saleae_logic2-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1082 2023-03-30 18:18:56.468671 pysigrok_saleae_logic2-0.0.2/LICENSE
+-rw-r--r--   0        0        0      587 2023-04-06 22:17:46.024563 pysigrok_saleae_logic2-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4599 2023-07-11 22:31:05.506344 pysigrok_saleae_logic2-0.0.2/pysigrok_logic2.py
+-rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 pysigrok_saleae_logic2-0.0.2/PKG-INFO
```

### Comparing `pysigrok-saleae-logic2-0.0.1/.gitignore` & `pysigrok_saleae_logic2-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pysigrok-saleae-logic2-0.0.1/LICENSE` & `pysigrok_saleae_logic2-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigrok-saleae-logic2-0.0.1/pyproject.toml` & `pysigrok_saleae_logic2-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysigrok-saleae-logic2-0.0.1/pysigrok_logic2.py` & `pysigrok_saleae_logic2-0.0.2/pysigrok_logic2.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pathlib
 import struct
 
 from sigrokdecode.input import Input
 
 from sigrokdecode import cond_matches, OUTPUT_PYTHON
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 class Logic2Input(Input):
     name = "logic2"
     desc = "Logic 2 export file format data"
     def __init__(self, filename, initial_state=None, samplecount=None):
         super().__init__()
 
@@ -63,24 +63,26 @@
                 self.next_sample |= (1 if value == "1" else 0) << bit
             if self.next_samplenum >= 0:
                 break
 
     def wait(self, conds=[]):
         if conds is None:
             conds = []
-        self.matched = [False]
+        if not conds:
+            conds = [{"skip": 1}]
+        self.matched = [False] * (len(conds) if conds else 1)
         while not any(self.matched):
-            self.matched = [False] * (len(conds) if conds else 1)
             for i, cond in enumerate(conds):
                 if "skip" in cond and cond["skip"] <= (self.next_samplenum - self.samplenum):
-                    self.matched[i] = cond["skip"] == 0
+                    self.matched[i] = True
                     self.samplenum += cond["skip"]
                     continue
 
             if any(self.matched):
+                sample = self.last_sample
                 break
 
             self.samplenum = self.next_samplenum
             if self.start_samplenum is not None:
                 self.put(self.start_samplenum, self.samplenum, OUTPUT_PYTHON, ["logic", self.last_sample])
                 if self.samplecount is not None:
                     self.samplecount -= 1
```


# Comparing `tmp/pymcabc-0.6.0.tar.gz` & `tmp/pymcabc-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymcabc-0.6.0.tar", last modified: Fri Jun 30 10:20:25 2023, max compression
+gzip compressed data, was "pymcabc-0.7.0.tar", last modified: Wed Jul 12 16:13:19 2023, max compression
```

## Comparing `pymcabc-0.6.0.tar` & `pymcabc-0.7.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:20:25.416355 pymcabc-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-30 10:20:17.000000 pymcabc-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-30 10:20:17.000000 pymcabc-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-30 10:20:25.416355 pymcabc-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-30 10:20:17.000000 pymcabc-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:20:25.416355 pymcabc-0.6.0/pymcabc/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/cross_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/decay_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/feynman_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/generate_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/identify_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/save_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:20:25.416355 pymcabc-0.6.0/pymcabc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-30 10:20:25.000000 pymcabc-0.6.0/pymcabc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-30 10:20:25.000000 pymcabc-0.6.0/pymcabc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:20:25.000000 pymcabc-0.6.0/pymcabc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-30 10:20:25.000000 pymcabc-0.6.0/pymcabc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 10:20:25.000000 pymcabc-0.6.0/pymcabc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 10:20:25.416355 pymcabc-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-30 10:20:17.000000 pymcabc-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:20:25.416355 pymcabc-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-30 10:20:17.000000 pymcabc-0.6.0/tests/test_boost.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-30 10:20:17.000000 pymcabc-0.6.0/tests/test_crosssection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-30 10:20:17.000000 pymcabc-0.6.0/tests/test_evengen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-30 10:20:17.000000 pymcabc-0.6.0/tests/test_identify.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-30 10:20:17.000000 pymcabc-0.6.0/tests/test_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:13:19.979311 pymcabc-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-12 16:13:07.000000 pymcabc-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-12 16:13:07.000000 pymcabc-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-12 16:13:19.979311 pymcabc-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-12 16:13:07.000000 pymcabc-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:13:19.979311 pymcabc-0.7.0/pymcabc/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/cross_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/decay_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/feynman_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/generate_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/identify_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/save_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:13:19.979311 pymcabc-0.7.0/pymcabc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-12 16:13:19.000000 pymcabc-0.7.0/pymcabc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-12 16:13:19.000000 pymcabc-0.7.0/pymcabc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:13:19.000000 pymcabc-0.7.0/pymcabc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 16:13:19.000000 pymcabc-0.7.0/pymcabc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 16:13:19.000000 pymcabc-0.7.0/pymcabc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 16:13:19.979311 pymcabc-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-12 16:13:07.000000 pymcabc-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:13:19.979311 pymcabc-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-12 16:13:07.000000 pymcabc-0.7.0/tests/test_boost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-12 16:13:07.000000 pymcabc-0.7.0/tests/test_crosssection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-12 16:13:07.000000 pymcabc-0.7.0/tests/test_evengen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-12 16:13:07.000000 pymcabc-0.7.0/tests/test_identify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-12 16:13:07.000000 pymcabc-0.7.0/tests/test_plot.py
```

### Comparing `pymcabc-0.6.0/LICENSE` & `pymcabc-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymcabc-0.6.0/PKG-INFO` & `pymcabc-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcabc
-Version: 0.6.0
+Version: 0.7.0
 Summary: Monte Carlo Event Generator for the ABC theory
 Home-page: https://github.com/amanmdesai/pymcabc
 Author: Aman Desai
 Author-email: amanmukeshdesai@gmail.com
 Maintainer: Aman Desai
 Maintainer-email: amanmukeshdesai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymcabc-0.6.0/README.md` & `pymcabc-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pymcabc-0.6.0/pymcabc/cross_section.py` & `pymcabc-0.7.0/pymcabc/cross_section.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,122 +13,121 @@
         self.m1 = library["m1"][0]
         self.m2 = library["m2"][0]
         self.m3 = library["m3"][0]
         self.m4 = library["m4"][0]
         self.mx = library["mx"][0]
         self.Ecm = library["Ecm"][0]
         self.g = pymcabc.constants.g
-        self.pi = pymcabc.constants.pi
-        self.delta = pymcabc.constants.delta
-        self.p_i = library["pi"][0]  # math.sqrt((self.Ecm / 2) ** 2 - (self.m1) ** 2)
+        self.p_f = library["outgoing_p"][0]
+        self.bw = library["bw"][0]
+        self.p_i = library["pi"][0]  
+        # math.sqrt((self.Ecm / 2) ** 2 - (self.m1) ** 2)        
+        # #self.E1 + self.E2
+        #self.E1 = library["E1"][0]
+        #self.E2 = library["E2"][0]
 
     def s_channel(self):
-        """definition for s channel"""
-        # deno = self.Ecm**2 - self.mx**2
-        deno = math.sqrt(self.p_i**2 + self.m1**2) + math.sqrt(self.p_i**2 + self.m2**2)
-        deno = deno**2 - self.mx**2
-        #deno = deno + self.m1**2 + self.m2**2 
-        if abs(deno) <= 0.09:
-            return (self.g**2) / (deno + 100)
-        else:
-            return (self.g**2) / deno
-
+        #deno = math.sqrt(self.p_i**2 + self.m1**2) + math.sqrt(self.p_i**2 + self.m2**2)
+        deno = self.Ecm**2 - self.mx**2  + complex(0,1) * self.mx * self.bw
+        return self.g**2 / deno
+        
     def t_channel(self, costh, pf):
         """definition for t channel"""
         deno = (
             self.m1**2
             + self.m3**2
             - self.mx**2
             - (
                 2
                 * math.sqrt(self.p_i**2 + self.m1**2)
                 * math.sqrt(pf**2 + self.m3**2)
             )
             + (2 * self.p_i * pf * costh)
         )
-        if abs(deno) <= 0.09:
-            return (self.g**2) / (deno + 100)
-        else:
-            return (self.g**2) / deno
+        deno = deno + complex(0,1) * self.mx * self.bw
+        return self.g**2 / deno
 
     def u_channel(self, costh, pf):
         """definition for u channel"""
         deno = (
             self.m1**2
             + self.m4**2
             - self.mx**2
             - (
                 2
                 * math.sqrt(self.p_i**2 + self.m1**2)
                 * math.sqrt(pf**2 + self.m4**2)
             )
             - (2 * self.p_i * pf * costh)
         )
-        if abs(deno) <= 0.09:
-            return (self.g**2) / (deno + 100)
-        else:
-            return (self.g**2) / deno
+        deno = deno + complex(0,1) * self.mx * self.bw
+        return self.g**2 / deno
 
 
 class CrossSection:
     """
     class for cross section calculation
     """
 
     def __init__(self):
-        self.pi = pymcabc.constants.pi
-        self.delta = pymcabc.constants.delta
         with open("library.json", "r") as f:
             library = json.load(f)
         self.Ecm = library["Ecm"][0]
         self.m1 = library["m1"][0]
+        self.m2 = library["m2"][0]
         self.m3 = library["m3"][0]
         self.m4 = library["m4"][0]
         self.process = library["process_type"][0]
-        self.p_f = pymcabc.constants.outgoing_p(self.Ecm, self.m3, self.m4)
-        self.p_i = library["pi"][0]  # math.sqrt((self.Ecm / 2) ** 2 - (self.m1) ** 2)
+        self.p_f = library["outgoing_p"][0]
+        self.p_i = library["pi"][0]  
         self.channel = library["channel"][0]
+        # math.sqrt((self.Ecm / 2) ** 2 - (self.m1) ** 2)
+        #self.E1 = library["E1"][0]
+        #self.E2 = library["E2"][0]
+        #self.E1 + self.E2
+        #self.p1 = math.sqrt(self.E1**2 - self.m1**2) 
+        #self.p2 = math.sqrt(self.E2**2 - self.m2**2) 
+        #self.phase_factor = math.sqrt( (self.E1*self.E2 + self.p1*self.p2)**2 - (self.m1*self.m2)**2)
+        #self.p_f = pymcabc.constants.outgoing_p(self.Ecm, self.m3, self.m4)
 
     def dsigma_st(self, costh):
         if self.channel == "s":
             ME = MatrixElement().s_channel()
         elif self.channel == "t":
             ME = MatrixElement().t_channel(costh, self.p_f)
         else:
-            ME = MatrixElement().s_channel() + MatrixElement().t_channel(
-                costh, self.p_f
-            )
-        dsigma_st = 1 / ((8 * self.Ecm * self.pi) ** 2)
+            ME = MatrixElement().s_channel() + MatrixElement().t_channel(costh, self.p_f)
+        ME = abs(ME)
+        dsigma_st = 1 / ((self.Ecm*8  * math.pi) ** 2)
         dsigma_st = dsigma_st * abs(self.p_f / self.p_i) * ME**2
         return dsigma_st
 
     def dsigma_tu(self, costh):
         if self.channel == "t":
             ME = MatrixElement().t_channel(costh, self.p_f)
         elif self.channel == "u":
             ME = MatrixElement().u_channel(costh, self.p_f)
         else:
-            ME = MatrixElement().t_channel(costh, self.p_f) + MatrixElement().u_channel(
-                costh, self.p_f
-            )
-        dsigma_tu = 0.5 / ((self.Ecm * 8 * self.pi) ** 2)
+            ME = MatrixElement().t_channel(costh, self.p_f) + MatrixElement().u_channel(costh, self.p_f)
+        ME = abs(ME)
+        dsigma_tu = 0.5 / ((self.Ecm* 8 * math.pi) ** 2)
         dsigma_tu = dsigma_tu * abs(self.p_f / self.p_i) * ME**2
         return dsigma_tu
 
     def xsection(self, w_max):
-        costh = -1 + random.random() * self.delta
+        costh = -1 + random.random() * 2
         if self.process == "st":
-            w_i = CrossSection().dsigma_st(costh) * self.delta
+            w_i = CrossSection().dsigma_st(costh) * 2 * 2 * math.pi  
         elif self.process == "tu":
-            w_i = CrossSection().dsigma_tu(costh) * self.delta
+            w_i = CrossSection().dsigma_tu(costh) * 2 * 2 * math.pi 
         if w_max < w_i:
             w_max = w_i
         return w_i, w_max
 
-    def integrate_xsec(self, N=40000):
+    def integrate_xsec(self, N=20000):
         w_sum = 0
         w_max = 0
         w_square = 0
         for _i in range(N):
             w_i, w_max = CrossSection().xsection(w_max)
             w_sum += w_i
             w_square += w_i * w_i
@@ -137,20 +136,20 @@
         library["w_max"].append(w_max)
         library["w_square"].append(w_square)
         library["w_sum"].append(w_sum)
         with open("library.json", "w") as f:
             json.dump(library, f)
         return None
 
-    def calc_xsection(self, N: int = 40000):
+    def calc_xsection(self, N: int = 20000):
         self.integrate_xsec(N)
         with open("library.json", "r") as f:
             library = json.load(f)
         w_sum = library["w_sum"][0]
         w_square = library["w_square"][0]
         w_max = library["w_max"][0]
-        sigma_x = w_sum * pymcabc.constants.convert / (N * 1e12)  # result in barn unit
+        sigma_x = w_sum * pymcabc.constants.convert/ (N * 1e12)  # result in barn unit
         variance = math.sqrt(abs((w_square / N) - (w_sum / N) ** 2))  # barn unit
         error = (
             variance * pymcabc.constants.convert / (math.sqrt(N) * 1e12)
         )  # barn unit
         return sigma_x, error
```

### Comparing `pymcabc-0.6.0/pymcabc/decay_particle.py` & `pymcabc-0.7.0/pymcabc/decay_particle.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.mA = library["mA"][0]
         self.mB = library["mB"][0]
         self.mC = library["mC"][0]
         self.decay_process = library["decay_process"][0]
         self.decay1_mass = library["decay1_mass"][0]
         self.decay2_mass = library["decay2_mass"][0]
         self.massive = library["massive_mass"][0]
-        self.delta = pymcabc.constants.delta
+        self.delta = 2
 
     def rotate(self, pdecay: Particle):
         """rotate particle"""
         costh = (2 * random.random()) - 1
         sinth = math.sqrt(1 - costh**2)
         phi = 2 * math.pi * random.random()
         sinPhi = math.sin(phi)
```

### Comparing `pymcabc-0.6.0/pymcabc/detector.py` & `pymcabc-0.7.0/pymcabc/detector.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.6.0/pymcabc/feynman_diagram.py` & `pymcabc-0.7.0/pymcabc/feynman_diagram.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.6.0/pymcabc/generate_event.py` & `pymcabc-0.7.0/pymcabc/generate_event.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 import math
 import random
 import json
 import numpy as np
-import pymcabc.constants
 from pymcabc.cross_section import CrossSection
 
 
 class GENEvents:
     """
     internal class for generating events
     """
 
     def __init__(self, Nevent: int):
-        self.delta = pymcabc.constants.delta
+        self.delta = 2
         self.Nevent = Nevent
         with open("library.json", "r") as f:
             library = json.load(f)
         self.w_max = library["w_max"][0]
-        self.Ecm = library["Ecm"][0]
+        self.Ecm = library["Ecm"][0] #+ library["E2"][0]
         self.m3 = library["m3"][0]
         self.m4 = library["m4"][0]
         self.process = library["process_type"][0]
-        self.out_p = pymcabc.constants.outgoing_p(self.Ecm, self.m3, self.m4)
+        self.out_p = library["outgoing_p"][0]
 
     def gen_events(self):
         i = 0
         prob = 0
         m_costh = np.zeros(self.Nevent)
         p1_px = np.zeros(self.Nevent)
         p1_py = np.zeros(self.Nevent)
         p1_pz = np.zeros(self.Nevent)
         p1_e = np.zeros(self.Nevent)
         p2_px = np.zeros(self.Nevent)
         p2_py = np.zeros(self.Nevent)
         p2_pz = np.zeros(self.Nevent)
         p2_e = np.zeros(self.Nevent)
         while i < self.Nevent:
-            costh = -1 + (random.random() * self.delta)
+            costh = -1 + (random.random() * 2)
             phi = 2 * math.pi * random.random()  # * self.delta
             if self.process == "st":
-                w_ii = CrossSection().dsigma_st(costh) * self.delta
+                w_ii = CrossSection().dsigma_st(costh) *  2 * 2 * math.pi 
             elif self.process == "tu":
-                w_ii = CrossSection().dsigma_tu(costh) * self.delta
+                w_ii = CrossSection().dsigma_tu(costh) *  2 * 2 * math.pi 
             prob = w_ii / self.w_max
             random_point = random.random()
             if random_point < prob:
                 m_costh[i] = math.degrees(math.acos(costh))
                 sinth = math.sqrt(1 - costh**2)
                 p1_e[i] = math.sqrt(self.out_p * self.out_p + self.m3 * self.m3)
                 p1_px[i] = self.out_p * sinth * math.cos(phi)
```

### Comparing `pymcabc-0.6.0/pymcabc/identify_process.py` & `pymcabc-0.7.0/pymcabc/identify_process.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import json
 import math
+import pymcabc.constants
 
 
 def build_json():
     library = {
         "mA": [],
         "mB": [],
         "mC": [],
         "m1": [],
         "m2": [],
         "m3": [],
         "m4": [],
         "mx": [],
+        "outgoing_p": [],
+        "bw": [],
         "massive": [],
         "massive_mass": [],
         "decay_process": [],
         "decay1_mass": [],
         "decay2_mass": [],
         "mediator": [],
         "pi": [],
@@ -37,61 +40,61 @@
     """
     This is class to define the process, masses of particles and center of mass energy
     Parameters:
         input_string (str): Physics process. Example > 'A A > B B'
         mA (float): mass of particle A
         mB (float): mass of particle B
         mC (float): mass of particle C
-        Ecm (float): center of mass energy
+        E1 (float): center of mass energy for beam 1
+        E2 (float): center of mass energy for beam 2
         channel (str): optional, use to study effect a particular channel
     """
 
     def __init__(
         self,
         input_string: str,
         mA: float,
         mB: float,
         mC: float,
         pi: float,
+        #E1: float,
+        #E2: float,
         channel: str = "none",
     ):
-        """
-        Defines the process, masses of particles and center of mass energy
-        Parameters:
-            input_string (str): Physics process. Example > 'A A > B B'
-            mA (float): mass of particle A
-            mB (float): mass of particle B
-            mC (float): mass of particle C
-            Ecm (float): center of mass energy
-            channel (str): optional, use to study effect a particular channel
-        """
 
         build_json()
         with open("library.json", "r") as f:
             self.library = json.load(f)
         self.input_string = input_string
         self.mA = mA
         self.mB = mB
         self.mC = mC
         self.p_i = pi
+        #self.E1 = E1
+        #self.E2 = E2
         if self.mA < 0 or self.mB < 0 or self.mC < 0:
             raise Exception("Negative masses not accepted")
+        #if self.E1 < 0:
+        #    raise Exception("Negative Energy not accepted")
         if self.p_i <= 0:
             raise Exception("Negative or Zero absolute momentum not accepted")
         self.library["mA"].append(mA)
         self.library["mB"].append(mB)
         self.library["mC"].append(mC)
-        self.library["pi"].append(self.p_i)
+        self.library["pi"].append(pi)
+        #self.library["E2"].append(self.E2)
         self.library["channel"].append(channel)
         self.process()
         self.channel()
         self.masses()
-        self.ECM()
         self.identify_mediator()
         self.identify_decay()
+        self.ECM()
+        self.final_momenta()
+        self.bw()
 
     def process(self):
         """identify the physics process"""
         self.library["process"].append(self.input_string)
         string = self.input_string.replace(" > ", " ")
         string = string.split(" ")
         initial_1 = string[0]
@@ -139,28 +142,38 @@
         self.library["m1"].append(pmass[0])
         self.library["m2"].append(pmass[1])
         self.library["m3"].append(pmass[2])
         self.library["m4"].append(pmass[3])
         with open("library.json", "w") as f:
             json.dump(self.library, f)
         return None
-
+    
     def ECM(self):
-        """center of mass energy"""
+        #center of mass energy
         with open("library.json", "r") as f:
             library = json.load(f)
         m1 = library["m1"][0]
         m2 = library["m2"][0]
         E1 = math.sqrt(m1**2 + self.p_i**2)
         E2 = math.sqrt(m2**2 + self.p_i**2)
         Ecm = E1 + E2
-        self.library["Ecm"].append(Ecm)
+        if len(self.library["Ecm"]) == 0:
+            self.library["Ecm"].append(Ecm)
         with open("library.json", "w") as f:
             json.dump(self.library, f)
-        return Ecm
+        print(
+              "\n",
+            "Energy Beam 1 : ", E1,
+              "\n",
+            "Energy Beam 2 : ", E2,
+              "\n",
+            "Energy CM : ", Ecm,
+              )
+        return E1, E2, Ecm
+    
 
     def identify_mediator(self):
         """identify the mediator of the process"""
         process = self.library["process"][0]
         process = process.replace(" > ", " ")
         if (
             process == "A A B B"
@@ -187,14 +200,26 @@
             self.library["mx"].append(self.mA)
             self.library["mediator"].append("A")
         else:
             return None
         with open("library.json", "w") as f:
             json.dump(self.library, f)
         return None
+    
+    def final_momenta(self):
+        p_f = pymcabc.constants.outgoing_p(self.library["Ecm"][0], self.library["m3"][0], self.library["m4"][0])
+        self.library["outgoing_p"].append(p_f)
+        with open("library.json", "w") as f:
+            json.dump(self.library, f)
+
+    def bw(self):
+        deno  = 8*math.pi*(self.library["mx"][0])**2
+        self.library["bw"].append((pymcabc.constants.g**2*self.library["outgoing_p"][0])/deno)
+        with open("library.json", "w") as f:
+            json.dump(self.library, f)
 
     def identify_decay(self):
         """identify the decay chain associated with the process"""
         mA = self.library["mA"][0]
         mB = self.library["mB"][0]
         mC = self.library["mC"][0]
         if mA > mB + mC:
```

### Comparing `pymcabc-0.6.0/pymcabc/particle.py` & `pymcabc-0.7.0/pymcabc/particle.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.6.0/pymcabc/plotting.py` & `pymcabc-0.7.0/pymcabc/plotting.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.6.0/pymcabc/save_events.py` & `pymcabc-0.7.0/pymcabc/save_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.Nevent = Nevent
         self.detector_sigma = detector_sigma
         self.detector_factor = detector_factor
 
         with open("library.json", "r") as f:
             library = json.load(f)
         self.w_max = library["w_max"][0]
-        self.Ecm = library["Ecm"][0]
+        self.Ecm = library["Ecm"][0] 
         input_string = library["process"][0]
         input_string = input_string.replace(" > ", " ")
         input_string = input_string.split(" ")
         self.output_1 = input_string[2]
         self.output_2 = input_string[3]
         if self.output_1 == self.output_2:
             self.output_1 = self.output_1 + "_1"
```

### Comparing `pymcabc-0.6.0/pymcabc.egg-info/PKG-INFO` & `pymcabc-0.7.0/pymcabc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcabc
-Version: 0.6.0
+Version: 0.7.0
 Summary: Monte Carlo Event Generator for the ABC theory
 Home-page: https://github.com/amanmdesai/pymcabc
 Author: Aman Desai
 Author-email: amanmukeshdesai@gmail.com
 Maintainer: Aman Desai
 Maintainer-email: amanmukeshdesai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymcabc-0.6.0/pymcabc.egg-info/SOURCES.txt` & `pymcabc-0.7.0/pymcabc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymcabc-0.6.0/setup.py` & `pymcabc-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setuptools.setup(
     name="pymcabc",
-    version="0.6.0",
+    version="0.7.0",
     description="Monte Carlo Event Generator for the ABC theory",
     author="Aman Desai",
     author_email="amanmukeshdesai@gmail.com",
     maintainer="Aman Desai",
     maintainer_email="amanmukeshdesai@gmail.com",
     url="https://github.com/amanmdesai/pymcabc",
     long_description=long_description,
```

### Comparing `pymcabc-0.6.0/tests/test_evengen.py` & `pymcabc-0.7.0/tests/test_evengen.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.6.0/tests/test_identify.py` & `pymcabc-0.7.0/tests/test_identify.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     library["process_type"][0] == "st"
 
 
 def test_negative_param():
     with pytest.raises(Exception, match="Negative masses not accepted"):
         pymcabc.DefineProcess("A B > A B", mA=4, mB=-10, mC=1, pi=30)
 
+def test_negative_param_2():
     with pytest.raises(
-        Exception, match="Negative or Zero absolute momentum not accepted"
-    ):
+        Exception, match="Negative or Zero absolute momentum not accepted"):
         pymcabc.DefineProcess("A B > A B", mA=4, mB=10, mC=1, pi=-30)
 
 
 """
 def test_feynmandiagram_tu():
     pymcabc.DefineProcess('A A > B B',mA=4,mB=10,mC=1,pi=30)
     pymcabc.FeynmanDiagram()
```

### Comparing `pymcabc-0.6.0/tests/test_plot.py` & `pymcabc-0.7.0/tests/test_plot.py`

 * *Files identical despite different names*


# Comparing `tmp/I2MC-2.2.2.tar.gz` & `tmp/I2MC-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "I2MC-2.2.2.tar", last modified: Thu Jan  5 15:06:53 2023, max compression
+gzip compressed data, was "I2MC-2.2.4.tar", last modified: Wed Jul 12 18:50:35 2023, max compression
```

## Comparing `I2MC-2.2.2.tar` & `I2MC-2.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-05 15:06:53.181819 I2MC-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1104 2023-01-05 15:06:39.000000 I2MC-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     5551 2023-01-05 15:06:53.181819 I2MC-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3741 2023-01-05 15:06:39.000000 I2MC-2.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      104 2023-01-05 15:06:39.000000 I2MC-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-01-05 15:06:53.181819 I2MC-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1032 2023-01-05 15:06:39.000000 I2MC-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-05 15:06:53.177819 I2MC-2.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-05 15:06:53.177819 I2MC-2.2.2/src/I2MC/
--rw-r--r--   0 runner    (1001) docker     (116)    62969 2023-01-05 15:06:39.000000 I2MC-2.2.2/src/I2MC/I2MC.py
--rw-r--r--   0 runner    (1001) docker     (116)      189 2023-01-05 15:06:39.000000 I2MC-2.2.2/src/I2MC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-05 15:06:53.181819 I2MC-2.2.2/src/I2MC/plot/
--rw-r--r--   0 runner    (1001) docker     (116)       20 2023-01-05 15:06:39.000000 I2MC-2.2.2/src/I2MC/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3714 2023-01-05 15:06:39.000000 I2MC-2.2.2/src/I2MC/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (116)      411 2023-01-05 15:06:39.000000 I2MC-2.2.2/src/I2MC/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-05 15:06:53.181819 I2MC-2.2.2/src/I2MC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5551 2023-01-05 15:06:53.000000 I2MC-2.2.2/src/I2MC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      306 2023-01-05 15:06:53.000000 I2MC-2.2.2/src/I2MC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-05 15:06:53.000000 I2MC-2.2.2/src/I2MC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       30 2023-01-05 15:06:53.000000 I2MC-2.2.2/src/I2MC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2023-01-05 15:06:53.000000 I2MC-2.2.2/src/I2MC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:50:35.726591 I2MC-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-12 18:50:20.000000 I2MC-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-12 18:50:35.726591 I2MC-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-12 18:50:20.000000 I2MC-2.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 18:50:20.000000 I2MC-2.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:50:35.726591 I2MC-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-12 18:50:20.000000 I2MC-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:50:35.722591 I2MC-2.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:50:35.722591 I2MC-2.2.4/src/I2MC/
+-rw-r--r--   0 runner    (1001) docker     (123)    62969 2023-07-12 18:50:20.000000 I2MC-2.2.4/src/I2MC/I2MC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-12 18:50:20.000000 I2MC-2.2.4/src/I2MC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:50:35.726591 I2MC-2.2.4/src/I2MC/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 18:50:20.000000 I2MC-2.2.4/src/I2MC/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-12 18:50:20.000000 I2MC-2.2.4/src/I2MC/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-12 18:50:20.000000 I2MC-2.2.4/src/I2MC/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:50:35.726591 I2MC-2.2.4/src/I2MC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-12 18:50:35.000000 I2MC-2.2.4/src/I2MC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-12 18:50:35.000000 I2MC-2.2.4/src/I2MC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:50:35.000000 I2MC-2.2.4/src/I2MC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-12 18:50:35.000000 I2MC-2.2.4/src/I2MC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 18:50:35.000000 I2MC-2.2.4/src/I2MC.egg-info/top_level.txt
```

### Comparing `I2MC-2.2.2/LICENSE` & `I2MC-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `I2MC-2.2.2/PKG-INFO` & `I2MC-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: I2MC
-Version: 2.2.2
+Version: 2.2.4
 Summary: Noise-robust fixation classification (I2MC).
 Home-page: https://github.com/dcnieho/I2MC_Python
 Author: Diederick Niehorster
 Author-email: diederick_c.niehorster@humlab.lu.se
 License: MIT License
         
         Copyright (c) 2019-2021 Jonathan van Leeuwen, Diederick Niehorster
```

### Comparing `I2MC-2.2.2/README.md` & `I2MC-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `I2MC-2.2.2/setup.py` & `I2MC-2.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `I2MC-2.2.2/src/I2MC/I2MC.py` & `I2MC-2.2.4/src/I2MC/I2MC.py`

 * *Files identical despite different names*

### Comparing `I2MC-2.2.2/src/I2MC/plot/plot.py` & `I2MC-2.2.4/src/I2MC/plot/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,17 +69,17 @@
     else:
         ax1.set_ylim([0, res[0]])
 
     ax2 = plt.subplot(2,1,2, sharex=ax1)
     ax2.set_xlabel('Time (ms)')
     ax2.set_ylabel('Vertical position ({})'.format(unit), size = myLabelSize)
     if isinstance(res[1],list):
-        ax1.set_ylim([res[1][0], res[1][1]])
+        ax2.set_ylim([res[1][0], res[1][1]])
     else:
-        ax1.set_ylim([0, res[1]])
+        ax2.set_ylim([0, res[1]])
 
     ### Plot X position
     Xdatp = np.atleast_2d(Xdat)
     for p in range(Xdatp.shape[0]):
         ax1.plot(np.array(time),Xdatp[p,:],klr[p]+'-', linewidth = traceLW)
 
     ### Plot Y posiiton
```

### Comparing `I2MC-2.2.2/src/I2MC.egg-info/PKG-INFO` & `I2MC-2.2.4/src/I2MC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: I2MC
-Version: 2.2.2
+Version: 2.2.4
 Summary: Noise-robust fixation classification (I2MC).
 Home-page: https://github.com/dcnieho/I2MC_Python
 Author: Diederick Niehorster
 Author-email: diederick_c.niehorster@humlab.lu.se
 License: MIT License
         
         Copyright (c) 2019-2021 Jonathan van Leeuwen, Diederick Niehorster
```


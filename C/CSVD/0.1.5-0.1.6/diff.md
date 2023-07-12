# Comparing `tmp/CSVD-0.1.5.tar.gz` & `tmp/CSVD-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Work\pythonProject\CSVD_pip\dist\.tmp-a1o802ca\CSVD-0.1.5.tar", last modified: Wed Jul 12 10:28:13 2023, max compression
+gzip compressed data, was "D:\Work\pythonProject\CSVD_pip\dist\.tmp-kjmaoq9k\CSVD-0.1.6.tar", last modified: Wed Jul 12 10:39:42 2023, max compression
```

## Comparing `CSVD-0.1.5.tar` & `CSVD-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 10:28:13.000000 CSVD-0.1.5/
--rw-rw-rw-   0        0        0     1090 2022-06-04 21:48:47.000000 CSVD-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1917 2023-07-12 10:28:13.000000 CSVD-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1335 2023-03-08 11:58:00.000000 CSVD-0.1.5/README.md
--rw-rw-rw-   0        0        0      110 2022-06-04 17:41:15.000000 CSVD-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0      753 2023-07-12 10:28:13.000000 CSVD-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/CSVD/
--rw-rw-rw-   0        0        0     2899 2023-07-12 10:27:23.000000 CSVD-0.1.5/src/CSVD/CSVD.py
--rw-rw-rw-   0        0        0       24 2022-09-05 17:07:48.000000 CSVD-0.1.5/src/CSVD/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-03-08 11:46:19.000000 CSVD-0.1.5/src/CSVD/watrem.py
-drwxrwxrwx   0        0        0        0 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/CSVD.egg-info/
--rw-rw-rw-   0        0        0     1917 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/CSVD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/CSVD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/CSVD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/CSVD.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/CSVD.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-12 10:28:13.000000 CSVD-0.1.5/test/
--rw-rw-rw-   0        0        0      944 2023-03-08 11:47:56.000000 CSVD-0.1.5/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:39:42.000000 CSVD-0.1.6/
+-rw-rw-rw-   0        0        0     1090 2022-06-04 21:48:47.000000 CSVD-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1917 2023-07-12 10:39:42.000000 CSVD-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1335 2023-03-08 11:58:00.000000 CSVD-0.1.6/README.md
+-rw-rw-rw-   0        0        0      110 2022-06-04 17:41:15.000000 CSVD-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0      753 2023-07-12 10:39:42.000000 CSVD-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 10:39:42.000000 CSVD-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 10:39:42.000000 CSVD-0.1.6/src/CSVD/
+-rw-rw-rw-   0        0        0     2930 2023-07-12 10:39:21.000000 CSVD-0.1.6/src/CSVD/CSVD.py
+-rw-rw-rw-   0        0        0       24 2022-09-05 17:07:48.000000 CSVD-0.1.6/src/CSVD/__init__.py
+-rw-rw-rw-   0        0        0     1488 2023-03-08 11:46:19.000000 CSVD-0.1.6/src/CSVD/watrem.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:39:42.000000 CSVD-0.1.6/src/CSVD.egg-info/
+-rw-rw-rw-   0        0        0     1917 2023-07-12 10:39:42.000000 CSVD-0.1.6/src/CSVD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-07-12 10:39:42.000000 CSVD-0.1.6/src/CSVD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 10:39:42.000000 CSVD-0.1.6/src/CSVD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 10:39:42.000000 CSVD-0.1.6/src/CSVD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-12 10:39:42.000000 CSVD-0.1.6/src/CSVD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 10:39:42.000000 CSVD-0.1.6/test/
+-rw-rw-rw-   0        0        0      944 2023-03-08 11:47:56.000000 CSVD-0.1.6/test/test.py
```

### Comparing `CSVD-0.1.5/LICENSE` & `CSVD-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `CSVD-0.1.5/PKG-INFO` & `CSVD-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CSVD
-Version: 0.1.5
+Version: 0.1.6
 Summary: Fast and Scalable Water Removal in MR Spectroscopic Data using Casorati Lanczos Singular Value Decomposition
 Home-page: https://github.com/pypa/sampleproject
 Author: amir shamaei
 Author-email: amirshamaei@isibrno.cz
 Project-URL: Bug Tracker, https://github.com/amirshamaei/CSVD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CSVD-0.1.5/README.md` & `CSVD-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `CSVD-0.1.5/setup.cfg` & `CSVD-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 5356 440d 0a76 6572 7369 6f6e   = CSVD..version
-00000020: 203d 2030 2e31 2e35 0d0a 6175 7468 6f72   = 0.1.5..author
+00000020: 203d 2030 2e31 2e36 0d0a 6175 7468 6f72   = 0.1.6..author
 00000030: 203d 2061 6d69 7220 7368 616d 6165 690d   = amir shamaei.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 616d 6972 7368 616d 6165 6940 6973 6962  amirshamaei@isib
 00000060: 726e 6f2e 637a 0d0a 6465 7363 7269 7074  rno.cz..descript
 00000070: 696f 6e20 3d20 4661 7374 2061 6e64 2053  ion = Fast and S
 00000080: 6361 6c61 626c 6520 5761 7465 7220 5265  calable Water Re
 00000090: 6d6f 7661 6c20 696e 204d 5220 5370 6563  moval in MR Spec
```

### Comparing `CSVD-0.1.5/src/CSVD/CSVD.py` & `CSVD-0.1.6/src/CSVD/CSVD.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,16 @@
         :param rank: the rank of the SVD decomposition. If you set it to 'auto', it will use the optimal rank as determined
         by the optimal hard thresholding algorithm
         :param frequency_band: a tuple which contains two lists, i.e. ([fmins], [fmaxs])
         :param n_comp: number of components to remove
         :param sigma: the threshold for the singular values. If None, the default is the median of the singular values
         :return: The signal after the removal of the noise.
         """
-        if rank == 'auto':
+        self.rank = rank
+        if self.rank == 'auto':
             limit = svht(sigma, self.data.shape,self.s)
             self.rank = np.where(self.s < limit)[0][0]
             if self.rank == 0:
                 self.rank = 1
         U_ = self.U.copy()
         for i in range(0, self.rank):
             U_[:, i] = watrem(self.U[:, i],self.dt, n_comp, frequency_band)
```

### Comparing `CSVD-0.1.5/src/CSVD/watrem.py` & `CSVD-0.1.6/src/CSVD/watrem.py`

 * *Files identical despite different names*

### Comparing `CSVD-0.1.5/src/CSVD.egg-info/PKG-INFO` & `CSVD-0.1.6/src/CSVD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CSVD
-Version: 0.1.5
+Version: 0.1.6
 Summary: Fast and Scalable Water Removal in MR Spectroscopic Data using Casorati Lanczos Singular Value Decomposition
 Home-page: https://github.com/pypa/sampleproject
 Author: amir shamaei
 Author-email: amirshamaei@isibrno.cz
 Project-URL: Bug Tracker, https://github.com/amirshamaei/CSVD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CSVD-0.1.5/test/test.py` & `CSVD-0.1.6/test/test.py`

 * *Files identical despite different names*


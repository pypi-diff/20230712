# Comparing `tmp/CSVD-0.1.4.tar.gz` & `tmp/CSVD-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\pythonProject\CSVD_pip\dist\.tmp-req6v5es\CSVD-0.1.4.tar", last modified: Wed Mar  8 11:50:01 2023, max compression
+gzip compressed data, was "D:\Work\pythonProject\CSVD_pip\dist\.tmp-a1o802ca\CSVD-0.1.5.tar", last modified: Wed Jul 12 10:28:13 2023, max compression
```

## Comparing `CSVD-0.1.4.tar` & `CSVD-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-08 11:50:01.000000 CSVD-0.1.4/
--rw-rw-rw-   0        0        0     1090 2022-06-04 21:48:47.000000 CSVD-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1736 2023-03-08 11:50:01.000000 CSVD-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1154 2023-03-01 13:01:25.000000 CSVD-0.1.4/README.md
--rw-rw-rw-   0        0        0      110 2022-06-04 17:41:15.000000 CSVD-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      753 2023-03-08 11:50:01.000000 CSVD-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-08 11:50:01.000000 CSVD-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-03-08 11:50:01.000000 CSVD-0.1.4/src/CSVD/
--rw-rw-rw-   0        0        0     2879 2023-03-08 11:46:19.000000 CSVD-0.1.4/src/CSVD/CSVD.py
--rw-rw-rw-   0        0        0       24 2022-09-05 17:07:48.000000 CSVD-0.1.4/src/CSVD/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-03-08 11:46:19.000000 CSVD-0.1.4/src/CSVD/watrem.py
-drwxrwxrwx   0        0        0        0 2023-03-08 11:50:01.000000 CSVD-0.1.4/src/CSVD.egg-info/
--rw-rw-rw-   0        0        0     1736 2023-03-08 11:50:00.000000 CSVD-0.1.4/src/CSVD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-03-08 11:50:01.000000 CSVD-0.1.4/src/CSVD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-08 11:50:00.000000 CSVD-0.1.4/src/CSVD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-08 11:50:00.000000 CSVD-0.1.4/src/CSVD.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-08 11:50:00.000000 CSVD-0.1.4/src/CSVD.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-08 11:50:01.000000 CSVD-0.1.4/test/
--rw-rw-rw-   0        0        0      944 2023-03-08 11:47:56.000000 CSVD-0.1.4/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:28:13.000000 CSVD-0.1.5/
+-rw-rw-rw-   0        0        0     1090 2022-06-04 21:48:47.000000 CSVD-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1917 2023-07-12 10:28:13.000000 CSVD-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1335 2023-03-08 11:58:00.000000 CSVD-0.1.5/README.md
+-rw-rw-rw-   0        0        0      110 2022-06-04 17:41:15.000000 CSVD-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      753 2023-07-12 10:28:13.000000 CSVD-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/CSVD/
+-rw-rw-rw-   0        0        0     2899 2023-07-12 10:27:23.000000 CSVD-0.1.5/src/CSVD/CSVD.py
+-rw-rw-rw-   0        0        0       24 2022-09-05 17:07:48.000000 CSVD-0.1.5/src/CSVD/__init__.py
+-rw-rw-rw-   0        0        0     1488 2023-03-08 11:46:19.000000 CSVD-0.1.5/src/CSVD/watrem.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/CSVD.egg-info/
+-rw-rw-rw-   0        0        0     1917 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/CSVD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/CSVD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/CSVD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/CSVD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-12 10:28:13.000000 CSVD-0.1.5/src/CSVD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 10:28:13.000000 CSVD-0.1.5/test/
+-rw-rw-rw-   0        0        0      944 2023-03-08 11:47:56.000000 CSVD-0.1.5/test/test.py
```

### Comparing `CSVD-0.1.4/LICENSE` & `CSVD-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CSVD-0.1.4/PKG-INFO` & `CSVD-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CSVD
-Version: 0.1.4
+Version: 0.1.5
 Summary: Fast and Scalable Water Removal in MR Spectroscopic Data using Casorati Lanczos Singular Value Decomposition
 Home-page: https://github.com/pypa/sampleproject
 Author: amir shamaei
 Author-email: amirshamaei@isibrno.cz
 Project-URL: Bug Tracker, https://github.com/amirshamaei/CSVD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,36 +19,42 @@
 **Example code:**
 ```python
 
 import numpy as np
 import matplotlib.pyplot as plt
 from numpy.fft import fft, fftshift
 
-from src.CSVD import CSVD
+from CSVD import CSVD
 
 t=np.arange(0,1024)*.01
 ampl = np.random.normal(1,0.2,(1000,1))
 fr = np.random.normal(-15,0.1,(1000,1))
 sig1 = ampl * np.exp(-2*t) *np.exp(2*np.pi*fr*t*1j)
 
 ampl2 = np.random.normal(1,0.2,(1000,1))
 fr2 = np.random.normal(0,0.1,(1000,1))
 sig2 = ampl2 * np.exp(-2*t) *np.exp(2*np.pi*fr2*t*1j)
 
-sig = sig1 + sig2
+ampl3 = np.random.normal(1,0.2,(1000,1))
+fr3 = np.random.normal(15,0.1,(1000,1))
+sig3 = ampl3 * np.exp(-2*t) *np.exp(2*np.pi*fr3*t*1j)
+
+sig = sig1 + sig2 +sig3
 noise = np.random.normal(0,1,(sig.shape)) + 1j*np.random.normal(0,1,(sig.shape))
 sig = sig + 0.1*noise
 
 csvd = CSVD(sig.T, 0.01)
 
-sig_ = csvd.remove('auto',[-20,-10],3)
+sig_ = csvd.remove('auto',([-5,-20],[5,-10]),3)
 plt.plot(fftshift(fft(sig[0,:])).T)
 plt.plot(fftshift(fft(sig_[:,0])).T)
 plt.legend(['Orginal signal', 'Water-removed signal'])
+plt.savefig('example.jpg')
 plt.show()
+
 ```
 **output:**
 ![example](/test/example.jpg)
 
 
 **Acknowledgments**
```

### Comparing `CSVD-0.1.4/README.md` & `CSVD-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,36 +4,42 @@
 **Example code:**
 ```python
 
 import numpy as np
 import matplotlib.pyplot as plt
 from numpy.fft import fft, fftshift
 
-from src.CSVD import CSVD
+from CSVD import CSVD
 
 t=np.arange(0,1024)*.01
 ampl = np.random.normal(1,0.2,(1000,1))
 fr = np.random.normal(-15,0.1,(1000,1))
 sig1 = ampl * np.exp(-2*t) *np.exp(2*np.pi*fr*t*1j)
 
 ampl2 = np.random.normal(1,0.2,(1000,1))
 fr2 = np.random.normal(0,0.1,(1000,1))
 sig2 = ampl2 * np.exp(-2*t) *np.exp(2*np.pi*fr2*t*1j)
 
-sig = sig1 + sig2
+ampl3 = np.random.normal(1,0.2,(1000,1))
+fr3 = np.random.normal(15,0.1,(1000,1))
+sig3 = ampl3 * np.exp(-2*t) *np.exp(2*np.pi*fr3*t*1j)
+
+sig = sig1 + sig2 +sig3
 noise = np.random.normal(0,1,(sig.shape)) + 1j*np.random.normal(0,1,(sig.shape))
 sig = sig + 0.1*noise
 
 csvd = CSVD(sig.T, 0.01)
 
-sig_ = csvd.remove('auto',[-20,-10],3)
+sig_ = csvd.remove('auto',([-5,-20],[5,-10]),3)
 plt.plot(fftshift(fft(sig[0,:])).T)
 plt.plot(fftshift(fft(sig_[:,0])).T)
 plt.legend(['Orginal signal', 'Water-removed signal'])
+plt.savefig('example.jpg')
 plt.show()
+
 ```
 **output:**
 ![example](/test/example.jpg)
 
 
 **Acknowledgments**
```

### Comparing `CSVD-0.1.4/setup.cfg` & `CSVD-0.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 5356 440d 0a76 6572 7369 6f6e   = CSVD..version
-00000020: 203d 2030 2e31 2e34 0d0a 6175 7468 6f72   = 0.1.4..author
+00000020: 203d 2030 2e31 2e35 0d0a 6175 7468 6f72   = 0.1.5..author
 00000030: 203d 2061 6d69 7220 7368 616d 6165 690d   = amir shamaei.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 616d 6972 7368 616d 6165 6940 6973 6962  amirshamaei@isib
 00000060: 726e 6f2e 637a 0d0a 6465 7363 7269 7074  rno.cz..descript
 00000070: 696f 6e20 3d20 4661 7374 2061 6e64 2053  ion = Fast and S
 00000080: 6361 6c61 626c 6520 5761 7465 7220 5265  calable Water Re
 00000090: 6d6f 7661 6c20 696e 204d 5220 5370 6563  moval in MR Spec
```

### Comparing `CSVD-0.1.4/src/CSVD/CSVD.py` & `CSVD-0.1.5/src/CSVD/CSVD.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,19 @@
         :param frequency_band: a tuple which contains two lists, i.e. ([fmins], [fmaxs])
         :param n_comp: number of components to remove
         :param sigma: the threshold for the singular values. If None, the default is the median of the singular values
         :return: The signal after the removal of the noise.
         """
         if rank == 'auto':
             limit = svht(sigma, self.data.shape,self.s)
-            rank = np.where(self.s < limit)[0][0]
-            if rank == 0:
-                rank = 1
+            self.rank = np.where(self.s < limit)[0][0]
+            if self.rank == 0:
+                self.rank = 1
         U_ = self.U.copy()
-        for i in range(0, rank):
+        for i in range(0, self.rank):
             U_[:, i] = watrem(self.U[:, i],self.dt, n_comp, frequency_band)
         sigs = np.dot(U_[:, :len(self.s)] * self.s, self.V)
         return sigs
 
 def svht(var, data_shape, S):
     """
     > The function takes in the singular values of a matrix and returns the threshold value for the singular values
```

### Comparing `CSVD-0.1.4/src/CSVD/watrem.py` & `CSVD-0.1.5/src/CSVD/watrem.py`

 * *Files identical despite different names*

### Comparing `CSVD-0.1.4/src/CSVD.egg-info/PKG-INFO` & `CSVD-0.1.5/src/CSVD.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CSVD
-Version: 0.1.4
+Version: 0.1.5
 Summary: Fast and Scalable Water Removal in MR Spectroscopic Data using Casorati Lanczos Singular Value Decomposition
 Home-page: https://github.com/pypa/sampleproject
 Author: amir shamaei
 Author-email: amirshamaei@isibrno.cz
 Project-URL: Bug Tracker, https://github.com/amirshamaei/CSVD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,36 +19,42 @@
 **Example code:**
 ```python
 
 import numpy as np
 import matplotlib.pyplot as plt
 from numpy.fft import fft, fftshift
 
-from src.CSVD import CSVD
+from CSVD import CSVD
 
 t=np.arange(0,1024)*.01
 ampl = np.random.normal(1,0.2,(1000,1))
 fr = np.random.normal(-15,0.1,(1000,1))
 sig1 = ampl * np.exp(-2*t) *np.exp(2*np.pi*fr*t*1j)
 
 ampl2 = np.random.normal(1,0.2,(1000,1))
 fr2 = np.random.normal(0,0.1,(1000,1))
 sig2 = ampl2 * np.exp(-2*t) *np.exp(2*np.pi*fr2*t*1j)
 
-sig = sig1 + sig2
+ampl3 = np.random.normal(1,0.2,(1000,1))
+fr3 = np.random.normal(15,0.1,(1000,1))
+sig3 = ampl3 * np.exp(-2*t) *np.exp(2*np.pi*fr3*t*1j)
+
+sig = sig1 + sig2 +sig3
 noise = np.random.normal(0,1,(sig.shape)) + 1j*np.random.normal(0,1,(sig.shape))
 sig = sig + 0.1*noise
 
 csvd = CSVD(sig.T, 0.01)
 
-sig_ = csvd.remove('auto',[-20,-10],3)
+sig_ = csvd.remove('auto',([-5,-20],[5,-10]),3)
 plt.plot(fftshift(fft(sig[0,:])).T)
 plt.plot(fftshift(fft(sig_[:,0])).T)
 plt.legend(['Orginal signal', 'Water-removed signal'])
+plt.savefig('example.jpg')
 plt.show()
+
 ```
 **output:**
 ![example](/test/example.jpg)
 
 
 **Acknowledgments**
```

### Comparing `CSVD-0.1.4/test/test.py` & `CSVD-0.1.5/test/test.py`

 * *Files identical despite different names*


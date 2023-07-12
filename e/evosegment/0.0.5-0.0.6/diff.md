# Comparing `tmp/evosegment-0.0.5.tar.gz` & `tmp/evosegment-0.0.6.tar.gz`

## Comparing `evosegment-0.0.5.tar` & `evosegment-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0   746872 2020-02-02 00:00:00.000000 evosegment-0.0.5/example.ipynb
--rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_0.tif
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_1-bubble_0-registration.tsv
--rw-r--r--   0        0        0  2663864 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_1-reg-def.tif
--rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_1.tif
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_2-bubble_0-registration.tsv
--rw-r--r--   0        0        0  2663864 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_2-reg-def.tif
--rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_2.tif
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_3-bubble_0-registration.tsv
--rw-r--r--   0        0        0  2663864 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_3-reg-def.tif
--rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_3.tif
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 evosegment-0.0.5/evosegment/__init__.py
--rw-r--r--   0        0        0    17097 2020-02-02 00:00:00.000000 evosegment-0.0.5/evosegment/evoSegment.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 evosegment-0.0.5/evosegment/make_release
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 evosegment-0.0.5/.gitignore
--rw-r--r--   0        0        0    35076 2020-02-02 00:00:00.000000 evosegment-0.0.5/LICENSE
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 evosegment-0.0.5/README.md
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 evosegment-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    42703 2020-02-02 00:00:00.000000 evosegment-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0   746872 2020-02-02 00:00:00.000000 evosegment-0.0.6/example.ipynb
+-rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.6/data/bubble_0.tif
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 evosegment-0.0.6/data/bubble_1-bubble_0-registration.tsv
+-rw-r--r--   0        0        0  2663864 2020-02-02 00:00:00.000000 evosegment-0.0.6/data/bubble_1-reg-def.tif
+-rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.6/data/bubble_1.tif
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 evosegment-0.0.6/data/bubble_2-bubble_0-registration.tsv
+-rw-r--r--   0        0        0  2663864 2020-02-02 00:00:00.000000 evosegment-0.0.6/data/bubble_2-reg-def.tif
+-rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.6/data/bubble_2.tif
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 evosegment-0.0.6/data/bubble_3-bubble_0-registration.tsv
+-rw-r--r--   0        0        0  2663864 2020-02-02 00:00:00.000000 evosegment-0.0.6/data/bubble_3-reg-def.tif
+-rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.6/data/bubble_3.tif
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 evosegment-0.0.6/evosegment/__init__.py
+-rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 evosegment-0.0.6/evosegment/evoSegment.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 evosegment-0.0.6/evosegment/make_release
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 evosegment-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35076 2020-02-02 00:00:00.000000 evosegment-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 evosegment-0.0.6/README.md
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 evosegment-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    42694 2020-02-02 00:00:00.000000 evosegment-0.0.6/PKG-INFO
```

### Comparing `evosegment-0.0.5/example.ipynb` & `evosegment-0.0.6/example.ipynb`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.5/data/bubble_0.tif` & `evosegment-0.0.6/data/bubble_0.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.5/data/bubble_1-reg-def.tif` & `evosegment-0.0.6/data/bubble_1-reg-def.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.5/data/bubble_1.tif` & `evosegment-0.0.6/data/bubble_1.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.5/data/bubble_2-reg-def.tif` & `evosegment-0.0.6/data/bubble_2-reg-def.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.5/data/bubble_2.tif` & `evosegment-0.0.6/data/bubble_2.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.5/data/bubble_3-reg-def.tif` & `evosegment-0.0.6/data/bubble_3-reg-def.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.5/data/bubble_3.tif` & `evosegment-0.0.6/data/bubble_3.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.5/evosegment/evoSegment.py` & `evosegment-0.0.6/evosegment/evoSegment.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,16 +196,19 @@
             if dmin / ra + Pks / Pstar >= 1:
                 centers.append([coordinates[ii][0], coordinates[ii][1]])
                 retstat = 1
             else:
                 Pi[ii] = 0
     return retstat, centers, Pi
 
-def findAndFilterPeaks(data,k=1000,plot=False,verbose=False):
+def findAndFilterPeaks(data,k=1000,plot=False,verbose=False,filter=False,filterpars=(3,1)):
     npix = np.sum(data)
+    if filter:
+        data = scipy.signal.savgol_filter(data,filterpars[0],filterpars[1])
+
     peaks,properties = scipy.signal.find_peaks(data)#,width=1,height=1)
     widths,wh,lb,rb = scipy.signal.peak_widths(data,peaks,rel_height=0.5)
     peaksums = np.asarray([np.sum(data[int(np.floor(l)):int(np.ceil(r))]) for l,r in zip(lb,rb)])
     pph = peaksums > k
     peaks = peaks[pph]
     if verbose:
         print(f'The threshold is {k:d} voxels and there are {int(npix):d} voxels in this subset')
@@ -252,45 +255,50 @@
             dn = np.diag(H,-i)
             dn = np.pad(dn,(0,i),mode='constant')
             diags.append(dn)
     #sum the diagonals
     return np.sum(np.asarray(diags),axis=0)
 
 
-def detectClusterCenters(H, diagonalwidth=3, halfstripwidth=4, kd=10000,kod=1000,plot=False,verbose=False):
+def detectClusterCenters(H, diagonalwidth=3, halfstripwidth=4, kd=10000,kod=1000,plot=False,verbose=False,filter=False,filterpars=(3,1)):
     """
     Detects cluster centers (peaks) in a 2D histogram.
 
     The function applies smoothing to the diagonal of the histogram, identifies peaks in the smoothed diagonal,
     and extracts additional peaks in vertical strips around each diagonal peak. It also includes a peak in the
     bottom row of the histogram to account for padding during registration.
 
     Parameters:
         H (ndarray): 2D histogram array.
         diagonalwidth (int): Optional. Width of band extracted along the diagonal of H for finding peaks. Default=3.
         halfstripwidth (int): Optional. Half-width of the vertical band extracted around the diagonal clusters. Defaul=2.
         kd (int): Optional. Threshold on number of pixels in the peak for accepting a peak on the diagonal. Defalt = 10000
         kod (int): Optional. Threshold on number of pixels in the peak for accepting a peak off the diagonal. Defalt = 1000
+        filter (bool): Optional. If True performs savgol filtering before peaksearching
+        filterpars (tuple): Optional. Tuple of (window_length, order) for the savgol filter. Default =(3,1)
 
     Returns:
         tuple: A tuple containing the number of detected cluster centers and an array of their coordinates.
             - The coordinate array has shape (N, 2), where N is the number of clusters detected.
               Each row represents a cluster and contains the row and col coordinates.
 
     """
     diag = sumDiagonalBand(H,diagonalwidth)
-    diag_peaks = findAndFilterPeaks(diag,k=kd,plot=plot,verbose=verbose)
+    diag_peaks = findAndFilterPeaks(diag,k=kd,plot=plot,verbose=verbose,filter=filter,filterpars=filterpars)
     if verbose:
         print('diag_peaks:', diag_peaks,'\n')
     peaks = []
     
     for p in diag_peaks:
-        col = H[:, p - halfstripwidth:p + halfstripwidth]  # Take a vertical strip at the peak to increase signal-to-noise
-        col = np.mean(col, axis=-1)
-        odp = findAndFilterPeaks(col,k=kod,plot=plot,verbose=verbose)
+        if halfstripwidth==0:
+            col = H[:,p]
+        else:
+            col = H[:, p - halfstripwidth:p + halfstripwidth]  # Take a vertical strip at the peak to increase signal-to-noise
+            col = np.mean(col, axis=-1)
+        odp = findAndFilterPeaks(col,k=kod,plot=plot,verbose=verbose,filter=filter,filterpars=filterpars)
         if verbose:
             print(f'Peaks at column {p}:', odp,'\n')
         if len(odp)>0:
             peaks.append([[op, p] for op in odp])
 
     # # Add a peaks in the bottom row of the histogram to account for padding during registration
     # row = H[0, :]
@@ -323,20 +331,22 @@
     """
     if H.ndim != 2:
         raise ValueError("Input histogram must be a 2D ndarray.")
     if kcentroids.ndim != 2:
         raise ValueError("Cluster centroids must be a 2D ndarray.")
 
     labels = np.zeros(H.shape, dtype=int)
+    print(kcentroids)
     for ii in range(H.shape[0]):
         for jj in range(H.shape[1]):
             if H[ii, jj] >= threshold:
-                rc = [ii, jj]
+                rc = [ii+0.5, jj+0.5] #center of the pixel
                 distances = distance.cdist([rc], kcentroids)
                 labels[ii, jj] = np.argmin(distances) + 1
+
     
     if make_cmap:
         cmap = colors.ListedColormap(sns.color_palette(cc.glasbey_dark, n_colors=len(kcentroids)))
         return labels, cmap
     return labels
```

### Comparing `evosegment-0.0.5/LICENSE` & `evosegment-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.5/README.md` & `evosegment-0.0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # evoSegment
-This is a tool to segment microstructural evolution from 4D tomography data (or other image data).The method is based on k-means clustering of a 2D histogram built from the intensities in a reference state and in an evolved state.
+This is a tool to segment microstructural evolution from 4D tomography data (or other image data).The method is based on clustering of a 2D histogram built from the intensities in a reference state and in an evolved state.
 
 ## Installation
 The easiest is to install the package from PyPI using
 ```python3 - m pip install evosegment```
 
 It is also possible to clone the repository, build and install a local wheel. Something like this might work:
 ```
```

### Comparing `evosegment-0.0.5/pyproject.toml` & `evosegment-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "evosegment"
-version = "0.0.5"
-description = 'A tool for segmentation of grayscale evolution from 4D tomograhphy data (or other images)'
+version = "0.0.6"
+description = 'A tool for segmentation of grayscale evolution from 4D tomography data (or other images)'
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file="LICENSE"}
 keywords = []
 authors = [
   { name = "Johan Hektor", email = "johan.hektor@mau.se" },
 ]
```

### Comparing `evosegment-0.0.5/PKG-INFO` & `evosegment-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: evosegment
-Version: 0.0.5
-Summary: A tool for segmentation of grayscale evolution from 4D tomograhphy data (or other images)
+Version: 0.0.6
+Summary: A tool for segmentation of grayscale evolution from 4D tomography data (or other images)
 Project-URL: Documentation, https://gitlab.com/jhektor/evoSegment#readme
 Project-URL: Issues, https://gitlab.com/jhektor/evoSegment/-/issues
 Project-URL: Source, https://gitlab.com/jhektor/evoSegment
 Author-email: Johan Hektor <johan.hektor@mau.se>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -698,15 +698,15 @@
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: seaborn
 Requires-Dist: tifffile
 Description-Content-Type: text/markdown
 
 # evoSegment
-This is a tool to segment microstructural evolution from 4D tomography data (or other image data).The method is based on k-means clustering of a 2D histogram built from the intensities in a reference state and in an evolved state.
+This is a tool to segment microstructural evolution from 4D tomography data (or other image data).The method is based on clustering of a 2D histogram built from the intensities in a reference state and in an evolved state.
 
 ## Installation
 The easiest is to install the package from PyPI using
 ```python3 - m pip install evosegment```
 
 It is also possible to clone the repository, build and install a local wheel. Something like this might work:
 ```
```


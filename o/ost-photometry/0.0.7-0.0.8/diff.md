# Comparing `tmp/ost_photometry-0.0.7.tar.gz` & `tmp/ost_photometry-0.0.8.tar.gz`

## Comparing `ost_photometry-0.0.7.tar` & `ost_photometry-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/__init__.py
--rwxr-xr-x   0        0        0    21964 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/aux.py
--rwxr-xr-x   0        0        0     6453 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/calibration_data.py
--rwxr-xr-x   0        0        0     5281 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/checks.py
--rwxr-xr-x   0        0        0      336 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/style.py
--rwxr-xr-x   0        0        0     1761 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/terminal_output.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/analyze/__init__.py
--rwxr-xr-x   0        0        0   166982 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/analyze/analyze.py
--rwxr-xr-x   0        0        0    84313 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/analyze/aux.py
--rwxr-xr-x   0        0        0    30838 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/analyze/calib.py
--rwxr-xr-x   0        0        0    32008 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/analyze/correlate.py
--rwxr-xr-x   0        0        0    66907 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/analyze/plot.py
--rwxr-xr-x   0        0        0    60779 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/analyze/trans.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/reduce/__init__.py
--rwxr-xr-x   0        0        0    67568 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/reduce/aux.py
--rwxr-xr-x   0        0        0    10487 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/reduce/plot.py
--rwxr-xr-x   0        0        0    76037 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/src/ost_photometry/reduce/redu.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/LICENSE
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/README.md
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 ost_photometry-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/__init__.py
+-rwxr-xr-x   0        0        0    22583 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/aux.py
+-rwxr-xr-x   0        0        0    33224 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/calibration_data.py
+-rwxr-xr-x   0        0        0     5257 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/checks.py
+-rwxr-xr-x   0        0        0      336 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/style.py
+-rwxr-xr-x   0        0        0     1807 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/terminal_output.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/analyze/__init__.py
+-rwxr-xr-x   0        0        0   169411 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/analyze/analyze.py
+-rwxr-xr-x   0        0        0    93191 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/analyze/aux.py
+-rwxr-xr-x   0        0        0    30838 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/analyze/calib.py
+-rwxr-xr-x   0        0        0    32008 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/analyze/correlate.py
+-rwxr-xr-x   0        0        0    68510 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/analyze/plot.py
+-rwxr-xr-x   0        0        0    60651 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/analyze/trans.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/reduce/__init__.py
+-rwxr-xr-x   0        0        0    76958 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/reduce/aux.py
+-rwxr-xr-x   0        0        0    10238 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/reduce/plot.py
+-rwxr-xr-x   0        0        0    76895 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/src/ost_photometry/reduce/redu.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/LICENSE
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/README.md
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 ost_photometry-0.0.8/PKG-INFO
```

### Comparing `ost_photometry-0.0.7/src/ost_photometry/aux.py` & `ost_photometry-0.0.8/src/ost_photometry/aux.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,17 +100,14 @@
     #   Read ra and dec of image center
     ra  = header.get('OBJCTRA', '00 00 00')
     dec = header.get('OBJCTDEC', '+00 00 00')
 
     #   Convert ra & dec to degrees
     coord_fov = SkyCoord(ra, dec, unit=(u.hourangle, u.deg), frame="icrs")
 
-    #   Set instrument
-    instrument = header.get('INSTRUME', '')
-
     #   Number of pixels
     npixX = header.get('NAXIS1', 0)
     npixY = header.get('NAXIS2', 0)
 
     if npixX == 0:
         raise ValueError(
             f"{style.bcolors.FAIL}\nException in cal_fov(): X dimension of "
@@ -118,19 +115,41 @@
             )
     if npixY == 0:
         raise ValueError(
             f"{style.bcolors.FAIL}\nException in cal_fov(): Y dimension of "
             f"the image is 0 {style.bcolors.ENDC}"
             )
 
+    #   Get binning
+    binX = header.get('YBINNING', 1)
+    binY = header.get('YBINNING', 1)
+
+    #   Set instrument
+    instrument = header.get('INSTRUME', '')
+
+    if instrument in ['QHYCCD-Cameras-Capture', 'QHYCCD-Cameras2-Capture']:
+        #   Physical chip dimensions in pixel
+        xdim_phy = npixX * binX
+        ydim_phy = npixY * binY
+
+        #   Set instrument
+        if xdim_phy == 9576 and ydim_phy == 6388:
+            instrument = 'QHY600M'
+        elif xdim_phy == 6280 and ydim_phy == 4210:
+            instrument = 'QHY268M'
+        elif xdim_phy == 3864 and ydim_phy == 2180:
+            instrument = 'QHY485C'
+        else:
+            instrument = ''
+
     #   Calculate chip size in mm
     if 'XPIXSZ' in header:
         pixwidth = header['XPIXSZ']
-        d = npixX*pixwidth/1000
-        h = npixY*pixwidth/1000
+        d = npixX * pixwidth / 1000
+        h = npixY * pixwidth / 1000
     else:
         d, h = calibration_data.get_chip_dimensions(instrument)
 
     #   Calculate field of view
     fov_x = 2 * np.arctan(d/2/f)
     fov_y = 2 * np.arctan(h/2/f)
 
@@ -454,15 +473,15 @@
         string="Searching for a WCS solution (pixel to ra/dec conversion)",
         )
 
     #   Define WCS dir
     if wcs_dir is None:
         wcs_dir = (image.outpath / 'wcs_imgs')
     else:
-        wcs_dir = checks.check_pathlib_Path(wcs_dir)
+        wcs_dir = checks.check_pathlib_path(wcs_dir)
         wcs_dir = wcs_dir / random_string_generator(7)
         checks.check_out(wcs_dir)
 
 
     #   Check output directories
     checks.check_out(image.outpath, wcs_dir)
```

### Comparing `ost_photometry-0.0.7/src/ost_photometry/checks.py` & `ost_photometry-0.0.8/src/ost_photometry/checks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,190 +1,189 @@
-
 ############################################################################
 ####                            Libraries                               ####
 ############################################################################
 
 import os
 
-import sys
-
 from pathlib import Path
 
 from .style import bcolors
 
+
 ############################################################################
 ####                        Routines & definitions                      ####
 ############################################################################
 
 def check_path(path):
-    '''
+    """
         Check if paths are valid
 
         Parameters
         ----------
             path        : `string`
                 Path to check
-    '''
+    """
     if not os.path.isdir(path):
         raise RuntimeError(
             f"{bcolors.FAIL} \n{path} not found -> Check file name! "
             f"ABORT {bcolors.ENDC}"
-            )
+        )
 
 
 def check_file(test_file):
-    '''
+    """
         Check if file exsits
 
         Parameters
         ----------
         test_file        : `string`
                 File to check
-    '''
+    """
     if not os.path.isfile(test_file):
         raise RuntimeError(
             f"{bcolors.FAIL} \n{test_file} not found -> Check file name! "
             f"ABORT {bcolors.ENDC}"
-            )
+        )
+
 
 def list_subdir(path):
-    '''
+    """
         List sub directories
 
         Parameters
         ----------
         path            : `string`
             Path to directory with subdirectories
 
 
         Returns
         -------
                         : `list`
             List with the original path and paths to the subdirectories
-    '''
+    """
     #   List sub directories
     subs = os.listdir(path)
 
-    #result = [os.path.join(path,element) for element in subs]
+    # result = [os.path.join(path,element) for element in subs]
     result = []
     for element in subs:
-        newpath = os.path.join(path,element)
+        newpath = os.path.join(path, element)
         if os.path.isdir(newpath):
             result.append(newpath)
-    return [path]+result
+    return [path] + result
 
 
 def check_dir(path_dict):
-    '''
+    """
         Check whether the directories exist
 
         Parameters
         ----------
         path_dict       : `dictionary`
             Keys - Path identifier : `string`; values - Path : `string`
-    '''
+    """
     missing = ""
     fail = False
     for var_name, path in path_dict.items():
         if not os.path.isdir(path):
-            missing+=f"{var_name} ({path}), "
+            missing += f"{var_name} ({path}), "
             fail = True
     if fail:
         raise RuntimeError(
             f"{bcolors.FAIL}\nNo valid {missing} files found "
             f"-> Check directory! {bcolors.ENDC}"
-            )
+        )
 
 
 def check_unumpy_array(arr):
-    '''
+    """
         Check if an array is a unumpy array. Since those arrays are also
         numpy arrays, the for dtype. The dtype of unumpy arrays is always
         ``object``.
 
         Parameters
         ----------
         arr         : `numpy.ndarray`
 
         Returns
         -------
                     : `boolean`
             ``True`` if unumpy array, ``False`` otherwise.
-    '''
+    """
     if arr.dtype == "object":
         return True
 
     return False
 
 
-def check_pathlib_Path(path):
-    '''
+def check_pathlib_path(path):
+    """
         Check if the provided path is a pathlib.Path object
 
         Parameters
         ----------
         path            : `string` or `pathlib.Path`
             Path to the images
 
         Returns
         -------
                         : `pathlib.Path`
             Return `Path`` object.
-    '''
+    """
     if isinstance(path, str):
         return Path(path)
     elif isinstance(path, Path):
         return path
     else:
         raise RuntimeError(
-            f'{bcolors.FAIL}The provided path ({arg}) is neither a String nor'
+            f'{bcolors.FAIL}The provided path ({path}) is neither a String nor'
             f' a pathlib.Path object. {bcolors.ENDC}'
-            )
+        )
 
 
 def check_out(*args):
-    '''
+    """
         Check whether the provided paths exist
             -> Create new directories if not
-    '''
+    """
     for arg in args:
         if isinstance(arg, str):
             path = Path(arg)
             Path.mkdir(path, exist_ok=True)
         elif isinstance(arg, Path):
             Path.mkdir(arg, exist_ok=True)
         else:
             raise RuntimeError(
                 f'{bcolors.FAIL}The provided path ({arg}) is neither a String '
                 f'nor a pathlib.Path object. {bcolors.ENDC}'
-                )
+            )
 
 
 def clear_directory(path):
-    '''
+    """
         Check if path is a directory and if it is empty. If the path not
         exists, create it. If the directory is not empty, remove all files in
         this directory.
 
         Parameters
         ----------
         path            : `pathlib.Path`
             Path to the directory.
-    '''
+    """
 
     if path.is_dir():
         file_list = [x for x in path.iterdir()]
         for fil in file_list:
             fil.unlink()
     else:
         path.mkdir(exist_ok=True)
 
 
 def check_dir_empty(path, del_files=True):
-    '''
+    """
         Check if path is a directory and if it is empty.
 
         Parameters
         ----------
         path            : `pathlib.Path`
             Path to the directory.
 
@@ -192,14 +191,14 @@
             If `True` files in the input directory will be removed.
             Default is ``True``.
 
         Returns
         -------
                         : `boolean`
             `False` if the directory is not empty
-    '''
+    """
 
     if path.is_dir():
         file_list = [x for x in path.iterdir()]
         if file_list:
             return False
     return True
```

### Comparing `ost_photometry-0.0.7/src/ost_photometry/analyze/analyze.py` & `ost_photometry-0.0.8/src/ost_photometry/analyze/analyze.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 ############################################################################
 ####                            Libraries                               ####
 ############################################################################
 
 import os
 
 import numpy as np
@@ -10,115 +9,119 @@
 from uncertainties import unumpy
 
 from collections import Counter
 
 from pathlib import Path
 
 import warnings
-warnings.filterwarnings('ignore', category=UserWarning, append=True)
 
 from photutils import (
     DAOStarFinder,
     EPSFBuilder,
-    )
+)
 from photutils.psf import (
     extract_stars,
     DAOGroup,
     IterativelySubtractedPSFPhotometry,
-    )
+)
 from photutils.detection import IRAFStarFinder
 from photutils.background import (
     MMMBackground,
     MADStdBackgroundRMS,
-    )
+)
 
 import ccdproc as ccdp
 
 from astropy.stats import SigmaClip
 
 from astropy.table import Table
 from astropy.time import Time
 from astropy.nddata import NDData
 from astropy.stats import (gaussian_sigma_to_fwhm, sigma_clipped_stats)
 from astropy.modeling.fitting import LevMarLSQFitter
-from astropy.coordinates import SkyCoord, Angle, matching
+from astropy.coordinates import SkyCoord, Angle
 import astropy.units as u
 
+import pandas as pd
+
 #   hips2fits module is not in the Ubuntu 22.04 package version
 #   of astroquery (0.4.1)
-#from astroquery.hips2fits import hips2fits
+# from astroquery.hips2fits import hips2fits
 from astroquery.hips2fits import hips2fitsClass
 
 from astropy.nddata import CCDData
 
 from photutils.aperture import (
     aperture_photometry,
     CircularAperture,
     CircularAnnulus,
-    )
+)
 from photutils.background import Background2D, MedianBackground
-#from photutils.utils import calc_total_error
+# from photutils.utils import calc_total_error
 
 import multiprocessing as mp
 
 from . import aux, calib, trans, plot, correlate
 # from . import subtraction
 
 from .. import style, checks, terminal_output, calibration_data
 
 from .. import aux as base_aux
 
+warnings.filterwarnings('ignore', category=UserWarning, append=True)
+
 ############################################################################
 ####                        Routines & definitions                      ####
 ############################################################################
 
+
 class image_container:
-    '''
+    """
         Container class for image class objects
-    '''
+    """
+
     def __init__(self, **kwargs):
         #   Prepare dictionary
         self.ensembles = {}
 
         #   Add additional key words
         self.__dict__.update(kwargs)
 
         #   Check for right ascension and declination
-        ra  =  kwargs.get('ra', None)
+        ra = kwargs.get('ra', None)
         dec = kwargs.get('dec', None)
         if ra is not None:
-            self.ra  = Angle(ra, unit='hour').degree
+            self.ra = Angle(ra, unit='hour').degree
         else:
             self.ra = None
         if dec is not None:
             self.dec = Angle(dec, unit='degree').degree
         else:
             self.dec = None
 
         #   Check for a object name
-        self.name  = kwargs.get('name', None)
+        self.name = kwargs.get('name', None)
 
         #   Create SkyCoord object
         if self.name is not None and self.ra is None and self.dec is None:
             self.coord = SkyCoord.from_name(self.name)
         elif self.ra is not None and self.dec is not None:
             self.coord = SkyCoord(
                 ra=self.ra,
                 dec=self.dec,
                 unit=(u.degree, u.degree),
                 frame="icrs"
-                )
+            )
         else:
             self.coord = None
 
         #   Check if uncertainty should be calculated by means of the
         #   "uncertainties" package. Default is ``True``.
         self.unc = kwargs.get('unc', True)
 
-
     #   Get ePSF objects of all images
     def get_epsf(self):
         epsf_dict = {}
         for key, ensemble in self.ensembles.items():
             epsf_list = []
             for img in ensemble.image_list:
                 epsf_list.append(img.epsf)
@@ -166,54 +169,91 @@
     def get_ensembles(self, filter_list):
         ensembles = {}
         for filt in filter_list:
             ensembles[filt] = self.ensembles[filt]
 
         return ensembles
 
+    #   Get calibrated magnitudes as numpy.ndarray
+    def get_calibrated_magnitudes(self):
+        #   Get type of the magnitude arrays
+        #   Possibilities: unumpy.uarray & numpy structured ndarray
+        unc = getattr(self, 'unc', True)
+
+        #   Get calibrated magnitudes
+        cali_mags = getattr(self, 'cali', None)
+        if unc:
+            if (cali_mags is None or
+                    np.all(unumpy.nominal_values(cali_mags) == 0.)):
+                #   If array with magnitude transformation is not available
+                #   or if it is empty get the array without magnitude
+                #   transformation
+                cali_mags = getattr(self, 'noT', None)
+                if cali_mags is not None:
+                    #   Get only the magnitude values
+                    cali_mags = unumpy.nominal_values(cali_mags)
+            else:
+                #   Get only the magnitude values
+                cali_mags = unumpy.nominal_values(cali_mags)
+
+        #   numpy structured ndarray type:
+        else:
+            if (cali_mags is None or np.all(cali_mags['mag'] == 0.)):
+                #   If array with magnitude transformation is not available
+                #   or if it is empty get the array without magnitude
+                #   transformation
+                cali_mags = getattr(self, 'noT', None)
+                if cali_mags is not None:
+                    cali_mags = cali_mags['mag']
+            else:
+                cali_mags = cali_mags['mag']
+
+        return cali_mags
+
 
 class image_ensemble:
-    '''
+    """
         Image ensemble class: Used to handle multiple images, e.g.,
         an image series taken in a specific filter
-    '''
+    """
+
     def __init__(self, filt, obj_name, path, outdir, ref_ID):
         ###
         #   Get file list, if path is a directory, if path is a file put
         #   base name of this file in a list
         #
         if os.path.isdir(path):
-            formats=[".FIT",".fit",".FITS",".fits"]
+            formats = [".FIT", ".fit", ".FITS", ".fits"]
             fileList = os.listdir(path)
 
             #   Remove not FITS entries
             tempList = []
             for file_i in fileList:
                 for j, form in enumerate(formats):
-                    if file_i.find(form)!=-1:
+                    if file_i.find(form) != -1:
                         tempList.append(file_i)
-            fileList=tempList
+            fileList = tempList
         elif os.path.isfile(path):
-            fileList=[str(path).split('/')[-1]]
+            fileList = [str(path).split('/')[-1]]
             path = os.path.dirname(path)
         else:
             raise RuntimeError(
                 f'{style.bcolors.FAIL}ERROR: Provided path is neither a file'
                 f' nor a directory -> EXIT {style.bcolors.ENDC}'
-                )
+            )
 
         ###
         #   Check if the id of the reference image is valid
         #
         if ref_ID > len(fileList):
             raise ValueError(
                 f'{style.bcolors.FAIL} ERROR: Reference image ID [ref_ID] '
                 'is larger than the total number of images!'
                 f' -> EXIT {style.bcolors.ENDC}'
-                )
+            )
 
         #   Set filter
         self.filt = filt
 
         #   Set number of images
         self.nfiles = len(fileList)
 
@@ -229,24 +269,24 @@
         #   Set object name
         self.objname = obj_name
 
         #   Fill image list
         terminal_output.print_terminal(
             string="Read images and calculate FOV, PIXEL scale, etc. ... ",
             indent=2,
-            )
-        for pd, file_name in enumerate(fileList):
+        )
+        for image_id, file_name in enumerate(fileList):
             self.image_list.append(
                 #   Prepare image class instance
-                self.image(pd, filt, obj_name, path, file_name, outdir)
-                )
+                self.image(image_id, filt, obj_name, path, file_name, outdir)
+            )
 
             #   Calculate field of view and additional quantities and add
             #   them to the image class instance
-            base_aux.cal_fov(self.image_list[pd], verbose=False)
+            base_aux.cal_fov(self.image_list[image_id], verbose=False)
 
         #   Set reference image
         self.ref_img = self.image_list[ref_ID]
 
         #   Set field of view
         self.fov = self.ref_img.fov
 
@@ -265,25 +305,25 @@
         #   Get image shape
         self.img_shape = self.ref_img.get_data().shape
 
     #   Image class
     class image:
         def __init__(self, pd, filt, obj_name, path, file_name, outdir):
             #   Set image ID
-            self.pd       = pd
+            self.pd = pd
             #   Set filter
-            self.filt     = filt
+            self.filt = filt
             #   Set object name
-            self.objname  = obj_name
+            self.objname = obj_name
             #   Set file name
             self.filename = file_name
             #   Set complete path
-            self.path     = Path(Path(path) / file_name)
+            self.path = Path(Path(path) / file_name)
             #   Set path to output directory
-            self.outpath  = Path(outdir)
+            self.outpath = Path(outdir)
 
         #   Read image
         def read_image(self):
             return CCDData.read(self.path)
 
         #   Get header
         def get_header(self):
@@ -359,15 +399,15 @@
 
         return np.median(obs_time_list)
 
     #   Get list with dictionary and image class objects
     def get_list_dict(self):
         dict_list = []
         for img in self.image_list:
-            dict_list.append({img.filt:img})
+            dict_list.append({img.filt: img})
 
         return dict_list
 
 
 def rm_cosmic(image, objlim=5., readnoise=8., sigclip=4.5, satlevel=65535.,
               verbose=False, addmask=True):
     '''
@@ -401,67 +441,67 @@
             Default is ``False``.
 
         addmask         : `boolean`, optional
             If True add hot and bad pixel mask to the reduced science images.
             Default is ``True``.
     '''
     terminal_output.print_terminal(
-        #indent=1,
+        # indent=1,
         string="Remove cosmic rays ...",
-        )
+    )
 
     #   Get image
     ccd = image.read_image()
 
     #   Get status cosmic ray removal status
     status = ccd.meta.get('cosmics_rm', False)
 
     #   Get unit of the image to check if the image was scaled with the
     #   exposure time
     if ccd.unit == u.electron / u.s:
-        scaled   = True
+        scaled = True
         exposure = ccd.meta.get('exptime', 1.)
-        reduced  = ccd.multiply(exposure * u.second)
+        reduced = ccd.multiply(exposure * u.second)
     else:
-        scaled  = False
+        scaled = False
         reduced = ccd
 
     if not status:
         #   Remove cosmic rays
         reduced = ccdp.cosmicray_lacosmic(
             reduced,
             objlim=objlim,
             readnoise=readnoise,
             sigclip=sigclip,
             satlevel=satlevel,
             verbose=verbose,
-            )
+        )
         if not addmask:
             reduced.mask = np.zeros(reduced.shape, dtype=bool)
         if verbose:
             terminal_output.print_terminal()
 
         #   Add Header keyword to mark the file as combined
         reduced.meta['cosmics_rm'] = True
 
         #   Reapply scaling if image was scaled with the exposure time
         if scaled:
-            reduced  = reduced.divide(exposure * u.second)
+            reduced = reduced.divide(exposure * u.second)
 
         #   Set file name
-        basename  = base_aux.get_basename(image.filename)
-        file_name = basename+'_cosmic-rm.fit'
+        basename = base_aux.get_basename(image.filename)
+        file_name = basename + '_cosmic-rm.fit'
 
         #   Set new file name and path
         image.filename = file_name
-        image.path     = os.path.join(
+        image.path = os.path.join(
             str(image.outpath),
             'cosmics_rm',
             file_name,
-            )
+        )
 
         #   Check if the 'cosmics_rm' directory already exits.
         #   If not, create it.
         checks.check_out(os.path.join(str(image.outpath), 'cosmics_rm'))
 
         #   Save image
         reduced.write(image.path, overwrite=True)
@@ -495,37 +535,37 @@
             Default is ``False``.
     '''
     if verbose:
         terminal_output.print_terminal(
             image.filt,
             string="Determine background: {:s} band",
             indent=2,
-            )
+        )
 
     #   Load image data
-    img    = image.read_image()
+    img = image.read_image()
 
     #   Set up sigma clipping
     sigma_clip = SigmaClip(sigma=sigma_bkg)
 
     #   Calculate background RMS
-    bkgrms        = MADStdBackgroundRMS(sigma_clip=sigma_clip)
+    bkgrms = MADStdBackgroundRMS(sigma_clip=sigma_clip)
     image.std_rms = bkgrms(img.data)
 
     #   2D background?
     if D2:
         #   Estimate 2D background
         bkg_estimator = MedianBackground()
         bkg = Background2D(
             img.data,
             (50, 50),
             filter_size=(3, 3),
             sigma_clip=sigma_clip,
             bkg_estimator=bkg_estimator,
-            )
+        )
 
         #   Remove background
         img_no_bg = img.subtract(bkg.background * u.electron / u.s)
 
         #   Put meta data back on the image, because it is lost while
         #   subtracting the background
         img_no_bg.meta = img.meta
@@ -534,44 +574,42 @@
         #   Add Header keyword to mark the file as background subtracted
         img_no_bg.meta['NO_BG'] = True
 
         #   Get median of the background
         bkg_value = bkg.background_median
     else:
         #   Estimate 1D background
-        mmm_bkg    = MMMBackground(sigma_clip=sigma_clip)
-        bkg_value  = mmm_bkg.calc_background(img.data)
+        mmm_bkg = MMMBackground(sigma_clip=sigma_clip)
+        bkg_value = mmm_bkg.calc_background(img.data)
 
         #   Remove background
         img_no_bg = img.subtract(bkg_value)
 
         #   Put meta data back on the image, because it is lost while
         #   subtracting the background
-        img_no_bg.meta = img_meta
+        img_no_bg.meta = image.meta
         img_no_bg.meta['HIERARCH'] = '1D background removed'
 
         #   Add Header keyword to mark the file as background subtracted
         img_no_bg.meta['NO_BG'] = True
 
-
     #   Define name and save image
-    file_name = base_aux.get_basename(image.filename)+'_nobg.fit'
+    file_name = base_aux.get_basename(image.filename) + '_nobg.fit'
     outpath = image.outpath / 'nobg'
     checks.check_out(outpath)
     img_no_bg.write(outpath / file_name, overwrite=True)
 
-
     #   Set new path and file
     #   -> Background subtracted image will be used in further processing steps
     if apply_background:
-        image.path     = outpath / file_name
+        image.path = outpath / file_name
         image.filename = file_name
 
     #   Add background value to image class
-    image.bkg_value  = bkg_value
+    image.bkg_value = bkg_value
 
 
 def find_stars(image, sigma_psf, multi_start=5., method='IRAF',
                verbose=False, condense=False, indent=2):
     '''
         Find the stars on the images, using photutils and search and select
         stars for the ePSF stars
@@ -611,51 +649,51 @@
         outstring       : `string`, optional
             Information to be printed to the terminal
     '''
     outstring = terminal_output.print_terminal(
         indent=indent,
         string="Identify stars",
         condense=condense,
-        )
+    )
 
     #   Load image data
     img = image.read_image()
 
     #   Get background RMS
     sigma = image.std_rms
 
     #   Distinguish between different finder options
     if method == 'DAO':
         #   Set up DAO finder
         daofind = DAOStarFinder(
-            fwhm=sigma_psf*gaussian_sigma_to_fwhm,
-            threshold=multi_start*sigma
-            )
+            fwhm=sigma_psf * gaussian_sigma_to_fwhm,
+            threshold=multi_start * sigma
+        )
 
         #   Find stars - make table
         tbl_posi_all = daofind(img.data)
     elif method == 'IRAF':
         #   Set up IRAF finder
         iraffind = IRAFStarFinder(
-                threshold=multi_start*sigma,
-                fwhm=sigma_psf*gaussian_sigma_to_fwhm,
-                minsep_fwhm=0.01,
-                roundhi=5.0,
-                roundlo=-5.0,
-                sharplo=0.0,
-                sharphi=2.0,
-                )
+            threshold=multi_start * sigma,
+            fwhm=sigma_psf * gaussian_sigma_to_fwhm,
+            minsep_fwhm=0.01,
+            roundhi=5.0,
+            roundlo=-5.0,
+            sharplo=0.0,
+            sharphi=2.0,
+        )
 
         #   Find stars - make table
         tbl_posi_all = iraffind(img.data)
     else:
         raise RuntimeError(
             f"{style.bcolors.FAIL}\nExtraction method ({method}) not valid: "
             f"use either IRAF or DAO {style.bcolors.ENDC}"
-            )
+        )
 
     #   Add positions to image class
     image.positions = tbl_posi_all
 
     if condense:
         return outstring
 
@@ -706,139 +744,138 @@
     #   Number of objects
     num_stars = len(tbl)
 
     #   Get image data
     data = image.get_data()
 
     #   Combine identification string
-    istring = str(image.pd)+'. '+image.filt
+    istring = str(image.pd) + '. ' + image.filt
 
     #   Useful information
     outstring = terminal_output.print_terminal(
         num_stars,
         istring,
-        indent=indent+1,
+        indent=indent + 1,
         string="{:d} sources identified in the {:s} band image",
         style_name='OKBLUE',
         condense=condense,
-        )
+    )
 
     ##  Determine sample of stars used for estimating the ePSF
     #   (rm the brightest 1% of all stars because those are often saturated)
     #   Sort list with star positions according to flux
     tbl_sort = tbl.group_by('flux')
     # Determine the 99 percentile
-    p99=np.percentile(tbl_sort['flux'], 99)
+    p99 = np.percentile(tbl_sort['flux'], 99)
     #   Determine the position of the 99 percentile in the position list
-    id_p99=np.argmin(np.absolute(tbl_sort['flux']-p99))
+    id_p99 = np.argmin(np.absolute(tbl_sort['flux'] - p99))
 
     #   Based on the input list, set the minimal number of stars
-    frac=int(num_stars*frac_epsf)
+    frac = int(num_stars * frac_epsf)
     #   If the minimal number of stars ('frac') is lower than 'min_stars'
     #   set it to 'min_stars' (the default is 25 as required by the cutout
     #   plots, 25 also appears to be reasonable for a good ePSF)
     if frac < min_stars:
         frac = min_stars
 
     #   Check if enough stars have been identified
-    if (id_p99-frac < min_stars and strict) or (id_p99-frac<1 and not strict):
+    if (id_p99 - frac < min_stars and strict) or (id_p99 - frac < 1 and not strict):
         raise RuntimeError(
-            f"{style.bcolors.FAIL} \nNot enough stars ({id_p99-frac}) found "
+            f"{style.bcolors.FAIL} \nNot enough stars ({id_p99 - frac}) found "
             f"to determine the ePSF in the {istring} band{style.bcolors.ENDC}"
-            )
+        )
 
     #   Resize table -> limit it to the suitable stars
-    tbl_posi = tbl_sort[:][id_p99-frac:id_p99]
+    tbl_posi = tbl_sort[:][id_p99 - frac:id_p99]
 
     ##  Exclude stars that are too close to the image boarder
     #   Size of the extraction box around each star
     hsize = (size - 1) / 2
 
     #   New lists with x and y positions
     x = tbl_posi['xcentroid']
     y = tbl_posi['ycentroid']
 
-    mask = ((x > hsize) & (x < (data.shape[1] -1 - hsize)) &
-            (y > hsize) & (y < (data.shape[0] -1 - hsize)))
+    mask = ((x > hsize) & (x < (data.shape[1] - 1 - hsize)) &
+            (y > hsize) & (y < (data.shape[0] - 1 - hsize)))
 
     #   Updated positions table
-    tbl_posi  = tbl_posi[:][mask]
+    tbl_posi = tbl_posi[:][mask]
     num_clean = len(tbl_posi)
 
     #   Check if there are still enough stars
-    if (num_clean < min_stars and strict) or (num_clean<1 and not strict):
+    if (num_clean < min_stars and strict) or (num_clean < 1 and not strict):
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nNot enough stars ({num_clean}) for the "
             f"ePSF determination in the {istring} band image. Too many "
             "potential ePSF stars have been removed, because they are too "
             "close to the image border. Check first that enough stars have "
             "been identified, using the starmap_?.pdf files.\n If that is "
             "the case, shrink extraction region or allow for higher fraction "
             "of ePSF stars (size_epsf) from all identified stars "
             f"(frac_epsf_stars). {style.bcolors.ENDC}"
-            )
-
+        )
 
     ##  Find all potential ePSF stars with close neighbors
     dist_min = size
 
     #   Define and fill new arrays
     x1 = tbl_sort['xcentroid']
     y1 = tbl_sort['ycentroid']
     x2 = tbl_posi['xcentroid']
     y2 = tbl_posi['ycentroid']
-    nmax = np.max((len(x1),len(x2)))
-    xall = np.zeros((nmax,2))
-    yall = np.zeros((nmax,2))
-    xall[0:len(x1),0] = x1
-    xall[0:len(x2),1] = x2
-    yall[0:len(y1),0] = y1
-    yall[0:len(y2),1] = y2
+    nmax = np.max((len(x1), len(x2)))
+    xall = np.zeros((nmax, 2))
+    yall = np.zeros((nmax, 2))
+    xall[0:len(x1), 0] = x1
+    xall[0:len(x2), 1] = x2
+    yall[0:len(y1), 0] = y1
+    yall[0:len(y2), 1] = y2
 
     id_p99 = correlate.newsrcor(
         xall,
         yall,
         dist_min,
         option=3,
         silent=True,
-        )[1]
+    )[1]
 
     #   Determine multiple entries -> stars that are contaminated
-    id_p99_mult = [ite for ite,count in Counter(id_p99).items() if count>1]
+    id_p99_mult = [ite for ite, count in Counter(id_p99).items() if count > 1]
     num_spoiled = len(id_p99_mult)
 
     #   Determine unique entries -> stars that are not contaminated
-    id_p99_uniq = [ite for ite,count in Counter(id_p99).items() if count==1]
-    num_clean   = len(id_p99_uniq)
+    id_p99_uniq = [ite for ite, count in Counter(id_p99).items() if count == 1]
+    num_clean = len(id_p99_uniq)
 
     #   Remove ePSF stars with close neighbors from the corresponding table
     tbl_posi.remove_rows(id_p99_mult)
 
     #   Check if there are still enough stars
-    if (num_clean < min_stars and strict) or (num_clean<1 and not strict):
+    if (num_clean < min_stars and strict) or (num_clean < 1 and not strict):
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nNot enough stars ({num_clean}) for the "
             f"ePSF determination in the {istring} band image. Too many "
             "potential ePSF stars have been removed, because other "
             "stars are in the extraction region. Check first that enough "
             "stars have been identified, using the starmap_?.pdf files.\n"
             "If that is the case, shrink extraction region or allow for "
             "higher fraction of ePSF stars (size_epsf) from all identified "
             f"stars (frac_epsf_stars). {style.bcolors.ENDC}"
-            )
+        )
 
     #   Add ePSF stars to image class
     image.positions_epsf = tbl_posi
 
     if condense:
         return outstring
 
 
 def mk_epsf(image, size=25, oversampling=2, maxiters=7,
-                min_stars=25, multi=True, condense=False, indent=2):
+            min_stars=25, multi=True, condense=False, indent=2):
     '''
         Main function to determine the ePSF, using photutils
 
         Parameters
         ----------
         image           : `image.class`
             Image class with all image specific properties
@@ -880,95 +917,94 @@
     #   Get image data
     data = image.get_data()
 
     #   Get ePSF star positions
     tbl_posi = image.positions_epsf
 
     #   Number of ePSF stars
-    num_fit =  len(tbl_posi)
+    num_fit = len(tbl_posi)
 
     #   Get object name
     nameobj = image.objname
 
     outstring = terminal_output.print_terminal(
-            indent=indent,
-            string="Determine the point spread function",
-            condense=condense,
-            )
+        indent=indent,
+        string="Determine the point spread function",
+        condense=condense,
+    )
     outstring = terminal_output.print_terminal(
-            num_fit,
-            indent=indent+1,
-            string="{:d} bright stars used",
-            style_name='OKBLUE',
-            condense=condense,
-            )
-
+        num_fit,
+        indent=indent + 1,
+        string="{:d} bright stars used",
+        style_name='OKBLUE',
+        condense=condense,
+    )
 
     #   Create new table with the names required by "extract_stars"
     stars_tbl = Table()
     stars_tbl['x'] = tbl_posi['xcentroid']
     stars_tbl['y'] = tbl_posi['ycentroid']
 
     #   Put image into NDData container (required by "extract_stars")
     nddata = NDData(data=data)
 
     #   Extract cutouts of the selected stars
     stars = extract_stars(nddata, stars_tbl, size=size)
 
     #   Combine plot identification string
-    string = 'img-'+str(image.pd)+'-'+image.filt
+    string = 'img-' + str(image.pd) + '-' + image.filt
 
     #   Get output directory
     outdir = image.outpath.name
 
     #   Plot the brightest ePSF stars
     if multi:
         p = mp.Process(
             target=plot.plot_cutouts,
             args=(outdir, stars, string),
-            kwargs={'nameobj':nameobj,}
-            )
+            kwargs={'nameobj': nameobj, }
+        )
         p.start()
     else:
         if condense:
             tmpstr = plot.plot_cutouts(
                 outdir,
                 stars,
                 string,
                 nameobj=nameobj,
                 condense=True,
-                )
+            )
             outstring += tmpstr
         else:
             plot.plot_cutouts(
                 outdir,
                 stars,
                 string,
                 max_plot_stars=min_stars,
                 nameobj=nameobj,
-                )
+            )
 
     #   Build the ePSF (set oversampling and max. number of iterations)
     epsf_builder = EPSFBuilder(
         oversampling=oversampling,
         maxiters=maxiters,
         progress_bar=False,
-        )
+    )
     epsf, fitted_stars = epsf_builder(stars)
 
     #   Add ePSF and fitted stars to image class
-    image.epsf         = epsf
+    image.epsf = epsf
     image.fitted_stars = fitted_stars
 
     if condense:
-    	return outstring
+        return outstring
 
 
 def epsf_extract(image, sigma_psf, sigma_bkg=5., use_init_guesses=True,
-                 method_finder='IRAF', size_epsf=25.,  multi=5.0,
+                 method_finder='IRAF', size_epsf=25., multi=5.0,
                  multi_grouper=2.0, strict_cleaning=True, condense=False,
                  rmbackground=False, indent=2):
     '''
         Main function to perform the eEPSF photometry, using photutils
 
         Parameters
         ----------
@@ -1027,250 +1063,249 @@
     #   Get output path
     out_path = image.outpath
 
     #   Check output directories
     checks.check_out(
         out_path,
         out_path / 'tables',
-        )
+    )
 
     #   Get image data
     data = image.get_data()
 
     #   Get filter
     filt = image.filt
 
     #   Get already identified objects (position and flux)
     if use_init_guesses:
         try:
             #   Get position information
             positions_flux = image.positions
             init_guesses = Table(
-                names=['x_0','y_0', 'flux_0'],
+                names=['x_0', 'y_0', 'flux_0'],
                 data=[
                     positions_flux['xcentroid'],
                     positions_flux['ycentroid'],
                     positions_flux['flux'],
-                    ]
-                )
+                ]
+            )
         except:
             #   Switch to backup in case positions and fluxes are not
             #   available
-            use_init_guesses=False
+            use_init_guesses = False
 
     #   Set output and plot identification string
-    istring = str(image.pd)+'-'+filt
+    istring = str(image.pd) + '-' + filt
 
     #   Get background RMS
     sigma = image.std_rms
 
     #   Get ePSF
     epsf = image.epsf
 
     outstr = terminal_output.print_terminal(
-            istring,
-            indent=indent,
-            string="Performing the actual PSF photometry ({:s} image)",
-            condense=condense,
-            )
+        istring,
+        indent=indent,
+        string="Performing the actual PSF photometry ({:s} image)",
+        condense=condense,
+    )
 
     ##  Set up all necessary classes
     if method_finder == 'IRAF':
         #   IRAF finder
         finder = IRAFStarFinder(
-            threshold=multi*sigma,
-            fwhm=sigma_psf*gaussian_sigma_to_fwhm,
+            threshold=multi * sigma,
+            fwhm=sigma_psf * gaussian_sigma_to_fwhm,
             minsep_fwhm=0.01,
             roundhi=5.0,
             roundlo=-5.0,
             sharplo=0.0,
             sharphi=2.0,
-            )
+        )
     elif method_finder == 'DAO':
         #   DAO finder
         finder = DAOStarFinder(
-            fwhm=sigma_psf*gaussian_sigma_to_fwhm,
-            threshold=multi*sigma,
+            fwhm=sigma_psf * gaussian_sigma_to_fwhm,
+            threshold=multi * sigma,
             exclude_border=True,
-            )
+        )
     else:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nExtraction method ({method_finder}) "
             f"not valid: use either IRAF or DAO {style.bcolors.ENDC}"
-            )
+        )
     #   Fitter used
     fitter = LevMarLSQFitter()
 
     #   Size of the extraction region
     if size_epsf % 2 == 0:
         sizepho = size_epsf + 1
     else:
         sizepho = size_epsf
 
     #   Number of iterations
-    niter=1
+    niter = 1
 
     #   Set up sigma clipping
     if rmbackground:
         sigma_clip = SigmaClip(sigma=sigma_bkg)
-        mmm_bkg    = MMMBackground(sigma_clip=sigma_clip)
+        mmm_bkg = MMMBackground(sigma_clip=sigma_clip)
     else:
         mmm_bkg = None
 
     try:
         #   DAO grouper
-        daogroup = DAOGroup(multi_grouper*sigma_psf*gaussian_sigma_to_fwhm)
+        daogroup = DAOGroup(multi_grouper * sigma_psf * gaussian_sigma_to_fwhm)
 
         #  Set up the overall class to extract the data
         photometry = IterativelySubtractedPSFPhotometry(
             finder=finder,
             group_maker=daogroup,
             bkg_estimator=mmm_bkg,
             psf_model=epsf,
             fitter=fitter,
             niters=niter,
             fitshape=(sizepho, sizepho),
-            aperture_radius=(sizepho-1)/2
-            )
+            aperture_radius=(sizepho - 1) / 2
+        )
 
         #   Extract the photometry and make a table
         if use_init_guesses:
             result_tbl = photometry(image=data, init_guesses=init_guesses)
         else:
             result_tbl = photometry(image=data)
     except RuntimeError as e:
         if multi_grouper != 1.:
             terminal_output.print_terminal(
                 indent=indent,
                 string="IterativelySubtractedPSFPhotometry failed. " \
                        "Will try again with 'multi_grouper' set to 1...",
                 style_name='WARNING',
-                )
+            )
             multi_grouper = 1.
             #   DAO grouper
             daogroup = DAOGroup(
-                multi_grouper*sigma_psf*gaussian_sigma_to_fwhm
-                )
+                multi_grouper * sigma_psf * gaussian_sigma_to_fwhm
+            )
 
             #  Set up the overall class to extract the data
             photometry = IterativelySubtractedPSFPhotometry(
                 finder=finder,
                 group_maker=daogroup,
                 bkg_estimator=mmm_bkg,
                 psf_model=epsf,
                 fitter=fitter,
                 niters=niter,
                 fitshape=(sizepho, sizepho),
-                aperture_radius=(sizepho-1)/2
-                )
+                aperture_radius=(sizepho - 1) / 2
+            )
 
             #   Extract the photometry and make a table
             if use_init_guesses:
                 result_tbl = photometry(image=data, init_guesses=init_guesses)
             else:
                 result_tbl = photometry(image=data)
         else:
             terminal_output.print_terminal(
                 indent=0,
                 string=e,
-                )
-            #print(e)
+            )
+            # print(e)
 
     #   Check if result table contains a 'flux_unc' column
     #   For some reason, it's missing for some extractions....
     if 'flux_unc' not in result_tbl.colnames:
         #   Calculate a very very rough approximation of the uncertainty
         #   by means of the actual extraction result 'flux_fit' and the
         #   early estimate 'flux_0'
         est_unc = np.absolute(
             result_tbl['flux_fit'] - result_tbl['flux_0']
-            )
+        )
         result_tbl.add_column(est_unc, name='flux_unc')
 
     #   Clean output for objects with negative uncertainties
     try:
-        num_spoiled  = 0
+        num_spoiled = 0
         spoiled_fits = np.where(result_tbl['flux_fit'].data < 0.)
         result_tbl.remove_rows(spoiled_fits)
-        num_spoiled  = np.size(spoiled_fits)
+        num_spoiled = np.size(spoiled_fits)
         if strict_cleaning:
             spoiled_fits = np.where(result_tbl['flux_unc'].data < 0.)
-            num_spoiled  += len(spoiled_fits)
+            num_spoiled += len(spoiled_fits)
             result_tbl.remove_rows(spoiled_fits)
     except:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nProblem with cleanup of negative "
             f"uncertainties... {style.bcolors.ENDC}"
-            )
+        )
 
     #   Clean output for objects with negative pixel coordinates
     try:
-        spoiled_fits  = np.where(result_tbl['x_fit'].data < 0.)
-        num_spoiled  += np.size(spoiled_fits)
+        spoiled_fits = np.where(result_tbl['x_fit'].data < 0.)
+        num_spoiled += np.size(spoiled_fits)
         result_tbl.remove_rows(spoiled_fits)
-        spoiled_fits  = np.where(result_tbl['y_fit'].data < 0.)
-        num_spoiled  += np.size(spoiled_fits)
+        spoiled_fits = np.where(result_tbl['y_fit'].data < 0.)
+        num_spoiled += np.size(spoiled_fits)
         result_tbl.remove_rows(spoiled_fits)
     except:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nProblem with cleanup of negative pixel "
             f"coordinates... {style.bcolors.ENDC}"
-            )
+        )
 
     if num_spoiled != 0:
         strout = terminal_output.print_terminal(
-                num_spoiled,
-                indent=indent+1,
-                string="{:d} objects removed because of poor fit quality",
-                condense=condense,
-                )
+            num_spoiled,
+            indent=indent + 1,
+            string="{:d} objects removed because of poor fit quality",
+            condense=condense,
+        )
         if condense: outstr += strout
 
     try:
         nstars = len(result_tbl['flux_fit'].data)
     except:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nTable produced by "
             "IterativelySubtractedPSFPhotometry is empty after cleaning up "
             "of objects with negative pixel coordinates and negative "
             f"uncertainties {style.bcolors.ENDC}"
-            )
+        )
 
     strout = terminal_output.print_terminal(
-            nstars,
-            indent=indent+1,
-            string="{:d} good stars extracted from the image",
-            style_name='OKBLUE',
-            condense=condense,
-            )
+        nstars,
+        indent=indent + 1,
+        string="{:d} good stars extracted from the image",
+        style_name='OKBLUE',
+        condense=condense,
+    )
     if condense: outstr += strout
 
-
     #   Remove objects that are too close to the image edges
     result_tbl, strout = aux.rm_edge_objects(
         result_tbl,
         data,
-        (sizepho-1)/2,
+        (sizepho - 1) / 2,
         condense=condense,
-        )
+    )
     if condense: outstr += strout
 
     #   Write table
     filename = 'table_photometry_{}_PSF.dat'.format(istring)
     result_tbl.write(
         out_path / 'tables' / filename,
         format='ascii',
         overwrite=True,
-        )
+    )
 
     #  Make residual image
     residual_image = photometry.get_residual_image()
 
     #   Add photometry and residual image to image class
-    image.photometry     = result_tbl
+    image.photometry = result_tbl
     image.residual_image = residual_image
 
     if condense:
         return outstr
 
 
 def compute_phot_error(flux_variance, ap_area, nsky, stdev, gain=1.0):
@@ -1304,15 +1339,15 @@
         gain               : `float`, optional
             Electrons per ADU
             Default is ``1.0``. Usually we already work with gain corrected
             data.
     '''
 
     #   Calculate flux error as above
-    bg_variance_terms = (ap_area * stdev ** 2. ) * (1. + ap_area/nsky)
+    bg_variance_terms = (ap_area * stdev ** 2.) * (1. + ap_area / nsky)
     variance = flux_variance / gain + bg_variance_terms
     flux_error = variance ** .5
 
     return flux_error
 
 
 def define_apertures(image, r, r_in, r_out, r_unit):
@@ -1351,30 +1386,30 @@
     #   Extract positions and prepare a position list
     try:
         lst1 = tbl['x_fit']
         lst2 = tbl['y_fit']
     except:
         lst1 = tbl['xcentroid']
         lst2 = tbl['ycentroid']
-    positions = list(zip(lst1,lst2))
+    positions = list(zip(lst1, lst2))
 
     #   Check unit of radii
     if r_unit not in ['pixel', 'arcsec']:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nUnit of the aperture radii not valid: "
             f"set it either to pixel or arcsec {style.bcolors.ENDC}"
-            )
+        )
 
     #   Convert radii in arcsec to pixel
     #   (this part is prone to errors and needs to be rewritten)
     pixscale = image.pixscale
     if pixscale != None and r_unit == 'arcsec':
-        r     = r/pixscale
-        r_in  = r_in/pixscale
-        r_out = r_out/pixscale
+        r = r / pixscale
+        r_in = r_in / pixscale
+        r_out = r_out / pixscale
 
     #   Make stellar aperture
     aperture = CircularAperture(positions, r=r)
 
     #   Make background annulus
     annulus_aperture = CircularAnnulus(positions, r_in=r_in, r_out=r_out)
 
@@ -1398,15 +1433,15 @@
         bkg_median          : `float`
             Median of the background
 
         bkg_stdev           : `float`
             Standard deviation of the background
     '''
     bkg_median = []
-    bkg_stdev  = []
+    bkg_stdev = []
 
     #   Calculate mask from background annulus
     annulus_masks = annulus_aperture.to_mask(method='center')
 
     #   Loop over all masks
     for mask in annulus_masks:
         #   Extract annulus data
@@ -1420,15 +1455,15 @@
 
         #   Add to list
         bkg_median.append(median_sigclip)
         bkg_stdev.append(median_stdev)
 
     #   Convert to numpy array
     bkg_median = np.array(bkg_median)
-    bkg_stdev  = np.array(bkg_stdev)
+    bkg_stdev = np.array(bkg_stdev)
 
     return bkg_median, bkg_stdev
 
 
 def aperture_extract(image, r, r_in, r_out, r_unit='pixel', bg_simple=False,
                      plotaper=False, condense=False, indent=2):
     '''
@@ -1478,69 +1513,66 @@
         outstring       : `string`, optional
             Information to be printed to the terminal
 
             img_err     - numpy.ndarray or None
                           Error array for 'image'
     '''
     #   Load image data and uncertainty
-    img  = image.read_image()
+    img = image.read_image()
     data = img.data
-    err  = img.uncertainty.array
+    err = img.uncertainty.array
 
     #   Get filter
     filt = image.filt
 
     outstr = terminal_output.print_terminal(
         filt,
         indent=indent,
         string="Performing aperture photometry ({:s} image)",
         condense=condense,
-        )
-
+    )
 
     ###
     #   Define apertures
     #
     aperture, annulus_aperture = define_apertures(
         image,
         r,
         r_in,
         r_out,
         r_unit,
-        )
-
+    )
 
     ###
     #   Extract background and calculate median
     #
     if bg_simple:
         bkg_median, bkg_stdev = background_simple(image, annulus_aperture)
 
-
     ###
     #   Extract photometry
     #
     #   Extract aperture
     phot = aperture_photometry(data, aperture, mask=img.mask, error=err)
 
     #   Extract background aperture
     if not bg_simple:
         bkg_phot = aperture_photometry(
             data,
             annulus_aperture,
             mask=img.mask,
             error=err,
-            )
+        )
 
         #   Calculate aperture background and the corresponding error
         phot['aper_bkg'] = bkg_phot['aperture_sum'] * aperture.area \
-                        / annulus_aperture.area
+                           / annulus_aperture.area
 
         phot['aper_bkg_err'] = bkg_phot['aperture_sum_err'] * aperture.area \
-                        / annulus_aperture.area
+                               / annulus_aperture.area
     else:
         #   Add median background to the output table
         phot['annulus_median'] = bkg_median
 
         #   Calculate background for the apertures add to the output table
         phot['aper_bkg'] = bkg_median * aperture.area
 
@@ -1553,27 +1585,27 @@
     #   photometry)
     phot['flux_fit'] = phot['aper_sum_bkgsub']
 
     # Error estimate
     if err is not None:
         err_column = phot['aperture_sum_err']
     else:
-        err_column = phot['flux_fit']**(0.5)
+        err_column = phot['flux_fit'] ** (0.5)
 
     if bg_simple:
         bg_err = bkg_stdev
     else:
         bg_err = phot['aper_bkg_err']
 
     phot['flux_unc'] = compute_phot_error(
         err_column,
         aperture.area,
         annulus_aperture.area,
         bg_err,
-        )
+    )
 
     #   Rename position columns
     phot.rename_column('xcenter', 'x_fit')
     phot.rename_column('ycenter', 'y_fit')
 
     #   Remove objects that are too close to the image edges
     phot, strout = aux.rm_edge_objects(phot, data, r_out, condense=condense)
@@ -1585,54 +1617,53 @@
     flux = np.array(phot['flux_fit'])
     mask = np.where(flux <= 0.)
     phot['flux_fit'][mask] = 1E-10
 
     #   Add photometry to image class
     image.photometry = phot
 
-
     ###
     #   Plot star map with aperture overlay
     #
     if plotaper:
         plot.plot_apertures(
             image.outpath.name,
             data,
             aperture,
             annulus_aperture,
             filt,
-            )
+        )
 
     #   Number of stars
     nstars = len(flux)
 
     #   Useful info
     strout = terminal_output.print_terminal(
         nstars,
-        indent=indent+1,
+        indent=indent + 1,
         string="{:d} good stars extracted from the image",
         style_name='OKBLUE',
         condense=condense,
-        )
+    )
 
-    if condense: return outstr+strout
+    if condense: return outstr + strout
 
 
 def correlate_images(*args, **kwargs):
     '''
         Wrapper function: distinguish between astropy table
                           and pandas data frame
     '''
     if base_aux.dict_vs_df(args[1]):
         return correlate_pd(*args, **kwargs)
     else:
         return correlate_tbl(*args, **kwargs)
 
 
-#@timeis
+# @timeis
 def correlate_tbl(outdir, result_tbl, arr_img_IDs, dcr=3., option=1,
                   maxid=1, refORI=0, refOBJ=[], nmissed=1, bfrac=1.0,
                   s_refOBJ=True):
     '''
         WARNING: This function is not up to date
 
         Correlate star lists from the stacked images of all filters to find
@@ -1710,126 +1741,126 @@
         count               : `integer
             Number of matches found
     '''
     terminal_output.print_terminal(
         arr_img_IDs,
         indent=1,
         string="Correlate results from the images ({:s})",
-        )
+    )
 
     #   Define variables
-    nimg      = len(arr_img_IDs)
+    nimg = len(arr_img_IDs)
     nmax_list = []
     x = []
     y = []
 
     #   Number of objects in each table/image
     for i, img_ID in enumerate(arr_img_IDs):
         x.append(result_tbl[str(img_ID)]['x_fit'])
         y.append(result_tbl[str(img_ID)]['y_fit'])
         nmax_list.append(len(x[i]))
 
     #   Max. number of objects
     nmax = np.max(nmax_list)
 
     #   Define and fill new arrays
-    xall = np.zeros((nmax,nimg))
-    yall = np.zeros((nmax,nimg))
-    for i in range(0,nimg):
-        xall[0:len(x[i]),i] = x[i]
-        yall[0:len(y[i]),i] = y[i]
+    xall = np.zeros((nmax, nimg))
+    yall = np.zeros((nmax, nimg))
+    for i in range(0, nimg):
+        xall[0:len(x[i]), i] = x[i]
+        yall[0:len(y[i]), i] = y[i]
 
     #   Correlate the results from the two images
     indSR, reject, count, rej_obj = correlate.newsrcor(
         xall,
         yall,
         dcr,
         bfrac=bfrac,
         option=option,
         maxid=maxid,
         refORI=refORI,
         refOBJ=refOBJ,
         nmissed=nmissed,
         s_refOBJ=s_refOBJ,
-        )
+    )
 
     if count == 1:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nOnly one common object "
             f"found!{style.bcolors.ENDC}"
-            )
+        )
     elif count == 0:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nNo common objects "
             f"found!{style.bcolors.ENDC}"
-            )
+        )
 
     nbad = len(reject)
     if nbad > 0:
         terminal_output.print_terminal(
             nbad,
             indent=2,
             string="{:d} images do not meet the criteria -> removed",
-            )
+        )
 
     #   Remove bad origins listed in 'reject'
-    indSR       = np.delete(indSR, reject, 0)
+    indSR = np.delete(indSR, reject, 0)
     arr_img_IDs = np.delete(arr_img_IDs, reject, 0)
 
-    xall        = np.delete(xall, reject, 1)
-    yall        = np.delete(yall, reject, 1)
+    xall = np.delete(xall, reject, 1)
+    yall = np.delete(yall, reject, 1)
 
     #   Calculate shift for the reference origin
     shiftID = np.argwhere(reject < refORI)
-    Nshift  = len(shiftID)
+    Nshift = len(shiftID)
     refORI -= Nshift
 
     # Number of clean images
-    nclean = len(indSR[:,0])
+    nclean = len(indSR[:, 0])
 
     #   Rearrange arrays based on the newsrcor results
-    x_sort   = np.zeros((count))
-    y_sort   = np.zeros((count))
+    x_sort = np.zeros((count))
+    y_sort = np.zeros((count))
     ind_sort = np.arange(count)
 
-    for i in range(0,count):
-        x_sort[i]   = xall[indSR[refORI][i]][refORI]
-        y_sort[i]   = yall[indSR[refORI][i]][refORI]
+    for i in range(0, count):
+        x_sort[i] = xall[indSR[refORI][i]][refORI]
+        y_sort[i] = yall[indSR[refORI][i]][refORI]
 
     #   Array for the flux and uncertainty
     flux_arr = np.zeros(nclean, dtype=[('flux_fit', 'f8', (count)),
                                        ('flux_unc', 'f8', (count)),
-                                      ]
-                    )
+                                       ]
+                        )
 
     #   Fill arrays
     for j, img_ID in enumerate(arr_img_IDs):
         img_ID = str(img_ID)
 
         for i in range(0, count):
-            flux     = result_tbl[img_ID]['flux_fit'][indSR[j,i]]
-            flux_err = result_tbl[img_ID]['flux_unc'][indSR[j,i]]
+            flux = result_tbl[img_ID]['flux_fit'][indSR[j, i]]
+            flux_err = result_tbl[img_ID]['flux_unc'][indSR[j, i]]
             flux_arr['flux_fit'][j][i] = flux
             flux_arr['flux_unc'][j][i] = flux_err
 
     #   Remove nans
     flux_arr['flux_unc'] = np.nan_to_num(
         flux_arr['flux_unc'],
         nan=9999.,
         posinf=9999.,
         neginf=9999.,
-        )
+    )
 
     return ind_sort, x_sort, y_sort, flux_arr, reject, rej_obj, count
 
 
 def correlate_ensemble_img(img_ensemble, dcr=3., option=1, maxid=1,
                            refORI=0, refOBJ=[], nmissed=1, bfrac=1.0,
                            s_refOBJ=True, correl_method='astropy',
-                           seplimit=2.*u.arcsec):
+                           seplimit=2. * u.arcsec):
     '''
         Correlate star lists from the stacked images of all filters to find
         those stars that are visible on all images -> write calibrated CMD
 
         Parameters
         ----------
         img_ensemble        : `image ensemble`
@@ -1886,59 +1917,59 @@
     #   Get image IDs
     arr_img_IDs = img_ensemble.get_image_ids()
 
     terminal_output.print_terminal(
         arr_img_IDs,
         indent=1,
         string="Correlate results from the images ({})",
-        )
+    )
 
     #   Get WCS
     w = img_ensemble.wcs
 
     #   Get dictionary with astropy tables with the position and flux data
     result_tbl = img_ensemble.get_photometry()
 
     #   Number of images
-    nimg      = len(arr_img_IDs)
+    nimg = len(arr_img_IDs)
 
     #   Extract pixel positions of the objects -> needs to be improved!
     nmax_list = []
     x = []
     y = []
     for i, img_ID in enumerate(arr_img_IDs):
         x.append(result_tbl[str(img_ID)]['x_fit'])
         y.append(result_tbl[str(img_ID)]['y_fit'])
         nmax_list.append(len(x[i]))
 
     #   Max. number of objects
     nmax = np.max(nmax_list)
 
     #   Define and fill new arrays
-    xall = np.zeros((nmax,nimg))
-    yall = np.zeros((nmax,nimg))
+    xall = np.zeros((nmax, nimg))
+    yall = np.zeros((nmax, nimg))
 
-    for i in range(0,nimg):
-        xall[0:len(x[i]),i] = x[i]
-        yall[0:len(y[i]),i] = y[i]
+    for i in range(0, nimg):
+        xall[0:len(x[i]), i] = x[i]
+        yall[0:len(y[i]), i] = y[i]
 
     #   Correlate the object positions from the images
     #   -> find common objects
     if correl_method == 'astropy':
         #   Astropy version: 2x faster than own
         indSR, reject = correlate.astropycor(
             x,
             y,
             w,
             refORI=refORI,
             refOBJ=refOBJ,
             nmissed=nmissed,
             s_refOBJ=s_refOBJ,
             seplimit=seplimit,
-            )
+        )
         count = len(indSR[0])
 
     elif correl_method == 'own':
         #   Own version based on srcor from the IDL Astro Library
         indSR, reject, count, rej_obj = correlate.newsrcor(
             xall,
             yall,
@@ -1946,180 +1977,177 @@
             bfrac=bfrac,
             option=option,
             maxid=maxid,
             refORI=refORI,
             refOBJ=refOBJ,
             nmissed=nmissed,
             s_refOBJ=s_refOBJ,
-            )
+        )
     else:
         raise ValueError(
             f'{style.bcolors.FAIL}Correlation method not known. Expected: '
             f'"own" or astropy, but got "{correl_method}"{style.bcolors.ENDC}'
-            )
+        )
 
     ###
     #   Print correlation infos or raise error if not enough common
     #   objects were detected
     #
     if count == 1:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nOnly one common object "
             f"found! {style.bcolors.ENDC}"
-            )
+        )
     elif count == 0:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nNo common objects "
             f"found!{style.bcolors.ENDC}"
-            )
+        )
     else:
         terminal_output.print_terminal(
             count,
             indent=2,
             string="{} objects identified on all images",
-            )
+        )
 
     nbad = len(reject)
     if nbad > 0:
         terminal_output.print_terminal(
             nbad,
             indent=2,
             string="{:d} images do not meet the criteria -> removed",
-            )
+        )
     if nbad > 1:
         terminal_output.print_terminal(
             reject,
             indent=2,
             string="Rejected image IDs: {}",
-            )
+        )
     elif nbad == 1:
         terminal_output.print_terminal(
             reject,
             indent=2,
             string="ID of the rejected image: {}",
-            )
+        )
     terminal_output.print_terminal()
 
-
     ###
     #   Post process corelation results
     #
 
     #   Remove "bad" datasets from index array
     #   (only necessary for 'own' method)
     if correl_method == 'own':
-        indSR       = np.delete(indSR, reject, 0)
+        indSR = np.delete(indSR, reject, 0)
 
     # Number of "clean" datasets
-    nclean = len(indSR[:,0])
+    nclean = len(indSR[:, 0])
 
     #   Remove "bad" datasets from image IDs -> used in a later step
     arr_img_IDs = np.delete(arr_img_IDs, reject, 0)
 
     #   Calculate new index of the reference origin
     shiftID = np.argwhere(reject < refORI)
-    Nshift  = len(shiftID)
-    refORI_new = refORI-Nshift
-
+    Nshift = len(shiftID)
+    refORI_new = refORI - Nshift
 
     ###
     #   Rearrange arrays based on the correlation results
     #
     #   Prepare new arrays for positions and indexes
-    x_sort   = np.zeros((count))
-    y_sort   = np.zeros((count))
+    x_sort = np.zeros((count))
+    y_sort = np.zeros((count))
     ind_sort = np.arange(count)
 
     #   Fill position arrays -> distinguish between input sources
     #                           depending on correlation method
     if correl_method == 'astropy':
         x_sort = x[refORI][indSR[refORI_new]].value
         y_sort = y[refORI][indSR[refORI_new]].value
 
     elif correl_method == 'own':
         #   Remove "bad" datasets first
-        xall        = np.delete(xall, reject, 1)
-        yall        = np.delete(yall, reject, 1)
+        xall = np.delete(xall, reject, 1)
+        yall = np.delete(yall, reject, 1)
 
-        x_sort = xall[indSR[refORI_new]][:,refORI_new]
-        y_sort = yall[indSR[refORI_new]][:,refORI_new]
+        x_sort = xall[indSR[refORI_new]][:, refORI_new]
+        y_sort = yall[indSR[refORI_new]][:, refORI_new]
 
     #   Prepare array for the flux and uncertainty (all datasets)
     flux_arr = np.zeros(nclean, dtype=[('flux_fit', 'f8', (count)),
                                        ('flux_unc', 'f8', (count)),
-                                      ]
-                    )
+                                       ]
+                        )
 
     #   Fill flux arrays
     for j, img_ID in enumerate(arr_img_IDs):
         img_ID_str = str(img_ID)
 
         #   Flux and uncertainty array for individual images
         flux_img = np.zeros(
             count,
             dtype=[('flux_fit', 'f8'), ('flux_unc', 'f8')],
-            )
+        )
 
         #   Rearrange flux and error
-        flux_img['flux_fit'] = result_tbl[img_ID_str]['flux_fit'][indSR[j,:]]
-        flux_img['flux_unc'] = result_tbl[img_ID_str]['flux_unc'][indSR[j,:]]
+        flux_img['flux_fit'] = result_tbl[img_ID_str]['flux_fit'][indSR[j, :]]
+        flux_img['flux_unc'] = result_tbl[img_ID_str]['flux_unc'][indSR[j, :]]
 
         #   Remove nans etc. in error
         flux_img['flux_unc'] = np.nan_to_num(
             flux_img['flux_unc'],
             nan=9999.,
             posinf=9999.,
             neginf=9999.,
-            )
+        )
 
         #   Remove '--' entries in error
         flux_err_dash = np.argwhere(flux_img['flux_unc'] == '--')
         flux_img['flux_unc'][flux_err_dash] = 9999.
 
         uflux_img = unumpy.uarray(
             flux_img['flux_fit'],
             flux_img['flux_unc']
-            )
+        )
 
         #   Add sorted flux data and positions back to the image
-        img_ensemble.image_list[img_ID].flux    = flux_img
-        img_ensemble.image_list[img_ID].uflux   = uflux_img
-        img_ensemble.image_list[img_ID].x_sort  = x_sort
-        img_ensemble.image_list[img_ID].y_sort  = y_sort
+        img_ensemble.image_list[img_ID].flux = flux_img
+        img_ensemble.image_list[img_ID].uflux = uflux_img
+        img_ensemble.image_list[img_ID].x_sort = x_sort
+        img_ensemble.image_list[img_ID].y_sort = y_sort
         img_ensemble.image_list[img_ID].id_sort = ind_sort
 
-
         #   Add to overall array
         flux_arr['flux_fit'][j] = flux_img['flux_fit']
         flux_arr['flux_unc'][j] = flux_img['flux_unc']
 
     uflux_arr = unumpy.uarray(
-            flux_arr['flux_fit'],
-            flux_arr['flux_unc']
-            )
+        flux_arr['flux_fit'],
+        flux_arr['flux_unc']
+    )
 
     #   Update image ensemble object and add IDs, pixel coordinates, and
     #   flux of the correlated objects
     img_list = img_ensemble.image_list
     img_list = np.delete(img_list, reject)
     img_ensemble.image_list = img_list
-    img_ensemble.nfiles     = len(img_list)
-    img_ensemble.ref_id     = refORI_new
+    img_ensemble.nfiles = len(img_list)
+    img_ensemble.ref_id = refORI_new
 
     img_ensemble.id_s = ind_sort
-    img_ensemble.x_s  = x_sort
-    img_ensemble.y_s  = y_sort
+    img_ensemble.x_s = x_sort
+    img_ensemble.y_s = y_sort
     img_ensemble.flux = flux_arr
     img_ensemble.uflux = uflux_arr
 
 
 def correlate_ensemble(img_container, filt_list, dcr=3., option=1, maxid=1,
                        refORI=0, refOBJ=[], nmissed=1, bfrac=1.0,
                        s_refOBJ=True, correl_method='astropy',
-                       seplimit=2.*u.arcsec):
+                       seplimit=2. * u.arcsec):
     '''
         Correlate star lists from the stacked images of all filters to find
         those stars that are visible on all images -> write calibrated CMD
 
         Parameters
         ----------
         img_container       : `image.container`
@@ -2175,15 +2203,15 @@
         seplimit            : `astropy.units`, optional
             Allowed separation between objects.
             Default is ``2.*u.arcsec``.
     '''
     terminal_output.print_terminal(
         indent=1,
         string="Correlate results from image ensembles",
-        )
+    )
 
     #   Get image ensembles
     ensemble_dict = img_container.get_ensembles(filt_list)
 
     #   Define variables
     nobj_list = []
     keys = []
@@ -2205,17 +2233,17 @@
     #   Number of ''images''/image ensembles
     nimg = len(x)
 
     #   Define and fill new arrays
     xall = np.zeros((nobj_max, nimg))
     yall = np.zeros((nobj_max, nimg))
 
-    for i in range(0,nimg):
-        xall[0:len(x[i]),i] = x[i]
-        yall[0:len(y[i]),i] = y[i]
+    for i in range(0, nimg):
+        xall[0:len(x[i]), i] = x[i]
+        yall[0:len(y[i]), i] = y[i]
 
     #   Correlate the object positions from the images
     #   -> find common objects
     if correl_method == 'astropy':
         #   Astropy version: ~2x faster than own
         indSR, reject = correlate.astropycor(
             x,
@@ -2223,15 +2251,15 @@
             w[refORI],
             refORI,
             refOBJ,
             nmissed,
             s_refOBJ,
             cleanup_advanced=False,
             seplimit=seplimit,
-            )
+        )
         count = len(indSR[0])
 
     elif correl_method == 'own':
         #   Own version based on srcor from the IDL Astro Library
         indSR, reject, count, rej_obj = correlate.newsrcor(
             xall,
             yall,
@@ -2239,64 +2267,63 @@
             bfrac=bfrac,
             option=option,
             maxid=maxid,
             refORI=refORI,
             refOBJ=refOBJ,
             nmissed=nmissed,
             s_refOBJ=s_refOBJ,
-            )
+        )
     else:
         raise ValueError(
             f'{style.bcolors.FAIL}Correlation method not known. Expected: '
             f'"own" or astropy, but got "{correl_method}"{style.bcolors.ENDC}'
-            )
+        )
 
     ###
     #   Print correlation infos or raise error if not enough common
     #   objects were detected
     #
     if count == 1:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nOnly one common object "
             f"found! {style.bcolors.ENDC}"
-            )
+        )
     elif count == 0:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nNo common objects "
             f"found!{style.bcolors.ENDC}"
-            )
+        )
     else:
         terminal_output.print_terminal(
             count,
             indent=2,
             string="{} objects identified on all ensemble",
-            )
+        )
 
     nbad = len(reject)
     if nbad > 0:
         terminal_output.print_terminal(
             nbad,
             indent=2,
             string="{:d} images do not meet the criteria -> removed",
-            )
+        )
     if nbad > 1:
         terminal_output.print_terminal(
             reject,
             indent=2,
             string="Rejected ensemble IDs: {}",
-            )
+        )
     elif nbad == 1:
         terminal_output.print_terminal(
             reject,
             indent=2,
             string="ID of the rejected ensembles: {}",
-            )
+        )
     terminal_output.print_terminal()
 
-
     ###
     #   Post process corelation results
     #
 
     #   Remove "bad" datasets from index array
     #   (only necessary for 'own' method)
     if correl_method == 'own':
@@ -2304,118 +2331,115 @@
 
     #   Remove "bad"/rejected ensembles
     for ject in reject:
         ensemble_dict.pop(keys[ject])
 
     #   Calculate shift for the reference origin
     shiftID = np.argwhere(reject < refORI)
-    Nshift  = len(shiftID)
-    refORI_new = refORI-Nshift
-
+    Nshift = len(shiftID)
+    refORI_new = refORI - Nshift
 
     ###
     #   Rearrange arrays based on the correlation results
     #
     #   Prepare new arrays for positions and indexes
-    x_sort   = np.zeros((count))
-    y_sort   = np.zeros((count))
+    x_sort = np.zeros((count))
+    y_sort = np.zeros((count))
     ind_sort = np.arange(count)
 
     #   Fill position arrays -> distinguish between input sources
     #                           depending on correlation method
     if correl_method == 'astropy':
         if (isinstance(x[refORI], u.quantity.Quantity) or
-            isinstance(x[refORI], Table)):
-                x_sort = x[refORI][indSR[refORI_new]].value
-                y_sort = y[refORI][indSR[refORI_new]].value
+                isinstance(x[refORI], Table)):
+            x_sort = x[refORI][indSR[refORI_new]].value
+            y_sort = y[refORI][indSR[refORI_new]].value
         elif isinstance(x[refORI], np.ndarray):
             x_sort = x[refORI][indSR[refORI_new]]
             y_sort = y[refORI][indSR[refORI_new]]
         else:
             raise TypeError(
                 f"{style.bcolors.FAIL} \nType of the position arrays not "
                 "known. Expect numpy.float or astropy.units.quantity.Quantity "
                 f"but got {type(x[refORI])} {style.bcolors.ENDC}"
-                )
+            )
 
     elif correl_method == 'own':
         #   Remove "bad" datasets first
         xall = np.delete(xall, reject, 1)
         yall = np.delete(yall, reject, 1)
 
-        x_sort = xall[indSR[refORI_new]][:,refORI_new]
-        y_sort = yall[indSR[refORI_new]][:,refORI_new]
-
+        x_sort = xall[indSR[refORI_new]][:, refORI_new]
+        y_sort = yall[indSR[refORI_new]][:, refORI_new]
 
     #   Loop over image ensembles to rearrange flux arrays
     for j, ensemble in enumerate(ensemble_dict.values()):
 
         #   Get image list
         img_list = ensemble.image_list
 
         #   Get number of images
         nimg = len(img_list)
 
         #   Overall array for the flux and uncertainty
         flux_arr = np.zeros(nimg, dtype=[('flux_fit', 'f8', (count)),
-                                          ('flux_unc', 'f8', (count)),
-                                          ]
-                        )
+                                         ('flux_unc', 'f8', (count)),
+                                         ]
+                            )
 
         #   Loop over images -> assumes that the images/results within each
         #   ensemble are already correlated such that the objects have the
         #   same indexes
         for z, img in enumerate(img_list):
             #   Get flux
             flux = img.flux
             uflux = img.uflux
 
             #   Define new flux array
             flux_sort = np.zeros(
                 count,
                 dtype=[('flux_fit', 'f8'), ('flux_unc', 'f8')]
-                )
+            )
 
             #   Rearrange flux
-            flux_sort['flux_fit'] = flux['flux_fit'][indSR[j,:]]
-            flux_sort['flux_unc'] = flux['flux_unc'][indSR[j,:]]
+            flux_sort['flux_fit'] = flux['flux_fit'][indSR[j, :]]
+            flux_sort['flux_unc'] = flux['flux_unc'][indSR[j, :]]
 
-            uflux_sort = uflux[indSR[j,:]]
+            uflux_sort = uflux[indSR[j, :]]
 
             #   Add sorted flux data and positions back to the image
             img.flux_es = flux_sort
             img.uflux_es = uflux_sort
             img.x_es = x_sort
             img.y_es = y_sort
             img.id_es = ind_sort
 
             #   Add to overall array
             flux_arr['flux_fit'][z] = flux_sort['flux_fit']
             flux_arr['flux_unc'][z] = flux_sort['flux_unc']
 
-
         uflux_arr = getattr(ensemble, 'uflux', None)
         if uflux_arr is None:
             uflux_arr_sort = unumpy.uarray(
                 flux_arr['flux_fit'],
                 flux_arr['flux_unc']
-                )
+            )
         else:
-            uflux_arr_sort = uflux_arr[:,indSR[j,:]]
+            uflux_arr_sort = uflux_arr[:, indSR[j, :]]
 
         #   Update image ensemble object and add IDs, pixel coordinates, and
         #   flux of the correlated objects
         ensemble.id_es = ind_sort
-        ensemble.x_es  = x_sort
-        ensemble.y_es  = y_sort
+        ensemble.x_es = x_sort
+        ensemble.y_es = y_sort
         ensemble.flux_es = flux_arr
         ensemble.uflux_es = uflux_arr_sort
 
 
-#@timeis
+# @timeis
 def correlate_pd(outdir, input_df, img_IDs, dcr, option, maxid=1,
                  refORI=0, refOBJ=[], nmissed=1, bfrac=1.0):
     '''
         WARNING: This function is not up to date
 
         Correlate star lists from the stacked images of all filters to find
         those stars that are visible on all images -> write calibrated CMD
@@ -2487,29 +2511,29 @@
             IDs of the rejected objects
 
         count               : `integer
             Number of matches found
     '''
     terminal_output.print_terminal(
         img_IDs,
-        indent=indent,
+        indent=2,
         string="Correlate results from the images ({:d})",
-        )
+    )
 
     #   Number of images
     nimg = len(img_IDs)
 
     #   Define data frames for X and Y coordinates
     df_x = pd.DataFrame()
     df_y = pd.DataFrame()
 
     #   Loop over all images
     for ID in img_IDs:
         #   Restrict input data frame to current image
-        mask    = input_df['type'] == ID
+        mask = input_df['type'] == ID
         ID_data = input_df[mask]
 
         #   Compile data frames with all X and Y positions
         df_x = pd.concat([df_x, ID_data['x_fit']], axis=1)
         df_y = pd.concat([df_y, ID_data['y_fit']], axis=1)
 
     #   Replace potential Nans with 0
@@ -2523,59 +2547,59 @@
         dcr,
         option=option,
         maxid=maxid,
         refORI=refORI,
         refOBJ=refOBJ,
         nmissed=nmissed,
         bfrac=bfrac
-        )
+    )
 
     #   Checks
     if count == 1:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nOnly one common object "
             f"found! {style.bcolors.ENDC}"
-            )
+        )
     elif count == 0:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nNo common objects "
             f"found! {style.bcolors.ENDC}"
-            )
+        )
 
     nbad = len(reject)
     if nbad > 0:
         terminal_output.print_terminal(
             nbad,
             indent=2,
             string="{:d} images do not meet the criteria -> removed",
-            )
+        )
 
     #   Remove bad origins listed in 'reject'
-    indSR   = np.delete(indSR, reject, 0)
-    xall    = np.delete(xall,  reject, 1)
-    yall    = np.delete(yall,  reject, 1)
+    indSR = np.delete(indSR, reject, 0)
+    xall = np.delete(xall, reject, 1)
+    yall = np.delete(yall, reject, 1)
     img_IDs = np.delete(img_IDs, reject, 0)
 
     #   Calculate shift for the reference origin
     shiftID = np.argwhere(reject < refORI)
-    Nshift  = len(shiftID)
+    Nshift = len(shiftID)
     refORI -= Nshift
 
     # Number of clean images
-    nclean = len(indSR[:,0])
+    nclean = len(indSR[:, 0])
 
     #   Initialize new arrays for X, Y positions, and index
-    x_sort   = np.zeros((count))
-    y_sort   = np.zeros((count))
+    x_sort = np.zeros((count))
+    y_sort = np.zeros((count))
     ind_sort = np.arange(count)
 
     #   Sort X and Y positions according to correlation results
-    for i in range(0,count):
-        x_sort[i]   = xall[indSR[refORI][i]][refORI]
-        y_sort[i]   = yall[indSR[refORI][i]][refORI]
+    for i in range(0, count):
+        x_sort[i] = xall[indSR[refORI][i]][refORI]
+        y_sort[i] = yall[indSR[refORI][i]][refORI]
 
     #   New data frame to return
     result = pd.DataFrame()
 
     #   Loop over all images --> Check if this loop can be removed by
     #                            dropping the data of removed images from
     #                            'input_df'
@@ -2596,20 +2620,20 @@
         #   Add to data frame
         result = pd.concat([result, pre_result], axis=0)
 
     return ind_sort, x_sort, y_sort, result, reject, rej_obj, count
 
 
 def correlate_preserve_calibs(img_ensemble, filter_list,
-                              calib_method='APASS', mag_range=(0.,18.5),
+                              calib_method='APASS', mag_range=(0., 18.5),
                               vizier_dict={}, calib_file=None, dcr=3,
                               option=1, verbose=False, maxid=1, ref_ID=0,
                               nmissed=1, bfrac=1.0, s_refOBJ=True,
                               plot_test=True, correl_method='astropy',
-                              seplimit=2.*u.arcsec):
+                              seplimit=2. * u.arcsec):
     '''
         Correlate results from all images, while preserving the calibration
         stars
 
         Parameters
         ----------
         img_ensemble        : `image.ensemble` object
@@ -2693,65 +2717,63 @@
     calib_tbl, col_names, ra_unit = calib.load_calib(
         img_ensemble.image_list[ref_ID],
         filter_list,
         calib_method=calib_method,
         mag_range=mag_range,
         vizier_dict=vizier_dict,
         calib_file=calib_file,
-        )
+    )
 
     #   Number of calibration stars
     n_calib = len(calib_tbl)
 
     if n_calib == 0:
         raise Exception(
             f"{style.bcolors.FAIL} \nNo match between calibrations stars and "
             f"the\n extracted stars detected. -> EXIT {style.bcolors.ENDC}"
-            )
-
+        )
 
     ###
     #   Find IDs of calibration stars to ensure they are not deleted in
     #   the correlation process
     #
     #   Lists for IDs, and xy coordinates
     calib_IDs = []
-    calib_xs  = []
-    calib_ys  = []
+    calib_xs = []
+    calib_ys = []
 
     #   Loop over all calibration stars
-    for k in range(0,n_calib):
+    for k in range(0, n_calib):
         #   Find the calibration star
-        inds_obj, ref_count, x_obj, y_obj  = correlate.posi_obj_srcor_img(
+        inds_obj, ref_count, x_obj, y_obj = correlate.posi_obj_srcor_img(
             img_ensemble.image_list[ref_ID],
             calib_tbl[col_names['ra']].data[k],
             calib_tbl[col_names['dec']].data[k],
             img_ensemble.wcs,
             dcr=dcr,
             option=option,
             ra_unit=ra_unit,
             verbose=verbose,
-            )
+        )
         if verbose:
             terminal_output.print_terminal()
 
         #   Add ID and coordinates of the calibration star to the lists
         if ref_count != 0:
             calib_IDs.append(inds_obj[1][0])
             calib_xs.append(x_obj)
             calib_ys.append(y_obj)
     terminal_output.print_terminal(
         len(calib_IDs),
         indent=3,
         string="{:d} matches",
         style_name='OKBLUE',
-        )
+    )
     terminal_output.print_terminal()
 
-
     ###
     #   Correlate the results from all images
     #
     correlate_ensemble_img(
         img_ensemble,
         dcr=dcr,
         option=option,
@@ -2759,33 +2781,32 @@
         refORI=ref_ID,
         refOBJ=calib_IDs,
         nmissed=nmissed,
         bfrac=bfrac,
         s_refOBJ=s_refOBJ,
         correl_method=correl_method,
         seplimit=seplimit,
-        )
-
+    )
 
     ###
     #   Plot image with the final positions overlaid (final version)
     #
     aux.prepare_and_plot_starmap_final_3(
         img_ensemble,
         calib_xs,
         calib_ys,
         plot_test=plot_test,
-        )
+    )
 
 
 def correlate_preserve_variable(img_ensemble, ra_obj, dec_obj, dcr=3.,
                                 option=1, maxid=1, ref_ID=0, nmissed=1,
                                 bfrac=1.0, s_refOBJ=True,
                                 correl_method='astropy',
-                                seplimit=2.*u.arcsec, verbose=False,
+                                seplimit=2. * u.arcsec, verbose=False,
                                 plot_test=True):
     '''
         Correlate results from all images, while preserving the variable
         star
 
         Parameters
         ----------
@@ -2853,52 +2874,50 @@
     '''
     ###
     #   Find position of the variable star I
     #
     terminal_output.print_terminal(
         indent=1,
         string="Identify the variable star",
-        )
+    )
 
     if correl_method == 'astropy':
         variable_ID, count, x_obj, y_obj = correlate.posi_obj_astropy_img(
             img_ensemble.image_list[ref_ID],
             ra_obj,
             dec_obj,
             img_ensemble.wcs,
             seplimit=seplimit,
-            )
+        )
 
     elif correl_method == 'own':
-        inds_obj, count, x_obj, y_obj  = correlate.posi_obj_srcor_img(
+        inds_obj, count, x_obj, y_obj = correlate.posi_obj_srcor_img(
             img_ensemble.image_list[ref_ID],
             ra_obj,
             dec_obj,
             img_ensemble.wcs,
             dcr=dcr,
             option=option,
             verbose=verbose,
-            )
+        )
 
         #   Current object ID
-        variable_ID  = inds_obj[1]
+        variable_ID = inds_obj[1]
 
         if verbose:
             terminal_output.print_terminal()
 
-
     ###
     #   Check if variable star was detected I
     #
     if count == 0:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \tERROR: The variable object was not "
             f"detected in the reference image.\n\t-> EXIT{style.bcolors.ENDC}"
-            )
-
+        )
 
     ###
     #   Correlate the stellar positions from the different filter
     #
     correlate_ensemble_img(
         img_ensemble,
         dcr=dcr,
@@ -2907,72 +2926,69 @@
         refORI=ref_ID,
         refOBJ=int(variable_ID),
         nmissed=nmissed,
         bfrac=bfrac,
         s_refOBJ=s_refOBJ,
         correl_method=correl_method,
         seplimit=seplimit,
-        )
-
+    )
 
     ###
     #   Find position of the variable star II
     #
     terminal_output.print_terminal(
         indent=1,
         string="Reidentify the variable star",
-        )
+    )
 
     if correl_method == 'astropy':
         variable_ID, count, x_obj, y_obj = correlate.posi_obj_astropy(
             img_ensemble.x_s,
             img_ensemble.y_s,
             ra_obj,
             dec_obj,
             img_ensemble.wcs,
             seplimit=seplimit,
-            )
+        )
 
     elif correl_method == 'own':
-        inds_obj, count, x_obj, y_obj  = correlate.posi_obj_srcor(
+        inds_obj, count, x_obj, y_obj = correlate.posi_obj_srcor(
             img_ensemble.x_s,
             img_ensemble.y_s,
             ra_obj,
             dec_obj,
             img_ensemble.wcs,
             dcr=dcr,
             option=option,
             verbose=verbose,
-            )
+        )
         if verbose:
             terminal_output.print_terminal()
 
         #   Current object ID
-        variable_ID  = inds_obj[1]
-
+        variable_ID = inds_obj[1]
 
     ###
     #   Check if variable star was detected II
     #
     if count == 0:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \tERROR: The variable was not detected "
             f"in the reference image.\n\t-> EXIT{style.bcolors.ENDC}"
-            )
-
+        )
 
     ###
     #   Plot image with the final positions overlaid (final version)
     #
     aux.prepare_and_plot_starmap_final_3(
         img_ensemble,
         [x_obj],
         [y_obj],
         plot_test=plot_test,
-        )
+    )
 
     #   Add ID of the variable star to the image ensemble
     img_ensemble.variable_ID = variable_ID
 
 
 def extract_multiprocessing(img_ensemble, ncores, sigma_psf, sigma_bkg=5.,
                             multi_start=5., size_epsf=25,
@@ -3090,28 +3106,26 @@
             If True a star map plots only for the reference image [refid] is
             created
             Default is ``True``.
     '''
     #   Get filter
     filt = img_ensemble.filt
 
-
     ###
     #   Find the stars (via DAO or IRAF StarFinder)
     #
     if not search_image:
         mk_bg(img_ensemble.ref_img, sigma_bkg=sigma_bkg)
 
         find_stars(
             img_ensemble.ref_img,
             sigma_psf[filt],
             multi_start=multi_start,
             method=method,
-            )
-
+        )
 
     ###
     #   Main loop: Extract stars and info from all images, using
     #              multiprocessing
     #
     #   Initialize multiprocessing object
     executor = aux.Executor(ncores)
@@ -3124,50 +3138,49 @@
 
         #   Extract photometry
         executor.schedule(
             main_extract_condense,
             args=(
                 image,
                 sigma_psf[filt],
-                ),
+            ),
             kwargs={
-                'sigma_bkg':sigma_bkg,
-                'multi_start':multi_start,
-                'size_epsf':size_epsf,
-                'frac_epsf_stars':frac_epsf_stars,
-                'oversampling':oversampling,
-                'maxiters':maxiters,
-                'epsf_use_init_guesses':epsf_use_init_guesses,
-                'method':method,
-                'multi':multi,
-                'multi_grouper':multi_grouper,
-                'strict_cleaning':strict_cleaning,
-                'min_eps_stars':min_eps_stars,
-                'strict_eps':strict_eps,
-                'refid':img_ensemble.ref_id,
-                'photometry':photometry,
-                'rstars':rstars,
-                'rbg_in':rbg_in,
-                'rbg_out':rbg_out,
-                'r_unit':r_unit,
-                'search_image':search_image,
-                'plot_ifi':plot_ifi,
-                'plot_test':plot_test,
-                }
-            )
+                'sigma_bkg': sigma_bkg,
+                'multi_start': multi_start,
+                'size_epsf': size_epsf,
+                'frac_epsf_stars': frac_epsf_stars,
+                'oversampling': oversampling,
+                'maxiters': maxiters,
+                'epsf_use_init_guesses': epsf_use_init_guesses,
+                'method': method,
+                'multi': multi,
+                'multi_grouper': multi_grouper,
+                'strict_cleaning': strict_cleaning,
+                'min_eps_stars': min_eps_stars,
+                'strict_eps': strict_eps,
+                'refid': img_ensemble.ref_id,
+                'photometry': photometry,
+                'rstars': rstars,
+                'rbg_in': rbg_in,
+                'rbg_out': rbg_out,
+                'r_unit': r_unit,
+                'search_image': search_image,
+                'plot_ifi': plot_ifi,
+                'plot_test': plot_test,
+            }
+        )
     #   Close multiprocessing pool and wait until it finishes
     executor.wait()
 
     #   Exit if exceptions occurred
     if executor.err is not None:
         raise RuntimeError(
             f'\n{style.bcolors.FAIL}Extraction using multiprocessing failed '
             f'for {filt} :({style.bcolors.ENDC}'
-            )
-
+        )
 
     ###
     #   Sort multiprocessing results
     #
     #   Extract results
     res = executor.res
 
@@ -3296,184 +3309,175 @@
             If True a star map plots only for the reference image [refid] is
             created
             Default is ``True``.
     '''
     ###
     #   Initialize output string
     #
-    outstring  = "      "
+    outstring = "      "
     outstring += style.bcolors.UNDERLINE
-    outstring += "Image: "+str(image.pd)
-    outstring += style.bcolors.ENDC+"\n"
-
+    outstring += "Image: " + str(image.pd)
+    outstring += style.bcolors.ENDC + "\n"
 
     ###
     #   Estimate and remove background
     #
     mk_bg(image, sigma_bkg=sigma_bkg)
 
-
     ###
     #   Find the stars (via DAO or IRAF StarFinder)
     #
     if search_image:
         out_str = find_stars(
             image,
             sigma_psf,
             multi_start=multi_start,
             method=method,
             condense=True,
-            )
+        )
         outstring += out_str
 
     if photometry == 'PSF':
         ###
         #   Check if enough stars have been detected to allow ePSF
         #   calculations
         #
         out_str = check_epsf_stars(
             image,
             size=size_epsf,
             min_stars=min_eps_stars,
             frac_epsf=frac_epsf_stars,
             condense=True,
             strict=strict_eps,
-            )
+        )
         outstring += out_str
 
-
         ###
         #   Plot images with the identified stars overlaid
         #
         if plot_ifi or (plot_test and image.pd == refid):
             out_str = plot.starmap(
                 image.outpath.name,
                 image.get_data(),
                 image.filt,
                 image.positions,
                 tbl_2=image.positions_epsf,
                 label='identified stars',
                 label_2='stars used to determine the ePSF',
-                rts='initial-img-'+str(image.pd),
+                rts='initial-img-' + str(image.pd),
                 nameobj=image.objname,
                 condense=True,
-                )
+            )
         else:
             out_str = ''
         outstring += out_str
 
-
         ###
         #   Calculate the ePSF
         #
         out_str = mk_epsf(
             image,
             size=size_epsf,
             oversampling=oversampling,
             maxiters=maxiters,
             min_stars=min_eps_stars,
             multi=False,
             condense=True,
-            )
+        )
         outstring += out_str
 
-
         ###
         #   Plot the ePSFs
         #
         out_str = plot.plot_epsf(
             image.outpath.name,
-            {'img-'+str(image.pd)+'-'+image.filt:image.epsf},
+            {'img-' + str(image.pd) + '-' + image.filt: image.epsf},
             condense=True,
             nameobj=image.objname,
             indent=2,
-            )
+        )
         outstring += out_str
 
-
         ###
         #   Performing the PSF photometry
         #
         out_str = epsf_extract(
             image,
             sigma_psf,
             sigma_bkg=sigma_bkg,
             use_init_guesses=epsf_use_init_guesses,
             method_finder=method,
             size_epsf=size_epsf,
             multi=multi,
             multi_grouper=multi_grouper,
             strict_cleaning=strict_cleaning,
             condense=True,
-            )
+        )
         outstring += out_str
 
-
         ###
         #   Plot original and residual image
         #
         out_str = plot.plot_residual(
             image.objname,
-            {f'{image.pd}-{image.filt}':image.get_data()},
-            {f'{image.pd}-{image.filt}':image.residual_image},
-            #{str(image.pd)+'-'+image.filt:image.get_data()},
-            #{str(image.pd)+'-'+image.filt:image.residual_image},
+            {f'{image.pd}-{image.filt}': image.get_data()},
+            {f'{image.pd}-{image.filt}': image.residual_image},
+            # {str(image.pd)+'-'+image.filt:image.get_data()},
+            # {str(image.pd)+'-'+image.filt:image.residual_image},
             image.outpath.name,
             condense=True,
             nameobj=image.objname,
             indent=2,
-            )
+        )
         outstring += out_str
 
     elif photometry == 'APER':
         ###
         #   Perform aperture photometry
         #
         if image.pd == refid:
-            plotaper=True
+            plotaper = True
         else:
-            plotaper=False
+            plotaper = False
 
         out_str = aperture_extract(
             image,
             rstars,
             rbg_in,
             rbg_out,
             r_unit=r_unit,
             plotaper=plotaper,
             condense=True,
             indent=3,
-            )
+        )
         outstring += out_str
 
     else:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nExtraction method ({photometry}) not "
             f"valid: use either aper or PSF {style.bcolors.ENDC}"
-            )
-
+        )
 
     ###
     #   Plot images with extracted stars overlaid
     #
     if plot_ifi or (plot_test and image.pd == refid):
         out_str = aux.prepare_and_plot_starmap(image, condense=True)
     else:
         out_str = ''
     outstring += out_str
     outstring += '\n'
     terminal_output.print_terminal(
         indent=0,
         string=outstring,
-        )
+    )
 
     return image
 
 
-
 def main_extract(image, sigma_psf, sigma_bkg=5., multi_start=5.,
                  size_epsf=25, frac_epsf_stars=0.2, oversampling=2,
                  maxiters=7, epsf_use_init_guesses=True,
                  method='IRAF', multi=5.0, multi_grouper=2.0,
                  strict_cleaning=True, min_eps_stars=25, refid=0,
                  photometry='PSF', rstars=5., rbg_in=7., rbg_out=10.,
                  r_unit='arcsec', strict_eps=True, rmcos=False, objlim=5.,
@@ -3606,170 +3610,160 @@
     #   Initialize output string
     #
     terminal_output.print_terminal(
         image.pd,
         indent=2,
         string="Image: {:d}",
         style_name='UNDERLINE',
-        )
-
+    )
 
     ###
     #   Remove cosmics (optional)
     #
     if rmcos:
         rm_cosmic(
             image,
             objlim=objlim,
             readnoise=readnoise,
             sigclip=sigclip,
             satlevel=satlevel,
-            )
-
+        )
 
     ###
     #   Estimate and remove background
     #
     mk_bg(image, sigma_bkg=sigma_bkg)
 
-
     ###
     #   Find the stars (via DAO or IRAF StarFinder)
     #
     find_stars(
         image,
         sigma_psf,
         multi_start=multi_start,
         method=method,
-        )
-
+    )
 
     if photometry == 'PSF':
         ###
         #   Check if enough stars have been detected to allow ePSF
         #   calculations
         #
         check_epsf_stars(
             image,
             size=size_epsf,
             min_stars=min_eps_stars,
             frac_epsf=frac_epsf_stars,
             strict=strict_eps,
-            )
-
+        )
 
         ###
         #   Plot images with the identified stars overlaid
         #
         if plot_ifi or (plot_test and image.pd == refid):
             plot.starmap(
                 image.outpath.name,
                 image.get_data(),
                 image.filt,
                 image.positions,
                 tbl_2=image.positions_epsf,
                 label='identified stars',
                 label_2='stars used to determine the ePSF',
-                rts='initial-img-'+str(image.pd),
+                rts='initial-img-' + str(image.pd),
                 nameobj=image.objname,
-                )
-
+            )
 
         ###
         #   Calculate the ePSF
         #
         mk_epsf(
             image,
             size=size_epsf,
             oversampling=oversampling,
             maxiters=maxiters,
             min_stars=min_eps_stars,
             multi=False,
-            )
-
+        )
 
         ###
         #   Plot the ePSFs
         #
         plot.plot_epsf(
             image.outpath.name,
-            {'img-'+str(image.pd)+'-'+image.filt:image.epsf},
+            {'img-' + str(image.pd) + '-' + image.filt: image.epsf},
             nameobj=image.objname,
             indent=2,
-            )
-
+        )
 
         ###
         #   Performing the PSF photometry
         #
         epsf_extract(
             image,
             sigma_psf,
             sigma_bkg=sigma_bkg,
             use_init_guesses=epsf_use_init_guesses,
             method_finder=method,
             size_epsf=size_epsf,
             multi=multi,
             multi_grouper=multi_grouper,
             strict_cleaning=strict_cleaning,
-            )
-
+        )
 
         ###
         #   Plot original and residual image
         #
         plot.plot_residual(
             image.objname,
-            {str(image.pd)+'-'+image.filt:image.get_data()},
-            {str(image.pd)+'-'+image.filt:image.residual_image},
+            {str(image.pd) + '-' + image.filt: image.get_data()},
+            {str(image.pd) + '-' + image.filt: image.residual_image},
             image.outpath.name,
             nameobj=image.objname,
-            indent='      ',
-            )
+            indent=2,
+        )
 
     elif photometry == 'APER':
         ###
         #   Perform aperture photometry
         #
         if image.pd == refid:
-            plotaper=True
+            plotaper = True
         else:
-            plotaper=False
+            plotaper = False
 
         aperture_extract(
             image,
             rstars,
             rbg_in,
             rbg_out,
             r_unit=r_unit,
             plotaper=plotaper,
             indent=3,
-            )
+        )
     else:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nExtraction method ({photometry}) not "
             f"valid: use either APER or PSF {style.bcolors.ENDC}"
-            )
+        )
 
     #   Add flux array to image (is this really necessary?)
     flux_img = np.zeros(
         len(image.photometry['x_fit']),
         dtype=[('flux_fit', 'f8'), ('flux_unc', 'f8')],
-        )
+    )
     flux_img['flux_fit'] = image.photometry['flux_fit']
     flux_img['flux_unc'] = image.photometry['flux_unc']
 
     uflux_img = unumpy.uarray(
-            flux_img['flux_fit'],
-            flux_img['flux_unc']
-            )
+        flux_img['flux_fit'],
+        flux_img['flux_unc']
+    )
     image.flux = flux_img
     image.uflux = uflux_img
 
-
     ###
     #   Plot images with extracted stars overlaid
     #
     if plot_ifi or (plot_test and image.pd == refid):
         aux.prepare_and_plot_starmap(image)
 
     terminal_output.print_terminal()
@@ -3889,15 +3883,15 @@
 
         rbg_out         : `float`, optional
             Outer radius of the background annulus
             Default is ``10``.
 
         r_unit          : `string`, optional
             Unit of the radii above. Allowed are ``pixel`` and ``arcsec``.
-            Default is ``pixel``.
+            Default is ``arcsec``.
 
         strict_eps      ; `boolean`, optional
             If True a stringent test of the ePSF conditions is applied.
             Default is ``True``.
 
         rmcos           : `bool`
             If True cosmic rays will be removed from the image.
@@ -3931,60 +3925,73 @@
             Default is ``True``.
     '''
     ###
     #   Check output directories
     #
     checks.check_out(
         outdir,
-        os.path.join(outdir,'tables'),
-        )
+        os.path.join(outdir, 'tables'),
+    )
 
     ###
     #   Loop over all filter
     #
     for filt in filter_list:
         terminal_output.print_terminal(
             filt,
             string="Analyzing {:s} images",
             style_name='HEADER',
-            )
+        )
 
         ###
-        #   Check paths
+        #   Check input paths
         #
         checks.check_file(img_paths[filt])
 
-
         #   Initialize image ensemble object
-        img_container.ensembles[filt] = image_ensemble(
+        img_container.ensembles[filt] = current_ensemble = image_ensemble(
             filt,
             name,
             img_paths[filt],
             outdir,
             0,
-            )
-
+        )
 
         ###
         #   Find the WCS solution for the image
         #
-        aux.find_wcs(
-            img_container.ensembles[filt],
-            ref_id=0,
-            method=wcs_method,
-            force_wcs_determ=force_wcs_determ,
-            indent=3,
-            )
-
+        try:
+            aux.find_wcs(
+                current_ensemble,
+                ref_id=0,
+                method=wcs_method,
+                force_wcs_determ=force_wcs_determ,
+                indent=3,
+            )
+        except Exception as e:
+            for f in filter_list:
+                wcs = getattr(img_container.ensembles[f], 'wcs', None)
+                if wcs is not None:
+                    current_ensemble.set_wcs(wcs)
+                    terminal_output.print_terminal(
+                        string=f"WCS could not be determined for filter {filt}"
+                               f"The WCS of filter {f} will be used instead."
+                               f"This could lead to problems...",
+                        indent=1,
+                        style_name='WARNING',
+                    )
+                    break
+            else:
+                raise RuntimeError('')
 
         ###
         #   Main extraction
         #
         main_extract(
-            img_container.ensembles[filt].image_list[0],
+            current_ensemble.image_list[0],
             sigma_psf[filt],
             sigma_bkg=sigma_bkg,
             multi_start=multi_start,
             size_epsf=size_epsf,
             frac_epsf_stars=frac_epsf_stars,
             oversampling=oversampling,
             maxiters=maxiters,
@@ -4003,63 +4010,61 @@
             rmcos=rmcos,
             objlim=objlim,
             readnoise=readnoise,
             sigclip=sigclip,
             satlevel=satlevel,
             plot_ifi=plot_ifi,
             plot_test=plot_test,
-            )
+        )
 
         #   Add stellar positions to ensemble class
         #   TODO: Shift this into main extract
-        photo = img_container.ensembles[filt].image_list[0].photometry
-        img_container.ensembles[filt].x_s = photo['x_fit']
-        img_container.ensembles[filt].y_s = photo['y_fit']
-
+        photo = current_ensemble.image_list[0].photometry
+        current_ensemble.x_s = photo['x_fit']
+        current_ensemble.y_s = photo['y_fit']
 
     if photometry == 'PSF':
         ###
         #   Plot the ePSFs
         #
         p = mp.Process(
             target=plot.plot_epsf,
             args=(outdir, img_container.get_ref_epsf(),),
-            )
+        )
         p.start()
 
-
         ###
         #   Plot original and residual image
         #
         p = mp.Process(
             target=plot.plot_residual,
             args=(
                 name,
                 img_container.get_ref_img(),
                 img_container.get_ref_residual_img(),
                 outdir,
-                ),
+            ),
             kwargs={
-                'nameobj':'reference image'
-                }
-            )
+                'nameobj': 'reference image'
+            }
+        )
         p.start()
 
 
 def extract_flux_multi(img_container, filter_list, name, img_paths, outdir,
                        sigma_psf, ra_obj, dec_obj, ncores=6,
                        wcs_method='astrometry', force_wcs_determ=False,
                        sigma_bkg=5., multi_start=5., size_epsf=25,
                        frac_epsf_stars=0.2, oversampling=2, maxiters=7,
                        method='IRAF', multi=5.0, multi_grouper=2.0,
                        strict_cleaning=True, min_eps_stars=25, strict_eps=True,
                        photometry='PSF', rstars=5., rbg_in=7., rbg_out=10.,
                        r_unit='arcsec', dcr=3., option=1, maxid=1, ref_ID=0,
                        nmissed=1, bfrac=1.0, s_refOBJ=True,
-                       correl_method='astropy', seplimit=2.*u.arcsec,
+                       correl_method='astropy', seplimit=2. * u.arcsec,
                        verbose=False, search_image=True, plot_ifi=False,
                        plot_test=True):
     '''
         Extract flux from multiple images per filter and add results to
         the image container
 
         Parameters
@@ -4232,53 +4237,48 @@
             If True a star map plots only for the reference image [refid] is
             created
             Default is ``True``.
     '''
     ###
     #   Check output directories
     #
-    checks.check_out(outdir, os.path.join(outdir,'tables'))
-
+    checks.check_out(outdir, os.path.join(outdir, 'tables'))
 
     ###
     #   Check image directories
     #
     checks.check_dir(img_paths)
 
-
     #   Outer loop over all filter
     for filt in filter_list:
         terminal_output.print_terminal(
             filt,
             string="Analyzing {:s} images",
             style_name='HEADER',
-            )
-
+        )
 
         #   Initialize image ensemble object
         img_container.ensembles[filt] = image_ensemble(
             filt,
             name,
             img_paths[filt],
             outdir,
             ref_ID,
-            )
-
+        )
 
         ###
         #   Find the WCS solution for the image
         #
         aux.find_wcs(
             img_container.ensembles[filt],
             ref_id=ref_ID,
             method=wcs_method,
             force_wcs_determ=force_wcs_determ,
             indent=3,
-            )
-
+        )
 
         ###
         #   Main extraction of object positions and object fluxes
         #   using multiprocessing
         #
         extract_multiprocessing(
             img_container.ensembles[filt],
@@ -4300,16 +4300,15 @@
             rstars=rstars,
             rbg_in=rbg_in,
             rbg_out=rbg_out,
             r_unit=r_unit,
             search_image=search_image,
             plot_ifi=plot_ifi,
             plot_test=plot_test,
-            )
-
+        )
 
         if search_image:
             ###
             #   Correlate results from all images, while preserving
             #   the variable star
             #
             correlate_preserve_variable(
@@ -4323,67 +4322,65 @@
                 nmissed=nmissed,
                 bfrac=bfrac,
                 s_refOBJ=s_refOBJ,
                 verbose=verbose,
                 plot_test=plot_test,
                 correl_method=correl_method,
                 seplimit=seplimit,
-                )
+            )
 
         else:
             img_ensemble = img_container.ensembles[filt]
 
             ###
             #   Find position of the variable star
             #
             terminal_output.print_terminal(
                 indent=1,
                 string="Identify the variable star",
-                )
+            )
 
             if correl_method == 'astropy':
                 variable_ID, count, x_obj, y_obj = correlate.posi_obj_astropy_img(
                     img_ensemble.image_list[ref_ID],
                     ra_obj,
                     dec_obj,
                     img_ensemble.wcs,
-                    )
+                )
 
             elif correl_method == 'own':
-                inds_obj, count, x_obj, y_obj  = correlate.posi_obj_srcor_img(
+                inds_obj, count, x_obj, y_obj = correlate.posi_obj_srcor_img(
                     img_ensemble.image_list[ref_ID],
                     ra_obj,
                     dec_obj,
                     img_ensemble.wcs,
                     dcr=dcr,
                     option=option,
                     verbose=verbose,
-                    )
+                )
 
                 #   Current object ID
-                variable_ID  = inds_obj[1]
+                variable_ID = inds_obj[1]
 
                 if verbose:
                     terminal_output.print_terminal()
 
-
             ###
             #   Check if variable star was detected
             #
             if count == 0:
                 raise RuntimeError(
                     f"{style.bcolors.FAIL} \tERROR: The variable object was "
                     f"not detected in the reference image.\n"
                     f"\t-> EXIT {style.bcolors.ENDC}"
-                    )
+                )
 
             #   Add ID of the variable star to the image ensemble
             img_ensemble.variable_ID = variable_ID
 
-
             ###
             #
             #
 
             #   Get dictionary with astropy tables with the position and flux data
             result_tbl = img_ensemble.get_photometry()
 
@@ -4398,96 +4395,94 @@
 
             #   Number of images
             nimg = len(arr_img_IDs)
 
             #   Prepare array for the flux and uncertainty (all datasets)
             flux_arr = np.zeros(nimg, dtype=[('flux_fit', 'f8', (count)),
                                              ('flux_unc', 'f8', (count)),
-                                            ]
-                            )
+                                             ]
+                                )
 
             #   Fill flux arrays
             for j, img_ID in enumerate(arr_img_IDs):
                 img_ID_str = str(img_ID)
 
                 #   Flux and uncertainty array for individual images
                 flux_img = np.zeros(
                     count,
                     dtype=[('flux_fit', 'f8'), ('flux_unc', 'f8')],
-                    )
+                )
 
                 #   Rearrange flux and error
                 flux_img['flux_fit'] = result_tbl[img_ID_str]['flux_fit']
                 flux_img['flux_unc'] = result_tbl[img_ID_str]['flux_unc']
 
                 #   Remove nans etc. in error
                 flux_img['flux_unc'] = np.nan_to_num(
                     flux_img['flux_unc'],
                     nan=9999.,
                     posinf=9999.,
                     neginf=9999.,
-                    )
+                )
 
                 #   Remove '--' entries in error
                 flux_err_dash = np.argwhere(flux_img['flux_unc'] == '--')
                 flux_img['flux_unc'][flux_err_dash] = 9999.
 
                 uflux_img = unumpy.uarray(
                     flux_img['flux_fit'],
                     flux_img['flux_unc']
-                    )
+                )
 
                 #   Add sorted flux data and positions back to the image
-                img_ensemble.image_list[img_ID].flux    = flux_img
-                img_ensemble.image_list[img_ID].uflux   = uflux_img
-                img_ensemble.image_list[img_ID].x_sort  = x_s
-                img_ensemble.image_list[img_ID].y_sort  = y_s
+                img_ensemble.image_list[img_ID].flux = flux_img
+                img_ensemble.image_list[img_ID].uflux = uflux_img
+                img_ensemble.image_list[img_ID].x_sort = x_s
+                img_ensemble.image_list[img_ID].y_sort = y_s
                 img_ensemble.image_list[img_ID].id_sort = id_s
 
-
                 #   Add to overall array
                 flux_arr['flux_fit'][j] = flux_img['flux_fit']
                 flux_arr['flux_unc'][j] = flux_img['flux_unc']
 
             uflux_arr = unumpy.uarray(
-                    flux_arr['flux_fit'],
-                    flux_arr['flux_unc']
-                    )
+                flux_arr['flux_fit'],
+                flux_arr['flux_unc']
+            )
 
             #   Update image ensemble object and add IDs, pixel coordinates, and
             #   flux of the correlated objects
             img_ensemble.id_s = id_s
-            img_ensemble.x_s  = x_s
-            img_ensemble.y_s  = y_s
+            img_ensemble.x_s = x_s
+            img_ensemble.y_s = y_s
             img_ensemble.flux = flux_arr
             img_ensemble.uflux = uflux_arr
 
-
-
             ###
             #   Plot image with the final positions overlaid (final version)
             #
             aux.prepare_and_plot_starmap_final_3(
                 img_ensemble,
                 [x_obj],
                 [y_obj],
                 plot_test=plot_test,
-                )
+            )
 
 
 def correlate_calibrate(img_container, filter_list, dcr=3, option=1,
                         ref_img=0, calib_method='APASS', vizier_dict={},
                         calib_file=None, ID=None, ra_unit=u.deg,
-                        dec_unit=u.deg, mag_range=(0.,18.5), Tcs=None,
+                        dec_unit=u.deg, mag_range=(0., 18.5), Tcs=None,
                         derive_Tcs=False, plot_sigma=False, photo_type='',
                         region=False, radius=600, data_cluster=False,
                         pm_median=False, max_distance_cluster=6.,
                         find_cluster_para_set=1, correl_method='astropy',
-                        seplimit=2.*u.arcsec):
-    '''
+                        seplimit=2. * u.arcsec, r_limit=4., r_unit='arcsec',
+                        convert_mags=False, target_filter_system='SDSS'):
+    """
         Correlate photometric extraction results from 2 images and calibrate
         the magnitudes.
 
         Parameters
         ----------
         img_container           : `image.container`
             Container object with image ensemble objects for each filter
@@ -4516,15 +4511,15 @@
             calibration data
             Default is ``{}``.
 
         calib_file              : `string`, optional
             Path to the calibration file
             Default is ``None``.
 
-        ID                      : `integer`, optional
+        ID                      : `integer` or `None`, optional
             ID of the object
             Default is ``None``.
 
         ra_unit                 : `astropy.unit`, optional
             Right ascension unit
             Default is ``u.deg``.
 
@@ -4532,161 +4527,186 @@
             Declination unit
             Default is ``u.deg``.
 
         mag_range               : `tupel` or `float`, optional
             Magnitude range
             Default is ``(0.,18.5)``.
 
-        Tcs             : `dictionary`, optional
+        Tcs                     : `dictionary`, optional
             Calibration coefficients for the magnitude transformation
             Default is ``None``.
 
-        derive_Tcs      : `boolean`, optional
+        derive_Tcs              : `boolean`, optional
             If True the magnitude transformation coefficients will be
             calculated from the current data even if calibration coefficients
             are available in the data base.
             Default is ``False``
 
-        plot_sigma      : `boolean', optional
+        plot_sigma              : `boolean', optional
             If True sigma clipped magnitudes will be plotted.
             Default is ``False``.
 
-        photo_type      : `string`, optional
+        photo_type              : `string`, optional
             Applied extraction method. Posibilities: ePSF or APER`
             Default is ``''``.
 
-        region          : `boolean`, optional
+        region                  : `boolean`, optional
             If True the extracted objects will be filtered such that only
             objects with ``radius`` will be returned.
             Default is ``False``.
 
-        radius          : `float`, optional
+        radius                  : `float`, optional
             Radius around the object in arcsec.
             Default is ``600``.
 
-        data_cluster    : `boolean`, optional
+        data_cluster            : `boolean`, optional
             If True cluster in the Gaia distance and proper motion data
             will be identified.
             Default is ``False``.
 
-        pm_median       : `boolean`, optional
+        pm_median               : `boolean`, optional
             If True only the objects that are close to the median
             proper motion will be returned.
             Default is ``False``.
 
         max_distance_cluster    : `float`, optional
             Expected maximal distance of the cluster in kpc. Used to
             restrict the parameter space to facilitate an easy
             identification of the star cluster.
             Default is ``6``.
 
         find_cluster_para_set   : `integer`, optional
             Parameter set used to identify the star cluster in proper
             motion and distance data.
 
-        correl_method       : `string`, optional
+        correl_method           : `string`, optional
             Correlation method to be used to find the common objects on
             the images.
             Possibilities: ``astropy``, ``own``
             Default is ``astropy``.
 
-        seplimit            : `astropy.units`, optional
+        seplimit                : `astropy.units`, optional
             Allowed separation between objects.
             Default is ``2.*u.arcsec``.
-    '''
+
+        r_limit                 : `float`, optional
+            Radius of the aperture used to derive the limiting magnitude
+            Default is ``4``.
+
+        r_unit                  : `string`, optional
+            Unit of the radii above. Allowed are ``pixel`` and ``arcsec``.
+            Default is ``arcsec``.
+
+        convert_mags            : `boolean`, optional
+            If True the magnitudes will be converted to another
+            filter systems specified in `target_filter_system`.
+            Default is ``False``.
+
+        target_filter_system    : `string`, optional
+            Photometric system the magnitudes should be converted to
+            Default is ``SDSS``.
+    """
     ###
     #   Correlate the stellar positions from the different filter
     #
     correlate_ensemble(
         img_container,
         filter_list,
         dcr=dcr,
         option=option,
         correl_method=correl_method,
         seplimit=seplimit,
-        )
-
+    )
 
     ###
     #   Plot image with the final positions overlaid (final version)
     #
     if len(filter_list) > 1:
         aux.prepare_and_plot_starmap_final(
             img_container,
             filter_list,
-            )
-
+        )
 
     ###
     #   Calibrate the magnitudes
     #
     #   Load calibration information
     calib.deter_calib(
         img_container,
         filter_list,
         calib_method=calib_method,
         dcr=dcr,
         option=option,
         vizier_dict=vizier_dict,
         calib_file=calib_file,
         mag_range=mag_range,
-        )
+        ra_unit=ra_unit,
+        dec_unit=dec_unit,
+    )
 
     #   Apply calibration and perform magnitude transformation
     trans.apply_calib(
         img_container,
         filter_list,
         Tcs=Tcs,
         derive_Tcs=derive_Tcs,
         plot_sigma=plot_sigma,
         photo_type=photo_type,
         refid=ref_img,
-        )
-
+    )
 
     ###
     #   Restrict results to specific areas of the image and filter by means
     #   of proper motion and distance using Gaia
+    #
     aux.postprocess_results(
         img_container,
         filter_list,
+        id_object=ID,
         photo_type=photo_type,
         region=region,
         radius=radius,
         data_cluster=data_cluster,
         pm_median=pm_median,
         max_distance_cluster=max_distance_cluster,
         find_cluster_para_set=find_cluster_para_set,
-        )
-
+        convert_mags=convert_mags,
+        target_filter_system=target_filter_system,
+    )
 
     ###
     #   Determine limiting magnitudes
     #
-    aux.derive_limiting_mag(img_container, filter_list, ref_img)
+    aux.derive_limiting_mag(
+        img_container,
+        filter_list,
+        ref_img,
+        r_limit=r_limit,
+        r_unit=r_unit,
+    )
 
 
 def calibrate_data_mk_lc(img_container, filter_list, ra_obj, dec_obj, nameobj,
                          outdir, transit_time, period, valid_calibs=None,
                          binn=None, Tcs=None, derive_Tcs=False, ref_ID=0,
                          calib_method='APASS', vizier_dict={}, calib_file=None,
-                         mag_range=(0.,18.5), dcr=3., option=1, maxid=1,
+                         mag_range=(0., 18.5), dcr=3., option=1, maxid=1,
                          nmissed=1, bfrac=1.0, s_refOBJ=True, photo_type='',
-                         correl_method='astropy', seplimit=2.*u.arcsec,
+                         correl_method='astropy', seplimit=2. * u.arcsec,
                          verbose=False, plot_test=True, plot_ifi=False,
                          plot_sigma=False):
-    '''
+    """
         Calculate magnitudes, calibrate, and plot light curves
 
         Parameters
         ----------
         img_container       : `image.container`
             Container object with image ensemble objects for each filter
 
-        filt_list           : `list` of `strings`
+        filter_list           : `list` of `strings`
             List with filter names
 
         ra_obj              : `float`
             Right ascension of the object
 
         dec_obj             : `float`
             Declination of the object
@@ -4799,24 +4819,24 @@
             If True star map plots for all stars will be created.
             Default is ``False``.
 
         plot_sigma          : `boolean', optional
             If True sigma clipped magnitudes will be plotted.
             Default is ``False``.
 
-    '''
+    """
     if valid_calibs is None:
         valid_calibs = calibration_data.valid_calibs
 
     for filt in filter_list:
         terminal_output.print_terminal(
             filt,
             string="Working on filter: {:s}",
             style_name='OKBLUE',
-            )
+        )
 
         ###
         #   Try magnitude transformation
         #
         success = False
         #   Loop over valid filter combination for the transformation
         for calib_fil in valid_calibs:
@@ -4843,63 +4863,60 @@
                         maxid=maxid,
                         refOBJ=[objID],
                         nmissed=nmissed,
                         bfrac=bfrac,
                         s_refOBJ=s_refOBJ,
                         correl_method=correl_method,
                         seplimit=seplimit,
-                        )
-
+                    )
 
                     ###
                     #   Reidentify position of the variable star
                     #
                     terminal_output.print_terminal(
                         string="Identify the variable star",
-                        )
+                    )
 
                     if correl_method == 'astropy':
                         objID, count, _, _ = correlate.posi_obj_astropy(
                             img_container.ensembles[filt].x_es,
                             img_container.ensembles[filt].y_es,
                             ra_obj,
                             dec_obj,
                             img_container.ensembles[filt].wcs,
                             seplimit=seplimit,
-                            )
+                        )
 
                     elif correl_method == 'own':
-                        inds_obj, count, _, _  = correlate.posi_obj_srcor(
+                        inds_obj, count, _, _ = correlate.posi_obj_srcor(
                             img_container.ensembles[filt].x_es,
                             img_container.ensembles[filt].y_es,
                             ra_obj,
                             dec_obj,
                             img_container.ensembles[filt].wcs,
                             dcr=dcr,
                             option=option,
                             verbose=verbose,
-                            )
+                        )
                         if verbose:
                             terminal_output.print_terminal()
 
                         #   Current object ID
-                        objID  = inds_obj[1]
+                        objID = inds_obj[1]
 
                     #   Set new object ID
                     img_container.ensembles[filt].variable_ID = objID
 
-
                     #   Check if variable star was detected
                     if count == 0:
                         raise RuntimeError(
                             f"{style.bcolors.FAIL} \tERROR: The variable "
                             "star was not detected in the reference image.\n"
                             f"\t-> EXIT {style.bcolors.ENDC}"
-                            )
-
+                        )
 
                     ###
                     #   Load calibration information
                     #
                     calib.deter_calib(
                         img_container,
                         calib_fil,
@@ -4907,35 +4924,34 @@
                         dcr=dcr,
                         option=option,
                         vizier_dict=vizier_dict,
                         calib_file=calib_file,
                         mag_range=mag_range,
                         correl_method=correl_method,
                         seplimit=seplimit,
-                        )
+                    )
                     terminal_output.print_terminal()
 
                     #   Stop here if calibration data is not available
                     filter_calib = img_container.calib_parameters.column_names
-                    if ('mag'+calib_fil[0] not in filter_calib or
-                        'mag'+calib_fil[1] not in filter_calib):
-                            if 'mag'+calib_fil[0] not in filter_calib:
-                                err_filter = calib_fil[0]
-                            if 'mag'+calib_fil[1] not in filter_calib:
-                                err_filter = calib_fil[1]
-                            terminal_output.print_terminal(
-                                err_filter,
-                                indent=2,
-                                string="Magnitude transformation not "\
-                                "possible because no calibration data "\
-                                "available for filter {}",
-                                style_name='WARNING',
-                                )
-                            break
-
+                    if ('mag' + calib_fil[0] not in filter_calib or
+                            'mag' + calib_fil[1] not in filter_calib):
+                        if 'mag' + calib_fil[0] not in filter_calib:
+                            err_filter = calib_fil[0]
+                        if 'mag' + calib_fil[1] not in filter_calib:
+                            err_filter = calib_fil[1]
+                        terminal_output.print_terminal(
+                            err_filter,
+                            indent=2,
+                            string="Magnitude transformation not " \
+                                   "possible because no calibration data " \
+                                   "available for filter {}",
+                            style_name='WARNING',
+                        )
+                        break
 
                     ###
                     #   Calibrate magnitudes
                     #
 
                     #   Set boolean regarding magnitude plot
                     plot_mags = True if plot_test or plot_ifi else False
@@ -4944,116 +4960,114 @@
                     #   transformation
                     trans.apply_calib(
                         img_container,
                         calib_fil,
                         Tcs=Tcs,
                         derive_Tcs=derive_Tcs,
                         plot_mags=plot_mags,
-                        ID=filt,
+                        # id_object=filt,
                         photo_type=photo_type,
                         refid=ref_ID,
                         plot_sigma=plot_sigma,
-                        )
+                    )
                     cali_mags = getattr(img_container, 'cali', None)
                     if not checks.check_unumpy_array(cali_mags):
                         cali = cali_mags['mag']
                     else:
                         cali = cali_mags
                     if np.all(cali == 0):
                         break
 
-
                     ###
                     #   Plot light curve
                     #
                     #   Create a Time object for the observation times
                     otime = Time(
                         img_container.ensembles[filt].get_obs_time(),
                         format='jd',
-                        )
+                    )
 
                     #   Create mask for time series to remove images
                     #   without entries
-                    #mask_ts = np.isin(
-                        ##cali_mags['med'][i][:,objID],
-                        #cali_mags[i][:,objID],
-                        #[0.],
-                        #invert=True
-                        #)
+                    # mask_ts = np.isin(
+                    ##cali_mags['med'][i][:,objID],
+                    # cali_mags[i][:,objID],
+                    # [0.],
+                    # invert=True
+                    # )
 
                     #   Create a time series object
                     ts = aux.mk_ts(
                         otime,
                         cali_mags[i],
                         filt,
                         objID,
-                        )
+                    )
 
                     #   Write time series
                     ts.write(
-                        outdir+'/tables/light_curce_'+filt+'.dat',
+                        outdir + '/tables/light_curce_' + filt + '.dat',
                         format='ascii',
                         overwrite=True,
-                        )
+                    )
                     ts.write(
-                        outdir+'/tables/light_curce_'+filt+'.csv',
+                        outdir + '/tables/light_curce_' + filt + '.csv',
                         format='ascii.csv',
                         overwrite=True,
-                        )
+                    )
 
                     #   Plot light curve over JD
                     plot.light_curve_jd(
                         ts,
                         filt,
-                        filt+'_err',
+                        filt + '_err',
                         outdir,
                         nameobj=nameobj
-                        )
+                    )
 
                     #   Plot the light curve folded on the period
                     plot.light_curve_fold(
                         ts,
                         filt,
-                        filt+'_err',
+                        filt + '_err',
                         outdir,
                         transit_time,
                         period,
                         binn=binn,
                         nameobj=nameobj,
-                        )
+                    )
 
                     success = True
                     break
 
-
         if not success:
             #   Load calibration information
             calib.deter_calib(
                 img_container,
                 [filt],
                 calib_method=calib_method,
                 dcr=dcr,
                 option=option,
                 vizier_dict=vizier_dict,
                 calib_file=calib_file,
                 mag_range=mag_range,
-                )
+            )
 
             #   Check if calibration data is available
             filter_calib = img_container.calib_parameters.column_names
-            if 'mag'+filt not in filter_calib:
+            if 'mag' + filt not in filter_calib:
                 terminal_output.print_terminal(
                     filt,
                     indent=2,
-                    string="Magnitude calibration not "\
-                    "possible because no calibration data is "\
-                    "available for filter {}. Use normalized flux for light "\
-                    "curve.",
+                    string="Magnitude calibration not " \
+                           "possible because no calibration data is " \
+                           "available for filter {}. Use normalized flux for light " \
+                           "curve.",
                     style_name='WARNING',
-                    )
+                )
 
                 #   Get ensemble
                 ensemble = img_container.ensembles[filt]
 
                 #   Quasi calibration of the flux data
                 trans.flux_calibrate_ensemble(ensemble)
 
@@ -5067,67 +5081,65 @@
 
                 #   Apply calibration
                 trans.apply_calib(
                     img_container,
                     [filt],
                     plot_mags=plot_mags,
                     photo_type=photo_type,
-                    )
+                )
                 plot_quantity = getattr(img_container, 'noT', None)[0]
 
-
             ###
             #   Plot light curve
             #
             #   Create a Time object for the observation times
             otime = Time(
                 img_container.ensembles[filt].get_obs_time(),
                 format='jd',
-                )
+            )
 
             #   Create a time series object
             ts = aux.mk_ts(
                 otime,
                 plot_quantity,
                 filt,
                 img_container.ensembles[filt].variable_ID,
-                )
+            )
 
             #   Write time series
             ts.write(
-                outdir+'/tables/light_curce_'+filt+'.dat',
+                outdir + '/tables/light_curce_' + filt + '.dat',
                 format='ascii',
                 overwrite=True,
-                )
+            )
             ts.write(
-                outdir+'/tables/light_curce_'+filt+'.csv',
+                outdir + '/tables/light_curce_' + filt + '.csv',
                 format='ascii.csv',
                 overwrite=True,
-                )
+            )
 
             #   Plot light curve over JD
             plot.light_curve_jd(
                 ts,
                 filt,
-                filt+'_err',
+                filt + '_err',
                 outdir,
                 nameobj=nameobj)
 
-
             #   Plot the light curve folded on the period
             plot.light_curve_fold(
                 ts,
                 filt,
-                filt+'_err',
+                filt + '_err',
                 outdir,
                 transit_time,
                 period,
                 binn=binn,
                 nameobj=nameobj,
-                )
+            )
 
 
 def subtract_archive_img_from_img(filt, name, path, outdir,
                                   wcs_method='astrometry', plot_comp=True,
                                   hips_source='CDS/P/DSS2/blue'):
     '''
         Subtraction of a reference/archival image from the input image.
@@ -5157,104 +5169,97 @@
             Default is ``CDS/P/DSS2/blue``.
     '''
     ###
     #   Check output directories
     #
     checks.check_out(
         outdir,
-        os.path.join(outdir,'subtract'),
-        )
-    outdir = os.path.join(outdir,'subtract')
-
+        os.path.join(outdir, 'subtract'),
+    )
+    outdir = os.path.join(outdir, 'subtract')
 
     ###
     #   Check input path
     #
     checks.check_file(path)
 
-
     ###
     #   Trim image as needed (currently images with < 4*10^6 are required)
     #
     #   Load image
     img = CCDData.read(path)
 
     #   Trim
     xtrim = 2501
-    #xtrim = 2502
+    # xtrim = 2502
     ytrim = 1599
     img = ccdp.trim_image(img[0:ytrim, 0:xtrim])
     img.meta['NAXIS1'] = xtrim
     img.meta['NAXIS2'] = ytrim
 
     #   Save trimmed file
-    basename  = base_aux.get_basename(path)
-    file_name = basename+'_trimmed.fit'
+    basename = base_aux.get_basename(path)
+    file_name = basename + '_trimmed.fit'
     file_path = os.path.join(outdir, file_name)
     img.write(file_path, overwrite=True)
 
-
     ###
     #   Initialize image ensemble object
     #
     img_ensemble = image_ensemble(
         filt,
         name,
-        #file_path,
+        # file_path,
         path,
         outdir,
         0,
-        )
-
+    )
 
     ###
     #   Find the WCS solution for the image
     #
     aux.find_wcs(
         img_ensemble,
         ref_id=0,
         method=wcs_method,
         indent=3,
-        )
-
+    )
 
     ###
     #   Get image via hips2fits
     #
-    #from astropy.utils import data
-    #data.Conf.remote_timeout=600
+    # from astropy.utils import data
+    # data.Conf.remote_timeout=600
     hipsInstance = hips2fitsClass()
     hipsInstance.timeout = 120000
-    #hipsInstance.timeout = 1200000000
-    #hipsInstance.timeout = (200000000, 200000000)
+    # hipsInstance.timeout = 1200000000
+    # hipsInstance.timeout = (200000000, 200000000)
     hipsInstance.server = "https://alaskybis.cds.unistra.fr/hips-image-services/hips2fits"
     print(hipsInstance.timeout)
     print(hipsInstance.server)
-    #hips_hdus = hips2fits.query_with_wcs(
+    # hips_hdus = hips2fits.query_with_wcs(
     hips_hdus = hipsInstance.query_with_wcs(
         hips=hips_source,
         wcs=img_ensemble.wcs,
         get_query_payload=False,
         format='fits',
         verbose=True,
-        )
+    )
     #   Save downloaded file
     hips_hdus.writeto(os.path.join(outdir, 'hips.fits'), overwrite=True)
 
-
     ###
     #   Plot original and reference image
     #
     if plot_comp:
         plot.comp_img(
             outdir,
             img_ensemble.image_list[0].get_data(),
             hips_hdus[0].data,
-            )
-
+        )
 
     ###
     #   Perform image subtraction
     #
     #   Get image and image data
     img = img_ensemble.image_list[0].read_image()
     hips_data = hips_hdus[0].data.astype('float64').byteswap().newbyteorder()
@@ -5262,16 +5267,16 @@
     #   Run hotpants
     subtraction.run_hotpants(
         img.data,
         hips_data,
         img.mask,
         np.zeros(hips_data.shape, dtype=bool),
         image_gain=1.,
-        #template_gain=1,
+        # template_gain=1,
         template_gain=None,
         err=img.uncertainty.array,
-        #err=True,
+        # err=True,
         template_err=True,
-        #verbose=True,
+        # verbose=True,
         _workdir=outdir,
-        #_exe=exe_path,
-        )
+        # _exe=exe_path,
+    )
```

### Comparing `ost_photometry-0.0.7/src/ost_photometry/analyze/aux.py` & `ost_photometry-0.0.8/src/ost_photometry/analyze/aux.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-
 ############################################################################
 ####                            Libraries                               ####
 ############################################################################
 
 import sys
 
 import numpy as np
 
 from uncertainties import unumpy
 
-from pathlib import Path
-
 import pandas as pd
 
 from pytimedinput import timedInput
 
 from astropy.table import Table
 from astropy.stats import sigma_clipped_stats, sigma_clip
 from astropy.io import fits
@@ -23,248 +20,249 @@
 from astropy.modeling import models, fitting
 import astropy.units as u
 from astropy import wcs
 
 from astroquery.simbad import Simbad
 from astroquery.vizier import Vizier
 
+from photutils.utils import ImageDepth
+
 from regions import (
-    RectangleSkyRegion,
-    RectanglePixelRegion,
+    # RectangleSkyRegion,
+    # RectanglePixelRegion,
     PixCoord,
     CirclePixelRegion,
     Regions,
-    )
+)
 
 from sklearn.cluster import SpectralClustering
 
-import twirl
-
 import multiprocessing as mp
 
 import scipy.optimize as optimization
 
 from .. import aux as base_aux
 
-from .. import checks, style, terminal_output
+from .. import checks, style, terminal_output, calibration_data
 
 from . import plot
 
+
 ############################################################################
 ####                        Routines & definitions                      ####
 ############################################################################
 
+
 def err_prop(*args):
-    '''
+    """
         Calculate error propagation
 
         Parameters
         ----------
         args        : `list`
             List of errors that should be added
 
         Returns
         -------
-        u           : `float`
+        sum_error   : `float`
             Summed up error
-    '''
-    u = 0
+    """
+    sum_error = 0
     #   Adding up the errors
     for x in args:
-        u = np.sqrt(np.square(u) + np.square(x))
-    return u
-
-
-def mk_cmd_table(ind_sort, x, y, mags, list_bands):
-    '''
-        Create and export the CMD
-
-        Parameters
-        ----------
-        ind_sort        : `numpy.ndarray`
-            IDs of the stars
-
-        x               : `numpy.ndarray`
-            Position of the stars on the image in pixel in X direction
-
-        y               : `numpy.ndarray`
-            Position of the stars on the image in pixel in X direction
-
-        mags            : `numpy.ndarray`
-            Magnitudes of all stars
-
-        list_bands      : `list`
-            Filter
-
-        Returns
-        -------
-        tbl_cmd         : `astropy.table.Table`
-            Table with CMD data
-    '''
-    #   Number of filter
-    nfilter    = len(list_bands)
-
-    #   Dimensions of magnitude array & number of images
-    shape = mags['err'].shape
-    dim = len(shape)
-    if dim == 2:
-        nimg = 1
-    else:
-        nimg = shape[1]
-
-    # Make CMD table
-    tbl_cmd = Table(
-        names=['i','x', 'y',],
-        data=[
-            np.intc(ind_sort),
-            x,
-            y,
-            ]
-        )
-
-    #   Set name of the magnitude field
-    if 'med' in mags.dtype.names:
-        name_mag = 'med'
-    else:
-        name_mag = 'mag'
-
-    #   Add magnitude columns to CMD table
-    for i in range(0, nfilter):
-        if dim == 2:
-            if 'err' in mags.dtype.names:
-                tbl_cmd.add_columns(
-                    [
-                        mags[name_mag][i],
-                        mags['err'][i],
-                        ],
-                    names=[
-                        list_bands[i]+' [mag]',
-                        list_bands[i]+'_err [mag]',
-                        ]
-                    )
-            else:
-                tbl_cmd.add_column(
-                    mags[name_mag][i],
-                    name=list_bands[i]+' [mag]'
-                    )
-
-            if i != 0:
-                tbl_cmd.add_column(
-                    mags[name_mag][i-1] - mags[name_mag][i],
-                    name=list_bands[i-1]+'-'+list_bands[i]+' [mag]'
-                    )
-        else:
-            for j in range(0, nimg):
-                if nimg == 1:
-                    if 'err' in mags.dtype.names:
-                        tbl_cmd.add_columns(
-                            [
-                                mags[name_mag][i][j],
-                                mags['err'][i][j],
-                                ],
-                            names=[
-                                list_bands[i]+' [mag]',
-                                list_bands[i]+'_err [mag]',
-                                ]
-                            )
-                        if i != 0:
-                            tbl_cmd.add_columns(
-                                [
-                                    mags[name_mag][i-1][j]-mags[name_mag][i][j],
-                                    err_prop(
-                                        mags['err'][i-1][j],
-                                        mags['err'][i][j],
-                                        ),
-                                    ],
-                                names=[
-                                    list_bands[i-1]+'-'+list_bands[i]+' [mag]',
-                                    list_bands[i-1]+'-'\
-                                        +list_bands[i]+'_err [mag]',
-                                    ]
-                                )
-                    else:
-                        tbl_cmd.add_column(
-                            mags[name_mag][i][j],
-                            name=list_bands[i]+' [mag]'
-                            )
+        sum_error = np.sqrt(np.square(u) + np.square(x))
+    return sum_error
 
-                        if i != 0:
-                            tbl_cmd.add_column(
-                                mags[name_mag][i-1][j] - mags[name_mag][i][j],
-                                name=list_bands[i-1]+'-'+list_bands[i]+' [mag]'
-                                )
-
-                else:
-                    if 'err' in mags.dtype.names:
-                        tbl_cmd.add_columns(
-                            [
-                                mags[name_mag][i][j],
-                                mags['err'][i][j],
-                                ],
-                            names=[
-                                list_bands[i]+' [mag] ('+str(j)+')',
-                                list_bands[i]+'_err [mag] ('+str(j)+')',
-                                ]
-                            )
-                        if i != 0:
-                            tbl_cmd.add_columns(
-                                [
-                                    mags[name_mag][i-1][j]-mags[name_mag][i][j],
-                                    err_prop(
-                                        mags['err'][i-1][j],
-                                        mags['err'][i][j],
-                                        ),
-                                    ],
-                                names=[
-                                    list_bands[i-1]+'-'+list_bands[i]\
-                                        +' [mag] ('+str(j)+')',
-                                    list_bands[i-1]+'-'+list_bands[i]\
-                                        +'_err [mag] ('+str(j)+')',
-                                    ]
-                                )
-
-                    else:
-                        tbl_cmd.add_column(
-                            mags[name_mag][i][j],
-                            name=list_bands[i]+' [mag] ('+str(j)+')'
-                            )
-                        if i != 0:
-                            tbl_cmd.add_column(
-                                mags[name_mag][i-1][j] - mags[name_mag][i][j],
-                                name=list_bands[i-1]+'-'+list_bands[i]\
-                                        +' [mag] ('+str(j)+')'
-                                )
-
-    #   Sort CMD table
-    if nimg == 1:
-        tbl_cmd = tbl_cmd.group_by(list_bands[0]+' [mag]')
-    else:
-        tbl_cmd = tbl_cmd.group_by(list_bands[0]+' [mag] (0)')
 
-    return tbl_cmd
+# def mk_cmd_table(ind_sort, x, y, mags, list_bands):
+#     """
+#         Create and export the CMD
+#
+#         Parameters
+#         ----------
+#         ind_sort        : `numpy.ndarray`
+#             IDs of the stars
+#
+#         x               : `numpy.ndarray`
+#             Position of the stars on the image in pixel in X direction
+#
+#         y               : `numpy.ndarray`
+#             Position of the stars on the image in pixel in X direction
+#
+#         mags            : `numpy.ndarray`
+#             Magnitudes of all stars
+#
+#         list_bands      : `list`
+#             Filter
+#
+#         Returns
+#         -------
+#         tbl_cmd         : `astropy.table.Table`
+#             Table with CMD data
+#     """
+#     #   Number of filter
+#     nfilter = len(list_bands)
+#
+#     #   Dimensions of magnitude array & number of images
+#     shape = mags['err'].shape
+#     dim = len(shape)
+#     if dim == 2:
+#         nimg = 1
+#     else:
+#         nimg = shape[1]
+#
+#     # Make CMD table
+#     tbl_cmd = Table(
+#         names=['i', 'x', 'y'],
+#         data=[
+#             np.intc(ind_sort),
+#             x,
+#             y,
+#         ]
+#     )
+#
+#     #   Set name of the magnitude field
+#     if 'med' in mags.dtype.names:
+#         name_mag = 'med'
+#     else:
+#         name_mag = 'mag'
+#
+#     #   Add magnitude columns to CMD table
+#     for i in range(0, nfilter):
+#         if dim == 2:
+#             if 'err' in mags.dtype.names:
+#                 tbl_cmd.add_columns(
+#                     [
+#                         mags[name_mag][i],
+#                         mags['err'][i],
+#                     ],
+#                     names=[
+#                         list_bands[i] + ' [mag]',
+#                         list_bands[i] + '_err [mag]',
+#                     ]
+#                 )
+#             else:
+#                 tbl_cmd.add_column(
+#                     mags[name_mag][i],
+#                     name=list_bands[i] + ' [mag]'
+#                 )
+#
+#             if i != 0:
+#                 tbl_cmd.add_column(
+#                     mags[name_mag][i - 1] - mags[name_mag][i],
+#                     name=list_bands[i - 1] + '-' + list_bands[i] + ' [mag]'
+#                 )
+#         else:
+#             for j in range(0, nimg):
+#                 if nimg == 1:
+#                     if 'err' in mags.dtype.names:
+#                         tbl_cmd.add_columns(
+#                             [
+#                                 mags[name_mag][i][j],
+#                                 mags['err'][i][j],
+#                             ],
+#                             names=[
+#                                 list_bands[i] + ' [mag]',
+#                                 list_bands[i] + '_err [mag]',
+#                             ]
+#                         )
+#                         if i != 0:
+#                             tbl_cmd.add_columns(
+#                                 [
+#                                     mags[name_mag][i - 1][j] - mags[name_mag][i][j],
+#                                     err_prop(
+#                                         mags['err'][i - 1][j],
+#                                         mags['err'][i][j],
+#                                     ),
+#                                 ],
+#                                 names=[
+#                                     f'{list_bands[i - 1]}-{list_bands[i]} [mag]',
+#                                     f'{list_bands[i - 1]}-{list_bands[i]}_err [mag]',
+#                                 ]
+#                             )
+#                     else:
+#                         tbl_cmd.add_column(
+#                             mags[name_mag][i][j],
+#                             name=list_bands[i] + ' [mag]'
+#                         )
+#
+#                         if i != 0:
+#                             tbl_cmd.add_column(
+#                                 mags[name_mag][i - 1][j] - mags[name_mag][i][j],
+#                                 name=list_bands[i - 1] + '-' + list_bands[i] + ' [mag]'
+#                             )
+#
+#                 else:
+#                     if 'err' in mags.dtype.names:
+#                         tbl_cmd.add_columns(
+#                             [
+#                                 mags[name_mag][i][j],
+#                                 mags['err'][i][j],
+#                             ],
+#                             names=[
+#                                 list_bands[i] + ' [mag] (' + str(j) + ')',
+#                                 list_bands[i] + '_err [mag] (' + str(j) + ')',
+#                             ]
+#                         )
+#                         if i != 0:
+#                             tbl_cmd.add_columns(
+#                                 [
+#                                     mags[name_mag][i - 1][j] - mags[name_mag][i][j],
+#                                     err_prop(
+#                                         mags['err'][i - 1][j],
+#                                         mags['err'][i][j],
+#                                     ),
+#                                 ],
+#                                 names=[
+#                                     list_bands[i - 1] + '-' + list_bands[i] \
+#                                     + ' [mag] (' + str(j) + ')',
+#                                     list_bands[i - 1] + '-' + list_bands[i] \
+#                                     + '_err [mag] (' + str(j) + ')',
+#                                 ]
+#                             )
+#
+#                     else:
+#                         tbl_cmd.add_column(
+#                             mags[name_mag][i][j],
+#                             name=list_bands[i] + ' [mag] (' + str(j) + ')'
+#                         )
+#                         if i != 0:
+#                             tbl_cmd.add_column(
+#                                 mags[name_mag][i - 1][j] - mags[name_mag][i][j],
+#                                 name=list_bands[i - 1] + '-' + list_bands[i] \
+#                                      + ' [mag] (' + str(j) + ')'
+#                             )
+#
+#     #   Sort CMD table
+#     if nimg == 1:
+#         tbl_cmd = tbl_cmd.group_by(list_bands[0] + ' [mag]')
+#     else:
+#         tbl_cmd = tbl_cmd.group_by(list_bands[0] + ' [mag] (0)')
+#
+#     return tbl_cmd
 
 
 def mk_mag_table(*args, **kwargs):
-    '''
+    """
         Create and export astropy table with object positions and magnitudes
 
         Distinguishes between different input magnitude array types.
         Possibilities: unumpy.uarray & numpy structured ndarray
-    '''
+    """
     #   Get type of the magnitude arrays
     unc = checks.check_unumpy_array(args[3])
 
     if unc:
         return mk_mag_table_unc(*args, **kwargs)
     else:
         return mk_mag_table_str(*args, **kwargs)
 
 
 def mk_mag_table_str(ind_sort, x, y, mags, list_bands, id_tupels):
-    '''
+    """
         Create and export astropy table with object positions and magnitudes
         Input magnitude array is expected to be a numpy structured array.
 
         Parameters
         ----------
         ind_sort        : `numpy.ndarray`
             IDs of the stars
@@ -286,81 +284,75 @@
                       for the color calculation, ID of the images to
                       position 2)
 
         Returns
         -------
         tbl_cmd         : `astropy.table.Table`
             Table with CMD data
-    '''
-    #   Number of filter
-    nfilter    = len(list_bands)
-
+    """
     # Make CMD table
     tbl_cmd = Table(
-        names=['i','x', 'y',],
+        names=['i', 'x', 'y', ],
         data=[
             np.intc(ind_sort),
             x,
             y,
-            ]
-        )
+        ]
+    )
 
     #   Set name of the magnitude field
     name_mag = 'mag'
 
-    #   Add magnitude columns to CMD table
+    #   Add magnitude columns to table
     for ids in id_tupels:
         if 'err' in mags.dtype.names:
             tbl_cmd.add_columns(
                 [
-                    mags[name_mag][ids[0]][ids[1]],
-                    mags['err'][ids[0]][ids[1]],
-                    ],
+                    mags[name_mag][ids[0]][ids[1]] * u.mag,
+                    mags['err'][ids[0]][ids[1]] * u.mag,
+                ],
                 names=[
-                    list_bands[ids[0]]+' [mag] ('+str(ids[1])+')',
-                    list_bands[ids[0]]+'_err [mag] ('+str(ids[1])+')',
-                    ]
-                )
+                    f'{list_bands[ids[0]]} ({ids[1]})',
+                    f'{list_bands[ids[0]]}_err ({ids[1]})',
+                ]
+            )
             if len(id_tupels) == 4:
                 tbl_cmd.add_columns(
                     [
-                    mags[name_mag][ids[2]][ids[3]]\
-                        - mags[name_mag][ids[0]][ids[1]],
-                    err_prop(
-                        mags['err'][ids[2]][ids[3]],
-                        mags['err'][ids[0]][ids[1]],
-                        ),
+                        (mags[name_mag][ids[2]][ids[3]]
+                         - mags[name_mag][ids[0]][ids[1]]) * u.mag,
+                        err_prop(
+                            mags['err'][ids[2]][ids[3]],
+                            mags['err'][ids[0]][ids[1]],
+                        ) * u.mag,
                     ],
                     names=[
-                        list_bands[ids[2]]+'-'+list_bands[ids[0]]\
-                            +' [mag] ('+str(ids[1])+')',
-                        list_bands[ids[2]]+'-'+list_bands[ids[0]]\
-                            +'_err [mag] ('+str(ids[1])+')',
-                        ]
-                    )
+                        f'{list_bands[ids[2]]}-{list_bands[ids[0]]} ({ids[1]})',
+                        f'{list_bands[ids[2]]}-{list_bands[ids[0]]}_err ({ids[1]})',
+                    ]
+                )
 
         else:
             tbl_cmd.add_column(
-                mags[name_mag][ids[0]][ids[1]],
-                name=list_bands[ids[0]]+' [mag] ('+str(ids[1])+')'
-                )
+                mags[name_mag][ids[0]][ids[1]] * u.mag,
+                name=f'{list_bands[ids[0]]} ({ids[1]})'
+            )
             tbl_cmd.add_column(
-                mags[name_mag][ids[2]][ids[3]]-mags[name_mag][ids[0]][ids[1]],
-                name=list_bands[ids[2]]+'-'+list_bands[ids[0]]\
-                        +' [mag] ('+str(ids[1])+')'
-                )
+                (mags[name_mag][ids[2]][ids[3]] - mags[name_mag][ids[0]][ids[1]]) * u.mag,
+                name=f'{list_bands[ids[2]]}-{list_bands[ids[0]]} ({ids[1]})'
+            )
 
-    #   Sort CMD table
-    tbl_cmd = tbl_cmd.group_by(list_bands[0]+' [mag] (0)')
+    #   Sort table
+    tbl_cmd = tbl_cmd.group_by(f'{list_bands[0]} (0)')
 
     return tbl_cmd
 
 
 def mk_mag_table_unc(ind_sort, x, y, mags, list_bands, id_tupels):
-    '''
+    """
         Create and export astropy table with object positions and magnitudes
         Input magnitude array is expected to be a unumpy uarray.
 
         Parameters
         ----------
         ind_sort        : `numpy.ndarray`
             IDs of the stars
@@ -382,193 +374,183 @@
                       for the color calculation, ID of the images to
                       position 2)
 
         Returns
         -------
         tbl_cmd         : `astropy.table.Table`
             Table with CMD data
-    '''
-    #   Number of filter
-    nfilter    = len(list_bands)
-
+    """
     # Make CMD table
     tbl_cmd = Table(
-        names=['i','x', 'y',],
+        names=['i', 'x', 'y', ],
         data=[
             np.intc(ind_sort),
             x,
             y,
-            ]
-        )
+        ]
+    )
 
-    #   Add magnitude columns to CMD table
+    #   Add magnitude columns to table
     for ids in id_tupels:
         tbl_cmd.add_columns(
             [
-                unumpy.nominal_values(mags[ids[0]][ids[1]]),
-                unumpy.std_devs(mags[ids[0]][ids[1]]),
-                ],
+                unumpy.nominal_values(mags[ids[0]][ids[1]]) * u.mag,
+                unumpy.std_devs(mags[ids[0]][ids[1]]) * u.mag,
+            ],
             names=[
-                list_bands[ids[0]]+' [mag] ('+str(ids[1])+')',
-                list_bands[ids[0]]+'_err [mag] ('+str(ids[1])+')',
-                ]
-            )
+                f'{list_bands[ids[0]]} ({ids[1]})',
+                f'{list_bands[ids[0]]}_err ({ids[1]})',
+            ]
+        )
         if len(id_tupels) == 4:
             color = mags[ids[2]][ids[3]] - mags[ids[0]][ids[1]]
             tbl_cmd.add_columns(
                 [
-                    unumpy.nominal_values(color),
-                    unumpy.std_devs(color),
+                    unumpy.nominal_values(color) * u.mag,
+                    unumpy.std_devs(color) * u.mag,
                 ],
                 names=[
-                    list_bands[ids[2]]+'-'+list_bands[ids[0]]\
-                        +' [mag] ('+str(ids[1])+')',
-                    list_bands[ids[2]]+'-'+list_bands[ids[0]]\
-                        +'_err [mag] ('+str(ids[1])+')',
-                    ]
-                )
-
+                    f'{list_bands[ids[2]]}-{list_bands[ids[0]]} ({ids[1]})',
+                    f'{list_bands[ids[2]]}-{list_bands[ids[0]]}_err ({ids[1]})',
+                ]
+            )
 
-    #   Sort CMD table
+    #   Sort table
     tbl_cmd = tbl_cmd.group_by(
-        list_bands[id_tupels[0][0]]+' [mag] ('+str(id_tupels[0][1])+')'
-        )
+        f'{list_bands[id_tupels[0][0]]} ({id_tupels[0][1]})'
+    )
 
     return tbl_cmd
 
 
-def mk_cmd_table_u(ind_sort, x, y, mags, list_bands):
-    '''
-        Create and export the CMD
-
-        Parameters
-        ----------
-        ind_sort        : `numpy.ndarray`
-            IDs of the stars
-
-        x               : `numpy.ndarray`
-            Position of the stars on the image in pixel in X direction
-
-        y               : `numpy.ndarray`
-            Position of the stars on the image in pixel in X direction
-
-        mags            : `unumpy.ndarray`
-            Magnitudes of all stars
-
-        list_bands      : `list`
-            Filter
-
-        Returns
-        -------
-        tbl_cmd         : `astropy.table.Table`
-            Table with CMD data
-    '''
-    #   Number of filter
-    nfilter    = len(list_bands)
-
-    #   Dimensions of magnitude array & number of images
-    shape = mags.shape
-    dim = len(shape)
-    if dim == 2:
-        nimg = 1
-    else:
-        nimg = shape[1]
-
-    # Make CMD table
-    tbl_cmd = Table(
-        names=['i','x', 'y',],
-        data=[
-            np.intc(ind_sort),
-            x,
-            y,
-            ]
-        )
-
-    #   Add magnitude columns to CMD table
-    for i in range(0, nfilter):
-        if dim == 2:
-            tbl_cmd.add_columns(
-                [
-                    unumpy.nominal_values(mags)[i],
-                    unumpy.std_devs(mags)[i],
-                    ],
-                names=[
-                    list_bands[i]+' [mag]',
-                    list_bands[i]+'_err [mag]',
-                    ]
-                )
-
-            if i != 0:
-                tbl_cmd.add_column(
-                    unumpy.nominal_values(mags[i-1] - mags[i]),
-                    name=list_bands[i-1]+'-'+list_bands[i]+' [mag]'
-                    )
-        else:
-            for j in range(0, nimg):
-                if nimg == 1:
-                    tbl_cmd.add_columns(
-                        [
-                            unumpy.nominal_values(mags)[i][j],
-                            unumpy.std_devs(mags)[i][j],
-                            ],
-                        names=[
-                            list_bands[i]+' [mag]',
-                            list_bands[i]+'_err [mag]',
-                            ]
-                        )
-                    if i != 0:
-                        tbl_cmd.add_columns(
-                            [
-                                unumpy.nominal_values(mags[i-1][j]-mags[i][j]),
-                                unumpy.std_devs(mags[i-1][j]-mags[i][j]),
-                                ],
-                            names=[
-                                list_bands[i-1]+'-'+list_bands[i]+' [mag]',
-                                list_bands[i-1]+'-'\
-                                    +list_bands[i]+'_err [mag]',
-                                ]
-                            )
-                else:
-                    tbl_cmd.add_columns(
-                        [
-                            unumpy.nominal_values(mags[i][j]),
-                            unumpy.std_devs(mags[i][j]),
-                            ],
-                        names=[
-                            list_bands[i]+' [mag] ('+str(j)+')',
-                            list_bands[i]+'_err [mag] ('+str(j)+')',
-                            ]
-                        )
-                    if i != 0:
-                        tbl_cmd.add_columns(
-                            [
-                                unumpy.nominal_values(mags[i-1][j]-mags[i][j]),
-                                unumpy.std_devs(mags[i-1][j]-mags[i][j]),
-                                ],
-                            names=[
-                                list_bands[i-1]+'-'+list_bands[i]\
-                                    +' [mag] ('+str(j)+')',
-                                list_bands[i-1]+'-'+list_bands[i]\
-                                    +'_err [mag] ('+str(j)+')',
-                                ]
-                            )
-
-
-    #   Sort CMD table
-    if nimg == 1:
-        tbl_cmd = tbl_cmd.group_by(list_bands[0]+' [mag]')
-    else:
-        tbl_cmd = tbl_cmd.group_by(list_bands[0]+' [mag] (0)')
-
-    return tbl_cmd
+# def mk_cmd_table_u(ind_sort, x, y, mags, list_bands):
+#     """
+#         Create and export the CMD
+#
+#         Parameters
+#         ----------
+#         ind_sort        : `numpy.ndarray`
+#             IDs of the stars
+#
+#         x               : `numpy.ndarray`
+#             Position of the stars on the image in pixel in X direction
+#
+#         y               : `numpy.ndarray`
+#             Position of the stars on the image in pixel in X direction
+#
+#         mags            : `unumpy.ndarray`
+#             Magnitudes of all stars
+#
+#         list_bands      : `list`
+#             Filter
+#
+#         Returns
+#         -------
+#         tbl_cmd         : `astropy.table.Table`
+#             Table with CMD data
+#     """
+#     #   Number of filter
+#     nfilter = len(list_bands)
+#
+#     #   Dimensions of magnitude array & number of images
+#     shape = mags.shape
+#     dim = len(shape)
+#     if dim == 2:
+#         nimg = 1
+#     else:
+#         nimg = shape[1]
+#
+#     # Make CMD table
+#     tbl_cmd = Table(
+#         names=['i', 'x', 'y', ],
+#         data=[
+#             np.intc(ind_sort),
+#             x,
+#             y,
+#         ]
+#     )
+#
+#     #   Add magnitude columns to CMD table
+#     for i in range(0, nfilter):
+#         if dim == 2:
+#             tbl_cmd.add_columns(
+#                 [
+#                     unumpy.nominal_values(mags)[i] * u.mag,
+#                     unumpy.std_devs(mags)[i] * u.mag,
+#                 ],
+#                 names=[
+#                     f'{list_bands[i]}',
+#                     f'{list_bands[i]}_err',
+#                 ]
+#             )
+#
+#             if i != 0:
+#                 tbl_cmd.add_column(
+#                     unumpy.nominal_values(mags[i - 1] - mags[i]) * u.mag,
+#                     name=f'{list_bands[i - 1]}-{list_bands[i]}'
+#                 )
+#         else:
+#             for j in range(0, nimg):
+#                 if nimg == 1:
+#                     tbl_cmd.add_columns(
+#                         [
+#                             unumpy.nominal_values(mags)[i][j] * u.mag,
+#                             unumpy.std_devs(mags)[i][j] * u.mag,
+#                         ],
+#                         names=[
+#                             f'{list_bands[i]}',
+#                             f'{list_bands[i]}_err',
+#                         ]
+#                     )
+#                     if i != 0:
+#                         tbl_cmd.add_columns(
+#                             [
+#                                 unumpy.nominal_values(mags[i - 1][j] - mags[i][j]) * u.mag,
+#                                 unumpy.std_devs(mags[i - 1][j] - mags[i][j]) * u.mag,
+#                             ],
+#                             names=[
+#                                 f'{list_bands[i - 1]}-{list_bands[i]}',
+#                                 f'{list_bands[i - 1]}-{list_bands[i]}_err',
+#                             ]
+#                         )
+#                 else:
+#                     tbl_cmd.add_columns(
+#                         [
+#                             unumpy.nominal_values(mags[i][j]) * u.mag,
+#                             unumpy.std_devs(mags[i][j]) * u.mag,
+#                         ],
+#                         names=[
+#                             f'{list_bands[i]} ({j}) ',
+#                             f'{list_bands[i]}_err ({j})',
+#                         ]
+#                     )
+#                     if i != 0:
+#                         tbl_cmd.add_columns(
+#                             [
+#                                 unumpy.nominal_values(mags[i - 1][j] - mags[i][j]) * u.mag,
+#                                 unumpy.std_devs(mags[i - 1][j] - mags[i][j]) * u.mag,
+#                             ],
+#                             names=[
+#                                 f'{list_bands[i - 1]}-{list_bands[i]} ({j})',
+#                                 f'{list_bands[i - 1]}-{list_bands[i]}_err ({j})',
+#                             ]
+#                         )
+#
+#     #   Sort CMD table
+#     if nimg == 1:
+#         tbl_cmd = tbl_cmd.group_by(f'{list_bands[0]}')
+#     else:
+#         tbl_cmd = tbl_cmd.group_by(f'{list_bands[0]} (0)')
+#
+#     return tbl_cmd
 
 
 def find_wcs(image_ensemble, ref_id=None, method='astrometry', rmcos=False,
              path_cos=None, x=None, y=None, force_wcs_determ=False, indent=2):
-    '''
+    """
         Meta function for finding image WCS
 
         Parameters
         ----------
         image_ensemble  : `image.ensemble.class`
             Image class with all images taken in a specific filter
 
@@ -598,15 +580,15 @@
             If ``True`` a new WCS determination will be calculated even if
             a WCS is already present in the FITS Header.
             Default is ``False``.
 
         indent          : `integer`, optional
             Indentation for the console output lines
             Default is ``2``.
-    '''
+    """
     if ref_id is not None:
         #   Image
         img = image_ensemble.image_list[ref_id]
 
         #   Test if the image contains already a WCS
         cal_wcs, wcs_file = base_aux.check_wcs_exists(img)
 
@@ -615,40 +597,40 @@
             if method == 'astrometry':
                 image_ensemble.set_wcs(
                     base_aux.find_wcs_astrometry(
                         img,
                         rmcos=rmcos,
                         path_cos=path_cos,
                         indent=indent,
-                        )
                     )
+                )
 
             #   Calculate WCS -> ASTAP program
             elif method == 'astap':
                 image_ensemble.set_wcs(
                     base_aux.find_wcs_astap(img, indent=indent)
-                    )
+                )
 
             #   Calculate WCS -> twirl libary
             elif method == 'twirl':
                 if x is None or y is None:
                     raise RuntimeError(
                         f"{style.bcolors.FAIL} \nException in find_wcs(): '"
                         f"\n'x' or 'y' is None -> Exit {style.bcolors.ENDC}"
-                        )
+                    )
                 image_ensemble.set_wcs(
                     base_aux.find_wcs_twirl(img, x, y, indent=indent)
-                    )
+                )
             #   Raise exception
             else:
                 raise RuntimeError(
                     f"{style.bcolors.FAIL} \nException in find_wcs(): '"
                     f"\nWCS method not known -> Supplied method was {method}"
                     f"{style.bcolors.ENDC}"
-                    )
+                )
         else:
             image_ensemble.set_wcs(extract_wcs(wcs_file))
     else:
         for i, img in enumerate(image_ensemble.image_list):
             #   Test if the image contains already a WCS
             cal_wcs = base_aux.check_wcs_exists(img)
 
@@ -656,44 +638,46 @@
                 #   Calculate WCS -> astrometry.net
                 if method == 'astrometry':
                     w = base_aux.find_wcs_astrometry(
                         img,
                         rmcos=rmcos,
                         path_cos=path_cos,
                         indent=indent,
-                        )
+                    )
 
                 #   Calculate WCS -> ASTAP program
                 elif method == 'astap':
                     w = base_aux.find_wcs_astap(img, indent=indent)
 
                 #   Calculate WCS -> twirl libary
                 elif method == 'twirl':
                     if x is None or y is None:
                         raise RuntimeError(
                             f"{style.bcolors.FAIL} \nException in "
                             "find_wcs(): ' \n'x' or 'y' is None -> Exit"
                             f"{style.bcolors.ENDC}"
-                            )
+                        )
                     w = base_aux.find_wcs_twirl(img, x, y, indent=indent)
 
                 #   Raise exception
                 else:
                     raise RuntimeError(
                         f"{style.bcolors.FAIL} \nException in find_wcs(): '"
                         "\nWCS method not known -> Supplied method was "
                         f"{method} {style.bcolors.ENDC}"
-                        )
+                    )
+            else:
+                w = wcs.WCS(fits.open(img.path)[0].header)
 
             if i == 0:
                 image_ensemble.set_wcs(w)
 
 
 def extract_wcs(wcs_path, image_wcs=None, rmcos=False, filters=None):
-    '''
+    """
         Load wcs from FITS file
 
         Parameters
         ----------
         wcs_path         : `string`
             Path to the image with the WCS or path to the directory that
             contains this image
@@ -706,105 +690,105 @@
         rmcos           : `boolean`, optional
             If True cosmic rays will be removed.
             Default is ``False``.
 
         filters         : `list` of `string`, optional
             Filter list
             Default is ``None``.
-    '''
+    """
     #   Open the image with the WCS solution
     if image_wcs is not None:
         if rmcos:
             if filters is None:
                 raise Exception(
                     f"{style.bcolors.FAIL} \nException in extract_wcs(): '"
                     "\n'rmcos=True' buit no 'filters' given -> Exit"
                     f"{style.bcolors.ENDC}"
-                    )
+                )
             basename = f'img_cut_{filters[0]}_lacosmic'
         else:
             basename = image_wcs.split('/')[-1].split('.')[0]
         hdulist = fits.open(f'{wcs_path}/{basename}.new')
     else:
         hdulist = fits.open(wcs_path)
 
     #   Extract the WCS
     w = wcs.WCS(hdulist[0].header)
 
     return w
 
 
-def mk_ts(obs_time, cali_mags, filt, objID):
-    '''
+def mk_ts(obs_time, cali_mags, filt, obj_id):
+    """
         Make a time series object
 
         Parameters
         ----------
-        obs_time        : `numpy.ndarray`
+        obs_time        : `astropy.time.Time`
             Observation times
 
         cali_mags       : `numpy.ndarray`
             Magnitudes and uncertainties
 
-        filt            : `filter`
-            Filte
+        filt            : `string`
+            Filter
 
-        objID           : `integer`
+        obj_id          : `integer`
             ID/Number of the object for with the time series should be
             created
 
         Returns
         -------
         ts              : `astropy.timeseries.TimeSeries`
-    '''
+    """
     #   Extract magnitudes of the object 'objID' depending on array dtype
     if checks.check_unumpy_array(cali_mags):
-        umags = cali_mags[:,objID]
+        umags = cali_mags[:, obj_id]
         mags_obj = unumpy.nominal_values(umags)
         errs_obj = unumpy.std_devs(umags)
 
     else:
         try:
-            mags_obj = cali_mags['mag'][:,objID]
-            errs_obj = cali_mags['err'][:,objID]
-        except:
-            mags_obj = cali_mags['flux'][:,objID]
-            errs_obj = cali_mags['err'][:,objID]
+            mags_obj = cali_mags['mag'][:, obj_id]
+            errs_obj = cali_mags['err'][:, obj_id]
+        except KeyError:
+            mags_obj = cali_mags['flux'][:, obj_id]
+            errs_obj = cali_mags['err'][:, obj_id]
 
     #   Create mask for time series to remove images without entries
     mask = np.isin(
         mags_obj,
         [0.],
         invert=True
-        )
+    )
 
     #   Remove images without entries
     mags_obj = mags_obj[mask]
     errs_obj = errs_obj[mask]
 
     # Make time series and use reshape to get a justified array
     ts = TimeSeries(
-            time=obs_time,
-            data={
-                filt: mags_obj.reshape(mags_obj.size,) * u.mag,
-                filt+'_err': errs_obj.reshape(errs_obj.size,) * u.mag,
-                }
-            )
+        time=obs_time,
+        data={
+            filt: mags_obj.reshape(mags_obj.size, ) * u.mag,
+            filt + '_err': errs_obj.reshape(errs_obj.size, ) * u.mag,
+        }
+    )
     return ts
 
 
 def lin_func(x, a, b):
-    '''
+    """
         Linear function
-    '''
-    return a + b*x
+    """
+    return a + b * x
 
 
 def fit_curve(fit_func, x, y, x0, sigma):
-    '''
+    """
         Fit curve with supplied fit function
 
         Parameters
         ----------
         fit_func        : `function`
             Function used in the fitting process
 
@@ -829,44 +813,44 @@
             Error parameter I
 
         b               : `float`
             Parameter II
 
         b_err           : `float`
             Error parameter II
-    '''
+    """
 
     #   Fit curve
     if np.any(sigma == 0.):
         para, coma = optimization.curve_fit(fit_func, x, y, x0)
     else:
         para, coma = optimization.curve_fit(fit_func, x, y, x0, sigma)
     a = para[0]
     b = para[1]
-    a_err = coma[0,0]
-    b_err = coma[1,1]
+    a_err = coma[0, 0]
+    b_err = coma[1, 1]
 
     return a, a_err, b, b_err
 
 
-def fit_data_oneD(x, y, order):
-    '''
+def fit_data_one_d(x, y, order):
+    """
         Fit polynomial to the provided data.
 
         Parameters
         ----------
         x               : `nump.ndarray` or `unmapy.uarray`
             X data values
 
         y               : `nump.ndarray` or `unmapy.uarray`
             Y data values
 
         order           : `integer`
             Order of the polynomial to be fitted to the data
-    '''
+    """
     #   Check array type
     unc = checks.check_unumpy_array(x)
 
     #   Set model
     model = models.Polynomial1D(degree=order)
 
     #   Set fitter
@@ -877,43 +861,43 @@
         if np.all(unumpy.nominal_values(x) == 0.):
             fit_poly = None
         else:
             fit_poly = fitter_poly(
                 model,
                 unumpy.nominal_values(x),
                 unumpy.nominal_values(y),
-                )
+            )
     else:
         if np.all(x == 0.):
             fit_poly = None
         else:
             fit_poly = fitter_poly(
                 model,
                 x,
                 y,
-                )
+            )
 
     return fit_poly
 
 
 def prepare_arrays(img_container, nfilter, count):
-    '''
+    """
         Prepare arrays for magnitude calibration
 
         Parameters
         ----------
         img_container   : `image.container`
             Container object with image ensemble objects for each filter
 
         nfilter         : `integer`
             Number of filter
 
         count           : `integer`
             Number of stars
-    '''
+    """
     #   Get image ensembles
     img_ensembles = img_container.ensembles
 
     #   Get maximum number of images
     nimgs = []
     for ensemble in img_ensembles.values():
         nimgs.append(len(ensemble.image_list))
@@ -923,68 +907,68 @@
 
     #   Get required array type
     unc = getattr(img_container, 'unc', True)
 
     #   Define magnitude arrays
     if unc:
         cali = unumpy.uarray(
-            np.zeros((nfilter,nimg_max,count)),
-            np.zeros((nfilter,nimg_max,count))
-            )
+            np.zeros((nfilter, nimg_max, count)),
+            np.zeros((nfilter, nimg_max, count))
+        )
     else:
         #   Define arrays
         cali = np.zeros(nfilter, dtype=[('mag', 'f8', (nimg_max, count)),
                                         ('std', 'f8', (nimg_max, count)),
                                         ('err', 'f8', (nimg_max, count)),
-                                    ]
-            )
+                                        ]
+                        )
 
     img_container.cali = cali
     img_container.noT = np.copy(cali)
 
     #   Define flux arrays
     if unc:
         img_container.flux = np.copy(cali)
     else:
         img_container.flux = np.zeros(
             nfilter,
             dtype=[('flux', 'f8', (nimg_max, count)),
                    ('err', 'f8', (nimg_max, count)),
-                  ]
-            )
+                   ]
+        )
 
 
 def cal_mag(*args, **kwargs):
-    '''
+    """
         Wrapper function: distinguish between astropy table
                           and pandas data frame
-    '''
+    """
     if base_aux.np_vs_df(args[0]):
         return mag_df(*args, **kwargs)
     else:
         return mag_arr(*args, **kwargs)
 
 
-#@timeis
+# @timeis
 def mag_arr(flux_arr):
-    '''
+    """
         Calculate magnitudes from flux
 
         Parameters
         ----------
         flux_arr        : `numpy.ndarray`
             Numpy structured array containing flux values and corresponding
             uncertainties
 
         Returns
         -------
         mags            : `numpy.ndarray`
             Numpy structured array containing magnitudes and corresponding
             errors
-    '''
+    """
     #   Get dimensions
     shape = flux_arr['flux_fit'].shape
     if len(shape) == 1:
         nobj = shape[0]
 
         #   Prepare array for the magnitudes and uncertainty
         mags = np.zeros(nobj, dtype=[('mag', 'f8'), ('err', 'f8')])
@@ -992,99 +976,98 @@
     elif len(shape) == 2:
         nimg = shape[0]
         nobj = shape[1]
 
         #   Prepare array for the magnitudes and uncertainty
         mags = np.zeros(
             nimg,
-            dtype=[('mag', 'f8', (nobj)), ('err', 'f8', (nobj))],
-            )
+            dtype=[('mag', 'f8', nobj), ('err', 'f8', nobj)],
+        )
 
     else:
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nDimension of the flux array > 2. This "
             f"is not supported. -> Exit {style.bcolors.ENDC}"
-            )
+        )
 
     ###
     #   Calculate magnitudes
     #
     #   Extract flux
-    flux        = flux_arr['flux_fit']
+    flux = flux_arr['flux_fit']
     #   Calculate magnitudes
     mags['mag'] = -2.5 * np.log10(flux)
 
-
     ###
     #   Calculate magnitudes and error
     #
     #   Error propagation also used by DAOPHOT -> see 'compute_phot_error'
     mags['err'] = 1.0857 * flux_arr['flux_unc'] / flux_arr['flux_fit']
 
     return mags
 
 
 def mag_u_arr(flux):
-    '''
+    """
         Calculate magnitudes from flux
 
         Parameters
         ----------
         flux            : `unumpy.ndarray`
             Numpy structured array containing flux values and corresponding
             uncertainties
 
         Returns
         -------
         mags            : `unumpy.ndarray`
             Numpy structured array containing magnitudes and corresponding
             errors
-    '''
+    """
     #   Get dimensions
     shape = flux.shape
     dim = len(shape)
     if 0 == dim or dim > 2:
         raise ValueError(
             f"{style.bcolors.FAIL} \nDimension of the flux array > 2. This "
             f"is not supported. -> Exit {style.bcolors.ENDC}"
-            )
+        )
 
     #   Calculate magnitudes
     mags = -2.5 * unumpy.log10(flux)
 
     return mags
 
 
-#@timeis
+# @timeis
 def mag_df(flux_df, flux_id='flux_fit', unc_id='flux_unc'):
-    '''
+    """
         Calculate magnitudes from flux
 
         Parameters
         ----------
         flux_df         : `pandas.DataFrame`
             Flux values and corresponding uncertainties
 
         flux_id         : `string`, optional
             Name for the flux column
             Default is ``flux_fit``.
 
-        flux_unc        : `string`, optional
+        unc_id          : `string`, optional
             Name for the flux uncertainty column
             Default is ``flux_unc``.
 
         Returns
         -------
         flux_df         : `pandas.DataFrame`
             Magnitudes and orresponding uncertainties
-    '''
+    """
     #   Extract flux and flux uncertainty
-    flux          = flux_df[flux_id]
-    flux_err      = flux_df[unc_id]
-    flux_err      = np.absolute(flux_err)
+    flux = flux_df[flux_id]
+    flux_err = flux_df[unc_id]
+    flux_err = np.absolute(flux_err)
 
     #   Calculate magnitudes
     df_temp = -2.5 * np.log10(flux)
 
     #   Check if we are dealing with a Series or DataFrame
     if isinstance(df_temp, pd.Series):
         df_temp.name = 'mag'
@@ -1095,69 +1078,68 @@
         df_columns = df_temp.columns
         index = pd.MultiIndex.from_product([['mag'], df_columns])
         df_temp.columns = index
     else:
         raise Exception(
             f"{style.bcolors.FAIL} \nInput object is neither a Pandas Series "
             f"nor Dataframe -> EXIT {style.bcolors.ENDC}"
-            )
+        )
 
     #   Add magnitudes to input data frame
     flux_df = pd.concat([flux_df, df_temp], axis=1)
 
-    #   Prepare array with difference between flux and flux error
-    #   Sanitize -> ensure that the difference is > 0
-    pre_arr = np.where(
-        flux_err < flux,
-        flux - flux_err,
-        1E-20
-        )
+    # #   Prepare array with difference between flux and flux error
+    # #   Sanitize -> ensure that the difference is > 0
+    # pre_arr = np.where(
+    #     flux_err < flux,
+    #     flux - flux_err,
+    #     1E-20
+    # )
 
     #   Calculate Errors
     mag_err = 1.0857 * flux_err / flux
 
     #   Branch according to Series or DataFrame
-    if isinstance(mag_err_m, pd.DataFrame):
+    if isinstance(mag_err, pd.DataFrame):
         #   New index
         index = pd.MultiIndex.from_product([['err'], df_columns])
 
         #   Convert numpy array to data frame
-        err_df  = pd.DataFrame(
+        err_df = pd.DataFrame(
             mag_err,
             index=flux_df.index,
             columns=index,
-            )
+        )
     else:
         #   Convert numpy array to data frame
-        err_df  = pd.DataFrame({'err':mag_err}, index=flux_df.index)
-
+        err_df = pd.DataFrame({'err': mag_err}, index=flux_df.index)
 
     #   Attach errors to data frame
     flux_df = pd.concat([flux_df, err_df], axis=1)
 
     return flux_df
 
 
 def mk_posi_tbl(img_container, ensemble_IDs):
-    '''
+    """
         Make position tables
 
         Parameters
         ----------
         img_container           : `image.container`
             Container object with image ensemble objects for each filter
 
         ensemble_IDs            : `list`
             List with image IDs
 
         Returns
         -------
         tbl_xy          : `dictionary` of `astropy.table.Table` objects
             X and Y position in pixel among other data
-    '''
+    """
     #   Get image ensembles
     ensembles = img_container.ensembles
 
     tbl_xy = {}
     for ID in ensemble_IDs:
         #   Ensure ID is `string`
         ID = str(ID)
@@ -1170,71 +1152,71 @@
 
         #   Get magnitudes and positions
         try:
             mags = cal_mag(img.flux_es)['mag']
             ids = ensem.id_es
             xs = ensem.x_es
             ys = ensem.y_es
-        except:
+        except AttributeError:
             mags = cal_mag(img.flux)['mag']
             ids = ensem.id_s
             xs = ensem.x_s
             ys = ensem.y_s
 
         #   Fill astropy table
         tbl_xy[ID] = Table(
-            names=['id','xcentroid', 'ycentroid', 'mag'],
+            names=['id', 'xcentroid', 'ycentroid', 'mag'],
             data=[np.intc(ids), xs, ys, mags]
-            )
+        )
 
     return tbl_xy
 
 
 def mk_posi_tbl_ensem(ensemble):
-    '''
+    """
         Make position tables
 
         Parameters
         ----------
         ensemble                : `image ensemble`
             Image image ensemble class object
 
         Returns
         -------
         tbl_xy          : `dictionary` of `astropy.table.Table` objects
             X and Y position in pixel among other data
-    '''
+    """
     #   Define astropy table
     tbl_xy = {}
 
     #   Get image
     for img in ensemble.image_list:
         #   Get magnitudes and positions
         try:
             mags = cal_mag(img.flux_es)['mag']
             ids = ensemble.id_es
             xs = ensemble.x_es
             ys = ensemble.y_es
-        except:
+        except AttributeError:
             mags = cal_mag(img.flux)['mag']
             ids = ensemble.id_s
             xs = ensemble.x_s
             ys = ensemble.y_s
 
         #   Fill astropy table
         tbl_xy[img.pd] = Table(
-            names=['id','xcentroid', 'ycentroid', 'mag'],
+            names=['id', 'xcentroid', 'ycentroid', 'mag'],
             data=[np.intc(ids), xs, ys, mags]
-            )
+        )
 
     return tbl_xy
 
 
 def mk_posi_tbl_pd(ind_sort, img_IDs, x, y, mags):
-    '''
+    """
         Make position tables
 
         Parameters
         ----------
         ind_sort        : `numpy.ndarray`
             IDs of the stars
 
@@ -1250,15 +1232,15 @@
         mags            : `pandas.DataFrame`
             Magnitude array of the stars
 
         Returns
         -------
         tbl_xy          : `astropy.table.Table`
             X and Y position in pixel among other data
-    '''
+    """
     #   Drop level > 0, if column levels > 1
     if mags.columns.nlevels > 1:
         cols = mags.columns.droplevel(1)
     else:
         cols = mags.columns
     #   Check whether median values of the magnitudes are available
     #   in 'mags'
@@ -1266,32 +1248,32 @@
         col_name = 'mag'
     elif 'median' in cols.values:
         col_name = 'median'
     else:
         raise Exception(
             f"{style.bcolors.FAIL} \nMagnitude column not recognize in 'mags' "
             f"DataFrame -> EXIT {style.bcolors.ENDC}"
-            )
+        )
 
     tbl_xy = {}
     for j, img_ID in enumerate(img_IDs):
         #   Restrict input data frame to current image
         mask = mags['type'] == img_ID
 
         img_ID = str(img_ID)
         tbl_xy[img_ID] = Table(
-            names=['id','xcentroid', 'ycentroid', 'mag'],
+            names=['id', 'xcentroid', 'ycentroid', 'mag'],
             data=[np.intc(ind_sort), x, y, mags[mask][col_name]]
-            )
+        )
 
     return tbl_xy
 
 
 def find_filt(filt_list, in_dict, filt, camera, verbose=False, indent=2):
-    '''
+    """
         Find the position of the filter from the dictionary 'filt'
         in the dictionary 'in_dict' with reference to 'filt_list'
 
         Parameters
         ----------
         filt_list       : `list` - `string`
             List of available filter, e.g., ['U', 'B', 'V', ...]
@@ -1322,15 +1304,15 @@
             Entry from dictionary 'in_dict' corresponding to filter 'filt'
 
                         : `integer`
             ID of filter 1
 
                         : `integer`
             ID of filter 2
-    '''
+    """
     #   Initialize list of bools
     cam_bools = []
 
     #   Loop over outer dictionary: 'in_dict'
     for key_outer, value_outer in in_dict.items():
         #   Check if calibration data fits to the camera
         if camera == key_outer:
@@ -1352,40 +1334,40 @@
                     else:
                         if verbose:
                             terminal_output.print_terminal(
                                 f1,
                                 f2,
                                 filt_list,
                                 indent=indent,
-                                string='Magnitude transformation coefficients'\
-                                    ' do not apply. Wrong filter combination:'\
-                                    ' {} & {} vs. {}',
+                                string='Magnitude transformation coefficients'
+                                       ' do not apply. Wrong filter combination:'
+                                       ' {} & {} vs. {}',
                                 style_name='WARNING',
-                                )
+                            )
 
             cam_bools.append(True)
         else:
             cam_bools.append(False)
 
     if not any(cam_bools):
         terminal_output.print_terminal(
             camera,
             indent=indent,
-            string='Determined camera {} not consistent with the' \
-            +' one given in the dictionary with the transformation' \
-            +' coefficients.',
+            string='Determined camera {} not consistent with the'
+                   ' one given in the dictionary with the transformation'
+                   ' coefficients.',
             style_name='WARNING',
-            )
+        )
 
     return None, None, None
 
 
 def check_variable(filename, filetype, filt_1, filt_2, cali,
                    ISOcolumntype, ISOcolumn):
-    '''
+    """
         Check variables and set defaults for CMDs and isochrone plots
 
         This function exists for backwards compatibility.
 
         Parameters
         ----------
         filename            : `string`
@@ -1405,31 +1387,31 @@
             Keys = filter - Values = zero points
 
         ISOcolumntype       : `dictionary`
             Keys = filter - Values = type
 
         ISOcolumn           : `dictionary`
             Keys = filter - Values = column
-    '''
+    """
 
     filename, filetype = check_variable_apparent_cmd(
         filename,
         filetype,
         filt_1,
         filt_2,
         cali,
-        )
+    )
 
     check_variable_absolute_cmd(filt_1, filt_2, ISOcolumntype, ISOcolumn)
 
     return filename, filetype
 
 
 def check_variable_apparent_cmd(filename, filetype, filt_1, filt_2, cali):
-    '''
+    """
         Check variables and set defaults for CMDs and isochrone plots
 
         Parameters
         ----------
         filename            : `string`
             Specified file name - can also be empty -> set default
 
@@ -1441,68 +1423,68 @@
             First filter
 
         filt_2              : `string`
             Second filter
 
         cali                : `dictionary`
             Keys = filter - Values = zero points
-    '''
+    """
     #   Set figure type
-    if filename == "?" or filename =="":
+    if filename == "?" or filename == "":
         terminal_output.print_terminal(
             indent=1,
             string='[Warning] No filename given, us default (cmd)',
             style_name='WARNING',
-            )
+        )
         filename = 'cmd'
 
     if filetype == '?' or filetype == '':
         terminal_output.print_terminal(
             indent=1,
             string='[Warning] No filetype given, use default (pdf)',
             style_name='WARNING',
-            )
-        filetype ='pdf'
+        )
+        filetype = 'pdf'
 
     #   Check if file type is valid and set default
     filetype_list = ['pdf', 'png', 'eps', 'ps', 'svg']
     if filetype not in filetype_list:
         terminal_output.print_terminal(
             indent=1,
-            string='[Warning] Unknown filetype given, use default instead '\
-                  +'(pdf)',
+            string='[Warning] Unknown filetype given, use default instead '
+                   '(pdf)',
             style_name='WARNING',
-            )
+        )
         filetype = 'pdf'
 
     #   Check if calibration parameter is consistent with the number of
     #   filter
     if len(filt_2) + len(filt_1) != len(cali):
         if len(filt_2) + len(filt_1) > len(cali):
             terminal_output.print_terminal(
                 indent=1,
-                string="[Error] More filter ('filt_2') specified than zero"\
-                +" points ('cali')",
+                string="[Error] More filter ('filt_2') specified than zero"
+                       " points ('cali')",
                 style_name='WARNING',
             )
             sys.exit()
         else:
             terminal_output.print_terminal(
                 indent=1,
-                string="[Error] More zero points ('cali') specified than "\
-                +"filter ('filt_2')",
+                string="[Error] More zero points ('cali') specified than "
+                       "filter ('filt_2')",
                 style_name='WARNING',
             )
             sys.exit()
 
     return filename, filetype
 
 
 def check_variable_absolute_cmd(filt_1, filt_2, ISOcolumntype, ISOcolumn):
-    '''
+    """
         Check variables and set defaults for CMDs and isochrone plots
 
         Parameters
         ----------
         filt_1              : `string`
             First filter
 
@@ -1510,95 +1492,96 @@
             Second filter
 
         ISOcolumntype       : `dictionary`
             Keys = filter - Values = type
 
         ISOcolumn           : `dictionary`
             Keys = filter - Values = column
-    '''
+    """
     #   Check if the column declaration for the isochrones fits to the
     #   specified filter
     for fil in filt_2:
         if fil not in ISOcolumntype.keys():
             terminal_output.print_terminal(
                 fil,
                 indent=1,
-                string="[Error] No entry for filter {:d} specified in"\
-                +" 'ISOcolumntype'",
+                string="[Error] No entry for filter {:d} specified in"
+                       " 'ISOcolumntype'",
                 style_name='WARNING',
             )
             sys.exit()
         if fil not in ISOcolumn.keys():
             terminal_output.print_terminal(
                 fil,
                 indent=1,
-                string="[Error] No entry for filter {:d} specified in"\
-                +" 'ISOcolumn'",
+                string="[Error] No entry for filter {:d} specified in"
+                       " 'ISOcolumn'",
                 style_name='WARNING',
             )
             sys.exit()
     if filt_1 not in ISOcolumn.keys():
         terminal_output.print_terminal(
             filt_1,
             indent=1,
-            string="[Error] No entry for filter {:d} specified in"\
-                    +" 'ISOcolumn'",
+            string="[Error] No entry for filter {:d} specified in"
+                   " 'ISOcolumn'",
             style_name='WARNING',
         )
         sys.exit()
 
 
 class Executor:
-    '''
+    """
         Class that handels the multiprocessing, using apply_async.
         -> allows for easy catch of exceptions
-    '''
+    """
+
     def __init__(self, process_num):
         #   Init multiprocessing pool
         self.pool = mp.Pool(process_num)
         #   Init variables
         self.res = []
         self.err = None
 
     def collect_results(self, result):
-        '''
+        """
             Uses apply_async's callback to setup up a separate Queue
             for each process
-        '''
+        """
         #   Catch all results
         self.res.append(result)
 
     def callback_error(self, e):
-        '''
+        """
             Handles axceptions by apply_async's error callback
-        '''
+        """
         #   Termninate pool
         self.pool.terminate()
         #   Raise exceptions
         self.err = e
         raise e
 
     def schedule(self, function, args, kwargs):
-        '''
+        """
             Call to apply_async
-        '''
+        """
         self.pool.apply_async(function, args, kwargs,
                               callback=self.collect_results,
                               error_callback=self.callback_error)
 
     def wait(self):
-        '''
+        """
             Close pool and wait for completion
-        '''
+        """
         self.pool.close()
         self.pool.join()
 
 
-def mk_ds9_region(x, y, r, filename, wcs):
-    '''
+def mk_ds9_region(x, y, r, filename, wcs_object):
+    """
         Make and write a ds9 region file
 
         Parameters
         ----------
         x               : `numpy.ndarray`
             X coordinates in pixel
 
@@ -1607,42 +1590,42 @@
 
         r               : `float`
             Radius in pixel
 
         filename        : `string`
             File name
 
-        wcs             : `astropy.wcs.WCS`
+        wcs_object      : `astropy.wcs.WCS`
             WCS infos
-    '''
+    """
     #   Create the region
     c_regs = []
 
     for x_i, y_i in zip(x, y):
         #   Make a pixel coordinates object
         center = PixCoord(x=x_i, y=y_i)
 
         #   Create the region
         c = CirclePixelRegion(center, radius=r)
 
         #   Append region and convert to sky coordinates
-        c_regs.append(c.to_sky(wcs))
+        c_regs.append(c.to_sky(wcs_object))
 
     #   Convert to Regions that contain all individual regions
     reg = Regions(c_regs)
 
     #   Write the region file
     reg.write(filename, format='ds9', overwrite=True)
 
 
 def prepare_and_plot_starmap(image, condense=False, tbl=None,
                              x_name='x_fit', y_name='y_fit', rts_pre='img',
                              label='Stars with photometric extractions',
                              add_image_id=True):
-    '''
+    """
         Prepare table for star map and plot star map
 
         Parameters
         ----------
         image           : `image.class`
             Image class with all image specific properties
 
@@ -1669,103 +1652,103 @@
         label           : `string`, optional
             Label that characterizes the star map.
             Default is ``Stars with photometric extractions``.
 
         add_image_id    : `boolean`, optional
             If ``True`` the image ID will be added to the file name.
             Default is ``True``.
-    '''
+    """
     #   Get table, data, filter, & object name
     if tbl is None:
-        tbl  = image.photometry
+        tbl = image.photometry
     data = image.get_data()
     filt = image.filt
     name = image.objname
 
     #   Prepare table
     nstars = len(tbl)
     tbl_xy = Table(
         names=['id', 'xcentroid', 'ycentroid'],
-        data=[np.arange(0,nstars), tbl[x_name], tbl[y_name]],
-        )
+        data=[np.arange(0, nstars), tbl[x_name], tbl[y_name]],
+    )
 
     #   Prepare string for file name
     if add_image_id:
-        rts_pre += '-'+str(image.pd)
+        rts_pre += '-' + str(image.pd)
 
     #   Plot star map
     out_str = plot.starmap(
         image.outpath.name,
         data,
         filt,
         tbl_xy,
         label=label,
         rts=rts_pre,
         nameobj=name,
         condense=condense,
-        )
+    )
     if condense:
         return out_str
 
 
 def prepare_and_plot_starmap_final(img_container, filt_list):
-    '''
+    """
         Prepare table for star map and plot star map
 
         Parameters
         ----------
         img_container           : `image.container`
             Container object with image ensemble objects for each filter
 
         filt_list       : `list` of `strings`
             List with filter names
-    '''
+    """
     terminal_output.print_terminal(
-            indent=1,
-            string="Plot star maps with positions from the final "\
-                  +"correlation",
-            )
+        indent=1,
+        string="Plot star maps with positions from the final "
+               "correlation",
+    )
     #   Make position table
     tbl_xy_final = mk_posi_tbl(
         img_container,
         filt_list,
-        )
+    )
 
     for filt in filt_list:
         if filt == filt_list[0]:
-            rts = str(filt_list[1])+'_final'
+            rts = str(filt_list[1]) + '_final'
         else:
-            rts = str(filt_list[0])+'_final'
+            rts = str(filt_list[0]) + '_final'
 
         #   Get reference image
         image = img_container.ensembles[filt].ref_img
 
         #   Using multiprocessing to create the plot
         p = mp.Process(
             target=plot.starmap,
             args=(
                 str(image.outpath / 'final'),
                 image.get_data(),
                 filt,
                 tbl_xy_final[filt],
-                ),
+            ),
             kwargs={
-                'rts':rts,
-                'label':'Stars identified in '+str(filt_list[0])
-                +' and '+str(filt_list[1])+' filter',
-                'nameobj':image.objname,
-                }
-            )
+                'rts': rts,
+                'label': 'Stars identified in ' + str(filt_list[0])
+                         + ' and ' + str(filt_list[1]) + ' filter',
+                'nameobj': image.objname,
+            }
+        )
         p.start()
     terminal_output.print_terminal()
 
 
 def prepare_and_plot_starmap_final_3(img_ensemble, calib_xs, calib_ys,
                                      plot_test=True):
-    '''
+    """
         Prepare table for star map and plot star map
 
         Parameters
         ----------
         img_ensemble    : `image ensemble`
             Image img_ensemble class object
 
@@ -1777,237 +1760,265 @@
             Position of the claibration objects on the image in pixel
             in Y direction
 
         plot_test       : `boolean`, optional
             If True only the masterplot for the reference image will
             be created.
             Default is ``True``.
-    '''
+    """
     terminal_output.print_terminal(
         indent=1,
         string="Plot star map with the objects identified on all images",
-        )
+    )
 
     #   Get image IDs, IDs of the objects, and pixel coordinates
     img_ids = img_ensemble.get_image_ids()
 
     #   Make position table
     tbl_xy_final = mk_posi_tbl_ensem(img_ensemble)
 
     #   Make new table with the position of the calibration stars
     tbl_xy_calib = Table(
         names=['xcentroid', 'ycentroid'],
         data=[[calib_xs], [calib_ys]]
-        )
+    )
 
     #   Make the plot using multiprocessing
     for j, ID in enumerate(img_ids):
         key = str(ID)
-        if plot_test and j != img_ensemble.ref_id: continue
+        if plot_test and j != img_ensemble.ref_id:
+            continue
         p = mp.Process(
             target=plot.starmap,
             args=(
                 img_ensemble.outpath.name,
                 img_ensemble.image_list[j].get_data(),
                 img_ensemble.filt,
                 tbl_xy_final[ID],
-                ),
+            ),
             kwargs={
-                'tbl_2':tbl_xy_calib,
-                'rts':key+'_final',
-                'label':'Stars identified in all images',
-                'label_2':'Calibration stars',
-                'nameobj':img_ensemble.objname,
-                }
-            )
+                'tbl_2': tbl_xy_calib,
+                'rts': key + '_final',
+                'label': 'Stars identified in all images',
+                'label_2': 'Calibration stars',
+                'nameobj': img_ensemble.objname,
+            }
+        )
         p.start()
         terminal_output.print_terminal()
 
 
 def add_median_table(img_ensemble, meanb=False):
-    '''
+    """
         Calculate flux median or flux mean and add it to a new table
 
         Parameters
         ----------
         img_ensemble        : `image.ensemble` object
             Ensemble class object with all image data taken in a specific
             filter
 
         meanb               : `boolean`
             If True the mean instead of the median flux will be added to the
             table.
-    '''
+    """
     #   Get flux:
     try:
         flux = img_ensemble.flux_es['flux_fit']
         xs = img_ensemble.x_es
         ys = img_ensemble.y_es
-    except:
+    except AttributeError:
         flux = img_ensemble.flux['flux_fit']
         xs = img_ensemble.x_s
         ys = img_ensemble.y_s
 
     ###
     #   Calculate mean, median, and standard deviation of the
     #   object fluxes, using sigma clipping
     #
     mean, median, std = sigma_clipped_stats(
         flux,
         sigma=1.5,
         axis=0,
-        )
-
+    )
 
     ###
     #   Make new table to add the median of the flux
     #
     #   New table
     if meanb:
         _tbl = Table(
-            names=['x_fit', 'y_fit', 'flux_fit', 'flux_unc',],
-            data=[xs, ys, mean, std,]
-            )
+            names=['x_fit', 'y_fit', 'flux_fit', 'flux_unc', ],
+            data=[xs, ys, mean, std, ]
+        )
     else:
         _tbl = Table(
-            names=['x_fit', 'y_fit', 'flux_fit', 'flux_unc',],
-            data=[xs, ys, median, std,]
-            )
+            names=['x_fit', 'y_fit', 'flux_fit', 'flux_unc', ],
+            data=[xs, ys, median, std, ]
+        )
 
     #   Add to the overall dictionary
     img_ensemble.results = _tbl.group_by('x_fit')
 
 
-def derive_limiting_mag(img_container, filt_list, ref_img, indent=1):
-    '''
+def derive_limiting_mag(img_container, filt_list, ref_img, r_limit=4.,
+                        r_unit='arcsec', indent=1):
+    """
         Determine limiting magnitude
 
         Parameters
         img_container       : `image.container`
             Container object with image ensemble objects for each filter
 
         filt_list           : `list` of `strings`
             List with filter names
 
         ref_img             : `integer`, optional
             ID of the reference image
             Default is ``0``.
 
+        r_limit                 : `float`, optional
+            Radius of the aperture used to derive the limiting magnitude
+            Default is ``4``.
+
+        r_unit                  : `string`, optional
+            Unit of the radii above. Allowed are ``pixel`` and ``arcsec``.
+            Default is ``arcsec``.
+
         indent          : `integer`, optional
             Indentation for the console output lines
             Default is ``1``.
-    '''
+    """
     #   Get image ensembles
     img_ensembles = img_container.ensembles
 
-    #   Get type of the magnitude arrays
-    #   Possibilities: unumpy.uarray & numpy structured ndarray
-    unc = getattr(img_container, 'unc', True)
-
     #   Get calibrated magnitudes
-    cali_mags = getattr(img_container, 'cali', None)
-    if unc:
-        if (cali_mags is None or
-            np.all(unumpy.nominal_values(cali_mags) == 0.)):
-                #   If array with magnitude transformation is not available
-                #   or if it is empty get the array without magnitude
-                #   transformation
-                cali_mags = getattr(img_container, 'noT', None)
-                if cali_mags is not None:
-                    #   Get only the magnitude values
-                    cali_mags = unumpy.nominal_values(cali_mags)
-        else:
-            #   Get only the magnitude values
-            cali_mags = unumpy.nominal_values(cali_mags)
-
-    #   numpy structured ndarray type:
-    else:
-        if (cali_mags is None or np.all(cali_mags['mag'] == 0.)):
-            #   If array with magnitude transformation is not available
-            #   or if it is empty get the array without magnitude
-            #   transformation
-            cali_mags = getattr(img_container, 'noT', None)
-            if cali_mags is not None:
-                cali_mags = cali_mags['mag']
-        else:
-            cali_mags = cali_mags['mag']
+    cali_mags = img_container.get_calibrated_magnitudes()
 
     #   Get magnitudes of reference image
     for i, filt in enumerate(filt_list):
         #   Get image ensemble
         ensemble = img_ensembles[filt]
 
         #   Get object indices and X & Y pixel positions
         try:
-            ind = ensemble.id_es
-            x   = ensemble.x_es
-            y   = ensemble.y_es
-        except:
-            ind = ensemble.id_s
-            x   = ensemble.x_s
-            y   = ensemble.y_s
+            x = ensemble.x_es
+            y = ensemble.y_es
+        except AttributeError:
+            x = ensemble.x_s
+            y = ensemble.y_s
 
         #   Get reference image
         image = ensemble.image_list[ref_img]
 
-        mag_arr = cali_mags[i][ref_img]
+        mag_data = cali_mags[i][ref_img]
 
         #   Make astropy table
         tbl_mag = Table(
-            names=['xcentroid', 'ycentroid','mags'],
-            data=[x, y, mag_arr]
-            )
+            names=['xcentroid', 'ycentroid', 'mags'],
+            data=[x, y, mag_data]
+        )
         tbl_mag = tbl_mag.group_by('mags')
 
         #   Remove implausible dark results
         mask = tbl_mag['mags'] < 30
         tbl_mag = tbl_mag[mask]
 
         #   Plot star map
         if ref_img != '':
-            rts = 'mags_'+str(ref_img)
+            rts = 'mags_' + str(ref_img)
         else:
             rts = 'mags'
         p = mp.Process(
             target=plot.starmap,
             args=(
                 image.outpath.name,
                 image.get_data(),
                 filt,
                 tbl_mag[:][-10:],
-                ),
+            ),
             kwargs={
-                'label':'10 faintest stars',
-                'rts':rts,
-                'mode':'mags',
-                'nameobj':image.objname,
-                }
-            )
+                'label': '10 faintest stars',
+                'rts': rts,
+                'mode': 'mags',
+                'nameobj': image.objname,
+            }
+        )
         p.start()
 
         #   Print result
         terminal_output.print_terminal(
             filt,
             indent=indent,
             string="Determine limiting magnitude for filter: {}",
-            )
+        )
+        terminal_output.print_terminal(
+            indent=indent * 2,
+            string="Based on detected objects:",
+        )
         terminal_output.print_terminal(
             np.median(tbl_mag['mags'][-10:]),
-            indent=indent*2,
-            string="Median of the 10 faintest objects: {}",
-            )
+            indent=indent * 3,
+            string="Median of the 10 faintest objects: {} mag",
+        )
         terminal_output.print_terminal(
             np.mean(tbl_mag['mags'][-10:]),
-            indent=indent*2,
-            string="Mean of the 10 faintest objects: {}",
-            )
+            indent=indent * 3,
+            string="Mean of the 10 faintest objects: {} mag",
+        )
+
+        #   Convert object positions to pixel index values
+        index_x = np.rint(x).astype(int)
+        index_y = np.rint(y).astype(int)
+
+        #   Convert object positions to mask
+        mask = np.zeros(image.get_shape(), dtype=bool)
+        mask[index_y, index_x] = True
+
+        #   Set radius for the apertures
+        radius = r_limit
+        if r_unit == 'arcsec':
+            radius = radius / image.pixscale
+
+        #   Setup ImageDepth object from the photutils package
+        depth = ImageDepth(
+            radius,
+            nsigma=5.0,
+            napers=500,
+            niters=2,
+            overlap=False,
+            # seed=123,
+            zeropoint=np.median(image.ZP_clip),
+            progress_bar=False,
+        )
+
+        #   Derive limits
+        limits = depth(image.get_data(), mask)
+
+        #   Plot sky apertures
+        p = mp.Process(
+            target=plot.plot_limiting_mag_sky_apertures,
+            args=(image.outpath.name, image.get_data(), mask, depth),
+        )
+        p.start()
+
+        #   Print results
+        terminal_output.print_terminal(
+            indent=indent * 2,
+            string="Based on the ImageDepth (photutils) routine:",
+        )
+        terminal_output.print_terminal(
+            limits[1],
+            indent=indent * 3,
+            string="500 apertures, 5 sigma, 2 iterations: {} mag",
+        )
 
 
 def rm_edge_objects(table, data, border=10, condense=False, indent=3):
-    '''
+    """
         Remove detected objects that are too close to the image edges
 
         Parameters
         ----------
         table               : `astropy.table.Table` object
             Table with the object data
 
@@ -2023,43 +2034,43 @@
             If True the terminal output will be returned to the calling
             function.
             Default is ``False``.
 
         indent              : `integer`, optional
             Indentation for the console output lines
             Default is ``3``.
-    '''
+    """
     #   Border range
     hsize = border + 1
 
     #   Get position data
     x = table['x_fit'].value
     y = table['y_fit'].value
 
     #   Calculate mask of objects to be removed
-    mask = ((x > hsize) & (x < (data.shape[1] -1 - hsize)) &
-            (y > hsize) & (y < (data.shape[0] -1 - hsize)))
+    mask = ((x > hsize) & (x < (data.shape[1] - 1 - hsize)) &
+            (y > hsize) & (y < (data.shape[0] - 1 - hsize)))
 
     outstr = terminal_output.print_terminal(
         np.count_nonzero(np.invert(mask)),
         indent=indent,
-        string='{} objects removed because they are too close to the '\
-              +'image edges',
+        string='{} objects removed because they are too close to the '
+               'image edges',
         condense=condense,
-        )
+    )
     if condense:
         return table[mask], outstr
     else:
         return table[mask], ''
 
 
 def proper_motion_selection(ensemble, tbl, catalog="I/355/gaiadr3",
                             Gmag_limit=20, seplimit=1., sigma=3.,
                             maxiters_sigma=3):
-    '''
+    """
         Select a sub set of the objects that are close to the median
         proper motion
 
         Parameters
         ----------
         ensemble            : `image.ensemble` object
             Ensemble class object with all image data taken in a specific
@@ -2084,29 +2095,28 @@
             Sigma value used in the sigma clipping of the proper motion
             values.
             Default is ``3``.
 
         maxiters_sigma      : `integer`, optional
             Maximal number of iteration of the sigma clipping.
             Default is ``3``.
-    '''
+    """
     #   Get wcs
     w = ensemble.wcs
 
     #   Convert pixel coordinates to ra & dec
     coords = w.all_pix2world(tbl['x'], tbl['y'], 0)
 
     #   Create SkyCoord object with coordinates of all objects
     coords_img = SkyCoord(
         coords[0],
         coords[1],
         unit=(u.degree, u.degree),
         frame="icrs"
-        )
-
+    )
 
     ###
     #   Get Gaia data from Vizier
     #
     #   Columns to download
     columns = [
         'RA_ICRS',
@@ -2115,77 +2125,76 @@
         'Plx',
         'e_Plx',
         'pmRA',
         'e_pmRA',
         'pmDE',
         'e_pmDE',
         'RUWE',
-        ]
+    ]
 
     #   Define astroquery instance
     v = Vizier(
         columns=columns,
         row_limit=1e6,
         catalog=catalog,
-        column_filters={'Gmag':'<'+str(Gmag_limit)},
-        )
+        column_filters={'Gmag': '<' + str(Gmag_limit)},
+    )
 
     #   Get data from the corresponding catalog for the objects in the FOV
     result = v.query_region(
         ensemble.coord,
-        radius=ensemble.fov*u.arcmin,
-        )
+        radius=ensemble.fov * u.arcmin,
+    )
 
     #   Create SkyCoord object with coordinates of all Gaia objects
     coords_calib = SkyCoord(
-            result[0]['RA_ICRS'],
-            result[0]['DE_ICRS'],
-            unit=(u.degree, u.degree),
-            frame="icrs"
-            )
+        result[0]['RA_ICRS'],
+        result[0]['DE_ICRS'],
+        unit=(u.degree, u.degree),
+        frame="icrs"
+    )
 
     ###
     #   Correlate own objects with Gaia objects
     #
     #   Set maximal separation between objects
-    seplimit = seplimit*u.arcsec
+    seplimit = seplimit * u.arcsec
 
     #   Correlate data
     id_img, id_calib, d2ds, d3ds = matching.search_around_sky(
         coords_img,
         coords_calib,
         seplimit,
-        )
-
+    )
 
     ###
     #   Sigma clipping of the proper motion values
     #
 
     #   Proper motion of the common objects
     pmDE = result[0]['pmDE'][id_calib]
     pmRA = result[0]['pmRA'][id_calib]
 
     #   Parallax
-    parallax = result[0]['Plx'][id_calib].data/1000*u.arcsec
+    parallax = result[0]['Plx'][id_calib].data / 1000 * u.arcsec
 
     #   Distance
     distance = parallax.to_value(u.kpc, equivalencies=u.parallax())
 
     #   Sigma clipping
     sigma_clip_DE = sigma_clip(
         pmDE,
         sigma=sigma,
         maxiters=maxiters_sigma,
-        )
+    )
     sigma_clip_RA = sigma_clip(
         pmRA,
         sigma=sigma,
         maxiters=maxiters_sigma,
-        )
+    )
 
     #   Create mask from sigma clipping
     mask = sigma_clip_RA.mask | sigma_clip_DE.mask
 
     ###
     #   Make plots
     #
@@ -2193,53 +2202,53 @@
     result_cut = result[0][id_calib][mask]
 
     #   Convert ra & dec to pixel coordinates
     x_obj, y_obj = w.all_world2pix(
         result_cut['RA_ICRS'],
         result_cut['DE_ICRS'],
         0,
-        )
+    )
 
     #   Get image
     image = ensemble.ref_img
 
     #   Star map
     prepare_and_plot_starmap(
         image,
         tbl=Table(names=['x_fit', 'y_fit'], data=[x_obj, y_obj]),
         rts_pre='img-pmGaia-',
         label='Stars selected according to proper motion',
-        )
+    )
 
     #   2D and 3D plot of the proper motion and the distance
     plot.comp_scatter(
         pmRA,
         pmDE,
         'pm_RA * cos(DEC) (mas/yr)',
         'pm_DEC (mas/yr)',
         '_pm_',
         image.outpath.name,
         oneTOone=False,
-        )
+    )
     plot.D3_scatter(
         [pmRA],
         [pmDE],
         [distance],
         image.outpath.name,
         name_x='pm_RA * cos(DEC) (mas/yr)',
         name_y='pm_DEC (mas/yr)',
         name_z='d (kpc)',
-        )
+    )
 
     #   Apply mask
     return tbl[id_img][mask]
 
 
 def region_selection(ensemble, coord, tbl, radius=600.):
-    '''
+    """
         Select a sub set of the objects that are close to the median
         proper motion
 
         Parameters
         ----------
         ensemble            : `image.ensemble` object
             Ensemble class object with all image data taken in a specific
@@ -2258,28 +2267,28 @@
         Returns
         -------
         tbl                 : `astropy.table.Table`
             Table with object position information
 
         mask                : `boolean numpy.ndarray`
             Mask that needs to be applied to the table.
-    '''
+    """
     #   Get wcs
     w = ensemble.wcs
 
     #   Convert pixel coordinates to ra & dec
     coords = w.all_pix2world(tbl['x'], tbl['y'], 0)
 
     #   Create SkyCoord object with coordinates of all objects
     coords_img = SkyCoord(
         coords[0],
         coords[1],
         unit=(u.degree, u.degree),
         frame="icrs"
-        )
+    )
 
     #   Calculate separation between the coordinates defined in ``coord``
     #   the objects in ``tbl``
     sep = coords_img.separation(coord)
 
     #   Calculate mask of all object closer than ``radius``
     mask = sep.arcsec <= radius
@@ -2289,23 +2298,22 @@
 
     #   Plot starmap
     prepare_and_plot_starmap(
         ensemble.ref_img,
         tbl=Table(names=['x_fit', 'y_fit'], data=[tbl['x'], tbl['y']]),
         rts_pre='img-selection-',
         label='Stars selected within {}'.format(radius),
-        )
+    )
 
     return tbl, mask
 
 
 def find_cluster(ensemble, tbl, catalog="I/355/gaiadr3", Gmag_limit=20,
-                 seplimit=1., max_distance=6., n_clusters=10,
-                 random_state=2, n_neighbors=4, parameter_set=1):
-    '''
+                 seplimit=1., max_distance=6., parameter_set=1):
+    """
         Identify cluster in data
 
         Parameters
         ----------
         ensemble            : `image.ensemble` object
             Ensemble class object with all image data taken in a specific
             filter
@@ -2325,27 +2333,14 @@
             Maximal allowed separation between objects in arcsec.
             Default is ``1``.
 
         max_distance        : `float`, optional
             Maximal distance of the star cluster.
             Default is ``6.``.
 
-        n_clusters          : `integer`, optional
-            Number of expected cluster in the data. Should be at least 2.
-            One for the actual cluster and one for the filed stars.
-            Default is ``10``.
-
-        random_state        : `integer`, optional
-            Random state parameter used to identify the star cluster.
-            Default is ``2``.
-
-        n_neighbors         : `integer`, optional
-            Neighbors parameter used to identify the star cluster.
-            Default is ``4``.
-
         parameter_set       : `integer`, optional
             Predefined parameter sets can be used.
             Possibilities: ``1``, ``2``, ``3``
             Default is ``1``.
 
         Returns
         -------
@@ -2357,33 +2352,32 @@
         mask                : `boolean numpy.ndarray`
             Mask that needs to be applied to the table.
 
         cluster_mask        : `boolean numpy.ndarray`
             Mask that identifies cluster members according to the user
             input.
 
-    '''
+    """
     #   Get wcs
     w = ensemble.wcs
 
     #   Convert pixel coordinates to ra & dec
     coords = w.all_pix2world(tbl['x'], tbl['y'], 0)
 
     #   Create SkyCoord object with coordinates of all objects
     coords_img = SkyCoord(
         coords[0],
         coords[1],
         unit=(u.degree, u.degree),
         frame="icrs"
-        )
+    )
 
     #   Get reference image
     image = ensemble.ref_img
 
-
     ###
     #   Get Gaia data from Vizier
     #
     #   Columns to download
     columns = [
         'RA_ICRS',
         'DE_ICRS',
@@ -2391,77 +2385,75 @@
         'Plx',
         'e_Plx',
         'pmRA',
         'e_pmRA',
         'pmDE',
         'e_pmDE',
         'RUWE',
-        ]
+    ]
 
     #   Define astroquery instance
     v = Vizier(
         columns=columns,
         row_limit=1e6,
         catalog=catalog,
-        column_filters={'Gmag':'<'+str(Gmag_limit)},
-        )
+        column_filters={'Gmag': '<' + str(Gmag_limit)},
+    )
 
     #   Get data from the corresponding catalog for the objects in the FOV
     result = v.query_region(
         ensemble.coord,
-        radius=ensemble.fov*u.arcmin,
-        )[0]
+        radius=ensemble.fov * u.arcmin,
+    )[0]
 
     #   Restrict proper motion to Simbad value plus some margin
     customSimbad = Simbad()
     customSimbad.add_votable_fields('pm')
 
     result_simbad = customSimbad.query_object(ensemble.objname)
     pmra = result_simbad['PMRA'].value[0]
     pmde = result_simbad['PMDEC'].value[0]
     if pmra != '--' and pmde != '--':
         pm_m = 3.
-        mask_DE = (result['pmDE'] <= pmde-pm_m) | (result['pmDE'] >= pmde+pm_m)
-        mask_RA = (result['pmRA'] <= pmra-pm_m) | (result['pmRA'] >= pmra+pm_m)
+        mask_DE = (result['pmDE'] <= pmde - pm_m) | (result['pmDE'] >= pmde + pm_m)
+        mask_RA = (result['pmRA'] <= pmra - pm_m) | (result['pmRA'] >= pmra + pm_m)
         mask = np.invert(mask_DE | mask_RA)
         result = result[mask]
 
     #   Create SkyCoord object with coordinates of all Gaia objects
     coords_calib = SkyCoord(
-            result['RA_ICRS'],
-            result['DE_ICRS'],
-            unit=(u.degree, u.degree),
-            frame="icrs"
-            )
-
+        result['RA_ICRS'],
+        result['DE_ICRS'],
+        unit=(u.degree, u.degree),
+        frame="icrs"
+    )
 
     ###
     #   Correlate own objects with Gaia objects
     #
     #   Set maximal separation between objects
-    seplimit = seplimit*u.arcsec
+    seplimit = seplimit * u.arcsec
 
     #   Correlate data
     id_img, id_calib, d2ds, d3ds = matching.search_around_sky(
         coords_img,
         coords_calib,
         seplimit,
-        )
-
+    )
 
     ###
     #   Find cluster in proper motion and distance data
     #
 
     #   Proper motion of the common objects
     pmDE = result['pmDE'][id_calib]
     pmRA = result['pmRA'][id_calib]
 
     #   Parallax
-    parallax = result['Plx'][id_calib].data/1000*u.arcsec
+    parallax = result['Plx'][id_calib].data / 1000 * u.arcsec
 
     #   Distance
     distance = parallax.to_value(u.kpc, equivalencies=u.parallax())
 
     #   Restrict sample to objects closer than 'max_distance'
     #   and remove nans and infs
     if max_distance is not None:
@@ -2481,39 +2473,44 @@
 
     #   Prepare SpectralClustering object to identify the "cluster" in the
     #   proper motion and distance data sets
     if parameter_set == 1:
         n_clusters = 2
         random_state = 25
         n_neighbors = 20
-        affinity='nearest_neighbors'
+        affinity = 'nearest_neighbors'
     elif parameter_set == 2:
         n_clusters = 10
         random_state = 2
         n_neighbors = 4
-        affinity='nearest_neighbors'
+        affinity = 'nearest_neighbors'
     elif parameter_set == 3:
         n_clusters = 2
         random_state = 25
         n_neighbors = 20
-        affinity='rbf'
-    spectral_cluster_model= SpectralClustering(
-        #eigen_solver='lobpcg',
+        affinity = 'rbf'
+    else:
+        raise RuntimeError(
+            f"{style.bcolors.FAIL} \nNo valid parameter set defined: "
+            f"Possibilities are 1, 2, or 3. {style.bcolors.ENDC}"
+        )
+    spectral_cluster_model = SpectralClustering(
+        # eigen_solver='lobpcg',
         n_clusters=n_clusters,
         random_state=random_state,
-        #gamma=2.,
-        #gamma=5.,
+        # gamma=2.,
+        # gamma=5.,
         n_neighbors=n_neighbors,
         affinity=affinity,
     )
 
     #   Find "cluster" in the data
     pd_result['cluster'] = spectral_cluster_model.fit_predict(
         pd_result[['pmDE', 'pmRA', 'distance']],
-        )
+    )
 
     #   3D plot of the proper motion and the distance
     #   -> select the star cluster by eye
     groups = pd_result.groupby('cluster')
     pmRA_group = []
     pmDE_group = []
     distance_group = []
@@ -2522,88 +2519,87 @@
         pmDE_group.append(group.pmDE.values)
         distance_group.append(group.distance.values)
     plot.D3_scatter(
         pmRA_group,
         pmDE_group,
         distance_group,
         image.outpath.name,
-        #color=np.unique(pd_result['cluster']),
+        # color=np.unique(pd_result['cluster']),
         name_x='pm_RA * cos(DEC) (mas/yr)',
         name_y='pm_DEC (mas/yr)',
         name_z='d (kpc)',
         string='_3D_cluster_',
         pmra=pmra,
         pmde=pmde,
-        )
+    )
     plot.D3_scatter(
         pmRA_group,
         pmDE_group,
         distance_group,
         image.outpath.name,
-        #color=np.unique(pd_result['cluster']),
+        # color=np.unique(pd_result['cluster']),
         name_x='pm_RA * cos(DEC) (mas/yr)',
         name_y='pm_DEC (mas/yr)',
         name_z='d (kpc)',
         string='_3D_cluster_',
         pmra=pmra,
         pmde=pmde,
         display=True,
-        )
+    )
 
-    #plot.D3_scatter(
-        #[pd_result['pmRA']],
-        #[pd_result['pmDE']],
-        #[pd_result['distance']],
-        #image.outpath.name,
-        #color=[pd_result['cluster']],
-        #name_x='pm_RA * cos(DEC) (mas/yr)',
-        #name_y='pm_DEC (mas/yr)',
-        #name_z='d (kpc)',
-        #string='_3D_cluster_',
-        #)
+    # plot.D3_scatter(
+    # [pd_result['pmRA']],
+    # [pd_result['pmDE']],
+    # [pd_result['distance']],
+    # image.outpath.name,
+    # color=[pd_result['cluster']],
+    # name_x='pm_RA * cos(DEC) (mas/yr)',
+    # name_y='pm_DEC (mas/yr)',
+    # name_z='d (kpc)',
+    # string='_3D_cluster_',
+    # )
 
     #   Get user input
-    cluter_id, timedOut = timedInput(
-            style.bcolors.OKBLUE+
-            "   Which one is the correct cluster (id)? "
-            +style.bcolors.ENDC,
-            timeout=300,
-            )
-    if timedOut or cluter_id == '':
-        cluter_id = 0
+    cluster_id, timedOut = timedInput(
+        style.bcolors.OKBLUE +
+        "   Which one is the correct cluster (id)? "
+        + style.bcolors.ENDC,
+        timeout=300,
+    )
+    if timedOut or cluster_id == '':
+        cluster_id = 0
     else:
-        cluter_id = int(cluter_id)
+        cluster_id = int(cluster_id)
 
     #   Calculated mask according to user input
-    cluster_mask = pd_result['cluster']==cluter_id
+    cluster_mask = pd_result['cluster'] == cluster_id
 
     #   Apply correlation results and masks to the input table
     tbl = tbl[id_img][mask][cluster_mask.values]
 
-
     ###
     #   Make star map
     #
     prepare_and_plot_starmap(
         image,
         tbl=tbl,
         x_name='x',
         y_name='y',
         rts_pre='img-pmGaia-distance-cluster',
         label='Cluster members based on proper motion and distance',
         add_image_id=False,
-        )
+    )
 
     #   Return table
     return tbl, id_img, mask, cluster_mask.values
 
 
-def save_mags_ascii(container, tbl, trans=False, ID='', rts='',
+def save_mags_ascii(container, tbl, trans=False, id_object=None, rts='',
                     photo_type='', doadd=True):
-    '''
+    """
         Save magnitudes as ASCII files
 
         Parameters
         ----------
         container       : `image.container`
             Image container object with image ensemble objects for each
             filter
@@ -2611,106 +2607,119 @@
         tbl             : `astropy.table.Table`
             Table with magnitudes
 
         trans           : `boolean`, optional
             If True a magnitude transformation was performed
             Default is ``False``.
 
-        ID              : `string`, optional
+        id_object       : `integer` or `None`, optional
             ID of the object
-            Default is ``''``.
+            Default is ``None``.
 
         rts             : `string`, optional
             Additional string characterizing that should be included in the
             file name.
             Default is ``''``.
 
         photo_type      : `string`, optional
             Applied extraction method. Possibilities: ePSF or APER`
             Default is ``''``.
 
         doadd          : `boolean`, optional
             If True the file path will be added to the container object.
             Default is ``True``.
-    '''
+    """
     #   Check output directories
     outdir = list(container.ensembles.values())[0].outpath
     checks.check_out(
         outdir,
         outdir / 'tables',
-        )
+    )
 
     #   Define file name specifier
-    if ID != '':
-        ID = '_img_'+str(ID)
+    if id_object is not None:
+        id_object = f'_img_{id_object}'
+    else:
+        id_object = ''
     if photo_type != '':
-        photo_type = '_'+photo_type
-
-    #   Define output formats for the table columns
-    formats = {
-        'x': '%12.2f',
-        'y': '%12.2f',
-        "B [mag]": '%12.3f',
-        "B_err [mag]": '%12.3f',
-        "V [mag]": '%12.3f',
-        "V_err [mag]": '%12.3f',
-        "B-V [mag]": '%12.3f',
-        "B-V_err [mag]": '%12.3f',
-        }
+        photo_type = f'_{photo_type}'
 
     #   Check if ``container`` object contains already entries
     #   for file names/paths. If not add dictionary.
     photo_filepath = getattr(container, 'photo_filepath', None)
     if photo_filepath is None or not isinstance(photo_filepath, dict):
         container.photo_filepath = {}
 
     #   Set file name
     if trans:
         #   Set file name for file with magnitude transformation
-        filename = 'mags_TRANS_calibrated'+photo_type+ID+rts+'.dat'
+        filename = f'mags_TRANS_calibrated{photo_type}{id_object}{rts}.dat'
     else:
         #   File name for file without magnitude transformation
-        filename = 'mags_calibrated'+photo_type+ID+rts+'.dat'
+        filename = f'mags_calibrated{photo_type}{id_object}{rts}.dat'
 
     #   Combine to a path
     out_path = outdir / 'tables' / filename
 
     #   Add to object
     if doadd:
         container.photo_filepath[out_path] = trans
 
+    ###
+    #   Define output formats for the table columns
+    #
+    #   Get column names
+    colnames = tbl.colnames
+
+    #   Set default
+    for colname in colnames:
+        tbl[colname].info.format = '{:12.3f}'
+
+    #   Reset for x and y column
+    formats = {
+        'x': '{:12.2f}',
+        'y': '{:12.2f}',
+        # "B [mag]": '%12.3f',
+        # "B_err [mag]": '%12.3f',
+        # "V [mag]": '%12.3f',
+        # "V_err [mag]": '%12.3f',
+        # "B-V [mag]": '%12.3f',
+        # "B-V_err [mag]": '%12.3f',
+    }
+
     #   Write file
     tbl.write(
         str(out_path),
         format='ascii',
         overwrite=True,
         formats=formats,
-        )
+    )
 
 
-def postprocess_results(img_container, filter_list, ID='', photo_type='',
+def postprocess_results(img_container, filter_list, id_object=None, photo_type='',
                         region=False, radius=600, data_cluster=False,
-                        pm_median=False, n_clusters=10,
-                        max_distance_cluster=6., find_cluster_para_set=1):
-    '''
+                        pm_median=False, max_distance_cluster=6.,
+                        find_cluster_para_set=1, convert_mags=False,
+                        target_filter_system='SDSS', tbl_list=None):
+    """
         Restrict results to specific areas of the image and filter by means
         of proper motion and distance using Gaia
 
         Parameters
         ----------
         img_container           : `image.container`
             Image container object with image ensemble objects for each
             filter
 
         filter_list             : `list` of `string`
             Filter names
 
-        ID                      : `string`, optional
+        id_object               : `integer` or `None`, optional
             ID of the object
-            Default is ``''``.
+            Default is ``None``.
 
         photo_type              : `string`, optional
             Applied extraction method. Possibilities: ePSF or APER`
             Default is ``''``.
 
         region                  : `boolean`, optional
             If True the extracted objects will be filtered such that only
@@ -2727,93 +2736,332 @@
             Default is ``False``.
 
         pm_median               : `boolean`, optional
             If True only the objects that are close to the median
             proper motion will be returned.
             Default is ``False``.
 
-        n_clusters              : `integer`, optional
-            Number of expected cluster in the data. Should be at least 2.
-            One for the actual cluster and one for the filed stars.
-            Default is ``10``.
-
         max_distance_cluster    : `float`, optional
             Expected maximal distance of the cluster in kpc. Used to
             restrict the parameter space to facilitate an easy
             identification of the star cluster.
             Default is ``6``.
 
         find_cluster_para_set   : `integer`, optional
             Parameter set used to identify the star cluster in proper
             motion and distance data.
-    '''
+
+        convert_mags            : `boolean`, optional
+            If True the magnitudes will be converted to another
+            filter systems specified in `target_filter_system`.
+            Default is ``False``.
+
+        target_filter_system    : `string`, optional
+            Photometric system the magnitudes should be converted to
+            Default is ``SDSS``.
+
+        tbl_list                : `[astropy.table.Table]` or None, optional
+            List with Tables containing magnitudes etc. If None are provided,
+            the tables will be read from the image container.
+            Default is ``None``.
+
+    """
     #   Do nothing if no post process method were defined
-    if not region and not pm_median and not data_cluster:
+    if not region and not pm_median and not data_cluster and not convert_mags:
         return
 
     #   Get image ensembles
     img_ensembles = img_container.ensembles
 
     #   Get paths to the tables with the data
-    paths = img_container.photo_filepath
-
-    #   Loop over all Tables
-    first = True
-    for path, trans in paths.items():
-        #   Read Table
-        tbl = Table.read(path, format='ascii')
+    # paths = img_container.photo_filepath
 
+    #   Get astropy tables with positions and magnitudes
+    if tbl_list is None or not tbl_list:
+        tbl_list = [
+            (getattr(img_container, 'table_mags_transformed', None), True),
+            (getattr(img_container, 'table_mags_not_transformed', None), False),
+        ]
 
+    #   Loop over all Tables
+    mask_region = None
+    img_id_cluster = None
+    mask_cluster = None
+    mask_objects = None
+    img_id_pm = None
+    mask_pm = None
+    for (tbl, trans) in tbl_list:
         ###
         #   Postprocess data
         #
 
         #   Extract circular region around a certain object
         #   such as a star cluster
         if region:
-            if first:
+            if mask_region is None:
                 tbl, mask_region = region_selection(
                     img_ensembles[filter_list[0]],
                     img_container.coord,
                     tbl,
                     radius=radius
-                    )
+                )
             else:
                 tbl = tbl[mask_region]
 
         #   Find a cluster in the Gaia data that could be the star cluster
         if data_cluster:
-            if first:
+            if any(x is None for x in [img_id_cluster, mask_cluster, mask_objects]):
                 tbl, img_id_cluster, mask_cluster, mask_objects = find_cluster(
                     img_ensembles[filter_list[0]],
                     tbl,
-                    n_clusters=n_clusters,
                     max_distance=max_distance_cluster,
                     parameter_set=find_cluster_para_set,
-                    )
+                )
             else:
                 tbl = tbl[img_id_cluster][mask_cluster][mask_objects]
 
         #   Clean objects according to proper motion (Gaia)
         if pm_median:
-            if first:
+            if any(x is None for x in [img_id_pm, mask_pm]):
                 tbl, img_id_pm, mask_pm = proper_motion_selection(
                     img_ensembles[filter_list[0]],
                     tbl,
-                    )
+                )
             else:
                 tbl = tbl[img_id_pm][mask_pm]
 
+        #   Convert magnitudes to a different filter system
+        if convert_mags:
+            tbl = convert_magnitudes(tbl, target_filter_system)
+
         ###
         #   Save results as ASCII files
         #
         save_mags_ascii(
             img_container,
             tbl,
             trans=trans,
-            ID=ID,
-            rts='_selection',
+            id_object=id_object,
+            rts='_postprocessed',
             photo_type=photo_type,
             doadd=False,
-            )
+        )
+
+
+def convert_magnitudes_internal_wrapper(img_container, target_filter_system):
+    """
+        Gets astropy table with  magnitudes from image container and
+        calls then the magnitude conversion.
+
+        Parameters
+        ----------
+        img_container           : `image.container`
+            Container object with image ensemble objects for each filter
+
+        target_filter_system    : `string`
+            Photometric system the magnitudes should be converted to
+    """
+    # #   Get calibrated magnitudes
+    # cali_mags = img_container.get_calibrated_magnitudes()
+
+    #   Get astropy tables with magnitudes
+    tbl_transformed = getattr(img_container, 'table_mags_transformed', None)
+    tbl_not_transformed = getattr(
+        img_container,
+        'table_mags_not_transformed',
+        None,
+    )
+
+    #   Convert magnitudes
+    if tbl_transformed is not None:
+        convert_magnitudes(tbl_transformed, target_filter_system)
+    if tbl_not_transformed is not None:
+        convert_magnitudes(tbl_not_transformed, target_filter_system)
+
+
+def add_column_to_table(tbl, column_name, data, column_id):
+    """
+        Adds data from an unumpy array to an astropy Table
+
+        Parameters
+        ----------
+        tbl                 : `atropy.table.Table`
+            Table that already contains some data
+
+        column_name         : `string`
+            Name of the column to add
+
+        data                : `uncertainties.unumpy.ndarray`
+            Data to add
+
+        column_id           : `integer`
+            Additional ID that identifies the column. If the
+            ID is not -1 it will be added to the column header.
+
+        Returns
+        -------
+        tbl                 : `atropy.table.Table`
+            Table with the added column
+    """
+    if column_id == -1:
+        tbl.add_columns(
+            [
+                unumpy.nominal_values(data) * u.mag,
+                unumpy.std_devs(data) * u.mag,
+            ],
+            names=[column_name, f'{column_name}_err',
+                   ]
+        )
+    else:
+        tbl.add_columns(
+            [
+                unumpy.nominal_values(data) * u.mag,
+                unumpy.std_devs(data) * u.mag,
+            ],
+            names=[
+                f'{column_name} ({column_id})',
+                f'{column_name}_err ({column_id})',
+            ]
+        )
+
+    return tbl
+
+
+def convert_magnitudes(tbl: Table, target_filter_system: str) -> Table:
+    """
+        Convert magnitudes from one system to another
+
+        Parameters
+        ----------
+        tbl                 : `astropy.table.Table`
+            Table with magnitudes
+
+        target_filter_system    : `string`
+            Photometric system the magnitudes should be converted to
+    """
+    #   Get column names
+    colnames = tbl.colnames
+
+    #   Checks
+    if target_filter_system not in ['SDSS', 'AB', 'BESSELL']:
+        terminal_output.print_terminal(
+            target_filter_system,
+            string='Magnitude conversion not possible.Unfortunately, '
+                   'there is currently no conversion formula for this '
+                   'photometric system: {}.',
+            style_name='WARNING',
+        )
+
+    #   Select magnitudes and errors and corresponding filter
+    available_image_ids = []
+    available_filter_image_error = []
+
+    #   Loop over column names
+    for colname in colnames:
+        #   Detect color: 'continue in this case, since colors are not yet supported'
+        if len(colname) > 1 and colname[1] == '-':
+            continue
+
+        #   Get filter
+        column_filter = colname[0]
+        if column_filter in ['i', 'x', 'y']:
+            continue
+
+        #   Get the image ID
+        image_id = colname.split('(')[1].split(')')[0]
+
+        #   Is an image ID available?
+        if image_id != '':
+            #   Check for error column
+            error = any(x == f'{column_filter}_err ({image_id})' for x in colnames)
+
+            #   Combine derived infos -> (ID of the image, Filter, boolean: error available?)
+            info = (image_id, column_filter, error)
+        else:
+            #   Set dummy image ID
+            image_id = -1
+
+            #   Check for error column
+            error = any(x == f'{column_filter}_err' for x in colnames)
+
+            #   Combine derived infos -> (ID of the image, Filter, boolean: error available?)
+            info = (-1, column_filter, error)
+
+        #   Check if image and filter combination is already known. If yes continue.
+        if info in available_filter_image_error:
+            continue
+
+        #   Save image, filter, & error info
+        available_filter_image_error.append(info)
+
+        if image_id not in available_image_ids:
+            available_image_ids.append(image_id)
+
+    #   Make conversion for each image ID individually
+    for image_id in available_image_ids:
+        #   Reset dictionary with data
+        data_dict = {}
+
+        #   Get image ID, filter and error combination
+        for (current_image_id, column_filter, error) in available_filter_image_error:
+            #   Restrict to current image ID
+            if current_image_id != image_id:
+                continue
+
+            #   Fill data dictionary, branch according to error and image ID availability
+            if image_id == -1:
+                if error:
+                    data_dict[column_filter] = unumpy.uarray(
+                        tbl[f'{column_filter}'].value,
+                        tbl[f'{column_filter}_err'].value
+                    )
+                else:
+                    data_dict[column_filter] = tbl[f'{column_filter}'].value
+            else:
+                if error:
+                    data_dict[column_filter] = unumpy.uarray(
+                        tbl[f'{column_filter} ({image_id})'].value,
+                        tbl[f'{column_filter}_err ({image_id})'].value
+                    )
+                else:
+                    data_dict[column_filter] = tbl[f'{column_filter} ({image_id})'].value
+
+        # print('data_dict', data_dict)
+
+        if target_filter_system == 'AB':
+            print('Will be available soon...')
+
+        elif target_filter_system == 'SDSS':
+            #   Get conversion function - only Jordi et a. (2005) currently available:
+            calib_functions = calibration_data \
+                .filter_system_conversions['SDSS']['Jordi_et_al_2005']
+
+            #   Convert magnitudes and add those to data dictionary and the Table
+            g = calib_functions['g'](**data_dict)
+            if g is not None:
+                data_dict['g'] = g
+                tbl = add_column_to_table(tbl, 'g', g, image_id)
+
+            u = calib_functions['u'](**data_dict)
+            if u is not None:
+                data_dict['u'] = u
+                tbl = add_column_to_table(tbl, 'u', u, image_id)
+
+            r = calib_functions['r'](**data_dict)
+            if r is not None:
+                data_dict['r'] = r
+                tbl = add_column_to_table(tbl, 'r', r, image_id)
+
+            i = calib_functions['i'](**data_dict)
+            if i is not None:
+                data_dict['i'] = i
+                tbl = add_column_to_table(tbl, 'i', i, image_id)
+
+            z = calib_functions['z'](**data_dict)
+            if z is not None:
+                data_dict['z'] = z
+                tbl = add_column_to_table(tbl, 'z', z, image_id)
+
+        elif target_filter_system == 'BESSELL':
+            print('Will be available soon...')
 
-        first = False
+        return tbl
```

### Comparing `ost_photometry-0.0.7/src/ost_photometry/analyze/calib.py` & `ost_photometry-0.0.8/src/ost_photometry/analyze/calib.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.7/src/ost_photometry/analyze/correlate.py` & `ost_photometry-0.0.8/src/ost_photometry/analyze/correlate.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.7/src/ost_photometry/analyze/plot.py` & `ost_photometry-0.0.8/src/ost_photometry/analyze/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -2395,7 +2395,67 @@
     #   Save plot
     plt.savefig(
         outdir+'/scatter/'+rts+'.pdf',
         bbox_inches='tight',
         format='pdf',
                )
     plt.close()
+
+
+def plot_limiting_mag_sky_apertures(outdir, img_data, mask, depth):
+    '''
+        Plot the sky apertures that are used to estimate the limiting magnitude
+
+        Parameters
+        ----------
+        outdir          : `string`
+            Output directory
+
+        img_data            : `numpy.ndarray`
+            Image data
+
+        mask                : `numpy.ndarray`
+            Mask showing the position of detected objects
+
+        depth               : `photutils.utils.ImageDepth`
+            Object used to derive the limiting magnitude
+    '''
+    #   Check output directories
+    checks.check_out(
+        outdir,
+        os.path.join(outdir, 'limiting_mag'),
+        )
+
+    #   Plot magnitudes
+    fig, ax = plt.subplots(nrows=1, ncols=2, figsize=(9, 3))
+
+    #   Set titel
+    ax[0].set_title('Data with blank apertures')
+    ax[1].set_title('Mask with blank apertures')
+
+    #   Normalize the image data and plot
+    norm = simple_norm(img_data, 'sqrt', percent=99.)
+    ax[0].imshow(img_data, norm=norm)
+
+    #   Plot mask with object positions
+    ax[1].imshow(mask, interpolation='none')
+
+    #   Plot apertures used to derive limiting magnitude
+    color = 'orange'
+    depth.apertures[0].plot(ax[0], color=color)
+    depth.apertures[0].plot(ax[1], color=color)
+
+    plt.subplots_adjust(
+        left=0.05,
+        right=0.98,
+        bottom=0.05,
+        top=0.95,
+        wspace=0.15,
+        )
+
+    #   Save plot
+    plt.savefig(
+        outdir+'/limiting_mag/limiting_mag_sky_regions.pdf',
+        bbox_inches='tight',
+        format='pdf',
+               )
+    plt.close()
```

### Comparing `ost_photometry-0.0.7/src/ost_photometry/analyze/trans.py` & `ost_photometry-0.0.8/src/ost_photometry/analyze/trans.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from astropy.stats import sigma_clipped_stats
 from astropy.stats import sigma_clip as sigma_clipping
 
 from . import calib, analyze, aux, plot
 
 from .. import checks, style, calibration_data, terminal_output
 
+
 ############################################################################
 ####                        Routines & definitions                      ####
 ############################################################################
 
 def cal_err_T(image, lit_mags, color_mag, Tc, cali, id_1, id_2, id_f,
               ttype='simple', air_mass=1.0):
     '''
@@ -71,87 +72,87 @@
     #   Number of stars
     count = len(image.mags['err'])
 
     #   Define new array
     u = np.zeros(count, dtype=[('err', 'f8')])
 
     #   ZP errors
-    uZP      = aux.err_prop(image.mags_fit['err'], lit_mags['err'][id_f])
+    uZP = aux.err_prop(image.mags_fit['err'], lit_mags['err'][id_f])
     uZP_clip = np.median(uZP[mask])
 
     #   Literature color errors
-    ucl      = aux.err_prop(lit_mags['err'][id_1], lit_mags['err'][id_2])
+    ucl = aux.err_prop(lit_mags['err'][id_1], lit_mags['err'][id_2])
     ucl_clip = np.median(ucl[mask])
 
-    for i in range(0,count):
+    for i in range(0, count):
         #   Err: delta(color) [(inst_2 - inst_1) - (lit_2 - lit_1)]
         udc = aux.err_prop(
             image.mags_1['err'][i],
             image.mags_2['err'][i],
             ucl_clip,
-            )
+        )
 
         #   Color
         color = color_mag[i]
 
         #   Errors including magnitude transformation
         if ttype == 'simple':
             u_obj = aux.err_prop(
                 image.mags['err'][i],
                 uZP_clip,
                 Tc['color'] * color * Tc['C_err'],
                 Tc['C'] * color * Tc['color_err'],
                 Tc['C'] * Tc['color'] * udc,
-                )
+            )
         elif ttype == 'airmass':
             #   Calculate calibration factor
             C_1 = Tc['T_1'] - Tc['k_1'] * air_mass
             C_2 = Tc['T_2'] - Tc['k_2'] * air_mass
 
             #   C_1 & C_2 errors
-            uC_1 = aux.err_prop(Tc['T_1_err'], air_mass*Tc['k_1_err'])
-            uC_2 = aux.err_prop(Tc['T_2_err'], air_mass*Tc['k_2_err'])
+            uC_1 = aux.err_prop(Tc['T_1_err'], air_mass * Tc['k_1_err'])
+            uC_2 = aux.err_prop(Tc['T_2_err'], air_mass * Tc['k_2_err'])
 
         elif ttype == 'derive':
             C_1 = image.C_1
             C_2 = image.C_2
             uC_1 = image.C_1_err
             uC_2 = image.C_2_err
         else:
             raise Exception(
                 f"{style.bcolors.FAIL} \nType of magnitude transformation not "
                 "known \n\t-> Check calibration coefficients \n\t-> Exit"
                 f"{style.bcolors.ENDC}"
-                )
+            )
 
         if ttype in ['airmass', 'derive']:
             #   Calculate the corresponding denominator
-            d    = 1. - C_1 + C_2
+            d = 1. - C_1 + C_2
 
             #   Denominator error
-            u_d  = aux.err_prop(uC_1, uC_2)
+            u_d = aux.err_prop(uC_1, uC_2)
 
             #   C or more precise C'
             if id_f == id_1:
                 C = C_1 / d
             elif id_f == id_2:
                 C = C_2 / d
 
             #   C error
             if id_f == id_1:
-                u_C = aux.err_prop(uC_1*d, u_d*C_1/d/d)
+                u_C = aux.err_prop(uC_1 * d, u_d * C_1 / d / d)
             elif id_f == id_2:
-                u_C = aux.err_prop(uC_2*d, u_d*C_2/d/d)
+                u_C = aux.err_prop(uC_2 * d, u_d * C_2 / d / d)
 
             u_obj = aux.err_prop(
                 image.mags['err'][i],
                 uZP_clip,
                 u_C * color,
                 C * udc,
-                )
+            )
 
         u['err'][i] = np.mean(u_obj)
 
     return u['err']
 
 
 def cal_err(mask, mags_fit, lit_mags, mags, cali):
@@ -177,22 +178,22 @@
 
         Returns
         -------
         u           : `numpy.ndarray`
             Propagated uncertainty
     '''
     #   ZP errors
-    uZP      = aux.err_prop(mags_fit, lit_mags)
+    uZP = aux.err_prop(mags_fit, lit_mags)
     uZP_clip = np.median(uZP[mask])
 
     #   Add up errors
     u = aux.err_prop(
         mags,
         uZP_clip,
-        )
+    )
 
     return u
 
 
 def cal_sigma_plot(m_fit, masked, filt, m_lit, outdir, nameobj, rts,
                    fit=None, m_fit_err=None, m_lit_err=None):
     '''
@@ -234,42 +235,42 @@
             Error of the filter 1 magnitudes
 
     '''
     p = mp.Process(
         target=plot.plot_mags,
         args=(
             m_fit[masked],
-            filt+'_inst',
+            filt + '_inst',
             m_lit[masked],
-            filt+'_lit',
-            'mags_sigma_'+filt+rts,
+            filt + '_lit',
+            'mags_sigma_' + filt + rts,
             outdir,
-            ),
+        ),
         kwargs={
-            'nameobj':nameobj,
-            'fit':fit,
-            'err1':m_fit_err,
-            'err2':m_lit_err,
-            }
-        )
+            'nameobj': nameobj,
+            'fit': fit,
+            'err1': m_fit_err,
+            'err2': m_lit_err,
+        }
+    )
     p.start()
     p = mp.Process(
         target=plot.plot_mags,
         args=(
             m_fit,
-            filt+'_inst',
+            filt + '_inst',
             m_lit,
-            filt+'_lit',
-            'mags_no_sigma_'+filt+rts,
+            filt + '_lit',
+            'mags_no_sigma_' + filt + rts,
             outdir,
-            ),
+        ),
         kwargs={
-            'nameobj':nameobj,
-            }
-        )
+            'nameobj': nameobj,
+        }
+    )
     p.start()
 
 
 def cal_sigma_plot_color(filt, outdir, nameobj, f_list, id_1, id_2,
                          color_fit, color_lit, color_fit_clip,
                          color_lit_clip, rts):
     '''
@@ -310,39 +311,39 @@
         rts             : `string`
                 Expression characterizing the plot
     '''
     p = mp.Process(
         target=plot.plot_mags,
         args=(
             color_fit_clip,
-            f_list[id_1]+'-'+f_list[id_2]+'_inst',
+            f_list[id_1] + '-' + f_list[id_2] + '_inst',
             color_lit_clip,
-            f_list[id_1]+'-'+f_list[id_2]+'_lit',
-            'color_sigma_'+filt+rts,
+            f_list[id_1] + '-' + f_list[id_2] + '_lit',
+            'color_sigma_' + filt + rts,
             outdir,
-            ),
+        ),
         kwargs={
-            'nameobj':nameobj,
-            }
-        )
+            'nameobj': nameobj,
+        }
+    )
     p.start()
     p = mp.Process(
         target=plot.plot_mags,
         args=(
             color_fit,
-            f_list[id_1]+'-'+f_list[id_2]+'_inst',
+            f_list[id_1] + '-' + f_list[id_2] + '_inst',
             color_lit,
-            f_list[id_1]+'-'+f_list[id_2]+'_lit',
-            'color_no_sigma_'+filt+rts,
+            f_list[id_1] + '-' + f_list[id_2] + '_lit',
+            'color_no_sigma_' + filt + rts,
             outdir,
-            ),
+        ),
         kwargs={
-            'nameobj':nameobj,
-            }
-        )
+            'nameobj': nameobj,
+        }
+    )
     p.start()
 
 
 def prepare_trans_variables(img_container, id_img_i, filt_o, filt_i,
                             filt_id_1, filter_list, id_tuple_trans):
     '''
         Prepare variables for magnitude transformation
@@ -404,22 +405,22 @@
 
     #   Set values for mag_fit_1 and mag_fit_2 to allow
     #   calculation of the correct color later on
     if filt_id_1 == filt_i:
         img_i.mag_fit_1 = img_i.mags_fit
         img_i.mag_fit_2 = img_o.mags_fit
 
-        img_i.mags_1    = img_i.mags
-        img_i.mags_2    = img_o.mags
+        img_i.mags_1 = img_i.mags
+        img_i.mags_2 = img_o.mags
     else:
         img_i.mag_fit_1 = img_o.mags_fit
         img_i.mag_fit_2 = img_i.mags_fit
 
-        img_i.mags_1    = img_o.mags
-        img_i.mags_2    = img_i.mags
+        img_i.mags_1 = img_o.mags
+        img_i.mags_2 = img_i.mags
 
     return img_o
 
 
 def prepare_trans(img_container, Tcs, filter_list, filt_i, id_img_i,
                   id_tuple_notrans, derive_Tcs=False):
     '''
@@ -484,15 +485,15 @@
     #   coefficients. If not, try to derive calibration coefficients.
     if Tcs is not None and not derive_Tcs:
         Tc, filt_id_1, filt_id_2 = aux.find_filt(
             filter_list,
             Tcs,
             band,
             img_i.instrument,
-            )
+        )
 
         if Tc is not None and 'type' in Tc.keys():
             Tc_type = Tc['type']
 
             #   Get correct filter order
             if filt_id_1 == filt_i:
                 filt_o = filt_id_2
@@ -507,15 +508,15 @@
             #   the second in 'filter_list' or the one in 'filter_list'
             #    with the ID one below the first filter ID.
             filt_id_1 = filt_i
 
             if filt_id_1 == 0:
                 filt_id_2 = 1
             else:
-                filt_id_2 = filt_id_1-1
+                filt_id_2 = filt_id_1 - 1
 
             filt_o = filt_id_2
         else:
             Tc_type = None
 
     elif len(filter_list) >= 2:
         Tc_type = 'derive'
@@ -524,45 +525,44 @@
         filt_id_1 = None
         filt_id_2 = None
 
         #   Check if calibration data is available for the
         #   filter in``filter_list`
         filter_calib = img_container.calib_parameters.column_names
         for band in filter_list:
-            if 'mag'+band not in filter_calib:
+            if 'mag' + band not in filter_calib:
                 Tc_type = None
 
-
         if Tc_type is not None:
             #   Get correct filter ids: The first filter is the
             #   current filter, while the second filter is either
             #   the second in 'filter_list' or the one in 'filter_list'
             #    with the ID one below the first filter ID.
             filt_id_1 = filt_i
 
             if filt_id_1 == 0:
                 filt_id_2 = 1
             else:
-                filt_id_2 = filt_id_1-1
+                filt_id_2 = filt_id_1 - 1
 
             filt_o = filt_id_2
 
     if Tc_type is None:
         filt_o = None
         filt_id_1 = None
         filt_id_2 = None
         Tc = None
 
     if Tc_type == 'simple':
         string = "Apply simple magnitude transformation"
     elif Tc_type == 'airmass':
         string = "Apply magnitude transformation accounting for airmass"
     elif Tc_type == 'derive':
-        string = "Derive and apply magnitude transformation based on "\
-                "current image"
+        string = "Derive and apply magnitude transformation based on " \
+                 "current image"
     if Tc_type is not None:
         terminal_output.print_terminal(indent=3, string=string)
 
     #   Save filter and image ID configuration to allow
     #   for a better color calculation later on
     id_tuple_notrans.append((filt_i, id_img_i))
 
@@ -618,19 +618,19 @@
         T_1                 : `ufloat` or `float`
             Color correction term for filter 1.
 
         T_2                 : `ufloat` or `float`
             Color correction term for filter 2.
     '''
     #   Initial guess for the parameters
-    #x0    = np.array([0.0, 0.0])
-    x0    = np.array([1.0, 1.0])
+    # x0    = np.array([0.0, 0.0])
+    x0 = np.array([1.0, 1.0])
 
     #   Fit function
-    fit_func=aux.lin_func
+    fit_func = aux.lin_func
 
     #   Get required type for magnitude array.
     unc = checks.check_unumpy_array(color_lit_clip)
 
     #   Get variables
     diff_mag_1 = lit_mag_1 - mag_cali_fit_1
     diff_mag_2 = lit_mag_2 - mag_cali_fit_2
@@ -651,26 +651,26 @@
     #   Fit
     Z_1, Z_1_err, T_1, T_1_err = aux.fit_curve(
         fit_func,
         color_lit_plot,
         diff_mag_plot_1,
         x0,
         sigma,
-        )
+    )
     Z_2, Z_2_err, T_2, T_2_err = aux.fit_curve(
         fit_func,
         color_lit_plot,
         diff_mag_plot_2,
         x0,
         sigma,
-        )
+    )
     if np.isinf(Z_1_err):
-        Z_1_err=None
+        Z_1_err = None
     if np.isinf(Z_2_err):
-        Z_2_err=None
+        Z_2_err = None
 
     #   Plots magnitude difference (literature vs. measured) vs. color
     plot.plot_transform(
         image.outpath.name,
         f_list[id_1],
         f_list[id_2],
         color_lit_plot,
@@ -680,15 +680,15 @@
         T_1_err,
         fit_func,
         image.air_mass,
         filt=f_list[id_f],
         color_lit_err=color_lit_err_plot,
         fit_var_err=Z_1_err,
         nameobj=image.objname,
-        )
+    )
 
     if id_f == id_1:
         id_o = id_2
     else:
         id_o = id_1
     plot.plot_transform(
         image.outpath.name,
@@ -701,24 +701,24 @@
         T_2_err,
         fit_func,
         image.air_mass,
         filt=f_list[id_o],
         color_lit_err=color_lit_err_plot,
         fit_var_err=Z_2_err,
         nameobj=image.objname,
-        )
+    )
 
     #   Return ufloat of normal float
     if unc:
         return ufloat(T_1, T_1_err), ufloat(T_2, T_2_err)
     else:
-        image.C_1 = T_1             #   Dirty hack
-        image.C_2 = T_2             #   Dirty hack
-        image.C_1_err = T_1_err     #   Dirty hack
-        image.C_2_err = T_2_err     #   Dirty hack
+        image.C_1 = T_1  # Dirty hack
+        image.C_2 = T_2  # Dirty hack
+        image.C_1_err = T_1_err  # Dirty hack
+        image.C_2_err = T_2_err  # Dirty hack
         return T_1, T_2
 
 
 def apply_trans(*args, **kwargs):
     '''
         Apply magnitude transformation and return calibrated magnitude array
 
@@ -825,20 +825,19 @@
     color_fit_clip = color_fit[mask]
 
     #   Literature color of the calibration objects
     color_lit = lit_mag_1 - lit_mag_2
     #   Mask data according to sigma clipping
     color_lit_clip = color_lit[mask]
 
-
     ###
     #   Apply magnitude transformation and calibration
     #
     #   Color
-    color_mag   = mags_1 - mags_2
+    color_mag = mags_1 - mags_2
     image.color_mag = color_mag
 
     #   Distinguish between versions
     if ttype == 'simple':
         #   Calculate calibration factor
         C = Tc_C * Tc_color
     elif ttype == 'airmass':
@@ -855,57 +854,57 @@
             id_1,
             id_2,
             color_lit_clip,
             lit_mag_1[mask],
             lit_mag_2[mask],
             mag_cali_fit_1[mask],
             mag_cali_fit_2[mask],
-            )
+        )
 
     else:
         raise Exception(
             f"{style.bcolors.FAIL}\nType of magnitude transformation not known"
             "\n\t-> Check calibration coefficients \n\t-> Exit"
             f"{style.bcolors.ENDC}"
-            )
+        )
 
     if ttype in ['airmass', 'derive']:
         #   Calculate C or more precise C'
 
         denominator = 1. - C_1 + C_2
 
         if id_f == id_1:
-            C   = C_1 / denominator
+            C = C_1 / denominator
         elif id_f == id_2:
-            C   = C_2 / denominator
+            C = C_2 / denominator
         else:
             raise Exception(
                 f"{style.bcolors.FAIL} \nMagnitude transformation: filter "
                 "combination not valid \n\t-> This should never happen. The "
                 f"current filter  ID is {id_f}, while filter IDs are {id_1} "
                 f"and {id_2} {style.bcolors.ENDC}"
-                )
+            )
 
     #   Calculate calibrated magnitudes
     mag_cali = mags + np.median(ZP - C * color_fit_clip) + C * color_mag
 
     p = mp.Process(
         target=plot.plot_mags,
         args=(
             unumpy.nominal_values(mag_cali),
-            image.filt+'_calib',
+            image.filt + '_calib',
             unumpy.nominal_values(mags),
-            image.filt+'_no-calib',
-            'mag-cali_mags_'+image.filt+'_img_'+str(image.pd),
+            image.filt + '_no-calib',
+            'mag-cali_mags_' + image.filt + '_img_' + str(image.pd),
             image.outpath.name,
-            ),
+        ),
         kwargs={
-            'nameobj':image.objname,
-            }
-        )
+            'nameobj': image.objname,
+        }
+    )
     p.start()
 
     #   Add sigma clipping plots based on the color
     if plot_sigma:
         cal_sigma_plot_color(
             f_list[id_f],
             image.outpath.name,
@@ -913,16 +912,16 @@
             f_list,
             id_1,
             id_2,
             unumpy.nominal_values(color_fit),
             unumpy.nominal_values(color_lit),
             unumpy.nominal_values(color_fit_clip),
             unumpy.nominal_values(color_lit_clip),
-            '_img_'+str(image.pd),
-            )
+            '_img_' + str(image.pd),
+        )
 
     return mag_cali
 
 
 def apply_trans_str(img_container, image, lit_m, id_f, id_i, id_1, id_2,
                     f_list, Tc, plot_sigma=False, ttype='derive'):
     '''
@@ -964,39 +963,39 @@
 
         ttype               : `string`, optional
             Type of magnitude transformation.
             Possibilities: simple, airmass, or derive
             Default is ``derive``.
     '''
     #   Get current filter
-    filt  = f_list[id_f]
+    filt = f_list[id_f]
 
     #   Get necessary magnitudes arrays
-    lit_mag        = lit_m['mag']
+    lit_mag = lit_m['mag']
     mag_cali_fit_1 = image.mag_fit_1['mag']
     mag_cali_fit_2 = image.mag_fit_2['mag']
-    mags_1         = image.mags_1['mag']
-    mags_2         = image.mags_2['mag']
-    mags           = image.mags['mag']
+    mags_1 = image.mags_1['mag']
+    mags_2 = image.mags_2['mag']
+    mags = image.mags['mag']
 
     #   Prepare calibration parameters
-    Tc_T1    = None
-    Tc_k1    = None
-    Tc_T2    = None
-    Tc_k2    = None
-    Tc_C     = None
+    Tc_T1 = None
+    Tc_k1 = None
+    Tc_T2 = None
+    Tc_k2 = None
+    Tc_C = None
     Tc_color = None
     if ttype == 'simple':
-        Tc_C     = Tc['C']
+        Tc_C = Tc['C']
         Tc_color = Tc['color']
     elif ttype == 'airmass':
-        Tc_T1    = Tc['T_1']
-        Tc_k1    = Tc['k_1']
-        Tc_T2    = Tc['T_2']
-        Tc_k2    = Tc['k_2']
+        Tc_T1 = Tc['T_1']
+        Tc_k1 = Tc['k_1']
+        Tc_T2 = Tc['T_2']
+        Tc_k2 = Tc['k_2']
 
     #   Apply magnitude transformation
     mag_cali = trans_core(
         image,
         lit_mag[id_1],
         lit_mag[id_2],
         mag_cali_fit_1,
@@ -1012,15 +1011,15 @@
         Tc_k2,
         id_f,
         id_1,
         id_2,
         f_list,
         plot_sigma=plot_sigma,
         ttype=ttype,
-        )
+    )
 
     img_container.cali['mag'][id_f][id_i] = mag_cali
 
     #   Calculate uncertainties
     img_container.cali['err'][id_f][id_i] = cal_err_T(
         image,
         lit_m,
@@ -1028,15 +1027,15 @@
         Tc,
         mag_cali,
         id_1,
         id_2,
         id_f,
         ttype=ttype,
         air_mass=image.air_mass,
-        )
+    )
 
 
 def apply_trans_unc(img_container, image, lit_m, id_f, id_i, id_1, id_2,
                     f_list, Tc, plot_sigma=False, ttype='derive'):
     '''
         Apply transformation
 
@@ -1076,36 +1075,36 @@
 
         ttype               : `string`, optional
             Type of magnitude transformation.
             Possibilities: simple, airmass, or derive
             Default is ``derive``.
     '''
     #   Get necessary magnitudes arrays
-    lit_mag        = lit_m
+    lit_mag = lit_m
     mag_cali_fit_1 = image.mag_fit_1
     mag_cali_fit_2 = image.mag_fit_2
-    mags_1         = image.mags_1
-    mags_2         = image.mags_2
-    mags           = image.mags
+    mags_1 = image.mags_1
+    mags_2 = image.mags_2
+    mags = image.mags
 
     #   Prepare calibration parameters
-    Tc_T1    = None
-    Tc_k1    = None
-    Tc_T2    = None
-    Tc_k2    = None
-    Tc_C     = None
+    Tc_T1 = None
+    Tc_k1 = None
+    Tc_T2 = None
+    Tc_k2 = None
+    Tc_C = None
     Tc_color = None
     if ttype == 'simple':
-        Tc_C     = ufloat(Tc['C'], Tc['C_err'])
+        Tc_C = ufloat(Tc['C'], Tc['C_err'])
         Tc_color = ufloat(Tc['color'], Tc['color_err'])
     elif ttype == 'airmass':
-        Tc_T1    = ufloat(Tc['T_1'], Tc['T_1_err'])
-        Tc_k1    = ufloat(Tc['k_1'], Tc['k_1_err'])
-        Tc_T2    = ufloat(Tc['T_2'], Tc['T_2_err'])
-        Tc_k2    = ufloat(Tc['k_2'], Tc['k_2_err'])
+        Tc_T1 = ufloat(Tc['T_1'], Tc['T_1_err'])
+        Tc_k1 = ufloat(Tc['k_1'], Tc['k_1_err'])
+        Tc_T2 = ufloat(Tc['T_2'], Tc['T_2_err'])
+        Tc_k2 = ufloat(Tc['k_2'], Tc['k_2_err'])
 
     #   Apply magnitude transformation
     mag_cali = trans_core(
         image,
         lit_mag[id_1],
         lit_mag[id_2],
         mag_cali_fit_1,
@@ -1121,15 +1120,15 @@
         Tc_k2,
         id_f,
         id_1,
         id_2,
         f_list,
         plot_sigma=plot_sigma,
         ttype=ttype,
-        )
+    )
 
     img_container.cali[id_f][id_i] = mag_cali
 
 
 def calibrate_simple(*args, **kwargs):
     '''
         Apply minimal calibration: No magnitude transformation & no other
@@ -1218,15 +1217,15 @@
 
     m_out['err'][id_f][id_img] = cal_err(
         mask,
         image.mags_fit['err'],
         lit_m['err'][id_f],
         image.mags['err'],
         m_out['std'][id_f][id_img],
-        )
+    )
 
     #   Write data back to the image container
     img_container.noT = m_out
     try:
         img_container.flux['flux'][id_f][id_img] = image.flux_es['flux_fit']
         img_container.flux['err'][id_f][id_img] = image.flux_es['flux_unc']
     except:
@@ -1263,15 +1262,15 @@
     mag_cali = calibrate_simple_core(image, mag_arr)
 
     #   Sigma clipping to rm outliers
     mag_cali_sigma = sigma_clipping(
         unumpy.nominal_values(mag_cali),
         sigma=1.5,
         axis=1,
-        )
+    )
     mask = np.invert(mag_cali_sigma.mask)
     mask = np.any(mask, axis=0)
 
     #   Calculate median etc ...
     median = np.median(mag_cali[:, mask], axis=1)
 
     #   Write data back to the image container
@@ -1326,30 +1325,30 @@
 
     #   Calculated sigma clipped magnitudes
     sigma_clipp_flux = sigma_clipped_stats(
         flux_values,
         axis=0,
         sigma=1.5,
         mask_value=0.0,
-        )
+    )
 
     #   Get median values
     median = sigma_clipp_flux[1]
     std = sigma_clipp_flux[2]
 
     #   Add axis so that broadcasting to original array is possible
-    median_reshape = median[np.newaxis,:]
-    std_reshape = std[np.newaxis,:]
+    median_reshape = median[np.newaxis, :]
+    std_reshape = std[np.newaxis, :]
 
     #   Normalized magnitudes
-    ensemble.uflux_norm = flux / unumpy.uarray(median_reshape,std_reshape)
+    ensemble.uflux_norm = flux / unumpy.uarray(median_reshape, std_reshape)
 
 
 def prepare_ZP(img_container, image, image_o, id_i, id_o=None):
-    '''
+    """
         Prepare some values necessary for the magnitude calibration and add
         them to the image class
 
         Parameters
         ----------
         img_container   : `image.container`
             Container object with image ensemble objects for each filter
@@ -1363,58 +1362,57 @@
         id_i                : `integer`
             ID of the filter
 
         id_o                : `integer`, optional
             ID of the `second` image/filter that is used for the magnitude
             transformation.
             Default is ``None``.
-    '''
+    """
     #   Get type of the magnitudes array used
     #   Possibilities: structured numpy array & unumpy uarray
     unc = getattr(img_container, 'unc', True)
 
     #   Set array with literature magnitudes for the calibration stars
-    mag_lit  = img_container.calib_parameters.mags_lit
+    mag_lit = img_container.calib_parameters.mags_lit
     if not unc:
         mag_lit = mag_lit['mag']
 
     #   Get extracted magnitudes
-    mag_fit_i  = image.mags_fit
+    mag_fit_i = image.mags_fit
     if not unc:
         mag_fit_i = mag_fit_i['mag']
 
     if id_o is not None:
-        mag_fit_o  = image_o.mags_fit
+        mag_fit_o = image_o.mags_fit
         if not unc:
             mag_fit_o = mag_fit_o['mag']
 
     #   Calculated color. For two filter calculate delta color
     if id_o is not None:
         del_col_calib = mag_fit_i + mag_fit_o - mag_lit[id_i] - mag_lit[id_o]
 
     else:
         del_col_calib = mag_fit_i - mag_lit[id_i]
 
-
     #   Calculate mask according to sigma clipping
     if unc:
         clip_values = unumpy.nominal_values(del_col_calib)
     else:
         clip_values = del_col_calib
     clip = sigma_clipping(clip_values, sigma=1.5)
     image.ZP_mask = np.invert(clip.recordmask)
 
     #   Plot sigma clipping if it makes sense
     if not np.all(mag_lit == 0.):
         #   Make fit
-        ZP_fit = aux.fit_data_oneD(
+        ZP_fit = aux.fit_data_one_d(
             mag_fit_i[image.ZP_mask],
             mag_lit[id_i][image.ZP_mask],
             1,
-            )
+        )
 
         #   Get plot variables
         if unc:
             mag_fit_i_plot = unumpy.nominal_values(mag_fit_i)
             mag_lit_plot = unumpy.nominal_values(mag_lit[id_i])
             m_fit_err_plot = unumpy.std_devs(mag_fit_i[image.ZP_mask])
             m_lit_err_plot = unumpy.std_devs(mag_lit[id_i][image.ZP_mask])
@@ -1427,29 +1425,29 @@
         cal_sigma_plot(
             mag_fit_i_plot,
             image.ZP_mask,
             image.filt,
             mag_lit_plot,
             image.outpath.name,
             image.objname,
-            '_img_'+str(image.pd),
+            '_img_' + str(image.pd),
             fit=ZP_fit,
             m_fit_err=m_fit_err_plot,
             m_lit_err=m_lit_err_plot,
-            )
+        )
 
     #   Calculate zero points and clip
-    image.ZP       = mag_lit[id_i] - mag_fit_i
-    image.ZP_clip  = image.ZP[image.ZP_mask]
+    image.ZP = mag_lit[id_i] - mag_fit_i
+    image.ZP_clip = image.ZP[image.ZP_mask]
 
 
 def apply_calib(img_container, filter_list, Tcs=None, derive_Tcs=False,
-                plot_sigma=False, plot_mags=True, ID='', photo_type='',
+                plot_sigma=False, plot_mags=True, id_object=None, photo_type='',
                 refid=0, indent=1):
-    '''
+    """
         Apply the calibration to the magnitudes and perform a magnitude
         transformation if possible
 
         # Using:
         # Δ(b-v) = (b-v)obj - (b-v)cali
         # Δ(B-V) = Tbv * Δ(b-v)
         # Vobj = Δv + Tv_bv * Δ(B-V) + Vcomp or Vobj
@@ -1479,17 +1477,17 @@
             Default is ``False``.
 
         plot_mags       : `boolean', optional
             If True a star map plot with the 100 faintest objects will be
             created.
             Default is ``True``.
 
-        ID              : `string`, optional
+        id_object       : `integer` or `None`, optional
             ID of the object
-            Default is ``''``.
+            Default is ``None``.
 
         photo_type      : `string`, optional
             Applied extraction method. Possibilities: ePSF or APER`
             Default is ``''``.
 
         refid           : `integer`, optional
             ID of the reference image
@@ -1499,32 +1497,32 @@
             Indentation for the console output lines
             Default is ``1``.
 
         Returns
         -------
         cali or noT     : `numpy.ndarray`
             Array with magnitudes and errors
-    '''
+    """
     terminal_output.print_terminal(
         indent=indent,
         string="Apply calibration and perform magnitude transformation",
-        )
+    )
 
     #   Get image ensembles
     img_ensembles = img_container.ensembles
 
     #   Get object indices and X & Y pixel positions
     try:
         ind = img_ensembles[filter_list[0]].id_es
-        x   = img_ensembles[filter_list[0]].x_es
-        y   = img_ensembles[filter_list[0]].y_es
+        x = img_ensembles[filter_list[0]].x_es
+        y = img_ensembles[filter_list[0]].y_es
     except:
         ind = img_ensembles[filter_list[0]].id_s
-        x   = img_ensembles[filter_list[0]].x_s
-        y   = img_ensembles[filter_list[0]].y_s
+        x = img_ensembles[filter_list[0]].x_s
+        y = img_ensembles[filter_list[0]].y_s
 
     #   Number of filter
     nfilter = len(filter_list)
 
     #   Get number of objects
     try:
         count = len(img_ensembles[filter_list[0]].id_es)
@@ -1535,15 +1533,15 @@
     aux.prepare_arrays(img_container, nfilter, count)
 
     #   Initialize bool and image ID for transformation
     id_tuple_trans = []
     id_tuple_notrans = []
 
     #   Get calibration magnitudes
-    lit_mags    = img_container.calib_parameters.mags_lit
+    lit_mags = img_container.calib_parameters.mags_lit
 
     for filt_i, band in enumerate(filter_list):
         #   Get image ensemble
         img_ensemble = img_ensembles[band]
 
         #   Get image list
         img_list = img_ensemble.image_list
@@ -1553,15 +1551,15 @@
             img_container,
             Tcs,
             filter_list,
             filt_i,
             0,
             id_tuple_notrans,
             derive_Tcs=derive_Tcs
-            )
+        )
 
         #   Loop over images
         for id_img_i, img_i in enumerate(img_list):
             #   Get extracted magnitudes of the calibration stars for the
             #   current image
             calib.get_calib_fit(img_i, img_container)
 
@@ -1571,29 +1569,28 @@
                     img_container,
                     id_img_i,
                     filt_o,
                     filt_i,
                     filt_id_1,
                     filter_list,
                     id_tuple_trans,
-                    )
+                )
             else:
                 img_o = None
 
             #   Prepare ZP for the magnitude calibration and perform
             #   sigma clipping on the delta color or color, depending on
             #   whether magnitude transformation is possible or not.
             prepare_ZP(
                 img_container,
                 img_i,
                 img_o,
                 filt_i,
                 id_o=filt_o,
-                )
-
+            )
 
             ###
             #   Calculate transformation if possible
             #
             if Tc_type is not None:
                 apply_trans(
                     img_container,
@@ -1603,89 +1600,101 @@
                     id_img_i,
                     filt_id_1,
                     filt_id_2,
                     filter_list,
                     Tc,
                     plot_sigma=plot_sigma,
                     ttype=Tc_type,
-                    )
-
+                )
 
             ###
             #   Calibration without transformation
             #
             calibrate_simple(img_container, img_i, lit_mags, filt_i, id_img_i)
 
-
             ####
             ##   Plot star map
             ##
-            #if plot_mags:
-                #if u == refid:
-                    #if trans_key[i]:
-                        #mags_plot = cali['med'][i][u]
-                    #else:
-                        #mags_plot = noT['med'][i][u]
-                    #prepare_and_plot_starmap(
-                        #img,
-                        #x,
-                        #y,
-                        #mags_plot,
-                        #ID,
-                        #band,
-                        #)
+            # if plot_mags:
+            # if u == refid:
+            # if trans_key[i]:
+            # mags_plot = cali['med'][i][u]
+            # else:
+            # mags_plot = noT['med'][i][u]
+            # prepare_and_plot_starmap(
+            # img,
+            # x,
+            # y,
+            # mags_plot,
+            # ID,
+            # band,
+            # )
 
         img_container.Tc_type = None
 
-
     ###
     #   Save results as ASCII files
     #
     cali = img_container.cali
     if not checks.check_unumpy_array(cali):
         cali = cali['mag']
 
+    #   If transformation is available
     if np.any(cali != 0.):
-        #   If transformation is available
+        #   Make astropy table
+        table_mags_transformed = aux.mk_mag_table(
+            ind,
+            x,
+            y,
+            img_container.cali,
+            filter_list,
+            id_tuple_trans,
+        )
+
+        #   Add table to container
+        img_container.table_mags_transformed = table_mags_transformed
+
+        #   Save to file
         aux.save_mags_ascii(
             img_container,
-            aux.mk_mag_table(
-                ind,
-                x,
-                y,
-                img_container.cali,
-                filter_list,
-                id_tuple_trans,
-                ),
+            table_mags_transformed,
             trans=True,
-            ID=ID,
+            id_object=id_object,
             photo_type=photo_type,
-            )
+        )
     else:
         terminal_output.print_terminal(
             indent=indent,
             string="WARNING: No magnitude transformation possible",
             style_name='WARNING'
-            )
+        )
 
     #   Without transformation
+
+    #   Make astropy table
+    table_mags_not_transformed = aux.mk_mag_table(
+        ind,
+        x,
+        y,
+        img_container.noT,
+        filter_list,
+        id_tuple_notrans,
+    )
+
+    #   Add table to container
+    img_container.table_mags_not_transformed = table_mags_not_transformed
+
+    #   Save to file
     aux.save_mags_ascii(
         img_container,
-        aux.mk_mag_table(
-            ind,
-            x,
-            y,
-            img_container.noT,
-            filter_list,
-            id_tuple_notrans,
-            ),
+        table_mags_not_transformed,
         trans=False,
-        ID=ID,
+        id_object=id_object,
         photo_type=photo_type,
-        )
+    )
 
 
 def deter_trans(img_container, key_filt, filter_list, tbl_trans,
                 fit_func=aux.lin_func, weights=True, indent=2):
     '''
         Determine the magnitude transformation factors
 
@@ -1745,44 +1754,43 @@
 
         #   Extract values from a structured Numpy array
         calib.get_calib_fit(img_1, img_container)
         calib.get_calib_fit(img_2, img_container)
         calib.get_calib_fit(img_key, img_container)
 
         if unc:
-            fit_mags_1   = img_1.mags_fit
-            fit_mags_2   = img_2.mags_fit
+            fit_mags_1 = img_1.mags_fit
+            fit_mags_2 = img_2.mags_fit
             fit_mags_key = img_key.mags_fit
         else:
-            fit_mags_1   = img_1.mags_fit['mag']
-            fit_mags_2   = img_2.mags_fit['mag']
+            fit_mags_1 = img_1.mags_fit['mag']
+            fit_mags_2 = img_2.mags_fit['mag']
             fit_mags_key = img_key.mags_fit['mag']
-            fit_err_1    = img_1.mags_fit['err']
-            fit_err_2    = img_2.mags_fit['err']
-            fit_err_key  = img_key.mags_fit['err']
+            fit_err_1 = img_1.mags_fit['err']
+            fit_err_2 = img_2.mags_fit['err']
+            fit_err_key = img_key.mags_fit['err']
 
         #   Calculate values
         if unc:
             lit_mags = mags_lit
         else:
             lit_mags = mags_lit['mag']
             lit_errs = mags_lit['err']
 
             color_lit_err = aux.err_prop(lit_errs[0], lit_errs[1])
             color_fit_err = aux.err_prop(fit_err_1, fit_err_2)
-            zero_err      = aux.err_prop(lit_errs[id_filt], fit_err_key)
+            zero_err = aux.err_prop(lit_errs[id_filt], fit_err_key)
 
         color_lit = lit_mags[0] - lit_mags[1]
         color_fit = fit_mags_1 - fit_mags_2
-        zero      = lit_mags[id_filt] - fit_mags_key
+        zero = lit_mags[id_filt] - fit_mags_key
 
         #   Initial guess for the parameters
-        #x0    = np.array([0.0, 0.0])
-        x0    = np.array([1.0, 1.0])
-
+        # x0    = np.array([0.0, 0.0])
+        x0 = np.array([1.0, 1.0])
 
         ###
         #   Determine transformation coefficients
         #
 
         #   Plot variables
         if unc:
@@ -1796,79 +1804,76 @@
             color_lit_plot = color_lit
             color_lit_err_plot = color_lit_err
             color_fit_plot = color_fit
             color_fit_err_plot = color_fit_err
             zero_plot = zero
             zero_err_plot = zero_err
 
-
         #   Color transform - Fit the data with fit_func
         #   Set sigma, using errors calculate above
         if weights:
             sigma = np.array(color_fit_err_plot)
         else:
             sigma = 0.
 
         #   Fit
         a, _, b, Tcolor_err = aux.fit_curve(
             fit_func,
             color_lit_plot,
             color_fit_plot,
             x0,
             sigma,
-            )
+        )
 
-        Tcolor = 1./b
+        Tcolor = 1. / b
 
         #   Plot color transform
         terminal_output.print_terminal(
             key_filt,
             indent=indent,
             string="Plot color transformation ({})",
-            )
+        )
         plot.plot_transform(
             ensemble_dict[filter_list[0]].outpath.name,
             filter_list[0],
             filter_list[1],
             color_lit_plot,
             color_fit_plot,
             a,
             b,
             Tcolor_err,
             fit_func,
             ensemble_dict[filter_list[0]].get_air_mass()[0],
             color_lit_err=color_lit_err_plot,
             fit_var_err=color_fit_err_plot,
             nameobj=ensemble_dict[filter_list[0]].objname,
-            )
-
+        )
 
         ##  Mag transform - Fit the data with fit_func
         #   Set sigma, using errors calculate above
         if weights:
             sigma = zero_err_plot
         else:
             sigma = 0.
 
-
         #   Fit
         Zdash, Zdash_err, Tmag, Tmag_err = aux.fit_curve(
             fit_func,
             color_lit_plot,
             zero_plot,
             x0,
             sigma,
-            )
+        )
 
         #   Plot mag transformation
         terminal_output.print_terminal(
             key_filt,
             indent=indent,
             string="Plot magnitude transformation ({})",
-            )
+        )
 
         plot.plot_transform(
             ensemble_dict[filter_list[0]].outpath.name,
             filter_list[0],
             filter_list[1],
             color_lit_plot,
             zero_plot,
@@ -1877,85 +1882,85 @@
             Tmag_err,
             fit_func,
             ensemble_dict[filter_list[0]].get_air_mass()[0],
             filt=key_filt,
             color_lit_err=color_lit_err_plot,
             fit_var_err=zero_err_plot,
             nameobj=ensemble_dict[filter_list[0]].objname,
-            )
+        )
 
         #   Redefine variables -> shorter variables
         key_filt_l = key_filt.lower()
         f_0_l = filter_list[0].lower()
         f_1_l = filter_list[1].lower()
-        f_0   = filter_list[0]
-        f_1   = filter_list[1]
+        f_0 = filter_list[0]
+        f_1 = filter_list[1]
 
         #   Fill calibration table
-        tbl_trans['C'+key_filt_l+f_0_l+f_1_l]            = [Tmag]
-        tbl_trans['C'+key_filt_l+f_0_l+f_1_l+'_err']     = [Tmag_err]
-        tbl_trans['Zdash'+key_filt_l+f_0_l+f_1_l]        = [Zdash]
-        tbl_trans['Zdash'+key_filt_l+f_0_l+f_1_l+'_err'] = [Zdash_err]
-        tbl_trans['T'+f_0_l+f_1_l]                       = [Tcolor]
-        tbl_trans['T'+f_0_l+f_1_l+'_err']                = [Tcolor_err]
+        tbl_trans['C' + key_filt_l + f_0_l + f_1_l] = [Tmag]
+        tbl_trans['C' + key_filt_l + f_0_l + f_1_l + '_err'] = [Tmag_err]
+        tbl_trans['Zdash' + key_filt_l + f_0_l + f_1_l] = [Zdash]
+        tbl_trans['Zdash' + key_filt_l + f_0_l + f_1_l + '_err'] = [Zdash_err]
+        tbl_trans['T' + f_0_l + f_1_l] = [Tcolor]
+        tbl_trans['T' + f_0_l + f_1_l + '_err'] = [Tcolor_err]
 
         #   Print results
         terminal_output.print_terminal(
             key_filt,
             indent=indent,
             string="Plot magnitude transformation ({})",
-            )
+        )
         terminal_output.print_terminal(
             indent=indent,
             string="###############################################",
-            )
+        )
         terminal_output.print_terminal(
             f_0_l,
             f_1_l,
             f_0,
             f_1,
             indent=indent,
             string="Colortransform ({}-{} vs. {}-{}):",
-            )
+        )
         terminal_output.print_terminal(
             f_0_l,
             f_1_l,
             Tcolor,
             Tcolor_err,
-            indent=indent+1,
+            indent=indent + 1,
             string="T{}{} = {:.5f} +/- {:.5f}",
-            )
+        )
         terminal_output.print_terminal(
             key_filt,
             key_filt,
             key_filt_l,
             f_0,
             f_1,
             indent=indent,
             string="{}-mag transform ({}-{} vs. {}-{}):",
-            )
+        )
         terminal_output.print_terminal(
             key_filt_l,
             f_0_l,
             f_1_l,
             Tmag,
             Tmag_err,
-            indent=indent+1,
+            indent=indent + 1,
             string="T{}_{}{} = {:.5f} +/- {:.5f}",
-            )
+        )
         terminal_output.print_terminal(
             indent=indent,
             string="###############################################",
-            )
+        )
 
 
 def calculate_trans(img_container, key_filt, filt_list, tbl_trans,
                     weights=True, dcr=3., option=1, calib_method='APASS',
-                    vizier_dict={'APASS':'II/336/apass9'}, calib_file=None,
-                    mag_range=(0.,18.5), rm_obj_coord=None, indent='      '):
+                    vizier_dict={'APASS': 'II/336/apass9'}, calib_file=None,
+                    mag_range=(0., 18.5), rm_obj_coord=None, indent='      '):
     '''
         Calculate the transformation coefficients
 
         Parameters
         ----------
         img_container       : `image.container`
             Container object with image ensemble objects for each filter
@@ -2011,48 +2016,45 @@
     #   Correlate the results from the different filter
     #
     analyze.correlate_ensemble(
         img_container,
         filt_list,
         dcr=dcr,
         option=option,
-        )
-
+    )
 
     ###
     #   Plot image with the final positions overlaid
     #   (final version)
     #
     aux.prepare_and_plot_starmap_final(
         img_container,
         filt_list,
-        )
-
+    )
 
     ###
     #   Calibrate transformation coefficients
     #
     calib.deter_calib(
         img_container,
         filt_list,
         calib_method=calib_method,
         dcr=dcr,
         option=option,
         vizier_dict=vizier_dict,
         calib_file=calib_file,
         mag_range=mag_range,
-        )
+    )
     terminal_output.print_terminal()
 
-
     ###
     #   Determine transformation coefficients
     #   & Plot calibration plots
     #
     deter_trans(
         img_container,
         key_filt,
         filt_list,
         tbl_trans,
         weights=weights,
-        )
+    )
     terminal_output.print_terminal()
```

### Comparing `ost_photometry-0.0.7/src/ost_photometry/reduce/aux.py` & `ost_photometry-0.0.8/src/ost_photometry/reduce/aux.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from scipy.ndimage import shift as shift_scipy
 
 from astropy.nddata import CCDData, StdDevUncertainty
 import astropy.units as u
 from astropy.stats import sigma_clipped_stats
 from astropy.table import Table
+from astropy.time import Time
 
 from photutils.detection import DAOStarFinder
 from photutils.psf import extract_stars
 
 from scipy.interpolate import UnivariateSpline
 
 import ccdproc as ccdp
@@ -121,14 +122,176 @@
 
     #   Get instruments (set() allows to return only unique values)
     instruments = set(ifc.summary['instrume'])
 
     return instruments
 
 
+def get_instrument_infos(ifc, temp_tolerence):
+    '''
+        Extract information regarding the instruments and readout mode.
+        Currently the instrument and readout mode need to be unique. An
+        exception will be raised in case multiple readout modes or
+        instruments are detected.
+        -> TODO: make vector with instruments and readout modes
+
+        Parameters
+        ----------
+        ifc             : `ccdproc.ImageFileCollection`
+            Image file collection with all images
+
+        temp_tolerence      : `float`, optional
+            The images are required to have the temperature. This value
+            specifies the temperature difference that is acceptable.
+
+        Returns
+        -------
+        instruments           : `set`
+            List of instruments
+
+        redout_mode           : `string`
+            Mode used to readout the data from the camera chip.
+
+        gain_setting          : `integer` or `None`
+            Gain used in the camera setting for cameras such as the QHYs.
+            This is not the system gain, but it can be calculated from this
+            value. See below.
+
+        bit_pix                 : `integer`
+            Bit value of each pixel
+
+        temperature             : `float`
+            Temperature of the images
+    '''
+    #   Except if no files are found
+    if not ifc.files:
+        raise RuntimeError(
+            f'{style.bcolors.FAIL}No images found -> EXIT\n'
+            f'\t=> Check paths to the images!{style.bcolors.ENDC}'
+            )
+
+    #   Get instruments (set() allows to return only unique values)
+    instruments = set(ifc.summary['instrume'])
+
+    if len(instruments) > 1:
+        raise RuntimeError(
+            f'{style.bcolors.FAIL}Multiple instruments detected.\n'
+            f'This is currently not supported -> EXIT \n{style.bcolors.ENDC}'
+            )
+        # terminal_output.print_terminal(
+        #     instruments,
+        #     string="Images are taken with several instruments: {}. "\
+        #         "The pipeline cannot account for that, but will try anyway...",
+        #     indent=2,
+        #     style_name='WARNING',
+        #     )
+
+    instrument = list(instruments)[0]
+
+    #   Get the instrument in case of QHY cameras
+    if instrument in ['QHYCCD-Cameras-Capture', 'QHYCCD-Cameras2-Capture']:
+        #   Get image dimensions and binning
+        xdims = set(ifc.summary['naxis1'])
+        if len(xdims) > 1:
+            raise RuntimeError(
+                f'{style.bcolors.FAIL}Multiple image dimensions detected.\n'
+                f'This is not supported -> EXIT \n{style.bcolors.ENDC}'
+                )
+        xdim = list(xdims)[0]
+
+        ydims = set(ifc.summary['naxis2'])
+        if len(ydims) > 1:
+            raise RuntimeError(
+                f'{style.bcolors.FAIL}Multiple image dimensions detected.\n'
+                f'This is not supported -> EXIT \n{style.bcolors.ENDC}'
+                )
+        ydim = list(ydims)[0]
+
+        xbins = set(ifc.summary['xbinning'])
+        if len(xbins) > 1:
+            raise RuntimeError(
+                f'{style.bcolors.FAIL}Multiple binning values detected.\n'
+                f'This is not supported -> EXIT \n{style.bcolors.ENDC}'
+                )
+        xbin = list(xbins)[0]
+
+        ybins = set(ifc.summary['ybinning'])
+        if len(ybins) > 1:
+            raise RuntimeError(
+                f'{style.bcolors.FAIL}Multiple binning values detected.\n'
+                f'This is not supported -> EXIT \n{style.bcolors.ENDC}'
+                )
+        ybin = list(ybins)[0]
+
+        #   Physical chip dimensions in pixel
+        xdim_phy = xdim * xbin
+        ydim_phy = ydim * ybin
+
+        #   Set instrument
+        if xdim_phy == 9576 and ydim_phy == 6388:
+            instrument = 'QHY600M'
+        elif xdim_phy == 6280 and ydim_phy == 4210:
+            instrument = 'QHY268M'
+        elif xdim_phy == 3864 and ydim_phy == 2180:
+            instrument = 'QHY485C'
+        else:
+            instrument = ''
+
+
+    #   Get readout mode
+    redout_modes = set(ifc.summary['readoutm'])
+    if not redout_modes:
+        redout_mode = 'Extend Fullwell 2CMS'
+    elif len(redout_modes) == 1:
+        redout_mode = list(redout_modes)[0]
+
+        if redout_mode in ['Fast', 'Slow']:
+            redout_mode = 'Extend Fullwell 2CMS'
+    else:
+        raise RuntimeError(
+            f'{style.bcolors.FAIL}Multiple readout modes detected.\n'
+            f'This is currently not supported -> EXIT \n{style.bcolors.ENDC}'
+            )
+
+
+    #   Get gain setting
+    gain_settings = set(ifc.summary['gain'])
+    if len(gain_settings) > 1:
+        raise RuntimeError(
+            f'{style.bcolors.FAIL}Multiple gain values detected.\n'
+            f'This is not supported -> EXIT \n{style.bcolors.ENDC}'
+            )
+    gain_setting = list(gain_settings)[0]
+
+
+    #   Get bit setting
+    bit_pixs = set(ifc.summary['bitpix'])
+    if len(bit_pixs) > 1:
+        raise RuntimeError(
+            f'{style.bcolors.FAIL}Multiple bit values detected.\n'
+            f'This is not supported -> EXIT \n{style.bcolors.ENDC}'
+            )
+    bit_pix = list(bit_pixs)[0]
+
+
+    #   Get image temperature
+    temperatures = set(ifc.summary['ccd-temp'])
+    temp_list = list(temperatures)
+    temp_range = max(temp_list) - min(temp_list)
+    if temp_range > temp_tolerence:
+        raise RuntimeError(
+            f'{style.bcolors.FAIL}Significant difference detected between '
+            f'the images: {temp_range}\n'
+            f'This is not supported -> EXIT \n{style.bcolors.ENDC}'
+            )
+    temperature = np.median(temp_list)
+
+    return instrument, redout_mode, gain_setting, bit_pix, temperature
+
+
 def get_imaging_soft(ifc):
     '''
         Extract imaging software version.
 
         Parameters
         ----------
         ifc             : `ccdproc.ImageFileCollection`
@@ -605,15 +768,15 @@
             Default is ``None``.
 
         verbose         : `boolean`, optional
             If True additional output will be printed to the command line.
             Default is ``False``.
     '''
     #   Sanitize the provided paths
-    out_path  = checks.check_pathlib_Path(outdir)
+    out_path  = checks.check_pathlib_path(outdir)
 
     #   Get exposure time
     exposure   = dark.header['EXPTIME']
 
     #   Get image shape
     shape1 = dark.meta['naxis1']
     shape2 = dark.meta['naxis2']
@@ -666,15 +829,15 @@
             Path to the directory where the master files should be saved to
 
         verbose         : `boolean`, optional
             If True additional output will be printed to the command line.
             Default is ``False``.
     '''
     #   Sanitize the provided paths
-    out_path  = checks.check_pathlib_Path(outdir)
+    out_path  = checks.check_pathlib_path(outdir)
 
     #   Get information on the image dimensions/binning
     shape_list = []
     for bpm in mask_list:
         shape_list.append(bpm.shape)
     shape_list = set(shape_list)
 
@@ -1595,16 +1758,16 @@
             Default is ``False``.
 
         indent          : `string`
             Indentation for the console output lines.
             Default is ``      ``.
     '''
     #   Sanitize the provided paths
-    file_path = checks.check_pathlib_Path(path)
-    out_path  = checks.check_pathlib_Path(outdir)
+    file_path = checks.check_pathlib_path(path)
+    out_path  = checks.check_pathlib_path(outdir)
 
     #   New image collection for the images
     ifc = ccdp.ImageFileCollection(file_path)
 
     #   Determine filter
     filters = set(h['filter'] for h in ifc.headers(imagetyp=image_type))
 
@@ -1745,15 +1908,15 @@
 
         Returns
         -------
         check_master    : 'boolean`
             Is True if all required master files are already prepared.
     '''
     #   Sanitize the provided paths
-    file_path = checks.check_pathlib_Path(path)
+    file_path = checks.check_pathlib_path(path)
 
     #   Get image collection for the reduced files
     ifc_reduced = ccdp.ImageFileCollection(file_path)
 
     if not ifc_reduced.files:
         return False
 
@@ -2026,15 +2189,15 @@
         w                   : `astropy.wcs.WCS`
             WCS information
     '''
     ###
     #   Prepare variables
     #
     #   Check directories
-    file_path = checks.check_pathlib_Path(input_dir)
+    file_path = checks.check_pathlib_path(input_dir)
     checks.check_out(output_dir)
 
     #   Set up image collection for the images
     ifc = ccdp.ImageFileCollection(file_path)
 
     #   Filter priority list:
     #   Give highest priority to the filter with the highest probability of
@@ -2073,32 +2236,40 @@
     cal_wcs = base_aux.check_wcs_exists(reff_img)
 
 
     ###
     #   Determine WCS
     #
     if not cal_wcs or force_wcs_determ:
-        w = find_wcs_distinguish(reff_img, method=method, indent=indent)
+        w = find_wcs_distinguish(
+            reff_img,
+            method=method,
+            x=x,
+            y=y,
+            indent=indent,
+            )
 
         ###
         #   Add WCS to images
         #
         if w is not None:
             for img, file_name in ifc.ccds(return_fname=True):
 
                 img.wcs = w
 
                 #   Save the image
                 img.write(output_dir / file_name, overwrite=True)
 
 
 def find_wcs_all_imgs(input_dir, output_dir, force_wcs_determ=False,
-                      method='astrometry', x=None, y=None, indent=2):
+                      method='astrometry', x=None, y=None, combined=False,
+                      img_type=None, indent=2):
     '''
-        Determine the WCS of each image individually.
+        Determine the WCS of each image individually. Images can be filtered
+        based on image type and the 'combined' keyword.
 
         Parameters
         ----------
         input_dir           : `pathlib.Path` or string
             Path to the input directory.
 
         output_dir          : `pathlib.Path` or string
@@ -2114,28 +2285,43 @@
             Options: 'astrometry', 'astap', or 'twirl'
             Default is ``astrometry``.
 
         x, y                : `numpy.ndarray`, optional
             Pixel coordinates of the objects
             Default is ``None``.
 
+        combined            : `boolean`, optional
+            Filter for images that have a 'combined' fits header keyword.
+            Default is ``False``.
+
+        img_type        : `string` or `None`, optional
+            Image type to select. Possibilities: bias, dark, flat, light
+            Default is ``None``.
+
         indent              : `integer`, optional
             Indentation for the console output lines
             Default is ``2``.
     '''
     ###
     #   Prepare variables
     #
     #   Check directories
-    file_path = checks.check_pathlib_Path(input_dir)
+    file_path = checks.check_pathlib_path(input_dir)
     checks.check_out(output_dir)
 
     #   Set up image collection for the images
+    #   and filter according to requirements
     ifc = ccdp.ImageFileCollection(file_path)
 
+    if img_type is not None:
+        true_img_type = get_image_type(ifc, img_type)
+        ifc = ifc.filter(imagetyp=true_img_type)
+
+    if combined:
+        ifc = ifc.filter(combined=combined)
 
     ###
     #   Derive WCS
     #
     for i, (img_ccd, file_name) in enumerate(ifc.ccds(return_fname=True)):
         #   Prepare image object
         img = base_aux.image(
@@ -2147,15 +2333,21 @@
             )
         base_aux.cal_fov(img, verbose=False)
 
         #   Test if the image contains already a WCS
         cal_wcs = base_aux.check_wcs_exists(img)
 
         if not cal_wcs or force_wcs_determ:
-            w = find_wcs_distinguish(img, method=method, indent=indent)
+            w = find_wcs_distinguish(
+                img,
+                method=method,
+                x=x,
+                y=y,
+                indent=indent,
+                )
 
             #   Add WCS to image (not necessary for ASTAP method)
             if method in ['astrometry', 'twirl']:
                 img_ccd.wcs = w
 
                 #   Save the image
                 img_ccd.write(output_dir / file_name, overwrite=True)
@@ -2243,7 +2435,99 @@
         raise RuntimeError(
             f"{style.bcolors.FAIL} \nException in find_wcs(): '"
             f"\nWCS method not known -> Supplied method was {method}"
             f"{style.bcolors.ENDC}"
             )
 
     return w
+
+
+def update_header_information(img, nimg=1, new_target_name=None):
+    '''
+        Updates Header information. Adds among other Header keywords required
+        for the GRANDMA project.
+
+        Parameters
+        ----------
+        img                 : `image.class`
+            Image class with all image specific properties
+
+        nimg                : `integer`, optional
+            Number of stacked images
+            Default is ``1``.
+
+        new_target_name : str or None, optional
+            Name of the target. If not None, this target name will be written
+            to the FITS header.
+            Default is ``None``.
+    '''
+    #   Add Header keyword to mark the file as stacked
+    if nimg > 1:
+        img.meta['COMBINED'] = True
+        img.meta['N-IMAGES'] = nimg
+        img.meta['EXPTIME']  = nimg * img.meta['EXPTIME']
+
+        #  GRANDMA
+        img.meta['STACK'] = 1
+
+    #  GRANDMA
+    img.meta['EXPOSURE'] = img.meta['EXPTIME']
+
+    #   Add MJD of start and center of the observation
+    try:
+        jd = img.meta['JD']
+        mjd = jd - 2400000.5
+        img.meta['MJD_STA'] = mjd
+
+        mjd_mid = mjd + img.meta['EXPTIME'] / 172800
+        img.meta['MJD_MID'] = mjd_mid
+
+        img.meta['DATE-MID'] = Time(mjd_mid, format='mjd').fits
+
+    except Exception as e:
+        terminal_output.print_terminal(
+            # indent=indent,
+            string=f"MJD could not be added to the header:\n {e}",
+            style_name='WARNING',
+            )
+
+    #   Add observation date using a second keyword (GRANDMA)
+    try:
+        obs_date = img.meta['DATE-OBS']
+        img.meta['OBSDATE'] = obs_date
+
+    except Exception as e:
+        terminal_output.print_terminal(
+            # indent=indent,
+            string=f"OBSDATE could not be added to the header:\n {e}",
+            style_name='WARNING',
+            )
+
+    #   Add gain using a second keyword (GRANDMA)
+    gain = img.meta['EGAIN']
+    img.meta['GAIN'] = gain
+
+    #   Add target name using a second keyword
+    if new_target_name is not None:
+        img.meta['OBJECT'] = new_target_name
+        #   GRANDMA
+        img.meta['TARGET'] = new_target_name
+    else:
+        #   GRANDMA
+        target = img.meta['OBJECT']
+        img.meta['TARGET'] = target
+
+    #   Username and instrument string (GRANDMA)
+    img.meta['USERNAME'] = 'OST'
+    img.meta['INSTRU'] = 'CDK'
+
+    #   Add filter system to the Header
+    filt = img.meta['FILTER']
+    try:
+        filter_system = calibration_data.filter_sytems[filt]
+        img.meta['FILTER-S'] = filter_system
+    except Exception as e:
+        terminal_output.print_terminal(
+            # indent=indent,
+            string=f"Filter system could not be determined:\n {e}",
+            style_name='WARNING',
+            )
```

### Comparing `ost_photometry-0.0.7/src/ost_photometry/reduce/plot.py` & `ost_photometry-0.0.8/src/ost_photometry/reduce/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ############################################################################
 ####                            Libraries                               ####
 ############################################################################
 
 import numpy as np
 
 from scipy import stats
+import scipy.interpolate as interpolate
 
 from matplotlib import pyplot as plt
 
 from astropy.visualization import hist, simple_norm
 
 from .. import checks
 
@@ -116,23 +117,16 @@
         align='mid',
         density=True,
         label="Dark frame",
         )
 
     bins = h[1]
 
-    #   Dark rate is dictionary of different values for different
-    #   temperatures
-    #   Get value for the entry closes to the exposure time
-    dr_temp = list(dark_rate.keys())
-    delta_temp = np.array(dr_temp) - exposure
-    id_min = np.argmin(delta_temp)
-
     #   Expected mean of the dark
-    expected_mean_dark = list(dark_rate.values())[id_min] * exposure / gain
+    expected_mean_dark = dark_rate * exposure / gain
 
     #   Plot Poisson
     if show_poisson:
         #   Account for number of exposures
         pois = stats.poisson(expected_mean_dark * n_images)
 
         #   X range
```

### Comparing `ost_photometry-0.0.7/src/ost_photometry/reduce/redu.py` & `ost_photometry-0.0.8/src/ost_photometry/reduce/redu.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,18 @@
 
 def reduce_main(path, outdir, img_type=None, gain=None, readnoise=None,
                 dr=None, cosmics=True, mask_cosmics=False, satlevel=None,
                 objlim=5., sigclip=4.0, scale_expo=True, ref_img=0,
                 bias_enforce=False, verbose=False, addmask=True,
                 shift_method='skimage', stack=True, estimate_fwhm=False,
                 shift_all=False, tolerance=0.5, stack_method='average',
-                target=None, find_wcs=True, wcs_method='astrometry',
-                wcs_all=False, force_wcs_determ=False, rm_outliers_shift=True,
-                filter_window_shift=8, threshold_shift=10., debug=False):
+                dtype_stack=None, target=None, find_wcs=True,
+                wcs_method='astrometry', wcs_all=False, force_wcs_determ=False,
+                rm_outliers_shift=True, filter_window_shift=8,
+                threshold_shift=10., temp_tolerence=5, debug=False):
     '''
         Main reduction routine: Creates master images for bias, darks,
                                 flats, reduces the science images and trims
                                 them to the same filed of view.
 
 
         Reduce the science images
@@ -67,17 +68,16 @@
             will be extracted from the FITS header.
             Default is ``None``.
 
         readnoise           : `float`, optional
             The read noise (e-) of the camera chip.
             Default is ``None``.
 
-        dr                  : `dictionary(float:float)`, optional
-            Temperature dependent dark rate in e-/pix/s:
-            key = temperature, value = dark rate
+        dr                  : `float`, optional
+            Dark rate in e-/pix/s:
             Default is ``None``.
 
         cosmics             : `boolean`, optional
             If True cosmics rays will be removed.
             Default is ``True``.
 
         mask_cosmics        : `boolean`, optional
@@ -154,14 +154,18 @@
             Default is ``0.5``s.
 
         stack_method        : `string`, optional
             Method used for combining the images.
             Possibilities: ``median`` or ``average`` or ``sum``
             Default is ``average`.
 
+        dtype_stack         : str or numpy.dtype, optional
+            dtype that should be used while combining the images.
+            Default is ''None'' -> None is equivalent to float64
+
         target              : `string` or ``None``, optional
             Name of the target. Used for file selection.
             Default is ``None``.
 
         find_wcs            : `boolean`, optional
             If `True` the WCS will be determined for the images.
             Default is ``True``.
@@ -190,14 +194,18 @@
             Default is ``8``.
 
         threshold_shift     : `float` or `integer`, optional
             Difference above the running median above an element is
             considered to be an outlier.
             Default is ``10.``.
 
+        temp_tolerence      : `float`, optional
+            The images are required to have the temperature. This value
+            specifies the temperature difference that is acceptable.
+
         debug               : `boolean`, optional
             If `True` the intermediate files of the data reduction will not
             be removed.
             Default is ``False``.
     '''
 
     ###
@@ -267,40 +275,38 @@
         dark_times,
         bias_true,
         tolerance=tolerance,
         )
 
 
     ###
-    #   Check instrument
-    #
-    instruments = aux.get_instruments(ifc)
-    if len(instruments) > 1:
-        terminal_output.print_terminal(
-            instruments,
-            string="Images are taken with several instruments: {}. "\
-                "The pipeline cannot account for that, but will try anyway...",
-            indent=2,
-            style_name='WARNING',
-            )
-
-
-    ###
     #   Get camera specific parameters
     #
+    img_parameters = aux.get_instrument_infos(ifc, temp_tolerence)
+    instrument = img_parameters[0]
+    redout_mode = img_parameters[1]
+    gain_setting = img_parameters[2]
+    bit_pix = img_parameters[3]
+    temperature = img_parameters[4]
+
     if (readnoise is None or gain is None or dr is None or satlevel is None):
-        camera_info = calibration_data.camera_info(list(instruments)[0])
+        camera_info = calibration_data.camera_info(
+            instrument,
+            redout_mode,
+            temperature,
+            gain_setting=gain_setting,
+            )
         if readnoise == None:
             readnoise = camera_info[0]
         if gain == None:
             gain = camera_info[1]
         if dr == None:
             dr = camera_info[2]
         if satlevel == None:
-            satlevel = camera_info[3]
+            satlevel = pow(2, bit_pix) - 1
 
 
     ###
     #   Check master files on disk
     #
     #   Get all filter
     filters = set(
@@ -467,34 +473,25 @@
             rm_outliers=rm_outliers_shift,
             filter_window=filter_window_shift,
             threshold=threshold_shift,
             verbose=verbose,
             debug=debug,
             )
 
-    if find_wcs:
+    if find_wcs and wcs_all:
         ###
-        #   Determine WCS and add it to all images
+        #   Determine WCS and add it to all reduced images
         #
         terminal_output.print_terminal(string="Determine WCS ...", indent=1)
-        if wcs_all:
-            aux.find_wcs_all_imgs(
-                out_path / 'cut',
-                out_path / 'cut',
-                method=wcs_method,
-                force_wcs_determ=force_wcs_determ,
-                )
-        else:
-            aux.find_wcs(
-                out_path / 'cut',
-                out_path / 'cut',
-                ref_id=ref_img,
-                method=wcs_method,
-                force_wcs_determ=force_wcs_determ,
-                )
+        aux.find_wcs_all_imgs(
+            out_path / 'cut',
+            out_path / 'cut',
+            method=wcs_method,
+            force_wcs_determ=force_wcs_determ,
+            )
 
     if estimate_fwhm:
         ###
         #   Estimate FWHM
         #
         terminal_output.print_terminal(string="Estimate FWHM ...", indent=1)
         aux.estimate_fwhm(
@@ -512,17 +509,33 @@
             indent=1,
             )
         stack_img(
             out_path / 'cut',
             out_path,
             img_type['light'],
             method=stack_method,
+            dtype=dtype_stack,
             debug=debug,
         )
 
+        if find_wcs and not wcs_all:
+            ###
+            #   Determine WCS and add it to the stacked images
+            #
+            terminal_output.print_terminal(string="Determine WCS ...", indent=1)
+
+            aux.find_wcs_all_imgs(
+                out_path,
+                out_path,
+                force_wcs_determ=force_wcs_determ,
+                method=wcs_method,
+                combined=True,
+                img_type=img_type['light'],
+                )
+
         if not shift_all:
             if shift_method == 'aa_true':
                 ###
                 #   Trim stacked images using astroalign
                 #
                 shift_stack_aa(out_path, out_path, img_type['light'])
 
@@ -574,15 +587,15 @@
                 ]
             )
         for filt in filters:
             #   Remove old files in the output directory
             checks.clear_directory(out_path / filt)
 
             #   Set path to files
-            file_path = checks.check_pathlib_Path(out_path / 'cut')
+            file_path = checks.check_pathlib_path(out_path / 'cut')
 
             #   New image collection for the images
             ifc = ccdp.ImageFileCollection(file_path)
 
             #   Restrict to current filter
             filt_files = ifc.files_filtered(filter=filt, include_path=True)
 
@@ -604,16 +617,16 @@
             Path to the directory where the master files should be saved to
 
         img_type        : `dictionary`
             Image types of the images. Possibilities: bias, dark, flat,
             light
     '''
     #   Sanitize the provided paths
-    file_path = checks.check_pathlib_Path(path)
-    out_path  = checks.check_pathlib_Path(outdir)
+    file_path = checks.check_pathlib_path(path)
+    out_path  = checks.check_pathlib_path(outdir)
 
     #   Create image collection
     ifc = ccdp.ImageFileCollection(file_path)
 
     #   Return if image collection is empty
     if not ifc.files:
         return
@@ -680,16 +693,16 @@
             Default is ``None``.
 
         readnoise       : `float`, optional
             The read noise (e-) of the camera chip.
             Default is ``8`` e-.
     '''
     #   Sanitize the provided paths
-    file_path = checks.check_pathlib_Path(path)
-    out_path  = checks.check_pathlib_Path(outdir)
+    file_path = checks.check_pathlib_path(path)
+    out_path  = checks.check_pathlib_path(outdir)
 
     #   Create image collection for the flats
     ifc = ccdp.ImageFileCollection(file_path)
 
     #   Create image collection for the reduced data
     ifc_reduced = ccdp.ImageFileCollection(out_path)
 
@@ -786,16 +799,16 @@
 
         debug           : `boolean`, optional
             If `True` the intermediate files of the data reduction will not
             be removed.
             Default is ``False``.
     '''
     #   Sanitize the provided paths
-    file_path = checks.check_pathlib_Path(path)
-    out_path  = checks.check_pathlib_Path(outdir)
+    file_path = checks.check_pathlib_path(path)
+    out_path  = checks.check_pathlib_path(outdir)
 
     #   Create image collection
     try:
         ifc = ccdp.ImageFileCollection(out_path / 'dark')
     except:
         ifc = ccdp.ImageFileCollection(file_path)
 
@@ -832,17 +845,14 @@
     #   Return if no darks are found in this directory
     if not dark_mask:
         return
 
     #   Get exposure times (set allows to return only unique values)
     dark_times = set(ifc.summary['exptime'][dark_mask])
 
-    #   Larges exposure time
-    max_expo = np.max(dark_times)
-
     #   Loop over exposure times
     dark_type = aux.get_image_type(ifc, image_type, image_class='dark')
     for exp_time in sorted(dark_times):
         #   Get only the darks with the correct exposure time
         calibrated_darks = ifc.files_filtered(
             imagetyp=dark_type,
             exptime=exp_time,
@@ -939,16 +949,16 @@
         tolerance           : `float` or `None`, optional
             Maximum difference, in seconds, between the image and the
             closest entry from the exposure time list. Set to ``None`` to
             skip the tolerance test.
             Default is ``0.5``.
     '''
     #   Sanitize the provided paths
-    file_path = checks.check_pathlib_Path(path)
-    out_path  = checks.check_pathlib_Path(outdir)
+    file_path = checks.check_pathlib_path(path)
+    out_path  = checks.check_pathlib_path(outdir)
 
     #   Create image collection for the flats
     ifc_flats = ccdp.ImageFileCollection(file_path)
 
     #   Return if image collection is empty
     if not ifc_flats.files:
         return
@@ -1087,16 +1097,16 @@
 
         debug           : `boolean`, optional
             If `True` the intermediate files of the data reduction will not
             be removed.
             Default is ``False``.
     '''
     #   Sanitize the provided paths
-    file_path = checks.check_pathlib_Path(path)
-    out_path  = checks.check_pathlib_Path(outdir)
+    file_path = checks.check_pathlib_path(path)
+    out_path  = checks.check_pathlib_path(outdir)
 
     #   Create new image collection for the reduced flat images
     ifc_flats = ccdp.ImageFileCollection(file_path)
 
     #   Determine filter
     flat_type = aux.get_image_type(
         ifc_flats,
@@ -1264,16 +1274,16 @@
             Default is ``0.5``s.
 
         target          : `string` or ``None``, optional
             Name of the target. Used for file selection.
             Default is ``None``.
     '''
     #   Sanitize the provided paths
-    file_path = checks.check_pathlib_Path(path)
-    out_path  = checks.check_pathlib_Path(outdir)
+    file_path = checks.check_pathlib_path(path)
+    out_path  = checks.check_pathlib_path(outdir)
 
     #   Get image collection for the science images
     ifc_lights = ccdp.ImageFileCollection(file_path)
 
     #   Return if image collection is empty
     if not ifc_lights.files:
         return
@@ -1800,16 +1810,16 @@
 
         debug               : `boolean`, optional
             If `True` the intermediate files of the data reduction will not
             be removed.
             Default is ``False``.
     '''
     #   Sanitize the provided paths
-    file_path = checks.check_pathlib_Path(path)
-    out_path  = checks.check_pathlib_Path(outdir)
+    file_path = checks.check_pathlib_path(path)
+    out_path  = checks.check_pathlib_path(outdir)
 
     #   New image collection for the images
     ifc = ccdp.ImageFileCollection(file_path)
 
     #   Check if ifc is not empty
     if not ifc.files:
         raise RuntimeError(
@@ -1903,16 +1913,16 @@
 
         debug               : `boolean`, optional
             If `True` the intermediate files of the data reduction will not
             be removed.
             Default is ``False``.
     '''
     #   Sanitize the provided paths
-    file_path = checks.check_pathlib_Path(path)
-    out_path  = checks.check_pathlib_Path(outdir)
+    file_path = checks.check_pathlib_path(path)
+    out_path  = checks.check_pathlib_path(outdir)
 
     #   New image collection for the images
     ifc = ccdp.ImageFileCollection(file_path)
 
     #   Check if ifc is not empty
     if not ifc.files:
         raise RuntimeError(
@@ -2021,28 +2031,33 @@
 
             #   Build new CCDData object
             img_out = CCDData(
                 img_data,
                 mask=footprint,
                 meta=img_ccd.meta,
                 unit=img_ccd.unit,
+                wcs=img_ccd.wcs,
                 uncertainty=StdDevUncertainty(img_uncert),
                 )
 
         #   Get filter
         filt = img_out.meta['filter']
 
+        img_out.meta['trimmed'] = True
+        img_out.meta.remove('combined')
+
         #   Define name and write trimmed image to disk
         file_name = 'combined_trimmed_filter_{}.fit'.format(
             filt.replace("''", "p")
             )
         img_out.write(outdir / file_name, overwrite=True)
 
 
-def stack_img(path, outdir, image_type, method='average', debug=False):
+def stack_img(path, outdir, image_type, method='average', dtype=None,
+              new_target_name=None, debug=False):
     '''
         Combine images
 
         Parameters
         ----------
         path            : `string`
             Path to the images
@@ -2055,22 +2070,31 @@
             shifts shall be determined
 
         method          : `string`, optional
             Method used for combining the images.
             Possibilities: ``median`` or ``average`` or ``sum``
             Default is ``average`.
 
+        dtype           : str or numpy.dtype, optional
+            dtype that should be used while combining the images.
+            Default is ''None'' -> None is equivalent to float64
+
+        new_target_name : str or None, optional
+            Name of the target. If not None, this target name will be written
+            to the FITS header.
+            Default is ``None``.
+
         debug           : `boolean`, optional
             If `True` the intermediate files of the data reduction will not
             be removed.
             Default is ``False``.
     '''
     #   Sanitize the provided paths
-    file_path = checks.check_pathlib_Path(path)
-    out_path  = checks.check_pathlib_Path(outdir)
+    file_path = checks.check_pathlib_path(path)
+    out_path  = checks.check_pathlib_path(outdir)
 
     #   New image collection for the images
     ifc = ccdp.ImageFileCollection(file_path)
 
     #   Check if ifc is not empty
     if not ifc.files:
         raise RuntimeError(
@@ -2098,30 +2122,31 @@
             method=method,
             sigma_clip=True,
             sigma_clip_low_thresh=5,
             sigma_clip_high_thresh=5,
             sigma_clip_func=np.ma.median,
             signma_clip_dev_func=mad_std,
             mem_limit=15e9,
+            dtype=dtype,
             )
 
-        #   Add Header keyword to mark the file as combined
-        combined_img.meta['COMBINED'] = True
-        nimg                          = len(to_combine)
-        combined_img.meta['N-IMAGES'] = nimg
-        combined_img.meta['EXPTIME']  = nimg * combined_img.meta['EXPTIME']
-        combined_img.meta['EXPOSURE'] = combined_img.meta['EXPTIME']
+        #   Update Header keywords
+        aux.update_header_information(
+            combined_img,
+            len(to_combine),
+            new_target_name,
+            )
 
         #   Define name and write file to disk
         file_name = 'combined_filter_{}.fit'.format(
             filt.replace("''", "p")
             )
         combined_img.write(out_path / file_name, overwrite=True)
 
-    #   Remove reduced dark files if they exist
+    #   Remove individual reduced images
     if not debug:
         shutil.rmtree(file_path, ignore_errors=True)
 
 
 def make_big(path, outdir, image_type, combined=True):
     '''
         Image size unification:
@@ -2142,16 +2167,16 @@
         combined        : `boolean`, optional
             It true the file selection will be restricted to images with a
             header keyword 'combined' that is set to True.
             Default is ``True``.
 
     '''
     #   Sanitize the provided paths
-    file_path = checks.check_pathlib_Path(path)
-    out_path  = checks.check_pathlib_Path(outdir)
+    file_path = checks.check_pathlib_path(path)
+    out_path  = checks.check_pathlib_path(outdir)
 
     #   New image collection for the images
     ifc = ccdp.ImageFileCollection(file_path)
 
     #   Image list
     img_type = aux.get_image_type(ifc, image_type)
     img_dict = {file_name: ccd for ccd, file_name in ifc.ccds(
@@ -2265,16 +2290,16 @@
             Default is ``10.``.
 
         verbose             : `boolean`, optional
             If True additional output will be printed to the command line.
             Default is ``False``.
     '''
     #   Sanitize the provided paths
-    file_path = checks.check_pathlib_Path(path)
-    out_path  = checks.check_pathlib_Path(outdir)
+    file_path = checks.check_pathlib_path(path)
+    out_path  = checks.check_pathlib_path(outdir)
 
     #   New image collection for the images
     ifc = ccdp.ImageFileCollection(file_path)
 
     #   Restrict image collection to those images correct image type and
     #   the 'enlarged' Header keyword
     img_type = aux.get_image_type(ifc, image_type)
```

### Comparing `ost_photometry-0.0.7/LICENSE` & `ost_photometry-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.7/pyproject.toml` & `ost_photometry-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ost_photometry"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Rainer Hainich", email="rhainich@astro.physik.uni-potsdam.de" },
 ]
 description = "Phtometry reduction and analysis package for the OST observatory"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
@@ -22,15 +22,15 @@
     "astropy>=5.0",
     "pytimedinput>=2.0",
     "pathlib>=1.0",
     "ccdproc>=2.3",
     "astroalign>=2.4",
     "scipy",
     "matplotlib>=3.5",
-    "photutils>=1.5",
+    "photutils>=1.8",
     "scikit-image",
     "uncertainties>=3.1",
     "astroquery>=0.4",
     "regions>=0.6",
     "scikit-learn>=1.1",
     "twirl>=0.1",
 ]
```

### Comparing `ost_photometry-0.0.7/PKG-INFO` & `ost_photometry-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ost_photometry
-Version: 0.0.7
+Version: 0.0.8
 Summary: Phtometry reduction and analysis package for the OST observatory
 Project-URL: Homepage, https://github.com/OST-Observatory/ost_photometry_package
 Project-URL: Bug Tracker, https://github.com/OST-Observatory/ost_photometry_package/issues
 Author-email: Rainer Hainich <rhainich@astro.physik.uni-potsdam.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: astropy>=5.0
 Requires-Dist: astroquery>=0.4
 Requires-Dist: ccdproc>=2.3
 Requires-Dist: matplotlib>=3.5
 Requires-Dist: numpy>=1.18
 Requires-Dist: path>=16.0
 Requires-Dist: pathlib>=1.0
-Requires-Dist: photutils>=1.5
+Requires-Dist: photutils>=1.8
 Requires-Dist: pytimedinput>=2.0
 Requires-Dist: regions>=0.6
 Requires-Dist: scikit-image
 Requires-Dist: scikit-learn>=1.1
 Requires-Dist: scipy
 Requires-Dist: twirl>=0.1
 Requires-Dist: uncertainties>=3.1
```


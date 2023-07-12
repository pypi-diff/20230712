# Comparing `tmp/pyorbital-v0.3.2.tar.gz` & `tmp/pyorbital-v1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyorbital-v0.3.2.tar", last modified: Thu Apr 10 09:03:49 2014, max compression, from Unix
+gzip compressed data, was "dist/pyorbital-v1.0.0.tar", last modified: Tue Aug 25 19:08:16 2015, max compression
```

## Comparing `pyorbital-v0.3.2.tar` & `pyorbital-v1.0.0.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2014-04-10 09:03:49.000000 pyorbital-v0.3.2/
--rw-rw-r--   0 travis    (1000) travis    (1000)      107 2014-04-10 09:03:08.000000 pyorbital-v0.3.2/MANIFEST.in
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2014-04-10 09:03:49.000000 pyorbital-v0.3.2/pyorbital.egg-info/
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2014-04-10 09:03:46.000000 pyorbital-v0.3.2/pyorbital.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (1000) travis    (1000)      487 2014-04-10 09:03:49.000000 pyorbital-v0.3.2/pyorbital.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)       10 2014-04-10 09:03:49.000000 pyorbital-v0.3.2/pyorbital.egg-info/top_level.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)      701 2014-04-10 09:03:49.000000 pyorbital-v0.3.2/pyorbital.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2014-04-10 09:03:49.000000 pyorbital-v0.3.2/pyorbital.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        5 2014-04-10 09:03:49.000000 pyorbital-v0.3.2/pyorbital.egg-info/requires.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)      701 2014-04-10 09:03:49.000000 pyorbital-v0.3.2/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)     1847 2014-04-10 09:03:08.000000 pyorbital-v0.3.2/setup.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2014-04-10 09:03:49.000000 pyorbital-v0.3.2/doc/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2014-04-10 09:03:49.000000 pyorbital-v0.3.2/doc/source/
--rw-rw-r--   0 travis    (1000) travis    (1000)     7265 2014-04-10 09:03:08.000000 pyorbital-v0.3.2/doc/source/conf.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2426 2014-04-10 09:03:08.000000 pyorbital-v0.3.2/doc/source/index.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     4606 2014-04-10 09:03:08.000000 pyorbital-v0.3.2/doc/Makefile
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2014-04-10 09:03:49.000000 pyorbital-v0.3.2/pyorbital/
--rw-rw-r--   0 travis    (1000) travis    (1000)        0 2014-04-10 09:03:08.000000 pyorbital-v0.3.2/pyorbital/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2740 2014-04-10 09:03:08.000000 pyorbital-v0.3.2/pyorbital/geoloc_example.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     6174 2014-04-10 09:03:08.000000 pyorbital-v0.3.2/pyorbital/astronomy.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     5314 2014-04-10 09:03:08.000000 pyorbital-v0.3.2/pyorbital/tlefile.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     6341 2014-04-10 09:03:08.000000 pyorbital-v0.3.2/pyorbital/geoloc_instrument_definitions.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    27407 2014-04-10 09:03:08.000000 pyorbital-v0.3.2/pyorbital/orbital.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      911 2014-04-10 09:03:08.000000 pyorbital-v0.3.2/pyorbital/version.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     9406 2014-04-10 09:03:08.000000 pyorbital-v0.3.2/pyorbital/geoloc.py
--rw-rw-r--   0 travis    (1000) travis    (1000)       59 2014-04-10 09:03:49.000000 pyorbital-v0.3.2/setup.cfg
--rw-rw-r--   0 travis    (1000) travis    (1000)    35147 2014-04-10 09:03:08.000000 pyorbital-v0.3.2/LICENSE.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)      183 2014-04-10 09:03:08.000000 pyorbital-v0.3.2/README
+drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2015-08-25 19:08:16.000000 pyorbital-v1.0.0/
+drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2015-08-25 19:08:16.000000 pyorbital-v1.0.0/doc/
+drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2015-08-25 19:08:16.000000 pyorbital-v1.0.0/doc/source/
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     7247 2015-08-25 19:06:58.000000 pyorbital-v1.0.0/doc/source/conf.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     2426 2013-03-07 17:05:00.000000 pyorbital-v1.0.0/doc/source/index.rst
+-rw-r--r--   0 a001673  (62310) smhiprimgrp  (2000)     4606 2011-10-06 08:34:05.000000 pyorbital-v1.0.0/doc/Makefile
+drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2015-08-25 19:08:16.000000 pyorbital-v1.0.0/pyorbital/
+-rw-r--r--   0 a001673  (62310) smhiprimgrp  (2000)        0 2011-10-06 08:34:05.000000 pyorbital-v1.0.0/pyorbital/__init__.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     6174 2015-03-02 11:46:40.000000 pyorbital-v1.0.0/pyorbital/astronomy.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     9424 2015-08-25 19:06:58.000000 pyorbital-v1.0.0/pyorbital/geoloc.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     2740 2014-01-07 12:47:08.000000 pyorbital-v1.0.0/pyorbital/geoloc_example.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     7399 2015-08-25 19:06:58.000000 pyorbital-v1.0.0/pyorbital/geoloc_instrument_definitions.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     3502 2013-03-22 07:59:44.000000 pyorbital-v1.0.0/pyorbital/geoloc_mikhail.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    28755 2015-08-25 19:06:58.000000 pyorbital-v1.0.0/pyorbital/orbital.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     6287 2015-02-19 08:31:45.000000 pyorbital-v1.0.0/pyorbital/tbus.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     6133 2015-02-18 14:11:25.000000 pyorbital-v1.0.0/pyorbital/tbusold.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    12745 2015-02-20 16:14:32.000000 pyorbital-v1.0.0/pyorbital/test_geoloc.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      979 2015-04-22 06:56:43.000000 pyorbital-v1.0.0/pyorbital/tle2intdes.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     9524 2015-08-25 19:06:58.000000 pyorbital-v1.0.0/pyorbital/tlefile.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      827 2015-08-25 19:06:58.000000 pyorbital-v1.0.0/pyorbital/version.py
+drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2015-08-25 19:08:16.000000 pyorbital-v1.0.0/pyorbital.egg-info/
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      701 2015-08-25 19:08:16.000000 pyorbital-v1.0.0/pyorbital.egg-info/PKG-INFO
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      613 2015-08-25 19:08:16.000000 pyorbital-v1.0.0/pyorbital.egg-info/SOURCES.txt
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)        1 2015-08-25 19:08:16.000000 pyorbital-v1.0.0/pyorbital.egg-info/dependency_links.txt
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)        1 2012-05-14 20:38:36.000000 pyorbital-v1.0.0/pyorbital.egg-info/not-zip-safe
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)       12 2015-08-25 19:08:16.000000 pyorbital-v1.0.0/pyorbital.egg-info/requires.txt
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)       10 2015-08-25 19:08:16.000000 pyorbital-v1.0.0/pyorbital.egg-info/top_level.txt
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    35147 2013-03-07 17:05:00.000000 pyorbital-v1.0.0/LICENSE.txt
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      107 2014-01-07 14:38:55.000000 pyorbital-v1.0.0/MANIFEST.in
+-rw-r--r--   0 a001673  (62310) smhiprimgrp  (2000)      183 2011-10-06 08:34:05.000000 pyorbital-v1.0.0/README
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     1854 2015-08-25 19:06:59.000000 pyorbital-v1.0.0/setup.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      701 2015-08-25 19:08:16.000000 pyorbital-v1.0.0/PKG-INFO
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      143 2015-08-25 19:08:16.000000 pyorbital-v1.0.0/setup.cfg
```

### Comparing `pyorbital-v0.3.2/pyorbital.egg-info/PKG-INFO` & `pyorbital-v1.0.0/pyorbital.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.0
+Metadata-Version: 1.1
 Name: pyorbital
-Version: v0.3.2
+Version: v1.0.0
 Summary: Orbital parameters and astronomical computations in Python
 Home-page: https://github.com/mraspaud/pyorbital
 Author: Martin Raspaud, Esben S. Nielsen
 Author-email: martin.raspaud@smhi.se, esn@dmi.dk
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pyorbital-v0.3.2/PKG-INFO` & `pyorbital-v1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.0
+Metadata-Version: 1.1
 Name: pyorbital
-Version: v0.3.2
+Version: v1.0.0
 Summary: Orbital parameters and astronomical computations in Python
 Home-page: https://github.com/mraspaud/pyorbital
 Author: Martin Raspaud, Esben S. Nielsen
 Author-email: martin.raspaud@smhi.se, esn@dmi.dk
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pyorbital-v0.3.2/setup.py` & `pyorbital-v1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
                    "Programming Language :: Python",
                    "Topic :: Scientific/Engineering",
                    "Topic :: Scientific/Engineering :: Astronomy"],
       url="https://github.com/mraspaud/pyorbital",
       test_suite='pyorbital.tests.suite',
       package_dir = {'pyorbital': 'pyorbital'},
       packages = ['pyorbital'],      
-      install_requires=['numpy'],
+      install_requires=['numpy>=1.6.0'],
       zip_safe=False,
       )
```

### Comparing `pyorbital-v0.3.2/doc/source/conf.py` & `pyorbital-v1.0.0/doc/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import sys, os
+import sys
+import os
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #sys.path.insert(0, os.path.abspath('.'))
 sys.path.insert(0, os.path.abspath('../../'))
 sys.path.insert(0, os.path.abspath('../../pyorbital'))
-from pyorbital.version import __version__, __major__, __minor__
+from pyorbital.version import __version__
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
@@ -40,24 +41,24 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'pyorbital'
-copyright = u'2012-2014, The Pytroll crew'
+copyright = u'2012-2015, The Pytroll crew'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
-# The short X.Y version.
-version = "v" + ".".join([__major__, __minor__])
 # The full version, including alpha/beta/rc tags.
 release = __version__
+# The short X.Y version.
+version = ".".join(release.split(".")[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
@@ -177,16 +178,16 @@
 
 # The font size ('10pt', '11pt' or '12pt').
 #latex_font_size = '10pt'
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-  ('index', 'pyorbital.tex', u'pyorbital Documentation',
-   u'The Pytroll crew', 'manual'),
+    ('index', 'pyorbital.tex', u'pyorbital Documentation',
+     u'The Pytroll crew', 'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 #latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
```

### Comparing `pyorbital-v0.3.2/doc/source/index.rst` & `pyorbital-v1.0.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyorbital-v0.3.2/doc/Makefile` & `pyorbital-v1.0.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyorbital-v0.3.2/pyorbital/geoloc_example.py` & `pyorbital-v1.0.0/pyorbital/geoloc_example.py`

 * *Files identical despite different names*

### Comparing `pyorbital-v0.3.2/pyorbital/astronomy.py` & `pyorbital-v1.0.0/pyorbital/astronomy.py`

 * *Files identical despite different names*

### Comparing `pyorbital-v0.3.2/pyorbital/geoloc_instrument_definitions.py` & `pyorbital-v1.0.0/pyorbital/geoloc_instrument_definitions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2013, 2014 Martin Raspaud
+# Copyright (c) 2013, 2014, 2015 Martin Raspaud
 
 # Author(s):
 
 #   Martin Raspaud <martin.raspaud@smhi.se>
 #   Mikhail Itkin <itkin.m@gmail.com>
 
 # This program is free software: you can redistribute it and/or modify
@@ -35,97 +35,127 @@
 
 Both scan angles and scan times are then combined into a ScanGeometry object.
 """
 
 import numpy as np
 from pyorbital.geoloc import ScanGeometry
 
-# number of instrument scans to use.
-scans_nb = 10
-
 ################################################################
 #
 #   AVHRR
 #
 ################################################################
 
-def avhrr(scans_nb, scan_points, scan_angle=55.37, decimate=1):
+
+def avhrr(scans_nb, scan_points,
+          scan_angle=55.37, frequency=1 / 6.0):
     """Definition of the avhrr instrument.
 
     Source: NOAA KLM User's Guide, Appendix J
     http://www.ncdc.noaa.gov/oa/pod-guide/ncdc/docs/klm/html/j/app-j.htm
     """
     # build the avhrr instrument (scan angles)
     avhrr_inst = np.vstack(((scan_points / 1023.5 - 1)
                             * np.deg2rad(-scan_angle),
                             np.zeros((len(scan_points),)))).transpose()
     avhrr_inst = np.tile(avhrr_inst, [scans_nb, 1])
 
     # building the corresponding times array
-    offset = np.arange(scans_nb) * decimate / 6.0
-    #times = (np.tile(scan_points * 0.000025 + 0.0025415, [scans_nb, 1])
+    offset = np.arange(scans_nb) * frequency
+    # times = (np.tile(scan_points * 0.000025 + 0.0025415, [scans_nb, 1])
     #         + np.expand_dims(offset, 1))
     times = (np.tile(scan_points * 0.000025, [scans_nb, 1])
              + np.expand_dims(offset, 1))
 
     return ScanGeometry(avhrr_inst, times.ravel())
 
-################################################################
-#### avhrr, all pixels
 
-# we take all pixels
-scan_points = np.arange(2048)
+def avhrr_gac(scan_times, scan_points,
+              scan_angle=55.37, frequency=0.5):
+    """Definition of the avhrr instrument, gac version
 
-# build the scan geometry object
-avhrr_all_geom = avhrr(scans_nb, scan_points)
+    Source: NOAA KLM User's Guide, Appendix J
+    http://www.ncdc.noaa.gov/oa/pod-guide/ncdc/docs/klm/html/j/app-j.htm
+    """
+    try:
+        offset = np.array([(t - scan_times[0]).seconds +
+                           (t - scan_times[0]).microseconds / 1000000.0 for t in scan_times])
+    except TypeError:
+        offset = np.arange(scan_times) * frequency
+    scans_nb = len(offset)
+    # build the avhrr instrument (scan angles)
+    avhrr_inst = np.vstack(((scan_points / 1023.5 - 1)
+                            * np.deg2rad(-scan_angle),
+                            np.zeros((len(scan_points),)))).transpose()
+    avhrr_inst = np.tile(avhrr_inst, [scans_nb, 1])
+
+    # building the corresponding times array
+    times = (np.tile(scan_points * 0.000025, [scans_nb, 1])
+             + np.expand_dims(offset, 1))
+    return ScanGeometry(avhrr_inst, times.ravel())
 
 ################################################################
-#### avhrr, edge pixels
+# avhrr, all pixels
 
-# we take only edge pixels
-scan_points = np.array([0, 2047])
+# build the scan geometry object
 
 
-# build the scan geometry object
-avhrr_edge_geom = avhrr(scans_nb, scan_points)
+def avhrr_all_geom(scans_nb):
+    # we take all pixels
+    scan_points = np.arange(2048)
+    return avhrr(scans_nb, scan_points)
 
 ################################################################
-#### avhrr, every 40th pixel from the 24th (aapp style)
+# avhrr, edge pixels
+
+# build the scan geometry object
+
 
-# we take only every 40th pixel
-scan_points = np.arange(24, 2048, 40)
+def avhrr_edge_geom(scans_nb):
+    # we take only edge pixels
+    scan_points = np.array([0, 2047])
+    return avhrr(scans_nb, scan_points)
+
+################################################################
+# avhrr, every 40th pixel from the 24th (aapp style)
 
 # build the scan geometry object
-avhrr_40_geom = avhrr(scans_nb, scan_points)
+
+
+def avhrr_40_geom(scans_nb):
+    # we take only every 40th pixel
+    scan_points = np.arange(24, 2048, 40)
+    return avhrr(scans_nb, scan_points)
 
 ################################################################
 #
 #   VIIRS
 #
 ################################################################
 
+
 def viirs(scans_nb, scan_indices=slice(0, None)):
     """Describe VIIRS instrument geometry, I-band.
 
     """
 
     entire_width = np.arange(6400)
     scan_points = entire_width[scan_indices]
-    
+
     across_track = (scan_points / 3199.5 - 1) * np.deg2rad(-55.84)
-    y_max_angle = np.arctan2(11.87/2, 824.0)
+    y_max_angle = np.arctan2(11.87 / 2, 824.0)
     along_track = np.array([-y_max_angle, 0, y_max_angle])
 
     scan_pixels = len(scan_points)
 
     scan = np.vstack((np.tile(across_track, scan_pixels),
                       np.repeat(along_track, 6400))).T
-    
+
     npp = np.tile(scan, [scans_nb, 1])
-    
+
     # from the timestamp in the filenames, a granule takes 1:25.400 to record
     # (85.4 seconds) so 1.779166667 would be the duration of 1 scanline
     # dividing the duration of a single scan by a width of 6400 pixels results
     # in 0.0002779947917 seconds for each column of 32 pixels in the scanline
 
     # the individual times per pixel are probably wrong, unless the scanning
     # behaves the same as for AVHRR, The VIIRS sensor rotates to allow internal
@@ -145,43 +175,43 @@
 #
 #   AMSU-A
 #
 ################################################################
 
 def amsua(scans_nb, edges_only=False):
     """ Describe AMSU-A instrument geometry
-    
+
     Parameters:
        scans_nb | int -  number of scan lines
-     
+
      Keywords:
      * edges_only - use only edge pixels
 
     Returns:
        pyorbital.geoloc.ScanGeometry object
-    
+
     """
 
-    scan_len  = 30 # 30 samples per scan
-    scan_rate = 8 # single scan, seconds
-    scan_angle = -48.3 # swath, degrees
-    sampling_interval = 0.2 # single view, seconds
-    sync_time = 0.00355 # delay before the actual scan starts
+    scan_len = 30  # 30 samples per scan
+    scan_rate = 8  # single scan, seconds
+    scan_angle = -48.3  # swath, degrees
+    sampling_interval = 0.2  # single view, seconds
+    sync_time = 0.00355  # delay before the actual scan starts
 
     if edges_only:
         scan_points = np.array([0, scan_len - 1])
     else:
         scan_points = np.arange(0, scan_len)
 
     # build the instrument (scan angles)
-    samples = np.vstack(((scan_points / (scan_len*0.5-0.5) - 1)
+    samples = np.vstack(((scan_points / (scan_len * 0.5 - 0.5) - 1)
                          * np.deg2rad(scan_angle),
                          np.zeros((len(scan_points),)))).transpose()
     samples = np.tile(samples, [scans_nb, 1])
 
     # building the corresponding times array
     offset = np.arange(scans_nb) * scan_rate
     times = (np.tile(scan_points * sampling_interval + sync_time, [scans_nb, 1])
-	         + np.expand_dims(offset, 1))
+             + np.expand_dims(offset, 1))
 
     # build the scan geometry object
     return ScanGeometry(samples, times.ravel())
```

### Comparing `pyorbital-v0.3.2/pyorbital/orbital.py` & `pyorbital-v1.0.0/pyorbital/orbital.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 
 from datetime import datetime, timedelta
 import numpy as np
 from pyorbital import tlefile
 from pyorbital import astronomy
 import warnings
 
-ECC_EPS = 1.0e-6	# Too low for computing further drops.
+ECC_EPS = 1.0e-6  # Too low for computing further drops.
 ECC_LIMIT_LOW = -1.0e-3
-ECC_LIMIT_HIGH = 1.0 - ECC_EPS	# Too close to 1
+ECC_LIMIT_HIGH = 1.0 - ECC_EPS  # Too close to 1
 ECC_ALL = 1.0e-4
 
 EPS_COS = 1.5e-12
 
 NR_EPS = 1.0e-12
 
 CK2 = 5.413080e-4
@@ -50,31 +50,33 @@
 XKE = 0.743669161e-1
 XKMPER = 6378.135
 XMNPDA = 1440.0
 #MFACTOR = 7.292115E-5
 AE = 1.0
 SECDAY = 8.6400E4
 
-F = 1 / 298.257223563 # Earth flattening WGS-84
-A = 6378.137 # WGS84 Equatorial radius
+F = 1 / 298.257223563  # Earth flattening WGS-84
+A = 6378.137  # WGS84 Equatorial radius
 
 
 SGDP4_ZERO_ECC = 0
 SGDP4_DEEP_NORM = 1
 SGDP4_NEAR_SIMP = 2
 SGDP4_NEAR_NORM = 3
 
 KS = AE * (1.0 + S0 / XKMPER)
 A3OVK2 = (-XJ3 / CK2) * AE**3
 
+
 class OrbitalError(Exception):
     pass
 
 
 class Orbital(object):
+
     """Class for orbital computations.
 
     The *satellite* parameter is the name of the satellite to work on and is
     used to retreive the right TLE data for internet or from *tle_file* in case
     it is provided.
     """
 
@@ -134,37 +136,37 @@
 
         if normalize:
             pos /= XKMPER
             vel /= XKMPER * XMNPDA / SECDAY
 
         return pos, vel
 
-
     def get_lonlatalt(self, utc_time):
         """Calculate sublon, sublat and altitude of satellite.
         http://celestrak.com/columns/v02n03/
         """
-        (pos_x, pos_y, pos_z), (vel_x, vel_y, vel_z) = self.get_position(utc_time, normalize=True)
+        (pos_x, pos_y, pos_z), (vel_x, vel_y, vel_z) = self.get_position(
+            utc_time, normalize=True)
 
         lon = ((np.arctan2(pos_y * XKMPER, pos_x * XKMPER) - astronomy.gmst(utc_time))
                % (2 * np.pi))
 
         lon = np.where(lon > np.pi, lon - np.pi * 2, lon)
-        lon = np.where(lon <= -np.pi, lon + np.pi *2, lon)
+        lon = np.where(lon <= -np.pi, lon + np.pi * 2, lon)
 
         r = np.sqrt(pos_x ** 2 + pos_y ** 2)
         lat = np.arctan2(pos_z, r)
         e2 = F * (2 - F)
         while True:
             lat2 = lat
-            c = 1/(np.sqrt(1 - e2 * (np.sin(lat2) ** 2)))
-            lat = np.arctan2(pos_z + c * e2 *np.sin(lat2), r)
+            c = 1 / (np.sqrt(1 - e2 * (np.sin(lat2) ** 2)))
+            lat = np.arctan2(pos_z + c * e2 * np.sin(lat2), r)
             if np.all(abs(lat - lat2) < 1e-10):
                 break
-        alt = r / np.cos(lat)- c;
+        alt = r / np.cos(lat) - c
         alt *= A
         return np.rad2deg(lon), np.rad2deg(lat), alt
 
     def find_aos(self, utc_time, lon, lat):
         pass
 
     def find_aol(self, utc_time, lon, lat):
@@ -177,17 +179,18 @@
         utc_time: Observation time (datetime object)
         lon: Longitude of observer position on ground
         lat: Latitude of observer position on ground
         alt: Altitude above sea-level (geoid) of observer position on ground
 
         Return: (Azimuth, Elevation)
         """
-        (pos_x, pos_y, pos_z), (vel_x, vel_y, vel_z) = self.get_position(utc_time, normalize=False)
+        (pos_x, pos_y, pos_z), (vel_x, vel_y, vel_z) = self.get_position(
+            utc_time, normalize=False)
         (opos_x, opos_y, opos_z), (ovel_x, ovel_y, ovel_z) = \
-                                    astronomy.observer_position(utc_time, lon, lat, alt)
+            astronomy.observer_position(utc_time, lon, lat, alt)
 
         lon = np.deg2rad(lon)
         lat = np.deg2rad(lat)
 
         theta = (astronomy.gmst(utc_time) + lon) % (2 * np.pi)
 
         rx = pos_x - opos_x
@@ -195,17 +198,19 @@
         rz = pos_z - opos_z
 
         sin_lat = np.sin(lat)
         cos_lat = np.cos(lat)
         sin_theta = np.sin(theta)
         cos_theta = np.cos(theta)
 
-        top_s = sin_lat * cos_theta * rx + sin_lat * sin_theta * ry - cos_lat * rz
+        top_s = sin_lat * cos_theta * rx + \
+            sin_lat * sin_theta * ry - cos_lat * rz
         top_e = -sin_theta * rx + cos_theta * ry
-        top_z = cos_lat * cos_theta * rx + cos_lat * sin_theta * ry + sin_lat * rz
+        top_z = cos_lat * cos_theta * rx + \
+            cos_lat * sin_theta * ry + sin_lat * rz
 
         az_ = np.arctan(-top_e / top_s)
 
         az_ = np.where(top_s > 0, az_ + np.pi, az_)
         az_ = np.where(az_ < 0, az_ + 2 * np.pi, az_)
 
         rg_ = np.sqrt(rx * rx + ry * ry + rz * rz)
@@ -218,60 +223,63 @@
         Optionally use TBUS-style orbit numbering (TLE orbit number + 1)
         """
         try:
             dt = astronomy._days(utc_time - self.orbit_elements.an_time)
             orbit_period = astronomy._days(self.orbit_elements.an_period)
         except AttributeError:
             pos_epoch, vel_epoch = self.get_position(self.tle.epoch,
-                                                 normalize=False)
+                                                     normalize=False)
             if np.abs(pos_epoch[2]) > 1 or not vel_epoch[2] > 0:
                 # Epoch not at ascending node
-                self.orbit_elements.an_time = self.get_last_an_time(self.tle.epoch)
+                self.orbit_elements.an_time = self.get_last_an_time(
+                    self.tle.epoch)
             else:
                 # Epoch at ascending node (z < 1 km) and positive v_z
                 self.orbit_elements.an_time = self.tle.epoch
 
             self.orbit_elements.an_period = self.orbit_elements.an_time - \
-                                            self.get_last_an_time(self.orbit_elements.an_time
-                                                                  - timedelta(minutes=10))
+                self.get_last_an_time(self.orbit_elements.an_time
+                                      - timedelta(minutes=10))
 
             dt = astronomy._days(utc_time - self.orbit_elements.an_time)
             orbit_period = astronomy._days(self.orbit_elements.an_period)
 
-
         orbit = int(self.tle.orbit + dt / orbit_period +
-                 self.tle.mean_motion_derivative * dt**2 +
-                 self.tle.mean_motion_sec_derivative * dt**3)
+                    self.tle.mean_motion_derivative * dt**2 +
+                    self.tle.mean_motion_sec_derivative * dt**3)
 
         if tbus_style:
             orbit += 1
         return orbit
 
-    def get_next_passes(self, utc_time, length, lon, lat, alt, tol=0.001):
+    def get_next_passes(self, utc_time, length, lon, lat, alt, tol=0.001, horizon=0):
         """Calculate passes for the next hours for a given start time and a
         given observer.
 
         Original by Martin.
 
         utc_time: Observation time (datetime object)
         length: Number of hours to find passes (int)
         lon: Longitude of observer position on ground (float)
         lat: Latitude of observer position on ground (float)
         alt: Altitude above sea-level (geoid) of observer position on ground (float)
         tol: precision of the result in seconds
+        horizon: the elevation of horizon to compute risetime and falltime.
 
         Return: [(rise-time, fall-time, max-elevation-time), ...]
         """
 
         def elevation(minutes):
             """elevation
             """
             return self.get_observer_look(utc_time +
-                                          timedelta(minutes=minutes),
-                                          lon, lat, alt)[1]
+                                          timedelta(
+                                              minutes=np.float64(minutes)),
+                                          lon, lat, alt)[1] - horizon
+
         def elevation_inv(minutes):
             """inverse of elevation
             """
             return -elevation(minutes)
 
         def get_root_secant(fun, start, end, tol=0.01):
             """Secant method
@@ -301,50 +309,51 @@
             f_a = fun(a)
             f_b = fun(b)
             f_c = fun(c)
 
             while abs(c - a) > tol:
                 x = b - 0.5 * (((b - a) ** 2 * (f_b - f_c)
                                 - (b - c) ** 2 * (f_b - f_a)) /
-                               ((b - a) * (f_b - f_c)  - (b - c) * (f_b - f_a)))
+                               ((b - a) * (f_b - f_c) - (b - c) * (f_b - f_a)))
                 f_x = fun(x)
                 if x > b:
                     a, b, c = b, x, c
                     f_a, f_b, f_c = f_b, f_x, f_c
                 else:
                     a, b, c = a, x, b
                     f_a, f_b, f_c = f_a, f_x, f_b
 
             return x
 
         times = utc_time + np.array([timedelta(minutes=minutes)
-                                    for minutes in range(length * 60)])
-        elev = self.get_observer_look(times, lon, lat, alt)[1]
+                                     for minutes in range(length * 60)])
+        elev = self.get_observer_look(times, lon, lat, alt)[1] - horizon
         zcs = np.where(np.diff(np.sign(elev)))[0]
 
         res = []
         risetime = None
         falltime = None
         for guess in zcs:
-            horizon_mins = get_root_secant(elevation, guess, guess + 1.0, tol=tol/60.0)
+            horizon_mins = get_root_secant(
+                elevation, guess, guess + 1.0, tol=tol / 60.0)
             horizon_time = utc_time + timedelta(minutes=horizon_mins)
             if elev[guess] < 0:
                 risetime = horizon_time
                 risemins = horizon_mins
                 falltime = None
             else:
                 falltime = horizon_time
                 fallmins = horizon_mins
                 if risetime:
                     middle = (risemins + fallmins) / 2.0
                     highest = utc_time + \
                         timedelta(minutes=get_max_parab(
-                        elevation_inv,
-                        middle - 0.1, middle + 0.1,
-                        tol=tol/60.0
+                            elevation_inv,
+                            middle - 0.1, middle + 0.1,
+                            tol=tol / 60.0
                         ))
                     res += [(risetime, falltime, highest)]
                 risetime = None
         return res
 
     def _get_time_at_horizon(self, utc_time, obslon, obslat, **kwargs):
         """Get the time closest in time to *utc_time* when the
@@ -362,15 +371,15 @@
             precision = timedelta(seconds=0.001)
         if "max_iterations" in kwargs:
             nmax_iter = kwargs["max_iterations"]
         else:
             nmax_iter = 100
 
         sec_step = 0.5
-        t_step = timedelta(seconds=sec_step/2.0)
+        t_step = timedelta(seconds=sec_step / 2.0)
 
         # Local derivative:
         def fprime(timex):
             el0 = self.get_observer_look(timex - t_step,
                                          obslon, obslat, 0.0)[1]
             el1 = self.get_observer_look(timex + t_step,
                                          obslon, obslat, 0.0)[1]
@@ -385,77 +394,82 @@
             tx0 = tx1
             fpr = fprime(tx0)
             # When the elevation is high the scale is high, and when
             # the elevation is low the scale is low
             #var_scale = np.abs(np.sin(fpr[0] * np.pi/180.))
             #var_scale = np.sqrt(var_scale)
             var_scale = np.abs(fpr[0])
-            tx1 = tx0 - timedelta(seconds = (eps * var_scale * fpr[1]))
+            tx1 = tx0 - timedelta(seconds=(eps * var_scale * fpr[1]))
             idx = idx + 1
-            #print idx, tx0, tx1, var_scale, fpr
+            # print idx, tx0, tx1, var_scale, fpr
             if abs(tx1 - utc_time) < precision and idx < 2:
                 tx1 = tx1 + timedelta(seconds=1.0)
 
         if abs(tx1 - tx0) <= precision and idx < nmax_iter:
             return tx1
         else:
             return None
 
+
 class OrbitElements(object):
+
     """Class holding the orbital elements.
     """
 
     def __init__(self, tle):
         self.epoch = tle.epoch
         self.excentricity = tle.excentricity
         self.inclination = np.deg2rad(tle.inclination)
         self.right_ascension = np.deg2rad(tle.right_ascension)
         self.arg_perigee = np.deg2rad(tle.arg_perigee)
         self.mean_anomaly = np.deg2rad(tle.mean_anomaly)
 
         self.mean_motion = tle.mean_motion * (np.pi * 2 / XMNPDA)
-        self.mean_motion_derivative = tle.mean_motion_derivative * np.pi * 2 / XMNPDA ** 2
-        self.mean_motion_sec_derivative = tle.mean_motion_sec_derivative * np.pi * 2 / XMNPDA ** 3
+        self.mean_motion_derivative = tle.mean_motion_derivative * \
+            np.pi * 2 / XMNPDA ** 2
+        self.mean_motion_sec_derivative = tle.mean_motion_sec_derivative * \
+            np.pi * 2 / XMNPDA ** 3
         self.bstar = tle.bstar * AE
 
         n_0 = self.mean_motion
         k_e = XKE
         k_2 = CK2
         i_0 = self.inclination
         e_0 = self.excentricity
 
-        a_1 = (k_e / n_0) ** (2.0/3)
-        delta_1 = ((3/2.0) * (k_2 / a_1**2) * ((3 * np.cos(i_0)**2 - 1) /
-                                              (1 - e_0**2)**(2.0/3)))
+        a_1 = (k_e / n_0) ** (2.0 / 3)
+        delta_1 = ((3 / 2.0) * (k_2 / a_1**2) * ((3 * np.cos(i_0)**2 - 1) /
+                                                 (1 - e_0**2)**(2.0 / 3)))
 
-        a_0 = a_1 * (1 - delta_1/3 - delta_1**2 - (134.0/81) * delta_1**3)
+        a_0 = a_1 * (1 - delta_1 / 3 - delta_1**2 - (134.0 / 81) * delta_1**3)
 
-        delta_0 = ((3/2.0) * (k_2 / a_0**2) * ((3 * np.cos(i_0)**2 - 1) /
-                                              (1 - e_0**2)**(2.0/3)))
+        delta_0 = ((3 / 2.0) * (k_2 / a_0**2) * ((3 * np.cos(i_0)**2 - 1) /
+                                                 (1 - e_0**2)**(2.0 / 3)))
 
         # original mean motion
         n_0pp = n_0 / (1 + delta_0)
         self.original_mean_motion = n_0pp
 
         # semi major axis
         a_0pp = a_0 / (1 - delta_0)
         self.semi_major_axis = a_0pp
 
         self.period = np.pi * 2 / n_0pp
 
         self.perigee = (a_0pp * (1 - e_0) / AE - AE) * XKMPER
 
         self.right_ascension_lon = (self.right_ascension
-                                           - astronomy.gmst(self.epoch))
+                                    - astronomy.gmst(self.epoch))
 
         if self.right_ascension_lon > np.pi:
             self.right_ascension_lon -= 2 * np.pi
 
 
 class _SGDP4(object):
+
     """Class for the SGDP4 computations.
     """
 
     def __init__(self, orbit_elements):
         self.mode = None
 
         perigee = orbit_elements.perigee
@@ -493,15 +507,16 @@
         self.x7thm1 = 7.0 * theta2 - 1.0
 
         a1 = (XKE / self.xn_0) ** (2. / 3)
         betao2 = 1.0 - self.eo**2
         betao = np.sqrt(betao2)
         temp0 = 1.5 * CK2 * self.x3thm1 / (betao * betao2)
         del1 = temp0 / (a1**2)
-        a0 = a1 * (1.0 - del1 * (1.0 / 3.0 + del1 * (1.0 + del1 * 134.0 / 81.0)))
+        a0 = a1 * \
+            (1.0 - del1 * (1.0 / 3.0 + del1 * (1.0 + del1 * 134.0 / 81.0)))
         del0 = temp0 / (a0**2)
         self.xnodp = self.xn_0 / (1.0 + del0)
         self.aodp = (a0 / (1.0 - del0))
         self.perigee = (self.aodp * (1.0 - self.eo) - AE) * XKMPER
         self.apogee = (self.aodp * (1.0 + self.eo) - AE) * XKMPER
         self.period = (2 * np.pi * 1440.0 / XMNPDA) / self.xnodp
 
@@ -532,127 +547,137 @@
         etasq = self.eta**2
         eeta = self.eo * self.eta
         psisq = np.abs(1.0 - etasq)
         coef = qoms24 * tsi**4
         coef_1 = coef / psisq**3.5
 
         self.c2 = (coef_1 * self.xnodp * (self.aodp *
-             (1.0 + 1.5 * etasq + eeta * (4.0 + etasq)) +
-             (0.75 * CK2) * tsi / psisq * self.x3thm1 *
-             (8.0 + 3.0 * etasq * (8.0 + etasq))))
+                                          (1.0 + 1.5 * etasq + eeta * (4.0 + etasq)) +
+                                          (0.75 * CK2) * tsi / psisq * self.x3thm1 *
+                                          (8.0 + 3.0 * etasq * (8.0 + etasq))))
 
         self.c1 = self.bstar * self.c2
 
         self.c4 = (2.0 * self.xnodp * coef_1 * self.aodp * betao2 * (self.eta *
-             (2.0 + 0.5 * etasq) + self.eo * (0.5 + 2.0 *
-             etasq) - (2.0 * CK2) * tsi / (self.aodp * psisq) * (-3.0 *
-             self.x3thm1 * (1.0 - 2.0 * eeta + etasq *
-             (1.5 - 0.5 * eeta)) + 0.75 * self.x1mth2 * (2.0 *
-             etasq - eeta * (1.0 + etasq)) * np.cos(2.0 * self.omegao))))
+                                                                     (2.0 + 0.5 * etasq) + self.eo * (0.5 + 2.0 *
+                                                                                                      etasq) - (2.0 * CK2) * tsi / (self.aodp * psisq) * (-3.0 *
+                                                                                                                                                          self.x3thm1 * (1.0 - 2.0 * eeta + etasq *
+                                                                                                                                                                         (1.5 - 0.5 * eeta)) + 0.75 * self.x1mth2 * (2.0 *
+                                                                                                                                                                                                                     etasq - eeta * (1.0 + etasq)) * np.cos(2.0 * self.omegao))))
 
         self.c5, self.c3, self.omgcof = 0.0, 0.0, 0.0
 
-
         if self.mode == SGDP4_NEAR_NORM:
             self.c5 = (2.0 * coef_1 * self.aodp * betao2 *
-             (1.0 + 2.75 * (etasq + eeta) + eeta * etasq))
+                       (1.0 + 2.75 * (etasq + eeta) + eeta * etasq))
             if self.eo > ECC_ALL:
-                self.c3 = coef * tsi * A3OVK2 * self.xnodp * AE * self.sinIO / self.eo
+                self.c3 = coef * tsi * A3OVK2 * \
+                    self.xnodp * AE * self.sinIO / self.eo
             self.omgcof = self.bstar * self.c3 * np.cos(self.omegao)
 
         temp1 = 3.0 * CK2 * pinvsq * self.xnodp
         temp2 = temp1 * CK2 * pinvsq
         temp3 = 1.25 * CK4 * pinvsq**2 * self.xnodp
 
         self.xmdot = (self.xnodp + (0.5 * temp1 * betao * self.x3thm1 + 0.0625 *
-                temp2 * betao * (13.0 - 78.0 * theta2 +
-                137.0 * theta4)))
+                                    temp2 * betao * (13.0 - 78.0 * theta2 +
+                                                     137.0 * theta4)))
 
         x1m5th = 1.0 - 5.0 * theta2
 
         self.omgdot = (-0.5 * temp1 * x1m5th + 0.0625 * temp2 *
-                 (7.0 - 114.0 * theta2 + 395.0 * theta4) +
-                 temp3 * (3.0 - 36.0 * theta2 + 49.0 * theta4))
+                       (7.0 - 114.0 * theta2 + 395.0 * theta4) +
+                       temp3 * (3.0 - 36.0 * theta2 + 49.0 * theta4))
 
         xhdot1 = -temp1 * self.cosIO
         self.xnodot = (xhdot1 + (0.5 * temp2 * (4.0 - 19.0 * theta2) +
-                 2.0 * temp3 * (3.0 - 7.0 * theta2)) * self.cosIO)
+                                 2.0 * temp3 * (3.0 - 7.0 * theta2)) * self.cosIO)
 
         if self.eo > ECC_ALL:
             self.xmcof = (-(2. / 3) * AE) * coef * self.bstar / eeta
         else:
             self.xmcof = 0.0
 
         self.xnodcf = 3.5 * betao2 * xhdot1 * self.c1
         self.t2cof = 1.5 * self.c1
 
-        # Check for possible divide-by-zero for X/(1+cos(xincl)) when calculating xlcof */
-    	temp0 = 1.0 + self.cosIO
-    	if np.abs(temp0) < EPS_COS:
-    	    temp0 = np.sign(temp0) * EPS_COS
+        # Check for possible divide-by-zero for X/(1+cos(xincl)) when
+        # calculating xlcof */
+        temp0 = 1.0 + self.cosIO
+        if np.abs(temp0) < EPS_COS:
+            temp0 = np.sign(temp0) * EPS_COS
 
-    	self.xlcof = 0.125 * A3OVK2 * self.sinIO * (3.0 + 5.0 * self.cosIO) / temp0
+        self.xlcof = 0.125 * A3OVK2 * self.sinIO * \
+            (3.0 + 5.0 * self.cosIO) / temp0
 
         self.aycof = 0.25 * A3OVK2 * self.sinIO
 
         self.cosXMO = np.cos(self.xmo)
         self.sinXMO = np.sin(self.xmo)
         self.delmo = (1.0 + self.eta * self.cosXMO)**3
 
         if self.mode == SGDP4_NEAR_NORM:
             c1sq = self.c1**2
             self.d2 = 4.0 * self.aodp * tsi * c1sq
             temp0 = self.d2 * tsi * self.c1 / 3.0
             self.d3 = (17.0 * self.aodp + s4) * temp0
-            self.d4 = 0.5 * temp0 * self.aodp * tsi * (221.0 * self.aodp + 31.0 * s4) * self.c1
+            self.d4 = 0.5 * temp0 * self.aodp * tsi * \
+                (221.0 * self.aodp + 31.0 * s4) * self.c1
             self.t3cof = self.d2 + 2.0 * c1sq
-            self.t4cof = 0.25 * (3.0 * self.d3 + self.c1 * (12.0 * self.d2 + 10.0 * c1sq))
+            self.t4cof = 0.25 * \
+                (3.0 * self.d3 + self.c1 * (12.0 * self.d2 + 10.0 * c1sq))
             self.t5cof = (0.2 * (3.0 * self.d4 + 12.0 * self.c1 * self.d3 + 6.0 * self.d2**2 +
-                    15.0 * c1sq * (2.0 * self.d2 + c1sq)))
+                                 15.0 * c1sq * (2.0 * self.d2 + c1sq)))
 
         elif self.mode == SGDP4_DEEP_NORM:
             raise NotImplementedError('Deep space calculations not supported')
 
     def propagate(self, utc_time):
         kep = {}
 
         ts = astronomy._days(utc_time - self.t_0) * XMNPDA
 
         em = self.eo
         xinc = self.xincl
 
-        xmp   = self.xmo + self.xmdot * ts
+        xmp = self.xmo + self.xmdot * ts
         xnode = self.xnodeo + ts * (self.xnodot + ts * self.xnodcf)
         omega = self.omegao + self.omgdot * ts
 
         if self.mode == SGDP4_ZERO_ECC:
             raise NotImplementedError('Mode SGDP4_ZERO_ECC not implemented')
         elif self.mode == SGDP4_NEAR_SIMP:
             raise NotImplementedError('Mode "Near-space, simplified equations"'
                                       ' not implemented')
         elif self.mode == SGDP4_NEAR_NORM:
-            delm  = self.xmcof * ((1.0 + self.eta * np.cos(xmp))**3 - self.delmo)
+            delm = self.xmcof * \
+                ((1.0 + self.eta * np.cos(xmp))**3 - self.delmo)
             temp0 = ts * self.omgcof + delm
             xmp += temp0
             omega -= temp0
-            tempa = 1.0 - (ts * (self.c1 + ts * (self.d2 + ts * (self.d3 + ts * self.d4))))
-            tempe = self.bstar * (self.c4 * ts + self.c5 * (np.sin(xmp) - self.sinXMO))
-            templ = ts * ts * (self.t2cof + ts * (self.t3cof + ts * (self.t4cof + ts * self.t5cof)))
+            tempa = 1.0 - \
+                (ts *
+                 (self.c1 + ts * (self.d2 + ts * (self.d3 + ts * self.d4))))
+            tempe = self.bstar * \
+                (self.c4 * ts + self.c5 * (np.sin(xmp) - self.sinXMO))
+            templ = ts * ts * \
+                (self.t2cof + ts *
+                 (self.t3cof + ts * (self.t4cof + ts * self.t5cof)))
             a = self.aodp * tempa**2
             e = em - tempe
             xl = xmp + omega + xnode + self.xnodp * templ
 
         else:
-            raise  NotImplementedError('Deep space calculations not supported')
+            raise NotImplementedError('Deep space calculations not supported')
 
         if np.any(a < 1):
             raise Exception('Satellite crased at time %s', utc_time)
         elif np.any(e < ECC_LIMIT_LOW):
-            raise ValueError('Satellite modified eccentricity to low: %e < %e'
-                             % (e, ECC_LIMIT_LOW))
+            raise ValueError('Satellite modified eccentricity to low: %s < %e'
+                             % (str(e[e < ECC_LIMIT_LOW]), ECC_LIMIT_LOW))
 
         e = np.where(e < ECC_EPS, ECC_EPS, e)
         e = np.where(e > ECC_LIMIT_HIGH, ECC_LIMIT_HIGH, e)
 
         beta2 = 1.0 - e**2
 
         # Long period periodics
@@ -689,15 +714,15 @@
 
             # 1st order Newton-Raphson correction.
             nr = f / df
 
             # 2nd order Newton-Raphson correction.
             nr = np.where(np.logical_and(i == 0, np.abs(nr) > 1.25 * maxnr),
                           np.sign(nr) * maxnr,
-                          f / (df + 0.5*esinE*nr))
+                          f / (df + 0.5 * esinE * nr))
             epw += nr
 
         # Short period preliminary quantities
         temp0 = 1.0 - elsq
         betal = np.sqrt(temp0)
         pl = a * temp0
         r = a * (1.0 - ecosE)
@@ -711,28 +736,29 @@
         cos2u = 2.0 * cosu**2 - 1.0
         temp0 = 1.0 / pl
         temp1 = CK2 * temp0
         temp2 = temp1 * temp0
 
         # Update for short term periodics to position terms.
 
-        rk = r * (1.0 - 1.5 * temp2 * betal * self.x3thm1) + 0.5 * temp1 * self.x1mth2 * cos2u
+        rk = r * (1.0 - 1.5 * temp2 * betal * self.x3thm1) + \
+            0.5 * temp1 * self.x1mth2 * cos2u
         uk = u - 0.25 * temp2 * self.x7thm1 * sin2u
         xnodek = xnode + 1.5 * temp2 * self.cosIO * sin2u
         xinck = xinc + 1.5 * temp2 * self.cosIO * self.sinIO * cos2u
 
         if np.any(rk < 1):
             raise Exception('Satellite crased at time %s', utc_time)
 
         temp0 = np.sqrt(a)
         temp2 = XKE / (a * temp0)
-        rdotk = ((XKE * temp0 * esinE * invR -temp2 * temp1 * self.x1mth2 * sin2u) *
+        rdotk = ((XKE * temp0 * esinE * invR - temp2 * temp1 * self.x1mth2 * sin2u) *
                  (XKMPER / AE * XMNPDA / 86400.0))
         rfdotk = ((XKE * np.sqrt(pl) * invR + temp2 * temp1 *
-                  (self.x1mth2 * cos2u + 1.5 * self.x3thm1)) *
+                   (self.x1mth2 * cos2u + 1.5 * self.x3thm1)) *
                   (XKMPER / AE * XMNPDA / 86400.0))
 
         kep['radius'] = rk * XKMPER / AE
         kep['theta'] = uk
         kep['eqinc'] = xinck
         kep['ascn'] = xnodek
         kep['argp'] = omega
```

### Comparing `pyorbital-v0.3.2/pyorbital/version.py` & `pyorbital-v1.0.0/pyorbital/version.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2014 Martin Raspaud
+# Copyright (c) 2014, 2015 Martin Raspaud
 
 # Author(s):
 
 #   Martin Raspaud <martin.raspaud@smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -19,12 +19,8 @@
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Version file.
 """
 
-__major__ = "0"
-__minor__ = "3"
-__patch__ = "2"
-
-__version__ = "v" + ".".join([__major__, __minor__, __patch__])
+__version__ = "v1.0.0"
```

### Comparing `pyorbital-v0.3.2/pyorbital/geoloc.py` & `pyorbital-v1.0.0/pyorbital/geoloc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2011, 2012, 2013, 2014.
+# Copyright (c) 2011, 2012, 2013, 2014, 2015.
 
 # Author(s):
 
 #   Martin Raspaud <martin.raspaud@smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -30,52 +30,54 @@
 # - test !!!
 
 import numpy as np
 from numpy import cos, sin, sqrt
 from datetime import timedelta
 from pyorbital.orbital import Orbital
 
-a = 6378.137 # km
-b = 6356.75231414 # km, GRS80
-#b = 6356.752314245 # km, WGS84
+a = 6378.137  # km
+b = 6356.75231414  # km, GRS80
+# b = 6356.752314245 # km, WGS84
+
 
 def geodetic_lat(point, a=a, b=b):
 
     x, y, z = point
-    r = np.sqrt(x*x + y*y)
+    r = np.sqrt(x * x + y * y)
     geoc_lat = np.arctan2(z, r)
 
     geod_lat = geoc_lat
-    e2 = (a*a - b*b) / (a*a)
+    e2 = (a * a - b * b) / (a * a)
     while True:
         phi = geod_lat
-        C = 1  / sqrt(1 - e2 * sin(phi)**2)
-        geod_lat = np.arctan2(z + a*C*e2 * sin(phi), r)
+        C = 1 / sqrt(1 - e2 * sin(phi)**2)
+        geod_lat = np.arctan2(z + a * C * e2 * sin(phi), r)
         if np.allclose(geod_lat, phi):
             return geod_lat
-                      
+
 
 def subpoint(query_point, a=a, b=b):
     """Get the point on the ellipsoid under the *query_point*.
     """
     x, y, z = query_point
-    r = sqrt(x*x + y*y)
+    r = sqrt(x * x + y * y)
 
     lat = geodetic_lat(query_point)
     lon = np.arctan2(y, x)
-    e2_ = (a*a - b*b) / (a*a)
+    e2_ = (a * a - b * b) / (a * a)
     n__ = a / sqrt(1 - e2_ * sin(lat)**2)
     nx_ = n__ * cos(lat) * cos(lon)
     ny_ = n__ * cos(lat) * sin(lon)
-    nz_ = (1-e2_) * n__ * sin(lat)
+    nz_ = (1 - e2_) * n__ * sin(lat)
 
     return np.vstack([nx_, ny_, nz_])
-    
+
 
 class ScanGeometry(object):
+
     """Description of the geometry of an instrument.
 
     *fovs* is the x and y viewing angles of the instrument. y is zero if the we
     talk about scanlines of course. *times* is the time of viewing of each
     angle relative to the start of the scanning, so it should have the same
     size as the *fovs*. *attitude* is the attitude correction to apply.
     """
@@ -91,25 +93,24 @@
     def vectors(self, pos, vel, roll=0.0, pitch=0.0, yaw=0.0):
         """Get unit vectors pointing to the different pixels.
 
         *pos* and *vel* are column vectors, or matrices of column
         vectors. Returns vectors as stacked rows.
         """
         # TODO: yaw steering mode !
-        
-        
+
         # Fake nadir: This is the intersection point between the satellite
         # looking down at the centre of the ellipsoid and the surface of the
         # ellipsoid. Nadir on the other hand is the point which vertical goes
         # through the satellite...
         #nadir = -pos / vnorm(pos)
 
         nadir = subpoint(-pos)
         nadir /= vnorm(nadir)
-        
+
         # x is along track (roll)
         x = vel / vnorm(vel)
 
         # y is cross track (pitch)
         y = np.cross(nadir, vel, 0, 0, 0)
         y /= vnorm(y)
 
@@ -120,167 +121,171 @@
         # then around z
         return qrotate(xy_rotated, nadir, yaw)
 
     def times(self, start_of_scan):
         tds = [timedelta(seconds=i) for i in self._times]
         return np.array(tds) + start_of_scan
 
+
 class Quaternion(object):
 
     def __init__(self, scalar, vector):
         self.__x, self.__y, self.__z = vector
         self.__w = scalar
 
     def rotation_matrix(self):
         x, y, z, w = self.__x, self.__y, self.__z, self.__w
         zero = np.zeros_like(x)
         return np.array(
             ((w**2 + x**2 - y**2 - z**2,
-              2*x*y + 2*z*w,
-              2*x*z - 2*y*w,
+              2 * x * y + 2 * z * w,
+              2 * x * z - 2 * y * w,
               zero),
-             (2*x*y - 2*z*w,
+             (2 * x * y - 2 * z * w,
               w**2 - x**2 + y**2 - z**2,
-              2*y*z + 2*x*w,
+              2 * y * z + 2 * x * w,
               zero),
-             (2*x*z + 2*y*w,
-              2*y*z - 2*x*w,
+             (2 * x * z + 2 * y * w,
+              2 * y * z - 2 * x * w,
               w**2 - x**2 - y**2 + z**2,
               zero),
              (zero, zero, zero, w**2 + x**2 + y**2 + z**2)))
 
+
 def qrotate(vector, axis, angle):
     """Rotate *vector* around *axis* by *angle* (in radians).
 
     *vector* is a matrix of column vectors, as is *axis*.
     This function uses quaternion rotation.
     """
     n_axis = axis / vnorm(axis)
-    sin_angle = np.expand_dims(sin(angle/2), 0)
-    if np.rank(n_axis)==1:
+    sin_angle = np.expand_dims(sin(angle / 2), 0)
+    if np.rank(n_axis) == 1:
         n_axis = np.expand_dims(n_axis, 1)
         p__ = np.dot(n_axis, sin_angle)[:, np.newaxis]
     else:
         p__ = n_axis * sin_angle
 
-    q__ = Quaternion(cos(angle/2), p__)
+    q__ = Quaternion(cos(angle / 2), p__)
     return np.einsum("kj, ikj->ij",
                      vector,
                      q__.rotation_matrix()[:3, :3])
 
 
-
-### DIRTY STUFF. Needed the get_lonlatalt function to work on pos directly if
-### we want to print out lonlats in the end.
+# DIRTY STUFF. Needed the get_lonlatalt function to work on pos directly if
+# we want to print out lonlats in the end.
 from pyorbital import astronomy
 from pyorbital.orbital import *
 
+
 def get_lonlatalt(pos, utc_time):
     """Calculate sublon, sublat and altitude of satellite, considering the
     earth an ellipsoid.
 
     http://celestrak.com/columns/v02n03/
     """
     (pos_x, pos_y, pos_z) = pos / XKMPER
     lon = ((np.arctan2(pos_y * XKMPER, pos_x * XKMPER) - astronomy.gmst(utc_time))
            % (2 * np.pi))
 
     lon = np.where(lon > np.pi, lon - np.pi * 2, lon)
-    lon = np.where(lon <= -np.pi, lon + np.pi *2, lon)
+    lon = np.where(lon <= -np.pi, lon + np.pi * 2, lon)
 
     r = np.sqrt(pos_x ** 2 + pos_y ** 2)
     lat = np.arctan2(pos_z, r)
     e2 = F * (2 - F)
 
     while True:
         lat2 = lat
-        c = 1/(np.sqrt(1 - e2 * (np.sin(lat2) ** 2)))
-        lat = np.arctan2(pos_z + c * e2 *np.sin(lat2), r)
+        c = 1 / (np.sqrt(1 - e2 * (np.sin(lat2) ** 2)))
+        lat = np.arctan2(pos_z + c * e2 * np.sin(lat2), r)
         if np.all(abs(lat - lat2) < 1e-10):
             break
-    alt = r / np.cos(lat)- c
+    alt = r / np.cos(lat) - c
     alt *= A
     return np.rad2deg(lon), np.rad2deg(lat), alt
 
-### END OF DIRTY STUFF
+# END OF DIRTY STUFF
+
+
 def compute_pixels((tle1, tle2), sgeom, times, rpy=(0.0, 0.0, 0.0)):
     """Compute cartesian coordinates of the pixels in instrument scan.
     """
     orb = Orbital("mysatellite", line1=tle1, line2=tle2)
 
     # get position and velocity for each time of each pixel
     pos, vel = orb.get_position(times, normalize=False)
 
     # now, get the vectors pointing to each pixel
     vectors = sgeom.vectors(pos, vel, *rpy)
 
-    ## compute intersection of lines (directed by vectors and passing through
-    ## (0, 0, 0)) and ellipsoid. Derived from:
-    ## http://en.wikipedia.org/wiki/Line%E2%80%93sphere_intersection
-    
+    # compute intersection of lines (directed by vectors and passing through
+    # (0, 0, 0)) and ellipsoid. Derived from:
+    # http://en.wikipedia.org/wiki/Line%E2%80%93sphere_intersection
 
     # do the computation between line and ellipsoid (WGS 84)
     # NB: AAPP uses GRS 80...
     centre = -pos
-    a__ = 6378.137 # km
-    #b__ = 6356.75231414 # km, GRS80
-    b__ = 6356.752314245 # km, WGS84
-    radius = np.array([[1/a__, 1/a__, 1/b__]]).T
+    a__ = 6378.137  # km
+    # b__ = 6356.75231414 # km, GRS80
+    b__ = 6356.752314245  # km, WGS84
+    radius = np.array([[1 / a__, 1 / a__, 1 / b__]]).T
     xr_ = vectors * radius
     cr_ = centre * radius
     ldotc = np.einsum("ij,ij->j", xr_, cr_)
     lsq = np.einsum("ij,ij->j", xr_, xr_)
     csq = np.einsum("ij,ij->j", cr_, cr_)
 
     d1_ = (ldotc - np.sqrt(ldotc ** 2 - csq * lsq + lsq)) / lsq
 
-
     # return the actual pixel positions
     return vectors * d1_ - centre
 
-    
+
 def norm(v):
     return np.sqrt(np.dot(v, v.conj()))
 
+
 def mnorm(m, axis=None):
     """norm of a matrix of vectors stacked along the *axis* dimension.
     """
     if axis is None:
         axis = np.rank(m) - 1
     return np.sqrt((m**2).sum(axis))
 
+
 def vnorm(m):
     """norms of a matrix of column vectors.
     """
     return np.sqrt((m**2).sum(0))
+
+
 def hnorm(m):
     """norms of a matrix of row vectors.
     """
     return np.sqrt((m**2).sum(1))
 
 if __name__ == '__main__':
-    #NOAA 18 (from the 2011-10-12, 16:55 utc)                 
-    #1 28654U 05018A   11284.35271227  .00000478  00000-0  28778-3 0  9246
-    #2 28654  99.0096 235.8581 0014859 135.4286 224.8087 14.11526826329313
-    
-    
+    # NOAA 18 (from the 2011-10-12, 16:55 utc)
+    # 1 28654U 05018A   11284.35271227  .00000478  00000-0  28778-3 0  9246
+    # 2 28654  99.0096 235.8581 0014859 135.4286 224.8087 14.11526826329313
+
     noaa18_tle1 = "1 28654U 05018A   11284.35271227  .00000478  00000-0  28778-3 0  9246"
     noaa18_tle2 = "2 28654  99.0096 235.8581 0014859 135.4286 224.8087 14.11526826329313"
 
     from datetime import datetime
     t = datetime(2011, 10, 12, 13, 45)
 
-    ## edge and centre of an avhrr scanline
-    #sgeom = ScanGeometry([(-0.9664123687741623, 0),
+    # edge and centre of an avhrr scanline
+    # sgeom = ScanGeometry([(-0.9664123687741623, 0),
     #                      (0, 0)],
     #                     [0, 0.0, ])
-    #print compute_pixels((noaa18_tle1, noaa18_tle2), sgeom, t)
-
+    # print compute_pixels((noaa18_tle1, noaa18_tle2), sgeom, t)
 
-    ## avhrr swath
+    # avhrr swath
     scanline_nb = 1
 
     # building the avhrr angles, 2048 pixels from +55.37 to -55.37 degrees
     avhrr = np.vstack(((np.arange(2048) - 1023.5) / 1024 * np.deg2rad(-55.37),
                        np.zeros((2048,)))).transpose()
     avhrr = np.tile(avhrr, [scanline_nb, 1])
     # building the corresponding times array
```

### Comparing `pyorbital-v0.3.2/LICENSE.txt` & `pyorbital-v1.0.0/LICENSE.txt`

 * *Files identical despite different names*


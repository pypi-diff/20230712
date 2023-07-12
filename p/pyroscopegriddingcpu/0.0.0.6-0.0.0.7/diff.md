# Comparing `tmp/pyroscopegriddingcpu-0.0.0.6.tar.gz` & `tmp/pyroscopegriddingcpu-0.0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscopegriddingcpu-0.0.0.6.tar", last modified: Wed Jul 12 19:26:01 2023, max compression
+gzip compressed data, was "pyroscopegriddingcpu-0.0.0.7.tar", last modified: Wed Jul 12 19:43:35 2023, max compression
```

## Comparing `pyroscopegriddingcpu-0.0.0.6.tar` & `pyroscopegriddingcpu-0.0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 19:26:01.907537 pyroscopegriddingcpu-0.0.0.6/
--rw-rw-rw-   0        0        0     1077 2023-04-06 22:17:54.000000 pyroscopegriddingcpu-0.0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0    11069 2023-07-12 19:26:01.907537 pyroscopegriddingcpu-0.0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     9962 2023-04-06 22:20:54.000000 pyroscopegriddingcpu-0.0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 19:26:01.876289 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/
--rw-rw-rw-   0        0        0      247 2023-07-12 16:34:35.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/__init__.py
--rw-rw-rw-   0        0        0     3506 2023-07-12 16:24:51.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/fileparser.py
--rw-rw-rw-   0        0        0    10415 2023-07-12 16:27:48.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/filter_data.py
--rw-rw-rw-   0        0        0    30817 2023-07-12 16:27:22.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/grid_ncf.py
--rw-rw-rw-   0        0        0     6329 2023-07-12 19:11:53.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/gridding.py
--rw-rw-rw-   0        0        0    25955 2023-07-12 19:25:35.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/gtools.py
--rw-rw-rw-   0        0        0     9373 2023-07-12 16:33:56.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/naming_conventions.py
--rw-rw-rw-   0        0        0    13976 2023-07-12 16:33:50.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/sat_data_input.py
--rw-rw-rw-   0        0        0     6275 2023-07-12 15:44:36.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/solar_zenith.py
--rw-rw-rw-   0        0        0     5191 2023-07-12 19:12:34.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/time_conv.py
-drwxrwxrwx   0        0        0        0 2023-07-12 19:26:01.907537 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/
--rw-rw-rw-   0        0        0    11069 2023-07-12 19:26:01.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      650 2023-07-12 19:26:01.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 19:26:01.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-07-12 19:26:01.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       84 2023-07-12 19:26:01.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-12 19:26:01.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 19:26:01.907537 pyroscopegriddingcpu-0.0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1914 2023-07-12 19:25:41.000000 pyroscopegriddingcpu-0.0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:43:35.211325 pyroscopegriddingcpu-0.0.0.7/
+-rw-rw-rw-   0        0        0     1077 2023-04-06 22:17:54.000000 pyroscopegriddingcpu-0.0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0    11069 2023-07-12 19:43:35.210325 pyroscopegriddingcpu-0.0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     9962 2023-04-06 22:20:54.000000 pyroscopegriddingcpu-0.0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 19:43:35.158266 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/
+-rw-rw-rw-   0        0        0      247 2023-07-12 16:34:35.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/__init__.py
+-rw-rw-rw-   0        0        0     3506 2023-07-12 16:24:51.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/fileparser.py
+-rw-rw-rw-   0        0        0    10325 2023-07-12 19:41:52.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/filter_data.py
+-rw-rw-rw-   0        0        0    30817 2023-07-12 16:27:22.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/grid_ncf.py
+-rw-rw-rw-   0        0        0     6305 2023-07-12 19:42:57.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/gridding.py
+-rw-rw-rw-   0        0        0    25955 2023-07-12 19:25:35.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/gtools.py
+-rw-rw-rw-   0        0        0     9373 2023-07-12 16:33:56.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/naming_conventions.py
+-rw-rw-rw-   0        0        0    13976 2023-07-12 16:33:50.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/sat_data_input.py
+-rw-rw-rw-   0        0        0     6275 2023-07-12 15:44:36.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/solar_zenith.py
+-rw-rw-rw-   0        0        0     5191 2023-07-12 19:12:34.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/time_conv.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:43:35.207365 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/
+-rw-rw-rw-   0        0        0    11069 2023-07-12 19:43:34.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      650 2023-07-12 19:43:34.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 19:43:34.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-07-12 19:43:34.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       84 2023-07-12 19:43:34.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-12 19:43:34.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 19:43:35.212322 pyroscopegriddingcpu-0.0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1914 2023-07-12 19:43:27.000000 pyroscopegriddingcpu-0.0.0.7/setup.py
```

### Comparing `pyroscopegriddingcpu-0.0.0.6/LICENSE.txt` & `pyroscopegriddingcpu-0.0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.6/PKG-INFO` & `pyroscopegriddingcpu-0.0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegriddingcpu
-Version: 0.0.0.6
+Version: 0.0.0.7
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Keywords: data fusion,satellite,L2,L3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyroscopegriddingcpu-0.0.0.6/README.md` & `pyroscopegriddingcpu-0.0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/fileparser.py` & `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/filter_data.py` & `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/filter_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 def filter_data_nc(GeoID,PhyID,geo_list,phy_list, phy_nc = None):
     if geo_list is None:
        geo_list = ["latitude", "longitude"]
     if phy_list is None:
         phy_list = [] 
     
     #basic read in
-    geo = sat_data_input.read_geo_data_nc(GeoID, var_list=geo_list)
-    phy = sat_data_input.read_phy_data_nc(PhyID, GeoID, phy_list, phy_nc)
+    geo = read_geo_data_nc(GeoID, var_list=geo_list)
+    phy = read_phy_data_nc(PhyID, GeoID, phy_list, phy_nc)
     lat = []
     lon = []
     phy_vars = []
     metadata = []
     
 
     for p in range(len(phy_list)):
@@ -107,16 +107,16 @@
 def filter_data_hdf(GeoID,PhyID,geo_list,phy_list, phy_hdf = None):
     if geo_list is None:
        geo_list = ["latitude", "longitude"]
     if phy_list is None:
         phy_list = [] 
     
     #basic read in
-    geo = sat_data_input.read_geo_data_hdf(GeoID, var_list=geo_list)
-    phy = sat_data_input.read_phy_data_hdf(PhyID, GeoID, phy_list, phy_hdf)
+    geo = read_geo_data_hdf(GeoID, var_list=geo_list)
+    phy = read_phy_data_hdf(PhyID, GeoID, phy_list, phy_hdf)
     lat = []
     lon = []
     phy_vars = []
     metadata = []
 
     for p in range(len(phy_list)):
         lat1 = geo['data'][0][:,:]
@@ -192,16 +192,16 @@
 def filter_data(GeoID,PhyID,geo_list,phy_list, phy_nc = None, phy_hdf=None):
     if geo_list is None:
        geo_list = ["latitude", "longitude"]
     if phy_list is None:
         phy_list = [] 
     
     #basic read in
-    geo = sat_data_input.read_geo_data(GeoID, var_list=geo_list)
-    phy = sat_data_input.read_phy_data(PhyID, GeoID, phy_list, phy_nc, phy_hdf)
+    geo = read_geo_data(GeoID, var_list=geo_list)
+    phy = read_phy_data(PhyID, GeoID, phy_list, phy_nc, phy_hdf)
     lat = []
     lon = []
     phy_vars = []
     metadata = []
 
     for p in range(len(phy_list)):
         lat1 = geo['data'][0][:,:]
```

### Comparing `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/grid_ncf.py` & `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/grid_ncf.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/gridding.py` & `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/gridding.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,24 +109,24 @@
     indata = []
     inlat = []
     inlon = []
     
     #open files
     #append data in
     for filename in filelist:
-        L2FID,GeoID,PhyID = sat_data_input.open_file(filename)
+        L2FID,GeoID,PhyID = open_file(filename)
 
         # check for hdf files 
         if (filename.split(".")[-1] == "hdf"):
             geo_list = ['Latitude', 'Longitude']
         else:
             geo_list = ['latitude', 'longitude']
 
         # valid data points
-        lat,lon,phy_vars, metadata = filter_data.filter_data(GeoID, PhyID, geo_list, phy_list, phy_nc=phy_list, phy_hdf=phy_list)
+        lat,lon,phy_vars, metadata = filter_data_nc(GeoID, PhyID, geo_list, phy_list, phy_nc=phy_list, phy_hdf=phy_list)
         
         #append
         #indata = np.concatenate(indata, np.ndarray(phy_vars[0]).flatten()).flatten()
         #inlat = np.concatenate(inlat, np.ndarray(lat[0]).flatten()).flatten()
         #inlon = np.concatenate(inlon, np.ndarray(lon[0]).flatten()).flatten()
         
         if len(indata) == 0:
```

### Comparing `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/gtools.py` & `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/gtools.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/naming_conventions.py` & `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/sat_data_input.py` & `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/solar_zenith.py` & `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/time_conv.py` & `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/PKG-INFO` & `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegriddingcpu
-Version: 0.0.0.6
+Version: 0.0.0.7
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Keywords: data fusion,satellite,L2,L3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/SOURCES.txt` & `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.6/setup.py` & `pyroscopegriddingcpu-0.0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name = 'pyroscopegriddingcpu',         # Package name
     packages = ['pyroscopegriddingcpu'],   
-    version = '0.0.0.6',      # Initial version
+    version = '0.0.0.7',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     long_description = long_description,
     long_description_content_type='text/markdown',
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository
```


# Comparing `tmp/pyroscopegriddingcpu-0.0.0.5.tar.gz` & `tmp/pyroscopegriddingcpu-0.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscopegriddingcpu-0.0.0.5.tar", last modified: Wed Jul 12 19:19:53 2023, max compression
+gzip compressed data, was "pyroscopegriddingcpu-0.0.0.6.tar", last modified: Wed Jul 12 19:26:01 2023, max compression
```

## Comparing `pyroscopegriddingcpu-0.0.0.5.tar` & `pyroscopegriddingcpu-0.0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 19:19:53.079991 pyroscopegriddingcpu-0.0.0.5/
--rw-rw-rw-   0        0        0     1077 2023-04-06 22:17:54.000000 pyroscopegriddingcpu-0.0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0    11069 2023-07-12 19:19:53.079991 pyroscopegriddingcpu-0.0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     9962 2023-04-06 22:20:54.000000 pyroscopegriddingcpu-0.0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 19:19:53.033123 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/
--rw-rw-rw-   0        0        0      247 2023-07-12 16:34:35.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/__init__.py
--rw-rw-rw-   0        0        0     3506 2023-07-12 16:24:51.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/fileparser.py
--rw-rw-rw-   0        0        0    10415 2023-07-12 16:27:48.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/filter_data.py
--rw-rw-rw-   0        0        0    30817 2023-07-12 16:27:22.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/grid_ncf.py
--rw-rw-rw-   0        0        0     6329 2023-07-12 19:11:53.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/gridding.py
--rw-rw-rw-   0        0        0    26404 2023-07-12 19:19:46.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/gtools.py
--rw-rw-rw-   0        0        0     9373 2023-07-12 16:33:56.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/naming_conventions.py
--rw-rw-rw-   0        0        0    13976 2023-07-12 16:33:50.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/sat_data_input.py
--rw-rw-rw-   0        0        0     6275 2023-07-12 15:44:36.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/solar_zenith.py
--rw-rw-rw-   0        0        0     5191 2023-07-12 19:12:34.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/time_conv.py
-drwxrwxrwx   0        0        0        0 2023-07-12 19:19:53.064370 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu.egg-info/
--rw-rw-rw-   0        0        0    11069 2023-07-12 19:19:52.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      650 2023-07-12 19:19:52.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 19:19:52.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-07-12 19:19:52.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       84 2023-07-12 19:19:52.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-12 19:19:52.000000 pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 19:19:53.079991 pyroscopegriddingcpu-0.0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1914 2023-07-12 19:19:28.000000 pyroscopegriddingcpu-0.0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:26:01.907537 pyroscopegriddingcpu-0.0.0.6/
+-rw-rw-rw-   0        0        0     1077 2023-04-06 22:17:54.000000 pyroscopegriddingcpu-0.0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0    11069 2023-07-12 19:26:01.907537 pyroscopegriddingcpu-0.0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9962 2023-04-06 22:20:54.000000 pyroscopegriddingcpu-0.0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 19:26:01.876289 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/
+-rw-rw-rw-   0        0        0      247 2023-07-12 16:34:35.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/__init__.py
+-rw-rw-rw-   0        0        0     3506 2023-07-12 16:24:51.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/fileparser.py
+-rw-rw-rw-   0        0        0    10415 2023-07-12 16:27:48.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/filter_data.py
+-rw-rw-rw-   0        0        0    30817 2023-07-12 16:27:22.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/grid_ncf.py
+-rw-rw-rw-   0        0        0     6329 2023-07-12 19:11:53.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/gridding.py
+-rw-rw-rw-   0        0        0    25955 2023-07-12 19:25:35.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/gtools.py
+-rw-rw-rw-   0        0        0     9373 2023-07-12 16:33:56.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/naming_conventions.py
+-rw-rw-rw-   0        0        0    13976 2023-07-12 16:33:50.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/sat_data_input.py
+-rw-rw-rw-   0        0        0     6275 2023-07-12 15:44:36.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/solar_zenith.py
+-rw-rw-rw-   0        0        0     5191 2023-07-12 19:12:34.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/time_conv.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:26:01.907537 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/
+-rw-rw-rw-   0        0        0    11069 2023-07-12 19:26:01.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      650 2023-07-12 19:26:01.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 19:26:01.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-07-12 19:26:01.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       84 2023-07-12 19:26:01.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-12 19:26:01.000000 pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 19:26:01.907537 pyroscopegriddingcpu-0.0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1914 2023-07-12 19:25:41.000000 pyroscopegriddingcpu-0.0.0.6/setup.py
```

### Comparing `pyroscopegriddingcpu-0.0.0.5/LICENSE.txt` & `pyroscopegriddingcpu-0.0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.5/PKG-INFO` & `pyroscopegriddingcpu-0.0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegriddingcpu
-Version: 0.0.0.5
+Version: 0.0.0.6
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Keywords: data fusion,satellite,L2,L3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyroscopegriddingcpu-0.0.0.5/README.md` & `pyroscopegriddingcpu-0.0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/fileparser.py` & `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/filter_data.py` & `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/grid_ncf.py` & `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/grid_ncf.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/gridding.py` & `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/gtools.py` & `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/gtools.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,19 +135,19 @@
 """
 #gridNC_time(limit, gsize, indata, inlat, inlon, 1, phy_list, geo_list, sat_files[:10], fpath + "viirs_time_compv1.nc")
 def netCDF_multi(filelist, geo_list, phy_list, output):
     geo_list = geo_list.split(" ")
     print(geo_list)
     phy_list = phy_list.split(" ")
     print(phy_list)
-    filelist = fileparser.read_file_sat_data(filelist)
+    filelist = read_file_sat_data(filelist)
 
     print(filelist)
 
-    lat,lon,phy_vars = gridding.multi_sensor_grid_data(filelist, phy_list, geo_list)
+    lat,lon,phy_vars = multi_sensor_grid_data(filelist, phy_list, geo_list)
 
     print(lat)
     print(lon)
     print(phy_vars)
 
     #grid parameters
     limit = [min(lat), max(lat), min(lon),  max(lon)]
@@ -167,22 +167,22 @@
 def netCDF_multi_time(filelist, gsize, geo_list, phy_list, output, time_interval, time_start, time_end):
     start_timer = time.time()
 
     geo_list = geo_list.split(" ")
     print(geo_list)
     phy_list = phy_list.split(" ")
     print(phy_list)
-    filelist = fileparser.read_file_sat_data(filelist)
+    filelist = read_file_sat_data(filelist)
 
-    start = time_conv.to_datetime(time_start)
-    end = time_conv.to_datetime(time_end)
+    start = to_datetime(time_start)
+    end = to_datetime(time_end)
 
-    split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
+    split_files = split_filetimes(filelist, start, end, int(time_interval))
 
-    lat,lon,phy_vars = gridding.multi_sensor_grid_data(filelist, phy_list, geo_list)
+    lat,lon,phy_vars = multi_sensor_grid_data(filelist, phy_list, geo_list)
     #grid parameters
     limit = [min(lat), max(lat), min(lon),  max(lon)]
     gsize = float(gsize)
     indata = phy_vars
     inlat=lat
     inlon = lon
 
@@ -196,20 +196,20 @@
     start_timer = time.time()
     
     geo_list = geo_list.split(" ")
     print(geo_list)
     phy_list = phy_list.split(" ")
     print(phy_list)
     limit = [float(item) for item in limit.split(" ")]
-    filelist = fileparser.read_file_sat_data(filelist)
+    filelist = read_file_sat_data(filelist)
 
-    start = time_conv.to_datetime(time_start)
-    end = time_conv.to_datetime(time_end)
+    start = to_datetime(time_start)
+    end = to_datetime(time_end)
 
-    split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
+    split_files = split_filetimes(filelist, start, end, int(time_interval))
 
     gsize = float(gsize)
 
     curr = start
     for f in split_files:
         name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
 
@@ -226,26 +226,26 @@
     start_timer = time.time()
 
     geo_list = geo_list.split(" ")
     print(geo_list)
     phy_list = phy_list.split(" ")
     print(phy_list)
     limit = [float(item) for item in limit.split(" ")]
-    filelist = fileparser.read_file_sat_data(filelist)
+    filelist = read_file_sat_data(filelist)
 
-    start = time_conv.to_datetime(time_start)
-    end = time_conv.to_datetime(time_end)
+    start = to_datetime(time_start)
+    end = to_datetime(time_end)
 
     # [[filenames for a time interval] , [], []]
-    split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
+    split_files = split_filetimes(filelist, start, end, int(time_interval))
     
     # [{sensor: array of filenames}, {}, {}, {}, {}]
     # code should record bugs - always six sensors available
     # code should report that modis is not available
-    split_files = time_conv.split_filenames(split_files)
+    split_files = split_filenames(split_files)
 
     gsize = float(gsize)
 
     curr = start
     for f in split_files:
         name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
 
@@ -262,26 +262,26 @@
     start_timer = time.time()
 
     geo_list = geo_list.split(" ")
     print(geo_list)
     phy_list = phy_list.split(" ")
     print(phy_list)
     limit = [float(item) for item in limit.split(" ")]
-    filelist = fileparser.read_file_sat_data(filelist)
+    filelist = read_file_sat_data(filelist)
 
-    start = time_conv.to_datetime(time_start)
-    end = time_conv.to_datetime(time_end)
+    start = to_datetime(time_start)
+    end = to_datetime(time_end)
 
     # [[filenames for a time interval] , [], []]
-    split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
+    split_files = split_filetimes(filelist, start, end, int(time_interval))
     
     # [{sensor: array of filenames}, {}, {}, {}, {}]
     # code should record bugs - always six sensors available
     # code should report that modis is not available
-    split_files = time_conv.split_filenames(split_files)
+    split_files = split_filenames(split_files)
 
     gsize = float(gsize)
 
     curr = start
     for f in split_files:
         name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
         #print(f)
@@ -294,163 +294,163 @@
 
     end_timer = time.time()
     print("Full execution time: ", end_timer - start_timer)
 
 # output - folder location
 def netCDF_yaml_config(file_name):
 
-    grid_settings, variables, file_io = fileparser.read_config(file_name)
+    grid_settings, variables, file_io = read_config(file_name)
 
     start_timer = time.time()
 
     geo_list = variables["geo_var"]
     phy_list = variables["phy_var"]
     phy_nc = variables["phy_var_nc"]
     phy_hdf = variables["phy_var_hdf"]
     limit = grid_settings["limit"]
     pixel_range = variables["pixel_range"]
     
     # list of file paths for specific files to read
     if file_io["file_directory_folder"] == "NA":
         if file_io["file_location_folder"] == "NA":
-            filelist = fileparser.read_file_sat_data(file_io["file_location_file"])
+            filelist = read_file_sat_data(file_io["file_location_file"])
         else:
-            filelist = fileparser.read_folder_sat_data(file_io["file_location_folder"])
+            filelist = read_folder_sat_data(file_io["file_location_folder"])
     else:
-        filelist = fileparser.read_directory_sat_data(file_io["file_directory_folder"])
+        filelist = read_directory_sat_data(file_io["file_directory_folder"])
         
         
     #static file for Land_Sea_Mask and Topographic_Altitude
     static_file = file_io["static_file"]
     print("static file:", static_file)
 
     time_start = grid_settings["time_start"]
     time_end = grid_settings["time_end"]
-    start = time_conv.to_datetime(time_start)
-    end = time_conv.to_datetime(time_end)
+    start = to_datetime(time_start)
+    end = to_datetime(time_end)
 
     # [[filenames for a time interval] , [], []]
     time_interval = grid_settings["time_interval"]
-    split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
+    split_files = split_filetimes(filelist, start, end, int(time_interval))
     
     # [{sensor: array of filenames}, {}, {}, {}, {}]
     # code should record bugs - always six sensors available
     # code should report that modis is not available
-    split_files = time_conv.split_filenames(split_files)
+    split_files = split_filenames(split_files)
 
     gsize = float(grid_settings["gridsize"])
 
     curr = start
     outputfolder = file_io["output_location"]
     outputname = file_io["output_name"]
     
     count= 0
     for f in split_files:
         #name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
         #XAERDT_L3_MEASURES_QD_HH.YYYYMMDD.HHMM.V0.ProcessingDate.nc
         time_string = str(curr).replace(":", "").replace("-", "").replace(" ", "")
         time_string = time_string[:8] + '.' + time_string[8:-2]
-        processing_date = time_conv.sys_time()
+        processing_date = sys_time()
         name = outputfolder + "XAERDT_L3_MEASURES_QD_HH." + time_string+ ".V0." +processing_date+ ".nc"
         
         #print(f) f = dict (key: sensor, values: array of filelocs)
         # print(split_files)
         
         #print("\n\nNAME:", name)
         #print("\n\TIME STRING:", curr)
         #print("\n\PROCESS DATE:", time_interval)
         
         # grid files
         #grid_nc_sensor_statistics_metadata
         
-        ds = grid_ncf.grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, curr, time_interval, phy_nc, phy_hdf, static_file, pixel_range)
+        ds = grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, curr, time_interval, phy_nc, phy_hdf, static_file, pixel_range)
         ds.close()
         curr = curr + datetime.timedelta(minutes = int(time_interval))
 
     end_timer = time.time()
     print("Full execution time: ", end_timer - start_timer)
     
 # output - folder location
 def netCDF_yaml_config_time(file_name, time_start, time_end):
 
-    grid_settings, variables, file_io = fileparser.read_config(file_name)
+    grid_settings, variables, file_io = read_config(file_name)
 
     start_timer = time.time()
 
     geo_list = variables["geo_var"]
     phy_list = variables["phy_var"]
     phy_nc = variables["phy_var_nc"]
     phy_hdf = variables["phy_var_hdf"]
     limit = grid_settings["limit"]
     pixel_range = variables["pixel_range"]
     
     # list of file paths for specific files to read
     if file_io["file_directory_folder"] == "NA":
         if file_io["file_location_folder"] == "NA":
-            filelist = fileparser.read_file_sat_data(file_io["file_location_file"])
+            filelist = read_file_sat_data(file_io["file_location_file"])
         else:
-            filelist = fileparser.read_folder_sat_data(file_io["file_location_folder"])
+            filelist = read_folder_sat_data(file_io["file_location_folder"])
     else:
-        filelist = fileparser.read_directory_sat_data(file_io["file_directory_folder"])
+        filelist = read_directory_sat_data(file_io["file_directory_folder"])
         
     print("FILELIST: ", filelist)
     #static file for Land_Sea_Mask and Topographic_Altitude
     static_file = file_io["static_file"]
     print("static file:", static_file)
 
     #time_start = grid_settings["time_start"]
     #time_end = grid_settings["time_end"]
-    start = time_conv.to_datetime(time_start)
-    end = time_conv.to_datetime(time_end)
+    start = to_datetime(time_start)
+    end = to_datetime(time_end)
     
 
     # [[filenames for a time interval] , [], []]
     time_interval = grid_settings["time_interval"]
-    split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
+    split_files = split_filetimes(filelist, start, end, int(time_interval))
     
     # [{sensor: array of filenames}, {}, {}, {}, {}]
     # code should record bugs - always six sensors available
     # code should report that modis is not available
-    split_files = time_conv.split_filenames(split_files)
+    split_files = split_filenames(split_files)
 
     gsize = float(grid_settings["gridsize"])
 
     curr = start
     outputfolder = file_io["output_location"]
     outputname = file_io["output_name"]
     
     count= 0
     for f in split_files:
         #name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
         #XAERDT_L3_MEASURES_QD_HH.YYYYMMDD.HHMM.V0.ProcessingDate.nc
         time_string = str(curr).replace(":", "").replace("-", "").replace(" ", "")
         time_string = time_string[:8] + '.' + time_string[8:-2]
-        processing_date = time_conv.sys_time()
+        processing_date = sys_time()
         name = outputfolder + "XAERDT_L3_MEASURES_QD_HH." + time_string+ ".V0." +processing_date+ ".nc"
         
-        ds = grid_ncf.grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, curr, time_interval, phy_nc, phy_hdf, static_file, pixel_range)
+        ds = grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, curr, time_interval, phy_nc, phy_hdf, static_file, pixel_range)
         ds.close()
         curr = curr + datetime.timedelta(minutes = int(time_interval))
 
     end_timer = time.time()
     print("Full execution time: ", end_timer - start_timer)
 
     
 
 def execute_file(filename):
-    filelist, gsize, time_interval, start, end, output, geo_list, phy_list = fileparser.read_in_commands(filename)
-    lat,lon,phy_vars = gridding.multi_sensor_grid_data(filelist, phy_list, geo_list)
+    filelist, gsize, time_interval, start, end, output, geo_list, phy_list = read_in_commands(filename)
+    lat,lon,phy_vars = multi_sensor_grid_data(filelist, phy_list, geo_list)
     #grid parameters
     limit = [min(lat), max(lat), min(lon),  max(lon)]
     gsize = float(gsize)
     indata = phy_vars
     inlat=lat
     inlon = lon
 
-    split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
+    split_files = split_filetimes(filelist, start, end, int(time_interval))
 
     #grid_ncf.grid_nc_mult_files_time(limit, gsize, indata, inlat, inlon, phy_list, geo_list, split_files, output)
 
 
 
 def control():
     # parser object
```

### Comparing `pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/naming_conventions.py` & `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/sat_data_input.py` & `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/solar_zenith.py` & `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu/time_conv.py` & `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu.egg-info/PKG-INFO` & `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegriddingcpu
-Version: 0.0.0.5
+Version: 0.0.0.6
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Keywords: data fusion,satellite,L2,L3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyroscopegriddingcpu-0.0.0.5/pyroscopegriddingcpu.egg-info/SOURCES.txt` & `pyroscopegriddingcpu-0.0.0.6/pyroscopegriddingcpu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.5/setup.py` & `pyroscopegriddingcpu-0.0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name = 'pyroscopegriddingcpu',         # Package name
     packages = ['pyroscopegriddingcpu'],   
-    version = '0.0.0.5',      # Initial version
+    version = '0.0.0.6',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     long_description = long_description,
     long_description_content_type='text/markdown',
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository
```


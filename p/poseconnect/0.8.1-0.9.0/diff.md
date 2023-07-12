# Comparing `tmp/poseconnect-0.8.1.tar.gz` & `tmp/poseconnect-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poseconnect-0.8.1.tar", last modified: Tue Mar 29 21:15:40 2022, max compression
+gzip compressed data, was "poseconnect-0.9.0.tar", last modified: Tue May 17 21:53:03 2022, max compression
```

## Comparing `poseconnect-0.8.1.tar` & `poseconnect-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 tcquinn   (1000) tcquinn   (1000)        0 2022-03-29 21:15:40.299557 poseconnect-0.8.1/
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)       18 2021-06-21 20:15:13.000000 poseconnect-0.8.1/MANIFEST.in
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)     2999 2022-03-29 21:15:40.299557 poseconnect-0.8.1/PKG-INFO
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)     2087 2022-01-02 22:59:40.000000 poseconnect-0.8.1/README.md
-drwxrwxr-x   0 tcquinn   (1000) tcquinn   (1000)        0 2022-03-29 21:15:40.299557 poseconnect-0.8.1/poseconnect/
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)      263 2022-03-29 21:15:08.000000 poseconnect-0.8.1/poseconnect/__init__.py
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    31265 2022-03-12 17:19:22.000000 poseconnect-0.8.1/poseconnect/cli.py
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)     3747 2022-03-12 17:19:22.000000 poseconnect-0.8.1/poseconnect/defaults.py
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    14957 2021-07-05 15:18:47.000000 poseconnect-0.8.1/poseconnect/filter.py
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    14275 2021-07-07 01:20:34.000000 poseconnect-0.8.1/poseconnect/identify.py
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    44736 2022-03-29 21:02:54.000000 poseconnect-0.8.1/poseconnect/overlay.py
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    51450 2022-03-29 21:10:57.000000 poseconnect-0.8.1/poseconnect/reconstruct.py
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    26583 2022-02-22 02:58:04.000000 poseconnect-0.8.1/poseconnect/track.py
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    20105 2022-03-12 17:19:22.000000 poseconnect-0.8.1/poseconnect/utils.py
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    31936 2022-01-02 22:59:40.000000 poseconnect-0.8.1/poseconnect/visualize.py
-drwxrwxr-x   0 tcquinn   (1000) tcquinn   (1000)        0 2022-03-29 21:15:40.299557 poseconnect-0.8.1/poseconnect.egg-info/
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)     2999 2022-03-29 21:15:40.000000 poseconnect-0.8.1/poseconnect.egg-info/PKG-INFO
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)      472 2022-03-29 21:15:40.000000 poseconnect-0.8.1/poseconnect.egg-info/SOURCES.txt
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)        1 2022-03-29 21:15:40.000000 poseconnect-0.8.1/poseconnect.egg-info/dependency_links.txt
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)       53 2022-03-29 21:15:40.000000 poseconnect-0.8.1/poseconnect.egg-info/entry_points.txt
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)      185 2022-03-29 21:15:40.000000 poseconnect-0.8.1/poseconnect.egg-info/requires.txt
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)       12 2022-03-29 21:15:40.000000 poseconnect-0.8.1/poseconnect.egg-info/top_level.txt
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)       38 2022-03-29 21:15:40.299557 poseconnect-0.8.1/setup.cfg
--rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)     1849 2022-01-02 22:59:40.000000 poseconnect-0.8.1/setup.py
+drwxrwxr-x   0 tcquinn   (1000) tcquinn   (1000)        0 2022-05-17 21:53:03.758501 poseconnect-0.9.0/
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)       18 2021-06-21 20:15:13.000000 poseconnect-0.9.0/MANIFEST.in
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)     2999 2022-05-17 21:53:03.754501 poseconnect-0.9.0/PKG-INFO
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)     2087 2022-01-02 22:59:40.000000 poseconnect-0.9.0/README.md
+drwxrwxr-x   0 tcquinn   (1000) tcquinn   (1000)        0 2022-05-17 21:53:03.754501 poseconnect-0.9.0/poseconnect/
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)      263 2022-05-17 21:51:47.000000 poseconnect-0.9.0/poseconnect/__init__.py
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    31265 2022-03-12 17:19:22.000000 poseconnect-0.9.0/poseconnect/cli.py
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)     3747 2022-03-12 17:19:22.000000 poseconnect-0.9.0/poseconnect/defaults.py
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    14957 2021-07-05 15:18:47.000000 poseconnect-0.9.0/poseconnect/filter.py
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    14275 2021-07-07 01:20:34.000000 poseconnect-0.9.0/poseconnect/identify.py
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    44736 2022-05-06 18:08:42.000000 poseconnect-0.9.0/poseconnect/overlay.py
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    51450 2022-05-06 18:08:42.000000 poseconnect-0.9.0/poseconnect/reconstruct.py
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    26583 2022-02-22 02:58:04.000000 poseconnect-0.9.0/poseconnect/track.py
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    20766 2022-05-06 18:20:45.000000 poseconnect-0.9.0/poseconnect/utils.py
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)    31936 2022-01-02 22:59:40.000000 poseconnect-0.9.0/poseconnect/visualize.py
+drwxrwxr-x   0 tcquinn   (1000) tcquinn   (1000)        0 2022-05-17 21:53:03.754501 poseconnect-0.9.0/poseconnect.egg-info/
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)     2999 2022-05-17 21:53:03.000000 poseconnect-0.9.0/poseconnect.egg-info/PKG-INFO
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)      472 2022-05-17 21:53:03.000000 poseconnect-0.9.0/poseconnect.egg-info/SOURCES.txt
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)        1 2022-05-17 21:53:03.000000 poseconnect-0.9.0/poseconnect.egg-info/dependency_links.txt
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)       53 2022-05-17 21:53:03.000000 poseconnect-0.9.0/poseconnect.egg-info/entry_points.txt
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)      185 2022-05-17 21:53:03.000000 poseconnect-0.9.0/poseconnect.egg-info/requires.txt
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)       12 2022-05-17 21:53:03.000000 poseconnect-0.9.0/poseconnect.egg-info/top_level.txt
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)       38 2022-05-17 21:53:03.758501 poseconnect-0.9.0/setup.cfg
+-rw-rw-r--   0 tcquinn   (1000) tcquinn   (1000)     1849 2022-01-02 22:59:40.000000 poseconnect-0.9.0/setup.py
```

### Comparing `poseconnect-0.8.1/PKG-INFO` & `poseconnect-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poseconnect
-Version: 0.8.1
+Version: 0.9.0
 Summary: Tools for constructing 3D pose tracks from multi-camera 2D poses
 Home-page: https://github.com/WildflowerSchools/poseconnect
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 License: UNKNOWN
 Description: # poseconnect
```

### Comparing `poseconnect-0.8.1/README.md` & `poseconnect-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `poseconnect-0.8.1/poseconnect/cli.py` & `poseconnect-0.9.0/poseconnect/cli.py`

 * *Files identical despite different names*

### Comparing `poseconnect-0.8.1/poseconnect/defaults.py` & `poseconnect-0.9.0/poseconnect/defaults.py`

 * *Files identical despite different names*

### Comparing `poseconnect-0.8.1/poseconnect/filter.py` & `poseconnect-0.9.0/poseconnect/filter.py`

 * *Files identical despite different names*

### Comparing `poseconnect-0.8.1/poseconnect/identify.py` & `poseconnect-0.9.0/poseconnect/identify.py`

 * *Files identical despite different names*

### Comparing `poseconnect-0.8.1/poseconnect/overlay.py` & `poseconnect-0.9.0/poseconnect/overlay.py`

 * *Files identical despite different names*

### Comparing `poseconnect-0.8.1/poseconnect/reconstruct.py` & `poseconnect-0.9.0/poseconnect/reconstruct.py`

 * *Files identical despite different names*

### Comparing `poseconnect-0.8.1/poseconnect/track.py` & `poseconnect-0.9.0/poseconnect/track.py`

 * *Files identical despite different names*

### Comparing `poseconnect-0.8.1/poseconnect/utils.py` & `poseconnect-0.9.0/poseconnect/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,23 @@
             pose_type
         ))
     df['timestamp'] = pd.to_datetime(df['timestamp'], utc=True)
     if 'camera_id' in all_column_names:
         df['camera_id'] = df['camera_id'].astype('object')
     if 'keypoint_coordinates_2d' in all_column_names:
         df['keypoint_coordinates_2d'] = df['keypoint_coordinates_2d'].apply(convert_to_array)
+        df['keypoint_coordinates_2d'] = df['keypoint_coordinates_2d'].apply(remove_zeroes)
     if 'keypoint_quality_2d' in all_column_names:
         df['keypoint_quality_2d'] = df['keypoint_quality_2d'].apply(convert_to_array)
+        df['keypoint_quality_2d'] = df['keypoint_quality_2d'].apply(remove_zeroes)
     if 'pose_quality_2d' in all_column_names:
         df['pose_quality_2d'] = pd.to_numeric(df['pose_quality_2d']).astype('float')
     if 'keypoint_coordinates_3d' in all_column_names:
         df['keypoint_coordinates_3d'] = df['keypoint_coordinates_3d'].apply(convert_to_array)
+        df['keypoint_coordinates_3d'] = df['keypoint_coordinates_3d'].apply(remove_zeroes)
     if 'pose_2d_ids' in all_column_names:
         df['pose_2d_ids'] = df['pose_2d_ids'].apply(convert_to_list)
     return df
 
 def ingest_poses_2d(data_object):
     df = convert_to_df(data_object)
     df = set_index_columns(
@@ -57,15 +60,17 @@
         raise ValueError('Data is missing fields: {}'.format(
             set(target_columns) - set(df.columns)
         ))
     df = df.reindex(columns=target_columns)
     df['timestamp'] = pd.to_datetime(df['timestamp'], utc=True)
     df['camera_id'] = df['camera_id'].astype('object')
     df['keypoint_coordinates_2d'] = df['keypoint_coordinates_2d'].apply(convert_to_array)
+    df['keypoint_coordinates_2d'] = df['keypoint_coordinates_2d'].apply(remove_zeroes)
     df['keypoint_quality_2d'] = df['keypoint_quality_2d'].apply(convert_to_array)
+    df['keypoint_quality_2d'] = df['keypoint_quality_2d'].apply(remove_zeroes)
     df['pose_quality_2d'] = pd.to_numeric(df['pose_quality_2d']).astype('float')
     return df
 
 def ingest_camera_calibrations(data_object):
     df = convert_to_df(data_object)
     df = set_index_columns(
         df=df,
@@ -113,14 +118,15 @@
     if not set(target_columns).issubset(set(df.columns)):
         raise ValueError('Data is missing fields: {}'.format(
             set(target_columns) - set(df.columns)
         ))
     df = df.reindex(columns=target_columns)
     df['timestamp'] = pd.to_datetime(df['timestamp'], utc=True)
     df['keypoint_coordinates_3d'] = df['keypoint_coordinates_3d'].apply(convert_to_array)
+    df['keypoint_coordinates_3d'] = df['keypoint_coordinates_3d'].apply(remove_zeroes)
     df['pose_2d_ids'] = df['pose_2d_ids'].apply(convert_to_list)
     return df
 
 def output_poses_3d(df, path):
     df['timestamp'] = pd.to_datetime(df['timestamp'], utc=True)
     file_extension = os.path.splitext(path)[1]
     if len(file_extension) == 0:
@@ -485,7 +491,11 @@
                 pass
     equality_df = pd.DataFrame.from_dict(equality_dict, orient='index')
     is_equal = np.all(equality_df)
     return is_equal, equality_df
 
 def convert_to_datetime_utc(datetime_object):
     return pd.to_datetime(datetime_object, utc=True).to_pydatetime()
+
+def remove_zeroes(array_object):
+    array_object_output = np.where(array_object == 0.0, np.nan, array_object)
+    return array_object_output
```

### Comparing `poseconnect-0.8.1/poseconnect/visualize.py` & `poseconnect-0.9.0/poseconnect/visualize.py`

 * *Files identical despite different names*

### Comparing `poseconnect-0.8.1/poseconnect.egg-info/PKG-INFO` & `poseconnect-0.9.0/poseconnect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poseconnect
-Version: 0.8.1
+Version: 0.9.0
 Summary: Tools for constructing 3D pose tracks from multi-camera 2D poses
 Home-page: https://github.com/WildflowerSchools/poseconnect
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 License: UNKNOWN
 Description: # poseconnect
```

### Comparing `poseconnect-0.8.1/setup.py` & `poseconnect-0.9.0/setup.py`

 * *Files identical despite different names*


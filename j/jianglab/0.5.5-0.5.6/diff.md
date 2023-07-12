# Comparing `tmp/jianglab-0.5.5.tar.gz` & `tmp/jianglab-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.5.5.tar", last modified: Mon Jul 10 18:24:02 2023, max compression
+gzip compressed data, was "jianglab-0.5.6.tar", last modified: Wed Jul 12 19:27:23 2023, max compression
```

## Comparing `jianglab-0.5.5.tar` & `jianglab-0.5.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 18:24:02.592613 jianglab-0.5.5/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-10 18:24:02.592280 jianglab-0.5.5/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.5.5/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 18:24:02.588593 jianglab-0.5.5/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.5.5/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    29067 2023-07-10 18:23:12.000000 jianglab-0.5.5/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.5.5/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 18:24:02.591627 jianglab-0.5.5/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-10 18:24:02.000000 jianglab-0.5.5/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-10 18:24:02.000000 jianglab-0.5.5/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-10 18:24:02.000000 jianglab-0.5.5/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      111 2023-07-10 18:24:02.000000 jianglab-0.5.5/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-10 18:24:02.000000 jianglab-0.5.5/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-10 18:24:02.592741 jianglab-0.5.5/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1038 2023-07-10 18:23:20.000000 jianglab-0.5.5/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-12 19:27:23.356721 jianglab-0.5.6/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-12 19:27:23.356193 jianglab-0.5.6/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1172 2023-07-12 19:22:38.000000 jianglab-0.5.6/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-12 19:27:23.352324 jianglab-0.5.6/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.5.6/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    30559 2023-07-12 19:27:19.000000 jianglab-0.5.6/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.5.6/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-12 19:27:23.355279 jianglab-0.5.6/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-12 19:27:23.000000 jianglab-0.5.6/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-12 19:27:23.000000 jianglab-0.5.6/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-12 19:27:23.000000 jianglab-0.5.6/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      111 2023-07-12 19:27:23.000000 jianglab-0.5.6/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-12 19:27:23.000000 jianglab-0.5.6/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-12 19:27:23.357118 jianglab-0.5.6/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1038 2023-07-12 19:27:11.000000 jianglab-0.5.6/setup.py
```

### Comparing `jianglab-0.5.5/PKG-INFO` & `jianglab-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.5.5
+Version: 0.5.6
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.5.5/README.md` & `jianglab-0.5.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -36,7 +36,14 @@
 
 ```bash
 twine upload dist/*
 
 ```
 Since the version number has been incremented, you should not encounter the "file already exists" error, and your package should be uploaded successfully. Users can now install the new version of your package using pip.
 
+
+
+To use video output. 
+```bash
+pip install PyQt5
+conda install -c conda-forge ffmpeg
+```
```

### Comparing `jianglab-0.5.5/jianglab/common_functions.py` & `jianglab-0.5.6/jianglab/common_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import scipy.signal as signal
 from tqdm import tqdm
 import pickle
 import cv2
 import xmltodict
 import matplotlib.animation as animation
 from IPython.display import HTML
+import matplotlib
 
 
 def frame_ref_to_onset(frame_ref, first_onset_index = 184, visualize_window = (250_000,350_000), stimulus_interval = 60, on_duration = 30, sampling_rate = 20000,overlay_split_num = 5):
     '''
         Convert frame_ref to onset_index
         input:
             frame_ref: 2d array, first row is the light, second row is the frame
@@ -294,14 +295,26 @@
         # total resample 1000 result in 20 Hz acq rate
         # 30 mins processing time for 10 mins data
     np_array = raw_cmcr_data.Acquisition.Sensor_Data.SensorData_1_1
     images = np_array[::pre_resample_rate]
     images = resample_med(images, kernel_size= kernel_size, resample_rate = post_resample_rate) 
     return images
 
+def get_lowpass_data_from_file_path(cmcr_file_path,
+                                    pre_resample_rate = 100,
+                                    post_resample_rate = 10,
+                                    kernel_size = 51,
+                                    save_data = False):
+    raw_cmcr_data = load_raw_data(cmcr_file_path)
+    lowpass_data = get_lowpass_data(raw_cmcr_data, pre_resample_rate=pre_resample_rate,\
+                                     post_resample_rate=post_resample_rate, \
+                                        kernel_size=kernel_size)
+    if save_data:
+        save_instance(cmcr_file_path[:-5]+"_lp.npy", lowpass_data)
+    return lowpass_data
 
 def remove_bad_lanes(data, bad_lanes): # for low pass filtered data
     if len(bad_lanes) != 0:
         data = np.delete(data, [int(lane)-1 for lane in bad_lanes], axis= 2)
     else:
         pass
     return data
@@ -629,21 +642,22 @@
 
     # Place the second image onto the canvas, shifted by the specified amount
     stitched[shift_y : shift_y + img2.shape[0], shift_x : shift_x + img2.shape[1]] = img2
 
     return stitched
 
 
-def array_to_video(np_array, filename, frame_rate = 30.0, save_to_avi = True, display_inline = True, color_map = 'jet'):
+def array_to_video_old(np_array, filename, frame_rate = 30.0, save_to_avi = True, display_inline = True, color_map = 'jet'):
     """
     Converts a 3D numpy array to a video file and displays it in the notebook.
     :param np_array: 3D numpy array
     :param filename: Name of the video file to be saved
     :param save_to_avi: If True, saves the video to an AVI file
     :param color_map: Color map to be used for the video
+    :param frame_rate: Frame rate of the video
     """
 
     # Ensure the array is 3D
     if len(np_array.shape) != 3:
         raise ValueError("Array must be 3-dimensional")
 
     # Define the codec and create a VideoWriter object
@@ -669,7 +683,33 @@
     if save_to_avi:
         for i in range(np_array.shape[0]):
             frame = np_array[i].astype('uint8')  # Ensure data type is uint8
             out.write(cv2.cvtColor(frame, cv2.COLOR_GRAY2BGR))  # OpenCV uses BGR color space
 
     # Close the video file
     out.release()
+
+
+def array_to_video(data, filename, min = 0, max =1, cmap = "jet", save_to_avi = True):
+    """
+    data: 3D numpy array
+    filename: Name of the video file to be saved
+    save_to_avi: If True, saves the video to an AVI file
+    color_map: Color map to be used for the video
+    """
+    matplotlib.rcParams['animation.embed_limit'] = 2**128
+    
+    fig, axs = plt.subplots()
+    im0 = axs.imshow(data[0], vmin = min, vmax =max, cmap = cmap )
+
+    def init():
+        im0.set_data(data[0])
+
+    def animate(i):
+        im0.set_data(data[i])
+
+        return im0
+
+    anim = animation.FuncAnimation(fig, animate, init_func=init, frames=data.shape[0], repeat = True)
+    if save_to_avi:
+        anim.save(filename)
+    return HTML(anim.to_jshtml())
```

### Comparing `jianglab-0.5.5/jianglab.egg-info/PKG-INFO` & `jianglab-0.5.6/jianglab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.5.5
+Version: 0.5.6
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.5.5/setup.py` & `jianglab-0.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.5.5',
+    version='0.5.6',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```


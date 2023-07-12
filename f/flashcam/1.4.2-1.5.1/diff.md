# Comparing `tmp/flashcam-1.4.2.tar.gz` & `tmp/flashcam-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.4.2.tar", last modified: Thu Apr 20 12:49:38 2023, max compression
+gzip compressed data, was "flashcam-1.5.1.tar", last modified: Wed Jul 12 09:17:50 2023, max compression
```

## Comparing `flashcam-1.4.2.tar` & `flashcam-1.5.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:49:38.909970 flashcam-1.4.2/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-04-20 12:49:38.909970 flashcam-1.4.2/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-04-17 13:40:53.000000 flashcam-1.4.2/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:49:38.905970 flashcam-1.4.2/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24826 2023-04-20 12:20:29.000000 flashcam-1.4.2/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-04-06 11:29:38.000000 flashcam-1.4.2/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2023-04-06 11:29:38.000000 flashcam-1.4.2/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-06 11:48:21.000000 flashcam-1.4.2/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:49:38.905970 flashcam-1.4.2/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8079 2023-04-17 13:40:53.000000 flashcam-1.4.2/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:49:38.909970 flashcam-1.4.2/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-20 08:33:53.000000 flashcam-1.4.2/flashcam/data/win_rain.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-20 08:33:53.000000 flashcam-1.4.2/flashcam/data/win_skull.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-20 08:33:53.000000 flashcam-1.4.2/flashcam/data/win_storm.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-20 08:33:53.000000 flashcam-1.4.2/flashcam/data/win_winter.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-04-20 08:33:53.000000 flashcam-1.4.2/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    44831 2023-04-20 12:48:48.000000 flashcam-1.4.2/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-20 12:14:15.000000 flashcam-1.4.2/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)   100516 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-06 11:51:33.000000 flashcam-1.4.2/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    27417 2023-04-06 11:29:38.000000 flashcam-1.4.2/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-04-20 12:49:38.000000 flashcam-1.4.2/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30138 2023-04-20 12:48:25.000000 flashcam-1.4.2/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-20 12:49:38.909970 flashcam-1.4.2/flashcam.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-04-20 12:49:38.000000 flashcam-1.4.2/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      820 2023-04-20 12:49:38.000000 flashcam-1.4.2/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-04-20 12:49:38.000000 flashcam-1.4.2/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-04-20 12:49:38.000000 flashcam-1.4.2/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-04-20 12:49:38.000000 flashcam-1.4.2/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-04-20 12:49:38.909970 flashcam-1.4.2/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-18 08:31:29.000000 flashcam-1.4.2/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 09:17:50.111114 flashcam-1.5.1/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-07-12 09:17:50.111114 flashcam-1.5.1/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-04-17 13:40:53.000000 flashcam-1.5.1/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 09:17:50.107114 flashcam-1.5.1/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24826 2023-04-20 12:20:29.000000 flashcam-1.5.1/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-04-06 11:29:38.000000 flashcam-1.5.1/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2023-04-06 11:29:38.000000 flashcam-1.5.1/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-06 11:48:21.000000 flashcam-1.5.1/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 09:17:50.111114 flashcam-1.5.1/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8079 2023-04-17 13:40:53.000000 flashcam-1.5.1/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 09:17:50.111114 flashcam-1.5.1/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-20 08:33:53.000000 flashcam-1.5.1/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-20 08:33:53.000000 flashcam-1.5.1/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-20 08:33:53.000000 flashcam-1.5.1/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-20 08:33:53.000000 flashcam-1.5.1/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-04-20 08:33:53.000000 flashcam-1.5.1/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40421 2023-07-12 09:16:16.000000 flashcam-1.5.1/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-20 12:14:15.000000 flashcam-1.5.1/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)   100516 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/uniwrec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-06 11:51:33.000000 flashcam-1.5.1/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    27692 2023-07-12 09:16:16.000000 flashcam-1.5.1/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-07-12 09:17:49.000000 flashcam-1.5.1/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30138 2023-04-20 12:48:25.000000 flashcam-1.5.1/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 09:17:50.111114 flashcam-1.5.1/flashcam.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-07-12 09:17:50.000000 flashcam-1.5.1/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      820 2023-07-12 09:17:50.000000 flashcam-1.5.1/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-07-12 09:17:50.000000 flashcam-1.5.1/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-07-12 09:17:50.000000 flashcam-1.5.1/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-07-12 09:17:50.000000 flashcam-1.5.1/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-07-12 09:17:50.111114 flashcam-1.5.1/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-18 08:31:29.000000 flashcam-1.5.1/setup.py
```

### Comparing `flashcam-1.4.2/PKG-INFO` & `flashcam-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.4.2
+Version: 1.5.1
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.4.2/README.md` & `flashcam-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/bin/flashcam` & `flashcam-1.5.1/bin/flashcam`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/bin/flashcamg` & `flashcam-1.5.1/bin/flashcamg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/base_camera2.py` & `flashcam-1.5.1/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/config.py` & `flashcam-1.5.1/flashcam/config.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.5.1/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.5.1/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/data/DET_NRDY.jpg` & `flashcam-1.5.1/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/data/DET_RDY_.jpg` & `flashcam-1.5.1/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/data/digital-7.mono.ttf` & `flashcam-1.5.1/flashcam/data/digital-7.mono.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/data/monoskop.jpg` & `flashcam-1.5.1/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/data/win_rain.jpg` & `flashcam-1.5.1/flashcam/data/win_rain.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/data/win_skull.jpg` & `flashcam-1.5.1/flashcam/data/win_skull.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/data/win_storm.jpg` & `flashcam-1.5.1/flashcam/data/win_storm.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/data/win_winter.jpg` & `flashcam-1.5.1/flashcam/data/win_winter.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/data/windows.jpg` & `flashcam-1.5.1/flashcam/data/windows.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/direct.py` & `flashcam-1.5.1/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/izmq_receiver.py` & `flashcam-1.5.1/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/mmapwr.py` & `flashcam-1.5.1/flashcam/mmapwr.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/real_camera.py` & `flashcam-1.5.1/flashcam/real_camera.py`

 * *Files 12% similar despite different names*

```diff
@@ -368,78 +368,14 @@
 
         camera = Camera(  )
         vidnum = None # it will be re-asked gain and again
 
         cap, vidnum = camera.init_cam(  ) # can return None,None; of jpg,-1
 
 
-        # # **************** try to init camera here; if impossilble, stay here ****
-        # # earlier while (vidnum is None) or (vidnum == -1):
-        # if (vidnum is None) or (vidnum == -1):
-        #     cap, vidnum = camera.init_cam(  ) # can return None,None; of jpg,-1
-        #     camera.camera_or_image( cap, vidnum)
-
-        #     fullpath_fixed_image = "~/.config/flashcam/monoskop.jpg"
-        #     fullpath_fixed_image = os.path.expanduser( fullpath_fixed_image)
-        #     # ***************** screenshot mode *************
-        #     if not (vidnum is None) and (vidnum==-1): # it is jpg
-        #         if (cap.find("screenshot.jpg")==0) and ('pyautogui' in globals()):
-        #             image = pyautogui.screenshot()
-        #             image = cv2.cvtColor(np.array(image), cv2.COLOR_RGB2BGR)
-
-        #             scale_percent = 50
-        #             width = int(image.shape[1] * scale_percent / 100)
-        #             height = int(image.shape[0] * scale_percent / 100)
-        #             # dsize
-        #             dsize = (width, height)
-        #             # resize image
-        #             image = cv2.resize(image, dsize)
-        #             frame = image
-        #             #cv2.imwrite("screenshot.jpg", image)
-        #             #print("i... screenshot.jpg")
-        #             fullpath_fixed_image = "screenshot.jpg"
-
-        #         # *********************** jpg image mode *************
-        #         elif cap.find(".jpg")>=0:
-        #             #print(cap)
-        #             #print(cap)
-        #             fullpath_fixed_image = f"{cap}"
-        #             fullpath_fixed_image = os.path.expanduser( fullpath_fixed_image )
-        #             if not os.path.exists(fullpath_fixed_image):
-        #                 fullpath_fixed_image = f"~/.config/flashcam/{cap}"
-        #                 fullpath_fixed_image = os.path.expanduser( fullpath_fixed_image )
-        #                 if not os.path.exists(fullpath_fixed_image):
-        #                     fullpath_fixed_image = f"~/.config/flashcam/monoskop.jpg"
-        #                     fullpath_fixed_image = os.path.expanduser( fullpath_fixed_image)
-
-        #     # ******************* no video available mode **********************
-        #     if (vidnum is None) or (vidnum==-1):
-        #         print(f"!... no VID recommended, I'm in a loop (realcam/frames) {dt.datetime.now().strftime('%H:%M:%S')}", end = "\r")
-
-        #         #print(fullpath_fixed_image)
-        #         # fullpath_fixed_image = "~/.config/flashcam/monoskop.jpg"
-
-        #         # special treatment for fixed image/screenshot.jpg...
-
-        #         if os.path.exists(fullpath_fixed_image):
-        #             frame = cv2.imread( fullpath_fixed_image)
-        #             #print(f"i...  {fullpath_fixed_image}")
-        #             senh.add_frame(frame)
-        #             senh.setbox(" ", senh.TIME)
-        #             frame = senh.get_frame(  )
-        #             # this is not giving anything
-        #             yield frame
-        #         elif fullpath_fixed_image=="screenshot.jpg":
-        #             senh.add_frame(frame)
-        #             senh.setbox(" ", senh.TIME)
-        #             frame = senh.get_frame(  )
-        #             yield frame
-        #         else:
-        #             print(f"!... broadcast image not found: {fullpath_fixed_image}")
-        #         time.sleep(0.5)
 
 
 
 
         # *********  video works,  get capacities and go with EXPO GAIN
         if not( (vidnum is None) or (vidnum == -1) ):
 
@@ -462,26 +398,26 @@
             if aga!=None: ga,gad,ming,maxg,ga10 = aga
 
             # very stupid camera    ZC0303 Webcam
             if "exposure" in capa:
                 exposure = cc.get_exposure()
                 exposuredef = cc.getdef_exposure()
                 #?????
-                #exposure_autodef = cc.getdef_exposure()
+                #auto_exposuredef = cc.getdef_exposure()
                 print(f"i... EXPOAUTO (top) == {exposure} vs def={exposuredef}; ")
 
 
-            if "exposure_auto" in capa:
-                expo_auto = cc.get_exposure_auto()
-                expo_autodef = cc.getdef_exposure_auto()
+            if "auto_exposure" in capa:
+                expo_auto = cc.get_auto_exposure()
+                expo_autodef = cc.getdef_auto_exposure()
                 print(f"i... EXPOAUTO (TOP) == {expo_auto} vs def={expo_autodef}; ")
 
-            if "exposure_absolute" in capa:
-                exposure_absolute = cc.get_exposure_absolute()
-                exposuredef = cc.getdef_exposure_absolute() # i think all cams
+            if "exposure_time_absolute" in capa:
+                exposure_time_absolute = cc.get_exposure_time_absolute()
+                exposuredef = cc.getdef_exposure_time_absolute() # i think all cams
 
             if "gain" in capa:
                 gain = cc.get_gain()
                 gaindef = cc.getdef_gain()
 
             if "gamma" in capa:
                 gamma = cc.get_gamma()
@@ -510,122 +446,33 @@
             # can change cap to a new one
             ccoi1, frame, cap = camera.camera_or_image(cap, vidnum)
             #print( ccoi1 * 30 )
             ret = True # for the next
             if ccoi1 == "camera" and frame is None:
                 ret = False
 
-            # if ccoi1 == "camera":
-            #     if type(cap) == tuple:
-            #         print("i... TUPLE cap==", cap)
-            #         cap = cap[0] # THIS IS STRANGE FOR newcam20211117
-            #         print("i...   new cap==", cap , type(cap) )
-
-            #     if (cap is None) or (not cap.isOpened()):
-            #         print("X... camera is None ")
-            #         ret = False
-            #     elif not cap.isOpened():
-            #         print("X... camera  not Opened(real)")
-            #         ret = False
-            #     else:
-            #         try: #----this catches errors of libjpeg with cv2.CAP_V4L2
-            #             print(f"i... frame {nfrm:8d}   ", end="\r" )
-            #             ret, frame = cap.read()
-            #             BaseCamera.nframes+=1
-
-            #             #wname = f"res {frame.shape[1]}x{frame.shape[0]}"
-            #             nfrm+=1
-            #             #print(f"D... got frame (frames iter)   ret={ret}  {frame.shape}")
-            #         except Exception as ex:
-            #             print("D... SOME OTHER EXCEPTION ON RECV...", ex)
-            #             config.CONFIG["camera_on"] = False
-
-            #     # --- camera probably works ret True
-            #     if not ret:
-            #         time.sleep(0.5)
-            #         config.CONFIG["camera_on"] = False
-            #         print("i... ??? cap didnt go ok, graying...")
-            #         cap = Camera.init_cam( ) # WHAT IS THIS? the same?<= static?
-            #         nfrm = 0
-
-            #         # create gray + moving lines BUT prev_frame is bad sometimes
-            #         try:
-            #             print("D... trying to gray frame")
-            #             frame = cv2.cvtColor(frame_prev, cv2.COLOR_BGR2GRAY)
-            #             height, width = frame.shape[0] , frame.shape[1]
-
-            #             skip = 10
-            #             startl = 2*(nfrm % skip) # moving lines
-            #             for il in range(startl,height,skip):
-            #                 x1, y1 = 0, il
-            #                 x2, y2 = width, il
-            #                 #image = np.ones((height, width)) * 255
-            #                 line_thickness = 1
-            #                 cv2.line(frame, (x1, y1), (x2, y2), (111, 111, 111),
-            #                          thickness=line_thickness)
-            #         except:
-            #             print("X... prev_frame was bad, no gray image")
-            #     # _____________ finished with camera communication ________
-            # #elif camera.camera_or_image()[0] == "image":
-            # else:
-            #     frame = camera.camera_or_image()[1]
-
-
-
-
             #print("D... ret==", ret)
             if ret: #********************************************************* operations
-                # fixed_image = "beamon.jpg"
-                # ----- probably mmap COMMAND FROM seread "fixed_image imgname"
+
+                # FIXED IMAGE NOT ALLOWED DURING NORMAL CAMERA MODE - ONLY
+                # FIXED IMAGE NOT ALLOWED DURING NORMAL CAMERA MODE - ONLY  from 202304027
+                # FIXED IMAGE NOT ALLOWED DURING NORMAL CAMERA MODE - ONLY
                 #
-                if fixed_image is not None:
-                    fullpath_fixed_image = "~/.config/flashcam/"+fixed_image
-                    fullpath_fixed_image = os.path.expanduser( fullpath_fixed_image )
-                    if os.path.exists(fullpath_fixed_image):
-                        frame = cv2.imread( fullpath_fixed_image)
+                # if fixed_image is not None:
+                #     fullpath_fixed_image = "~/.config/flashcam/"+fixed_image
+                #     fullpath_fixed_image = os.path.expanduser( fullpath_fixed_image )
+                #     if os.path.exists(fullpath_fixed_image):
+                #         frame = cv2.imread( fullpath_fixed_image)
 
                 frame_prev = frame
 
 
 
                 if senh.add_frame(frame):  # it is a proper image....
 
-
-                    #------------------------------ BRUTAL ------------test exposure V4L
-                    # if (BaseCamera.nframes % 100==0):
-                    #     cc = v4lc.V4L2_CTL("/dev/video"+str(vidnum))
-                    #     capa = cc.get_capbilities()
-                    #     #cc.refresh()
-                    #     exposure_absolute = 100
-                    #     expo_auto = 3
-                    #     expo_autodef = 3
-
-
-                    #     # stupid camera ZC0303 Webcam - parallel to exposure_auto
-                    #     if "exposure" in capa:
-                    #         exposure = cc.get_exposure()
-
-                    #     if "exposure_auto" in capa: # notauto? alway show _absolute
-                    #         expo_auto = cc.get_exposure_auto()
-                    #         expo_autodef = cc.getdef_exposure_auto()
-                    #         print(f"i...                   EXPOAUTO (inloop) == {expo_auto}/{expo_autodef}  [{BaseCamera.nframes%3}]; ",end="\r")
-
-                    #     if "exposure_absolute" in capa:
-                    #         exposure_absolute = cc.get_exposure_absolute()
-
-
-                    #     if "gain" in capa:
-                    #         gain = cc.get_gain()
-                    #         gaindef = cc.getdef_gain()
-                    #     if "gamma" in capa:
-                    #         gamma = cc.get_gamma()
-                    #         gammadef = cc.getdef_gamma()
-                    # #------------------------------------------------------------
-
-
                     #=========== BEFORE OTHER === Create final image ====
                     #=========== like ZOOM
                     #=========== THEN CALCULATE HISTO =====
                     #=========== THEN do other stuff
 
 
                     # 1. rotate (+translate of the center)
@@ -666,15 +513,15 @@
 
                     if restart_translate:
                         senh.reset_camera_start()
                         restart_translate = False
 
 
                     # ------------- commands comming from web.py----------------
-                    #  expressions
+                    #  expressions     external commands
                     # ------------- COMMANDS COMMING FROM WEB.PY----------------
                     #  expressions
                     # ------------- commands comming from web.py----------------
                     #           -------------- or from seread (fixed_image ...)
                     expression,value = mmread_n_clear( )
 
                     if expression[:5] != "xxxxx":
@@ -815,72 +662,125 @@
                                 gain_setdef = False
                                 if "gain" in capa:
                                     cc.setdef_gain( )
                                     gain = gaindef
 
                             # HIDDEN CAPABILITY
                             if gainvalue>=0 and gainvalue<=1:
-                                #cc.set_exposure_auto(1) #harcoded 1
-                                #exposure_absolute = cc.get_exposure_absolute()
-                                #e10 = (exposure_absolute-mine)/(maxe-mine)
+                                #cc.set_auto_exposure(1) #harcoded 1
+                                #exposure_time_absolute = cc.get_exposure_time_absolute()
+                                #e10 = (exposure_time_absolute-mine)/(maxe-mine)
                                 newgain = (maxg-ming)*gainvalue + ming
                                 cc.set_gain( newgain )
                                 gain = newgain # SENH
                                 gainvalue = -999
 
                             if  'gain' in locals() and gain != gaindef:
                                 senh.setbox(f"g {(gain-ming)/(maxg-ming):.4f}",  senh.gain)
                         #-----------------gain in capa
 
-                        if "exposure_absolute" in capa:
+                        # Sony Chip v2
+                        if  "exposure_time_absolute" in capa:
                             if expo_divide:
                                 expo_divide = False
-                                if "exposure_absolute" in capa:
-                                    cc.set_exposure_auto(1) #hardcoded 1
-                                    exposure_absolute = cc.get_exposure_absolute()
-                                    newexposure =  int(exposure_absolute/2)
-                                    if newexposure<mine: newexposure = mine
-                                    print("i... ex:", exposure_absolute, newexposure)
-                                    cc.set_exposure_absolute( newexposure)
-                                    exposure = newexposure # SENH
+                                #if "exposure_time_absolute" in capa:
+                                cc.set_auto_exposure(1) #hardcoded 1
+                                exposure_time_absolute = cc.get_exposure_time_absolute()
+                                newexposure =  int(exposure_time_absolute/2)
+                                if newexposure<mine: newexposure = mine
+                                print("i... ex:", exposure_time_absolute, newexposure)
+                                cc.set_exposure_time_absolute( newexposure)
+                                exposure = newexposure # SENH
 
                             if expo_multiply:
                                 expo_multiply = False
-                                if "exposure_absolute" in capa:
-                                    cc.set_exposure_auto(1) #harcoded 1
-                                    exposure_absolute = cc.get_exposure_absolute()
-                                    e10 = (exposure_absolute-mine)/(maxe-mine)
-                                    print("i... e10===", e10)
-                                    if (e10>=0.0001) and (e10<=0.5):
-                                        newexposure = int(exposure_absolute*2)
-                                    elif (e10>0.5):
-                                        newexposure = int(maxe)
-                                    elif (e10<=0.0001):
-                                        newexposure = int(mine+1)
-                                    else:
-                                        newexposure =  int(mine+1)
-                                    cc.set_exposure_absolute( newexposure )
-                                    exposure = newexposure # SENH
+                                #if "exposure_time_absolute" in capa:
+                                cc.set_auto_exposure(1) #harcoded 1
+                                exposure_time_absolute = cc.get_exposure_time_absolute()
+                                e10 = (exposure_time_absolute-mine)/(maxe-mine)
+                                print("i... e10===", e10)
+                                if (e10>=0.0001) and (e10<=0.5):
+                                    newexposure = int(exposure_time_absolute*2)
+                                elif (e10>0.5):
+                                    newexposure = int(maxe)
+                                elif (e10<=0.0001):
+                                    newexposure = int(mine+1)
+                                else:
+                                    newexposure =  int(mine+1)
+                                cc.set_exposure_time_absolute( newexposure )
+                                exposure = newexposure # SENH
+
+                            if expo_setdef:
+                                expo_setdef = False
+                                #if "auto_exposure" in capa:
+                                cc.setdef_auto_exposure()
+                                cc.setdef_exposure_time_absolute( )
+                                exposure = exposuredef
+                                print("i... exposure to def: ",exposure)
+
+                            # HIDDEN CAPABILITY ??? Sony Chipv2
+                            if expovalue>=0 and expovalue<=1:
+                                cc.set_auto_exposure(1) #harcoded 1
+                                #exposure_time_absolute = cc.get_exposure_time_absolute()
+                                #e10 = (exposure_time_absolute-mine)/(maxe-mine)
+                                newexposure = int( (maxe-mine)*expovalue ) + mine
+                                print(f"NEW: {newexposure} from {expovalue}")
+                                cc.set_exposure_time_absolute( newexposure )
+                                exposure = newexposure # SENH
+                                expovalue = -999
+
+                            if  'exposure' in locals() and exposure != exposuredef:
+                                senh.setbox(f"expo {(exposure-mine)/(maxe-mine):.4f}",  senh.expo)
+
+                        if "exposure_time_absolute" in capa:
+                            if expo_divide:
+                                expo_divide = False
+                                #if "exposure_time_absolute" in capa:
+                                cc.set_auto_exposure(1) #hardcoded 1
+                                exposure_time_absolute = cc.get_exposure_time_absolute()
+                                newexposure =  int(exposure_time_absolute/2)
+                                if newexposure<mine: newexposure = mine
+                                print("i... ex:", exposure_time_absolute, newexposure)
+                                cc.set_exposure_time_absolute( newexposure)
+                                exposure = newexposure # SENH
+
+                            if expo_multiply:
+                                expo_multiply = False
+                                #if "exposure_time_absolute" in capa:
+                                cc.set_auto_exposure(1) #harcoded 1
+                                exposure_time_absolute = cc.get_exposure_time_absolute()
+                                e10 = (exposure_time_absolute-mine)/(maxe-mine)
+                                print("i... e10===", e10)
+                                if (e10>=0.0001) and (e10<=0.5):
+                                    newexposure = int(exposure_time_absolute*2)
+                                elif (e10>0.5):
+                                    newexposure = int(maxe)
+                                elif (e10<=0.0001):
+                                    newexposure = int(mine+1)
+                                else:
+                                    newexposure =  int(mine+1)
+                                cc.set_exposure_time_absolute( newexposure )
+                                exposure = newexposure # SENH
 
                             if expo_setdef:
                                 expo_setdef = False
-                                if "exposure_auto" in capa:
-                                    cc.setdef_exposure_auto()
-                                    cc.setdef_exposure_absolute( )
-                                    exposure = exposuredef
-                                    print("i... exposure to def: ",exposure)
+                                #if "auto_exposure" in capa:
+                                cc.setdef_auto_exposure()
+                                cc.setdef_exposure_time_absolute( )
+                                exposure = exposuredef
+                                print("i... exposure to def: ",exposure)
 
                             # HIDDEN CAPABILITY
                             if expovalue>=0 and expovalue<=1:
-                                cc.set_exposure_auto(1) #harcoded 1
-                                #exposure_absolute = cc.get_exposure_absolute()
-                                #e10 = (exposure_absolute-mine)/(maxe-mine)
+                                cc.set_auto_exposure(1) #harcoded 1
+                                #exposure_time_absolute = cc.get_exposure_time_absolute()
+                                #e10 = (exposure_time_absolute-mine)/(maxe-mine)
                                 newexposure = int( (maxe-mine)*expovalue ) + mine
                                 print(f"NEW: {newexposure} from {expovalue}")
-                                cc.set_exposure_absolute( newexposure )
+                                cc.set_exposure_time_absolute( newexposure )
                                 exposure = newexposure # SENH
                                 expovalue = -999
 
 
 
                             if  'exposure' in locals() and exposure != exposuredef:
                                 senh.setbox(f"expo {(exposure-mine)/(maxe-mine):.4f}",  senh.expo)
@@ -926,17 +826,17 @@
                     # # ----------------expo gain gamma
                     # # very stupid camera    ZC0303 Webcam
                     # # print(capa, exposure,exposuredef) # crashes
                     # if "exposure" in capa:
                     #     if exposure!=exposuredef: # manual
                     #         senh.setbox(f"expo {exposure}",  senh.expo)
 
-                    # if "exposure_auto" in capa:
+                    # if "auto_exposure" in capa:
                     #     if expo_auto!=expo_autodef: # manual
-                    #         senh.setbox(f"expo {exposure_absolute}",  senh.expo)
+                    #         senh.setbox(f"expo {exposure_time_absolute}",  senh.expo)
 
                     # if ("gain" in capa) and (gain!=gaindef): # gain is not frequently tunable
                     #     senh.setbox(f"g {gain}",  senh.gain)
 
                     # if ("gamma" in capa):
                     #     if (gamma!=gammadef): # manual
                     #         senh.setbox(f"m {gamma}",  senh.gamma)
```

### Comparing `flashcam-1.4.2/flashcam/stream_enhancer.py` & `flashcam-1.5.1/flashcam/stream_enhancer.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/uniwrec.py` & `flashcam-1.5.1/flashcam/uniwrec.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/usbcheck.py` & `flashcam-1.5.1/flashcam/usbcheck.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam/v4lc.py` & `flashcam-1.5.1/flashcam/v4lc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 #!/usr/bin/env python3
 '''
  on https://github.com/TheStaticTurtle/RemoteV4L2-CTL/blob/master/remote_v4l2ctl/utils.py
 '''
 from flashcam.version import __version__
 from fire import Fire
 from flashcam import config
@@ -293,47 +292,48 @@
 
 
 def get_gem( cc, capa ):
     # capa = cc.get_capbilities()
 
     agm = None
     aex = None
-    aea = None
+    aea = None # auto_exposure (exposure_auto for <ubu22)
     aga = None
 
     if "gamma" in capa:
         gm = cc.get_gamma()
         gmd = cc.getdef_gamma()
         minm = cc.getmin_gamma()
         maxm = cc.getmax_gamma()
         gm10 = (gm-minm)/(maxm-minm)
-        agm = (gm,gmd,minm,maxm,gm10)
+        agm = (gm,gmd,minm,maxm,gm10) # gamma, defa, min, max, divided-0-1
         print(f"I... gamma             {gm:5d};  range({minm:4d},{maxm:5d}) def: {gmd} {gm10:.5f}")
 
-    if "exposure_absolute" in capa:
-        ex = cc.get_exposure_absolute()
-        exd=  cc.getdef_exposure_absolute()
-        mine = cc.getmin_exposure_absolute()
-        maxe = cc.getmax_exposure_absolute()
+    if "exposure_time_absolute" in capa:
+        ex = cc.get_exposure_time_absolute()
+        exd=  cc.getdef_exposure_time_absolute()
+        mine = cc.getmin_exposure_time_absolute()
+        maxe = cc.getmax_exposure_time_absolute()
         ex10 = (ex-mine)/(maxe-mine)
         aex = (ex,exd,mine,maxe,ex10)
-        print(f"I... exposure_absolute {ex:5d};  range({mine:4d},{maxe:5d}) def: {exd} {ex10:.5f}")
+        print(f"I... exposure_time_absolute {ex:5d};  range({mine:4d},{maxe:5d}) def: {exd} {ex10:.5f}")
 
-    if "exposure_auto" in capa:
-        ea = cc.get_exposure_auto()
-        ead=  cc.getdef_exposure_auto()
-        minea = cc.getmin_exposure_auto()
-        maxea = cc.getmax_exposure_auto()
+    if "auto_exposure" in capa:
+        ea = cc.get_auto_exposure()
+        ead=  cc.getdef_auto_exposure()
+        minea = cc.getmin_auto_exposure() # I think IT IS 1
+        minea = 1
+        maxea = cc.getmax_auto_exposure()
         aea = (ea,ead,minea,maxea)
         print(f"I... exposure auto     {ea:5d};  range({minea:4d},{maxea:5d}) def: {ead}")
 
     # A STRANGE CAMERA
     if "exposure" in capa:
         ex = cc.get_exposure()
-        exd=  cc.getdef_exposure_absolute()
+        exd=  cc.getdef_exposure_time_absolute()
         mine = cc.getmin_exposure()
         maxe = cc.getmax_exposure()
         gm10 = (ex-mine)/(maxe-mine)
         aex = (ex,exd,mine,maxe,ex10)
         print(f"I...  exposure         {ex:4d};  range({mine:4d},{maxe:5d}) def: {exd} {ex10:.5f}")
 
 
@@ -374,43 +374,43 @@
 
     if not "ex" in locals():  return
 
     print(f"i1... in set_gem: ex={ex}")
     if not expo is None:
         print(f"ix... expo demand {expo}")
         if (expo == "auto"):
-            if "exposure_absolute" in capa:
+            if "exposure_time_absolute" in capa:
                 print("D... AUTO EXPOSURE ON")
-                cc.setdef_exposure_auto()  # i thik he knows what is auto
+                cc.setdef_auto_exposure()  # i thik he knows what is auto
         elif expo !=-1:
-            if "exposure_absolute" in capa:
-                if "exposure_auto" in capa:
+            if "exposure_time_absolute" in capa:
+                if "auto_exposure" in capa:
                     print("D... AUTO EXPOSURE OFF")
-                    cc.setdef_exposure_auto() # doesnt do default 3
-                    #print("ex def",cc.get_exposure_auto())
-                    cc.set_exposure_auto(1)  # I just a guess, 1 may be manual, 3
+                    cc.setdef_auto_exposure() # doesnt do default 3
+                    #print("ex def",cc.get_auto_exposure())
+                    cc.set_auto_exposure(1)  # I just a guess, 1 may be manual, 3
 
 
-                    ex = cc.get_exposure_absolute()
-                    mine = cc.getmin_exposure_absolute()
-                    maxe = cc.getmax_exposure_absolute()
+                    ex = cc.get_exposure_time_absolute()
+                    mine = cc.getmin_exposure_time_absolute()
+                    maxe = cc.getmax_exposure_time_absolute()
                     print(f"i... current exposure {ex}   range {mine}, {maxe}")
 
                     if (expo == "def"):
-                        cc.setdef_exposure_absolute()
+                        cc.setdef_exposure_time_absolute()
                         print("i... new ex= default")
                     else:
                         ex = int( expo * (maxe-mine)+mine)
                         if expo>1: ex+=1
                         if expo<1: ex-=1
                         if ex>maxe: ex=maxe
                         if ex<mine: ex=mine
                         print(f"i... new ex1= {ex};   {expo}")
 
-                    cc.set_exposure_absolute(ex)
+                    cc.set_exposure_time_absolute(ex)
             # very stupid wabcam
             elif "exposure" in capa:
                 ex = cc.get_exposure()
                 mine = cc.getmin_exposure()
                 maxe = cc.getmax_exposure()
                 print(f"i... current exposure {ex}   range {mine}, {maxe}")
 
@@ -419,15 +419,15 @@
                 if expo<1: ex-=1
                 if ex>maxe: ex=maxe
                 if ex<mine: ex=mine
                 print("i... new ex2= ",ex)
 
                 cc.set_exposure(ex)
             else:
-                print("X... exposure_absolute NOR exposure not in capacities")
+                print("X... exposure_time_absolute NOR exposure not in capacities")
 
     print(f"i2... in set_gem: ex={ex}")
 
     if not gain is None:
         if gain == "def":
             if "gain" in capa:
                 print("Q... messing with default gain")
@@ -614,25 +614,25 @@
         mg = cc.get_gamma()
         maxm = cc.getmax_gamma()
         minm = cc.getmin_gamma()
         defm = cc.getdef_gamma()
         maxm = limitgamma # terrible result if too much
 
 
-    if "exposure_absolute" in capa:
-        ex = cc.get_exposure_absolute()
-        mine = cc.getmin_exposure_absolute()
-        maxe = cc.getmax_exposure_absolute()
+    if "exposure_time_absolute" in capa:
+        ex = cc.get_exposure_time_absolute()
+        mine = cc.getmin_exposure_time_absolute()
+        maxe = cc.getmax_exposure_time_absolute()
 
 
     if dist<-1:
-        if "exposure_auto" in capa:
-            exposure_auto = cc.get_exposure_auto()
-            #if exposure_auto!=1:
-            cc.set_exposure_auto(3)
+        if "auto_exposure" in capa:
+            auto_exposure = cc.get_auto_exposure()
+            #if auto_exposure!=1:
+            cc.set_auto_exposure(3)
         else:
             print("X... cannot tune the exposure (no auto)")
             return
         return
 
     elif dist>4:
         FAC = 0.5
@@ -647,18 +647,18 @@
     # no caf     CAF = 1/FAC
 
     # CAF = 1/FAC_BASE # I override the speed from bottom to up
 
     print(f"i...  {med} +- {dg}  <{h_avg}>  {dist:4.1f}sigma  {FAC:5.2f}x")
 
 
-    if "exposure_absolute" in capa:
-        exposure_absolute = cc.get_exposure_absolute()
-        if exposure_absolute!=1:
-            cc.set_exposure_auto(1)
+    if "exposure_time_absolute" in capa:
+        exposure_time_absolute = cc.get_exposure_time_absolute()
+        if exposure_time_absolute!=1:
+            cc.set_auto_exposure(1)
     else:
         print("X... cannot tune the exposure (no auto)")
         return
 
 
     gg2,ex2,mg2 = gg,ex,mg
 
@@ -715,40 +715,40 @@
 
 
     #print(f"                   gain {gg}  expo {ex} gamma {mg} ")
     #print(f"                   gain {gg}  expo {ex} gamma {mg} ")
     print(f"        gain {gg} ({ming}/{maxg})  expo {ex} ({mine}/{maxe}) gamma {mg} ({minm}/{maxm}) ")
     time.sleep(0.6)
 
-    if "exposure_absolute" in capa: cc.set_exposure_absolute(ex)
+    if "exposure_time_absolute" in capa: cc.set_exposure_time_absolute(ex)
     if "gain" in capa: cc.set_gain(gg)
     if "gamma" in capa: cc.set_gamma(mg2)
 
     # if gg>maxg:
     #     if h_avg<glow:
     #         ex+=2
-    #         cc.set_exposure_absolute(ex)
+    #         cc.set_exposure_time_absolute(ex)
     #     elif h_avg>ghigh:
     #        gg-=2
     #        if "gain" in capa: cc.set_gain(gg)
     # elif gg<ming:
     #     if h_avg>ghigh:
     #        ex-=2
-    #        cc.set_exposure_absolute(ex)
+    #        cc.set_exposure_time_absolute(ex)
     #     if h_avg<glow:
     #        gg+=2
     #        if "gain" in capa: cc.set_gain(gg)
     # else:
     #     if h_avg<glow:
     #         gg+=2
     #         if "gain" in capa: cc.set_gain(gg)
     #     elif h_avg>ghigh:
     #         gg-=2
     #         if "gain" in capa: cc.set_gain(gg)
-    #res = cc.set_exposure_absolute(ex)
+    #res = cc.set_exposure_time_absolute(ex)
     return gg,ex
 
 
 def main( devid ):
     """
     Here it is a test to set exposure and gain by histogram
     """
@@ -763,40 +763,40 @@
     lw=1
     bins=256
 
     initme = True
     gain = 100
     capa = cc.get_capbilities()
 
-    if "exposure_auto" in capa:
+    if "auto_exposure" in capa:
         print("D... AUTO EXPOSURE OFF")
-        cc.setdef_exposure_auto() # doesnt do default 3
-        print("ex def",cc.get_exposure_auto())
-        cc.set_exposure_auto(1)
+        cc.setdef_auto_exposure() # doesnt do default 3
+        print("ex def",cc.get_auto_exposure())
+        cc.set_auto_exposure(1)
 
-    #print("ex 3",cc.get_exposure_auto())
+    #print("ex 3",cc.get_auto_exposure())
     if "gain" in capa:
         cc.setdef_gain()
         gg = cc.get_gain()
         print("defgain ",gg)
 
-    if "exposure_absolute" in capa:
-        ex = cc.get_exposure_absolute()
-        cc.setdef_exposure_absolute()
+    if "exposure_time_absolute" in capa:
+        ex = cc.get_exposure_time_absolute()
+        cc.setdef_exposure_time_absolute()
 
     gain= 0
 
     #create two subplots
     ax1 = plt.subplot(1,2,1)
     ax2 = plt.subplot(1,2,2)
     lineGray, = ax2.plot(np.arange(bins), np.zeros((bins,1)), c='r', lw=lw)
     ax2.set_xlim(-10, bins + 10)
 
     while(True):# https://github.com/nrsyed/computer-vision/blob/master/real_time_histogram/real_time_histogram.py
-        #print(" ... gain,  exposure   ",cc.get_gain(), cc.get_exposure_absolute() )
+        #print(" ... gain,  exposure   ",cc.get_gain(), cc.get_exposure_time_absolute() )
 
         ret, frame = vid.read()
         # if initme:
 
         #     #ax2.set_ylim(0, 1)
         #     ax1.set_axis_off()
         #     ax2.spines['right'].set_visible(False)
```

### Comparing `flashcam-1.4.2/flashcam/web.py` & `flashcam-1.5.1/flashcam/web.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/flashcam.egg-info/PKG-INFO` & `flashcam-1.5.1/flashcam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.4.2
+Version: 1.5.1
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.4.2/flashcam.egg-info/SOURCES.txt` & `flashcam-1.5.1/flashcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flashcam-1.4.2/setup.py` & `flashcam-1.5.1/setup.py`

 * *Files identical despite different names*


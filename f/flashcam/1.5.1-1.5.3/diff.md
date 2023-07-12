# Comparing `tmp/flashcam-1.5.1.tar.gz` & `tmp/flashcam-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.5.1.tar", last modified: Wed Jul 12 09:17:50 2023, max compression
+gzip compressed data, was "flashcam-1.5.3.tar", last modified: Wed Jul 12 13:26:08 2023, max compression
```

## Comparing `flashcam-1.5.1.tar` & `flashcam-1.5.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 09:17:50.111114 flashcam-1.5.1/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-07-12 09:17:50.111114 flashcam-1.5.1/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-04-17 13:40:53.000000 flashcam-1.5.1/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 09:17:50.107114 flashcam-1.5.1/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24826 2023-04-20 12:20:29.000000 flashcam-1.5.1/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-04-06 11:29:38.000000 flashcam-1.5.1/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2023-04-06 11:29:38.000000 flashcam-1.5.1/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-06 11:48:21.000000 flashcam-1.5.1/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 09:17:50.111114 flashcam-1.5.1/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8079 2023-04-17 13:40:53.000000 flashcam-1.5.1/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 09:17:50.111114 flashcam-1.5.1/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-20 08:33:53.000000 flashcam-1.5.1/flashcam/data/win_rain.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-20 08:33:53.000000 flashcam-1.5.1/flashcam/data/win_skull.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-20 08:33:53.000000 flashcam-1.5.1/flashcam/data/win_storm.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-20 08:33:53.000000 flashcam-1.5.1/flashcam/data/win_winter.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-04-20 08:33:53.000000 flashcam-1.5.1/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40421 2023-07-12 09:16:16.000000 flashcam-1.5.1/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-20 12:14:15.000000 flashcam-1.5.1/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)   100516 2023-04-06 11:29:38.000000 flashcam-1.5.1/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-06 11:51:33.000000 flashcam-1.5.1/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    27692 2023-07-12 09:16:16.000000 flashcam-1.5.1/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-07-12 09:17:49.000000 flashcam-1.5.1/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30138 2023-04-20 12:48:25.000000 flashcam-1.5.1/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 09:17:50.111114 flashcam-1.5.1/flashcam.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-07-12 09:17:50.000000 flashcam-1.5.1/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      820 2023-07-12 09:17:50.000000 flashcam-1.5.1/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-07-12 09:17:50.000000 flashcam-1.5.1/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-07-12 09:17:50.000000 flashcam-1.5.1/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-07-12 09:17:50.000000 flashcam-1.5.1/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-07-12 09:17:50.111114 flashcam-1.5.1/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-18 08:31:29.000000 flashcam-1.5.1/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 13:26:08.468169 flashcam-1.5.3/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-07-12 13:26:08.468169 flashcam-1.5.3/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-04-17 13:40:53.000000 flashcam-1.5.3/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 13:26:08.464169 flashcam-1.5.3/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24826 2023-04-20 12:20:29.000000 flashcam-1.5.3/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-04-06 11:29:38.000000 flashcam-1.5.3/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2023-04-06 11:29:38.000000 flashcam-1.5.3/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-06 11:48:21.000000 flashcam-1.5.3/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 13:26:08.464169 flashcam-1.5.3/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8079 2023-04-17 13:40:53.000000 flashcam-1.5.3/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 13:26:08.468169 flashcam-1.5.3/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-20 08:33:53.000000 flashcam-1.5.3/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-20 08:33:53.000000 flashcam-1.5.3/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-20 08:33:53.000000 flashcam-1.5.3/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-20 08:33:53.000000 flashcam-1.5.3/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-04-20 08:33:53.000000 flashcam-1.5.3/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40421 2023-07-12 09:16:16.000000 flashcam-1.5.3/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-20 12:14:15.000000 flashcam-1.5.3/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)   102690 2023-07-12 13:24:22.000000 flashcam-1.5.3/flashcam/uniwrec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-06 11:51:33.000000 flashcam-1.5.3/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    27692 2023-07-12 09:16:16.000000 flashcam-1.5.3/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-07-12 13:26:08.000000 flashcam-1.5.3/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30433 2023-07-12 13:08:09.000000 flashcam-1.5.3/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 13:26:08.464169 flashcam-1.5.3/flashcam.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-07-12 13:26:08.000000 flashcam-1.5.3/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      820 2023-07-12 13:26:08.000000 flashcam-1.5.3/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-07-12 13:26:08.000000 flashcam-1.5.3/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-07-12 13:26:08.000000 flashcam-1.5.3/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-07-12 13:26:08.000000 flashcam-1.5.3/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-07-12 13:26:08.468169 flashcam-1.5.3/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-18 08:31:29.000000 flashcam-1.5.3/setup.py
```

### Comparing `flashcam-1.5.1/PKG-INFO` & `flashcam-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.5.1
+Version: 1.5.3
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.5.1/README.md` & `flashcam-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/bin/flashcam` & `flashcam-1.5.3/bin/flashcam`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/bin/flashcamg` & `flashcam-1.5.3/bin/flashcamg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/base_camera2.py` & `flashcam-1.5.3/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/config.py` & `flashcam-1.5.3/flashcam/config.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.5.3/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.5.3/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/data/DET_NRDY.jpg` & `flashcam-1.5.3/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/data/DET_RDY_.jpg` & `flashcam-1.5.3/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/data/digital-7.mono.ttf` & `flashcam-1.5.3/flashcam/data/digital-7.mono.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/data/monoskop.jpg` & `flashcam-1.5.3/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/data/win_rain.jpg` & `flashcam-1.5.3/flashcam/data/win_rain.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/data/win_skull.jpg` & `flashcam-1.5.3/flashcam/data/win_skull.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/data/win_storm.jpg` & `flashcam-1.5.3/flashcam/data/win_storm.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/data/win_winter.jpg` & `flashcam-1.5.3/flashcam/data/win_winter.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/data/windows.jpg` & `flashcam-1.5.3/flashcam/data/windows.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/direct.py` & `flashcam-1.5.3/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/izmq_receiver.py` & `flashcam-1.5.3/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/mmapwr.py` & `flashcam-1.5.3/flashcam/mmapwr.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/real_camera.py` & `flashcam-1.5.3/flashcam/real_camera.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/stream_enhancer.py` & `flashcam-1.5.3/flashcam/stream_enhancer.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/uniwrec.py` & `flashcam-1.5.3/flashcam/uniwrec.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,51 +74,55 @@
 global countdownpause, optimgain, optimexpo, optim_histo, countdown_gain
 countdownpause = 5
 optimgain = -1
 optimexpo = -1
 optim_histo = 49  # we try middle of the range in %
 countdown_gain = False  # Sonix USB 0c45:62c0 has broken expo, but gain ok
 
+jpgkompr2 = [100, 95, 90, 80, 70, 60, 50, 40, 30,20,10, 5]
+jpgkompr1 = [x for x in jpgkompr2]
+
+
 # i needed a warning before 't'
 global allow_tracker, allow_tracker_demand
 allow_tracker = False
 allow_tracker_demand = False
 
 global show_help
 show_help = False
 
 
 # x ... expand 2x ... buggy
-HELPTEXT = """ a/A ... AVI/stop (~/DATA/) (alt-a PNG)
+HELPTEXT = """ a/A ... AVI/stop (~/DATA/) (ctl-a PNG)
  s/S ... save 1 JPG (PNG) (to ~/DATA/)
 
  z ... cycle zoom 2x (mouse click fixes the center)
  Z ... zoom 1x
- r/R ... rotate by +-1; Alt-r= 180 degrees
+ r/R ... rotate by +-1; Ctl-r= 180 degrees
 
  c/C ... red cross on/off (save when off)
  hjkl ... move the red/green* cross (HJKL)
  t/u ... tracker 1 (cross sync, speed)
  T/u ... tracker 2 (more steady, but fragile)
 
  m/M ... measure/not distance,  (-v 110,1.2)
  n/N ... inc/decrease distance
  f/F ... inc/dec Field Of View (-v FOV,dist)
 
  v/V* ... green cross ON/OFF
  b/f* ... substract BG, mix FG
  B/F* ... SAVE BG/ SAVE FG
 
- eg* ...  expo/gain (+ shift or alt)
- y   ...  gamma (local) (+shift or alt)
+ eg* ...  expo/gain (+ shift or ctl)
+ y   ...  gamma (local) (+shift or ctl)
  o/O ... autotune expo / break tuning
  i/I* ... accumulate images
 
  w ... open web browser
- q ... quit
+ q ... quit     ctl-t ... some test
        * with remote flashcam server """
 
 
 
 
 
 def rotate_image(image, angle):
@@ -130,74 +134,89 @@
     #print(rot_mat)
     result = cv2.warpAffine(image, rot_mat, image.shape[1::-1], flags=cv2.INTER_LINEAR)
     #print("rotated by ", angle)
     return result
 
 
 
-
+# NOT IN UBUNTU22
 def kb_on_press(key):
     global SHIFT, CTRL
+    print("                                              =v=")
     try:
         a = key.char
         # print('alphanumeric key {0} pressed'.format( key.char))
         # CTRL  = False
     except AttributeError:
-        # print('special key {0} pressed'.format(  key))
-        if key == Key.alt:
-            CTRL = True
-        if key == Key.shift:
-            SHIFT = True
+        print('special key {0} pressed'.format(  key))
+    if key == Key.alt:
+        CTRL = True
+    if key == Key.shift:
+        SHIFT = True
     return
 
-
+# NOT ON UBUNTU22
 def kb_on_release(key):
     global SHIFT, CTRL
+    print("                                              =^=")
     if key == Key.alt:
         CTRL = False
     if key == Key.shift:
         SHIFT = False
-    # print('{0} released'.format( key))
+    print('{0} released'.format( key))
     if key == Key.esc:
         # Stop listener
         return False
 
 
 def remap_keys(key):
     """
     Problem - THIS TABLE WORKS ON  gigajm
         , while zen : 65505
     """
     # print(f" KEY==/{key}/")
+    global CTRL
+    CTRL=False
+    if key==1310821: CTRL=True # ctrl e
+    if key==1310834: CTRL=True #  ctrl r
+    if key==1310817: CTRL=True # ctrl a
+    if key==1310823: CTRL=True # ctrl g
+    if key==1310841: CTRL=True # ctrl y
+    if key==1310836: CTRL=True # ctrl t
     table = {
         1048673: "a",
+        1310817: "a", #ctrl
         1048674: "b",
         1048675: "c",
         1048676: "d",
+        1310821: "e", #ctrl
         1048677: "e",
         1048678: "f",
         1048679: "g",
+        1310823: "g", # ctrl g
         1048680: "h",
         1048681: "i",
         1048682: "j",
         1048683: "k",
         1048684: "l",
         1048685: "m",
         1048686: "n",
         1048687: "o",
         1048688: "p",
         1048689: "q",
         1048690: "r",
         1048691: "s",
         1048692: "t",
+        1310836: "t", # ctrl
         1048693: "u",
         1048694: "v",
         1048695: "w",
         1048696: "x",
         1048697: "y",
+        1310841: "y", #ctrl
         1048698: "z",
         1114177: "A",
         1114178: "B",
         1114179: "C",
         1114180: "D",
         1114181: "E",
         1114182: "F",
@@ -400,28 +419,30 @@
 ):
     """ """
     # sname,sfilenamea,sme,sfilenamea,sfilenamea,sfourcc,saviout
 
     sme = socket.gethostname()
     # frame = None  #  gigavg a vaio have strange behaviour
 
+    global jpgkompr1, jpgkompr2
     global CTRL, SHIFT
     global centerX1, centerY1, clicked
     global FILE_USERPASS, FILE_REDCROSS
     global show_help
     global allow_tracker, allow_tracker_demand
     global local_gamma, integrate
     global countdown_gain
     centerX1, centerY1, clicked = 0, 0, True  # center zoom ion start
 
     filesource = False
 
     # ==========================  I fire here the listener from pynput !!!
-    listener = Listener(on_press=kb_on_press, on_release=kb_on_release)
-    listener.start()
+    # NOT ON UBUNTU22 ############################################################
+    #listener = Listener(on_press=kb_on_press, on_release=kb_on_release)
+    #listener.start()
     # ------------------------------------------------------ let;s see
 
     def MOUSE(event, x, y, flags, param):
         global centerX1, centerY1, clicked
         if event == cv2.EVENT_LBUTTONDOWN:
             clicked = not clicked
         if event == cv2.EVENT_MOUSEMOVE:
@@ -930,17 +951,18 @@
                 cv2.namedWindow(wname, cv2.WINDOW_GUI_NORMAL)  #
                 # cv2.namedWindow( wname , 2 ) # 2 may allow resize on gigavg
                 if frames_total < 2:
                     # cv2.namedWindow(wname,cv2.WND_PROP_FULLSCREEN)
                     # ?https://stackoverflow.com/questions/62870031/pixel-coordinates-and-colours-not-showing
                     # TRICK !!!!!!!!!!!!
                     # https://stackoverflow.com/a/52776376
-                    cv2.setWindowProperty(
-                        wname, cv2.WND_PROP_FULLSCREEN, cv2.WINDOW_FULLSCREEN
-                    )
+                    #  remove bars....  BUT IN UBUNTU 22 - I remove this and all is fine
+                    #cv2.setWindowProperty( wname, cv2.WND_PROP_FULLSCREEN, cv2.WINDOW_FULLSCREEN  )
+
+                    #cv2.setWindowProperty( wname, cv2.WND_PROP_FULLSCREEN, cv2.WINDOW_FULLSCREEN  )
                     bit_fs = 0
                     if sme in [
                         "gigavg",
                         "vaio",
                     ]:  # strange behavior on some PC concerning resize...(checked in MS with vadim)
                         bit_fs = 1
                     cv2.setWindowProperty(wname, cv2.WND_PROP_FULLSCREEN, bit_fs)
@@ -1565,29 +1587,38 @@
                     # print(frame.shape)
                 # cv2.setWindowProperty(rpi_name, cv2.WND_PROP_TOPMOST, 1)
                 # cv2.namedWindow(rpi_name, cv2.WINDOW_GUI_EXPANDED)
                 # time.sleep(0.2)
                 cv2.setMouseCallback(rpi_name, MOUSE)
                 #
                 #  waitkeyex sometimes sees shift and ctrl... but not on zen...
+                #########################################################################
+                #########################################################################
+                #########################################################################
+                #key = cv2.waitKey(1)  # same problem with shift on ubu22 as ex
+                #########################################################################
+                #########################################################################
+                #########################################################################
                 #
-                key = cv2.waitKey(1)  # same problem with shift on ubu22 as ex
-                #
-                # key = cv2.waitKeyEx(1)
+                key = cv2.waitKeyEx(1) # this may work in ubuntu 22 - let us check....
 
                 c = s = "     "
-                if CTRL:
-                    c = "ALT  "
-                if SHIFT:
-                    s = "SHIFT"
+                # non-ubuntu22 version makes sense with Listener
+                #if CTRL:  c = "ALT  "
+                #if SHIFT: s = "SHIFT"
                 # print(f" {c} x {s} ...      ", end = "       \n")
+
+                #
+                # UBUNTU 22 - ctrl and alt give 227 and 233 resp
+                #
                 if key != -1:
-                    print(f" readkey== {key}   /{chr(0xFF&key)}/  .. {c} : {s}  >>>. ")
-                    if SHIFT:
-                        key = ord(chr(key).upper())
+                    print(f" key== {key}   /{chr(0xFF&key)}/  .. {c} : {s}  >>>.      ")
+                    key = remap_keys(key) # make compatible with waitKey()
+                    print(f" ... --------------------------------------------- remapped {key}")
+                    if SHIFT: key = ord(chr(key).upper())
 
                 # i will not use the translation,,
                 # key = remap_keys(key) # make compatible with waitKey()
                 # print(f"remapped {key}")
 
                 # print(f"{centerX1} {centerY1}")
                 if (cross is None) and not greencross:
@@ -1694,15 +1725,15 @@
                         sfilenamea, saviout = setupsave((width, height))
                         print(">>>", sfilenamea)
 
 
 
                 if (frame is not None) and \
                    (rpi_name != "") and \
-                   (key == ord("A") and not CTRL):  # not with alt
+                   (key == ord("A") and not CTRL):  # not with ctl
                     if save:
                         print("A PRESSED! - STOPPING AVI (mkv)  decor ==", save_decor)
                         sfilenamea = ""
                         savepngcont = False
                         save = False
                     else:
                         print("A PRESSED! - WITH DECOR saving AVI (mkv)")
@@ -1717,15 +1748,15 @@
 
                 if ( (frame is not None) and \
                      (rpi_name != "") and \
                      (key == ord("a"))  and (CTRL) ):  # (key == 1310817):
                     if savepngcont:
                         savepngcont = False
                     else:
-                        print("alt-a PRESSED! - saving PNG continuosly !!!")  # ctrla
+                        print("ctl-a PRESSED! - saving PNG continuosly !!!")  # ctrla
                         savepngcont = True
 
 
 
 
                 saved_jpg = 0
                 if (
@@ -2268,21 +2299,22 @@
 
                 if (frame is not None) and (rpi_name != "") and (key == ord("E")):
                     print("e PRESSED! - ")
                     post_addr = videodev.replace("/video", "/cross")
                     post_data = {"expo05": "EXPO05"}
                     post_response = requests.post(url=post_addr, data=post_data)
 
+                # ------------------default expo----------------------
                 if (
                     (frame is not None)
                     and (rpi_name != "")
                     and (key == ord("e"))
                     and (CTRL)
                 ):  # (key == 1310821 ): # ctrle
-                    print("alt-e PRESSED! - ")
+                    print("ctl-e PRESSED! - ")
                     post_addr = videodev.replace("/video", "/cross")
                     post_data = {"expo": "EXPO"}
                     post_response = requests.post(url=post_addr, data=post_data)
 
                 if (
                     (frame is not None)
                     and (rpi_name != "")
@@ -2301,42 +2333,42 @@
 
                 if (
                     (frame is not None)
                     and (rpi_name != "")
                     and (key == ord("g"))
                     and (CTRL)
                 ):  # and  (key == 1310823): # ctrlg
-                    print("alt-g PRESSED! - ")
+                    print("ctl-g PRESSED! - ")
                     post_addr = videodev.replace("/video", "/cross")
                     post_data = {"gain": "GAIN"}
                     post_response = requests.post(url=post_addr, data=post_data)
 
                 if (
                     (frame is not None)
                     and (rpi_name != "")
-                    and (key == ord("y") and not (CTRL))
+                    and (key == ord("y") and not CTRL)
                 ):
                     print("y PRESSED! - ")
                     local_gamma = local_gamma * 1.4
 
                 if (
                     (frame is not None)
                     and (rpi_name != "")
-                    and (key == ord("Y") and not (CTRL))
+                    and (key == ord("Y") and not CTRL)
                 ):
                     print("Y PRESSED! - ")
                     local_gamma = local_gamma / 1.4
 
                 if (
                     (frame is not None)
                     and (rpi_name != "")
                     and (key == ord("y"))
                     and (CTRL)
                 ):  # and  (key == 1310841): #ctrly
-                    print("alt-y PRESSED! - ")
+                    print("ctl-y PRESSED! - ")
                     local_gamma = 1
 
                 if (frame is not None) and (rpi_name != "") and (key == ord("p")):
                     print("p PRESSED! - ")
                     post_addr = videodev.replace("/video", "/cross")
                     post_data = {"fixed": "FIXED"}
                     post_response = requests.post(url=post_addr, data=post_data)
@@ -2412,20 +2444,26 @@
                     post_addr = videodev.replace("/video", "/cross")
                     post_data = {"accum": "ACCUM", "accumtxt": 0}
                     post_response = requests.post(url=post_addr, data=post_data)
 
                 if (
                     (frame is not None)
                     and (rpi_name != "")
-                    and (key == ord("t") and (CTRL))
+                    and (key == ord("t") and CTRL)
                 ):
-                    print("alt-t PRESSED! - TEST BUTTON ---------------------")
-                    print(" try to keep alt pressed and then press t")
+                    print("ctl-t PRESSED! - TEST BUTTON ---------------------")
+                    print(" ... clears countdown .... ")
+                    #print(" try to keep ctl pressed and then press t")
                     post_addr = videodev.replace("/video", "/cross")
-                    post_data = {"kompress": "KOMPRESS", "kompressvalue": 95}
+                    if len(jpgkompr1)==0:
+                        jpgkompr1 = [x for x in jpgkompr2]
+                    aaa = jpgkompr1.pop(0)
+                    print(" ... available comp",jpgkompr1)
+                    print(" ... sets  kompression:", aaa)
+                    post_data = {"kompress": "KOMPRESS", "kompressvalue": aaa}
                     post_response = requests.post(url=post_addr, data=post_data)
                     if "countdown" in locals():
                         countdown = []
 
                 # TEST key code
                 # if key!=-1:
                 #    print(f"\n{key}\n")
```

### Comparing `flashcam-1.5.1/flashcam/usbcheck.py` & `flashcam-1.5.3/flashcam/usbcheck.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/v4lc.py` & `flashcam-1.5.3/flashcam/v4lc.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/flashcam/web.py` & `flashcam-1.5.3/flashcam/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 import random
 
 import cv2
 import numpy as np
 
 from flashcam.real_camera import Camera
+from flashcam import real_camera # for is_int()
 
 #----------------------------------------------
 from flashcam.mmapwr import mmwrite
 
 try:
     import pantilthat
 except:
@@ -542,23 +543,28 @@
             else :
                 print("ZOOM2 ->1")
                 zoom2_on = 1
                 mmwrite(f"zoom 1" )
 
         #---------------- I am blindly adding functionality ... compression now
         if  request.form.get('kompress') == 'KOMPRESS':
-            print("kompress asked  ....... ")
-            #kompressvalue = request.form.get('kompressvalue')
-            if config.CONFIG['kompress']>90:
-                config.CONFIG['kompress'] = 9
-                print("i... KOMPRESS", config.CONFIG['kompress'] )
+            kompressvalue = request.form.get('kompressvalue')
+            if real_camera.is_int(kompressvalue):
+                kompressvalue = int(kompressvalue)
             else:
-                config.CONFIG['kompress'] = 99
-                print("i... KOMPRESS", config.CONFIG['kompress'] )
-                #mmwrite(f"zoom 2" ) # not here...
+                kompressvalue = 85
+            print("kompress asked  ....... with value=", kompressvalue)
+            config.CONFIG['kompress'] = kompressvalue
+            # if config.CONFIG['kompress']>90:
+            #     config.CONFIG['kompress'] = 9
+            #     print("i... KOMPRESS", config.CONFIG['kompress'] )
+            # else:
+            #     config.CONFIG['kompress'] = 99
+            #     print("i... KOMPRESS", config.CONFIG['kompress'] )
+            #     #mmwrite(f"zoom 2" ) # not here...
 
         #---------------- TELEGRAM TEST
         if  request.form.get('telegram') == 'TELEGRAM':
             print("i...  telegram asked  ....... ")
             mmwrite(f"telegram TELEGRAM" )
```

### Comparing `flashcam-1.5.1/flashcam.egg-info/PKG-INFO` & `flashcam-1.5.3/flashcam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.5.1
+Version: 1.5.3
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.5.1/flashcam.egg-info/SOURCES.txt` & `flashcam-1.5.3/flashcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.1/setup.py` & `flashcam-1.5.3/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/irene_pro-0.0.95.tar.gz` & `tmp/irene_pro-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.95.tar", last modified: Mon Jul 10 14:15:45 2023, max compression
+gzip compressed data, was "irene_pro-0.0.96.tar", last modified: Wed Jul 12 13:22:33 2023, max compression
```

## Comparing `irene_pro-0.0.95.tar` & `irene_pro-0.0.96.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 14:15:45.578576 irene_pro-0.0.95/
--rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro-0.0.95/LICENSE
--rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro-0.0.95/MANIFEST.in
--rw-rw-rw-   0        0        0     1280 2023-07-10 14:15:45.577578 irene_pro-0.0.95/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro-0.0.95/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 14:15:45.555636 irene_pro-0.0.95/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro-0.0.95/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     8188 2023-07-06 14:04:14.000000 irene_pro-0.0.95/irene_pro/logics.py
--rw-rw-rw-   0        0        0    37020 2023-07-10 14:13:04.000000 irene_pro-0.0.95/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:15:45.573589 irene_pro-0.0.95/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1280 2023-07-10 14:15:45.000000 irene_pro-0.0.95/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-07-10 14:15:45.000000 irene_pro-0.0.95/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 14:15:45.000000 irene_pro-0.0.95/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-10 14:15:45.000000 irene_pro-0.0.95/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-10 14:15:45.000000 irene_pro-0.0.95/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 14:15:45.579573 irene_pro-0.0.95/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-07-10 14:14:34.000000 irene_pro-0.0.95/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:22:33.880844 irene_pro-0.0.96/
+-rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro-0.0.96/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro-0.0.96/MANIFEST.in
+-rw-rw-rw-   0        0        0     1280 2023-07-12 13:22:33.877852 irene_pro-0.0.96/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro-0.0.96/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 13:22:33.835994 irene_pro-0.0.96/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro-0.0.96/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     8188 2023-07-06 14:04:14.000000 irene_pro-0.0.96/irene_pro/logics.py
+-rw-rw-rw-   0        0        0    37080 2023-07-12 13:19:01.000000 irene_pro-0.0.96/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:22:33.869871 irene_pro-0.0.96/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1280 2023-07-12 13:22:33.000000 irene_pro-0.0.96/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-07-12 13:22:33.000000 irene_pro-0.0.96/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 13:22:33.000000 irene_pro-0.0.96/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-12 13:22:33.000000 irene_pro-0.0.96/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 13:22:33.000000 irene_pro-0.0.96/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 13:22:33.881839 irene_pro-0.0.96/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-07-12 13:20:50.000000 irene_pro-0.0.96/setup.py
```

### Comparing `irene_pro-0.0.95/PKG-INFO` & `irene_pro-0.0.96/irene_pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: irene_pro
-Version: 0.0.95
+Name: irene-pro
+Version: 0.0.96
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.95/README.md` & `irene_pro-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.95/irene_pro/logics.py` & `irene_pro-0.0.96/irene_pro/logics.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.95/irene_pro/widgets.py` & `irene_pro-0.0.96/irene_pro/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -567,21 +567,21 @@
 
         cal = Calendar(self.datetime_fr1, weekendbackground = "pink", weekendforeground = "#000", selectmode = "day")
         cal.pack(fill = BOTH, expand = True)
 
         time_fr = lframe(self.datetime_fr2, width = w(50))
         time_fr.pack(padx = w(2), fill=BOTH)
         label(time_fr, text = "Hour").pack(side = TOP, fill = X, pady = h(1))
-        hour = spinbox(time_fr, from_=0, to=23)
+        hour = spinbox(time_fr, from_=0, to=23, state = 'readonly')
         hour.pack(side = TOP, fill = X)
         Label(time_fr, text = "Minute").pack(side = TOP, fill = X, pady = h(1))
-        minute = spinbox(time_fr, from_=0, to=59)
+        minute = spinbox(time_fr, from_=0, to=59, state = 'readonly')
         minute.pack(side = TOP, fill = X, pady = h(1))
         Label(time_fr, text = "Second").pack(side = TOP, fill = X, pady = h(1))
-        second = spinbox(time_fr, from_=0, to=59)
+        second = spinbox(time_fr, from_=0, to=59, state = 'readonly')
         second.pack(side = TOP, fill = X, pady = h(1))
         
 
         def set_selected():
             global global_date_holder
             data = str(cal.get_date()).split("/")
             h = str(hour.get())
```

### Comparing `irene_pro-0.0.95/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.96/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: irene-pro
-Version: 0.0.95
+Name: irene_pro
+Version: 0.0.96
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.95/setup.py` & `irene_pro-0.0.96/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3935 270d 0a44 4553 4352   '0.0.95'..DESCR
+00000100: 2027 302e 302e 3936 270d 0a44 4553 4352   '0.0.96'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```


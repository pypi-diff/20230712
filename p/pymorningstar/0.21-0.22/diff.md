# Comparing `tmp/pymorningstar-0.21.tar.gz` & `tmp/pymorningstar-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymorningstar-0.21.tar", last modified: Thu Jul  6 16:04:22 2023, max compression
+gzip compressed data, was "pymorningstar-0.22.tar", last modified: Wed Jul 12 15:45:00 2023, max compression
```

## Comparing `pymorningstar-0.21.tar` & `pymorningstar-0.22.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 16:04:22.070987 pymorningstar-0.21/
--rw-rw-rw-   0        0        0       41 2022-09-08 19:02:29.000000 pymorningstar-0.21/MANIFEST.in
--rw-rw-rw-   0        0        0      431 2023-07-06 16:04:22.069985 pymorningstar-0.21/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 16:04:22.060664 pymorningstar-0.21/pymorningstar/
--rw-rw-rw-   0        0        0        0 2022-09-08 17:48:16.000000 pymorningstar-0.21/pymorningstar/__init__.py
--rw-rw-rw-   0        0        0     7636 2023-07-06 15:55:22.000000 pymorningstar-0.21/pymorningstar/excel.py
--rw-rw-rw-   0        0        0     5244 2021-11-22 08:29:25.000000 pymorningstar-0.21/pymorningstar/morning_limit.png
-drwxrwxrwx   0        0        0        0 2023-07-06 16:04:22.068987 pymorningstar-0.21/pymorningstar.egg-info/
--rw-rw-rw-   0        0        0      431 2023-07-06 16:04:21.000000 pymorningstar-0.21/pymorningstar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-07-06 16:04:21.000000 pymorningstar-0.21/pymorningstar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 16:04:21.000000 pymorningstar-0.21/pymorningstar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-19 20:07:58.000000 pymorningstar-0.21/pymorningstar.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-07-06 16:04:21.000000 pymorningstar-0.21/pymorningstar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-06 16:04:21.000000 pymorningstar-0.21/pymorningstar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      158 2023-07-06 15:57:32.000000 pymorningstar-0.21/readme.md
--rw-rw-rw-   0        0        0       42 2023-07-06 16:04:22.071074 pymorningstar-0.21/setup.cfg
--rw-rw-rw-   0        0        0      683 2023-07-06 16:03:37.000000 pymorningstar-0.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:45:00.315578 pymorningstar-0.22/
+-rw-rw-rw-   0        0        0       41 2022-09-08 19:02:29.000000 pymorningstar-0.22/MANIFEST.in
+-rw-rw-rw-   0        0        0      431 2023-07-12 15:45:00.314364 pymorningstar-0.22/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 15:45:00.305872 pymorningstar-0.22/pymorningstar/
+-rw-rw-rw-   0        0        0        0 2022-09-08 17:48:16.000000 pymorningstar-0.22/pymorningstar/__init__.py
+-rw-rw-rw-   0        0        0     7834 2023-07-12 15:44:22.000000 pymorningstar-0.22/pymorningstar/excel.py
+-rw-rw-rw-   0        0        0     5244 2021-11-22 08:29:25.000000 pymorningstar-0.22/pymorningstar/morning_limit.png
+drwxrwxrwx   0        0        0        0 2023-07-12 15:45:00.313366 pymorningstar-0.22/pymorningstar.egg-info/
+-rw-rw-rw-   0        0        0      431 2023-07-12 15:45:00.000000 pymorningstar-0.22/pymorningstar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-07-12 15:45:00.000000 pymorningstar-0.22/pymorningstar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 15:45:00.000000 pymorningstar-0.22/pymorningstar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-19 20:07:58.000000 pymorningstar-0.22/pymorningstar.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-07-12 15:45:00.000000 pymorningstar-0.22/pymorningstar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-12 15:45:00.000000 pymorningstar-0.22/pymorningstar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      158 2023-07-06 15:57:32.000000 pymorningstar-0.22/readme.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 15:45:00.315578 pymorningstar-0.22/setup.cfg
+-rw-rw-rw-   0        0        0      683 2023-07-12 15:44:52.000000 pymorningstar-0.22/setup.py
```

### Comparing `pymorningstar-0.21/pymorningstar/excel.py` & `pymorningstar-0.22/pymorningstar/excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 from dateutil.relativedelta import relativedelta
 
 
 PATH = os.path.dirname(os.path.abspath(__file__))
 
 class ExcelMorning():
     
-    def __init__(self):
+    def __init__(self, is_american_format=False):
         
         # Store Info about the Attributes Download
         self.attr_info = pd.DataFrame(columns =['Index Len', 'Col Len', 'NaN', 'Size','Time','Formula'])
         self.attr_info.index.name ='serie_code'
         # Store Info about the Attributes Download
         self.hold_info= pd.DataFrame(columns =['SerieCode', 'StarDown', 'EndDown', 'StarDate','EndDate',
                                 'IndexLen', 'ColLen', 'NaN', 'Size','Time','Formula']).set_index(  
                                 ['SerieCode', 'StarDown', 'EndDown'])
-        
+        self.is_american_format = is_american_format
         self.initialize_morning()
     
     def initialize_morning(self):
         self.wb = xw.Book()
         time.sleep(0.5)
         self.wb.app.api.WindowState = xw.constants.WindowState.xlMaximized
         self.wb.app.activate(steal_focus=True)
@@ -59,16 +59,16 @@
         # Get the holdings in yearly basis 
         start_date = inception_date.replace(day=1)
         end_date = start_date
         while end_date < obsolete_date:
             end_date = start_date + relativedelta(months=months_frac) - timedelta(days=1)
             if end_date > obsolete_date:
                 end_date = obsolete_date.replace(day=1) + relativedelta(months=1) - timedelta(days=1)            
-            start_date = start_date.strftime("%d/%m/%Y")
-            end_date = end_date.strftime("%d/%m/%Y")
+            start_date = start_date.strftime("%m/%d/%Y") if self.is_american_format  else start_date.strftime("%d/%m/%Y")
+            end_date = end_date.strftime("%m/%d/%Y") if self.is_american_format  else end_date.strftime("%d/%m/%Y")
             # Create the formula
             formula = ",".join(['"'+word+ '"' for word in [isin_fund, asset_id, start_date, end_date] ]) 
             formula = '=MSHOLDING(' + formula + formula_1 +'")' 
             
             # introduce formula and get the data
             df = self.get_data(formula, wait_time=wait_time)
             # Info about the download of holding
```

### Comparing `pymorningstar-0.21/pymorningstar/morning_limit.png` & `pymorningstar-0.22/pymorningstar/morning_limit.png`

 * *Files identical despite different names*

### Comparing `pymorningstar-0.21/setup.py` & `pymorningstar-0.22/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='pymorningstar', 
-    version='0.21',
+    version='0.22',
     description = "Automating the download of information from Morningstar's Excel Add-In API",
     author = 'Pablo Vilas',
     author_email='pablo.vilas.naval@gmail.com',
     packages = ['pymorningstar'],
     install_requires=['xlwings','pandas','pyautogui', 'opencv-python', 'Pillow'],
     url='https://github.com/VilasPablo/pymorningstar',
     classifiers=[
```


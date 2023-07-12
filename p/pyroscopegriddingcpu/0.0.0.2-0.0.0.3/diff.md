# Comparing `tmp/pyroscopegriddingcpu-0.0.0.2.tar.gz` & `tmp/pyroscopegriddingcpu-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscopegriddingcpu-0.0.0.2.tar", last modified: Wed Jul 12 18:57:53 2023, max compression
+gzip compressed data, was "pyroscopegriddingcpu-0.0.0.3.tar", last modified: Wed Jul 12 19:02:06 2023, max compression
```

## Comparing `pyroscopegriddingcpu-0.0.0.2.tar` & `pyroscopegriddingcpu-0.0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 18:57:53.775836 pyroscopegriddingcpu-0.0.0.2/
--rw-rw-rw-   0        0        0     1077 2023-04-06 22:17:54.000000 pyroscopegriddingcpu-0.0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0    11069 2023-07-12 18:57:53.775836 pyroscopegriddingcpu-0.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     9962 2023-04-06 22:20:54.000000 pyroscopegriddingcpu-0.0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 18:57:53.729003 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/
--rw-rw-rw-   0        0        0      247 2023-07-12 16:34:35.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/__init__.py
--rw-rw-rw-   0        0        0     3506 2023-07-12 16:24:51.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/fileparser.py
--rw-rw-rw-   0        0        0    10415 2023-07-12 16:27:48.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/filter_data.py
--rw-rw-rw-   0        0        0    30817 2023-07-12 16:27:22.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/grid_ncf.py
--rw-rw-rw-   0        0        0     6323 2023-07-12 18:27:40.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/gridding.py
--rw-rw-rw-   0        0        0    26374 2023-07-12 16:34:02.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/gtools.py
--rw-rw-rw-   0        0        0     9373 2023-07-12 16:33:56.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/naming_conventions.py
--rw-rw-rw-   0        0        0    13976 2023-07-12 16:33:50.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/sat_data_input.py
--rw-rw-rw-   0        0        0     6275 2023-07-12 15:44:36.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/solar_zenith.py
--rw-rw-rw-   0        0        0     5191 2023-07-12 16:34:13.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/time_conv.py
-drwxrwxrwx   0        0        0        0 2023-07-12 18:57:53.760213 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/
--rw-rw-rw-   0        0        0    11069 2023-07-12 18:57:53.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      650 2023-07-12 18:57:53.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 18:57:53.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-07-12 18:57:53.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-07-12 18:57:53.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-12 18:57:53.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 18:57:53.775836 pyroscopegriddingcpu-0.0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1908 2023-07-12 18:42:08.000000 pyroscopegriddingcpu-0.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:02:06.781079 pyroscopegriddingcpu-0.0.0.3/
+-rw-rw-rw-   0        0        0     1077 2023-04-06 22:17:54.000000 pyroscopegriddingcpu-0.0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    11069 2023-07-12 19:02:06.781079 pyroscopegriddingcpu-0.0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9962 2023-04-06 22:20:54.000000 pyroscopegriddingcpu-0.0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 19:02:06.734671 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/
+-rw-rw-rw-   0        0        0      247 2023-07-12 16:34:35.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/__init__.py
+-rw-rw-rw-   0        0        0     3506 2023-07-12 16:24:51.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/fileparser.py
+-rw-rw-rw-   0        0        0    10415 2023-07-12 16:27:48.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/filter_data.py
+-rw-rw-rw-   0        0        0    30817 2023-07-12 16:27:22.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/grid_ncf.py
+-rw-rw-rw-   0        0        0     6323 2023-07-12 18:27:40.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/gridding.py
+-rw-rw-rw-   0        0        0    26374 2023-07-12 16:34:02.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/gtools.py
+-rw-rw-rw-   0        0        0     9373 2023-07-12 16:33:56.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/naming_conventions.py
+-rw-rw-rw-   0        0        0    13976 2023-07-12 16:33:50.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/sat_data_input.py
+-rw-rw-rw-   0        0        0     6275 2023-07-12 15:44:36.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/solar_zenith.py
+-rw-rw-rw-   0        0        0     5191 2023-07-12 16:34:13.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/time_conv.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:02:06.781079 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu.egg-info/
+-rw-rw-rw-   0        0        0    11069 2023-07-12 19:02:06.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      650 2023-07-12 19:02:06.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 19:02:06.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-07-12 19:02:06.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       84 2023-07-12 19:02:06.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-12 19:02:06.000000 pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 19:02:06.781079 pyroscopegriddingcpu-0.0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1914 2023-07-12 19:01:52.000000 pyroscopegriddingcpu-0.0.0.3/setup.py
```

### Comparing `pyroscopegriddingcpu-0.0.0.2/LICENSE.txt` & `pyroscopegriddingcpu-0.0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.2/PKG-INFO` & `pyroscopegriddingcpu-0.0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegriddingcpu
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Keywords: data fusion,satellite,L2,L3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyroscopegriddingcpu-0.0.0.2/README.md` & `pyroscopegriddingcpu-0.0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/fileparser.py` & `pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/filter_data.py` & `pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/grid_ncf.py` & `pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/grid_ncf.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/gridding.py` & `pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/gtools.py` & `pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/gtools.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/naming_conventions.py` & `pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/sat_data_input.py` & `pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/solar_zenith.py` & `pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/time_conv.py` & `pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/PKG-INFO` & `pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegriddingcpu
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Keywords: data fusion,satellite,L2,L3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/SOURCES.txt` & `pyroscopegriddingcpu-0.0.0.3/pyroscopegriddingcpu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.2/setup.py` & `pyroscopegriddingcpu-0.0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,37 +5,38 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name = 'pyroscopegriddingcpu',         # Package name
     packages = ['pyroscopegriddingcpu'],   
-    version = '0.0.0.2',      # Initial version
+    version = '0.0.0.3',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     long_description = long_description,
     long_description_content_type='text/markdown',
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository  
     keywords = ['data fusion', 'satellite', 'L2', 'L3'],   # Keywords
     #packages = find_packages(),
     entry_points ={
         'console_scripts': [
             'pyroscopegriddingcpu = pyroscopegriddingcpu.gtools:main',
         ],
     },
-    install_requires=[            
+    install_requires=[    
+            'pyhdf',        
             'numpy ==1.23.5',
             'joblib ==1.2.0',
             'netCDF4 ==1.6.3',
-            'pyhdf ==0.10.5',
+            'pandas ==2.0.0',
             'pyyaml ==6.0',
             'argparse',
-            'pandas ==2.0.0'
+            
         ],
     classifiers=[
     'Development Status :: 3 - Alpha',     
     'Intended Audience :: Developers',     
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   
     'Programming Language :: Python :: 3',      #supported versions
```


# Comparing `tmp/pharaglow-0.9.0.tar.gz` & `tmp/pharaglow-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/valerio/pharaglow/dist/.tmp-fyaoptc3/pharaglow-0.9.0.tar", last modified: Wed Jun 21 07:12:43 2023, max compression
+gzip compressed data, was "/home/runner/work/PharaGlow/PharaGlow/dist/.tmp-b8ee22f5/pharaglow-0.9.3.tar", last modified: Wed Jul 12 09:25:09 2023, max compression
```

## Comparing `pharaglow-0.9.0.tar` & `pharaglow-0.9.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 07:12:42.000000 pharaglow-0.9.0/
--rwxrwxr-x   0 valerio   (1000) valerio   (1000)    35149 2023-05-01 18:39:04.000000 pharaglow-0.9.0/LICENSE
--rw-rw-r--   0 valerio   (1000) valerio   (1000)    51379 2023-06-21 07:12:42.000000 pharaglow-0.9.0/PKG-INFO
--rwxrwxr-x   0 valerio   (1000) valerio   (1000)     9644 2023-05-01 18:39:04.000000 pharaglow-0.9.0/README.md
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 07:12:42.000000 pharaglow-0.9.0/pharaglow/
--rwxrwxr-x   0 valerio   (1000) valerio   (1000)       23 2023-05-01 18:39:04.000000 pharaglow-0.9.0/pharaglow/__init__.py
--rwxrwxr-x   0 valerio   (1000) valerio   (1000)    12843 2023-05-01 18:39:04.000000 pharaglow-0.9.0/pharaglow/extract.py
--rwxrwxr-x   0 valerio   (1000) valerio   (1000)    13985 2023-05-01 18:39:04.000000 pharaglow-0.9.0/pharaglow/features.py
--rwxrwxr-x   0 valerio   (1000) valerio   (1000)     2409 2023-05-01 18:39:04.000000 pharaglow-0.9.0/pharaglow/io.py
--rwxrwxr-x   0 valerio   (1000) valerio   (1000)     8552 2023-05-01 18:39:04.000000 pharaglow-0.9.0/pharaglow/run.py
--rwxrwxr-x   0 valerio   (1000) valerio   (1000)    21947 2023-05-01 18:39:04.000000 pharaglow-0.9.0/pharaglow/tracking.py
--rwxrwxr-x   0 valerio   (1000) valerio   (1000)     7210 2023-05-01 18:39:04.000000 pharaglow-0.9.0/pharaglow/util.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 07:12:42.000000 pharaglow-0.9.0/pharaglow.egg-info/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)    51379 2023-06-21 07:12:42.000000 pharaglow-0.9.0/pharaglow.egg-info/PKG-INFO
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      353 2023-06-21 07:12:42.000000 pharaglow-0.9.0/pharaglow.egg-info/SOURCES.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        1 2023-06-21 07:12:42.000000 pharaglow-0.9.0/pharaglow.egg-info/dependency_links.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       70 2023-06-21 07:12:42.000000 pharaglow-0.9.0/pharaglow.egg-info/requires.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       10 2023-06-21 07:12:42.000000 pharaglow-0.9.0/pharaglow.egg-info/top_level.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     4316 2023-06-21 07:11:23.000000 pharaglow-0.9.0/pyproject.toml
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       74 2023-06-21 07:12:43.000000 pharaglow-0.9.0/setup.cfg
--rwxrwxr-x   0 valerio   (1000) valerio   (1000)      655 2023-06-19 13:12:50.000000 pharaglow-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:25:09.000000 pharaglow-0.9.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-07-12 09:24:31.000000 pharaglow-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    51640 2023-07-12 09:25:09.000000 pharaglow-0.9.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9744 2023-07-12 09:24:31.000000 pharaglow-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:25:09.000000 pharaglow-0.9.3/pharaglow/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-07-12 09:24:32.000000 pharaglow-0.9.3/pharaglow/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12843 2023-07-12 09:24:32.000000 pharaglow-0.9.3/pharaglow/extract.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13985 2023-07-12 09:24:32.000000 pharaglow-0.9.3/pharaglow/features.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2409 2023-07-12 09:24:32.000000 pharaglow-0.9.3/pharaglow/io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8552 2023-07-12 09:24:32.000000 pharaglow-0.9.3/pharaglow/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22543 2023-07-12 09:24:32.000000 pharaglow-0.9.3/pharaglow/tracking.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7210 2023-07-12 09:24:32.000000 pharaglow-0.9.3/pharaglow/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:25:09.000000 pharaglow-0.9.3/pharaglow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    51640 2023-07-12 09:25:09.000000 pharaglow-0.9.3/pharaglow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-12 09:25:09.000000 pharaglow-0.9.3/pharaglow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:25:09.000000 pharaglow-0.9.3/pharaglow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 09:25:09.000000 pharaglow-0.9.3/pharaglow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 09:25:09.000000 pharaglow-0.9.3/pharaglow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:24:48.000000 pharaglow-0.9.3/pharaglow.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-12 09:24:32.000000 pharaglow-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-12 09:25:09.000000 pharaglow-0.9.3/setup.cfg
```

### Comparing `pharaglow-0.9.0/LICENSE` & `pharaglow-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pharaglow-0.9.0/PKG-INFO` & `pharaglow-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: pharaglow
-Version: 0.9.0
+Version: 0.9.3
 Summary: A toolset to analyze videos of foraging animals.
+Home-page: https://github.com/scholz-lab/PharaGlow
 Author: M.Scholz
 Author-email: "M.Scholz" <monika.k.scholz@gmail.com>
+Maintainer: Omar Valerio
 Maintainer-email: Omar Valerio <omar.valerio@mpinb.mpg.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -679,103 +681,107 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: PharaGlow Homepage, https://github.com/scholz-lab/PharaGlow
 Project-URL: Bug Reports, https://github.com/scholz-lab/PharaGlow/issues
 Project-URL: Source, https://github.com/scholz-lab/PharaGlow
+Project-URL: API Reference, https://scholz-lab.github.io/PharaGlow/build/html/pharaglow.html
 Keywords: toolset,tracking,feeding,behaviour,pumping
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
 
+
+![](examples/pglowLogo.png)
+<!-- ![](https://raw.githubusercontent.com/scholz-lab/PharaGlow/master/examples/pglowLogo.png) -->
 # PharaGlow - tracking locomotion and feeding behavior of moving worms
 
-![png](examples/pglow_header.png)
+<!-- ![](https://raw.githubusercontent.com/scholz-lab/PharaGlow/master/examples/pglow_header.png) -->
 
 PharaGlow is a python package for tracking and analyzing *C. elegans* motion and feeding behavior from videos.
  The package can be used to simply track labelled pharynxes
  (or whole animals from brightfield) as a simple center of mass tracker,
  but it also has a pipeline to extract pharyngeal pumping and features of the pharynx.
 
 ## Installation
 
 1. Install Anaconda
 You need to have Anaconda (https://www.anaconda.com/products/individual) and Python >=3.7.
 We recommend using Anaconda to install Python.
 
+2. Create and activate a new `conda` environment
 
-2. Clone PharaGlow repository from Github in your local directory
- 
- * Copy the repository link from Github in https://github.com/scholz-lab/PharaGlow/
- (in Branch Master > Code > HTTPS (OR SSH))
- 
- *  In the terminal (Linux)/Anaconda Command Prompt (Windows),
- navigate to the directory where to clone PharaGlow
- and write the git clone command:
-
-```
-git clone https://github.com/scholz-lab/PharaGlow.git
-```
-
-Note that you can also download PharaGlow from our Github repository
- (Branch Master > Code > Download ZIP)
-to have the current copy of PharaGlow.
-
-3. Create and activate the required anaconda environment
-In the terminal (Linux)/Anaconda Command Prompt (Windows),
- naviguate to your newly cloned PharaGlow directory
- and run:
+In the terminal (Linux)/Anaconda Command Prompt (Windows) run:
 
 ```bash
-conda env create --file environmentPumping.yml
+conda env create --name pumping
 ```
 
 You can now use this environment by running:
 
 ```
 conda activate pumping
 ```
 
+3. Install PharaGlow package from PyPI using pip
+
+```
+python -m pip install pharaglow
+``` 
 
-4. Install PharaGlow
+Alternatively you can clone PharaGlow repository from Github
+ 
+ * Copy the repository link from Github in https://github.com/scholz-lab/PharaGlow/
+ 
+ *  In the terminal (Linux)/Anaconda Command Prompt (Windows),
+ navigate to the directory where you wish to download PharaGlow
+ and enter the command:
 
-Last step, (don't forget to activate the pumping environment) run: 
 ```
-python setup.py install --user
+git clone https://github.com/scholz-lab/PharaGlow.git pharaglow
 ```
-in the main directory of the software, which has the file called setup.py
+Change to the pharaglow directory and run:
+ 
+```
+cd pharaglow
+conda activate pumping
+pip install -e .
+```
+in the main directory of the software, which has the file called `pyproject.toml`
 
-5. (*optional*)
+5. (*Optional*)
  *Create a dedicated environment kernel*
 
 ```
 conda activate pumping
 python -m ipykernel install --user --name pumping --display-name "Python (pumping)"
 ```
 
 *And remove notebook output before committing*
 
 ```
 conda install -c conda-forge nbstripout
 ```
 ## Overview
 
+![](https://raw.githubusercontent.com/scholz-lab/PharaGlow/master/examples/pglow_header.png)
+
+
 **1. Step -  Basic object detection**
     This step creates a "_features.json" file
 	which contains a table of objects (worms) detected in each frame.
 	It creates also a stack of images that contain a cropped area around each worm.
     
 **2. Step - Linking objects into trajectories**
     This step results in individual files "_trajectory.json" and _images.tiff for each tracked animal.
```

### Comparing `pharaglow-0.9.0/README.md` & `pharaglow-0.9.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,79 +1,83 @@
+
+![](examples/pglowLogo.png)
+<!-- ![](https://raw.githubusercontent.com/scholz-lab/PharaGlow/master/examples/pglowLogo.png) -->
 # PharaGlow - tracking locomotion and feeding behavior of moving worms
 
-![png](examples/pglow_header.png)
+<!-- ![](https://raw.githubusercontent.com/scholz-lab/PharaGlow/master/examples/pglow_header.png) -->
 
 PharaGlow is a python package for tracking and analyzing *C. elegans* motion and feeding behavior from videos.
  The package can be used to simply track labelled pharynxes
  (or whole animals from brightfield) as a simple center of mass tracker,
  but it also has a pipeline to extract pharyngeal pumping and features of the pharynx.
 
 ## Installation
 
 1. Install Anaconda
 You need to have Anaconda (https://www.anaconda.com/products/individual) and Python >=3.7.
 We recommend using Anaconda to install Python.
 
+2. Create and activate a new `conda` environment
 
-2. Clone PharaGlow repository from Github in your local directory
- 
- * Copy the repository link from Github in https://github.com/scholz-lab/PharaGlow/
- (in Branch Master > Code > HTTPS (OR SSH))
- 
- *  In the terminal (Linux)/Anaconda Command Prompt (Windows),
- navigate to the directory where to clone PharaGlow
- and write the git clone command:
-
-```
-git clone https://github.com/scholz-lab/PharaGlow.git
-```
-
-Note that you can also download PharaGlow from our Github repository
- (Branch Master > Code > Download ZIP)
-to have the current copy of PharaGlow.
-
-3. Create and activate the required anaconda environment
-In the terminal (Linux)/Anaconda Command Prompt (Windows),
- naviguate to your newly cloned PharaGlow directory
- and run:
+In the terminal (Linux)/Anaconda Command Prompt (Windows) run:
 
 ```bash
-conda env create --file environmentPumping.yml
+conda env create --name pumping
 ```
 
 You can now use this environment by running:
 
 ```
 conda activate pumping
 ```
 
+3. Install PharaGlow package from PyPI using pip
+
+```
+python -m pip install pharaglow
+``` 
 
-4. Install PharaGlow
+Alternatively you can clone PharaGlow repository from Github
+ 
+ * Copy the repository link from Github in https://github.com/scholz-lab/PharaGlow/
+ 
+ *  In the terminal (Linux)/Anaconda Command Prompt (Windows),
+ navigate to the directory where you wish to download PharaGlow
+ and enter the command:
 
-Last step, (don't forget to activate the pumping environment) run: 
 ```
-python setup.py install --user
+git clone https://github.com/scholz-lab/PharaGlow.git pharaglow
 ```
-in the main directory of the software, which has the file called setup.py
+Change to the pharaglow directory and run:
+ 
+```
+cd pharaglow
+conda activate pumping
+pip install -e .
+```
+in the main directory of the software, which has the file called `pyproject.toml`
 
-5. (*optional*)
+5. (*Optional*)
  *Create a dedicated environment kernel*
 
 ```
 conda activate pumping
 python -m ipykernel install --user --name pumping --display-name "Python (pumping)"
 ```
 
 *And remove notebook output before committing*
 
 ```
 conda install -c conda-forge nbstripout
 ```
 ## Overview
 
+![](https://raw.githubusercontent.com/scholz-lab/PharaGlow/master/examples/pglow_header.png)
+
+
 **1. Step -  Basic object detection**
     This step creates a "_features.json" file
 	which contains a table of objects (worms) detected in each frame.
 	It creates also a stack of images that contain a cropped area around each worm.
     
 **2. Step - Linking objects into trajectories**
     This step results in individual files "_trajectory.json" and _images.tiff for each tracked animal.
```

### Comparing `pharaglow-0.9.0/pharaglow/extract.py` & `pharaglow-0.9.3/pharaglow/extract.py`

 * *Files identical despite different names*

### Comparing `pharaglow-0.9.0/pharaglow/features.py` & `pharaglow-0.9.3/pharaglow/features.py`

 * *Files identical despite different names*

### Comparing `pharaglow-0.9.0/pharaglow/io.py` & `pharaglow-0.9.3/pharaglow/io.py`

 * *Files identical despite different names*

### Comparing `pharaglow-0.9.0/pharaglow/run.py` & `pharaglow-0.9.3/pharaglow/run.py`

 * *Files identical despite different names*

### Comparing `pharaglow-0.9.0/pharaglow/tracking.py` & `pharaglow-0.9.3/pharaglow/tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,18 @@
         bg = filters.gaussian(img, s, preserve_range = True)
         img = filters.gaussian(img-bg, 1)
         img[img<0] = 0
         img = img.astype(int)
         # mask
         mask = img>filters.threshold_li(img, initial_guess = np.min)
         mask = ndi.binary_closing(mask)
-        mask = morphology.remove_small_objects(mask, min_size=min_size, connectivity=2, in_place=True)
+        #NOTE: in_place argument is deprecated. The default behavior is creating a new array.
+        #REF: https://scikit-image.org/docs/stable/api/skimage.morphology.html#skimage.morphology.remove_small_objects
+        #mask = morphology.remove_small_objects(mask, min_size=min_size, connectivity=2, in_place=True)
+        mask = morphology.remove_small_objects(mask, min_size=min_size, connectivity=2)
         labelled, num = label(mask, background=0, connectivity = 2,return_num=True)
         if num ==2:
             min_mask = labelled
         if num<current_no and num>0:
             min_mask = labelled
             current_no = num
     min_mask = min_mask.astype(int)
@@ -225,15 +228,18 @@
     Returns:
         pandas.Dataframe, list: dataframe with information for each image, list of corresponding images.
     """
     assert mask.shape == img.shape, 'Image and Mask size do not match.'
     df = pd.DataFrame()
     crop_images = []
     label_image = measure.label(mask, background=0, connectivity = 1)
-    label_image = segmentation.clear_border(label_image, buffer_size=0, bgval=0, in_place=False, mask=None)
+    #label_image = segmentation.clear_border(label_image, buffer_size=0, bgval=0, in_place=False, mask=None)
+    #NOTE: in_place argument is deprecated. The default behavior is creating a new array.
+    #REF: https://scikit-image.org/docs/stable/api/skimage.segmentation.html#skimage.segmentation.clear_border
+    label_image = segmentation.clear_border(label_image, buffer_size=0, bgval=0, mask=None)
 
     for region in measure.regionprops(label_image, intensity_image=img):
         if region.area > params['minSize'] and region.area < params['maxSize']:
             # get the image of an object
             im, sliced = extractImagePad(img, region.bbox, params['pad'], mask=label_image==region.label)
             bbox = [sliced[0].start, sliced[1].start, sliced[0].stop, sliced[1].stop]
             # bbox is min_row, min_col, max_row, max_col
```

### Comparing `pharaglow-0.9.0/pharaglow/util.py` & `pharaglow-0.9.3/pharaglow/util.py`

 * *Files identical despite different names*

### Comparing `pharaglow-0.9.0/pharaglow.egg-info/PKG-INFO` & `pharaglow-0.9.3/pharaglow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: pharaglow
-Version: 0.9.0
+Version: 0.9.3
 Summary: A toolset to analyze videos of foraging animals.
+Home-page: https://github.com/scholz-lab/PharaGlow
 Author: M.Scholz
 Author-email: "M.Scholz" <monika.k.scholz@gmail.com>
+Maintainer: Omar Valerio
 Maintainer-email: Omar Valerio <omar.valerio@mpinb.mpg.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -679,103 +681,107 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: PharaGlow Homepage, https://github.com/scholz-lab/PharaGlow
 Project-URL: Bug Reports, https://github.com/scholz-lab/PharaGlow/issues
 Project-URL: Source, https://github.com/scholz-lab/PharaGlow
+Project-URL: API Reference, https://scholz-lab.github.io/PharaGlow/build/html/pharaglow.html
 Keywords: toolset,tracking,feeding,behaviour,pumping
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
 
+
+![](examples/pglowLogo.png)
+<!-- ![](https://raw.githubusercontent.com/scholz-lab/PharaGlow/master/examples/pglowLogo.png) -->
 # PharaGlow - tracking locomotion and feeding behavior of moving worms
 
-![png](examples/pglow_header.png)
+<!-- ![](https://raw.githubusercontent.com/scholz-lab/PharaGlow/master/examples/pglow_header.png) -->
 
 PharaGlow is a python package for tracking and analyzing *C. elegans* motion and feeding behavior from videos.
  The package can be used to simply track labelled pharynxes
  (or whole animals from brightfield) as a simple center of mass tracker,
  but it also has a pipeline to extract pharyngeal pumping and features of the pharynx.
 
 ## Installation
 
 1. Install Anaconda
 You need to have Anaconda (https://www.anaconda.com/products/individual) and Python >=3.7.
 We recommend using Anaconda to install Python.
 
+2. Create and activate a new `conda` environment
 
-2. Clone PharaGlow repository from Github in your local directory
- 
- * Copy the repository link from Github in https://github.com/scholz-lab/PharaGlow/
- (in Branch Master > Code > HTTPS (OR SSH))
- 
- *  In the terminal (Linux)/Anaconda Command Prompt (Windows),
- navigate to the directory where to clone PharaGlow
- and write the git clone command:
-
-```
-git clone https://github.com/scholz-lab/PharaGlow.git
-```
-
-Note that you can also download PharaGlow from our Github repository
- (Branch Master > Code > Download ZIP)
-to have the current copy of PharaGlow.
-
-3. Create and activate the required anaconda environment
-In the terminal (Linux)/Anaconda Command Prompt (Windows),
- naviguate to your newly cloned PharaGlow directory
- and run:
+In the terminal (Linux)/Anaconda Command Prompt (Windows) run:
 
 ```bash
-conda env create --file environmentPumping.yml
+conda env create --name pumping
 ```
 
 You can now use this environment by running:
 
 ```
 conda activate pumping
 ```
 
+3. Install PharaGlow package from PyPI using pip
+
+```
+python -m pip install pharaglow
+``` 
 
-4. Install PharaGlow
+Alternatively you can clone PharaGlow repository from Github
+ 
+ * Copy the repository link from Github in https://github.com/scholz-lab/PharaGlow/
+ 
+ *  In the terminal (Linux)/Anaconda Command Prompt (Windows),
+ navigate to the directory where you wish to download PharaGlow
+ and enter the command:
 
-Last step, (don't forget to activate the pumping environment) run: 
 ```
-python setup.py install --user
+git clone https://github.com/scholz-lab/PharaGlow.git pharaglow
 ```
-in the main directory of the software, which has the file called setup.py
+Change to the pharaglow directory and run:
+ 
+```
+cd pharaglow
+conda activate pumping
+pip install -e .
+```
+in the main directory of the software, which has the file called `pyproject.toml`
 
-5. (*optional*)
+5. (*Optional*)
  *Create a dedicated environment kernel*
 
 ```
 conda activate pumping
 python -m ipykernel install --user --name pumping --display-name "Python (pumping)"
 ```
 
 *And remove notebook output before committing*
 
 ```
 conda install -c conda-forge nbstripout
 ```
 ## Overview
 
+![](https://raw.githubusercontent.com/scholz-lab/PharaGlow/master/examples/pglow_header.png)
+
+
 **1. Step -  Basic object detection**
     This step creates a "_features.json" file
 	which contains a table of objects (worms) detected in each frame.
 	It creates also a stack of images that contain a cropped area around each worm.
     
 **2. Step - Linking objects into trajectories**
     This step results in individual files "_trajectory.json" and _images.tiff for each tracked animal.
```


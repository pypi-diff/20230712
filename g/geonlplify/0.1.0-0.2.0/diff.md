# Comparing `tmp/GeoNLPlify-0.1.0.tar.gz` & `tmp/geonlplify-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/rdecoupe/PycharmProjects/geonlplify/dist/.tmp-n6huebeh/GeoNLPlify-0.1.0.tar", last modified: Mon Nov 28 16:26:00 2022, max compression
+gzip compressed data, was "dist/geonlplify-0.2.0.tar", last modified: Wed Jul 12 09:44:19 2023, max compression
```

## Comparing `GeoNLPlify-0.1.0.tar` & `geonlplify-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rdecoupe  (1000) rdecoupe  (1000)        0 2022-11-28 16:26:00.000000 GeoNLPlify-0.1.0/
-drwxr-xr-x   0 rdecoupe  (1000) rdecoupe  (1000)        0 2022-11-28 16:26:00.000000 GeoNLPlify-0.1.0/GeoNLPlify.egg-info/
--rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)     3126 2022-11-28 16:26:00.000000 GeoNLPlify-0.1.0/GeoNLPlify.egg-info/PKG-INFO
--rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)      302 2022-11-28 16:26:00.000000 GeoNLPlify-0.1.0/GeoNLPlify.egg-info/SOURCES.txt
--rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)        1 2022-11-28 16:26:00.000000 GeoNLPlify-0.1.0/GeoNLPlify.egg-info/dependency_links.txt
--rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)       22 2022-11-28 16:26:00.000000 GeoNLPlify-0.1.0/GeoNLPlify.egg-info/requires.txt
--rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)       16 2022-11-28 16:26:00.000000 GeoNLPlify-0.1.0/GeoNLPlify.egg-info/top_level.txt
--rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)    35149 2022-11-28 15:19:22.000000 GeoNLPlify-0.1.0/LICENSE
--rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)     3126 2022-11-28 16:26:00.000000 GeoNLPlify-0.1.0/PKG-INFO
--rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)     2413 2022-11-24 15:01:52.000000 GeoNLPlify-0.1.0/README.md
-drwxr-xr-x   0 rdecoupe  (1000) rdecoupe  (1000)        0 2022-11-28 16:26:00.000000 GeoNLPlify-0.1.0/geonlplify/
--rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)      147 2022-11-28 14:13:10.000000 GeoNLPlify-0.1.0/geonlplify/__init__.py
--rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)     7878 2022-11-28 14:34:15.000000 GeoNLPlify-0.1.0/geonlplify/geonlplify.py
--rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)      742 2022-11-28 16:25:07.000000 GeoNLPlify-0.1.0/pyproject.toml
--rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)       38 2022-11-28 16:26:00.000000 GeoNLPlify-0.1.0/setup.cfg
--rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)      575 2022-11-28 14:00:19.000000 GeoNLPlify-0.1.0/setup.py
-drwxr-xr-x   0 rdecoupe  (1000) rdecoupe  (1000)        0 2022-11-28 16:26:00.000000 GeoNLPlify-0.1.0/test/
--rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)        0 2022-11-08 16:39:22.000000 GeoNLPlify-0.1.0/test/__init__.py
--rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)      180 2022-11-08 17:28:24.000000 GeoNLPlify-0.1.0/test/manipulate_package.py
+drwxr-xr-x   0 rdecoupe  (1000) rdecoupe  (1000)        0 2023-07-12 09:44:19.000000 geonlplify-0.2.0/
+-rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)    35149 2022-11-28 15:19:22.000000 geonlplify-0.2.0/LICENSE
+-rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)     3487 2023-07-12 09:44:19.000000 geonlplify-0.2.0/PKG-INFO
+-rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)     3038 2023-07-12 09:19:44.000000 geonlplify-0.2.0/README.md
+drwxr-xr-x   0 rdecoupe  (1000) rdecoupe  (1000)        0 2023-07-12 09:44:19.000000 geonlplify-0.2.0/geonlplify/
+-rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)      147 2022-11-28 14:13:10.000000 geonlplify-0.2.0/geonlplify/__init__.py
+-rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)     7570 2023-07-12 09:14:29.000000 geonlplify-0.2.0/geonlplify/geonlplify.py
+drwxr-xr-x   0 rdecoupe  (1000) rdecoupe  (1000)        0 2023-07-12 09:44:19.000000 geonlplify-0.2.0/geonlplify.egg-info/
+-rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)     3487 2023-07-12 09:44:19.000000 geonlplify-0.2.0/geonlplify.egg-info/PKG-INFO
+-rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)      302 2023-07-12 09:44:19.000000 geonlplify-0.2.0/geonlplify.egg-info/SOURCES.txt
+-rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)        1 2023-07-12 09:44:19.000000 geonlplify-0.2.0/geonlplify.egg-info/dependency_links.txt
+-rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)       22 2023-07-12 09:44:19.000000 geonlplify-0.2.0/geonlplify.egg-info/requires.txt
+-rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)       16 2023-07-12 09:44:19.000000 geonlplify-0.2.0/geonlplify.egg-info/top_level.txt
+-rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)      742 2022-11-28 16:25:07.000000 geonlplify-0.2.0/pyproject.toml
+-rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)       38 2023-07-12 09:44:19.000000 geonlplify-0.2.0/setup.cfg
+-rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)      624 2023-07-12 09:43:06.000000 geonlplify-0.2.0/setup.py
+drwxr-xr-x   0 rdecoupe  (1000) rdecoupe  (1000)        0 2023-07-12 09:44:19.000000 geonlplify-0.2.0/test/
+-rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)        0 2022-11-08 16:39:22.000000 geonlplify-0.2.0/test/__init__.py
+-rw-r--r--   0 rdecoupe  (1000) rdecoupe  (1000)      339 2023-07-12 08:55:09.000000 geonlplify-0.2.0/test/manipulate_package.py
```

### Comparing `GeoNLPlify-0.1.0/GeoNLPlify.egg-info/PKG-INFO` & `geonlplify-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 Metadata-Version: 2.1
-Name: GeoNLPlify
-Version: 0.1.0
-Summary: A NLP library for data augmentation focusing on spatial information contained in text.
-Home-page: 
+Name: geonlplify
+Version: 0.2.0
+Summary: GeoNLPlify aims to make variations of an input sentence working on spatial information contained in words
+Home-page: UNKNOWN
 Author: Rémy Decoupes
-Author-email: Rémy Decoupes <remy.decoupes@inrae.fr>
-Project-URL: Homepage, https://github.com/remydecoupes/GeoNLPlify
-Project-URL: Bug Tracker, https://github.com/remydecoupes/GeoNLPlify/issues
-Project-URL: Documentation, https://geonlplify.readthedocs.io/en/latest/
+Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center"> GeoNLPlify
 :earth_africa: :book:
 </h1>
 
 [![Documentation Status](https://readthedocs.org/projects/geonlplify/badge/?version=latest)](https://geonlplify.readthedocs.io/en/latest/?badge=latest)
+![GitHub](https://img.shields.io/github/license/remydecoupes/GeoNLPlify)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/remydecoupes/GeoNLPlify)
 
 A NLP library for data augmentation focusing on spatial information contained in text.
 
-<p align="center">
-  <img src="./readme_ressources/geonlplify_example_schema.png" />
-</p>
+![geonplify_schema](./readme_ressources/geonlplify_example_schema.png)
 
 
 ## Usage
 ```python
 import geonlplify
 
 my_text = "My name is Clara and I live in Berkeley."
 geonlplify.geonlplify(my_text)
 ```
 ```bash
 'My name is Clara and I live in Bristol'
 ```
 
 ## Installation
-You can install GeoNLPlify in three ways: in a [virtual_env](#virtual-environment), in a [conda environment](#conda-environment), or using :construction: [pip](#pip-install)
+```bash
+pip install GeoNLPlify
+# Download data. Please visit Simplemaps: https://simplemaps.com/data/world-cities
+python3 -c "from geonlplify import download_simplemaps_data; download_simplemaps_data()"
+# Download spacy model
+python -m spacy download en_core_web_trf  
+```
+
+## Contributions
+You can install GeoNLPlify in three ways: in a [virtual_env](#virtual-environment), in a [conda environment](#conda-environment)
 ### Virtual Environment
 1. Git clone this repository
   ```bash
   git clone https://github.com/remydecoupes/GeoNLPlify.git
   ```
 2. Create a virtual env
   ```bash
@@ -77,16 +84,21 @@
   ```bash 
   python -m spacy download en_core_web_trf
   ```
 4. Donwload [world-cities from simple maps](https://simplemaps.com/data/world-cities)
   ```bash
   wget -qO- https://simplemaps.com/static/data/world-cities/basic/simplemaps_worldcities_basicv1.75.zip  | bsdtar -xvf- -C ./geonlplify/simplemaps/
   ```
-### Pip install
-:construction: **Packaging in progress** :construction:
 
 ## Acknowledgement
 :pray: This library use those terrific tools/libraries/data :muscle::
 + [Spacy](https://spacy.io/)
 + [The Komoot geocoder Photon](https://photon.komoot.io/)
 + [OpenStreeMap](https://www.openstreetmap.org/copyright)
 + [Simplemaps data](https://simplemaps.com/data/world-cities)
+
+## Scientific publication
+| Conference   |      paper      |  description |
+|----------|:-------------:|------:|
+| [EGC'2023](https://egc2023.sciencesconf.org/) |  [short paper (in French)](https://editions-rnti.fr/?inprocid=1002848) | [video](https://youtu.be/-QaTBtjWr9g) |
+
+
```

### Comparing `GeoNLPlify-0.1.0/LICENSE` & `geonlplify-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GeoNLPlify-0.1.0/PKG-INFO` & `geonlplify-0.2.0/geonlplify.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 Metadata-Version: 2.1
-Name: GeoNLPlify
-Version: 0.1.0
-Summary: A NLP library for data augmentation focusing on spatial information contained in text.
-Home-page: 
+Name: geonlplify
+Version: 0.2.0
+Summary: GeoNLPlify aims to make variations of an input sentence working on spatial information contained in words
+Home-page: UNKNOWN
 Author: Rémy Decoupes
-Author-email: Rémy Decoupes <remy.decoupes@inrae.fr>
-Project-URL: Homepage, https://github.com/remydecoupes/GeoNLPlify
-Project-URL: Bug Tracker, https://github.com/remydecoupes/GeoNLPlify/issues
-Project-URL: Documentation, https://geonlplify.readthedocs.io/en/latest/
+Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center"> GeoNLPlify
 :earth_africa: :book:
 </h1>
 
 [![Documentation Status](https://readthedocs.org/projects/geonlplify/badge/?version=latest)](https://geonlplify.readthedocs.io/en/latest/?badge=latest)
+![GitHub](https://img.shields.io/github/license/remydecoupes/GeoNLPlify)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/remydecoupes/GeoNLPlify)
 
 A NLP library for data augmentation focusing on spatial information contained in text.
 
-<p align="center">
-  <img src="./readme_ressources/geonlplify_example_schema.png" />
-</p>
+![geonplify_schema](./readme_ressources/geonlplify_example_schema.png)
 
 
 ## Usage
 ```python
 import geonlplify
 
 my_text = "My name is Clara and I live in Berkeley."
 geonlplify.geonlplify(my_text)
 ```
 ```bash
 'My name is Clara and I live in Bristol'
 ```
 
 ## Installation
-You can install GeoNLPlify in three ways: in a [virtual_env](#virtual-environment), in a [conda environment](#conda-environment), or using :construction: [pip](#pip-install)
+```bash
+pip install GeoNLPlify
+# Download data. Please visit Simplemaps: https://simplemaps.com/data/world-cities
+python3 -c "from geonlplify import download_simplemaps_data; download_simplemaps_data()"
+# Download spacy model
+python -m spacy download en_core_web_trf  
+```
+
+## Contributions
+You can install GeoNLPlify in three ways: in a [virtual_env](#virtual-environment), in a [conda environment](#conda-environment)
 ### Virtual Environment
 1. Git clone this repository
   ```bash
   git clone https://github.com/remydecoupes/GeoNLPlify.git
   ```
 2. Create a virtual env
   ```bash
@@ -77,16 +84,21 @@
   ```bash 
   python -m spacy download en_core_web_trf
   ```
 4. Donwload [world-cities from simple maps](https://simplemaps.com/data/world-cities)
   ```bash
   wget -qO- https://simplemaps.com/static/data/world-cities/basic/simplemaps_worldcities_basicv1.75.zip  | bsdtar -xvf- -C ./geonlplify/simplemaps/
   ```
-### Pip install
-:construction: **Packaging in progress** :construction:
 
 ## Acknowledgement
 :pray: This library use those terrific tools/libraries/data :muscle::
 + [Spacy](https://spacy.io/)
 + [The Komoot geocoder Photon](https://photon.komoot.io/)
 + [OpenStreeMap](https://www.openstreetmap.org/copyright)
 + [Simplemaps data](https://simplemaps.com/data/world-cities)
+
+## Scientific publication
+| Conference   |      paper      |  description |
+|----------|:-------------:|------:|
+| [EGC'2023](https://egc2023.sciencesconf.org/) |  [short paper (in French)](https://editions-rnti.fr/?inprocid=1002848) | [video](https://youtu.be/-QaTBtjWr9g) |
+
+
```

### Comparing `GeoNLPlify-0.1.0/README.md` & `geonlplify-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 <h1 align="center"> GeoNLPlify
 :earth_africa: :book:
 </h1>
 
 [![Documentation Status](https://readthedocs.org/projects/geonlplify/badge/?version=latest)](https://geonlplify.readthedocs.io/en/latest/?badge=latest)
+![GitHub](https://img.shields.io/github/license/remydecoupes/GeoNLPlify)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/remydecoupes/GeoNLPlify)
 
 A NLP library for data augmentation focusing on spatial information contained in text.
 
 <p align="center">
   <img src="./readme_ressources/geonlplify_example_schema.png" />
 </p>
 
@@ -19,15 +21,24 @@
 geonlplify.geonlplify(my_text)
 ```
 ```bash
 'My name is Clara and I live in Bristol'
 ```
 
 ## Installation
-You can install GeoNLPlify in three ways: in a [virtual_env](#virtual-environment), in a [conda environment](#conda-environment), or using :construction: [pip](#pip-install)
+```bash
+pip install GeoNLPlify
+# Download data. Please visit Simplemaps: https://simplemaps.com/data/world-cities
+python3 -c "from geonlplify import download_simplemaps_data; download_simplemaps_data()"
+# Download spacy model
+python -m spacy download en_core_web_trf  
+```
+
+## Contributions
+You can install GeoNLPlify in three ways: in a [virtual_env](#virtual-environment), in a [conda environment](#conda-environment)
 ### Virtual Environment
 1. Git clone this repository
   ```bash
   git clone https://github.com/remydecoupes/GeoNLPlify.git
   ```
 2. Create a virtual env
   ```bash
@@ -60,16 +71,19 @@
   ```bash 
   python -m spacy download en_core_web_trf
   ```
 4. Donwload [world-cities from simple maps](https://simplemaps.com/data/world-cities)
   ```bash
   wget -qO- https://simplemaps.com/static/data/world-cities/basic/simplemaps_worldcities_basicv1.75.zip  | bsdtar -xvf- -C ./geonlplify/simplemaps/
   ```
-### Pip install
-:construction: **Packaging in progress** :construction:
 
 ## Acknowledgement
 :pray: This library use those terrific tools/libraries/data :muscle::
 + [Spacy](https://spacy.io/)
 + [The Komoot geocoder Photon](https://photon.komoot.io/)
 + [OpenStreeMap](https://www.openstreetmap.org/copyright)
-+ [Simplemaps data](https://simplemaps.com/data/world-cities)
++ [Simplemaps data](https://simplemaps.com/data/world-cities)
+
+## Scientific publication
+| Conference   |      paper      |  description |
+|----------|:-------------:|------:|
+| [EGC'2023](https://egc2023.sciencesconf.org/) |  [short paper (in French)](https://editions-rnti.fr/?inprocid=1002848) | [video](https://youtu.be/-QaTBtjWr9g) |
```

### Comparing `GeoNLPlify-0.1.0/geonlplify/geonlplify.py` & `geonlplify-0.2.0/geonlplify/geonlplify.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,26 +77,18 @@
     if list_of_variant:  # list is not empty
         for sne in list_of_variant:
             try:
                 if sne[method] != np.nan and sne["name"] != str(sne[method]):
                     if conserve_n_gram:
                         if sne["name"].count(' ') == str(sne[method]).count(' '):
                             text = text.replace(sne["name"], str(sne[method]))
-                        else:
-                            text = np.nan
                     else:
                         text = text.replace(sne["name"], str(sne[method]))
-                else:
-                    text = np.nan
             except:
-                # print("Couldn't replace text with SNE: " + str(sne) + "and text: " + text)
-                text = np.nan
-                return text
-    else:  # empty list
-        text = np.nan
+                pass
     return text
 
 
 def geocode(sne_name):
     """
     Input a place name and retrieves OSM properties.
     Exemple for sne_name="Montpellier":
@@ -195,15 +187,15 @@
                 except:
                     print("No country for " + sne["name"] + "  | geocode: \n" + str(geocoded))
                     sne["spatial_synonym"] = np.nan
         else:
             print("The method is unknown")
             raise Exception("The method is unknown")
         list_of_variants_sne.append(sne)
-        return list_of_variants_sne
+    return list_of_variants_sne
 
 def download_simplemaps_data():
     import requests, zipfile
     from io import BytesIO
 
     print("GeoNLPlify uses simplemaps data: https://simplemaps.com/data/world-cities.\n Please be respectfull with their license (CC-BY)")
     url = "https://simplemaps.com/static/data/world-cities/basic/simplemaps_worldcities_basicv1.75.zip"
```

### Comparing `GeoNLPlify-0.1.0/pyproject.toml` & `geonlplify-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `GeoNLPlify-0.1.0/setup.py` & `geonlplify-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import setuptools
 
 setuptools.setup(
     name="geonlplify",
-    version="0.1.0",
+    version="0.2.0",
     url="",
     author="Rémy Decoupes",
     author_email="",
     description="GeoNLPlify aims to make variations of an input sentence working on spatial information contained in words",
-    long_description=open('README.md').read(),
+    long_description=open('pypi.md').read(),
+    long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=["pandas", "spacy", "requests"],
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.10',
     ],
```


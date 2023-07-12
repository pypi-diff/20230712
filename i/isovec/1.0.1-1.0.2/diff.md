# Comparing `tmp/isovec-1.0.1.tar.gz` & `tmp/isovec-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isovec-1.0.1.tar", last modified: Tue Jun 20 11:52:44 2023, max compression
+gzip compressed data, was "isovec-1.0.2.tar", last modified: Wed Jul 12 19:39:52 2023, max compression
```

## Comparing `isovec-1.0.1.tar` & `isovec-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 11:52:44.038947 isovec-1.0.1/
--rw-rw-rw-   0        0        0      473 2023-06-20 11:44:39.000000 isovec-1.0.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1088 2023-02-25 13:24:32.000000 isovec-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       20 2023-06-20 11:39:46.000000 isovec-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    11118 2023-06-20 11:52:44.037952 isovec-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9093 2023-06-20 11:51:58.000000 isovec-1.0.1/README.md
--rw-rw-rw-   0        0        0     1024 2023-06-20 11:49:18.000000 isovec-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 11:52:44.039944 isovec-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 11:52:43.887050 isovec-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 11:52:44.012079 isovec-1.0.1/src/isovec/
--rw-rw-rw-   0        0        0     6376 2023-06-14 14:05:46.000000 isovec-1.0.1/src/isovec/Element.py
--rw-rw-rw-   0        0        0     3255 2023-06-11 17:54:14.000000 isovec-1.0.1/src/isovec/Isotope.py
--rw-rw-rw-   0        0        0     3994 2023-06-11 18:01:58.000000 isovec-1.0.1/src/isovec/Mixture.py
--rw-rw-rw-   0        0        0     5100 2023-06-11 18:02:42.000000 isovec-1.0.1/src/isovec/Molecule.py
--rw-rw-rw-   0        0        0      206 2023-06-20 11:28:10.000000 isovec-1.0.1/src/isovec/__init__.py
--rw-rw-rw-   0        0        0     2499 2023-06-20 11:31:29.000000 isovec-1.0.1/src/isovec/conversion.py
--rw-rw-rw-   0        0        0    21330 2023-06-14 14:12:06.000000 isovec-1.0.1/src/isovec/elements.py
--rw-rw-rw-   0        0        0      173 2023-06-14 14:03:24.000000 isovec-1.0.1/src/isovec/exceptions.py
--rw-rw-rw-   0        0        0    21141 2023-05-23 19:45:40.000000 isovec-1.0.1/src/isovec/isotopes.py
--rw-rw-rw-   0        0        0      109 2023-05-23 19:42:08.000000 isovec-1.0.1/src/isovec/printer.py
-drwxrwxrwx   0        0        0        0 2023-06-20 11:52:44.033276 isovec-1.0.1/src/isovec.egg-info/
--rw-rw-rw-   0        0        0    11118 2023-06-20 11:52:43.000000 isovec-1.0.1/src/isovec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      423 2023-06-20 11:52:43.000000 isovec-1.0.1/src/isovec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 11:52:43.000000 isovec-1.0.1/src/isovec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-20 11:52:43.000000 isovec-1.0.1/src/isovec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 19:39:52.336807 isovec-1.0.2/
+-rw-rw-rw-   0        0        0     1685 2023-07-12 19:06:28.000000 isovec-1.0.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1088 2023-07-01 14:21:12.000000 isovec-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       20 2023-07-01 14:21:12.000000 isovec-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    11603 2023-07-12 19:39:52.336311 isovec-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9523 2023-07-12 19:19:09.000000 isovec-1.0.2/README.md
+-rw-rw-rw-   0        0        0     1071 2023-07-12 19:19:51.000000 isovec-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 19:39:52.336807 isovec-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 19:39:52.307543 isovec-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 19:39:52.328872 isovec-1.0.2/src/isovec/
+-rw-rw-rw-   0        0        0      206 2023-07-11 18:22:30.000000 isovec-1.0.2/src/isovec/__init__.py
+-rw-rw-rw-   0        0        0     2467 2023-07-10 20:57:17.000000 isovec-1.0.2/src/isovec/conversion.py
+-rw-rw-rw-   0        0        0     6924 2023-07-11 19:29:01.000000 isovec-1.0.2/src/isovec/element.py
+-rw-rw-rw-   0        0        0    21333 2023-07-10 20:42:42.000000 isovec-1.0.2/src/isovec/elements.py
+-rw-rw-rw-   0        0        0      169 2023-07-10 21:01:47.000000 isovec-1.0.2/src/isovec/exceptions.py
+-rw-rw-rw-   0        0        0     3317 2023-07-10 20:49:15.000000 isovec-1.0.2/src/isovec/isotope.py
+-rw-rw-rw-   0        0        0    21145 2023-07-10 20:10:57.000000 isovec-1.0.2/src/isovec/isotopes.py
+-rw-rw-rw-   0        0        0     4926 2023-07-11 19:53:06.000000 isovec-1.0.2/src/isovec/mixture.py
+-rw-rw-rw-   0        0        0     5510 2023-07-11 19:51:44.000000 isovec-1.0.2/src/isovec/molecule.py
+-rw-rw-rw-   0        0        0      112 2023-07-10 20:58:25.000000 isovec-1.0.2/src/isovec/printer.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:39:52.335319 isovec-1.0.2/src/isovec.egg-info/
+-rw-rw-rw-   0        0        0    11603 2023-07-12 19:39:52.000000 isovec-1.0.2/src/isovec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2023-07-12 19:39:52.000000 isovec-1.0.2/src/isovec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 19:39:52.000000 isovec-1.0.2/src/isovec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 19:39:52.000000 isovec-1.0.2/src/isovec.egg-info/top_level.txt
```

### Comparing `isovec-1.0.1/LICENSE` & `isovec-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `isovec-1.0.1/PKG-INFO` & `isovec-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isovec
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package to calculate isotopic composition of (custom) Elements, Molecules and Mixtures.
 Author-email: Julius Mercz <julius.mercz@tum.de>
 License: MIT License
         
         Copyright (c) 2023 Julius Mercz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,14 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: PyPI, https://pypi.org/project/isovec/
+Project-URL: GitHub, https://github.com/jmercz/isoVec
 Keywords: isotope,element,molecule,mixture,alloy,composition,weight,atomic
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -46,41 +47,42 @@
 This information is given in the form of `Isotope` and `Element` classes.
 The user can create custom elements and specify the isotopic composition manually. `Element`s make up `Molecule`s and `Element`s and `Molecule`s can make up a `Mixture`.
 A thorough example is given in Section Example.
 
 
 ## Installation
 
-The source code and binary installers are currently only available on the project site on the [Python Package Index (PyPI)](https://pypi.org/project/isovec) and can be simply installed from the repository via
+The source code of the most recent development version is hosted on [GitHub](https://github.com/jmercz/isoVec).
+The binary installers and the source code of stable releases is available on the project site on the [Python Package Index (PyPI)](https://pypi.org/project/isovec) and can be simply installed from the repository via
 
 ```sh
 pip install isovec
 ```
 
 There are no additional dependencies other than core Python packages of Python 3.9.
 
 
 ## Example
 
 The composition of the atmosphere of the Earth may serve as an example how to use isoVec.
 The constituents and their atomic (mole) fractions are taken from the respective [Wikipedia](https://en.wikipedia.org/wiki/Atmosphere_of_Earth#Composition) article and are as of April 2022:
 
-| Constituent                     | Atomic Fraction [at.%] |
+| Constituent                     | Atomic Fraction        |
 | ------------------------------- | ---------------------- |
-| Nitrogen (N<sub>2</sub>)        | 78.084                 |
-| Oxygen (O<sub>2</sub>)          | 20.946                 |
-| Argon (Ar)                      | 0.9340                 |
-| Carbon dioxide (CO<sub>2</sub>) | 0.0417                 |
-| Neon (Ne)                       | 0.001818               |
-| Helium (He)                     | 0.000524               |
-| Methane (CH<sub>4</sub>)        | 0.000187               |
-| Krypton (Kr)                    | 0.000114               |
+| Nitrogen (N<sub>2</sub>)        | 78.084 %               |
+| Oxygen (O<sub>2</sub>)          | 20.946 %               |
+| Argon (Ar)                      | 0.9340 %               |
+| Carbon dioxide (CO<sub>2</sub>) | 417 ppm                |
+| Neon (Ne)                       | 18.18 ppm              |
+| Helium (He)                     | 5.24 ppm               |
+| Methane (CH<sub>4</sub>)        | 1.87 ppm               |
+| Krypton (Kr)                    | 1.14 ppm               |
 
 Let's assume for the following that you import isoVec with the following (shorter) alias.
-Keep in mind, that all content is packed inside the isovec namespace.
+Keep in mind, that all content is packed inside the given namespace.
 
 ```python
 import isovec as iso
 ```
 
 ### Element
 
@@ -104,20 +106,20 @@
 Also, the composition doesn't necessarily need to add up to one.
 Instead, each fraction is normalised by the total sum of given fractions.
 
 ### Molecule
 
 Straightforward, the composition for a molecule is the number of atoms per element.
 Therefore, only positive values for the compoosition are reasonable here.
-The atomic weight of a molecule is calculated automatically, but could be overwritten when supplying the kwargs key-value pair `atomicWeight=value` in the constructor.
+The atomic weight of a molecule is calculated automatically, but could be overwritten when supplying the kwargs key-value pair `atomic_wt=value` in the constructor.
 However, this class isn't strictly limited to molecules, but can be used for crystalline or amorphous structures with a stochiometric distribution.
 Using the implemented natural elements, the `Molecule` for carbon dioxide is given by a name identifier and the atomic composition:
 
 ```python
-carbonDioxide = iso.Molecule("carbon dioxide", {
+carbon_dioxide = iso.Molecule("carbon dioxide", {
     iso.C_nat: 1,
     iso.O_nat: 2
 })
 ```
 
 Likewise we generate the other molecules:
 
@@ -129,41 +131,43 @@
 nitrogen2 = iso.Molecule("molecular nitrogen", { iso.N_nat: 2})
 oxygen2 = iso.Molecule("molecular oxygen", { iso.O_nat: 2})
 ```
 
 ### Mixture
 
 The air is now a mixture of several molecules and pure elements, as stated in the table from the introduction.
-This `Mixture` is given by a name identifier and the composition, in this case atomic (which again doesn't necessarily need to add up):
+This `Mixture` is given by a name identifier and the composition, in this case atomic (which again doesn't necessarily need to add up).
+In the following definition, we also utilise helper functions for conversion (an extensive list ca be found in the documentation):
 
 ```python
 air = iso.Mixture("air", {
-    nitrogen2:     78.084000E-02, # Molecule
-    oxygen2:       20.946000E-02, # Molecule
-    iso.Ar_nat:     0.934000E-02, # Element
-    carbonDioxide:  0.041700E-02, # Molecule
-    iso.Ne_nat:     0.001818E-02, # Element
-    iso.He_nat:     0.000524E-02, # Element
-    methane:        0.000187E-02, # Molecule
-    iso.Kr_nat:     0.000114E-02  # Element
+    nitrogen2:                 78.084E-02,  # Molecule
+    oxygen2:        iso.percent(20.946),    # Molecule
+    iso.Ar_nat:     iso.percent( 0.9340),   # Element
+    carbon_dioxide:            417.0E-06,   # Molecule
+    iso.Ne_nat:        iso.ppm( 18.18),     # Element
+    iso.He_nat:        iso.ppm(  5.24),     # Element
+    methane:           iso.ppm(  1.87),     # Molecule
+    iso.Kr_nat:        iso.ppm(  1.14)      # Element
 })
 ```
 
-A printed overview of all subcomponents can be obtained by invoking `PrintOverview` ony any substance we want to inspect:
+A printed overview of all subcomponents can be obtained by invoking `print_overview()` ony any substance we want to inspect:
 
 ```python
-air.PrintOverview(True)
+air.print_overview(True)
 ```
 
 which yields the following (excerpt of the) output:
 
 ```
 ________________________________________________________________
 
-Mixture "air"
+ Mixture "air"
+  100.0000 at.%  |  100.0000 wt.%
 
 ----------------------------------------------------------------
 1. Molecule "molecular nitrogen": 28.0134 g/mol
      78.0775 at.%  |   75.5097 wt.%
 - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 1.1. Element "natural nitrogen": 14.0067 g/mol
        78.0775 at.%  |   75.5097 wt.%
@@ -212,21 +216,21 @@
 If scaled, it will yield the fraction of the subcomponent compared to the top-level component, where the function was invoked on.
 In other words, the fractions are multiplicative *downwards*.
 If not scaled, the fractions will only sum up on their respective layer, for example 4.1 and 4.2 would add up to 100 %.
 
 ### Isotope Composition
 
 As can be seen above, this doesn't sum up the fractions for the single isotopes, something we might be interested in.
-The method `GetIsotopes()` can be called upon every component and yields an ordered dictionary with the isotopes and their respective summed atomic fractions.
+The method `get_isotopes()` can be called upon every component and yields an ordered dictionary with the isotopes and their respective summed atomic fractions.
 For our mixture of air, the following code
 
 ```python
-isotopeVector = air.GetIsotopes()
-for isotope, atFrac in isotopeVector.items():
-    print(f"{isotope.name:>6}: {atFrac:.4E}")
+isotope_vector = air.get_isotopes()
+for isotope, at_frac in isotope_vector.items():
+    print(f"{isotope.name:>6}: {at_frac:.4E}")
 ```
 
 yields the final isotope vector:
 
 ```
    H-1: 1.4957E-06
    H-2: 1.7203E-10
@@ -241,12 +245,12 @@
   O-18: 4.2993E-04
    [...]
 ```
 
 
 ## Changelog
 
-For a history of changes, refer to the file `CHANGELOG.md` in the source distribution available under "Navigation/Download files".
+For a history of changes, refer to the file `CHANGELOG.md` in the source code distributions or directly on the [GitHub repository](https://github.com/jmercz/isoVec/blob/main/README.md).
 
 ## References
 
 1. Coursey, J.S., Schwab, D.J., Tsai, J.J., and Dragoset, R.A. (2015), Atomic Weights and Isotopic Compositions (version 4.1). [Online] Available: http://physics.nist.gov/Comp [Accessed 23 November 2022]. National Institute of Standards and Technology, Gaithersburg, MD.
```

### Comparing `isovec-1.0.1/README.md` & `isovec-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,41 +7,42 @@
 This information is given in the form of `Isotope` and `Element` classes.
 The user can create custom elements and specify the isotopic composition manually. `Element`s make up `Molecule`s and `Element`s and `Molecule`s can make up a `Mixture`.
 A thorough example is given in Section Example.
 
 
 ## Installation
 
-The source code and binary installers are currently only available on the project site on the [Python Package Index (PyPI)](https://pypi.org/project/isovec) and can be simply installed from the repository via
+The source code of the most recent development version is hosted on [GitHub](https://github.com/jmercz/isoVec).
+The binary installers and the source code of stable releases is available on the project site on the [Python Package Index (PyPI)](https://pypi.org/project/isovec) and can be simply installed from the repository via
 
 ```sh
 pip install isovec
 ```
 
 There are no additional dependencies other than core Python packages of Python 3.9.
 
 
 ## Example
 
 The composition of the atmosphere of the Earth may serve as an example how to use isoVec.
 The constituents and their atomic (mole) fractions are taken from the respective [Wikipedia](https://en.wikipedia.org/wiki/Atmosphere_of_Earth#Composition) article and are as of April 2022:
 
-| Constituent                     | Atomic Fraction [at.%] |
+| Constituent                     | Atomic Fraction        |
 | ------------------------------- | ---------------------- |
-| Nitrogen (N<sub>2</sub>)        | 78.084                 |
-| Oxygen (O<sub>2</sub>)          | 20.946                 |
-| Argon (Ar)                      | 0.9340                 |
-| Carbon dioxide (CO<sub>2</sub>) | 0.0417                 |
-| Neon (Ne)                       | 0.001818               |
-| Helium (He)                     | 0.000524               |
-| Methane (CH<sub>4</sub>)        | 0.000187               |
-| Krypton (Kr)                    | 0.000114               |
+| Nitrogen (N<sub>2</sub>)        | 78.084 %               |
+| Oxygen (O<sub>2</sub>)          | 20.946 %               |
+| Argon (Ar)                      | 0.9340 %               |
+| Carbon dioxide (CO<sub>2</sub>) | 417 ppm                |
+| Neon (Ne)                       | 18.18 ppm              |
+| Helium (He)                     | 5.24 ppm               |
+| Methane (CH<sub>4</sub>)        | 1.87 ppm               |
+| Krypton (Kr)                    | 1.14 ppm               |
 
 Let's assume for the following that you import isoVec with the following (shorter) alias.
-Keep in mind, that all content is packed inside the isovec namespace.
+Keep in mind, that all content is packed inside the given namespace.
 
 ```python
 import isovec as iso
 ```
 
 ### Element
 
@@ -65,20 +66,20 @@
 Also, the composition doesn't necessarily need to add up to one.
 Instead, each fraction is normalised by the total sum of given fractions.
 
 ### Molecule
 
 Straightforward, the composition for a molecule is the number of atoms per element.
 Therefore, only positive values for the compoosition are reasonable here.
-The atomic weight of a molecule is calculated automatically, but could be overwritten when supplying the kwargs key-value pair `atomicWeight=value` in the constructor.
+The atomic weight of a molecule is calculated automatically, but could be overwritten when supplying the kwargs key-value pair `atomic_wt=value` in the constructor.
 However, this class isn't strictly limited to molecules, but can be used for crystalline or amorphous structures with a stochiometric distribution.
 Using the implemented natural elements, the `Molecule` for carbon dioxide is given by a name identifier and the atomic composition:
 
 ```python
-carbonDioxide = iso.Molecule("carbon dioxide", {
+carbon_dioxide = iso.Molecule("carbon dioxide", {
     iso.C_nat: 1,
     iso.O_nat: 2
 })
 ```
 
 Likewise we generate the other molecules:
 
@@ -90,41 +91,43 @@
 nitrogen2 = iso.Molecule("molecular nitrogen", { iso.N_nat: 2})
 oxygen2 = iso.Molecule("molecular oxygen", { iso.O_nat: 2})
 ```
 
 ### Mixture
 
 The air is now a mixture of several molecules and pure elements, as stated in the table from the introduction.
-This `Mixture` is given by a name identifier and the composition, in this case atomic (which again doesn't necessarily need to add up):
+This `Mixture` is given by a name identifier and the composition, in this case atomic (which again doesn't necessarily need to add up).
+In the following definition, we also utilise helper functions for conversion (an extensive list ca be found in the documentation):
 
 ```python
 air = iso.Mixture("air", {
-    nitrogen2:     78.084000E-02, # Molecule
-    oxygen2:       20.946000E-02, # Molecule
-    iso.Ar_nat:     0.934000E-02, # Element
-    carbonDioxide:  0.041700E-02, # Molecule
-    iso.Ne_nat:     0.001818E-02, # Element
-    iso.He_nat:     0.000524E-02, # Element
-    methane:        0.000187E-02, # Molecule
-    iso.Kr_nat:     0.000114E-02  # Element
+    nitrogen2:                 78.084E-02,  # Molecule
+    oxygen2:        iso.percent(20.946),    # Molecule
+    iso.Ar_nat:     iso.percent( 0.9340),   # Element
+    carbon_dioxide:            417.0E-06,   # Molecule
+    iso.Ne_nat:        iso.ppm( 18.18),     # Element
+    iso.He_nat:        iso.ppm(  5.24),     # Element
+    methane:           iso.ppm(  1.87),     # Molecule
+    iso.Kr_nat:        iso.ppm(  1.14)      # Element
 })
 ```
 
-A printed overview of all subcomponents can be obtained by invoking `PrintOverview` ony any substance we want to inspect:
+A printed overview of all subcomponents can be obtained by invoking `print_overview()` ony any substance we want to inspect:
 
 ```python
-air.PrintOverview(True)
+air.print_overview(True)
 ```
 
 which yields the following (excerpt of the) output:
 
 ```
 ________________________________________________________________
 
-Mixture "air"
+ Mixture "air"
+  100.0000 at.%  |  100.0000 wt.%
 
 ----------------------------------------------------------------
 1. Molecule "molecular nitrogen": 28.0134 g/mol
      78.0775 at.%  |   75.5097 wt.%
 - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 1.1. Element "natural nitrogen": 14.0067 g/mol
        78.0775 at.%  |   75.5097 wt.%
@@ -173,21 +176,21 @@
 If scaled, it will yield the fraction of the subcomponent compared to the top-level component, where the function was invoked on.
 In other words, the fractions are multiplicative *downwards*.
 If not scaled, the fractions will only sum up on their respective layer, for example 4.1 and 4.2 would add up to 100 %.
 
 ### Isotope Composition
 
 As can be seen above, this doesn't sum up the fractions for the single isotopes, something we might be interested in.
-The method `GetIsotopes()` can be called upon every component and yields an ordered dictionary with the isotopes and their respective summed atomic fractions.
+The method `get_isotopes()` can be called upon every component and yields an ordered dictionary with the isotopes and their respective summed atomic fractions.
 For our mixture of air, the following code
 
 ```python
-isotopeVector = air.GetIsotopes()
-for isotope, atFrac in isotopeVector.items():
-    print(f"{isotope.name:>6}: {atFrac:.4E}")
+isotope_vector = air.get_isotopes()
+for isotope, at_frac in isotope_vector.items():
+    print(f"{isotope.name:>6}: {at_frac:.4E}")
 ```
 
 yields the final isotope vector:
 
 ```
    H-1: 1.4957E-06
    H-2: 1.7203E-10
@@ -202,12 +205,12 @@
   O-18: 4.2993E-04
    [...]
 ```
 
 
 ## Changelog
 
-For a history of changes, refer to the file `CHANGELOG.md` in the source distribution available under "Navigation/Download files".
+For a history of changes, refer to the file `CHANGELOG.md` in the source code distributions or directly on the [GitHub repository](https://github.com/jmercz/isoVec/blob/main/README.md).
 
 ## References
 
 1. Coursey, J.S., Schwab, D.J., Tsai, J.J., and Dragoset, R.A. (2015), Atomic Weights and Isotopic Compositions (version 4.1). [Online] Available: http://physics.nist.gov/Comp [Accessed 23 November 2022]. National Institute of Standards and Technology, Gaithersburg, MD.
```

### Comparing `isovec-1.0.1/pyproject.toml` & `isovec-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 where = ["src"]
 include = ["isovec*"]
 exclude = ["extension*"]
 
 
 [project]
 name = "isovec"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name="Julius Mercz", email="julius.mercz@tum.de" }
 ]
 description = "A package to calculate isotopic composition of (custom) Elements, Molecules and Mixtures."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
@@ -32,8 +32,9 @@
 ]
 dependencies = [
     
 ]
 
 
 [project.urls]
-"PyPI" = "https://pypi.org/project/isovec/"
+"PyPI" = "https://pypi.org/project/isovec/"
+"GitHub" = "https://github.com/jmercz/isoVec"
```

### Comparing `isovec-1.0.1/src/isovec/Element.py` & `isovec-1.0.2/src/isovec/element.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,193 +1,198 @@
 # Python class for element, made of isotopes
 
 from collections import defaultdict
 
 from .exceptions import *
+from .conversion import wt_to_at, at_to_wt, percent
 
-from .Isotope import Isotope
-
-from .conversion import WtToAt, AtToWt
+from .isotope import Isotope
 
 class Element:
 
-    def __init__(self, name: str, isotopes: dict[Isotope, float], **kwargs) -> 'Element':
-        """
-        Element object
+    def __init__(self, name: str, isotopes: dict[Isotope, float], **kwargs) -> None:
+        """Element object
 
         Optional parameters:
-          "atomicWeight": float - overwrite atomic weight of element
+          "atomic_wt": float - overwrite atomic weight of element
         """
         
         self._name: str = name                     # name
-        self._atomicNumber: int                    # atomic number (protons)
+        self._atomic_num: int                        # atomic number (protons)
         self._isotopes: dict[Isotope, float] = {}  # {isotope: atomic fraction}
-        self._atomicWeight: float                  # atomic weight, weighted by (atomic) abundance of isootopes
+        self._atomic_wt: float                       # atomic weight, weighted by (atomic) abundance of isootopes
 
-        if not all(fraction > 0 for fraction in isotopes.values()):
+        if not all(frac > 0 for frac in isotopes.values()):
             # either all negative or mixed
-            if all(fraction < 0 for fraction in isotopes.values()):
+            if all(frac < 0 for frac in isotopes.values()):
                 # given in terms of weight fraction
                 
                 # remove negative sign from input
-                for isotope, wtFraction in isotopes.items():
-                    isotopes[isotope] = abs(wtFraction)
+                for isotope, wt_frac in isotopes.items():
+                    isotopes[isotope] = abs(wt_frac)
 
                 # convert to atomic fraction
-                isotopes = WtToAt(isotopes)
+                isotopes = wt_to_at(isotopes)
 
             else:
                 raise FractionError(f"Element \"{self._name}\": Mixing of atomic and weight fractions is not allowed.")
 
         # set atomic number from first isotope
-        self._atomicNumber = list(isotopes.keys())[0].atomicNumber
+        self._atomic_num = list(isotopes.keys())[0].atomic_num
 
-        fractionSum = sum(isotopes.values())
-        for isotope, fraction in isotopes.items():
+        frac_sum = sum(isotopes.values())
+        for isotope, frac in isotopes.items():
             
             # check if atomic number matches
-            if isotope.atomicNumber != self._atomicNumber:
+            if isotope.atomic_num != self._atomic_num:
                 raise ValueError(f"Atomic number of all isotopes of Element \"{self._name}\" must match!")
 
-            if fraction == 0:
+            if frac == 0:
                 # not present in element
                 pass
             else:
                 # given as atomic fraction or already converted to atomic fraction
-                self._isotopes[isotope] = fraction / fractionSum # normalised
+                self._isotopes[isotope] = frac / frac_sum  # normalised
 
-        if "atomicWeight" in kwargs:
-            self._atomicWeight = kwargs["atomicWeight"]
-        else:
-            self._atomicWeight = self.CalcAtomicWeight()
+        # process kwargs
+        self._atomic_wt = kwargs.get("atomic_wt", self.calc_atomic_wt())  # use given atomic weight or calculate
             
 
         return
                 
     
 
     # ########
     # Getter
     # ########
 
     @property
     def name(self):
-        """ Name of the element """
+        """Name of the element."""
         return self._name
 
     @property
-    def atomicNumber(self):
-        """ Atomic number (number of protons) """
-        return self._atomicNumber
+    def atomic_num(self):
+        """Atomic number (number of protons)."""
+        return self._atomic_num
 
     @property
     def isotopes(self):
-        """ Dictionary of isotopes and their abundance (atomic fractions) """
+        """Dictionary of isotopes and their abundance (atomic fractions)."""
         return self._isotopes
     
     @property
-    def atomicWeight(self):
-        """ Atomic weight of element, weighted by (atomic) abundance of isotopes """
-        return self._atomicWeight
+    def atomic_wt(self):
+        """Atomic weight of element, weighted by (atomic) abundance of isotopes."""
+        return self._atomic_wt
 
 
     # ########
     # Functions
     # ########
 
-    def CalcAtomicWeight(self) -> float:
-        """
-        Calculate atomic weight of element, weighted by (atomic) abundance of isotopes
-        """
+    def calc_atomic_wt(self) -> float:
+        """Calculates atomic weight of element, weighted by (atomic) abundance of isotopes."""
 
-        atomicWeight = sum([atFrac * isotope.atomicWeight for isotope, atFrac in self._isotopes.items()])
+        atomic_wt = sum([at_frac * isotope.atomic_wt for isotope, at_frac in self._isotopes.items()])
 
-        return atomicWeight
+        return atomic_wt
 
-    def AppendIsotopes(self, dictList: defaultdict[Isotope, list[float]] = defaultdict(list), topFraction: float = 1.0) -> list[dict[Isotope, float]]:
-        """
-        Takes input dictionary and appends all isotopes with their atomic fraction
-        """
+    def _append_isotopes(self, dict_list: defaultdict[Isotope, list[float]] = None, par_at_frac: float = 1.0) -> defaultdict[Isotope, list[float]]:
+        """Appends all isotopes with their atomic fraction to given dictionary."""
 
-        for isotope, fraction in self._isotopes.items():
-            dictList[isotope].append(topFraction*fraction)
+        if dict_list is None:
+            dict_list = defaultdict(list)  # new defaultdict should be the default value for dict_list, but those are mutable and stay the same object over multiple function calls (clutter up)
+                                           # thanks to Don Cross' article: https://towardsdatascience.com/python-pitfall-mutable-default-arguments-9385e8265422
 
-        return dictList
+        for isotope, at_frac in self._isotopes.items():
+            dict_list[isotope].append(par_at_frac*at_frac)
 
-    def GetIsotopes(self) -> dict[Isotope, float]:
-        """ Gets all isotopes with their atomic fraction from the constituents """
-        return {isotope: sum(atFractions) for isotope, atFractions in sorted(self.AppendIsotopes().items())}
+        return dict_list
+
+    def get_isotopes(self) -> dict[Isotope, float]:
+        """Returns dict of all contained isotopes with their summed atomic fraction."""
+        return {isotope: sum(at_fracs) for isotope, at_fracs in sorted(self._append_isotopes().items())}
+
+    def hash(self) -> int:
+        """Hashes element via name."""
+        return hash(self._name)
 
 
     # ########
     # Print
     # ########
 
-    def String(self) -> str:
-        """ Return Element as string """
+    def string(self) -> str:
+        """Returns element name."""
         return self._name
 
-    def PrintOverview(self, scale: bool = False, numberStr: str = "", atFrac: float = 1.0, wtFrac: float = 1.0) -> None:
-        """
-        Prints an overview of the element.
+    def print_overview(self, scale: bool = False, numbering_str: str = "", par_at_frac: float = 1.0, par_wt_frac: float = 1.0) -> None:
+        """Prints an overview of the element.
+
           scale = True - adapts the fractions of sub-components according to the fraction of the parent-component
         """
 
-        print("{0} Element \"{1}\": {2:.4f} g/mol".format(numberStr, self._name, self._atomicWeight))
-        print("{0}  {1:8.4f} at.%  |  {2:8.4f} wt.%".format(" "*len(numberStr), atFrac*1e2, wtFrac*1e2))
+        print("{0} Element \"{1}\": {2:.4f} g/mol".format(numbering_str, self._name, self._atomic_wt))
+        print("{0}  {1:8.4f} at.%  |  {2:8.4f} wt.%".format(" "*len(numbering_str), par_at_frac*1e2, par_wt_frac*1e2))
         print()
 
-        dictWtFrac = AtToWt(self._isotopes)
+        # calculate weight fractions of isotopes
+        wt_fracs = at_to_wt(self._isotopes)
 
-        for i, (isotope, atFraction) in enumerate(self._isotopes.items(), start = 1):
-            iStr = numberStr + str(i) + "."
-            wtFraction = dictWtFrac[isotope]
+        for i, (isotope, iso_at_frac) in enumerate(self._isotopes.items(), start = 1):
+            cur_num_str = numbering_str + str(i) + "."  # list indention string
+            iso_wt_frac = wt_fracs[isotope]
 
             if scale:
-                atFraction = atFrac * atFraction
-                wtFraction = wtFrac * wtFraction
+                # scale with parent fraction
+                iso_at_frac = par_at_frac * iso_at_frac
+                iso_wt_frac = par_wt_frac * iso_wt_frac
             
-            print("{0:<9} {1:<7} {2:8.4f} at.%  |  {3:8.4f} wt.%".format(iStr, isotope._name + ":", atFraction*1e2, wtFraction*1e2))
+            print("{0:<9} {1:<7} {2:8.4f} at.%  |  {3:8.4f} wt.%".format(cur_num_str, isotope._name + ":", iso_at_frac*1e2, iso_wt_frac*1e2))
 
         return
 
 
 
     # ########
     # Operators
     # ########
 
     def __str__(self):
-        return self.String()
+        return self.string()
 
     def __repr__(self):
-        return self.String()
+        return self.string()
 
     def __hash__(self):
-        return hash(self._name)
+        return self.hash()
 
-    def __eq__(self, other: 'Element'):
+    def __eq__(self, other):
         try:
             return self._name == other._name
         except:
-            raise TypeError(f"Cannot compare Element with type \"{type(other)}\".")
+            #raise TypeError(f"Cannot compare Element with type \"{type(other)}\".")
+            return NotImplemented
 
-    def __ne__(self, other: 'Element'):
+    def __ne__(self, other):
         return not self.__eq__(other)
 
-    def __lt__(self, other: 'Element'):
+    def __lt__(self, other):
         try:
-            return self._atomicNumber < other._atomicNumber
+            return self._atomic_num < other._atomic_num
         except:
-            raise TypeError(f"Cannot compare Element with type \"{type(other)}\".")
+            #raise TypeError(f"Cannot compare Element with type \"{type(other)}\".")
+            return NotImplemented
 
-    def __le__(self, other: 'Element'):
+    def __le__(self, other):
         return self.__lt__(other) or self.__eq__(other)
 
-    def __gt__(self, other: 'Element'):
+    def __gt__(self, other):
         try:
-            return self._atomicNumber > other._atomicNumber
+            return self._atomic_num > other._atomic_num
         except:
-            raise TypeError(f"Cannot compare Element with type \"{type(other)}\".")
+            #raise TypeError(f"Cannot compare Element with type \"{type(other)}\".")
+            return NotImplemented
 
-    def __ge__(self, other: 'Element'):
+    def __ge__(self, other):
         return self.__gt__(other) or self.__eq__(other)
```

### Comparing `isovec-1.0.1/src/isovec/Isotope.py` & `isovec-1.0.2/src/isovec/isotope.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,114 +1,121 @@
 # Python class for isotope
 
 class Isotope:
 
-    def __init__(self, name: str, atomicNumber: int, massNumber: int, atomicWeight: float) -> 'Isotope':
+    def __init__(self, name: str, atomic_num: int, mass_num: int, atomic_wt: float) -> None:
         
-        self._name: str = name                    # name
-        self._atomicNumber: int = atomicNumber    # atomic number (protons)
-        self._massNumber: int = massNumber        # (atomic) mass number (protons + neutrons)
-        self._atomicWeight: float = atomicWeight  # atomic weight
+        self._name: str = name          # name
+        self._atomic_num: int = atomic_num  # atomic number (protons)
+        self._mass_num: int = mass_num  # (atomic) mass number (protons + neutrons)
+        self._atomic_wt: float = atomic_wt  # atomic weight
 
     # ########
     # Getter
     # ########
 
     @property
     def name(self):
-        """ Name of the isotope """
+        """Name of the isotope."""
         return self._name
 
     @property
-    def atomicNumber(self):
-        """ Atomic number (number of protons) """
-        return self._atomicNumber
+    def atomic_num(self):
+        """Atomic number (number of protons)."""
+        return self._atomic_num
 
     @property
-    def massNumber(self):
-        """ (Atomic) Mass number (number of protons + neutrons) """
-        return self._massNumber
+    def mass_num(self):
+        """(Atomic) Mass number (number of protons + neutrons)."""
+        return self._mass_num
 
     @property
-    def atomicWeight(self):
-        """ Atomic weight of the isotope """
-        return self._atomicWeight
+    def atomic_wt(self):
+        """Atomic weight of the isotope."""
+        return self._atomic_wt
 
 
     # ########
     # Functions
     # ########
 
-    def NeutronNumber(self) -> int:
-        """ Neutron number (number of neutrons) """
-        return self._massNumber - self._atomicNumber
+    def neutron_number(self) -> int:
+        """Calculates neutron number (number of neutrons)."""
+        return self._mass_num - self._atomic_num
+
+    def hash(self) -> int:
+        """Hashes isotope via atomic and mass number."""
+        return hash((self._atomic_num, self._mass_num))
 
 
     # ########
     # Print
     # ########
 
-    def String(self) -> str:
-        """ Return Isotope as string """
+    def string(self) -> str:
+        """Returns isotope name."""
         return self._name
 
 
     # ########
     # Operators
     # ########
 
     def __str__(self):
-        return self.String()
+        return self.string()
 
     def __repr__(self):
-        return self.String()
+        return self.string()
 
     def __hash__(self):
-        return hash((self._atomicNumber, self._massNumber))
+        return self.hash()
 
-    def __eq__(self, other: 'Isotope'):
+    def __eq__(self, other):
         try:
-            if (self._atomicNumber == other._atomicNumber) and (self._massNumber == other._massNumber):
+            if (self._atomic_num == other._atomic_num) and (self._mass_num == other._mass_num):
                 return True
             else:
                 return False
         except:
-            raise TypeError(f"Cannot compare Isotope with type \"{type(other)}\".")
+            #raise TypeError(f"Cannot compare Isotope with type \"{type(other)}\".")
+            return NotImplemented
 
-    def __ne__(self, other: 'Isotope'):
+    def __ne__(self, other):
         return not self.__eq__(other)
 
-    def __lt__(self, other: 'Isotope'):
+    def __lt__(self, other):
         try:
-            if self._atomicNumber < other._atomicNumber:
+            if self._atomic_num < other._atomic_num:
                 return True
-            elif self._atomicNumber == other._atomicNumber:
-                if self._massNumber < other._massNumber:
+            elif self._atomic_num == other._atomic_num:
+                if self._mass_num < other._mass_num:
                     return True
                 else:
                     return False
             else:
                 return False
         except:
-            raise TypeError(f"Cannot compare Isotope with type \"{type(other)}\".")
+            #raise TypeError(f"Cannot compare Isotope with type \"{type(other)}\".")
+            return NotImplemented
 
-    def __le__(self, other: 'Isotope'):
+    def __le__(self, other):
         return self.__lt__(other) or self.__eq__(other)
 
 
-    def __gt__(self, other: 'Isotope'):
+    def __gt__(self, other):
         try:
-            if self._atomicNumber > other._atomicNumber:
+            if self._atomic_num > other._atomic_num:
                 return True
-            elif self._atomicNumber == other._atomicNumber:
-                if self._massNumber > other._massNumber:
+            elif self._atomic_num == other._atomic_num:
+                if self._mass_num > other._mass_num:
                     return True
                 else:
                     return False
             else:
                 return False
         except:
-            raise TypeError(f"Cannot compare Isotope with type \"{type(other)}\".")
+            #raise TypeError(f"Cannot compare Isotope with type \"{type(other)}\".")
+            return NotImplemented
 
-    def __ge__(self, other: 'Isotope'):
+    def __ge__(self, other):
         return self.__gt__(other) or self.__eq__(other)
```

### Comparing `isovec-1.0.1/src/isovec/conversion.py` & `isovec-1.0.2/src/isovec/conversion.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 
-def WtToAt(constituents: dict[any, float]) -> dict[any, float]:
-    """
-    Converts weight fraction from dictionary to atomic fraction
-    """
+from typing import Any
+
+def wt_to_at(constituents: dict[Any, float]) -> dict[Any, float]:
+    """Converts weight fractions from dictionary to atomic fractions."""
 
     try:
         # calculate (constant) denominator for conversion
-        denominator = sum([wtFraction / constituent.atomicWeight for constituent, wtFraction in constituents.items()])
+        denominator = sum([wt_frac / constituent.atomic_wt for constituent, wt_frac in constituents.items()])
 
         # convert and overwrite to atomic fraction
-        conv_constituents: dict[any, float] = {}
-        for constituent, wtFraction in constituents.items():
-            conv_constituents[constituent] = (wtFraction/constituent.atomicWeight) / denominator # now atomic fraction
+        conv_constituents: dict[Any, float] = {}
+        for constituent, wt_frac in constituents.items():
+            conv_constituents[constituent] = (wt_frac/constituent.atomic_wt) / denominator # now atomic fraction
 
         return conv_constituents
 
     except:
         raise TypeError(f"One of the constituents does not have an atomic weight.")
 
-def AtToWt(constituents: dict[any, float]) -> dict[any, float]:
-    """
-    Converts atomic fraction from dictionary to weight fraction 
-    """
+def at_to_wt(constituents: dict[Any, float]) -> dict[Any, float]:
+    """Converts atomic fractions from dictionary to weight fractions."""
 
     try:
         # calculate (constant) denominator for conversion
-        denominator = sum([atFraction * constituent.atomicWeight for constituent, atFraction in constituents.items()])
+        denominator = sum([at_frac * constituent.atomic_wt for constituent, at_frac in constituents.items()])
 
         # convert and overwrite to weight fraction
-        conv_constituents: dict[any, float] = {}
-        for constituent, atFraction in constituents.items():
-            conv_constituents[constituent] = (atFraction * constituent.atomicWeight) / denominator # now weight fraction
+        conv_constituents: dict[Any, float] = {}
+        for constituent, at_frac in constituents.items():
+            conv_constituents[constituent] = (at_frac * constituent.atomic_wt) / denominator # now weight fraction
 
         return conv_constituents
 
     except:
         raise TypeError(f"One of the constituents does not have an atomic weight.")
 
+
 def percent(value: float):
-    """ Converts value from percent """
+    """Converts value from percent."""
     return value*1e-2
 perc = percent # function alias
 pc   = percent # function alias
 
 def permille(value: float):
-    """ Converts value from per mille """
+    """Converts value from per mille."""
     return value*1e-3
 pm = permille # function alias
 
 def permyriad(value: float):
-    """ Converts value from per myriad """
+    """Converts value from per myriad."""
     return value*1e-4
 bp = permyriad # function alias
 
 def percentmille(value: float):
-    """ Converts value from per cent mille """
+    """Converts value from per cent mille."""
     return value*1e-5
 pcm = percentmille # function alias
 
 def ppm(value: float):
-    """ Converts value from parts per million """
+    """Converts value from parts per million."""
     return value*1e-6
 
 def ppb(value: float):
-    """ Converts value from parts per billion  """
+    """Converts value from parts per billion."""
     return value*1e-9
 
 def ppt(value: float):
-    """ Converts value from parts per trillion """
+    """Converts value from parts per trillion."""
     return value*1e-12
 
 def ppq(value: float):
-    """ Converts value from parts per quadrillion """
+    """Converts value from parts per quadrillion."""
     return value*1e-15
```

### Comparing `isovec-1.0.1/src/isovec/elements.py` & `isovec-1.0.2/src/isovec/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # module for element symbols and names and natural elements
 
 from .exceptions import *
-
-from .Element import Element
-
+from .element import Element
 from .isotopes import *
 
 
-numberToSymbol = {
+atom_numb_to_symbol = {
     1:   "H",
     2:   "He",
     3:   "Li",
     4:   "Be",
     5:   "B",
     6:   "C",
     7:   "N",
@@ -124,15 +122,15 @@
     114: "Fl",
     115: "Mc",
     116: "Lv",
     117: "Ts",
     118: "Og"
 }
 
-symbolToName = {
+symbol_to_name = {
     "H":  "hydrogen",
     "He": "helium",
     "Li": "lithium",
     "Be": "berylium",
     "B":  "boron",
     "C":  "carbon",
     "N":  "nitrogen",
```

### Comparing `isovec-1.0.1/src/isovec/isotopes.py` & `isovec-1.0.2/src/isovec/isotopes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # module with all isotopes
 
-from .Isotope import Isotope
+from .isotope import Isotope
 
 
 #   1: H  (hydrogen)
 H_1    = Isotope("H-1"   ,   1,   1, 1.00782503223)
-H      = Isotope("H"     ,   1,   1, 1.00782503223) # alias
+H      = Isotope("H"     ,   1,   1, 1.00782503223)  # alias
 H_2    = Isotope("H-2"   ,   1,   2, 2.01410177812)
-D      = Isotope("D"     ,   1,   2, 2.01410177812) # alias
+D      = Isotope("D"     ,   1,   2, 2.01410177812)  # alias
 H_3    = Isotope("H-3"   ,   1,   3, 3.0160492779)
-T      = Isotope("T"     ,   1,   3, 3.0160492779) # alias
+T      = Isotope("T"     ,   1,   3, 3.0160492779)   # alias
 
 #   2: He (helium)
 He_3   = Isotope("He-3"  ,   2,   3, 3.0160293201)
 He_4   = Isotope("He-4"  ,   2,   4, 4.00260325413)
 
 #   3: Li (lithium)
 Li_6   = Isotope("Li-6"  ,   3,   6, 6.0151228874)
```

### Comparing `isovec-1.0.1/src/isovec.egg-info/PKG-INFO` & `isovec-1.0.2/src/isovec.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isovec
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package to calculate isotopic composition of (custom) Elements, Molecules and Mixtures.
 Author-email: Julius Mercz <julius.mercz@tum.de>
 License: MIT License
         
         Copyright (c) 2023 Julius Mercz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,14 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: PyPI, https://pypi.org/project/isovec/
+Project-URL: GitHub, https://github.com/jmercz/isoVec
 Keywords: isotope,element,molecule,mixture,alloy,composition,weight,atomic
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -46,41 +47,42 @@
 This information is given in the form of `Isotope` and `Element` classes.
 The user can create custom elements and specify the isotopic composition manually. `Element`s make up `Molecule`s and `Element`s and `Molecule`s can make up a `Mixture`.
 A thorough example is given in Section Example.
 
 
 ## Installation
 
-The source code and binary installers are currently only available on the project site on the [Python Package Index (PyPI)](https://pypi.org/project/isovec) and can be simply installed from the repository via
+The source code of the most recent development version is hosted on [GitHub](https://github.com/jmercz/isoVec).
+The binary installers and the source code of stable releases is available on the project site on the [Python Package Index (PyPI)](https://pypi.org/project/isovec) and can be simply installed from the repository via
 
 ```sh
 pip install isovec
 ```
 
 There are no additional dependencies other than core Python packages of Python 3.9.
 
 
 ## Example
 
 The composition of the atmosphere of the Earth may serve as an example how to use isoVec.
 The constituents and their atomic (mole) fractions are taken from the respective [Wikipedia](https://en.wikipedia.org/wiki/Atmosphere_of_Earth#Composition) article and are as of April 2022:
 
-| Constituent                     | Atomic Fraction [at.%] |
+| Constituent                     | Atomic Fraction        |
 | ------------------------------- | ---------------------- |
-| Nitrogen (N<sub>2</sub>)        | 78.084                 |
-| Oxygen (O<sub>2</sub>)          | 20.946                 |
-| Argon (Ar)                      | 0.9340                 |
-| Carbon dioxide (CO<sub>2</sub>) | 0.0417                 |
-| Neon (Ne)                       | 0.001818               |
-| Helium (He)                     | 0.000524               |
-| Methane (CH<sub>4</sub>)        | 0.000187               |
-| Krypton (Kr)                    | 0.000114               |
+| Nitrogen (N<sub>2</sub>)        | 78.084 %               |
+| Oxygen (O<sub>2</sub>)          | 20.946 %               |
+| Argon (Ar)                      | 0.9340 %               |
+| Carbon dioxide (CO<sub>2</sub>) | 417 ppm                |
+| Neon (Ne)                       | 18.18 ppm              |
+| Helium (He)                     | 5.24 ppm               |
+| Methane (CH<sub>4</sub>)        | 1.87 ppm               |
+| Krypton (Kr)                    | 1.14 ppm               |
 
 Let's assume for the following that you import isoVec with the following (shorter) alias.
-Keep in mind, that all content is packed inside the isovec namespace.
+Keep in mind, that all content is packed inside the given namespace.
 
 ```python
 import isovec as iso
 ```
 
 ### Element
 
@@ -104,20 +106,20 @@
 Also, the composition doesn't necessarily need to add up to one.
 Instead, each fraction is normalised by the total sum of given fractions.
 
 ### Molecule
 
 Straightforward, the composition for a molecule is the number of atoms per element.
 Therefore, only positive values for the compoosition are reasonable here.
-The atomic weight of a molecule is calculated automatically, but could be overwritten when supplying the kwargs key-value pair `atomicWeight=value` in the constructor.
+The atomic weight of a molecule is calculated automatically, but could be overwritten when supplying the kwargs key-value pair `atomic_wt=value` in the constructor.
 However, this class isn't strictly limited to molecules, but can be used for crystalline or amorphous structures with a stochiometric distribution.
 Using the implemented natural elements, the `Molecule` for carbon dioxide is given by a name identifier and the atomic composition:
 
 ```python
-carbonDioxide = iso.Molecule("carbon dioxide", {
+carbon_dioxide = iso.Molecule("carbon dioxide", {
     iso.C_nat: 1,
     iso.O_nat: 2
 })
 ```
 
 Likewise we generate the other molecules:
 
@@ -129,41 +131,43 @@
 nitrogen2 = iso.Molecule("molecular nitrogen", { iso.N_nat: 2})
 oxygen2 = iso.Molecule("molecular oxygen", { iso.O_nat: 2})
 ```
 
 ### Mixture
 
 The air is now a mixture of several molecules and pure elements, as stated in the table from the introduction.
-This `Mixture` is given by a name identifier and the composition, in this case atomic (which again doesn't necessarily need to add up):
+This `Mixture` is given by a name identifier and the composition, in this case atomic (which again doesn't necessarily need to add up).
+In the following definition, we also utilise helper functions for conversion (an extensive list ca be found in the documentation):
 
 ```python
 air = iso.Mixture("air", {
-    nitrogen2:     78.084000E-02, # Molecule
-    oxygen2:       20.946000E-02, # Molecule
-    iso.Ar_nat:     0.934000E-02, # Element
-    carbonDioxide:  0.041700E-02, # Molecule
-    iso.Ne_nat:     0.001818E-02, # Element
-    iso.He_nat:     0.000524E-02, # Element
-    methane:        0.000187E-02, # Molecule
-    iso.Kr_nat:     0.000114E-02  # Element
+    nitrogen2:                 78.084E-02,  # Molecule
+    oxygen2:        iso.percent(20.946),    # Molecule
+    iso.Ar_nat:     iso.percent( 0.9340),   # Element
+    carbon_dioxide:            417.0E-06,   # Molecule
+    iso.Ne_nat:        iso.ppm( 18.18),     # Element
+    iso.He_nat:        iso.ppm(  5.24),     # Element
+    methane:           iso.ppm(  1.87),     # Molecule
+    iso.Kr_nat:        iso.ppm(  1.14)      # Element
 })
 ```
 
-A printed overview of all subcomponents can be obtained by invoking `PrintOverview` ony any substance we want to inspect:
+A printed overview of all subcomponents can be obtained by invoking `print_overview()` ony any substance we want to inspect:
 
 ```python
-air.PrintOverview(True)
+air.print_overview(True)
 ```
 
 which yields the following (excerpt of the) output:
 
 ```
 ________________________________________________________________
 
-Mixture "air"
+ Mixture "air"
+  100.0000 at.%  |  100.0000 wt.%
 
 ----------------------------------------------------------------
 1. Molecule "molecular nitrogen": 28.0134 g/mol
      78.0775 at.%  |   75.5097 wt.%
 - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 1.1. Element "natural nitrogen": 14.0067 g/mol
        78.0775 at.%  |   75.5097 wt.%
@@ -212,21 +216,21 @@
 If scaled, it will yield the fraction of the subcomponent compared to the top-level component, where the function was invoked on.
 In other words, the fractions are multiplicative *downwards*.
 If not scaled, the fractions will only sum up on their respective layer, for example 4.1 and 4.2 would add up to 100 %.
 
 ### Isotope Composition
 
 As can be seen above, this doesn't sum up the fractions for the single isotopes, something we might be interested in.
-The method `GetIsotopes()` can be called upon every component and yields an ordered dictionary with the isotopes and their respective summed atomic fractions.
+The method `get_isotopes()` can be called upon every component and yields an ordered dictionary with the isotopes and their respective summed atomic fractions.
 For our mixture of air, the following code
 
 ```python
-isotopeVector = air.GetIsotopes()
-for isotope, atFrac in isotopeVector.items():
-    print(f"{isotope.name:>6}: {atFrac:.4E}")
+isotope_vector = air.get_isotopes()
+for isotope, at_frac in isotope_vector.items():
+    print(f"{isotope.name:>6}: {at_frac:.4E}")
 ```
 
 yields the final isotope vector:
 
 ```
    H-1: 1.4957E-06
    H-2: 1.7203E-10
@@ -241,12 +245,12 @@
   O-18: 4.2993E-04
    [...]
 ```
 
 
 ## Changelog
 
-For a history of changes, refer to the file `CHANGELOG.md` in the source distribution available under "Navigation/Download files".
+For a history of changes, refer to the file `CHANGELOG.md` in the source code distributions or directly on the [GitHub repository](https://github.com/jmercz/isoVec/blob/main/README.md).
 
 ## References
 
 1. Coursey, J.S., Schwab, D.J., Tsai, J.J., and Dragoset, R.A. (2015), Atomic Weights and Isotopic Compositions (version 4.1). [Online] Available: http://physics.nist.gov/Comp [Accessed 23 November 2022]. National Institute of Standards and Technology, Gaithersburg, MD.
```


# Comparing `tmp/assesspy-1.0.1.tar.gz` & `tmp/assesspy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\assesspy-1.0.1.tar", last modified: Wed Sep 14 15:11:17 2022, max compression
+gzip compressed data, was "assesspy-1.0.2.tar", last modified: Wed Jul 12 18:59:54 2023, max compression
```

## Comparing `assesspy-1.0.1.tar` & `assesspy-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-09-14 15:11:17.859572 assesspy-1.0.1/
--rw-rw-rw-   0        0        0    35823 2022-09-08 19:28:37.000000 assesspy-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       17 2022-07-21 17:03:04.000000 assesspy-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1698 2022-09-14 15:11:17.859572 assesspy-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1484 2022-09-13 17:35:55.000000 assesspy-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-09-14 15:11:17.824723 assesspy-1.0.1/assesspy/
--rw-rw-rw-   0        0        0      478 2022-07-20 20:56:51.000000 assesspy-1.0.1/assesspy/__init__.py
--rw-rw-rw-   0        0        0     3398 2022-09-12 21:53:11.000000 assesspy-1.0.1/assesspy/ci.py
-drwxrwxrwx   0        0        0        0 2022-09-14 15:11:17.844872 assesspy-1.0.1/assesspy/data/
--rw-rw-rw-   0        0        0        0 2022-07-19 19:20:12.000000 assesspy-1.0.1/assesspy/data/__init__.py
--rw-rw-rw-   0        0        0    31633 2022-07-11 15:51:35.000000 assesspy-1.0.1/assesspy/data/ratios_sample.parquet
--rw-rw-rw-   0        0        0     6010 2022-09-12 22:45:27.000000 assesspy-1.0.1/assesspy/formulas.py
--rw-rw-rw-   0        0        0     1140 2022-08-25 19:42:17.000000 assesspy-1.0.1/assesspy/load_data.py
--rw-rw-rw-   0        0        0     3327 2022-09-12 21:53:27.000000 assesspy-1.0.1/assesspy/outliers.py
--rw-rw-rw-   0        0        0     5235 2022-09-07 18:18:20.000000 assesspy-1.0.1/assesspy/sales_chasing.py
-drwxrwxrwx   0        0        0        0 2022-09-14 15:11:17.859572 assesspy-1.0.1/assesspy/tests/
--rw-rw-rw-   0        0        0        0 2022-07-14 19:16:06.000000 assesspy-1.0.1/assesspy/tests/__init__.py
--rw-rw-rw-   0        0        0     3967 2022-08-17 16:18:23.000000 assesspy-1.0.1/assesspy/tests/test_ci.py
--rw-rw-rw-   0        0        0     4281 2022-09-12 22:55:07.000000 assesspy-1.0.1/assesspy/tests/test_formulas.py
--rw-rw-rw-   0        0        0     2333 2022-07-21 20:23:53.000000 assesspy-1.0.1/assesspy/tests/test_outliers.py
--rw-rw-rw-   0        0        0     2034 2022-07-21 21:08:12.000000 assesspy-1.0.1/assesspy/tests/test_sales_chasing.py
--rw-rw-rw-   0        0        0     1121 2022-07-21 18:58:09.000000 assesspy-1.0.1/assesspy/utils.py
-drwxrwxrwx   0        0        0        0 2022-09-14 15:11:17.839817 assesspy-1.0.1/assesspy.egg-info/
--rw-rw-rw-   0        0        0     1698 2022-09-14 15:11:17.000000 assesspy-1.0.1/assesspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2022-09-14 15:11:17.000000 assesspy-1.0.1/assesspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-14 15:11:17.000000 assesspy-1.0.1/assesspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2022-09-14 15:11:17.000000 assesspy-1.0.1/assesspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-09-14 15:11:17.000000 assesspy-1.0.1/assesspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      148 2022-09-14 15:11:17.859572 assesspy-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1172 2022-09-14 15:10:36.000000 assesspy-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:59:54.016886 assesspy-1.0.2/
+-rw-rw-rw-   0        0        0    35131 2023-07-12 15:52:53.000000 assesspy-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       19 2023-07-12 15:52:53.000000 assesspy-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2397 2023-07-12 18:59:54.016886 assesspy-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2048 2023-07-12 15:52:53.000000 assesspy-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 18:59:53.950924 assesspy-1.0.2/assesspy/
+-rw-rw-rw-   0        0        0      284 2023-07-12 15:52:53.000000 assesspy-1.0.2/assesspy/__init__.py
+-rw-rw-rw-   0        0        0     3396 2023-07-12 15:52:53.000000 assesspy-1.0.2/assesspy/ci.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:59:53.982883 assesspy-1.0.2/assesspy/data/
+-rw-rw-rw-   0        0        0        0 2023-07-12 15:52:53.000000 assesspy-1.0.2/assesspy/data/__init__.py
+-rw-rw-rw-   0        0        0    31633 2023-07-12 15:52:53.000000 assesspy-1.0.2/assesspy/data/ratios_sample.parquet
+-rw-rw-rw-   0        0        0     6050 2023-07-12 15:52:53.000000 assesspy-1.0.2/assesspy/formulas.py
+-rw-rw-rw-   0        0        0     1109 2023-07-12 15:52:53.000000 assesspy-1.0.2/assesspy/load_data.py
+-rw-rw-rw-   0        0        0     3212 2023-07-12 15:52:53.000000 assesspy-1.0.2/assesspy/outliers.py
+-rw-rw-rw-   0        0        0     5176 2023-07-12 15:52:53.000000 assesspy-1.0.2/assesspy/sales_chasing.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:59:54.008930 assesspy-1.0.2/assesspy/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-12 15:52:53.000000 assesspy-1.0.2/assesspy/tests/__init__.py
+-rw-rw-rw-   0        0        0     3739 2023-07-12 15:52:53.000000 assesspy-1.0.2/assesspy/tests/test_ci.py
+-rw-rw-rw-   0        0        0     4255 2023-07-12 15:52:53.000000 assesspy-1.0.2/assesspy/tests/test_formulas.py
+-rw-rw-rw-   0        0        0     2225 2023-07-12 15:52:53.000000 assesspy-1.0.2/assesspy/tests/test_outliers.py
+-rw-rw-rw-   0        0        0     1956 2023-07-12 15:52:53.000000 assesspy-1.0.2/assesspy/tests/test_sales_chasing.py
+-rw-rw-rw-   0        0        0     1115 2023-07-12 15:52:53.000000 assesspy-1.0.2/assesspy/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:59:53.970899 assesspy-1.0.2/assesspy.egg-info/
+-rw-rw-rw-   0        0        0     2397 2023-07-12 18:59:53.000000 assesspy-1.0.2/assesspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2023-07-12 18:59:53.000000 assesspy-1.0.2/assesspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 18:59:53.000000 assesspy-1.0.2/assesspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-12 18:59:53.000000 assesspy-1.0.2/assesspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 18:59:53.000000 assesspy-1.0.2/assesspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      302 2023-07-12 18:59:54.016886 assesspy-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1110 2023-07-12 18:48:13.000000 assesspy-1.0.2/setup.py
```

### Comparing `assesspy-1.0.1/LICENSE` & `assesspy-1.0.2/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,70 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
 
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
 
   The licenses for most software and other practical works are designed
 to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
+our General Public Licenses are intended to guarantee your freedom to
 share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
+software for all its users.
 
   When we speak of free software, we are referring to freedom, not
 price.  Our General Public Licenses are designed to make sure that you
 have the freedom to distribute copies of free software (and charge for
 them if you wish), that you receive source code or can get it if you
 want it, that you can change the software or use pieces of it in new
 free programs, and that you know you can do these things.
 
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
 
   The precise terms and conditions for copying, distribution and
 modification follow.
 
                        TERMS AND CONDITIONS
 
   0. Definitions.
 
-  "This License" refers to version 3 of the GNU General Public License.
+  "This License" refers to version 3 of the GNU Affero General Public License.
 
   "Copyright" also means copyright-like laws that apply to other kinds of
 works, such as semiconductor masks.
 
   "The Program" refers to any copyrightable work licensed under this
 License.  Each licensee is addressed as "you".  "Licensees" and
 "recipients" may be individuals or organizations.
@@ -545,43 +533,53 @@
 covered work so as to satisfy simultaneously your obligations under this
 License and any other pertinent obligations, then as a consequence you may
 not convey it at all.  For example, if you agree to terms that obligate you
 to collect a royalty for further conveying from those to whom you convey
 the Program, the only way you could satisfy both those terms and this
 License would be to refrain entirely from conveying the Program.
 
-  13. Use with the GNU Affero General Public License.
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
 
   Notwithstanding any other provision of this License, you have
 permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
+under version 3 of the GNU General Public License into a single
 combined work, and to convey the resulting work.  The terms of this
 License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
 
   14. Revised Versions of this License.
 
   The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
 address new problems or concerns.
 
   Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
+Program specifies that a certain numbered version of the GNU Affero General
 Public License "or any later version" applies to it, you have the
 option of following the terms and conditions either of that numbered
 version or of any later version published by the Free Software
 Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
+GNU Affero General Public License, you may choose any version ever published
 by the Free Software Foundation.
 
   If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
+versions of the GNU Affero General Public License can be used, that proxy's
 public statement of acceptance of a version permanently authorizes you
 to choose that version for the Program.
 
   Later license versions may give you additional or different
 permissions.  However, no additional obligations are imposed on any
 author or copyright holder as a result of your choosing to follow a
 later version.
@@ -627,48 +625,37 @@
 free software which everyone can redistribute and change under these terms.
 
   To do so, attach the following notices to the program.  It is safest
 to attach them to the start of each source file to most effectively
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
+    Residential
+    Copyright (C) 2019  CCAO Data Science - Modeling
 
     This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
+    it under the terms of the GNU Affero General Public License as published
+    by the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
+    GNU Affero General Public License for more details.
 
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+For more information on this, and how to apply and follow the GNU AGPL, see
+<http://www.gnu.org/licenses/>.
```

### Comparing `assesspy-1.0.1/assesspy/ci.py` & `assesspy-1.0.2/assesspy/ci.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # Import necessary libraries
 import pandas as pd
 from pandas.api.types import is_numeric_dtype
-from .formulas import cod
-from .formulas import prd
+
+from .formulas import cod, prd
 from .utils import check_inputs
 
 
 def boot_ci(fun, nboot=100, alpha=0.05, **kwargs):
-
     """
     Calculate the non-parametric bootstrap confidence interval
     for a given numeric input and a chosen function.
 
     :param fun:
         Function to bootstrap. Must return a single value.
     :param nboot:
@@ -47,60 +46,64 @@
             assessed = ap.ratios_sample().assessed,
             sale_price = ap.ratios_sample().sale_price,
             nboot = 100
             )
     """
 
     # Make sure prd is passed arguments in correct order
-    if fun.__name__ == 'prd' and set(['assessed', 'sale_price']).issubset(kwargs.keys()):
+    if fun.__name__ == "prd" and set(["assessed", "sale_price"]).issubset(
+        kwargs.keys()
+    ):
         kwargs = (kwargs["assessed"], kwargs["sale_price"])
-    elif fun.__name__ == 'prd' and not set(['assessed', 'sale_price']).issubset(kwargs.keys()):
-        raise Exception(
-                "PRD function expects argurments 'assessed' and 'sale_price'."
-                )
+    elif fun.__name__ == "prd" and not set(["assessed", "sale_price"]).issubset(
+        kwargs.keys()
+    ):
+        raise Exception("PRD function expects argurments 'assessed' and 'sale_price'.")
     else:
         kwargs = tuple(kwargs.values())
 
     check_inputs(kwargs)  # Input checking and error handling
 
     num_kwargs = len(kwargs)
     kwargs = pd.DataFrame(kwargs).T
     n = len(kwargs)
 
     # Check that the input function returns a numeric vector
-    out = fun(kwargs.iloc[:, 0]) if num_kwargs < 2 else fun(
-        kwargs.iloc[:, 0], kwargs.iloc[:, 1]
-        )
+    out = (
+        fun(kwargs.iloc[:, 0])
+        if num_kwargs < 2
+        else fun(kwargs.iloc[:, 0], kwargs.iloc[:, 1])
+    )
     if not is_numeric_dtype(out):
         raise Exception("Input function outputs non-numeric datatype.")
 
     ests = []
 
     # Take a random sample of input, with the same number of rows as input,
     # with replacement.
     for i in list(range(1, nboot)):
         sample = kwargs.sample(n=n, replace=True)
-        if fun.__name__ == 'cod' or num_kwargs == 1:
+        if fun.__name__ == "cod" or num_kwargs == 1:
             ests.append(fun(sample.iloc[:, 0]))
-        elif fun.__name__ == 'prd':
+        elif fun.__name__ == "prd":
             ests.append(fun(sample.iloc[:, 0], sample.iloc[:, 1]))
         else:
             raise Exception(
                 "Input function should require 1 argument or be assesspy.prd."
-                )
+            )
 
     ests = pd.Series(ests)
 
     ci = [ests.quantile(alpha / 2), ests.quantile(1 - alpha / 2)]
 
     return ci
 
 
 # Formula specific bootstrapping functions
 def cod_ci(ratio, nboot=100, alpha=0.05):
-
     return boot_ci(cod, ratio=ratio, nboot=nboot, alpha=alpha)
 
 
 def prd_ci(assessed, sale_price, nboot=100, alpha=0.05):
-
-    return boot_ci(prd, assessed=assessed, sale_price=sale_price, nboot=nboot, alpha=alpha)
+    return boot_ci(
+        prd, assessed=assessed, sale_price=sale_price, nboot=nboot, alpha=alpha
+    )
```

### Comparing `assesspy-1.0.1/assesspy/data/ratios_sample.parquet` & `assesspy-1.0.2/assesspy/data/ratios_sample.parquet`

 * *Files identical despite different names*

### Comparing `assesspy-1.0.1/assesspy/formulas.py` & `assesspy-1.0.2/assesspy/formulas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Import necessary libraries
 import numpy as np
 import statsmodels.api as sm
+
 from .utils import check_inputs
 
 
 # COD, PRD, PRB functions
 def cod(ratio):
-
     """
     COD is the average absolute percent deviation from the
     median ratio. It is a measure of horizontal equity in assessment.
     Horizontal equity means properties with a similar fair market value
     should be similarly assessed.
 
     Lower COD indicates higher uniformity/horizontal equity in assessment.
@@ -54,15 +54,14 @@
     median_ratio = np.median(ratio)
     cod = 100 / median_ratio * (sum(abs(ratio - median_ratio)) / n)
 
     return cod
 
 
 def prd(assessed, sale_price):
-
     """
     PRD is the mean ratio divided by the mean ratio weighted by sale
     price. It is a measure of vertical equity in assessment. Vertical equity
     means that properties at different levels of the income distribution
     should be similarly assessed.
 
     PRD centers slightly above 1 and has a generally accepted value of between
@@ -106,16 +105,15 @@
     ratio = assessed / sale_price
     prd = ratio.mean() / np.average(a=ratio, weights=sale_price)
 
     return prd
 
 
 def prb(assessed, sale_price, round=None):
-
-    """
+    r"""
     PRB is an index of vertical equity that quantifies the
     relationship betweem ratios and assessed values as a percentage. In
     concrete terms, a PRB of 0.02 indicates that, on average, ratios increase
     by 2\% whenever assessed values increase by 100 percent.
 
     PRB is centered around 0 and has a generally accepted value of between
     -0.05 and 0.05, as defined in the `IAAO Standard on Ratio Studies`_
@@ -168,22 +166,26 @@
 
     prb_model = sm.OLS(lhs, rhs).fit()
 
     prb_val = float(prb_model.params)
     prb_ci = prb_model.conf_int(alpha=0.05)[0].tolist()
 
     if round is not None:
+        out = {"prb": np.round(prb_val, round), "95% ci": np.round(prb_ci, round)}
 
-        prb_val = np.round(prb_val, round)
-        prb_ci = np.round(prb_ci, round)
+    else:
+        out = {"prb": prb_val, "95% ci": prb_ci}
 
-    return {"prb": prb_val, "95% ci": prb_ci}
+    return out
 
 
 # Functions to determine whether assessment fairness criteria has been met
-def cod_met(x): return 5 <= x <= 15
+def cod_met(x):
+    return 5 <= x <= 15
 
 
-def prd_met(x): return 0.98 <= x <= 1.03
+def prd_met(x):
+    return 0.98 <= x <= 1.03
 
 
-def prb_met(x): return -0.05 <= x <= 0.05
+def prb_met(x):
+    return -0.05 <= x <= 0.05
```

### Comparing `assesspy-1.0.1/assesspy/load_data.py` & `assesspy-1.0.2/assesspy/load_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Import necessary libraries
-import pkg_resources
 import pandas as pd
+import pkg_resources
 
 
 # Load pre-made ratios sample data.
 def ratios_sample():
-
     """
     This sample was take from Evanston and New Trier in 2019. Ratios are
     calculated using assessor certified (post-appeal) fair market values.
 
     :return:
         A data frame with 979 observation and 4 variables:
 
@@ -20,12 +19,9 @@
         **ratio** (`float`)      Sales ratio representing fair market value / sale price
         **town** (`object`)      Township name the property is in
         ======================== =======================================================
 
     :rtype: DataFrame
     """
 
-    stream = pkg_resources.resource_stream(
-        __name__,
-        'data/ratios_sample.parquet'
-        )
+    stream = pkg_resources.resource_stream(__name__, "data/ratios_sample.parquet")
     return pd.read_parquet(stream)
```

### Comparing `assesspy-1.0.1/assesspy/outliers.py` & `assesspy-1.0.2/assesspy/outliers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,74 +1,65 @@
 # Import necessary libraries
 import numbers
+import warnings
+
 import numpy as np
 from scipy import stats
-import warnings
+
 from .utils import check_inputs
 
 
 # Outlier functions
 def quantile_outlier(x, probs=[0.05, 0.95]):
-
     """
     Quantile method for identifying outliers.
 
     """
 
     check_inputs(x)
 
     # Determine valid range of the data
-    range = [
-        np.quantile(a=x, q=probs[0]),
-        np.quantile(a=x, q=probs[1])
-    ]
+    range = [np.quantile(a=x, q=probs[0]), np.quantile(a=x, q=probs[1])]
 
     # Determine which input values are in range
     out = (x < range[0]) | (x > range[1])
 
     return out
 
 
 def iqr_outlier(x, mult=3):
-
     """
     IQR method for identifying outliers.
 
     """
 
     check_inputs(x)
 
     # Check that inputs are well-formed numeric vector
     if isinstance(mult, numbers.Number) & mult > 0:
-
         # Calculate quartiles and mult*IQR
-        quartiles = [
-            np.quantile(a=x, q=0.25),
-            np.quantile(a=x, q=0.75)
-            ]
+        quartiles = [np.quantile(a=x, q=0.25), np.quantile(a=x, q=0.75)]
 
         iqr_mult = mult * stats.iqr(x)
 
         # Find values that are outliers
         out = (x < (quartiles[0] - iqr_mult)) | (x > (quartiles[1] + iqr_mult))
 
         # Warn if IQR trimmed values are within 95% CI. This indicates
         # potentially non-normal/narrow distribution of data
         if any(out & (quantile_outlier(x) == False)):  # noqa
-
             warnings.warn(
                 """Some values flagged as outliers despite being within 95% CI.
                 Check for narrow or skewed distribution."""
             )
 
         return out
 
 
-def is_outlier(x, method='iqr', probs=[0.05, 0.95]):
-
+def is_outlier(x, method="iqr", probs=[0.05, 0.95]):
     """
     Detect outliers in a numeric vector using standard methods.
 
     Certain assessment performance statistics are sensitive to extreme
     outliers. As such, it is often necessary to remove outliers before
     performing a sales ratio study.
 
@@ -101,22 +92,18 @@
 
         # Detect outliers:
         import assesspy as ap
 
         ap.is_outlier(ap.ratios_sample().ratio)
     """
 
-    out = {
-            'iqr': iqr_outlier(x),
-            'quantile': quantile_outlier(x, probs)
-        }.get(method)
+    out = {"iqr": iqr_outlier(x), "quantile": quantile_outlier(x, probs)}.get(method)
 
     # Warn about removing data from small samples, as it can severely distort
     # ratio study outcomes
     if any(out) & (len(out) < 30):
-
         warnings.warn(
             """Values flagged as outliers despite small sample size (N < 30).
             Use caution when removing values from a small sample."""
-            )
+        )
 
     return out
```

### Comparing `assesspy-1.0.1/assesspy/sales_chasing.py` & `assesspy-1.0.2/assesspy/sales_chasing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Import necessary libraries
+import warnings
+
 import numpy as np
 from statsmodels.distributions.empirical_distribution import ECDF
-import warnings
+
 from .utils import check_inputs
 
 
 # Sales chasing functions
 def detect_chasing_cdf(ratio, bounds=[0.98, 1.02], cdf_gap=0.03):
     # CDF gap method for detecting sales chasing.
 
@@ -21,17 +23,15 @@
     # Calculate the difference between each value and the next value, the
     # largest difference will be the CDF gap
     diffs = np.diff(cdf)
 
     # Check if the largest difference is greater than the threshold and make
     # sure it's within the specified boundaries
     diff_loc = sorted_ratio[np.argmax(diffs)]
-    out = (max(diffs) > cdf_gap) & (
-        (diff_loc > bounds[0]) & (diff_loc < bounds[1])
-        )
+    out = (max(diffs) > cdf_gap) & ((diff_loc > bounds[0]) & (diff_loc < bounds[1]))
 
     return out
 
 
 def detect_chasing_dist(ratio, bounds=[0.98, 1.02]):
     # Distribution comparison method for detecting sales chasing.
 
@@ -42,32 +42,27 @@
 
     # Return the percentage of x within the specified range
     def pct_in_range(x, min, max):
         out = np.mean(((x >= min) & (x <= max)))
         return out
 
     # Calculate the ideal normal distribution using observed values from input
-    ideal_dist = np.random.normal(
-        np.mean(ratio),
-        np.std(ratio),
-        10000
-        )
+    ideal_dist = np.random.normal(np.mean(ratio), np.std(ratio), 10000)
 
     # Determine what percentage of the data would be within the specified
     # bounds in the ideal distribution
     pct_ideal = pct_in_range(ideal_dist, bounds[0], bounds[1])
 
     # Determine what percentage of the data is actually within the bounds
     pct_actual = pct_in_range(ratio, bounds[0], bounds[1])
 
     return pct_actual > pct_ideal
 
 
-def detect_chasing(ratio, method='both'):
-
+def detect_chasing(ratio, method="both"):
     """
     Sales chasing is when a property is selectively reappraised to
     shift its assessed value toward its actual sale price. Sales chasing is
     difficult to detect. This function is NOT a statistical test and does
     not provide the probability of the given result. Rather, it combines two
     novel methods to roughly estimate if sales chasing has occurred.
 
@@ -123,28 +118,28 @@
 
         ecdf = ECDF(chased_ratios)
         pyplot.plot(ecdf.x, ecdf.y)
         pyplot.show()
         ap.detect_chasing(chased_ratios)
     """
 
-    if method not in ('both', 'cdf', 'dist'):
-        raise Exception('Unrecognized method.')
+    if method not in ("both", "cdf", "dist"):
+        raise Exception("Unrecognized method.")
 
     if len(ratio) < 30:
         warnings.warn(
             """
             Sales chasing detection can be misleading when applied to small
             samples (N < 30). Increase N or use a different statistical test.
             """
-            )
+        )
 
         out = None
 
     else:
         out = {
-            'cdf': detect_chasing_cdf(ratio),
-            'dist': detect_chasing_dist(ratio),
-            'both': (detect_chasing_cdf(ratio) & detect_chasing_dist(ratio))
+            "cdf": detect_chasing_cdf(ratio),
+            "dist": detect_chasing_dist(ratio),
+            "both": (detect_chasing_cdf(ratio) & detect_chasing_dist(ratio)),
         }.get(method)
 
     return out
```

### Comparing `assesspy-1.0.1/assesspy/tests/test_ci.py` & `assesspy-1.0.2/assesspy/tests/test_ci.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,141 +1,122 @@
 # Import necessary libraries
-import assesspy
 import numpy as np
-from numpy import testing as npt
 import pandas as pd
 import pytest as pt
+from numpy import testing as npt
+
+import assesspy
 
 # Load the ratios sample dataset for testing
 ratios_sample = assesspy.ratios_sample()
 
 ratio = ratios_sample.ratio
 assessed = ratios_sample.assessed
 sale_price = ratios_sample.sale_price
 
 ##### TEST BOOT CI ##### # noqa
 
 
 class TestBOOTCI:  # Ensure input function is appropriate
-
     def test_in_fun(self):
-
         with pt.raises(Exception):
-            assert assesspy.boot_ci(str, ratio = ratio)
+            assert assesspy.boot_ci(str, ratio=ratio)
 
         with pt.raises(Exception):
-            assesspy.boot_ci(np.add, one = ratio, two = ratio, three = ratio)
+            assesspy.boot_ci(np.add, one=ratio, two=ratio, three=ratio)
 
         with pt.raises(Exception):
-            assesspy.boot_ci(assesspy.prd, fmv = assessed, sale_price = sale_price)
+            assesspy.boot_ci(assesspy.prd, fmv=assessed, sale_price=sale_price)
 
         with pt.raises(Exception):
-            assesspy.boot_ci(np.add, one = ratio, two = ratio)
+            assesspy.boot_ci(np.add, one=ratio, two=ratio)
+
 
 ##### TEST COD ##### # noqa
 
 
 # Calculate COD CI
 cod_ci_out_95 = assesspy.cod_ci(ratio, nboot=1000)
 cod_ci_out_80 = assesspy.cod_ci(ratio, nboot=1000, alpha=0.2)
 
 
 class TestCODCI:
-
     def test_output_type(self):  # Output is expected type
-
         assert type(cod_ci_out_95) is list
         assert type(cod_ci_out_95[0]) is np.float64
 
     def test_cod(self):  # Output equal to expected
-
         npt.assert_allclose(
-            cod_ci_out_80,
-            [16.89576541901062, 18.641992815316588],
-            rtol=0.02
-            )
+            cod_ci_out_80, [16.89576541901062, 18.641992815316588], rtol=0.02
+        )
         npt.assert_allclose(
-            cod_ci_out_95,
-            [16.32413038955943, 19.226428249424757],
-            rtol=0.02
-            )
+            cod_ci_out_95, [16.32413038955943, 19.226428249424757], rtol=0.02
+        )
 
     def test_bad_input(self):  # Bad input data stops execution
-
         with pt.raises(Exception):
             assesspy.cod_ci([1] * 29 + [0])
 
         with pt.raises(Exception):
             assesspy.cod_ci(10)
 
         with pt.raises(Exception):
-            assesspy.cod_ci(
-                pd.concat([ratio, pd.Series(float('Inf'))])
-                )
+            assesspy.cod_ci(pd.concat([ratio, pd.Series(float("Inf"))]))
 
         with pt.raises(Exception):
             assesspy.cod_ci(pd.DataFrame(ratio))
 
         with pt.raises(Exception):
-            assesspy.cod_ci(
-                pd.concat([ratio, pd.Series(float('NaN'))])
-                )
+            assesspy.cod_ci(pd.concat([ratio, pd.Series(float("NaN"))]))
 
         with pt.raises(Exception):
-            assesspy.cod_ci([1] * 29 + ['1'])
+            assesspy.cod_ci([1] * 29 + ["1"])
+
 
 ##### TEST PRD ##### # noqa
 
 
 # Calculate PRD CI
 prd_ci_out_95 = assesspy.prd_ci(assessed, sale_price, nboot=1000)
 prd_ci_out_80 = assesspy.prd_ci(assessed, sale_price, nboot=1000, alpha=0.2)
 
 
 class TestPRDCI:
-
     def test_output_type(self):  # Output is expected type
-
         assert type(prd_ci_out_95) is list
         assert type(prd_ci_out_95[0]) is np.float64
 
     def test_prd(self):  # Output equal to expected
-
         npt.assert_allclose(
-            prd_ci_out_80,
-            [1.0388355155405569, 1.0588098520230935],
-            rtol=0.02
-            )
+            prd_ci_out_80, [1.0388355155405569, 1.0588098520230935], rtol=0.02
+        )
         npt.assert_allclose(
-            prd_ci_out_95,
-            [1.0333716711646226, 1.0643056985556307],
-            rtol=0.02
-            )
+            prd_ci_out_95, [1.0333716711646226, 1.0643056985556307], rtol=0.02
+        )
 
     def test_bad_input(self):  # Bad input data stops execution
-
         with pt.raises(Exception):
             assesspy.prd_ci([1] * 30, [1] * 29 + [0])
 
         with pt.raises(Exception):
             assesspy.prd_ci([1, 1, 1], [1, 1])
 
         with pt.raises(Exception):
             assesspy.prd_ci(10, 10)
 
         with pt.raises(Exception):
             assesspy.prd_ci(
-                pd.concat([assessed, pd.Series(float('Inf'))]),
-                pd.concat([sale_price, pd.Series(1.0)])
-                )
+                pd.concat([assessed, pd.Series(float("Inf"))]),
+                pd.concat([sale_price, pd.Series(1.0)]),
+            )
 
         with pt.raises(Exception):
             assesspy.prd_ci(pd.DataFrame(ratio))
 
         with pt.raises(Exception):
             assesspy.prd_ci(
-                pd.concat([assessed, pd.Series(float('NaN'))]),
-                pd.concat([sale_price, pd.Series(1.0)])
-                )
+                pd.concat([assessed, pd.Series(float("NaN"))]),
+                pd.concat([sale_price, pd.Series(1.0)]),
+            )
 
         with pt.raises(Exception):
-            assesspy.prd_ci([1] * 30, [1] * 29 + ['1'])
+            assesspy.prd_ci([1] * 30, [1] * 29 + ["1"])
```

### Comparing `assesspy-1.0.1/assesspy/tests/test_formulas.py` & `assesspy-1.0.2/assesspy/tests/test_formulas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Import necessary libraries
-import assesspy
 import numpy as np
-from numpy import testing as npt
 import pandas as pd
 import pytest as pt
+from numpy import testing as npt
+
+import assesspy
 
 # Load the ratios sample dataset for testing
 ratios_sample = assesspy.ratios_sample()
 
 ratio = ratios_sample.ratio
 fmv = ratios_sample.assessed
 sale_price = ratios_sample.sale_price
@@ -15,148 +16,132 @@
 ##### TEST COD ##### # noqa
 
 # Calculate COD
 cod_out = assesspy.cod(ratios_sample.ratio)
 
 
 class TestCOD:
-
     def test_cod(self):  # Output equal to expected
-
         npt.assert_allclose(cod_out, 17.81456901196891, rtol=0.02)
 
     def test_numeric_output(self):  # Output is numeric
-
         assert type(cod_out) is np.float64
 
     def test_bad_input(self):  # Bad input data stops execution
-
         with pt.raises(Exception):
             assesspy.cod([1] * 29 + [0])
 
         with pt.raises(Exception):
             assesspy.cod(10)
 
         with pt.raises(Exception):
-            assesspy.cod(
-                pd.concat([ratio, pd.Series(float('Inf'))])
-                )
+            assesspy.cod(pd.concat([ratio, pd.Series(float("Inf"))]))
 
         with pt.raises(Exception):
             assesspy.cod(pd.DataFrame(ratio))
 
         with pt.raises(Exception):
-            assesspy.cod(
-                pd.concat([ratio, pd.Series(float('NaN'))])
-                )
+            assesspy.cod(pd.concat([ratio, pd.Series(float("NaN"))]))
 
         with pt.raises(Exception):
-            assesspy.cod([1] * 29 + ['1'])
+            assesspy.cod([1] * 29 + ["1"])
 
     def test_cod_met(self):  # Standard met function
-
         assert not assesspy.cod_met(cod_out)
 
+
 ##### TEST PRD ##### # noqa
 
 
 # Calculate PRD
 prd_out = assesspy.prd(fmv, sale_price)
 
 
 class TestPRD:
-
     def test_prd(self):  # Output equal to expected
-
         npt.assert_allclose(prd_out, 1.0484192615223522, rtol=0.02)
 
     def test_numeric_output(self):  # Output is numeric
-
         assert type(prd_out) is np.float64
 
     def test_bad_input(self):  # Bad input data stops execution
-
         with pt.raises(Exception):
             assesspy.prd_ci([1] * 30, [1] * 29 + [0])
 
         with pt.raises(Exception):
             assesspy.prd_ci([1, 1, 1], [1, 1])
 
         with pt.raises(Exception):
             assesspy.prd(10, 10)
 
         with pt.raises(Exception):
             assesspy.prd(
-                pd.concat([fmv, pd.Series(float('Inf'))]),
-                pd.concat([sale_price, pd.Series(1.0)])
-                )
+                pd.concat([fmv, pd.Series(float("Inf"))]),
+                pd.concat([sale_price, pd.Series(1.0)]),
+            )
 
         with pt.raises(Exception):
             assesspy.prd(pd.DataFrame(ratio))
 
         with pt.raises(Exception):
             assesspy.prd(
-                pd.concat([fmv, pd.Series(float('NaN'))]),
-                pd.concat([sale_price, pd.Series(1.0)])
-                )
+                pd.concat([fmv, pd.Series(float("NaN"))]),
+                pd.concat([sale_price, pd.Series(1.0)]),
+            )
 
         with pt.raises(Exception):
-            assesspy.prd([1] * 30, [1] * 29 + ['1'])
+            assesspy.prd([1] * 30, [1] * 29 + ["1"])
 
     def test_prd_met(self):  # Standard met function
-
         assert not assesspy.prd_met(prd_out)
 
 
 ##### TEST PRB ##### # noqa
 
 # Calculate PRB
-prb_out = assesspy.prb(fmv, sale_price)['prb']
+prb_out = assesspy.prb(fmv, sale_price)["prb"]
 
 
 class TestPRB:
-
     def test_prb(self):  # Output equal to expected
-
         npt.assert_allclose(prb_out, 0.0009470721642262901, rtol=0.02)
 
     def test_numeric_output(self):  # Output is numeric
-
         assert type(prb_out) is float
 
     def test_bad_input(self):  # Bad input data stops execution
-
         with pt.raises(Exception):
             assesspy.prb_ci([1] * 30, [1] * 29 + [0])
 
         with pt.raises(Exception):
             assesspy.prb([1, 1, 1], [1, 1])
 
         with pt.raises(Exception):
             assesspy.prb(10, 10)
 
         with pt.raises(Exception):
             assesspy.prb(
-                pd.concat([fmv, pd.Series(float('Inf'))]),
-                pd.concat([sale_price, pd.Series(1.0)])
-                )
+                pd.concat([fmv, pd.Series(float("Inf"))]),
+                pd.concat([sale_price, pd.Series(1.0)]),
+            )
 
         with pt.raises(Exception):
             assesspy.prb(pd.DataFrame(ratio))
 
         with pt.raises(Exception):
             assesspy.prb(
-                pd.concat([fmv, pd.Series(float('NaN'))]),
-                pd.concat([sale_price, pd.Series(1.0)])
-                )
+                pd.concat([fmv, pd.Series(float("NaN"))]),
+                pd.concat([sale_price, pd.Series(1.0)]),
+            )
 
         with pt.raises(Exception):
-            assesspy.prb([1] * 30, [1] * 29 + ['1'])
+            assesspy.prb([1] * 30, [1] * 29 + ["1"])
 
     def test_round(self):  # Rounding must be int
+        with pt.raises(Exception):
+            assesspy.prb(fmv, sale_price, "z")
 
         with pt.raises(Exception):
-            assesspy.prb(fmv, sale_price, 'z')
+            assesspy.prb(fmv, sale_price, 1.1)
 
     def test_prb_met(self):  # Standard met function
-
         assert assesspy.prb_met(prb_out)
```

### Comparing `assesspy-1.0.1/assesspy/tests/test_outliers.py` & `assesspy-1.0.2/assesspy/tests/test_outliers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,69 @@
 # Import necessary libraries
-import assesspy
 import numpy as np
 import pandas as pd
 import pytest as pt
 
+import assesspy
+
 # Create test vectors of data with certain distributions
 np.random.seed(13378)
 
 # Normal distribution, no outliers
 test_dist1 = np.random.normal(size=100)
 
 # Normal distribution, some outliers
 test_dist2 = np.append(np.random.normal(size=100), [3, 4, 5, 6, 7])
 
 # Non-normal, super narrow distribution
 test_dist3 = np.append(
-    np.append(
-        np.random.uniform(size=20), np.repeat(1, 50)
-        ), [5, 6, 7]
-        )
+    np.append(np.random.uniform(size=20), np.repeat(1, 50)), [5, 6, 7]
+)
 
 # Create outputs for all distributions
 dist1_iqr_out = assesspy.is_outlier(test_dist1, method="iqr")
 dist1_qnt_out = assesspy.is_outlier(test_dist1, method="quantile")
 dist2_iqr_out = assesspy.is_outlier(test_dist2, method="iqr")
 dist2_qnt_out = assesspy.is_outlier(test_dist2, method="quantile")
 
 ##### TEST OUTLIER ##### # noqa
 
 
 class TestOUTTIES:
-
     def test_output_type(self):  # Output is logical array
-
         assert type(dist1_iqr_out[0]) is np.bool_
         assert type(dist1_iqr_out) is np.ndarray
 
         assert type(dist1_qnt_out[0]) is np.bool_
         assert type(dist1_qnt_out) is np.ndarray
 
     def test_output_value(self):
-
         assert sum(dist1_iqr_out) == 0
         assert sum(dist1_qnt_out) == 10
         assert sum(dist2_iqr_out) == 3
         assert sum(dist2_qnt_out) == 12
 
     def test_bad_input(self):  # Bad input data stops execution
-
         with pt.raises(Exception):
             assesspy.is_outlier([1] * 29 + [0])
 
         with pt.raises(Exception):
             assesspy.is_outlier(10)
 
         with pt.raises(Exception):
-            assesspy.is_outlier(
-                np.append(test_dist1, float('Inf'))
-                )
+            assesspy.is_outlier(np.append(test_dist1, float("Inf")))
 
         with pt.raises(Exception):
             assesspy.is_outlier(pd.DataFrame(test_dist1))
 
         with pt.raises(Exception):
-            assesspy.is_outlier(
-                np.append(test_dist1, float('NaN'))
-                )
+            assesspy.is_outlier(np.append(test_dist1, float("NaN")))
 
         with pt.raises(Exception):
-            assesspy.is_outlier([1] * 29 + ['1'])
+            assesspy.is_outlier([1] * 29 + ["1"])
 
     def test_warnings(self):
-
         with pt.warns(UserWarning):
             assesspy.is_outlier(test_dist3, method="iqr")
 
         with pt.warns(UserWarning):
             assesspy.is_outlier(np.random.normal(size=20), method="quantile")
```

### Comparing `assesspy-1.0.1/assesspy/tests/test_sales_chasing.py` & `assesspy-1.0.2/assesspy/tests/test_sales_chasing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,62 @@
 # Import necessary libraries
 # Import necessary libraries
-import assesspy
 import numpy as np
 import pandas as pd
 import pytest as pt
 
+import assesspy
+
 # Create test vectors of data with certain distributions
 np.random.seed(13378)
 
 # Load the ratios sample dataset for testing
 ratios_sample = assesspy.ratios_sample()
 
 # Extract the components of the dataframe as vectors
 sample_ratios = ratios_sample.ratio
-normal_ratios = np.random.normal(1, .15, 100)
-chased_ratios = np.append(np.random.normal(1, .15, 900), [1] * 100)
+normal_ratios = np.random.normal(1, 0.15, 100)
+chased_ratios = np.append(np.random.normal(1, 0.15, 900), [1] * 100)
 
 ##### TEST CHASING DETECTION ##### # noqa
 
 # Run detection
 sample_out = assesspy.detect_chasing(sample_ratios)
 normal_out = assesspy.detect_chasing(normal_ratios)
 chased_out = assesspy.detect_chasing(chased_ratios)
 
 
 class TestCHASE:
-
     def test_method(self):
-
         with pt.raises(Exception):
-            assesspy.detect_chasing(sample_ratios, method='hug')
+            assesspy.detect_chasing(sample_ratios, method="hug")
 
     def test_output_type(self):  # Output is logical
-
         assert type(sample_out) is np.bool_
 
     def test_output_value(self):
-
         assert not sample_out
         assert not normal_out
         assert chased_out
 
     def test_bad_input(self):  # Bad input data stops execution
-
         with pt.raises(Exception):
             assesspy.detect_chasing([1] * 29 + [0])
 
         with pt.raises(Exception):
             assesspy.detect_chasing(10)
 
         with pt.raises(Exception):
-            assesspy.detect_chasing(
-                np.append(sample_ratios, float('Inf'))
-                )
+            assesspy.detect_chasing(np.append(sample_ratios, float("Inf")))
 
         with pt.raises(Exception):
             assesspy.detect_chasing(pd.DataFrame(sample_ratios))
 
         with pt.raises(Exception):
-            assesspy.detect_chasing(
-                np.append(sample_ratios, float('NaN'))
-                )
+            assesspy.detect_chasing(np.append(sample_ratios, float("NaN")))
 
         with pt.raises(Exception):
-            assesspy.detect_chasing([1] * 29 + ['1'])
+            assesspy.detect_chasing([1] * 29 + ["1"])
 
     def test_warnings(self):  # Small sample throughs a warning
-
         with pt.warns(UserWarning):
-            assesspy.detect_chasing(np.random.normal(size=29))
+            assesspy.detect_chasing(np.random.normal(size=29))
```

### Comparing `assesspy-1.0.1/assesspy/utils.py` & `assesspy-1.0.2/assesspy/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 # Import necessary libraries
-from pandas.api.types import is_numeric_dtype
 import numpy as np
 import pandas as pd
+from pandas.api.types import is_numeric_dtype
 
 
 def check_inputs(*args):
-
-    out = ['']
+    out = [""]
 
     for x in args:
-
         # *args passed into *args can created nested tuples - unnest
         if isinstance(x, tuple):
             args = x
 
     for x in args:
-
         if type(x) == pd.core.frame.DataFrame:
-            raise Exception('Input cannot be a dataframe.')
+            raise Exception("Input cannot be a dataframe.")
 
         check = pd.Series(x)
 
         if not is_numeric_dtype(check):
-            raise Exception('All input vectors must be numeric.')
+            raise Exception("All input vectors must be numeric.")
         if check.isnull().values.any():
-            out.append('\nInput vectors contain null values.')
+            out.append("\nInput vectors contain null values.")
         if len(check) <= 1:
-            out.append('\nAll input vectors must have length greater than 1.')
+            out.append("\nAll input vectors must have length greater than 1.")
         if not all(np.isfinite(check) | check.isnull()):
-            out.append('\nInfinite values in input vectors.')
+            out.append("\nInfinite values in input vectors.")
         if any(check == 0):
-            out.append('\nInput vectors cannot contain values of 0.')
+            out.append("\nInput vectors cannot contain values of 0.")
 
     out = set(out)
 
     if len(out) > 1:
-        raise Exception(''.join(map(str, out)))
+        raise Exception("".join(map(str, out)))
```

### Comparing `assesspy-1.0.1/assesspy.egg-info/SOURCES.txt` & `assesspy-1.0.2/assesspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assesspy-1.0.1/setup.py` & `assesspy-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from setuptools import setup, find_packages
-
 # read the contents of your README file, remove image
 from pathlib import Path
+
+from setuptools import find_packages, setup
+
 this_directory = Path(__file__).parent
-image = '<a href="https://gitlab.com/ccao-data-science---modeling/packages/assesspy"><img src="docs/images/logo.png" align="right" height="139"/></a>'
+image = '<a href="https://github.com/ccao-data/assesspy/tree/main"><img src="docs/images/logo.png" align="right" height="139"/></a>'
 long_description = (this_directory / "README.md").read_text().replace(image, '')
 
 setup(
     name="assesspy",
-    version="1.0.1",
+    version="1.0.2",
     description="General purpose Python package for measuring assessment performance",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url="https://gitlab.com/ccao-data-science---modeling/packages/assesspy/",
+    url="https://github.com/ccao-data/assesspy",
     author="CCAO",
     author_email="assessor.data@cookcountyil.gov",
-    license="GPL-3",
+    license="AGPL-3",
     packages=find_packages(),
     install_requires=[
         "pandas",
         "pyarrow",
         "numpy",
         "scipy",
-        "sklearn",
         "statsmodels"
         ],
     setup_requires=["pytest-runner"],
     tests_require=["pytest", "pytest-cov"],
     include_package_data = True,
     package_data={
         "": ["*.parquet"],
     }
-    )
+    )
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
-from setuptools import setup, find_packages # read the contents of your README
-file, remove image from pathlib import Path this_directory = Path
+# read the contents of your README file, remove image from pathlib import Path
+from setuptools import find_packages, setup this_directory = Path
 (__file__).parent image = '[docs/images/logo.png]' long_description =
 (this_directory / "README.md").read_text().replace(image, '') setup
-( name="assesspy", version="1.0.1", description="General purpose Python package
+( name="assesspy", version="1.0.2", description="General purpose Python package
 for measuring assessment performance", long_description=long_description,
-long_description_content_type='text/markdown', url="https://gitlab.com/ccao-
-data-science---modeling/packages/assesspy/", author="CCAO",
-author_email="assessor.data@cookcountyil.gov", license="GPL-3",
-packages=find_packages(), install_requires=[ "pandas", "pyarrow", "numpy",
-"scipy", "sklearn", "statsmodels" ], setup_requires=["pytest-runner"],
+long_description_content_type='text/markdown', url="https://github.com/ccao-
+data/assesspy", author="CCAO", author_email="assessor.data@cookcountyil.gov",
+license="AGPL-3", packages=find_packages(), install_requires=[ "pandas",
+"pyarrow", "numpy", "scipy", "statsmodels" ], setup_requires=["pytest-runner"],
 tests_require=["pytest", "pytest-cov"], include_package_data = True,
 package_data={ "": ["*.parquet"], } )
```


# Comparing `tmp/mapdata-2.8.6.tar.gz` & `tmp/mapdata-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-2.8.6.tar", last modified: Mon Jul  3 18:55:12 2023, max compression
+gzip compressed data, was "mapdata-2.9.0.tar", last modified: Wed Jul 12 03:55:14 2023, max compression
```

## Comparing `mapdata-2.8.6.tar` & `mapdata-2.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-07-03 18:55:12.982781 mapdata-2.8.6/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.8.6/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.8.6/MANIFEST.in
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-07-03 18:55:12.982781 mapdata-2.8.6/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     2870 2023-06-28 13:59:57.000000 mapdata-2.8.6/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-07-03 18:55:12.982781 mapdata-2.8.6/mapdata/
--rwxrwxr-x   0 dreas     (1000) dreas     (1000)   339131 2023-07-03 18:22:21.000000 mapdata-2.8.6/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-07-03 18:55:12.982781 mapdata-2.8.6/mapdata.egg-info/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-07-03 18:55:12.000000 mapdata-2.8.6/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-07-03 18:55:12.000000 mapdata-2.8.6/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-07-03 18:55:12.000000 mapdata-2.8.6/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-07-03 18:55:12.000000 mapdata-2.8.6/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-07-03 18:55:12.982781 mapdata-2.8.6/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1366 2023-07-03 12:55:05.000000 mapdata-2.8.6/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-07-12 03:55:14.317345 mapdata-2.9.0/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.9.0/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.9.0/MANIFEST.in
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-07-12 03:55:14.317345 mapdata-2.9.0/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     2870 2023-06-28 13:59:57.000000 mapdata-2.9.0/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-07-12 03:55:14.317345 mapdata-2.9.0/mapdata/
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   341285 2023-07-12 03:39:29.000000 mapdata-2.9.0/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-07-12 03:55:14.317345 mapdata-2.9.0/mapdata.egg-info/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-07-12 03:55:14.000000 mapdata-2.9.0/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-07-12 03:55:14.000000 mapdata-2.9.0/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-07-12 03:55:14.000000 mapdata-2.9.0/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-07-12 03:55:14.000000 mapdata-2.9.0/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-07-12 03:55:14.317345 mapdata-2.9.0/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1366 2023-07-12 03:40:02.000000 mapdata-2.9.0/setup.py
```

### Comparing `mapdata-2.8.6/LICENSE.txt` & `mapdata-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-2.8.6/PKG-INFO` & `mapdata-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.8.6
+Version: 2.9.0
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-2.8.6/README.md` & `mapdata-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mapdata-2.8.6/mapdata/mapdata.py` & `mapdata-2.9.0/mapdata/mapdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # 	The GNU General Public License is available at <http://www.gnu.org/licenses/>
 #
 # AUTHOR
 #	Dreas Nielsen (RDN)
 #
 # ==================================================================
 
-version = "2.8.6"
-vdate = "2023-07-03"
+version = "2.9.0"
+vdate = "2023-07-11"
 
 copyright = "2023"
 
 
 import sys
 import os.path
 import io
@@ -37,14 +37,15 @@
 import argparse
 from configparser import ConfigParser
 import csv
 import re
 import datetime
 import time
 import math
+import statistics
 import collections
 import webbrowser
 import threading
 import queue
 import sqlite3
 import tempfile
 import random
@@ -737,14 +738,41 @@
 	win.update_idletasks()
 	m = re.match(r"(\d+)x(\d+)\+(-?\d+)\+(-?\d+)", win.geometry())
 	if m is not None:
 		xpos = int(m.group(1)) + x_offset
 		ypos = int(m.group(2)) + y_offset
 		win.geometry("+%d+%d" % (xpos, ypos))
 
+# Inverse normal CDF function (qnorm) by Acklam's algorithm
+A = (-3.969683028665376e+01, 2.209460984245205e+02, -2.759285104469687e+02,
+		1.383577518672690e+02, -3.066479806614716e+01, 2.506628277459239e+00)
+B = (-5.447609879822406e+01, 1.615858368580409e+02, -1.556989798598866e+02,
+		6.680131188771972e+01, -1.328068155288572e+01)
+C = (-7.784894002430293e-03, -3.223964580411365e-01, -2.400758277161838e+00,
+		-2.549732539343734e+00, 4.374664141464968e+00, 2.938163982698783e+00)
+D = (7.784695709041462e-03, 3.224671290700398e-01, 2.445134137142996e+00,
+		3.754408661907416e+00)
+P_LOW = 0.02425
+P_HIGH = 1.0 - P_LOW
+def qnorm(p):
+	if p <= 0 or p >= 1.0:
+		raise ValueError("Invalid input to qnorm()")
+	if p >= P_LOW and p <= P_HIGH:
+		q = p - 0.5
+		r = q*q
+		return (((((A[0]*r+A[1])*r+A[2])*r+A[3])*r+A[4])*r+A[5])*q / \
+        (((((B[0]*r+B[1])*r+B[2])*r+B[3])*r+B[4])*r+1)
+	elif p < P_LOW:
+		q = math.sqrt(-2 * math.log(p))
+		return (((((C[0]*q+C[1])*q+C[2])*q+C[3])*q+C[4])*q+C[5]) / \
+         ((((D[0]*q+D[1])*q+D[2])*q+D[3])*q+1)
+	else:
+		q = math.sqrt(-2 * math.log(1.0 - p))
+		return -(((((C[0]*q+C[1])*q+C[2])*q+C[3])*q+C[4])*q+C[5]) / \
+          ((((D[0]*q+D[1])*q+D[2])*q+D[3])*q+1)
 
 
 class MapUI(object):
 	def __init__(self, src_name, message, lat_col, lon_col, crs=4326, sheet=None,
 			label_col=None, symbol_col=None, color_col=None,
 			map_export_file=None, export_time_sec=10):
 		self.win = tk.Tk()
@@ -2734,15 +2762,15 @@
 		ctrl_frame = tk.Frame(self.dlg)
 		ctrl_frame.grid(row=1, column=0, sticky=tk.N+tk.EW)
 
 		self.type_var = tk.StringVar(ctrl_frame, "")
 		type_lbl = ttk.Label(ctrl_frame, text="Plot type:")
 		type_lbl.grid(row=0, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
 		self.type_sel = ttk.Combobox(ctrl_frame, state="readonly", textvariable=self.type_var, width=20,
-				values=["Box plot", "Category counts", "Empirical CDF", "Histogram", "Line plot", "Scatter plot", "Y range plot"])
+				values=["Box plot", "Category counts", "Empirical CDF", "Histogram", "Line plot", "Normal Q-Q plot", "Scatter plot", "Y range plot"])
 		self.type_sel.grid(row=0, column=1, columnspan=2, sticky=tk.W, padx=(3,6), pady=(3,3))
 		self.type_sel.bind("<<ComboboxSelected>>", self.set_xy)
 
 		self.sel_only_var = tk.StringVar(ctrl_frame, "0")
 		self.sel_only_ck = ttk.Checkbutton(ctrl_frame, text="Selected data only", command=self.q_redraw, variable=self.sel_only_var,
 				onvalue="1", offvalue="0")
 		self.sel_only_ck.grid(row=1, column=0, columnspan=2, sticky=tk.W, padx=(6,3), pady=(3,3))
@@ -2908,15 +2936,15 @@
 		self.y_sel["state"] = "readonly"
 		plot_type = self.type_var.get()
 		if plot_type == "Category counts":
 			self.x_sel["values"] = categ_columns
 			self.xlog_ck["state"] = "disabled"
 			self.y_sel["state"] = "disabled"
 			self.ylog_ck["state"] = "disabled"
-		elif plot_type in ("Histogram", "Empirical CDF"):
+		elif plot_type in ("Histogram", "Empirical CDF", "Normal Q-Q plot"):
 			self.x_sel["values"] = numeric_columns
 			self.y_sel["state"] = "disabled"
 			self.ylog_ck["state"] = "disabled"
 			if plot_type == "Histogram":
 				self.dlg.bind("<Alt-b>", self.set_bins)
 		elif plot_type == "Box plot":
 			self.x_sel["values"] = list(set(categ_columns) | set(date_columns))
@@ -2925,15 +2953,15 @@
 		else:
 			self.x_sel["values"] = quant_columns
 			self.y_sel["values"] = quant_columns
 
 	def q_redraw(self, get_data=True, *args):
 		# Conditionally (re)draw the plot.
 		plot_type = self.type_var.get()
-		can_redraw = (plot_type in ("Category counts", "Empirical CDF", "Histogram") and self.x_var.get() != '') \
+		can_redraw = (plot_type in ("Category counts", "Empirical CDF", "Normal Q-Q plot", "Histogram") and self.x_var.get() != '') \
 				or (plot_type in ("Scatter plot", "Line plot", "Box plot", "Y range plot") and self.x_var.get() != '' and self.y_var.get() != '')
 		if can_redraw:
 			self.plotfig.clear()
 			self.plot_axes = self.plotfig.add_subplot(111)
 			self.plotfig_canvas.draw()
 			if get_data or self.dataset is None or self.plot_data is None:
 				self.get_data()
@@ -3041,14 +3069,25 @@
 				self.plot_data_labels = x_vals
 			elif plot_type == "Empirical CDF":
 				# Y is the fraction of data points below each X value
 				x_counts = np.unique(self.dataset[0], return_counts=True)
 				y_vals = list(np.cumsum(x_counts[1]/np.sum(x_counts[1])))
 				self.plot_data = [list(x_counts[0]), y_vals]
 				self.plot_data_labels = [self.data_labels[0], "Cumulative frequency"]
+			elif plot_type == "Normal Q-Q plot":
+				x_vals = list(set(self.dataset[0]))
+				x_vals.sort()
+				x_mean = statistics.mean(x_vals)
+				x_sd = statistics.stdev(x_vals)
+				x_quantiles = [(x - x_mean)/x_sd for x in x_vals]
+				x_len = len(x_vals)
+				q = [(i + 0.5)/x_len for i in range(x_len)]
+				norm_quantiles = [qnorm(p) for p in q]
+				self.plot_data = [x_vals, x_quantiles, norm_quantiles]
+				self.plot_data_labels = [self.x_var.get(), "Sample quantiles", "Theoretical quantiles"]
 			elif plot_type == "Y range plot":
 				# Min and max Y for each X
 				x_vals = list(set(self.dataset[0]))
 				x_vals.sort()
 				y_vals = [[None, None]] * len(x_vals)
 				plotdata = dict(zip(x_vals, y_vals))
 				for i in range(len(self.dataset[0])):
@@ -3095,14 +3134,21 @@
 				self.plot_axes.plot(self.plot_data[0], self.plot_data[1])
 				self.plot_axes.set_xlabel(self.plot_data_labels[0])
 				self.plot_axes.set_ylabel(self.plot_data_labels[1])
 			elif plot_type == "Empirical CDF":
 				self.plot_axes.stackplot(self.plot_data[0], self.plot_data[1])
 				self.plot_axes.set_xlabel(self.plot_data_labels[0])
 				self.plot_axes.set_ylabel(self.plot_data_labels[1])
+			elif plot_type == "Normal Q-Q plot":
+				self.plot_axes.scatter(self.plot_data[2], self.plot_data[1])
+				pmin = min(self.plot_data[2][0], self.plot_data[1][0])
+				pmax = max(self.plot_data[2][-1], self.plot_data[1][-1])
+				self.plot_axes.plot([pmin, pmax], [pmin, pmax])
+				self.plot_axes.set_xlabel(self.plot_data_labels[2])
+				self.plot_axes.set_ylabel(self.plot_data_labels[1])
 			elif plot_type == "Y range plot":
 				self.plot_axes.fill_between(self.plot_data[0], self.plot_data[1], self.plot_data[2])
 				self.plot_axes.set_xlabel(self.x_var.get())
 				self.plot_axes.set_ylabel(self.y_var.get())
 			elif plot_type == "Box plot":
 				self.plot_axes.boxplot(self.plot_data, labels=self.plot_data_labels)
 				self.plot_axes.set_xlabel(self.x_var.get())
```

### Comparing `mapdata-2.8.6/mapdata.egg-info/PKG-INFO` & `mapdata-2.9.0/mapdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.8.6
+Version: 2.9.0
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-2.8.6/setup.py` & `mapdata-2.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import io
 
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 setuptools.setup(name='mapdata',
-	version='2.8.6',
+	version='2.9.0',
 	description="An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database",
 	author='Dreas Nielsen',
 	author_email='dreas.nielsen@gmail.com',
     url='https://osdn.net/project/mapdata/',
 	scripts=['mapdata/mapdata.py'],
     license='GPL',
 	requires=['tkintermapview', 'pyproj', 'odfpy', 'openpyxl', 'xlrd', 'matplotlib'],
```


# Comparing `tmp/inviz-0.2.0.tar.gz` & `tmp/inviz-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.2.0.tar", last modified: Tue Jul 11 00:27:56 2023, max compression
+gzip compressed data, was "inviz-0.2.1.tar", last modified: Wed Jul 12 08:20:13 2023, max compression
```

## Comparing `inviz-0.2.0.tar` & `inviz-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-11 00:27:56.098684 inviz-0.2.0/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.0/LICENSE
--rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.0/MANIFEST.in
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2165 2023-07-11 00:27:56.098684 inviz-0.2.0/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1643 2023-06-15 14:20:14.000000 inviz-0.2.0/README.md
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-11 00:27:56.088684 inviz-0.2.0/inviz/
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-11 00:27:56.098684 inviz-0.2.0/inviz/inviz.egg-info/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2165 2023-07-11 00:27:55.000000 inviz-0.2.0/inviz/inviz.egg-info/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-07-11 00:27:55.000000 inviz-0.2.0/inviz/inviz.egg-info/SOURCES.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-07-11 00:27:55.000000 inviz-0.2.0/inviz/inviz.egg-info/dependency_links.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)       89 2023-07-11 00:27:55.000000 inviz-0.2.0/inviz/inviz.egg-info/requires.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-07-11 00:27:55.000000 inviz-0.2.0/inviz/inviz.egg-info/top_level.txt
--rwxr-xr-x   0 jswen     (1000) jswen     (1000)    10342 2023-07-10 23:57:56.000000 inviz-0.2.0/inviz/inviz.py
--rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-07-11 00:27:56.098684 inviz-0.2.0/setup.cfg
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1100 2023-07-11 00:03:27.000000 inviz-0.2.0/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-12 08:20:13.456552 inviz-0.2.1/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.1/LICENSE
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.1/MANIFEST.in
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-07-12 08:20:13.456552 inviz-0.2.1/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1641 2023-07-12 08:18:52.000000 inviz-0.2.1/README.md
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-12 08:20:13.456552 inviz-0.2.1/inviz/
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-12 08:20:13.456552 inviz-0.2.1/inviz/inviz.egg-info/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-07-12 08:20:13.000000 inviz-0.2.1/inviz/inviz.egg-info/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-07-12 08:20:13.000000 inviz-0.2.1/inviz/inviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-07-12 08:20:13.000000 inviz-0.2.1/inviz/inviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       89 2023-07-12 08:20:13.000000 inviz-0.2.1/inviz/inviz.egg-info/requires.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-07-12 08:20:13.000000 inviz-0.2.1/inviz/inviz.egg-info/top_level.txt
+-rwxr-xr-x   0 jswen     (1000) jswen     (1000)    10524 2023-07-12 08:18:52.000000 inviz-0.2.1/inviz/inviz.py
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-07-12 08:20:13.456552 inviz-0.2.1/setup.cfg
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1100 2023-07-12 08:18:52.000000 inviz-0.2.1/setup.py
```

### Comparing `inviz-0.2.0/LICENSE` & `inviz-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.2.0/PKG-INFO` & `inviz-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.0
+Version: 0.2.1
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
@@ -12,31 +12,32 @@
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # InViz
 
-InViz (Interactive Visualizer) is a tool for exploratory analysis of high-dimensional datasets where data points from the parameter space are used to calculate to some set of real-world observables. This enables you to easily see how the derived observables change as you traverse the parameter space. If you have pre-computed observables, simply import them alongside the  dataset containing the parameters to start visualizing. Or, write your own function that takes your parameters as inputs, and give it to InViz to compute on the fly!
+InViz (Interactive Visualizer) is a tool for exploratory analysis of high-dimensional datasets where data points from the parameter space are used to calculate some set of real-world observables. This enables you to easily see how the derived observables change as you traverse the parameter space. If you have pre-computed observables, simply import them alongside the  dataset containing the parameters to start visualizing. Or, write your own function that takes your parameters as inputs, and give it to InViz to compute on the fly!
 
 ## Installation
+
+### Dependencies
+- Python versions $\geq$ 3.8 and $<$ 3.11 are supported.
+- Holoviews $\leq$ 1.15.4 (this package and its dependencies will be installed automatically)
+
 InViz can be installed with pip:
 
     python -m pip install inviz
 
 Or, if you want to test the latest changes, you can clone the repository with
     
     git clone https://github.com/wen-jams/inviz
     cd inviz
     python setup.py install
 
-### Dependencies
-- Python versions $\geq$ 3.8 and $<$ 3.11 are supported.
-- Holoviews $\leq$ 1.15.4 (this package and its dependencies will be installed automatically)
-
 ## Getting Started
 
 ### Test Installation
 To verify that inviz and all the dependencies have been installed correctly, open a Jupyter Notebook and run:
 ```python
 import inviz as nv
 ```
```

### Comparing `inviz-0.2.0/README.md` & `inviz-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # InViz
 
-InViz (Interactive Visualizer) is a tool for exploratory analysis of high-dimensional datasets where data points from the parameter space are used to calculate to some set of real-world observables. This enables you to easily see how the derived observables change as you traverse the parameter space. If you have pre-computed observables, simply import them alongside the  dataset containing the parameters to start visualizing. Or, write your own function that takes your parameters as inputs, and give it to InViz to compute on the fly!
+InViz (Interactive Visualizer) is a tool for exploratory analysis of high-dimensional datasets where data points from the parameter space are used to calculate some set of real-world observables. This enables you to easily see how the derived observables change as you traverse the parameter space. If you have pre-computed observables, simply import them alongside the  dataset containing the parameters to start visualizing. Or, write your own function that takes your parameters as inputs, and give it to InViz to compute on the fly!
 
 ## Installation
+
+### Dependencies
+- Python versions $\geq$ 3.8 and $<$ 3.11 are supported.
+- Holoviews $\leq$ 1.15.4 (this package and its dependencies will be installed automatically)
+
 InViz can be installed with pip:
 
     python -m pip install inviz
 
 Or, if you want to test the latest changes, you can clone the repository with
     
     git clone https://github.com/wen-jams/inviz
     cd inviz
     python setup.py install
 
-### Dependencies
-- Python versions $\geq$ 3.8 and $<$ 3.11 are supported.
-- Holoviews $\leq$ 1.15.4 (this package and its dependencies will be installed automatically)
-
 ## Getting Started
 
 ### Test Installation
 To verify that inviz and all the dependencies have been installed correctly, open a Jupyter Notebook and run:
 ```python
 import inviz as nv
 ```
```

### Comparing `inviz-0.2.0/inviz/inviz.egg-info/PKG-INFO` & `inviz-0.2.1/inviz/inviz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.0
+Version: 0.2.1
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
@@ -12,31 +12,32 @@
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # InViz
 
-InViz (Interactive Visualizer) is a tool for exploratory analysis of high-dimensional datasets where data points from the parameter space are used to calculate to some set of real-world observables. This enables you to easily see how the derived observables change as you traverse the parameter space. If you have pre-computed observables, simply import them alongside the  dataset containing the parameters to start visualizing. Or, write your own function that takes your parameters as inputs, and give it to InViz to compute on the fly!
+InViz (Interactive Visualizer) is a tool for exploratory analysis of high-dimensional datasets where data points from the parameter space are used to calculate some set of real-world observables. This enables you to easily see how the derived observables change as you traverse the parameter space. If you have pre-computed observables, simply import them alongside the  dataset containing the parameters to start visualizing. Or, write your own function that takes your parameters as inputs, and give it to InViz to compute on the fly!
 
 ## Installation
+
+### Dependencies
+- Python versions $\geq$ 3.8 and $<$ 3.11 are supported.
+- Holoviews $\leq$ 1.15.4 (this package and its dependencies will be installed automatically)
+
 InViz can be installed with pip:
 
     python -m pip install inviz
 
 Or, if you want to test the latest changes, you can clone the repository with
     
     git clone https://github.com/wen-jams/inviz
     cd inviz
     python setup.py install
 
-### Dependencies
-- Python versions $\geq$ 3.8 and $<$ 3.11 are supported.
-- Holoviews $\leq$ 1.15.4 (this package and its dependencies will be installed automatically)
-
 ## Getting Started
 
 ### Test Installation
 To verify that inviz and all the dependencies have been installed correctly, open a Jupyter Notebook and run:
 ```python
 import inviz as nv
 ```
```

### Comparing `inviz-0.2.0/inviz/inviz.py` & `inviz-0.2.1/inviz/inviz.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,62 +17,67 @@
     
     Parameters
     ----------
     name: string or list of strings
         specifies the display name of the observable for things like plot titles
 
     parameters: dict-like or list of dict-likes
-        the data to associated with that observable. can be python dict (or DataFrame)
-        whose keys (or column names) will be used for things like plot axis labels.
+        the data to associated with that observable. can be python dict (or pandas DataFrame)
+        whose keys (or column names) will be used for things like plot axis labels. 
+
+    latex_labels: dict or list of dicts
+        key: value -> parameter label: latex version. parameter label must match the
+        corresponding one in the parameters dict
 
     myfunc: callable
         a user-provided function that returns parameters. can return more than one
         set of parameters if the "grouped" option is True
 
     myfunc_args: tuple
         arguments for user-provided function
 
     grouped: boolean
         specifies if user-provided function returns more than one set of parameters
 
-    plot_type: string or list of strings
+    plot_type: string
         specifies how the data should be visualized. currently can pick either 'Curve'
         or 'Scatter'
 
     plot_opts: holoviews Options object
         customization options for the observable plot. see Holoviews documentation
-
-    latex_labels: dict
-        key: value -> parameter label: latex version. parameter label must match the
-        corresponding one in the parameters dict
     """
     
     def __init__(
         self, 
         name: str | list[str] = None, 
         parameters: dict | list[dict] = None, 
         myfunc: Callable = None,
         myfunc_args: tuple = None, 
         grouped: bool = False, 
         plot_type: str | list[str] = None,
         plot_opts: type[opts] | list[type[opts]] = None,
         latex_labels: dict = None
     ):
         self.name = [name]
-        self.parameters = [parameters]
+        self.parameters = parameters
+        if parameters is not None:
+            self.parameters = [parameters]
         self.myfunc = myfunc
         self.myfunc_args = myfunc_args
-        self.latex_labels = [latex_labels]
-        self.plot_type = [plot_type]
-        self.plot_opts = [plot_opts]
+        self.plot_type = plot_type
+        if plot_type is not None:
+            self.plot_type = [plot_type]
+        self.plot_opts = plot_opts
+        if plot_opts is not None:
+            self.plot_opts = [plot_opts]
         self.grouped = grouped
+        self.latex_labels = latex_labels
         if self.grouped:
             self.name = name
             self.parameters = parameters
-            self.latex_labels = latex_labels
             self.plot_type = plot_type
             self.plot_opts = plot_opts
         self.number = len(self.name)
     
     def properties(self):
         if self.grouped:
             print("InViz Grouped Observable")
@@ -95,41 +100,48 @@
                 vdim = list(dataset.keys())[1]
                 plot = hv_element(dataset[index], kdim, vdim, label=self.name[i])
             elif computed_data:
                 dataset = computed_data[i]
                 kdim = list(dataset.keys())[0]
                 vdim = list(dataset.keys())[1]
                 plot = hv_element(dataset, kdim, vdim, label=self.name[i])
-            plot.opts(xlabel=lookup_latex_label(kdim, self.latex_labels), ylabel=lookup_latex_label(vdim, self.latex_labels))
-            if self.plot_opts is not None:
+            # set defaults
+            plot.opts(
+                height=400,
+                width=500,
+                fontscale=1.1,
+                xlabel=lookup_latex_label(kdim, self.latex_labels), 
+                ylabel=lookup_latex_label(vdim, self.latex_labels),
+                framewise=True
+            )
+            # add user defined customizations
+            if self.plot_opts and self.plot_opts[i] is not None:
                 plot.opts(self.plot_opts[i])
             self.plots_list.append(plot)
         return self.plots_list
         
-    def draw_plot(self, index, observable_name=None):
-        if observable_name is not None:
-            return 
+    def draw_plot(self, index):
         layout = hv.Layout(self.generate_plot(index))
         return layout.opts(shared_axes=False)
+        
 
-
+#  given a param name, find corresponding latex-formatted param name
 def lookup_latex_label(param, latex_dict):
     try:
         latex_param = latex_dict[param]
         label = r'$${}$$'.format(latex_param)
         return label
     except KeyError:
         label = param
         return label
 
-# Viz in its base form generates a scatter plot with a table that updates based on user's selection on the plot
-# takes the Observable class to create the full visualization
+
 def viz(
-    data: type[pd.DataFrame], 
-    observables: type[Observable]| list[type[Observable]] = None, 
+    data, 
+    observables: list = None, 
     show_observables: bool = True, 
     latex_dict: dict = None
 ):
     # handle default case of no latex paramname dictionary
     if latex_dict is None:
         latex_dict = dict()
     # setting Panel widgets for user interaction
@@ -180,46 +192,52 @@
     
     # function to generate a table of all the selected points
     def make_table(kdim1, kdim2, colordim):
         table_options = opts.Table(height=300, width=1000, hooks=[hook], bgcolor='#f5f5f5')
         table = hv.DynamicMap(lambda index: hv.Table(data.iloc[index], kdims=[kdim1, kdim2, colordim]), streams=[selection])
         return table.opts(table_options).relabel('Selected Points')
     
+    
     # generate the table
     selected_table = pn.bind(make_table, kdim1=var1, kdim2=var2, colordim=cmap_var)
     
     #table_stream = streams.Selection1D(source=selected_table)
     
-    # save plots that have already been generated to save computation time
+    # handles the null selection case and multiple selections
     plots = {}
-    # get plotting options from each observable to be used to generate the empty plots
+    # get total number of plots to draw from list of observables
     plotting_info = {}
     for each in observables:
         for i in range(len(each.name)):
-            plotting_info[each.name[i]] = {'type': each.plot_type[i], 'opts': each.plot_opts[i]}
+            if each.plot_opts is None:
+                specific_opts = None
+            elif each.plot_opts[i] is not None:
+                specific_opts = each.plot_opts[i]
+            plotting_info[each.name[i]] = {'type': each.plot_type[i], 'opts': specific_opts}
     def plot_observables(index):
         if not index:
-            # handle the null selection case by generating empty plots as placeholders
             plots_list = []
             for name in plotting_info:
                 hv_type = getattr(hv, plotting_info[name]['type'])
-                empty_plot = hv_type(np.random.rand(0, 2)).opts(framewise=True)
-                plots_list.append([empty_plot.relabel(f'{name} - No Selection').opts(plotting_info[name]['opts'])])
+                empty_plot = hv_type(np.random.rand(0, 2)).relabel(f'{name} - No Selection').opts(
+                    height=400, 
+                    width=500, 
+                    fontscale=1.1, 
+                    framewise=True)
+                if plotting_info[name]['opts'] is not None:
+                    empty_plot.opts(plotting_info[name]['opts'])
+                plots_list.append([empty_plot])
         else:
-            # holoviews selection1D stream returns an 'index' list object. figure out what indices have not already been selected
             new_index = [x for x in index if x not in list(plots.keys())]
-
-            # generate plots for each index by using the Observable generate_plot method
             for element in new_index:
                 new_plots = []
                 for each in observables:
                     new_plots.extend(each.generate_plot(element))
                 plots[element] = {plot.label: plot for plot in new_plots}
             
-            # create a list containing lists of plots of the same label which will be overlaid
             plots_list = []
             for index_item in index:
                 plot_types = list(plots[index_item].keys())
 
             for plot_item in plot_types:
                 same_type = [plots[key][plot_item] for key in index]
                 plots_list.append(same_type)
@@ -234,8 +252,9 @@
     # put it all together using Panel
     dashboard = pn.Column(pn.Row(var1, var2, cmap_var, cmap_option), pn.Row(points_dmap, selected_table))
     
     if show_observables == True:
         observables_dmap = hv.DynamicMap(plot_observables, streams=[selection]).opts(framewise=True)
         observables_pane = pn.panel(observables_dmap)
         dashboard = pn.Column(dashboard, observables_pane)
+    
     return dashboard
```

### Comparing `inviz-0.2.0/setup.py` & `inviz-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.2.0",
+    version = "0.2.1",
     author = "James Wen",
     author_email = "jswen@usc.edu",
     description = ("An interactive visualizer to help explore high-dimensional data and its observables."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
     py_modules=["inviz"],
```


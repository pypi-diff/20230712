# Comparing `tmp/fusionprov-1.2.2-py3-none-any.whl.zip` & `tmp/fusionprov-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 15861 bytes, number of entries: 10
--rw-r--r--  2.0 unx      794 b- defN 23-Jul-03 12:23 fusionprov/__init__.py
--rw-r--r--  2.0 unx     9390 b- defN 23-Jun-22 10:40 fusionprov/imasprov.py
--rw-r--r--  2.0 unx    20659 b- defN 23-Jul-03 12:11 fusionprov/mastprov.py
--rw-r--r--  2.0 unx      749 b- defN 23-Jun-22 10:40 fusionprov/utilities.py
--rw-r--r--  2.0 unx    11345 b- defN 23-Jul-03 12:28 fusionprov-1.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4927 b- defN 23-Jul-03 12:28 fusionprov-1.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 12:28 fusionprov-1.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       91 b- defN 23-Jul-03 12:28 fusionprov-1.2.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-03 12:28 fusionprov-1.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      816 b- defN 23-Jul-03 12:28 fusionprov-1.2.2.dist-info/RECORD
-10 files, 48874 bytes uncompressed, 14467 bytes compressed:  70.4%
+Zip file size: 16019 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      794 b- defN 23-Jul-12 09:08 fusionprov/__init__.py
+-rw-r--r--  2.0 unx     9390 b- defN 23-Jul-12 09:08 fusionprov/imasprov.py
+-rw-r--r--  2.0 unx    20716 b- defN 23-Jul-12 09:08 fusionprov/mastprov.py
+-rw-r--r--  2.0 unx      749 b- defN 23-Jul-12 09:08 fusionprov/utilities.py
+-rw-r--r--  2.0 unx    11345 b- defN 23-Jul-12 09:18 fusionprov-1.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5008 b- defN 23-Jul-12 09:18 fusionprov-1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 09:18 fusionprov-1.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       91 b- defN 23-Jul-12 09:18 fusionprov-1.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-12 09:18 fusionprov-1.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      816 b- defN 23-Jul-12 09:18 fusionprov-1.3.0.dist-info/RECORD
+10 files, 49012 bytes uncompressed, 14625 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: fusionprov/mastprov.py
 Comment: 
 
 Filename: fusionprov/utilities.py
 Comment: 
 
-Filename: fusionprov-1.2.2.dist-info/LICENSE
+Filename: fusionprov-1.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: fusionprov-1.2.2.dist-info/METADATA
+Filename: fusionprov-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: fusionprov-1.2.2.dist-info/WHEEL
+Filename: fusionprov-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: fusionprov-1.2.2.dist-info/entry_points.txt
+Filename: fusionprov-1.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: fusionprov-1.2.2.dist-info/top_level.txt
+Filename: fusionprov-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fusionprov-1.2.2.dist-info/RECORD
+Filename: fusionprov-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fusionprov/__init__.py

```diff
@@ -15,8 +15,8 @@
 try:
     from .mastprov import write_provenance
 except ModuleNotFoundError as error:
     logging.info(f"{error}. A UDA installation is required write provenance for MAST signals.")
 except ImportError as error:
     logging.info(f"{error}. A UDA installation is required write provenance for MAST signals.")
 
-__version__ = "1.2.2"
+__version__ = "1.3.0"
```

## fusionprov/mastprov.py

```diff
@@ -49,14 +49,16 @@
         self.prov_doc = ProvDocument()
         self.client = pyuda.Client()
         self.client.set_property("get_meta", True)
         self.data = params["data"]
         self.shot = params["shot"]
         self.run = params["run"]
         self.graph = params["graph"]
+        self.xml = params['xml']
+        self.json = params['json']
         self.log_file = None
 
     machine = "MAST"
     namespace_uri = "https://users.mastu.ukaea.uk"
     data_location = "$MAST_DATA"
 
     def get_input_files(self, log_file=None):
@@ -184,38 +186,44 @@
                             scheduler_run_activity,
                             record_shot_activity,
                             scheduler_pass_trigger_agent,
                             signals_done=signals_done,
                         )
             signals_done.append(signal)
 
+    def get_file_name(self):
+        file_name = f"{self.data}_{self.shot}_{self.run}_prov"
+        return file_name
+
     def write_prov(self):
         self.build_prov()
 
-        directories = ("prov-xml", "prov-json", "prov-graph")
-        for directory in directories:
-            if not os.path.exists(directory):
-                os.makedirs(directory)
-
-        file_name = f"{self.data}_{self.shot}_{self.run}_prov"
+        file_name = self.get_file_name()
 
-        json_file = utilities.slugify(file_name) + ".json"
-        xml_file = utilities.slugify(file_name) + ".xml"
-        json_path = os.path.join("prov-json", json_file)
-        xml_path = os.path.join("prov-xml", xml_file)
-        self.prov_doc.serialize(json_path)
-        self.prov_doc.serialize(xml_path, format="xml")
+        if self.json:
+            os.makedirs('prov-json', exist_ok=True)
+            json_file = utilities.slugify(file_name) + ".json"
+            json_path = os.path.join("prov-json", json_file)
+            self.prov_doc.serialize(json_path)
+
+        if self.xml:
+            os.makedirs('prov-xml', exist_ok=True)
+            xml_file = utilities.slugify(file_name) + ".xml"
+            xml_path = os.path.join("prov-xml", xml_file)
+            self.prov_doc.serialize(xml_path, format="xml")
 
         if self.graph:
+            os.makedirs('prov-graph', exist_ok=True)
             dot = prov_to_dot(self.prov_doc)
             graph_file = utilities.slugify(file_name) + ".png"
             graph_path = os.path.join("prov-graph", graph_file)
             dot.write_png(graph_path)
 
 
+
 @MastProvFactory.register_subclass("data_file")
 class MastFileProv(MastProv):
     def __init__(self, params):
         super().__init__(params)
         if self.run is None:
             self.run = self.get_latest_run()
         if FREIA:
@@ -383,14 +391,16 @@
             self.signal_name = self.signal.meta["signal_name"]
         self.file_prov = MastFileProv(
             {
                 "data": self.signal.meta["filename"][:3].decode("utf-8"),
                 "shot": self.shot,
                 "run": self.run,
                 "graph": self.graph,
+                "xml": self.xml,
+                "json": self.json
             }
         )
 
     @staticmethod
     def validate(params) -> bool:
         client = pyuda.Client()
         signal = params["data"]
@@ -438,14 +448,16 @@
         self.prov_doc = ProvDocument()
         self.client = pyuda.Client()
         self.client.set_property("get_meta", True)
         self.data = params["data"]
         self.shot = params["shot"]
         self.run = params["run"]
         self.graph = params["graph"]
+        self.xml = params['xml']
+        self.json = params['json']
         self.ipx = self.client.get_images(
             self.data, self.shot, first_frame=0, last_frame=0
         )
 
     @staticmethod
     def validate(params) -> bool:
         client = pyuda.Client()
@@ -487,48 +499,28 @@
         session_leader_agent = self.prov_doc.agent(
             f"{MastProv.machine}:{session_leader}"
         )
 
         self.prov_doc.wasAssociatedWith(run_shot_activity, session_leader_agent)
         self.prov_doc.used(run_shot_activity, camera_entity)
 
-    def write_prov(self):
-        self.build_prov()
-
-        directories = ("prov-xml", "prov-json", "prov-graph")
-        for directory in directories:
-            if not os.path.exists(directory):
-                os.makedirs(directory)
-
+    def get_file_name(self):
         file_name = f"{self.data}_{self.shot}_prov"
-
-        json_file = utilities.slugify(file_name) + ".json"
-        xml_file = utilities.slugify(file_name) + ".xml"
-        json_path = os.path.join("prov-json", json_file)
-        xml_path = os.path.join("prov-xml", xml_file)
-        self.prov_doc.serialize(json_path)
-        self.prov_doc.serialize(xml_path, format="xml")
-
-        if self.graph:
-            dot = prov_to_dot(self.prov_doc)
-            graph_file = utilities.slugify(file_name) + ".png"
-            graph_path = os.path.join("prov-graph", graph_file)
-            dot.write_png(graph_path)
-
+        return file_name
 
 def parse_params(*args, **kwargs) -> Dict:
     """
     Collates the user-provided parameters into a dictionary of the type that the classes are expecting.
 
     Returns
     -------
     Dict
         A dictionary with keys: data, shot, run and graph.
     """
-    params = {"data": None, "shot": None, "run": None, "graph": False}
+    params = {"data": None, "shot": None, "run": None, "graph": False, 'xml': False, 'json': False}
     if args:
         if len(args) == 1 and isinstance(args[0], Mapping):
             for key, _ in params.items():
                 if key in args[0]:
                     params[key] = args[0][key]
         else:
             args_dict = dict(zip_longest(params, args))
@@ -570,23 +562,43 @@
         nargs="?",
         default=None,
         help="Run number. Will default to the latest run.",
         type=int,
     )
     parser.add_argument("data", help="Data or signal to document provenance for.")
     parser.add_argument(
+        "--xml",
+        "-x",
+        help="Write provenance data in the XML format"
+        "Default: false",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--json",
+        "-j",
+        help="Write provenance data in the JSON format"
+        "Default: false",
+        action="store_true",
+    )
+    parser.add_argument(
         "--graph",
         "-g",
         help="In addition to text formats, write provenance in graph form as .png. "
         "Default: false",
         action="store_true",
     )
+
     args = parser.parse_args()
 
     params = {
         "data": args.data,
         "shot": args.shot,
         "run": args.run,
         "graph": args.graph,
+        "xml": args.xml,
+        "json": args.json
     }
 
     write_provenance(params)
+
+if __name__ == "__main__":
+    main()
```

## Comparing `fusionprov-1.2.2.dist-info/LICENSE` & `fusionprov-1.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fusionprov-1.2.2.dist-info/METADATA` & `fusionprov-1.3.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionprov
-Version: 1.2.2
+Version: 1.3.0
 Summary: A python package for retrieving and documenting the provenance of fusion data.
 Home-page: https://gitlab.com/fair-for-fusion/fusionprov
 Author: Nathan Cummings
 Author-email: nathan.cummings@ukaea.uk
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
@@ -31,21 +31,21 @@
 ------------
 This module provides the `write_provenance()` function that will collate the provenance information for the signal, image data or analysed data file into a W3C-PROV compliant provenance document in json and xml formats. Optionally, it will also output a graphical representation of the provenance as a png.
 
 EXAMPLE:
 ```
 import fusionprov
 
-fusionprov.write_provenance("ip", 30420, graph=True)
+fusionprov.write_provenance("ip", 30420, json=True, xml=True, graph=True)
 ```
 <br/>
 
 The `mastprov` module can also be run from the command line:
 
-```> mastprov 30420 ip --graph```
+```> mastprov 30420 ip --xml --json --graph```
 
 <br/>
 
 Both examples will generate directories in the current working directory for json, xml and png, storing the PROV documents in the relevant location.
 
 <br/>
 
@@ -53,19 +53,19 @@
 
 Provenance documents can also be generated from the level of the data file itself within your Python script or from the command line:
 
 EXAMPLE:
 ```
 import fusionprov
 
-fusionprov.write_provenance("efm", 30420, graph=True)
+fusionprov.write_provenance("efm", 30420, json=True, xml=True, graph=True)
 ```
 or
 
-```> mastprov 30420 efm -g```
+```> mastprov 30420 efm -j -x -g```
 
 <br/>
 
 ### imasprov
 ------------
 This module provides the `ImasProv` class. The class should be instantiated with an IDS (Interface Data Structure) containing the dataset, and optionally the accompanying dataset_descritption/dataset_fair IDSs.
 
@@ -103,15 +103,15 @@
 `pip install fusionprov`
 
 <br/>
 
 DEVELOPERS
 ----------
 ----------
-For those wishing to define further data types and generate provenance documents for them, a Factory Design Pattern is implemented in the `mastprov` module. Write a class for your data type, including a (static) `validate` method and a `write_prov` method. The class should expect parameters as a dictionary with keys, `"data"`, `"shot"`, `"run"` and `"graph"`.
+For those wishing to define further data types and generate provenance documents for them, a Factory Design Pattern is implemented in the `mastprov` module. Write a class for your data type, including a (static) `validate` method and a `write_prov` method. The class should expect parameters as a dictionary with keys, `"data"`, `"shot"`, `"run"`, `"json"`,  `"xml"` and `"graph"`.
 
 Finally, decorate your class with `@MastProvFactory.register_subclass("<data_type>")` replacing `<data_type>` with a label that is not yet in use by the other classes.
 
 EXAMPLE:
 ```
 @MastProvFactory.register_subclass("my_data_type")
 class MyMastDataType:
```

## Comparing `fusionprov-1.2.2.dist-info/RECORD` & `fusionprov-1.3.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-fusionprov/__init__.py,sha256=4MtIBAWUHEZpzzr4frTXRZEC5qoDvznEaH43pKcw5S0,794
+fusionprov/__init__.py,sha256=aoZnsKg1rkeWMPKtKWM1oopvLeCgtSCNNF_NA5e54no,794
 fusionprov/imasprov.py,sha256=zHWNdcn7aSgR5JibUiDaCb95yUN9HmcR8uRXniLI43c,9390
-fusionprov/mastprov.py,sha256=azKhnEJOWAhqindlSuaX-BZ6yUYXJeTM5p_rQLHhCMk,20659
+fusionprov/mastprov.py,sha256=eAjcTaFdZWc-Wearx8DtolXQ9gGMLLIxdpsIwYu_few,20716
 fusionprov/utilities.py,sha256=cq0xU4rErDMSVWc0uBNxboXsMyE84lsz1I20yCGxI5M,749
-fusionprov-1.2.2.dist-info/LICENSE,sha256=nWy-cQl2dVZGb5nuNnCIKy23ToY1xnb0oJ8tUmtrKUc,11345
-fusionprov-1.2.2.dist-info/METADATA,sha256=sHHSsS36aZm9uBbCY5_pKWv3hGPyXLlU2bcignqgK4M,4927
-fusionprov-1.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fusionprov-1.2.2.dist-info/entry_points.txt,sha256=l116zSk3D6w87ZQ2JUvMzY32bp3nYWAqJJExuXlQeZ4,91
-fusionprov-1.2.2.dist-info/top_level.txt,sha256=zUlig65HQFDHJG-3DhxRFEpTQ9g2KthDgSQL89j0bAI,11
-fusionprov-1.2.2.dist-info/RECORD,,
+fusionprov-1.3.0.dist-info/LICENSE,sha256=nWy-cQl2dVZGb5nuNnCIKy23ToY1xnb0oJ8tUmtrKUc,11345
+fusionprov-1.3.0.dist-info/METADATA,sha256=B_ls_L8DV5bOY2md_Z4CVsUe1WNTqZPhYuGwmO8IPfc,5008
+fusionprov-1.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fusionprov-1.3.0.dist-info/entry_points.txt,sha256=l116zSk3D6w87ZQ2JUvMzY32bp3nYWAqJJExuXlQeZ4,91
+fusionprov-1.3.0.dist-info/top_level.txt,sha256=zUlig65HQFDHJG-3DhxRFEpTQ9g2KthDgSQL89j0bAI,11
+fusionprov-1.3.0.dist-info/RECORD,,
```


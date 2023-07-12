# Comparing `tmp/pyceurspt-0.0.4.tar.gz` & `tmp/pyceurspt-0.0.6.tar.gz`

## Comparing `pyceurspt-0.0.4.tar` & `pyceurspt-0.0.6.tar`

### file list

```diff
@@ -1,38 +1,55 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/.pydevproject
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/ceurspt/__init__.py
--rw-r--r--   0        0        0    23416 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/ceurspt/ceurws.py
--rw-r--r--   0        0        0    16059 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/ceurspt/ceurws_base.py
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/ceurspt/spt_cmd.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/ceurspt/version.py
--rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/ceurspt/webserver.py
--rwxr-xr-x   0        0        0     3121 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/scripts/getSamples
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/scripts/install
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/scripts/test
--rw-r--r--   0        0        0    22727 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/static/CEUR-WS-logo-blue.png
--rw-r--r--   0        0        0    17047 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/static/CEUR-WS-logo-xmas.png
--rw-r--r--   0        0        0    21611 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/static/CEUR-WS-logo.png
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/static/cc-by_100x35.png
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/static/ceur-ws.css
--rw-r--r--   0        0        0     9896 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/static/ceurws-bg.png
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/static/icons/32px-DNB.svg.png
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/static/icons/32px-EventIcon.png
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/static/icons/32px-EventSeriesIcon.png
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/static/icons/32px-GROBID-icon.png
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/static/icons/32px-JSON_vector_logo.svg.png
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/static/icons/32px-Scholia_logo.svg.png
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/static/icons/32px-Wikidata_Query_Service_Favicon_wbg.svg.png
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/static/icons/32px-dblp-icon.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/tests/base_spt_test.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/tests/basetest.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/tests/test_app.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/tests/test_ceurws.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/tests/test_json_cache.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/LICENSE
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/README.md
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 pyceurspt-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/.pydevproject
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/ceurspt/__init__.py
+-rw-r--r--   0        0        0     8578 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/ceurspt/bibtex.py
+-rw-r--r--   0        0        0    43361 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/ceurspt/ceurws.py
+-rw-r--r--   0        0        0    16059 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/ceurspt/ceurws_base.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/ceurspt/dataclass_util.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/ceurspt/profiler.py
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/ceurspt/spt_cmd.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/ceurspt/version.py
+-rw-r--r--   0        0        0    10414 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/ceurspt/webserver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/ceurspt/models/__init__.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/ceurspt/models/dblp.py
+-rwxr-xr-x   0        0        0     3210 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/scripts/getSamples
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/scripts/install
+-rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/scripts/refreshCache
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/scripts/test
+-rw-r--r--   0        0        0    22727 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/CEUR-WS-logo-blue.png
+-rw-r--r--   0        0        0    17047 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/CEUR-WS-logo-xmas.png
+-rw-r--r--   0        0        0    21611 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/CEUR-WS-logo.png
+-rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/OpenAccesslogo_200x313.png
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/cc-by_100x35.png
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/ceur-ws.css
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/ceur-ws.ico
+-rw-r--r--   0        0        0     9896 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/ceurws-bg.png
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/favicon.ico
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/icons/32px-Cermine-Icon.png
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/icons/32px-DNB.svg.png
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/icons/32px-EventIcon.png
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/icons/32px-EventSeriesIcon.png
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/icons/32px-GROBID-icon.png
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/icons/32px-JSON_vector_logo.svg.png
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/icons/32px-ORCID-icon.png
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/icons/32px-PDF_icon.svg.png
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/icons/32px-QuickStatements-icon.png
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/icons/32px-SMW-icon.png
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/icons/32px-Scholia_logo.svg.png
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/icons/32px-Wikidata_Query_Service_Favicon_wbg.svg.png
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/icons/32px-dblp-icon.png
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/icons/32px-text-icon.png
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/static/icons/32px-wbjson-icon.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/tests/base_spt_test.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/tests/basetest.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/tests/test_app.py
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/tests/test_bibtex.py
+-rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/tests/test_ceurws.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/tests/test_json_cache.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/README.md
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 pyceurspt-0.0.6/PKG-INFO
```

### Comparing `pyceurspt-0.0.4/.github/workflows/build.yml` & `pyceurspt-0.0.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/.github/workflows/upload-to-pypi.yml` & `pyceurspt-0.0.6/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/ceurspt/ceurws_base.py` & `pyceurspt-0.0.6/ceurspt/ceurws_base.py`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/ceurspt/spt_cmd.py` & `pyceurspt-0.0.6/ceurspt/spt_cmd.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 @author: wf
 """
 from argparse import ArgumentParser, Namespace
 from argparse import RawDescriptionHelpFormatter
 from ceurspt.version import Version
 from ceurspt.webserver import WebServer
+from ceurspt.profiler import Profiler
+from ceurspt.ceurws import JsonCacheManager
 import socket
 import sys
 import traceback
 import webbrowser
 import uvicorn
 from pathlib import Path
 from ceurspt.ceurws import VolumeManager, PaperManager
@@ -36,14 +38,18 @@
         base_url="http://cvb.bitplan.com"
         parser = ArgumentParser(description=description, formatter_class=RawDescriptionHelpFormatter)
         parser.add_argument("-a", "--about", help="show about info [default: %(default)s]", action="store_true")
         parser.add_argument("-b","--basepath",help="the base path to the ceur-ws volumes [default: %(default)s]",default=base_path)
         parser.add_argument("-bu","--baseurl",help="the base url to use for the RESTFul metadata service [default: %(default)s]",default=base_url)
         parser.add_argument("-d", "--debug", dest="debug", action="store_true",
                             help="show debug info [default: %(default)s]")
+        parser.add_argument("-rc","--recreate",action="store_true",help="reload caches e.g. volume table")
+
+        parser.add_argument("-v", "--verbose", action="store_true",
+                            help="show verbose infos e.g. on startup [default: %(default)s]")
         parser.add_argument("--host", default=self.get_default_host(),
                             help="the host to serve / listen from [default: %(default)s]")
         parser.add_argument("--port", type=int, default=9990, help="the port to serve from [default: %(default)s]")
         parser.add_argument("-s", "--serve", action="store_true", help="start webserver [default: %(default)s]")
         parser.add_argument("-V", "--version", action='version', version=version_msg)
         return parser
 
@@ -56,24 +62,40 @@
             str: the hostname
         """
         host = socket.getfqdn()
         # work around https://github.com/python/cpython/issues/79345
         if host == "1.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.ip6.arpa":
             host = "localhost"  # host="127.0.0.1"
         return host
-
+    
+    def recreate(self, args: Namespace):
+        """
+        recreate the caches
+        
+        Args:
+            args(Arguments): command line arguments
+        """
+        jcm=JsonCacheManager(base_url=args.baseurl)
+        for lod_name in ["volumes","papers","proceedings","papers_dblp"]:
+            profiler=Profiler(f"read {lod_name} ...",profile=True)
+            lod=jcm.load_lod(lod_name)    
+            _elapsed=profiler.time(f" read {len(lod)} {lod_name}")
+            jcm.store(lod_name,lod)
+            profiler=Profiler(f"store {lod_name} ...",profile=True)
+            _elapsed=profiler.time(f" store {len(lod)} {lod_name}")
+         
     def start(self, args: Namespace):
         """
         Args:
             args(Arguments): command line arguments
         """
         vm=VolumeManager(base_path=args.basepath,base_url=args.baseurl)
-        vm.getVolumes()
+        vm.getVolumes(args.verbose)
         pm=PaperManager(base_url=args.baseurl)
-        pm.getPapers(vm)
+        pm.getPapers(vm,args.verbose)
         ws = WebServer(vm,pm)
         uvicorn.run(ws.app, host=args.host, port=args.port)
 
 def main(argv=None):  # IGNORE:C0111
     """main program."""
 
     if argv is None:
@@ -92,14 +114,16 @@
         if len(argv) < 1:
             parser.print_usage()
             sys.exit(1)
         if args.about:
             print(program_version_message)
             print(f"see {Version.doc_url}")
             webbrowser.open(Version.doc_url)
+        if args.recreate:
+            spt_cmd.recreate(args)
         elif args.serve:
             spt_cmd.start(args)
 
     except KeyboardInterrupt:
         ###
         # handle keyboard interrupt
         # ###
```

### Comparing `pyceurspt-0.0.4/ceurspt/version.py` & `pyceurspt-0.0.6/ceurspt/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class Version(object):
     """
     Version handling for VolumeBrowser
     """
     name = ""
     version = ceurspt.__version__
     date = '2023-03-17'
-    updated = '2023-03-17'
+    updated = '2023-07-12'
     description = 'CEUR-WS Single Point of Truth RestFUL server',
 
     authors = 'Tim Holzheim, Wolfgang Fahl'
 
     doc_url = "https://github.com/ceurws/ceur-spt"
     chat_url = "https://github.com/ceurws/ceur-spt/discussions"
     cm_url = "https://github.com/ceurws/ceur-spt"
```

### Comparing `pyceurspt-0.0.4/scripts/getSamples` & `pyceurspt-0.0.6/scripts/getSamples`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 #
 # show the usage
 #
 usage() {
   echo "usage: $0 [-h|--help][--ceurws]"
   echo "  -h|--help: show this usage"
   echo "  -p|--papers: mine paper details"
+  echo "  -t|--text: extract text from papers"
+  echo "  -v|--volume: set volume number"
   echo "  --ceurws: force getting samples for CEURWS and exit"
 }
 
 #
 # volume dir
 #
 # params
```

### Comparing `pyceurspt-0.0.4/static/CEUR-WS-logo-blue.png` & `pyceurspt-0.0.6/static/CEUR-WS-logo-blue.png`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/static/CEUR-WS-logo-xmas.png` & `pyceurspt-0.0.6/static/CEUR-WS-logo-xmas.png`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/static/CEUR-WS-logo.png` & `pyceurspt-0.0.6/static/CEUR-WS-logo.png`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/static/cc-by_100x35.png` & `pyceurspt-0.0.6/static/cc-by_100x35.png`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/static/ceur-ws.css` & `pyceurspt-0.0.6/static/ceur-ws.css`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/static/ceurws-bg.png` & `pyceurspt-0.0.6/static/ceurws-bg.png`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/static/icons/32px-DNB.svg.png` & `pyceurspt-0.0.6/static/icons/32px-DNB.svg.png`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/static/icons/32px-EventIcon.png` & `pyceurspt-0.0.6/static/icons/32px-EventIcon.png`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/static/icons/32px-EventSeriesIcon.png` & `pyceurspt-0.0.6/static/icons/32px-EventSeriesIcon.png`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/static/icons/32px-GROBID-icon.png` & `pyceurspt-0.0.6/static/icons/32px-GROBID-icon.png`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/static/icons/32px-JSON_vector_logo.svg.png` & `pyceurspt-0.0.6/static/icons/32px-JSON_vector_logo.svg.png`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/static/icons/32px-Scholia_logo.svg.png` & `pyceurspt-0.0.6/static/icons/32px-Scholia_logo.svg.png`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/static/icons/32px-Wikidata_Query_Service_Favicon_wbg.svg.png` & `pyceurspt-0.0.6/static/icons/32px-Wikidata_Query_Service_Favicon_wbg.svg.png`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/static/icons/32px-dblp-icon.png` & `pyceurspt-0.0.6/static/icons/32px-dblp-icon.png`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/tests/base_spt_test.py` & `pyceurspt-0.0.6/tests/base_spt_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-'''
+"""
 Created on 2023-03-23
 
 @author: wf
-'''
+"""
 from tests.basetest import Basetest
 from ceurspt.ceurws import VolumeManager, PaperManager
 from pathlib import Path
 
+
 class BaseSptTest(Basetest):
     """
     Basetest for Single Point of Truth
     """
     
     def setUp(self, debug=False, profile=True):
         """
         prepare the test environment
         """
         Basetest.setUp(self, debug=debug, profile=profile)
-        self.script_path=Path(__file__)
-        self.base_path=f"{self.script_path.parent.parent}/ceur-ws"
-        self.base_url="http://cvb.bitplan.com"
-        self.vm=VolumeManager(base_path=self.base_path,base_url=self.base_url)
+        self.script_path = Path(__file__)
+        self.base_path = f"{self.script_path.parent.parent}/ceur-ws"
+        self.base_url = "http://cvb.bitplan.com"
+        self.vm = VolumeManager(base_path=self.base_path, base_url=self.base_url)
         self.vm.getVolumes()
-        self.pm=PaperManager(base_url=self.base_url)
+        self.pm = PaperManager(base_url=self.base_url)
         self.pm.getPapers(self.vm)
```

### Comparing `pyceurspt-0.0.4/tests/basetest.py` & `pyceurspt-0.0.6/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/tests/test_app.py` & `pyceurspt-0.0.6/tests/test_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,24 @@
         """
         response = self.client.get("/")
         self.assertEqual(404, response.status_code)
         debug=self.debug
         debug=True
         if debug:
             print(response.text)
+            
+    def test_index(self):
+        """
+        test the index html file
+        """
+        response=self.checkResponse("/index.html", 200)
+        html=response.text
+        debug=True
+        if debug:
+            print(html)
     
     def test_read_volume(self):
         """
         test reading a volume
         """
        
         debug=self.debug
```

### Comparing `pyceurspt-0.0.4/tests/test_json_cache.py` & `pyceurspt-0.0.6/tests/test_json_cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     
     @unittest.skipIf(True,"only manual")
     def test_json_cache(self):
         """
         test reading list of dicts 
         """
         jcm=JsonCacheManager()
-        for lod_name in ["volumes","papers","proceedings"]:
+        for lod_name in ["volumes","papers","proceedings","papers_dblp"]:
             profiler=Profiler(f"read {lod_name}")
             lod=jcm.load_lod(lod_name)    
             elapsed=profiler.time()
             print(f"read {len(lod)} {lod_name} in {elapsed:5.1f} s")
             jcm.store(lod_name,lod)
             profiler=Profiler(f"store {lod_name}")
             elapsed=profiler.time()
```

### Comparing `pyceurspt-0.0.4/.gitignore` & `pyceurspt-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/LICENSE` & `pyceurspt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyceurspt-0.0.4/README.md` & `pyceurspt-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,10 +15,11 @@
 Free Open-Access Proceedings for Computer Science Workshops
 https://ceur-ws.org/
 ### Semantification of CEUR-WS
 - http://ceur-ws-browser.bitplan.com
 - http://ceur-ws.bitplan.com
 
 ### Single Point of Truth
+- http://ceurspt.wikidata.dbis.rwth-aachen.de/index.html
 - http://ceurspt.wikidata.dbis.rwth-aachen.de/docs
```

### Comparing `pyceurspt-0.0.4/pyproject.toml` & `pyceurspt-0.0.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,21 @@
   # https://pypi.org/project/fastapi/
   "fastapi[all]",
   # https://pypi.org/project/uvicorn/
   "uvicorn",
   # https://pypi.org/project/linkml-runtime/
   "linkml-runtime",
   # https://pypi.org/project/beautifulsoup4/
-  "beautifulsoup4"
+  "beautifulsoup4",
+  # https://github.com/tqdm/tqdm
+  # optional?
+  "tqdm",
+  # https://github.com/ijl/orjson
+  'orjson>=3.8.9',
+    "bibtexparser"
 ]
 
 requires-python = ">=3.8"
 classifiers=[
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `pyceurspt-0.0.4/PKG-INFO` & `pyceurspt-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCEURspt
-Version: 0.0.4
+Version: 0.0.6
 Project-URL: Home, https://github.com/ceurws/ceur-spt
 Project-URL: Documentation, https://github.com/ceurws/ceur-spt
 Project-URL: Source, https://github.com/ceurws/ceur-spt
 Author-email: Tim Holzheim <tim.holzheim@rwth-aachen.de>, Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>, Tim Holzheim <tim.holzheim@rwth-aachen.de>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -19,16 +19,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: beautifulsoup4
+Requires-Dist: bibtexparser
 Requires-Dist: fastapi[all]
 Requires-Dist: linkml-runtime
+Requires-Dist: orjson>=3.8.9
+Requires-Dist: tqdm
 Requires-Dist: uvicorn
 Provides-Extra: test
 Requires-Dist: green; extra == 'test'
 Description-Content-Type: text/markdown
 
 # ceur-spt
 RESTFul Single Point of Truth Server for CEUR-WS
@@ -47,10 +50,11 @@
 Free Open-Access Proceedings for Computer Science Workshops
 https://ceur-ws.org/
 ### Semantification of CEUR-WS
 - http://ceur-ws-browser.bitplan.com
 - http://ceur-ws.bitplan.com
 
 ### Single Point of Truth
+- http://ceurspt.wikidata.dbis.rwth-aachen.de/index.html
 - http://ceurspt.wikidata.dbis.rwth-aachen.de/docs
```


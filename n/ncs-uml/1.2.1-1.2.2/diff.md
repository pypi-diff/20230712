# Comparing `tmp/ncs-uml-1.2.1.tar.gz` & `tmp/ncs-uml-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncs-uml-1.2.1.tar", last modified: Mon Jul 10 20:14:16 2023, max compression
+gzip compressed data, was "ncs-uml-1.2.2.tar", last modified: Tue Jul 11 23:02:40 2023, max compression
```

## Comparing `ncs-uml-1.2.1.tar` & `ncs-uml-1.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-10 20:14:16.040436 ncs-uml-1.2.1/
--rw-r--r--   0 kkotari    (501) staff       (20)    11370 2023-06-23 13:28:47.000000 ncs-uml-1.2.1/LICENSE
--rw-r--r--   0 kkotari    (501) staff       (20)       58 2023-07-09 04:23:25.000000 ncs-uml-1.2.1/MANIFEST.in
--rw-r--r--   0 kkotari    (501) staff       (20)    15652 2023-07-10 20:14:16.040256 ncs-uml-1.2.1/PKG-INFO
--rw-r--r--   0 kkotari    (501) staff       (20)    14651 2023-07-09 04:49:56.000000 ncs-uml-1.2.1/README.md
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-10 20:14:16.038224 ncs-uml-1.2.1/ncs_uml/
--rw-r--r--   0 kkotari    (501) staff       (20)      253 2023-07-10 19:47:27.000000 ncs-uml-1.2.1/ncs_uml/__init__.py
--rw-r--r--   0 kkotari    (501) staff       (20)     5258 2023-07-10 20:09:01.000000 ncs-uml-1.2.1/ncs_uml/main.py
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-10 20:14:16.039392 ncs-uml-1.2.1/ncs_uml/plugins/
--rw-r--r--   0 kkotari    (501) staff       (20)        0 2023-07-10 19:04:44.000000 ncs-uml-1.2.1/ncs_uml/plugins/__init__.py
--rw-r--r--   0 kkotari    (501) staff       (20)    45628 2023-07-10 19:45:13.000000 ncs-uml-1.2.1/ncs_uml/plugins/uml_patch.py
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-10 20:14:16.040046 ncs-uml-1.2.1/ncs_uml/scripts/
--rw-r--r--   0 kkotari    (501) staff       (20)        0 2023-07-07 21:00:13.000000 ncs-uml-1.2.1/ncs_uml/scripts/__init__.py
--rw-r--r--   0 kkotari    (501) staff       (20)     2985 2023-07-10 19:52:41.000000 ncs-uml-1.2.1/ncs_uml/scripts/run.py
--rw-r--r--   0 kkotari    (501) staff       (20)     6206 2023-07-09 04:21:24.000000 ncs-uml-1.2.1/ncs_uml/utils.py
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-10 20:14:16.039120 ncs-uml-1.2.1/ncs_uml.egg-info/
--rw-r--r--   0 kkotari    (501) staff       (20)    15652 2023-07-10 20:14:15.000000 ncs-uml-1.2.1/ncs_uml.egg-info/PKG-INFO
--rw-r--r--   0 kkotari    (501) staff       (20)      404 2023-07-10 20:14:15.000000 ncs-uml-1.2.1/ncs_uml.egg-info/SOURCES.txt
--rw-r--r--   0 kkotari    (501) staff       (20)        1 2023-07-10 20:14:15.000000 ncs-uml-1.2.1/ncs_uml.egg-info/dependency_links.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       87 2023-07-10 20:14:15.000000 ncs-uml-1.2.1/ncs_uml.egg-info/entry_points.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-07-10 20:14:15.000000 ncs-uml-1.2.1/ncs_uml.egg-info/requires.txt
--rw-r--r--   0 kkotari    (501) staff       (20)        8 2023-07-10 20:14:15.000000 ncs-uml-1.2.1/ncs_uml.egg-info/top_level.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-24 00:36:25.000000 ncs-uml-1.2.1/requirements.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       38 2023-07-10 20:14:16.040490 ncs-uml-1.2.1/setup.cfg
--rw-r--r--   0 kkotari    (501) staff       (20)     1699 2023-07-10 15:28:57.000000 ncs-uml-1.2.1/setup.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-11 23:02:40.794175 ncs-uml-1.2.2/
+-rw-r--r--   0 kkotari    (501) staff       (20)    11370 2023-06-23 13:28:47.000000 ncs-uml-1.2.2/LICENSE
+-rw-r--r--   0 kkotari    (501) staff       (20)       58 2023-07-09 04:23:25.000000 ncs-uml-1.2.2/MANIFEST.in
+-rw-r--r--   0 kkotari    (501) staff       (20)    15766 2023-07-11 23:02:40.793980 ncs-uml-1.2.2/PKG-INFO
+-rw-r--r--   0 kkotari    (501) staff       (20)    14765 2023-07-11 22:34:53.000000 ncs-uml-1.2.2/README.md
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-11 23:02:40.791587 ncs-uml-1.2.2/ncs_uml/
+-rw-r--r--   0 kkotari    (501) staff       (20)      253 2023-07-11 22:30:48.000000 ncs-uml-1.2.2/ncs_uml/__init__.py
+-rw-r--r--   0 kkotari    (501) staff       (20)     5296 2023-07-11 23:00:13.000000 ncs-uml-1.2.2/ncs_uml/main.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-11 23:02:40.792968 ncs-uml-1.2.2/ncs_uml/plugins/
+-rw-r--r--   0 kkotari    (501) staff       (20)        0 2023-07-10 19:04:44.000000 ncs-uml-1.2.2/ncs_uml/plugins/__init__.py
+-rw-r--r--   0 kkotari    (501) staff       (20)    45889 2023-07-11 23:00:56.000000 ncs-uml-1.2.2/ncs_uml/plugins/uml_patch.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-11 23:02:40.793652 ncs-uml-1.2.2/ncs_uml/scripts/
+-rw-r--r--   0 kkotari    (501) staff       (20)        0 2023-07-07 21:00:13.000000 ncs-uml-1.2.2/ncs_uml/scripts/__init__.py
+-rw-r--r--   0 kkotari    (501) staff       (20)     2820 2023-07-11 23:00:34.000000 ncs-uml-1.2.2/ncs_uml/scripts/run.py
+-rw-r--r--   0 kkotari    (501) staff       (20)     6206 2023-07-09 04:21:24.000000 ncs-uml-1.2.2/ncs_uml/utils.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-11 23:02:40.792645 ncs-uml-1.2.2/ncs_uml.egg-info/
+-rw-r--r--   0 kkotari    (501) staff       (20)    15766 2023-07-11 23:02:40.000000 ncs-uml-1.2.2/ncs_uml.egg-info/PKG-INFO
+-rw-r--r--   0 kkotari    (501) staff       (20)      404 2023-07-11 23:02:40.000000 ncs-uml-1.2.2/ncs_uml.egg-info/SOURCES.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)        1 2023-07-11 23:02:40.000000 ncs-uml-1.2.2/ncs_uml.egg-info/dependency_links.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       87 2023-07-11 23:02:40.000000 ncs-uml-1.2.2/ncs_uml.egg-info/entry_points.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-07-11 23:02:40.000000 ncs-uml-1.2.2/ncs_uml.egg-info/requires.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)        8 2023-07-11 23:02:40.000000 ncs-uml-1.2.2/ncs_uml.egg-info/top_level.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-24 00:36:25.000000 ncs-uml-1.2.2/requirements.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       38 2023-07-11 23:02:40.794230 ncs-uml-1.2.2/setup.cfg
+-rw-r--r--   0 kkotari    (501) staff       (20)     1699 2023-07-10 15:28:57.000000 ncs-uml-1.2.2/setup.py
```

### Comparing `ncs-uml-1.2.1/LICENSE` & `ncs-uml-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ncs-uml-1.2.1/PKG-INFO` & `ncs-uml-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncs-uml
-Version: 1.2.1
+Version: 1.2.2
 Summary: The ncs-uml creates plantUML files for the given YANG file and its dependencies
 Home-page: https://github.com/kirankotari/ncs-uml.git
 Author: Kiran Kumar Kotari
 Author-email: kirankotari@live.com
 License: UNKNOWN
 Keywords: ncs-uml,ncs_uml
 Platform: UNKNOWN
@@ -53,31 +53,32 @@
 Creates plantUML file for the YANG module in <filename>, and all its dependencies.
 It can be converted into PNG/SVG images using www.plantuml.com or with editor plugins.
 
 Options:
   -h, --help            Show this help message and exit
   -v, --version         Show version number and exit
   -V, --verbose
-  --skip=SKIP           skip given yang modules
-  --skip-grouping
-  --dpath=DPATH         dependent yang module paths
-  --skip-module=SKIP MODULE
-                        skips given modules, i.e., --skip-module=tailf-ncs
+  --no-inline-groupings
+  --dependent-yang-paths=DEPENDENT_YANG_PATHS
+                        dependent yang module paths
+  --no-inline-groupings-from=NO_INLINE_GROUPINGS_FROM
+                        Skips given modules from inline groupings.  Example
+                        --uml-no-inline-groupings-from=ietf-yang-push
   --add-legend          Adds legend about grouping yang file in the UML
 ```
 
 ## Docs
 
 **How to use ncs-uml?**
 
 - Command Line  
   Type `ncs-uml <YangFile>`. For more help type `ncs-uml --help`
 
 ```shell
-user$ ncs-uml $NCS_DIR/examples.ncs/getting-started/developing-with-ncs/17-mpls-vpn-python/packages/l3vpn/src/yang/l3vpn.yang --skip-module=tailf-ncs --add-legend
+user$ ncs-uml $NCS_DIR/examples.ncs/getting-started/developing-with-ncs/17-mpls-vpn-python/packages/l3vpn/src/yang/l3vpn.yang --no-inline-groupings-from=tailf-ncs --add-legend
  INFO |   main | uml file: l3vpn.uml
  INFO |   main | uml clean up done.
 user$
 ```
 
 It returns plantUML code, which can easily converted to image.
```

### Comparing `ncs-uml-1.2.1/README.md` & `ncs-uml-1.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,31 +28,32 @@
 Creates plantUML file for the YANG module in <filename>, and all its dependencies.
 It can be converted into PNG/SVG images using www.plantuml.com or with editor plugins.
 
 Options:
   -h, --help            Show this help message and exit
   -v, --version         Show version number and exit
   -V, --verbose
-  --skip=SKIP           skip given yang modules
-  --skip-grouping
-  --dpath=DPATH         dependent yang module paths
-  --skip-module=SKIP MODULE
-                        skips given modules, i.e., --skip-module=tailf-ncs
+  --no-inline-groupings
+  --dependent-yang-paths=DEPENDENT_YANG_PATHS
+                        dependent yang module paths
+  --no-inline-groupings-from=NO_INLINE_GROUPINGS_FROM
+                        Skips given modules from inline groupings.  Example
+                        --uml-no-inline-groupings-from=ietf-yang-push
   --add-legend          Adds legend about grouping yang file in the UML
 ```
 
 ## Docs
 
 **How to use ncs-uml?**
 
 - Command Line  
   Type `ncs-uml <YangFile>`. For more help type `ncs-uml --help`
 
 ```shell
-user$ ncs-uml $NCS_DIR/examples.ncs/getting-started/developing-with-ncs/17-mpls-vpn-python/packages/l3vpn/src/yang/l3vpn.yang --skip-module=tailf-ncs --add-legend
+user$ ncs-uml $NCS_DIR/examples.ncs/getting-started/developing-with-ncs/17-mpls-vpn-python/packages/l3vpn/src/yang/l3vpn.yang --no-inline-groupings-from=tailf-ncs --add-legend
  INFO |   main | uml file: l3vpn.uml
  INFO |   main | uml clean up done.
 user$
 ```
 
 It returns plantUML code, which can easily converted to image.
```

### Comparing `ncs-uml-1.2.1/ncs_uml/main.py` & `ncs-uml-1.2.2/ncs_uml/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 class NcsUml(metaclass=Singleton):
     name = 'ncs-yang'
     ncs_uml = "/tmp/.ncs_uml"
 
     command = []
     ncs_path = None
-    skip_uses = False
 
     def __init__(self, opt, *args, **kwargs):
         self.path = getcwd()
         self.util = Utils(**kwargs)
 
         self.log = self.util.log
         self.opt = opt
@@ -91,15 +90,15 @@
             if Path(each).exists() == False:
                 msg = f"mandatory files are missing: {paths}"
                 raise FileNotFoundError(msg)
         return pyang_path
 
     def generate(self, yf):
         self.create_workdir()
-        self.copy([self.get_ncs_path()] + self.opt.dpath)
+        self.copy([self.get_ncs_path()] + self.opt.dependent_yang_paths)
         cmd = self.get_pyang()
 
         if not self.util.file.is_file(yf):
             msg = f"could not find yang file {yf} in {self.path}"
             raise FileNotFoundError(msg)
 
         self.log.debug("file {file} exists, fetching dependencies")
@@ -108,18 +107,18 @@
         self.generate_umlfile(cmd, file)
 
     def generate_umlfile(self, cmd, file):
         path = Path(__file__).absolute().parent.as_posix()
         uml_file = f"{file.stem}.uml"
         cmd += f" --plugindir={path}/plugins/ -f uml {file} --path={self.ncs_uml}"
         cmd += f" --uml-no=module,import,annotation"
-        if not self.opt.skip_grouping:
+        if not self.opt.no_inline_groupings:
             cmd += f" --uml-inline-groupings "
-        if getattr(self.opt, 'skip_module', False):
-            cmd += f"--uml-skip-module={','.join(self.opt.skip_module)} "
+        if getattr(self.opt, 'no_inline_groupings_from', False):
+            cmd += f"--uml-no-inline-groupings-from={','.join(self.opt.no_inline_groupings_from)} "
         if getattr(self.opt, 'add_legend', False):
             cmd += f"--uml-add-legend "
         cmd += f" --uml-output-directory=. 1> {uml_file} 2> /dev/null"
         self.log.debug(f"command: {cmd}")
         self.util.cmd.call(cmd)
         self.log.info(f"uml file: {uml_file}")
```

### Comparing `ncs-uml-1.2.1/ncs_uml/plugins/uml_patch.py` & `ncs-uml-1.2.2/ncs_uml/plugins/uml_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,34 +25,44 @@
 from pyang import util
 from pyang.error import err_add
 
 
 def pyang_plugin_init():
     plugin.register_plugin(UMLPatchPlugin())
 
+
 class UMLPatchPlugin(plugin.PyangPlugin):
     def add_opts(self, optparser):
-        optlist = [
-            optparse.make_option("--uml-skip-module",
-                                 dest="uml_skip_module",
+        opt1 = [
+            optparse.make_option("--uml-no-inline-groupings-from",
+                                 dest="uml_no_inline_groupings_from",
                                  action="append",
                                  default=[],
-                                 metavar="SKIP MODULE",
-                                 help="skips given modules, i.e., --uml-skip-module=tailf-ncs"),
+                                 help="Skips given modules from inline groupings. \nExample --uml-no-inline-groupings-from=ietf-yang-push")
+        ]
+        opt2 =[
             optparse.make_option("--uml-add-legend",
                                  dest="uml_add_legend",
                                  action="store_true",
                                  help="Adds legend about grouping yang file in the UML"),
             ]
+
         if hasattr(optparser, 'uml_opts'):
             g = optparser.uml_opts
         else:
             g = optparser.add_option_group("UML specific options")
             optparser.uml_opts = g
-        g.add_options(optlist)
+        try:
+            g.add_options(opt1)
+        except optparse.OptionConflictError:
+            pass
+        try:
+            g.add_options(opt2)
+        except optparse.OptionConflictError:
+            pass
 
     def add_output_format(self, fmts):
         self.multiple_modules = True
         fmts['uml'] = self
 
     def pre_validate(self, ctx, modules):
         module = modules[0]
@@ -134,15 +144,15 @@
         if ctx.opts.uml_pages_layout is not None:
             self.ctx_pagelayout = ctx.opts.uml_pages_layout
 
         # Title from option -t
         self.ctx_title = ctx.opts.uml_title
 
         self.ctx_inline_augments = ctx.opts.uml_inline_augments
-        self.ctx_skip_module = set(ctx.opts.uml_skip_module)
+        self.ctx_no_inline_groupings_from = set(ctx.opts.uml_no_inline_groupings_from)
         self.ctx_add_legend = ctx.opts.uml_add_legend
 
         no = ctx.opts.uml_no.split(",")
         self.ctx_leafrefs = not "leafref" in no
         self.ctx_uses = not "uses" in no
         self.ctx_annotations = not "annotation" in no
         self.ctx_identityrefs = not "identityref" in no
@@ -367,15 +377,15 @@
             if not self._ctx.opts.uml_inline:
                 self.emit_uses(parent, node)
             if hasattr(node, 'i_grouping') and (self._ctx.opts.uml_inline) and cont:
                 grouping_node = node.i_grouping
                 if grouping_node is not None:
                     # skip grouping modules if given
                     module = str(grouping_node.main_module()).split()[-1]
-                    if module in self.ctx_skip_module:
+                    if module in self.ctx_no_inline_groupings_from:
                         fd.write('%s : %s {uses} \n' %(self.full_path(parent), node.arg))
                         return
                     # inline grouping here
                     # collecting grouping module file names
                     self.ctx_grp_files.add(str(grouping_node.pos).split(':')[0].split('/')[-1])
                     # sys.stderr.write('Found  target grouping to inline %s %s \n' %(grouping_node.keyword, grouping_node.arg))
                     for children in grouping_node.substmts:
@@ -1058,8 +1068,8 @@
 
         if not self.ctx_no_module:
             fd.write("} \n\n")
             if self.ctx_imports:
                 imports = module.search('import')
                 for i in imports:
                     mod = self.make_plantuml_keyword(i.search_one('prefix').arg) + '_' + self.make_plantuml_keyword(i.arg)
-                    fd.write('%s +-- %s_%s\n' %(mod,self.make_plantuml_keyword(self.thismod_prefix), self.make_plantuml_keyword(module.arg)))
+                    fd.write('%s +-- %s_%s\n' %(mod,self.make_plantuml_keyword(self.thismod_prefix), self.make_plantuml_keyword(module.arg)))
```

### Comparing `ncs-uml-1.2.1/ncs_uml/scripts/run.py` & `ncs-uml-1.2.2/ncs_uml/scripts/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 import ncs_uml
 from ncs_uml.main import NcsUml
 from ncs_uml.utils import Command
 
 
 def get_pyang_addons():
     addl_opt = [
-        optparse.make_option("--skip-module",
-                             dest="skip_module",
+        optparse.make_option("--no-inline-groupings-from",
+                             dest="no_inline_groupings_from",
                              action="append",
                              default=[],
-                             metavar="SKIP MODULE",
-                             help="skips given modules, i.e., --skip-module=tailf-ncs"),
+                             help="Skips given modules from inline groupings. \nExample --uml-no-inline-groupings-from=ietf-yang-push"),
         optparse.make_option("--add-legend",
                              dest="add_legend",
                              action="store_true",
                              help="Adds legend about grouping yang file in the UML"),
     ]
     return addl_opt
 
@@ -35,24 +34,19 @@
                              action="help",
                              help="Show this help message and exit"),
         optparse.make_option("-v", "--version",
                              action="version",
                              help="Show version number and exit"),
         optparse.make_option("-V", "--verbose",
                              action="store_true"),
-        optparse.make_option("--skip",
-                             dest="skip",
-                             default=[],
-                             action="append",
-                             help="skip given yang modules"),
-        optparse.make_option("--skip-grouping",
-                             dest="skip_grouping",
+        optparse.make_option("--no-inline-groupings",
+                             dest="no_inline_groupings",
                              action="store_true"),
-        optparse.make_option("--dpath",
-                             dest="dpath",
+        optparse.make_option("--dependent-yang-paths",
+                             dest="dependent_yang_paths",
                              default=[],
                              action="append",
                              help="dependent yang module paths"),
     ]
     optparser = optparse.OptionParser(usage, add_help_option = False)
     optparser.version = f'{ncs_uml.__name__} {ncs_uml.__version__}'
     optlist += get_pyang_addons()
@@ -79,7 +73,8 @@
         uml.util.exit
 
     if 'yang' not in args[0]:
         uml.log.error("invalid yang file given\n")
         uml.util.exit
 
     uml.generate(args[0])
+
```

### Comparing `ncs-uml-1.2.1/ncs_uml/utils.py` & `ncs-uml-1.2.2/ncs_uml/utils.py`

 * *Files identical despite different names*

### Comparing `ncs-uml-1.2.1/ncs_uml.egg-info/PKG-INFO` & `ncs-uml-1.2.2/ncs_uml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncs-uml
-Version: 1.2.1
+Version: 1.2.2
 Summary: The ncs-uml creates plantUML files for the given YANG file and its dependencies
 Home-page: https://github.com/kirankotari/ncs-uml.git
 Author: Kiran Kumar Kotari
 Author-email: kirankotari@live.com
 License: UNKNOWN
 Keywords: ncs-uml,ncs_uml
 Platform: UNKNOWN
@@ -53,31 +53,32 @@
 Creates plantUML file for the YANG module in <filename>, and all its dependencies.
 It can be converted into PNG/SVG images using www.plantuml.com or with editor plugins.
 
 Options:
   -h, --help            Show this help message and exit
   -v, --version         Show version number and exit
   -V, --verbose
-  --skip=SKIP           skip given yang modules
-  --skip-grouping
-  --dpath=DPATH         dependent yang module paths
-  --skip-module=SKIP MODULE
-                        skips given modules, i.e., --skip-module=tailf-ncs
+  --no-inline-groupings
+  --dependent-yang-paths=DEPENDENT_YANG_PATHS
+                        dependent yang module paths
+  --no-inline-groupings-from=NO_INLINE_GROUPINGS_FROM
+                        Skips given modules from inline groupings.  Example
+                        --uml-no-inline-groupings-from=ietf-yang-push
   --add-legend          Adds legend about grouping yang file in the UML
 ```
 
 ## Docs
 
 **How to use ncs-uml?**
 
 - Command Line  
   Type `ncs-uml <YangFile>`. For more help type `ncs-uml --help`
 
 ```shell
-user$ ncs-uml $NCS_DIR/examples.ncs/getting-started/developing-with-ncs/17-mpls-vpn-python/packages/l3vpn/src/yang/l3vpn.yang --skip-module=tailf-ncs --add-legend
+user$ ncs-uml $NCS_DIR/examples.ncs/getting-started/developing-with-ncs/17-mpls-vpn-python/packages/l3vpn/src/yang/l3vpn.yang --no-inline-groupings-from=tailf-ncs --add-legend
  INFO |   main | uml file: l3vpn.uml
  INFO |   main | uml clean up done.
 user$
 ```
 
 It returns plantUML code, which can easily converted to image.
```

### Comparing `ncs-uml-1.2.1/setup.py` & `ncs-uml-1.2.2/setup.py`

 * *Files identical despite different names*


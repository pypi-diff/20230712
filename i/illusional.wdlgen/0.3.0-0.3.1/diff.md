# Comparing `tmp/illusional.wdlgen-0.3.0.tar.gz` & `tmp/illusional.wdlgen-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/illusional.wdlgen-0.3.0.tar", last modified: Mon Jul 13 02:37:15 2020, max compression
+gzip compressed data, was "illusional.wdlgen-0.3.1.tar", last modified: Wed Jul 12 21:46:41 2023, max compression
```

## Comparing `illusional.wdlgen-0.3.0.tar` & `illusional.wdlgen-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,30 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-13 02:37:15.000000 illusional.wdlgen-0.3.0/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-13 02:37:15.000000 illusional.wdlgen-0.3.0/wdlgen/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3271 2020-07-13 02:36:57.000000 illusional.wdlgen-0.3.0/wdlgen/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10580 2020-07-13 02:36:57.000000 illusional.wdlgen-0.3.0/wdlgen/task.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3339 2020-07-13 02:36:57.000000 illusional.wdlgen-0.3.0/wdlgen/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3788 2020-07-13 02:36:57.000000 illusional.wdlgen-0.3.0/wdlgen/workflow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5738 2020-07-13 02:36:57.000000 illusional.wdlgen-0.3.0/wdlgen/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2756 2020-07-13 02:36:57.000000 illusional.wdlgen-0.3.0/wdlgen/workflowcall.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      115 2020-07-13 02:36:57.000000 illusional.wdlgen-0.3.0/wdlgen/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11017 2020-07-13 02:37:15.000000 illusional.wdlgen-0.3.0/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-13 02:37:15.000000 illusional.wdlgen-0.3.0/illusional.wdlgen.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11017 2020-07-13 02:37:15.000000 illusional.wdlgen-0.3.0/illusional.wdlgen.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-13 02:37:15.000000 illusional.wdlgen-0.3.0/illusional.wdlgen.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2020-07-13 02:37:15.000000 illusional.wdlgen-0.3.0/illusional.wdlgen.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-13 02:37:15.000000 illusional.wdlgen-0.3.0/illusional.wdlgen.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      346 2020-07-13 02:37:15.000000 illusional.wdlgen-0.3.0/illusional.wdlgen.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     8664 2020-07-13 02:36:57.000000 illusional.wdlgen-0.3.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-07-13 02:37:15.000000 illusional.wdlgen-0.3.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      964 2020-07-13 02:36:57.000000 illusional.wdlgen-0.3.0/setup.py
+drwxr-xr-x   0 lupat richard (648120765) wheel        (0)        0 2023-07-12 21:46:41.580698 illusional.wdlgen-0.3.1/
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)      101 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/.gitignore
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)     1022 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/.travis.yml
+drwxr-xr-x   0 lupat richard (648120765) wheel        (0)        0 2023-07-12 21:46:41.565607 illusional.wdlgen-0.3.1/.vscode/
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)      214 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/.vscode/settings.json
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)    35149 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/LICENSE
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)     9256 2023-07-12 21:46:41.580254 illusional.wdlgen-0.3.1/PKG-INFO
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)     8664 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/README.md
+drwxr-xr-x   0 lupat richard (648120765) wheel        (0)        0 2023-07-12 21:46:41.568177 illusional.wdlgen-0.3.1/illusional.wdlgen.egg-info/
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)     9256 2023-07-12 21:46:41.000000 illusional.wdlgen-0.3.1/illusional.wdlgen.egg-info/PKG-INFO
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)      521 2023-07-12 21:46:41.000000 illusional.wdlgen-0.3.1/illusional.wdlgen.egg-info/SOURCES.txt
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)        1 2023-07-12 21:46:41.000000 illusional.wdlgen-0.3.1/illusional.wdlgen.egg-info/dependency_links.txt
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)        1 2023-07-12 21:46:41.000000 illusional.wdlgen-0.3.1/illusional.wdlgen.egg-info/not-zip-safe
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)        7 2023-07-12 21:46:41.000000 illusional.wdlgen-0.3.1/illusional.wdlgen.egg-info/top_level.txt
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)       38 2023-07-12 21:46:41.580793 illusional.wdlgen-0.3.1/setup.cfg
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)      971 2023-07-12 21:45:13.000000 illusional.wdlgen-0.3.1/setup.py
+drwxr-xr-x   0 lupat richard (648120765) wheel        (0)        0 2023-07-12 21:46:41.575198 illusional.wdlgen-0.3.1/tests/
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)      319 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/tests/helpers.py
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)      528 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/tests/test_common.py
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)    11912 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/tests/test_task_generation.py
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)     1486 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/tests/test_types.py
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)     3708 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/tests/test_workflow_generation.py
+drwxr-xr-x   0 lupat richard (648120765) wheel        (0)        0 2023-07-12 21:46:41.579692 illusional.wdlgen-0.3.1/wdlgen/
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)      115 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/wdlgen/__init__.py
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)     3339 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/wdlgen/common.py
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)    10592 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/wdlgen/task.py
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)     5738 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/wdlgen/types.py
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)     3271 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/wdlgen/util.py
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)     3806 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/wdlgen/workflow.py
+-rw-r--r--   0 lupat richard (648120765) wheel        (0)     6259 2023-07-12 21:44:06.000000 illusional.wdlgen-0.3.1/wdlgen/workflowcall.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `illusional.wdlgen-0.3.0/wdlgen/util.py` & `illusional.wdlgen-0.3.1/wdlgen/util.py`

 * *Files identical despite different names*

### Comparing `illusional.wdlgen-0.3.0/wdlgen/task.py` & `illusional.wdlgen-0.3.1/wdlgen/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,56 +228,56 @@
         name = self.name
         blocks = []
 
         if self.inputs:
             blocks.append(
                 f"{tb}input {{\n"
                 + "\n".join(2 * tb + i.get_string() for i in self.inputs)
-                + f"\n{tb}}}"
+                + f"\n{tb}}}\n"
             )
 
         if self.command:
 
             if isinstance(self.command, list):
                 com = "\n".join(c.get_string(indent=2) for c in self.command)
             else:
                 com = self.command.get_string(indent=2)
-            blocks.append("{tb}command <<<\n{args}\n{tb}>>>".format(tb=tb, args=com))
+            blocks.append("{tb}command <<<\n{args}\n{tb}>>>\n".format(tb=tb, args=com))
 
         if self.runtime:
             rt = self.runtime.get_string(indent=2)
             blocks.append(
-                "{tb}runtime {{\n{args}\n{tb}}}".format(
+                "{tb}runtime {{\n{args}\n{tb}}}\n".format(
                     tb=tb,
                     args=rt,
                 )
             )
 
         if self.meta:
             mt = self.meta.get_string(indent=2)
             if mt:
                 blocks.append(
-                    "{tb}meta {{\n{args}\n{tb}}}".format(
+                    "{tb}meta {{\n{args}\n{tb}}}\n".format(
                         tb=tb, args=mt
                     )
                 )
 
         if self.param_meta:
             pmt = self.param_meta.get_string(indent=2)
             if pmt:
                 blocks.append(
-                    "{tb}parameter_meta {{\n{args}\n{tb}}}".format(
+                    "{tb}parameter_meta {{\n{args}\n{tb}}}\n".format(
                         tb=tb,
                         args=pmt
                     )
                 )
 
         if self.outputs:
             blocks.append(
-                "{tb}output {{\n{outs}\n{tb}}}".format(
+                "{tb}output {{\n{outs}\n{tb}}}\n".format(
                     tb=tb,
                     outs="\n".join((2 * tb) + o.get_string() for o in self.outputs),
                 )
             )
 
         return self.format.format(
             name=name, blocks="\n".join(blocks), version=self.version
```

### Comparing `illusional.wdlgen-0.3.0/wdlgen/common.py` & `illusional.wdlgen-0.3.1/wdlgen/common.py`

 * *Files identical despite different names*

### Comparing `illusional.wdlgen-0.3.0/wdlgen/workflow.py` & `illusional.wdlgen-0.3.1/wdlgen/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         self.format = """
 version {version}
 
 {imports_block}
 
 workflow {name} {{
 {blocks}
+
 }}""".strip()
 
     def get_string(self):
         tb = "  "
 
         name = self.name
         imports_block = ""
@@ -59,36 +60,36 @@
             ins = []
             for i in self.inputs:
                 wd = i.get_string()
                 if isinstance(wd, list):
                     ins.extend(2 * tb + ii for ii in wd)
                 else:
                     ins.append(2 * tb + wd)
-            blocks.append(f"{tb}input {{\n" + "\n".join(ins) + f"\n{tb}}}")
+            blocks.append(f"\n{tb}input {{\n" + "\n".join(ins) + f"\n{tb}}}")
 
         if self.calls:
-            blocks.append("\n".join(c.get_string(indent=1) for c in self.calls))
+            blocks.append("\n" + "\n\n".join(c.get_string(indent=1) for c in self.calls))
 
         if self.imports:
             imports_block = "\n".join(i.get_string() for i in self.imports)
 
         if self.meta:
             mt = self.meta.get_string(indent=2)
             if mt:
                 blocks.append(
-                    "{tb}meta {{\n{args}\n{tb}}}".format(
+                    "\n{tb}meta {{\n{args}\n{tb}}}".format(
                         tb=tb, args=mt
                     )
                 )
 
         if self.param_meta:
             pmt = self.param_meta.get_string(indent=2)
             if pmt:
                 blocks.append(
-                    "{tb}parameter_meta {{\n{args}\n{tb}}}".format(
+                    "\n{tb}parameter_meta {{\n{args}\n{tb}}}".format(
                         tb=tb,
                         args=pmt
                     )
                 )
 
         if self.outputs:
             outs = []
@@ -99,15 +100,15 @@
                     if isinstance(wd, list):
                         outs.extend((2 * tb) + w for w in wd)
                     else:
                         outs.append((2 * tb) + wd)
                 else:
                     outs.append(str(o))
             blocks.append(
-                "{tb}output {{\n{outs}\n{tb}}}".format(tb=tb, outs="\n".join(outs))
+                "\n{tb}output {{\n{outs}\n{tb}}}".format(tb=tb, outs="\n".join(outs))
             )
 
         return self.format.format(
             name=name,
             imports_block=imports_block,
             blocks="\n".join(blocks),
             version=self.version,
```

### Comparing `illusional.wdlgen-0.3.0/wdlgen/types.py` & `illusional.wdlgen-0.3.1/wdlgen/types.py`

 * *Files identical despite different names*

### Comparing `illusional.wdlgen-0.3.0/PKG-INFO` & `illusional.wdlgen-0.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,234 +1,235 @@
 Metadata-Version: 2.1
 Name: illusional.wdlgen
-Version: 0.3.0
+Version: 0.3.1
 Summary: Contains classes and helpers to generate WDL without worrying about the syntax. This is primarily intended for generating WDL from other in-memory representations of a workflow.
-Home-page: https://github.com/illusional/python-wdlgen
-Author: Michael Franklin
-Author-email: michael.franklin@petermac.org
+Home-page: https://github.com/PMCC-BioinformaticsCore/python-wdlgen
+Author: Richard Lupat
+Author-email: richard.lupat@petermac.org
 License: GNU
-Description: # python-wdlgen
-        
-        [![Build Status](https://travis-ci.org/PMCC-BioinformaticsCore/python-wdlgen.svg?branch=master)](https://travis-ci.org/PMCC-BioinformaticsCore/python-wdlgen)
-        [![PyPI version](https://badge.fury.io/py/illusional.wdlgen.svg)](https://badge.fury.io/py/illusional.wdlgen)
-         
-        [Workflow Description Language](http://www.openwdl.org) is way to describe tasks and workflows in a "_human readable and writable way_". It was initially developed and offered by [Broad Institute](https://software.broadinstitute.org/) to be paired with their workflow engine [Cromwell](https://cromwell.readthedocs.io/en/stable/), however it has since been made open source with other engines such as [Toil](http://toil.readthedocs.io/en/3.14.0/running/wdl.html) and [DNAnexus\*](https://github.com/dnanexus/dxWDL).
-        
-        
-        ### WARNING
-        
-        This module now only generates developmental WDL, this includes Directories and wrapping all inputs in an input block. 
-        To use this generated WDL, you must use a version of **Cromwell higher than 37**. 
-        
-        This module automatically includes `version development` in the Workflow and Task outputs. 
-        The guides below may not reflect the current version of this repository, but will be updated soon.
-        
-        This syntax is based on the [Developmental Workflow Description Language specification](https://github.com/openwdl/wdl/blob/master/versions/development/SPEC.md).
-        
-        ___
-        
-        ## Motiviation
-        
-        I needed an easy way to generate some _BASIC_ WDL through some in memory objects, and I was using ([a fork](https://github.com/illusional/python-cwlgen) of) [common-workflow-language/python-cwlgen](https://github.com/common-workflow-language/python-cwlgen), I figured I could open this up to see what use it has.
-        
-        ## Installation
-        
-        ```
-        pip install illusional.wdlgen
-        ```
-        
-        ## General support
-        
-        This software is provided as-is, without warranty of any kind ... and so on.
-        
-        It's a pretty dumb wrapper that uses string interpolation to generate the structure. It wouldn't handle automatically escaping illegal characters.
-        
-        Generally it supports:
-        
-        - Types - All types are represented as a `WdlType`, which can either be a [`PrimitiveType`](https://github.com/openwdl/wdl/blob/master/versions/1.0/SPEC.md#types), or an `ArrayType` (see [goal](#goals)). Also supports the postfix quantifiers.
-        
-        - Workflow creation (`wdlgen.Workflow`)
-        	- manual imports (`wdlgen.Workflow.WorkflowImport`)
-        	- inputs (`wdlgen.Input`)
-        	- outputs (`wdlgen.Output`)
-        	- calls:
-        		- general call (`wdlgen.WorkflowCall`)
-        		- scatter (`wdlgen.WorkflowScatter(WorkflowCall[])`)
-            - meta: `wdlgen.Meta`
-            - parameter_meta: `wdlgen.ParameterMeta`
-            
-        - Task creation (`wdlgen.Task`) - This is based similar to how [CWL constructs its commands](https://www.commonwl.org/v1.0/CommandLineTool.html#CommandLineTool).
-        	- inputs: `wdlgen.Input`
-        	- outputs: `wdlgen.Output`
-        	- runtime: `wdlgen.Task.Runtime`
-        	- command: `wdlgen.Task.Command`
-        		- arguments: `wdlgen.Task.Command.Argument`
-        		- inputs: `wdlgen.Task.Command.Input`
-            - meta: `wdlgen.Meta`
-            - parameter_meta: `wdlgen.ParameterMeta`
-        
-        ## How to use
-        
-        This will give you a _brief_ overview on how to _use_ python-wdlgen. Goals are to improve the write a proper documentation spec, but if you have a moderate understanding of workflows in either CWL or WDL, this code will hopefully be fairly intuitive.
-        
-        Every class inherits from a `WDLBase` which means it must have a `get_string()` method which returns the string representation of the class, calling this on any children it may have.
-        
-        ### Types
-        
-        All types are represented as a WDLType, which has a parse method. It's a little overkill in some cases, but makes managing attributes a bit easier.
-        
-        ```python
-        parsed_string = wdlgen.WdlType.parse("String")	# WdlType<PrimitiveType<String>>
-        parsed_op_str = wdlgen.WdlType.parse("String?") # WdlType<PrimtiveType<String>>
-        parsed_array = wdlgen.WDLType.parse("File[]")	# WdlType<ArrayType<File>>
-        parsed_ar_oq = wdlgen.WdlType(parse("Int?[]+"))	# WdlType<ArrayType<Int?> (+)>
-        ```
-        
-        You can also construct these manually:
-        ```python
-        parsed_string = WdlType(PrimitiveType("String"))
-        parsed_op_str = WdlType(PrimtiveType("String", optional=True))
-        parsed_array = WdlType(ArrayType(WdlType(PrimitiveType("File"))))
-        parsed_ar_q = WdlType(ArrayType(WdlType(PrimitiveType("Int"), optional=True), requires_multiple=True))
-        ```
-        
-        ### Input / Output
-        Input: `wdlgen.Input(data_type: WdlType, name: str, expression: str = None)`
-        
-        Output: `wdlgen.Output(data_type: WdlType, name: str, expression: str = None)`
-        
-        both of which output something like:
-        	`{WdlType} {name} [= {expression}]`
-        
-        ### Task
-        
-        A task is a collection of Inputs, Outputs and a Command that are identified by a _name_. Inputs and Outputs are as above. Note that you can use functions such as `stdout()` or other for the expression.
-        
-        > If you don't want to play by these rules, don't include any inputs or outputs and just provide your whole string to the initializer for command.
-        
-        ```python
-        t = wdlgen.Task("task_name")
-        t.inputs.append(wdlgen.Input(wdlgen.WdlType.parse("String"), "taskGreeting"))
-        # command in next section
-        t.outputs.append(wdlgen.Output(wdlgen.WdlType.parse("File"), "standardOut", "stdout()"))
-        ```
-        
-        #### Command
-        
-        The command is broken up similar to how CWL breaks its command generation up, by itself it has a _base command_. Each component has a corresponding input (else use the `wdlgen.Task.Command.Argument` class), optionality, position, prefix (and whether the value should be separated from prefix; think `-o {val}` vs `outputDir={val}`) and potentially a default.
-        
-        Construct a command like the following:
-        ```python
-        command = wdlgen.Task.Command("echo")
-        command.inputs.append(wdlgen.Task.Command.CommandInput("taskGreeting", optional=False, position=None, prefix="-a", separate_value_from_prefix=True, default=None))
-        command.inputs.append(wdlgen.Task.Command.CommandInput("otherInput", optional=True, position=2, prefix="optional-param=", separate_value_from_prefix=False, default=None))
-        
-        # t is the task
-        t.command = command
-        print(command.get_string())
-        ```
-        
-        This will result in the following WDL command:
-        ```bash
-        echo \
-          -a ${taskGreeting} \
-          ${"optional-param=" + otherInput}
-        ```
-        
-        #### Task output:
-        
-        The combination of the task and command outputs:
-        ```wdl
-        version development
-        
-        task task_name {
-          input {
-            String taskGreeting
-          }
-          command {
-            echo \
-              -a ${taskGreeting} \
-              ${"optional-param=" + otherInput}
-          }
-        
-          output {
-            File standardOut = stdout()
-          }
-        }
-        ```
-        
-        ### Workflow
-        
-        You should have moderate idea of the structure of WDL as there's no cleverness or abstraction done anywhere. Beware: there's also no checking attributes (to see if your `inputMap` actually corresponds to inputs).
-        
-        The structure of a workflow is m
-        
-        ```python
-        w = wdlgen.Workflow("workflow_name")
-        
-        w.imports.append(wdlgen.Workflow.WorkflowImport("tool_file", ""))
-        w.inputs.append(
-            wdlgen.Input(
-                wdlgen.WdlType.parse("String"), 
-                "inputGreeting"
-            )
-        )
-        
-        
-        inputs_map = {"taskGreeting": "inputGreeting"}
-        w.calls.append(wdlgen.WorkflowCall("Q.namspaced_task_identifier", "task_alias", inputs_map))
-        w.outputs.append(wdlgen.Output(wdlgen.WdlType.parse("File"), "standardOut", "task_alias.standardOut")
-        ```
-        
-        Which outputs:
-        ```wdl
-        version development
-        
-        import "tools/tool_file.wdl"
-        
-        workflow workflow_name {
-          input { 
-            String inputGreeting
-          }
-          call Q.namspaced_task_identifier as task_alias {
-            input:
-              taskGreeting=inputGreeting
-          }
-          output {
-            File standardOut = task_alias.standardOut
-          }
-        }
-        ```
-        
-        
-        ## Known limitations
-        
-        I'm not a fan of the string interpolation generation of WDL that this module does. I think trying to build an [Abstract syntax tree](https://en.wikipedia.org/wiki/Abstract_syntax_tree) and then there should be something that convert that into the DSL that WDL uses.
-        
-        You could also cause syntax errors in generated WDL by providing illegal characters. 
-        
-        ## Goals
-        
-        - Improve code-level documentation.
-        - Increase the testing coverage + quality of unit tests.
-        - Better represent the WDL spec.
-        - ~~Find an easier distribution / release method - such as PIP.~~
-        - ~~Automate testing and delivery through TravisCI / CircleCI or similar.~~
-        - Validate each value by [WDL's language specifications](https://github.com/openwdl/wdl/blob/master/versions/1.0/SPEC.md#language-specification).
-        - Add support for structs
-        
-        ### Long goals
-        - Write a documentation site.
-        - Make classes convert into AST and then into DSL.
-        
-        ## Issues and Pull Requests
-        Feel free to log issues and make pull requests. I make no guarantee to the existence or timeliness of replies.
-        
-        
-        Links:
-        
-        - WDL description: https://github.com/openwdl/wdl/blob/master/versions/1.0/SPEC.md
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# python-wdlgen
+
+[![Build Status](https://travis-ci.org/PMCC-BioinformaticsCore/python-wdlgen.svg?branch=master)](https://travis-ci.org/PMCC-BioinformaticsCore/python-wdlgen)
+[![PyPI version](https://badge.fury.io/py/illusional.wdlgen.svg)](https://badge.fury.io/py/illusional.wdlgen)
+ 
+[Workflow Description Language](http://www.openwdl.org) is way to describe tasks and workflows in a "_human readable and writable way_". It was initially developed and offered by [Broad Institute](https://software.broadinstitute.org/) to be paired with their workflow engine [Cromwell](https://cromwell.readthedocs.io/en/stable/), however it has since been made open source with other engines such as [Toil](http://toil.readthedocs.io/en/3.14.0/running/wdl.html) and [DNAnexus\*](https://github.com/dnanexus/dxWDL).
+
+
+### WARNING
+
+This module now only generates developmental WDL, this includes Directories and wrapping all inputs in an input block. 
+To use this generated WDL, you must use a version of **Cromwell higher than 37**. 
+
+This module automatically includes `version development` in the Workflow and Task outputs. 
+The guides below may not reflect the current version of this repository, but will be updated soon.
+
+This syntax is based on the [Developmental Workflow Description Language specification](https://github.com/openwdl/wdl/blob/master/versions/development/SPEC.md).
+
+___
+
+## Motiviation
+
+I needed an easy way to generate some _BASIC_ WDL through some in memory objects, and I was using ([a fork](https://github.com/illusional/python-cwlgen) of) [common-workflow-language/python-cwlgen](https://github.com/common-workflow-language/python-cwlgen), I figured I could open this up to see what use it has.
+
+## Installation
+
+```
+pip install illusional.wdlgen
+```
+
+## General support
+
+This software is provided as-is, without warranty of any kind ... and so on.
+
+It's a pretty dumb wrapper that uses string interpolation to generate the structure. It wouldn't handle automatically escaping illegal characters.
+
+Generally it supports:
+
+- Types - All types are represented as a `WdlType`, which can either be a [`PrimitiveType`](https://github.com/openwdl/wdl/blob/master/versions/1.0/SPEC.md#types), or an `ArrayType` (see [goal](#goals)). Also supports the postfix quantifiers.
+
+- Workflow creation (`wdlgen.Workflow`)
+	- manual imports (`wdlgen.Workflow.WorkflowImport`)
+	- inputs (`wdlgen.Input`)
+	- outputs (`wdlgen.Output`)
+	- calls:
+		- general call (`wdlgen.WorkflowCall`)
+		- scatter (`wdlgen.WorkflowScatter(WorkflowCall[])`)
+    - meta: `wdlgen.Meta`
+    - parameter_meta: `wdlgen.ParameterMeta`
+    
+- Task creation (`wdlgen.Task`) - This is based similar to how [CWL constructs its commands](https://www.commonwl.org/v1.0/CommandLineTool.html#CommandLineTool).
+	- inputs: `wdlgen.Input`
+	- outputs: `wdlgen.Output`
+	- runtime: `wdlgen.Task.Runtime`
+	- command: `wdlgen.Task.Command`
+		- arguments: `wdlgen.Task.Command.Argument`
+		- inputs: `wdlgen.Task.Command.Input`
+    - meta: `wdlgen.Meta`
+    - parameter_meta: `wdlgen.ParameterMeta`
+
+## How to use
+
+This will give you a _brief_ overview on how to _use_ python-wdlgen. Goals are to improve the write a proper documentation spec, but if you have a moderate understanding of workflows in either CWL or WDL, this code will hopefully be fairly intuitive.
+
+Every class inherits from a `WDLBase` which means it must have a `get_string()` method which returns the string representation of the class, calling this on any children it may have.
+
+### Types
+
+All types are represented as a WDLType, which has a parse method. It's a little overkill in some cases, but makes managing attributes a bit easier.
+
+```python
+parsed_string = wdlgen.WdlType.parse("String")	# WdlType<PrimitiveType<String>>
+parsed_op_str = wdlgen.WdlType.parse("String?") # WdlType<PrimtiveType<String>>
+parsed_array = wdlgen.WDLType.parse("File[]")	# WdlType<ArrayType<File>>
+parsed_ar_oq = wdlgen.WdlType(parse("Int?[]+"))	# WdlType<ArrayType<Int?> (+)>
+```
+
+You can also construct these manually:
+```python
+parsed_string = WdlType(PrimitiveType("String"))
+parsed_op_str = WdlType(PrimtiveType("String", optional=True))
+parsed_array = WdlType(ArrayType(WdlType(PrimitiveType("File"))))
+parsed_ar_q = WdlType(ArrayType(WdlType(PrimitiveType("Int"), optional=True), requires_multiple=True))
+```
+
+### Input / Output
+Input: `wdlgen.Input(data_type: WdlType, name: str, expression: str = None)`
+
+Output: `wdlgen.Output(data_type: WdlType, name: str, expression: str = None)`
+
+both of which output something like:
+	`{WdlType} {name} [= {expression}]`
+
+### Task
+
+A task is a collection of Inputs, Outputs and a Command that are identified by a _name_. Inputs and Outputs are as above. Note that you can use functions such as `stdout()` or other for the expression.
+
+> If you don't want to play by these rules, don't include any inputs or outputs and just provide your whole string to the initializer for command.
+
+```python
+t = wdlgen.Task("task_name")
+t.inputs.append(wdlgen.Input(wdlgen.WdlType.parse("String"), "taskGreeting"))
+# command in next section
+t.outputs.append(wdlgen.Output(wdlgen.WdlType.parse("File"), "standardOut", "stdout()"))
+```
+
+#### Command
+
+The command is broken up similar to how CWL breaks its command generation up, by itself it has a _base command_. Each component has a corresponding input (else use the `wdlgen.Task.Command.Argument` class), optionality, position, prefix (and whether the value should be separated from prefix; think `-o {val}` vs `outputDir={val}`) and potentially a default.
+
+Construct a command like the following:
+```python
+command = wdlgen.Task.Command("echo")
+command.inputs.append(wdlgen.Task.Command.CommandInput("taskGreeting", optional=False, position=None, prefix="-a", separate_value_from_prefix=True, default=None))
+command.inputs.append(wdlgen.Task.Command.CommandInput("otherInput", optional=True, position=2, prefix="optional-param=", separate_value_from_prefix=False, default=None))
+
+# t is the task
+t.command = command
+print(command.get_string())
+```
+
+This will result in the following WDL command:
+```bash
+echo \
+  -a ${taskGreeting} \
+  ${"optional-param=" + otherInput}
+```
+
+#### Task output:
+
+The combination of the task and command outputs:
+```wdl
+version development
+
+task task_name {
+  input {
+    String taskGreeting
+  }
+  command {
+    echo \
+      -a ${taskGreeting} \
+      ${"optional-param=" + otherInput}
+  }
+
+  output {
+    File standardOut = stdout()
+  }
+}
+```
+
+### Workflow
+
+You should have moderate idea of the structure of WDL as there's no cleverness or abstraction done anywhere. Beware: there's also no checking attributes (to see if your `inputMap` actually corresponds to inputs).
+
+The structure of a workflow is m
+
+```python
+w = wdlgen.Workflow("workflow_name")
+
+w.imports.append(wdlgen.Workflow.WorkflowImport("tool_file", ""))
+w.inputs.append(
+    wdlgen.Input(
+        wdlgen.WdlType.parse("String"), 
+        "inputGreeting"
+    )
+)
+
+
+inputs_map = {"taskGreeting": "inputGreeting"}
+w.calls.append(wdlgen.WorkflowCall("Q.namspaced_task_identifier", "task_alias", inputs_map))
+w.outputs.append(wdlgen.Output(wdlgen.WdlType.parse("File"), "standardOut", "task_alias.standardOut")
+```
+
+Which outputs:
+```wdl
+version development
+
+import "tools/tool_file.wdl"
+
+workflow workflow_name {
+  input { 
+    String inputGreeting
+  }
+  call Q.namspaced_task_identifier as task_alias {
+    input:
+      taskGreeting=inputGreeting
+  }
+  output {
+    File standardOut = task_alias.standardOut
+  }
+}
+```
+
+
+## Known limitations
+
+I'm not a fan of the string interpolation generation of WDL that this module does. I think trying to build an [Abstract syntax tree](https://en.wikipedia.org/wiki/Abstract_syntax_tree) and then there should be something that convert that into the DSL that WDL uses.
+
+You could also cause syntax errors in generated WDL by providing illegal characters. 
+
+## Goals
+
+- Improve code-level documentation.
+- Increase the testing coverage + quality of unit tests.
+- Better represent the WDL spec.
+- ~~Find an easier distribution / release method - such as PIP.~~
+- ~~Automate testing and delivery through TravisCI / CircleCI or similar.~~
+- Validate each value by [WDL's language specifications](https://github.com/openwdl/wdl/blob/master/versions/1.0/SPEC.md#language-specification).
+- Add support for structs
+
+### Long goals
+- Write a documentation site.
+- Make classes convert into AST and then into DSL.
+
+## Issues and Pull Requests
+Feel free to log issues and make pull requests. I make no guarantee to the existence or timeliness of replies.
+
+
+Links:
+
+- WDL description: https://github.com/openwdl/wdl/blob/master/versions/1.0/SPEC.md
```

### Comparing `illusional.wdlgen-0.3.0/illusional.wdlgen.egg-info/PKG-INFO` & `illusional.wdlgen-0.3.1/illusional.wdlgen.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,234 +1,235 @@
 Metadata-Version: 2.1
 Name: illusional.wdlgen
-Version: 0.3.0
+Version: 0.3.1
 Summary: Contains classes and helpers to generate WDL without worrying about the syntax. This is primarily intended for generating WDL from other in-memory representations of a workflow.
-Home-page: https://github.com/illusional/python-wdlgen
-Author: Michael Franklin
-Author-email: michael.franklin@petermac.org
+Home-page: https://github.com/PMCC-BioinformaticsCore/python-wdlgen
+Author: Richard Lupat
+Author-email: richard.lupat@petermac.org
 License: GNU
-Description: # python-wdlgen
-        
-        [![Build Status](https://travis-ci.org/PMCC-BioinformaticsCore/python-wdlgen.svg?branch=master)](https://travis-ci.org/PMCC-BioinformaticsCore/python-wdlgen)
-        [![PyPI version](https://badge.fury.io/py/illusional.wdlgen.svg)](https://badge.fury.io/py/illusional.wdlgen)
-         
-        [Workflow Description Language](http://www.openwdl.org) is way to describe tasks and workflows in a "_human readable and writable way_". It was initially developed and offered by [Broad Institute](https://software.broadinstitute.org/) to be paired with their workflow engine [Cromwell](https://cromwell.readthedocs.io/en/stable/), however it has since been made open source with other engines such as [Toil](http://toil.readthedocs.io/en/3.14.0/running/wdl.html) and [DNAnexus\*](https://github.com/dnanexus/dxWDL).
-        
-        
-        ### WARNING
-        
-        This module now only generates developmental WDL, this includes Directories and wrapping all inputs in an input block. 
-        To use this generated WDL, you must use a version of **Cromwell higher than 37**. 
-        
-        This module automatically includes `version development` in the Workflow and Task outputs. 
-        The guides below may not reflect the current version of this repository, but will be updated soon.
-        
-        This syntax is based on the [Developmental Workflow Description Language specification](https://github.com/openwdl/wdl/blob/master/versions/development/SPEC.md).
-        
-        ___
-        
-        ## Motiviation
-        
-        I needed an easy way to generate some _BASIC_ WDL through some in memory objects, and I was using ([a fork](https://github.com/illusional/python-cwlgen) of) [common-workflow-language/python-cwlgen](https://github.com/common-workflow-language/python-cwlgen), I figured I could open this up to see what use it has.
-        
-        ## Installation
-        
-        ```
-        pip install illusional.wdlgen
-        ```
-        
-        ## General support
-        
-        This software is provided as-is, without warranty of any kind ... and so on.
-        
-        It's a pretty dumb wrapper that uses string interpolation to generate the structure. It wouldn't handle automatically escaping illegal characters.
-        
-        Generally it supports:
-        
-        - Types - All types are represented as a `WdlType`, which can either be a [`PrimitiveType`](https://github.com/openwdl/wdl/blob/master/versions/1.0/SPEC.md#types), or an `ArrayType` (see [goal](#goals)). Also supports the postfix quantifiers.
-        
-        - Workflow creation (`wdlgen.Workflow`)
-        	- manual imports (`wdlgen.Workflow.WorkflowImport`)
-        	- inputs (`wdlgen.Input`)
-        	- outputs (`wdlgen.Output`)
-        	- calls:
-        		- general call (`wdlgen.WorkflowCall`)
-        		- scatter (`wdlgen.WorkflowScatter(WorkflowCall[])`)
-            - meta: `wdlgen.Meta`
-            - parameter_meta: `wdlgen.ParameterMeta`
-            
-        - Task creation (`wdlgen.Task`) - This is based similar to how [CWL constructs its commands](https://www.commonwl.org/v1.0/CommandLineTool.html#CommandLineTool).
-        	- inputs: `wdlgen.Input`
-        	- outputs: `wdlgen.Output`
-        	- runtime: `wdlgen.Task.Runtime`
-        	- command: `wdlgen.Task.Command`
-        		- arguments: `wdlgen.Task.Command.Argument`
-        		- inputs: `wdlgen.Task.Command.Input`
-            - meta: `wdlgen.Meta`
-            - parameter_meta: `wdlgen.ParameterMeta`
-        
-        ## How to use
-        
-        This will give you a _brief_ overview on how to _use_ python-wdlgen. Goals are to improve the write a proper documentation spec, but if you have a moderate understanding of workflows in either CWL or WDL, this code will hopefully be fairly intuitive.
-        
-        Every class inherits from a `WDLBase` which means it must have a `get_string()` method which returns the string representation of the class, calling this on any children it may have.
-        
-        ### Types
-        
-        All types are represented as a WDLType, which has a parse method. It's a little overkill in some cases, but makes managing attributes a bit easier.
-        
-        ```python
-        parsed_string = wdlgen.WdlType.parse("String")	# WdlType<PrimitiveType<String>>
-        parsed_op_str = wdlgen.WdlType.parse("String?") # WdlType<PrimtiveType<String>>
-        parsed_array = wdlgen.WDLType.parse("File[]")	# WdlType<ArrayType<File>>
-        parsed_ar_oq = wdlgen.WdlType(parse("Int?[]+"))	# WdlType<ArrayType<Int?> (+)>
-        ```
-        
-        You can also construct these manually:
-        ```python
-        parsed_string = WdlType(PrimitiveType("String"))
-        parsed_op_str = WdlType(PrimtiveType("String", optional=True))
-        parsed_array = WdlType(ArrayType(WdlType(PrimitiveType("File"))))
-        parsed_ar_q = WdlType(ArrayType(WdlType(PrimitiveType("Int"), optional=True), requires_multiple=True))
-        ```
-        
-        ### Input / Output
-        Input: `wdlgen.Input(data_type: WdlType, name: str, expression: str = None)`
-        
-        Output: `wdlgen.Output(data_type: WdlType, name: str, expression: str = None)`
-        
-        both of which output something like:
-        	`{WdlType} {name} [= {expression}]`
-        
-        ### Task
-        
-        A task is a collection of Inputs, Outputs and a Command that are identified by a _name_. Inputs and Outputs are as above. Note that you can use functions such as `stdout()` or other for the expression.
-        
-        > If you don't want to play by these rules, don't include any inputs or outputs and just provide your whole string to the initializer for command.
-        
-        ```python
-        t = wdlgen.Task("task_name")
-        t.inputs.append(wdlgen.Input(wdlgen.WdlType.parse("String"), "taskGreeting"))
-        # command in next section
-        t.outputs.append(wdlgen.Output(wdlgen.WdlType.parse("File"), "standardOut", "stdout()"))
-        ```
-        
-        #### Command
-        
-        The command is broken up similar to how CWL breaks its command generation up, by itself it has a _base command_. Each component has a corresponding input (else use the `wdlgen.Task.Command.Argument` class), optionality, position, prefix (and whether the value should be separated from prefix; think `-o {val}` vs `outputDir={val}`) and potentially a default.
-        
-        Construct a command like the following:
-        ```python
-        command = wdlgen.Task.Command("echo")
-        command.inputs.append(wdlgen.Task.Command.CommandInput("taskGreeting", optional=False, position=None, prefix="-a", separate_value_from_prefix=True, default=None))
-        command.inputs.append(wdlgen.Task.Command.CommandInput("otherInput", optional=True, position=2, prefix="optional-param=", separate_value_from_prefix=False, default=None))
-        
-        # t is the task
-        t.command = command
-        print(command.get_string())
-        ```
-        
-        This will result in the following WDL command:
-        ```bash
-        echo \
-          -a ${taskGreeting} \
-          ${"optional-param=" + otherInput}
-        ```
-        
-        #### Task output:
-        
-        The combination of the task and command outputs:
-        ```wdl
-        version development
-        
-        task task_name {
-          input {
-            String taskGreeting
-          }
-          command {
-            echo \
-              -a ${taskGreeting} \
-              ${"optional-param=" + otherInput}
-          }
-        
-          output {
-            File standardOut = stdout()
-          }
-        }
-        ```
-        
-        ### Workflow
-        
-        You should have moderate idea of the structure of WDL as there's no cleverness or abstraction done anywhere. Beware: there's also no checking attributes (to see if your `inputMap` actually corresponds to inputs).
-        
-        The structure of a workflow is m
-        
-        ```python
-        w = wdlgen.Workflow("workflow_name")
-        
-        w.imports.append(wdlgen.Workflow.WorkflowImport("tool_file", ""))
-        w.inputs.append(
-            wdlgen.Input(
-                wdlgen.WdlType.parse("String"), 
-                "inputGreeting"
-            )
-        )
-        
-        
-        inputs_map = {"taskGreeting": "inputGreeting"}
-        w.calls.append(wdlgen.WorkflowCall("Q.namspaced_task_identifier", "task_alias", inputs_map))
-        w.outputs.append(wdlgen.Output(wdlgen.WdlType.parse("File"), "standardOut", "task_alias.standardOut")
-        ```
-        
-        Which outputs:
-        ```wdl
-        version development
-        
-        import "tools/tool_file.wdl"
-        
-        workflow workflow_name {
-          input { 
-            String inputGreeting
-          }
-          call Q.namspaced_task_identifier as task_alias {
-            input:
-              taskGreeting=inputGreeting
-          }
-          output {
-            File standardOut = task_alias.standardOut
-          }
-        }
-        ```
-        
-        
-        ## Known limitations
-        
-        I'm not a fan of the string interpolation generation of WDL that this module does. I think trying to build an [Abstract syntax tree](https://en.wikipedia.org/wiki/Abstract_syntax_tree) and then there should be something that convert that into the DSL that WDL uses.
-        
-        You could also cause syntax errors in generated WDL by providing illegal characters. 
-        
-        ## Goals
-        
-        - Improve code-level documentation.
-        - Increase the testing coverage + quality of unit tests.
-        - Better represent the WDL spec.
-        - ~~Find an easier distribution / release method - such as PIP.~~
-        - ~~Automate testing and delivery through TravisCI / CircleCI or similar.~~
-        - Validate each value by [WDL's language specifications](https://github.com/openwdl/wdl/blob/master/versions/1.0/SPEC.md#language-specification).
-        - Add support for structs
-        
-        ### Long goals
-        - Write a documentation site.
-        - Make classes convert into AST and then into DSL.
-        
-        ## Issues and Pull Requests
-        Feel free to log issues and make pull requests. I make no guarantee to the existence or timeliness of replies.
-        
-        
-        Links:
-        
-        - WDL description: https://github.com/openwdl/wdl/blob/master/versions/1.0/SPEC.md
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# python-wdlgen
+
+[![Build Status](https://travis-ci.org/PMCC-BioinformaticsCore/python-wdlgen.svg?branch=master)](https://travis-ci.org/PMCC-BioinformaticsCore/python-wdlgen)
+[![PyPI version](https://badge.fury.io/py/illusional.wdlgen.svg)](https://badge.fury.io/py/illusional.wdlgen)
+ 
+[Workflow Description Language](http://www.openwdl.org) is way to describe tasks and workflows in a "_human readable and writable way_". It was initially developed and offered by [Broad Institute](https://software.broadinstitute.org/) to be paired with their workflow engine [Cromwell](https://cromwell.readthedocs.io/en/stable/), however it has since been made open source with other engines such as [Toil](http://toil.readthedocs.io/en/3.14.0/running/wdl.html) and [DNAnexus\*](https://github.com/dnanexus/dxWDL).
+
+
+### WARNING
+
+This module now only generates developmental WDL, this includes Directories and wrapping all inputs in an input block. 
+To use this generated WDL, you must use a version of **Cromwell higher than 37**. 
+
+This module automatically includes `version development` in the Workflow and Task outputs. 
+The guides below may not reflect the current version of this repository, but will be updated soon.
+
+This syntax is based on the [Developmental Workflow Description Language specification](https://github.com/openwdl/wdl/blob/master/versions/development/SPEC.md).
+
+___
+
+## Motiviation
+
+I needed an easy way to generate some _BASIC_ WDL through some in memory objects, and I was using ([a fork](https://github.com/illusional/python-cwlgen) of) [common-workflow-language/python-cwlgen](https://github.com/common-workflow-language/python-cwlgen), I figured I could open this up to see what use it has.
+
+## Installation
+
+```
+pip install illusional.wdlgen
+```
+
+## General support
+
+This software is provided as-is, without warranty of any kind ... and so on.
+
+It's a pretty dumb wrapper that uses string interpolation to generate the structure. It wouldn't handle automatically escaping illegal characters.
+
+Generally it supports:
+
+- Types - All types are represented as a `WdlType`, which can either be a [`PrimitiveType`](https://github.com/openwdl/wdl/blob/master/versions/1.0/SPEC.md#types), or an `ArrayType` (see [goal](#goals)). Also supports the postfix quantifiers.
+
+- Workflow creation (`wdlgen.Workflow`)
+	- manual imports (`wdlgen.Workflow.WorkflowImport`)
+	- inputs (`wdlgen.Input`)
+	- outputs (`wdlgen.Output`)
+	- calls:
+		- general call (`wdlgen.WorkflowCall`)
+		- scatter (`wdlgen.WorkflowScatter(WorkflowCall[])`)
+    - meta: `wdlgen.Meta`
+    - parameter_meta: `wdlgen.ParameterMeta`
+    
+- Task creation (`wdlgen.Task`) - This is based similar to how [CWL constructs its commands](https://www.commonwl.org/v1.0/CommandLineTool.html#CommandLineTool).
+	- inputs: `wdlgen.Input`
+	- outputs: `wdlgen.Output`
+	- runtime: `wdlgen.Task.Runtime`
+	- command: `wdlgen.Task.Command`
+		- arguments: `wdlgen.Task.Command.Argument`
+		- inputs: `wdlgen.Task.Command.Input`
+    - meta: `wdlgen.Meta`
+    - parameter_meta: `wdlgen.ParameterMeta`
+
+## How to use
+
+This will give you a _brief_ overview on how to _use_ python-wdlgen. Goals are to improve the write a proper documentation spec, but if you have a moderate understanding of workflows in either CWL or WDL, this code will hopefully be fairly intuitive.
+
+Every class inherits from a `WDLBase` which means it must have a `get_string()` method which returns the string representation of the class, calling this on any children it may have.
+
+### Types
+
+All types are represented as a WDLType, which has a parse method. It's a little overkill in some cases, but makes managing attributes a bit easier.
+
+```python
+parsed_string = wdlgen.WdlType.parse("String")	# WdlType<PrimitiveType<String>>
+parsed_op_str = wdlgen.WdlType.parse("String?") # WdlType<PrimtiveType<String>>
+parsed_array = wdlgen.WDLType.parse("File[]")	# WdlType<ArrayType<File>>
+parsed_ar_oq = wdlgen.WdlType(parse("Int?[]+"))	# WdlType<ArrayType<Int?> (+)>
+```
+
+You can also construct these manually:
+```python
+parsed_string = WdlType(PrimitiveType("String"))
+parsed_op_str = WdlType(PrimtiveType("String", optional=True))
+parsed_array = WdlType(ArrayType(WdlType(PrimitiveType("File"))))
+parsed_ar_q = WdlType(ArrayType(WdlType(PrimitiveType("Int"), optional=True), requires_multiple=True))
+```
+
+### Input / Output
+Input: `wdlgen.Input(data_type: WdlType, name: str, expression: str = None)`
+
+Output: `wdlgen.Output(data_type: WdlType, name: str, expression: str = None)`
+
+both of which output something like:
+	`{WdlType} {name} [= {expression}]`
+
+### Task
+
+A task is a collection of Inputs, Outputs and a Command that are identified by a _name_. Inputs and Outputs are as above. Note that you can use functions such as `stdout()` or other for the expression.
+
+> If you don't want to play by these rules, don't include any inputs or outputs and just provide your whole string to the initializer for command.
+
+```python
+t = wdlgen.Task("task_name")
+t.inputs.append(wdlgen.Input(wdlgen.WdlType.parse("String"), "taskGreeting"))
+# command in next section
+t.outputs.append(wdlgen.Output(wdlgen.WdlType.parse("File"), "standardOut", "stdout()"))
+```
+
+#### Command
+
+The command is broken up similar to how CWL breaks its command generation up, by itself it has a _base command_. Each component has a corresponding input (else use the `wdlgen.Task.Command.Argument` class), optionality, position, prefix (and whether the value should be separated from prefix; think `-o {val}` vs `outputDir={val}`) and potentially a default.
+
+Construct a command like the following:
+```python
+command = wdlgen.Task.Command("echo")
+command.inputs.append(wdlgen.Task.Command.CommandInput("taskGreeting", optional=False, position=None, prefix="-a", separate_value_from_prefix=True, default=None))
+command.inputs.append(wdlgen.Task.Command.CommandInput("otherInput", optional=True, position=2, prefix="optional-param=", separate_value_from_prefix=False, default=None))
+
+# t is the task
+t.command = command
+print(command.get_string())
+```
+
+This will result in the following WDL command:
+```bash
+echo \
+  -a ${taskGreeting} \
+  ${"optional-param=" + otherInput}
+```
+
+#### Task output:
+
+The combination of the task and command outputs:
+```wdl
+version development
+
+task task_name {
+  input {
+    String taskGreeting
+  }
+  command {
+    echo \
+      -a ${taskGreeting} \
+      ${"optional-param=" + otherInput}
+  }
+
+  output {
+    File standardOut = stdout()
+  }
+}
+```
+
+### Workflow
+
+You should have moderate idea of the structure of WDL as there's no cleverness or abstraction done anywhere. Beware: there's also no checking attributes (to see if your `inputMap` actually corresponds to inputs).
+
+The structure of a workflow is m
+
+```python
+w = wdlgen.Workflow("workflow_name")
+
+w.imports.append(wdlgen.Workflow.WorkflowImport("tool_file", ""))
+w.inputs.append(
+    wdlgen.Input(
+        wdlgen.WdlType.parse("String"), 
+        "inputGreeting"
+    )
+)
+
+
+inputs_map = {"taskGreeting": "inputGreeting"}
+w.calls.append(wdlgen.WorkflowCall("Q.namspaced_task_identifier", "task_alias", inputs_map))
+w.outputs.append(wdlgen.Output(wdlgen.WdlType.parse("File"), "standardOut", "task_alias.standardOut")
+```
+
+Which outputs:
+```wdl
+version development
+
+import "tools/tool_file.wdl"
+
+workflow workflow_name {
+  input { 
+    String inputGreeting
+  }
+  call Q.namspaced_task_identifier as task_alias {
+    input:
+      taskGreeting=inputGreeting
+  }
+  output {
+    File standardOut = task_alias.standardOut
+  }
+}
+```
+
+
+## Known limitations
+
+I'm not a fan of the string interpolation generation of WDL that this module does. I think trying to build an [Abstract syntax tree](https://en.wikipedia.org/wiki/Abstract_syntax_tree) and then there should be something that convert that into the DSL that WDL uses.
+
+You could also cause syntax errors in generated WDL by providing illegal characters. 
+
+## Goals
+
+- Improve code-level documentation.
+- Increase the testing coverage + quality of unit tests.
+- Better represent the WDL spec.
+- ~~Find an easier distribution / release method - such as PIP.~~
+- ~~Automate testing and delivery through TravisCI / CircleCI or similar.~~
+- Validate each value by [WDL's language specifications](https://github.com/openwdl/wdl/blob/master/versions/1.0/SPEC.md#language-specification).
+- Add support for structs
+
+### Long goals
+- Write a documentation site.
+- Make classes convert into AST and then into DSL.
+
+## Issues and Pull Requests
+Feel free to log issues and make pull requests. I make no guarantee to the existence or timeliness of replies.
+
+
+Links:
+
+- WDL description: https://github.com/openwdl/wdl/blob/master/versions/1.0/SPEC.md
```

### Comparing `illusional.wdlgen-0.3.0/README.md` & `illusional.wdlgen-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `illusional.wdlgen-0.3.0/setup.py` & `illusional.wdlgen-0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "v0.3.0"
+__version__ = "v0.3.1"
 
 DESCRIPTION = (
     "Contains classes and helpers to generate WDL without worrying about the syntax. "
     "This is primarily intended for generating WDL from other in-memory representations of a workflow."
 )
 
 # ======== SHOULDN'T NEED EDITS BELOW THIS LINE ======== #
@@ -12,17 +12,17 @@
 with open("./README.md") as readme:
     long_description = readme.read()
 
 setup(
     name="illusional.wdlgen",
     version=__version__,
     description=DESCRIPTION,
-    url="https://github.com/illusional/python-wdlgen",
-    author="Michael Franklin",
-    author_email="michael.franklin@petermac.org",
+    url="https://github.com/PMCC-BioinformaticsCore/python-wdlgen",
+    author="Richard Lupat",
+    author_email="richard.lupat@petermac.org",
     license="GNU",
     packages=["wdlgen"],
     install_requires=[],
     zip_safe=False,
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```


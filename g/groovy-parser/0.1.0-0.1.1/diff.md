# Comparing `tmp/groovy-parser-0.1.0.tar.gz` & `tmp/groovy-parser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jmfernandez/projects/python-groovy-parser/dist/.tmp-tje5pi36/groovy-parser-0.1.0.tar", last modified: Tue Jul  4 11:05:28 2023, max compression
+gzip compressed data, was "/home/jmfernandez/projects/python-groovy-parser/dist/.tmp-4gw62z4w/groovy-parser-0.1.1.tar", last modified: Wed Jul 12 18:14:53 2023, max compression
```

## Comparing `groovy-parser-0.1.0.tar` & `groovy-parser-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2023-07-04 11:05:28.000000 groovy-parser-0.1.0/
--rw-r--r--   0 jmfernandez (10012) users      (100)    11357 2023-05-30 00:53:46.000000 groovy-parser-0.1.0/LICENSE
--rw-r--r--   0 jmfernandez (10012) users      (100)     3132 2023-07-04 11:05:28.000000 groovy-parser-0.1.0/PKG-INFO
--rw-r--r--   0 jmfernandez (10012) users      (100)     2471 2023-07-04 10:57:26.000000 groovy-parser-0.1.0/README.md
-drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2023-07-04 11:05:28.000000 groovy-parser-0.1.0/groovy_parser/
-drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2023-07-04 11:05:28.000000 groovy-parser-0.1.0/groovy_parser/GROOVY_3_0_X/
--rw-r--r--   0 jmfernandez (10012) users      (100)    23140 2023-07-02 23:48:42.000000 groovy-parser-0.1.0/groovy_parser/GROOVY_3_0_X/master_groovy_parser.g
--rw-r--r--   0 jmfernandez (10012) users      (100)      944 2023-07-04 10:07:30.000000 groovy-parser-0.1.0/groovy_parser/__init__.py
--rw-r--r--   0 jmfernandez (10012) users      (100)    14988 2023-07-04 10:11:58.000000 groovy-parser-0.1.0/groovy_parser/lexer.py
--rw-r--r--   0 jmfernandez (10012) users      (100)     5005 2023-07-04 10:15:11.000000 groovy-parser-0.1.0/groovy_parser/parser.py
--rw-r--r--   0 jmfernandez (10012) users      (100)        0 2023-07-03 15:08:06.000000 groovy-parser-0.1.0/groovy_parser/py.typed
--rw-r--r--   0 jmfernandez (10012) users      (100)     9801 2023-07-04 10:08:35.000000 groovy-parser-0.1.0/groovy_parser/tokenizer.py
-drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2023-07-04 11:05:28.000000 groovy-parser-0.1.0/groovy_parser.egg-info/
--rw-r--r--   0 jmfernandez (10012) users      (100)     3132 2023-07-04 11:05:28.000000 groovy-parser-0.1.0/groovy_parser.egg-info/PKG-INFO
--rw-r--r--   0 jmfernandez (10012) users      (100)      412 2023-07-04 11:05:28.000000 groovy-parser-0.1.0/groovy_parser.egg-info/SOURCES.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)        1 2023-07-04 11:05:28.000000 groovy-parser-0.1.0/groovy_parser.egg-info/dependency_links.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)       14 2023-07-04 11:05:28.000000 groovy-parser-0.1.0/groovy_parser.egg-info/requires.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)       14 2023-07-04 11:05:28.000000 groovy-parser-0.1.0/groovy_parser.egg-info/top_level.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)       38 2023-07-04 11:05:28.000000 groovy-parser-0.1.0/setup.cfg
--rw-r--r--   0 jmfernandez (10012) users      (100)     2690 2023-07-04 10:53:23.000000 groovy-parser-0.1.0/setup.py
--rw-r--r--   0 jmfernandez (10012) users      (100)    13303 2023-07-04 10:16:22.000000 groovy-parser-0.1.0/translated-groovy3-parser.py
+drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2023-07-12 18:14:53.000000 groovy-parser-0.1.1/
+-rw-r--r--   0 jmfernandez (10012) users      (100)    11357 2023-05-30 00:53:46.000000 groovy-parser-0.1.1/LICENSE
+-rw-r--r--   0 jmfernandez (10012) users      (100)       59 2023-07-12 16:41:17.000000 groovy-parser-0.1.1/MANIFEST.in
+-rw-r--r--   0 jmfernandez (10012) users      (100)     3831 2023-07-12 18:14:53.000000 groovy-parser-0.1.1/PKG-INFO
+-rw-r--r--   0 jmfernandez (10012) users      (100)     3170 2023-07-12 18:12:25.000000 groovy-parser-0.1.1/README.md
+-rw-r--r--   0 jmfernandez (10012) users      (100)    13380 2023-07-12 18:13:11.000000 groovy-parser-0.1.1/cached-translated-groovy3-parser.py
+drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2023-07-12 18:14:53.000000 groovy-parser-0.1.1/groovy_parser/
+drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2023-07-12 18:14:53.000000 groovy-parser-0.1.1/groovy_parser/GROOVY_3_0_X/
+-rw-r--r--   0 jmfernandez (10012) users      (100)    23140 2023-07-02 23:48:42.000000 groovy-parser-0.1.1/groovy_parser/GROOVY_3_0_X/master_groovy_parser.g
+-rw-r--r--   0 jmfernandez (10012) users      (100)      944 2023-07-12 18:06:16.000000 groovy-parser-0.1.1/groovy_parser/__init__.py
+-rw-r--r--   0 jmfernandez (10012) users      (100)    14988 2023-07-04 10:11:58.000000 groovy-parser-0.1.1/groovy_parser/lexer.py
+-rw-r--r--   0 jmfernandez (10012) users      (100)     7677 2023-07-12 18:05:58.000000 groovy-parser-0.1.1/groovy_parser/parser.py
+-rw-r--r--   0 jmfernandez (10012) users      (100)        0 2023-07-03 15:08:06.000000 groovy-parser-0.1.1/groovy_parser/py.typed
+-rw-r--r--   0 jmfernandez (10012) users      (100)     9801 2023-07-04 10:08:35.000000 groovy-parser-0.1.1/groovy_parser/tokenizer.py
+drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2023-07-12 18:14:53.000000 groovy-parser-0.1.1/groovy_parser.egg-info/
+-rw-r--r--   0 jmfernandez (10012) users      (100)     3831 2023-07-12 18:14:53.000000 groovy-parser-0.1.1/groovy_parser.egg-info/PKG-INFO
+-rw-r--r--   0 jmfernandez (10012) users      (100)      492 2023-07-12 18:14:53.000000 groovy-parser-0.1.1/groovy_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)        1 2023-07-12 18:14:53.000000 groovy-parser-0.1.1/groovy_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)       14 2023-07-12 18:14:53.000000 groovy-parser-0.1.1/groovy_parser.egg-info/requires.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)       14 2023-07-12 18:14:53.000000 groovy-parser-0.1.1/groovy_parser.egg-info/top_level.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)      408 2023-07-12 16:35:31.000000 groovy-parser-0.1.1/pyproject.toml
+-rw-r--r--   0 jmfernandez (10012) users      (100)       14 2023-05-30 00:54:58.000000 groovy-parser-0.1.1/requirements.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)       38 2023-07-12 18:14:53.000000 groovy-parser-0.1.1/setup.cfg
+-rw-r--r--   0 jmfernandez (10012) users      (100)     2796 2023-07-12 18:06:07.000000 groovy-parser-0.1.1/setup.py
+-rw-r--r--   0 jmfernandez (10012) users      (100)    13303 2023-07-04 10:16:22.000000 groovy-parser-0.1.1/translated-groovy3-parser.py
```

### Comparing `groovy-parser-0.1.0/LICENSE` & `groovy-parser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `groovy-parser-0.1.0/PKG-INFO` & `groovy-parser-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: groovy-parser
-Version: 0.1.0
-Summary: Groovy 3.0.x parser based on Pygments and Lark
-Home-page: https://github.com/inab/python-groovy-parser
-Author: José M. Fernández <https://orcid.org/0000-0002-4806-5140>
-Author-email: jose.m.fernandez@bsc.es
-License: Apache-2.0
-Project-URL: Bug Tracker, https://github.com/inab/python-groovy-parser/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # python-groovy-parser
 
 Python package which implements a Groovy 3.0.X parser, using both Pygments, Lark and the corresponding grammar.
 
 The tokenizer, lexer and grammar have being tested, stressed and fine tuned
 to be able to properly parse both Nextflow (i.e. `*.nf`), `nextflow.config`-like files
 and real Groovy code from:
@@ -33,20 +16,22 @@
 ## Install
 You can install the development version of this package through pip just running:
 
 ```bash
 pip install git+https://github.com/inab/python-groovy-parser.git
 ```
 
-## Test program
+## Test programs
 
-This repo contains a test program called [translated-groovy3-parser.py](translated-groovy3-parser.py),
-which demonstrates how to use the parser and digest it a bit.
+This repo contains a couple of test programs called
+[translated-groovy3-parser.py](translated-groovy3-parser.py) and
+[cached-translated-groovy3-parser.py](cached-translated-groovy3-parser.py),
+which demonstrate how to use the parser and digest it a bit.
 
-The program takes one or more files as input.
+The programs take one or more files as input.
 
 ```bash
 git pull https://github.com/nf-core/rnaseq.git
 translated-groovy3-parser.py $(find rnaseq -type f -name "*.nf")
 ```
 
 If an input file is for instance `rnaseq/modules/local/bedtools_genomecov.nf`,
@@ -57,14 +42,27 @@
 the parse tree into a file with extension `.lark.json` (for instance,
 `rnaseq/modules/local/bedtools_genomecov.nf.lark.json`).
 
 And as a proof of concept, it tries to identify features from Nextflow files,
 like the declared processes, includes and workflows, and they are roughly printed
 at a file with extension `.lark.result` (for instance `rnaseq/modules/local/bedtools_genomecov.nf.lark.result`).
 
+As parsing task is heavy, the parsing module also contains a method to
+be able to cache the parsed tree in JSON format in a persistent store,
+like a filesystem. So, next operation would be expensive the first time,
+but not the next ones:
+
+```bash
+GROOVY_CACHEDIR=/tmp/somecachedir cached-translated-groovy3-parser.py $(find rnaseq -type f -name "*.nf")
+```
+
+The caching directory contents depend on the grammar and the implementations, as well as versions of the dependencies.
+So, if this software is updated (due grammar is updated or a bug is fixed),
+cached contents from previous versions are not reused.
+
 # Acknowledgements
 
 The tokenizer is an evolution from Pygments Groovy lexer https://github.com/pygments/pygments/blob/b7c8f35440f591c6687cb912aa223f5cf37b6704/pygments/lexers/jvm.py#L543-L618
 
 The Lark grammar has been created from https://github.com/apache/groovy/blob/3b6909a3dbb574e66f5d0fb6aafb6e28316033a8/src/antlr/GroovyParser.g4 ,
 converting it to EBNF using https://bottlecaps.de/convert/ ,
 translating the EBNF representation to Lark format partially by hand.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `groovy-parser-0.1.0/groovy_parser/GROOVY_3_0_X/master_groovy_parser.g` & `groovy-parser-0.1.1/groovy_parser/GROOVY_3_0_X/master_groovy_parser.g`

 * *Files identical despite different names*

### Comparing `groovy-parser-0.1.0/groovy_parser/__init__.py` & `groovy-parser-0.1.1/groovy_parser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # limitations under the License.
 
 __author__ = "José M. Fernández <https://orcid.org/0000-0002-4806-5140>"
 __copyright__ = "© 2023 Barcelona Supercomputing Center (BSC), ES"
 __license__ = "Apache-2.0"
 
 # https://www.python.org/dev/peps/pep-0396/
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

### Comparing `groovy-parser-0.1.0/groovy_parser/lexer.py` & `groovy-parser-0.1.1/groovy_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `groovy-parser-0.1.0/groovy_parser/tokenizer.py` & `groovy-parser-0.1.1/groovy_parser/tokenizer.py`

 * *Files identical despite different names*

### Comparing `groovy-parser-0.1.0/groovy_parser.egg-info/PKG-INFO` & `groovy-parser-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groovy-parser
-Version: 0.1.0
+Version: 0.1.1
 Summary: Groovy 3.0.x parser based on Pygments and Lark
 Home-page: https://github.com/inab/python-groovy-parser
 Author: José M. Fernández <https://orcid.org/0000-0002-4806-5140>
 Author-email: jose.m.fernandez@bsc.es
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/inab/python-groovy-parser/issues
 Classifier: Programming Language :: Python :: 3
@@ -33,20 +33,22 @@
 ## Install
 You can install the development version of this package through pip just running:
 
 ```bash
 pip install git+https://github.com/inab/python-groovy-parser.git
 ```
 
-## Test program
+## Test programs
 
-This repo contains a test program called [translated-groovy3-parser.py](translated-groovy3-parser.py),
-which demonstrates how to use the parser and digest it a bit.
+This repo contains a couple of test programs called
+[translated-groovy3-parser.py](translated-groovy3-parser.py) and
+[cached-translated-groovy3-parser.py](cached-translated-groovy3-parser.py),
+which demonstrate how to use the parser and digest it a bit.
 
-The program takes one or more files as input.
+The programs take one or more files as input.
 
 ```bash
 git pull https://github.com/nf-core/rnaseq.git
 translated-groovy3-parser.py $(find rnaseq -type f -name "*.nf")
 ```
 
 If an input file is for instance `rnaseq/modules/local/bedtools_genomecov.nf`,
@@ -57,14 +59,27 @@
 the parse tree into a file with extension `.lark.json` (for instance,
 `rnaseq/modules/local/bedtools_genomecov.nf.lark.json`).
 
 And as a proof of concept, it tries to identify features from Nextflow files,
 like the declared processes, includes and workflows, and they are roughly printed
 at a file with extension `.lark.result` (for instance `rnaseq/modules/local/bedtools_genomecov.nf.lark.result`).
 
+As parsing task is heavy, the parsing module also contains a method to
+be able to cache the parsed tree in JSON format in a persistent store,
+like a filesystem. So, next operation would be expensive the first time,
+but not the next ones:
+
+```bash
+GROOVY_CACHEDIR=/tmp/somecachedir cached-translated-groovy3-parser.py $(find rnaseq -type f -name "*.nf")
+```
+
+The caching directory contents depend on the grammar and the implementations, as well as versions of the dependencies.
+So, if this software is updated (due grammar is updated or a bug is fixed),
+cached contents from previous versions are not reused.
+
 # Acknowledgements
 
 The tokenizer is an evolution from Pygments Groovy lexer https://github.com/pygments/pygments/blob/b7c8f35440f591c6687cb912aa223f5cf37b6704/pygments/lexers/jvm.py#L543-L618
 
 The Lark grammar has been created from https://github.com/apache/groovy/blob/3b6909a3dbb574e66f5d0fb6aafb6e28316033a8/src/antlr/GroovyParser.g4 ,
 converting it to EBNF using https://bottlecaps.de/convert/ ,
 translating the EBNF representation to Lark format partially by hand.
```

### Comparing `groovy-parser-0.1.0/setup.py` & `groovy-parser-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,17 +37,18 @@
 with open(readme_path, "r") as fh:
     long_description = fh.read()
 
 # Populating the install requirements
 requirements = []
 requirements_path = os.path.join(setupDir, "requirements.txt")
 if os.path.exists(requirements_path):
-    with open(requirements_path) as f:
+    with open(requirements_path, mode="r", encoding="utf-8") as f:
         egg = re.compile(r"#[^#]*egg=([^=&]+)")
         for line in f.read().splitlines():
+            print(f"R {line}")
             m = egg.search(line)
             requirements.append(line if m is None else m.group(1))
 
 setuptools.setup(
     name="groovy-parser",
     version=gp_version,
     author=gp_author,
@@ -62,14 +63,15 @@
     package_data={
         "groovy_parser": [
             "py.typed",
             "GROOVY_3_0_X/master_groovy_parser.g",
         ]
     },
     scripts=[
+        "cached-translated-groovy3-parser.py",
         "translated-groovy3-parser.py",
     ],
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `groovy-parser-0.1.0/translated-groovy3-parser.py` & `groovy-parser-0.1.1/translated-groovy3-parser.py`

 * *Files identical despite different names*


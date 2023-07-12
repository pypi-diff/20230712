# Comparing `tmp/devopstrabalhofinal-0.0.2.tar.gz` & `tmp/devopstrabalhofinal-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopstrabalhofinal-0.0.2.tar", last modified: Wed Jul 12 03:42:45 2023, max compression
+gzip compressed data, was "devopstrabalhofinal-0.0.3.tar", last modified: Wed Jul 12 03:53:38 2023, max compression
```

## Comparing `devopstrabalhofinal-0.0.2.tar` & `devopstrabalhofinal-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 03:42:45.076737 devopstrabalhofinal-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-07-12 00:25:49.000000 devopstrabalhofinal-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      879 2023-07-12 03:42:45.074738 devopstrabalhofinal-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-07-12 01:08:47.000000 devopstrabalhofinal-0.0.2/README.md
--rw-rw-rw-   0        0        0      938 2023-07-12 03:25:20.000000 devopstrabalhofinal-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       56 2023-06-29 21:54:22.000000 devopstrabalhofinal-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 03:42:45.077737 devopstrabalhofinal-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-12 03:42:44.893738 devopstrabalhofinal-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 03:42:44.995734 devopstrabalhofinal-0.0.2/src/codigo/
--rw-rw-rw-   0        0        0        0 2023-06-29 21:54:22.000000 devopstrabalhofinal-0.0.2/src/codigo/__init__.py
--rw-rw-rw-   0        0        0       53 2023-07-12 02:13:13.000000 devopstrabalhofinal-0.0.2/src/codigo/comando.py
-drwxrwxrwx   0        0        0        0 2023-07-12 03:42:45.052746 devopstrabalhofinal-0.0.2/src/devopstrabalhofinal.egg-info/
--rw-rw-rw-   0        0        0      879 2023-07-12 03:42:44.000000 devopstrabalhofinal-0.0.2/src/devopstrabalhofinal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-07-12 03:42:44.000000 devopstrabalhofinal-0.0.2/src/devopstrabalhofinal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 03:42:44.000000 devopstrabalhofinal-0.0.2/src/devopstrabalhofinal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-12 03:42:44.000000 devopstrabalhofinal-0.0.2/src/devopstrabalhofinal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 03:42:44.000000 devopstrabalhofinal-0.0.2/src/devopstrabalhofinal.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-12 03:42:45.060739 devopstrabalhofinal-0.0.2/test/
--rw-rw-rw-   0        0        0       86 2023-07-12 02:22:34.000000 devopstrabalhofinal-0.0.2/test/test_saudacao.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:53:38.256073 devopstrabalhofinal-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 03:53:28.000000 devopstrabalhofinal-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-12 03:53:38.256073 devopstrabalhofinal-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 03:53:28.000000 devopstrabalhofinal-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-12 03:53:28.000000 devopstrabalhofinal-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-12 03:53:28.000000 devopstrabalhofinal-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 03:53:38.256073 devopstrabalhofinal-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:53:38.256073 devopstrabalhofinal-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:53:38.256073 devopstrabalhofinal-0.0.3/src/codigo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 03:53:28.000000 devopstrabalhofinal-0.0.3/src/codigo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 03:53:28.000000 devopstrabalhofinal-0.0.3/src/codigo/comando.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:53:38.256073 devopstrabalhofinal-0.0.3/src/devopstrabalhofinal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-12 03:53:38.000000 devopstrabalhofinal-0.0.3/src/devopstrabalhofinal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-12 03:53:38.000000 devopstrabalhofinal-0.0.3/src/devopstrabalhofinal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:53:38.000000 devopstrabalhofinal-0.0.3/src/devopstrabalhofinal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-12 03:53:38.000000 devopstrabalhofinal-0.0.3/src/devopstrabalhofinal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 03:53:38.000000 devopstrabalhofinal-0.0.3/src/devopstrabalhofinal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:53:38.256073 devopstrabalhofinal-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-12 03:53:28.000000 devopstrabalhofinal-0.0.3/test/test_saudacao.py
```

### Comparing `devopstrabalhofinal-0.0.2/LICENSE` & `devopstrabalhofinal-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 João Victor
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 João Victor
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `devopstrabalhofinal-0.0.2/PKG-INFO` & `devopstrabalhofinal-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: devopstrabalhofinal
-Version: 0.0.2
-Summary: Código de Comando: Saudação
-Author-email: João Victor Milagres Guimarães <1398500@sga.pucminas.br>, Allan da Silveira e Silva <1405224@sga.pucminas.br>, Felipe Ferreira Alexandre <1386198@sga.pucminas.br>, Gabriel Murta Pimentagit <1286408@sga.pucminas.br>
-Project-URL: Homepage, https://github.com/jvmg96/devops_trabalho
-Project-URL: Bug Tracker, https://github.com/jvmg96/devops_trabalho/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Trabalho Final - DevOps
-
-## Grupo:
-João Victor Milgres Guimarães
-
-Allan da Silveira e Silva
-
-Felipe Ferreira Alexandre
-
-Gabriel Murta Pimentagit
+Metadata-Version: 2.1
+Name: devopstrabalhofinal
+Version: 0.0.3
+Summary: Código de Comando: Saudação
+Author-email: João Victor Milagres Guimarães <1398500@sga.pucminas.br>, Allan da Silveira e Silva <1405224@sga.pucminas.br>, Felipe Ferreira Alexandre <1386198@sga.pucminas.br>, Gabriel Murta Pimentagit <1286408@sga.pucminas.br>
+Project-URL: Homepage, https://github.com/jvmg96/devops_trabalho
+Project-URL: Bug Tracker, https://github.com/jvmg96/devops_trabalho/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Trabalho Final - DevOps
+
+## Grupo:
+João Victor Milgres Guimarães
+
+Allan da Silveira e Silva
+
+Felipe Ferreira Alexandre
+
+Gabriel Murta Pimentagit
```

### Comparing `devopstrabalhofinal-0.0.2/pyproject.toml` & `devopstrabalhofinal-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "devopstrabalhofinal"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="João Victor Milagres Guimarães", email="1398500@sga.pucminas.br" },
   { name="Allan da Silveira e Silva", email="1405224@sga.pucminas.br" },
   { name="Felipe Ferreira Alexandre", email="1386198@sga.pucminas.br" },
   { name="Gabriel Murta Pimentagit", email="1286408@sga.pucminas.br" },
 ]
 description = "Código de Comando: Saudação"
```

### Comparing `devopstrabalhofinal-0.0.2/src/devopstrabalhofinal.egg-info/PKG-INFO` & `devopstrabalhofinal-0.0.3/src/devopstrabalhofinal.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: devopstrabalhofinal
-Version: 0.0.2
-Summary: Código de Comando: Saudação
-Author-email: João Victor Milagres Guimarães <1398500@sga.pucminas.br>, Allan da Silveira e Silva <1405224@sga.pucminas.br>, Felipe Ferreira Alexandre <1386198@sga.pucminas.br>, Gabriel Murta Pimentagit <1286408@sga.pucminas.br>
-Project-URL: Homepage, https://github.com/jvmg96/devops_trabalho
-Project-URL: Bug Tracker, https://github.com/jvmg96/devops_trabalho/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Trabalho Final - DevOps
-
-## Grupo:
-João Victor Milgres Guimarães
-
-Allan da Silveira e Silva
-
-Felipe Ferreira Alexandre
-
-Gabriel Murta Pimentagit
+Metadata-Version: 2.1
+Name: devopstrabalhofinal
+Version: 0.0.3
+Summary: Código de Comando: Saudação
+Author-email: João Victor Milagres Guimarães <1398500@sga.pucminas.br>, Allan da Silveira e Silva <1405224@sga.pucminas.br>, Felipe Ferreira Alexandre <1386198@sga.pucminas.br>, Gabriel Murta Pimentagit <1286408@sga.pucminas.br>
+Project-URL: Homepage, https://github.com/jvmg96/devops_trabalho
+Project-URL: Bug Tracker, https://github.com/jvmg96/devops_trabalho/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Trabalho Final - DevOps
+
+## Grupo:
+João Victor Milgres Guimarães
+
+Allan da Silveira e Silva
+
+Felipe Ferreira Alexandre
+
+Gabriel Murta Pimentagit
```

